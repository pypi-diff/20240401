# Comparing `tmp/azureml_acft_image_components-0.0.9-py3-none-any.whl.zip` & `tmp/azureml_acft_image_components-47.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,95 +1,117 @@
-Zip file size: 178143 bytes, number of entries: 93
--rw-rw-rw-  2.0 fat      251 b- defN 23-May-17 17:31 azureml/__init__.py
--rw-rw-rw-  2.0 fat      295 b- defN 23-May-17 17:31 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat      822 b- defN 23-May-17 17:31 azureml/acft/image/__init__.py
--rw-rw-rw-  2.0 fat   600282 b- defN 23-May-17 17:31 azureml/acft/image/components/NOTICE.txt
--rw-rw-rw-  2.0 fat      498 b- defN 23-May-17 17:31 azureml/acft/image/components/__init__.py
--rw-rw-rw-  2.0 fat       34 b- defN 23-May-17 17:36 azureml/acft/image/components/_version.py
--rw-rw-rw-  2.0 fat      312 b- defN 23-May-17 17:31 azureml/acft/image/components/common/__init__.py
--rw-rw-rw-  2.0 fat      583 b- defN 23-May-17 17:31 azureml/acft/image/components/common/utils.py
--rw-rw-rw-  2.0 fat      320 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/__init__.py
--rw-rw-rw-  2.0 fat     7753 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/finetune_runner.py
--rw-rw-rw-  2.0 fat      464 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/__init__.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/utils.py
--rw-rw-rw-  2.0 fat      313 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/__init__.py
--rw-rw-rw-  2.0 fat     6267 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
--rw-rw-rw-  2.0 fat    14648 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
--rw-rw-rw-  2.0 fat    27652 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
--rw-rw-rw-  2.0 fat      320 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
--rw-rw-rw-  2.0 fat     1929 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
--rw-rw-rw-  2.0 fat     2580 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
--rw-rw-rw-  2.0 fat     1314 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml
--rw-rw-rw-  2.0 fat      309 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/constants/__init__.py
--rw-rw-rw-  2.0 fat     1550 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
--rw-rw-rw-  2.0 fat     4628 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/constants/constants.py
--rw-rw-rw-  2.0 fat      304 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/__init__.py
--rw-rw-rw-  2.0 fat     5216 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/base_dataset.py
--rw-rw-rw-  2.0 fat     9513 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/classification_dataset.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
--rw-rw-rw-  2.0 fat    10779 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/download_manager.py
--rw-rw-rw-  2.0 fat    10729 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py
--rw-rw-rw-  2.0 fat     7557 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
--rw-rw-rw-  2.0 fat      338 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/__init__.py
--rw-rw-rw-  2.0 fat     8813 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/common_constants.py
--rw-rw-rw-  2.0 fat     2546 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/common_utils.py
--rw-rw-rw-  2.0 fat    10883 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py
--rw-rw-rw-  2.0 fat     6194 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
--rw-rw-rw-  2.0 fat     3222 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
--rw-rw-rw-  2.0 fat     3677 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/masktools.py
--rw-rw-rw-  2.0 fat     6780 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py
--rw-rw-rw-  2.0 fat      170 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt
--rw-rw-rw-  2.0 fat      125 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt
--rw-rw-rw-  2.0 fat     6549 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
--rw-rw-rw-  2.0 fat    10790 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
--rw-rw-rw-  2.0 fat     7009 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
--rw-rw-rw-  2.0 fat      329 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/__init__.py
--rw-rw-rw-  2.0 fat     3091 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/classification_models_defaults.py
--rw-rw-rw-  2.0 fat     3507 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/constants.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
--rw-rw-rw-  2.0 fat      823 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
--rw-rw-rw-  2.0 fat      808 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
--rw-rw-rw-  2.0 fat     2021 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/task_defaults.py
--rw-rw-rw-  2.0 fat     7761 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/defaults/training_defaults.py
--rw-rw-rw-  2.0 fat      333 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/factory/__init__.py
--rw-rw-rw-  2.0 fat      764 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/factory/mappings.py
--rw-rw-rw-  2.0 fat     2253 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/factory/model_factory.py
--rw-rw-rw-  2.0 fat      548 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/factory/task_definitions.py
--rw-rw-rw-  2.0 fat     5944 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/__init__.py
--rw-rw-rw-  2.0 fat      347 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/classification/__init__.py
--rw-rw-rw-  2.0 fat     7964 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/classification/data_cls.py
--rw-rw-rw-  2.0 fat     2367 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py
--rw-rw-rw-  2.0 fat     5178 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py
--rw-rw-rw-  2.0 fat     1706 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py
--rw-rw-rw-  2.0 fat      339 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/common/__init__.py
--rw-rw-rw-  2.0 fat      951 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/common/constants.py
--rw-rw-rw-  2.0 fat    18943 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py
--rw-rw-rw-  2.0 fat      350 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py
--rw-rw-rw-  2.0 fat     8760 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py
--rw-rw-rw-  2.0 fat      265 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/interfaces/__init__.py
--rw-rw-rw-  2.0 fat    10706 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/interfaces/azml_interface.py
--rw-rw-rw-  2.0 fat     2327 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/__init__.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/__init__.py
--rw-rw-rw-  2.0 fat      759 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/constants.py
--rw-rw-rw-  2.0 fat    10253 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/data_class.py
--rw-rw-rw-  2.0 fat     8739 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/dataset.py
--rw-rw-rw-  2.0 fat     1083 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py
--rw-rw-rw-  2.0 fat     3015 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/inference.py
--rw-rw-rw-  2.0 fat    10152 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/metrics.py
--rw-rw-rw-  2.0 fat     7374 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/model.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
--rw-rw-rw-  2.0 fat     1784 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
--rw-rw-rw-  2.0 fat      264 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
--rw-rw-rw-  2.0 fat     7724 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py
--rw-rw-rw-  2.0 fat      259 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
--rw-rw-rw-  2.0 fat    11273 b- defN 23-May-17 17:31 azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
--rw-rw-rw-  2.0 fat      321 b- defN 23-May-17 17:31 azureml/acft/image/components/model_selector/__init__.py
--rw-rw-rw-  2.0 fat    17200 b- defN 23-May-17 17:31 azureml/acft/image/components/model_selector/component.py
--rw-rw-rw-  2.0 fat      851 b- defN 23-May-17 17:31 azureml/acft/image/components/model_selector/constants.py
--rw-rw-rw-  2.0 fat      859 b- defN 23-May-17 17:36 azureml_acft_image_components-0.0.9.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1315 b- defN 23-May-17 17:36 azureml_acft_image_components-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-17 17:36 azureml_acft_image_components-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 17:36 azureml_acft_image_components-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    11579 b- defN 23-May-17 17:36 azureml_acft_image_components-0.0.9.dist-info/RECORD
-93 files, 983954 bytes uncompressed, 158337 bytes compressed:  83.9%
+Zip file size: 235232 bytes, number of entries: 115
+-rw-rw-rw-  2.0 fat      251 b- defN 24-Mar-22 10:04 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      295 b- defN 24-Mar-22 10:04 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat      822 b- defN 24-Mar-22 10:04 azureml/acft/image/__init__.py
+-rw-rw-rw-  2.0 fat   552837 b- defN 24-Mar-22 10:04 azureml/acft/image/components/NOTICE.txt
+-rw-rw-rw-  2.0 fat      498 b- defN 24-Mar-22 10:04 azureml/acft/image/components/__init__.py
+-rw-rw-rw-  2.0 fat       36 b- defN 24-Mar-22 10:09 azureml/acft/image/components/_version.py
+-rw-rw-rw-  2.0 fat      312 b- defN 24-Mar-22 10:04 azureml/acft/image/components/common/__init__.py
+-rw-rw-rw-  2.0 fat     1656 b- defN 24-Mar-22 10:04 azureml/acft/image/components/common/constants.py
+-rw-rw-rw-  2.0 fat     1712 b- defN 24-Mar-22 10:04 azureml/acft/image/components/common/utils.py
+-rw-rw-rw-  2.0 fat     3810 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    13407 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/finetune_runner.py
+-rw-rw-rw-  2.0 fat      464 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/__init__.py
+-rw-rw-rw-  2.0 fat      313 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/__init__.py
+-rw-rw-rw-  2.0 fat     6267 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
+-rw-rw-rw-  2.0 fat    14648 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
+-rw-rw-rw-  2.0 fat    29218 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
+-rw-rw-rw-  2.0 fat     5379 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/openmmlab_augmentation.py
+-rw-rw-rw-  2.0 fat      320 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
+-rw-rw-rw-  2.0 fat     2035 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
+-rw-rw-rw-  2.0 fat     2784 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
+-rw-rw-rw-  2.0 fat      309 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/constants/__init__.py
+-rw-rw-rw-  2.0 fat     1859 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
+-rw-rw-rw-  2.0 fat     5014 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/constants/constants.py
+-rw-rw-rw-  2.0 fat      304 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/__init__.py
+-rw-rw-rw-  2.0 fat     5216 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/base_dataset.py
+-rw-rw-rw-  2.0 fat     9513 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/classification_dataset.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
+-rw-rw-rw-  2.0 fat     7240 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/data_utils.py
+-rw-rw-rw-  2.0 fat    10779 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/download_manager.py
+-rw-rw-rw-  2.0 fat    11053 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py
+-rw-rw-rw-  2.0 fat     7557 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
+-rw-rw-rw-  2.0 fat      338 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat     8813 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py
+-rw-rw-rw-  2.0 fat     5099 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/common_constants.py
+-rw-rw-rw-  2.0 fat     4537 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/common_utils.py
+-rw-rw-rw-  2.0 fat    16659 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py
+-rw-rw-rw-  2.0 fat     5143 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/custom_augmentations_openmm.py
+-rw-rw-rw-  2.0 fat     4076 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/masktools.py
+-rw-rw-rw-  2.0 fat    12582 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py
+-rw-rw-rw-  2.0 fat      234 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt
+-rw-rw-rw-  2.0 fat      188 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt
+-rw-rw-rw-  2.0 fat     7876 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
+-rw-rw-rw-  2.0 fat    13526 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
+-rw-rw-rw-  2.0 fat    12062 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
+-rw-rw-rw-  2.0 fat      444 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmtrack-mot-conda.yaml
+-rw-rw-rw-  2.0 fat     6619 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmtrack_mlflow_model_wrapper.py
+-rw-rw-rw-  2.0 fat     5253 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmtrack_module.py
+-rw-rw-rw-  2.0 fat     5985 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/mlflow/mmtrack_utils.py
+-rw-rw-rw-  2.0 fat      307 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/trainer/__init__.py
+-rw-rw-rw-  2.0 fat     6883 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/common/trainer/train_helper.py
+-rw-rw-rw-  2.0 fat      329 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/__init__.py
+-rw-rw-rw-  2.0 fat     5195 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/constants.py
+-rw-rw-rw-  2.0 fat     1163 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
+-rw-rw-rw-  2.0 fat      756 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
+-rw-rw-rw-  2.0 fat      750 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/multi_object_tracking_models_defaults.py
+-rw-rw-rw-  2.0 fat     3412 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/multiclass_classification_models_defaults.py
+-rw-rw-rw-  2.0 fat     4006 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/multilabel_classification_models_defaults.py
+-rw-rw-rw-  2.0 fat      741 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
+-rw-rw-rw-  2.0 fat     3879 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/task_defaults.py
+-rw-rw-rw-  2.0 fat     8777 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/defaults/training_defaults.py
+-rw-rw-rw-  2.0 fat      333 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/factory/__init__.py
+-rw-rw-rw-  2.0 fat      903 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/factory/mappings.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/factory/model_factory.py
+-rw-rw-rw-  2.0 fat      610 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/factory/task_definitions.py
+-rw-rw-rw-  2.0 fat     8297 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/__init__.py
+-rw-rw-rw-  2.0 fat      347 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/classification/__init__.py
+-rw-rw-rw-  2.0 fat     8430 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/classification/data_cls.py
+-rw-rw-rw-  2.0 fat     3231 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py
+-rw-rw-rw-  2.0 fat     5178 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py
+-rw-rw-rw-  2.0 fat     1706 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py
+-rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/common/__init__.py
+-rw-rw-rw-  2.0 fat     1004 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/common/constants.py
+-rw-rw-rw-  2.0 fat    17297 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py
+-rw-rw-rw-  2.0 fat      350 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat     8760 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py
+-rw-rw-rw-  2.0 fat      265 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/interfaces/__init__.py
+-rw-rw-rw-  2.0 fat    10706 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/interfaces/azml_interface.py
+-rw-rw-rw-  2.0 fat     7225 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/__init__.py
+-rw-rw-rw-  2.0 fat      249 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/__init__.py
+-rw-rw-rw-  2.0 fat     1059 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/constants.py
+-rw-rw-rw-  2.0 fat     9849 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/data_class.py
+-rw-rw-rw-  2.0 fat    10821 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/dataset.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py
+-rw-rw-rw-  2.0 fat     4146 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/inference.py
+-rw-rw-rw-  2.0 fat     1932 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/metrics.py
+-rw-rw-rw-  2.0 fat    11461 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/model.py
+-rw-rw-rw-  2.0 fat     1888 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/model_config_rules.py
+-rw-rw-rw-  2.0 fat     3131 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
+-rw-rw-rw-  2.0 fat     1863 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
+-rw-rw-rw-  2.0 fat      264 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
+-rw-rw-rw-  2.0 fat     9981 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py
+-rw-rw-rw-  2.0 fat      259 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
+-rw-rw-rw-  2.0 fat    20894 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
+-rw-rw-rw-  2.0 fat     2293 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/__init__.py
+-rw-rw-rw-  2.0 fat      248 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/__init__.py
+-rw-rw-rw-  2.0 fat     1563 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/constants.py
+-rw-rw-rw-  2.0 fat    14240 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/data_class.py
+-rw-rw-rw-  2.0 fat    27756 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/dataset.py
+-rw-rw-rw-  2.0 fat     1082 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/image_metadata.py
+-rw-rw-rw-  2.0 fat     3000 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/inference.py
+-rw-rw-rw-  2.0 fat     1911 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/metrics.py
+-rw-rw-rw-  2.0 fat     7291 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/model.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/trainer_arguments.py
+-rw-rw-rw-  2.0 fat     1767 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/common/trainer_classes.py
+-rw-rw-rw-  2.0 fat      263 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/mot/__init__.py
+-rw-rw-rw-  2.0 fat    18350 b- defN 24-Mar-22 10:04 azureml/acft/image/components/finetune/mmtracking/mot/model_wrapper.py
+-rw-rw-rw-  2.0 fat      321 b- defN 24-Mar-22 10:04 azureml/acft/image/components/model_selector/__init__.py
+-rw-rw-rw-  2.0 fat    27217 b- defN 24-Mar-22 10:04 azureml/acft/image/components/model_selector/component.py
+-rw-rw-rw-  2.0 fat     1289 b- defN 24-Mar-22 10:04 azureml/acft/image/components/model_selector/constants.py
+-rw-rw-rw-  2.0 fat      859 b- defN 24-Mar-22 10:09 azureml_acft_image_components-47.0.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1469 b- defN 24-Mar-22 10:09 azureml_acft_image_components-47.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 10:09 azureml_acft_image_components-47.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-22 10:09 azureml_acft_image_components-47.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    14429 b- defN 24-Mar-22 10:09 azureml_acft_image_components-47.0.0.dist-info/RECORD
+115 files, 1133302 bytes uncompressed, 210572 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -15,29 +15,29 @@
 
 Filename: azureml/acft/image/components/_version.py
 Comment: 
 
 Filename: azureml/acft/image/components/common/__init__.py
 Comment: 
 
+Filename: azureml/acft/image/components/common/constants.py
+Comment: 
+
 Filename: azureml/acft/image/components/common/utils.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/finetune_runner.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/__init__.py
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/common/utils.py
-Comment: 
-
 Filename: azureml/acft/image/components/finetune/common/augmentation/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
@@ -45,26 +45,26 @@
 
 Filename: azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
 Comment: 
 
+Filename: azureml/acft/image/components/finetune/common/augmentation/openmmlab_augmentation.py
+Comment: 
+
 Filename: azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml
-Comment: 
-
 Filename: azureml/acft/image/components/finetune/common/constants/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/constants/constants.py
@@ -78,14 +78,17 @@
 
 Filename: azureml/acft/image/components/finetune/common/data/classification_dataset.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
 Comment: 
 
+Filename: azureml/acft/image/components/finetune/common/data/data_utils.py
+Comment: 
+
 Filename: azureml/acft/image/components/finetune/common/data/download_manager.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
@@ -102,18 +105,15 @@
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/common_utils.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
+Filename: azureml/acft/image/components/finetune/common/mlflow/custom_augmentations_openmm.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/masktools.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py
 Comment: 
@@ -129,29 +129,53 @@
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/defaults/__init__.py
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmtrack-mot-conda.yaml
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmtrack_mlflow_model_wrapper.py
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/defaults/classification_models_defaults.py
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmtrack_module.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmtrack_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/trainer/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/trainer/train_helper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/defaults/constants.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
 Comment: 
 
+Filename: azureml/acft/image/components/finetune/defaults/multi_object_tracking_models_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/multiclass_classification_models_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/multilabel_classification_models_defaults.py
+Comment: 
+
 Filename: azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/defaults/task_defaults.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/defaults/training_defaults.py
@@ -231,14 +255,17 @@
 
 Filename: azureml/acft/image/components/finetune/mmdetection/common/metrics.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/mmdetection/common/model.py
 Comment: 
 
+Filename: azureml/acft/image/components/finetune/mmdetection/common/model_config_rules.py
+Comment: 
+
 Filename: azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
@@ -249,32 +276,71 @@
 
 Filename: azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
 Comment: 
 
+Filename: azureml/acft/image/components/finetune/mmtracking/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/data_class.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/dataset.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/image_metadata.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/inference.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/metrics.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/model.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/trainer_arguments.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/common/trainer_classes.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/mot/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmtracking/mot/model_wrapper.py
+Comment: 
+
 Filename: azureml/acft/image/components/model_selector/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/model_selector/component.py
 Comment: 
 
 Filename: azureml/acft/image/components/model_selector/constants.py
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.9.dist-info/LICENSE.txt
+Filename: azureml_acft_image_components-47.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.9.dist-info/METADATA
+Filename: azureml_acft_image_components-47.0.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.9.dist-info/WHEEL
+Filename: azureml_acft_image_components-47.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.9.dist-info/top_level.txt
+Filename: azureml_acft_image_components-47.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.9.dist-info/RECORD
+Filename: azureml_acft_image_components-47.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/acft/image/components/NOTICE.txt

```diff
@@ -13,230 +13,14 @@
 USA
 
 Notwithstanding any other terms, you may reverse engineer this software to the extent
 required to debug changes to any libraries licensed under the GNU Lesser General Public License.
 
 ---------------------------------------------------------
 
-accelerate 0.11.0 - Apache-2.0
-
-
-Copyright 2021 The HuggingFace Team
-Copyright 2022 The HuggingFace Team
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
-
-limitations under the License.
-
----------------------------------------------------------
-
----------------------------------------------------------
-
-aiohttp 3.8.4 - Apache-2.0
-
-
-Copyright Fedor Indutny, 2018
-copyright f project contributors
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
-
-limitations under the License.
-
----------------------------------------------------------
-
----------------------------------------------------------
-
 aiosignal 1.3.1 - Apache-2.0
 
 
 copyright 2013-2019, aiosignal contributors
 Copyright 2013-2019 Nikolay Kim and Andrew Svetlov
 
 Apache License
@@ -337,17 +121,18 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-argcomplete 2.0.0 - Apache-2.0
+argcomplete 2.1.2 - Apache-2.0
 
 
+Copyright 2012-2021, Andrey Kislyuk and argcomplete contributors
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -550,121 +335,14 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-async-timeout 4.0.2 - Apache-2.0
-
-
-Copyright 2016-2020 aio-libs collaboration
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
-
-limitations under the License.
-
----------------------------------------------------------
-
----------------------------------------------------------
-
 bcrypt 4.0.1 - Apache-2.0
 
 
 Copyright 2013-2022
 Copyright (c) 2013 Donald Stufft
 
 Apache License
@@ -872,129 +550,19 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-dataclasses 0.8 - Apache-2.0
-
-
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
-
-limitations under the License.
-
----------------------------------------------------------
-
----------------------------------------------------------
-
-datasets 2.3.2 - Apache-2.0
+distro 1.8.0 - Apache-2.0
 
 
-Copyright 2020 Optuna, Hugging Face
-Copyright 2020 The HuggingFace Authors
-Copyright 2020 The TensorFlow Datasets
-Copyright 2021 The HuggingFace Authors
-Copyright 2020 The HuggingFace Datasets
-Copyright 2022 The HuggingFace Datasets
+Copyright 2015,2016 Nir Cohen
+Copyright 2015,2016,2017 Nir Cohen
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1090,19 +658,19 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-distro 1.8.0 - Apache-2.0
+frozenlist 1.4.0 - Apache-2.0
 
 
-Copyright 2015,2016 Nir Cohen
-Copyright 2015,2016,2017 Nir Cohen
+copyright 2013-2019, frozenlist contributors
+Copyright 2013-2019 Nikolay Kim and Andrew Svetlov
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1198,18 +766,17 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-docker 5.0.3 - Apache-2.0
+importlib-metadata 5.2.0 - Apache-2.0
 
 
-Copyright 2016 Docker, Inc.
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1305,19 +872,24 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-frozenlist 1.3.3 - Apache-2.0
+mmcls 0.25.0 - Apache-2.0
 
 
-copyright 2013-2019, frozenlist contributors
-Copyright 2013-2019 Nikolay Kim and Andrew Svetlov
+Copyright (c) OpenMMLab
+Copyright 2021 Ross Wightman
+Copyright (c) 2019 cybertronai
+Copyright (c) 2019 Facebook, Inc
+Copyright (c) 2021, Habana Labs Ltd.
+Copyright (c) 2015-present, Facebook, Inc.
+Copyright (c) 2019-2020, NVIDIA CORPORATION.
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1413,17 +985,39 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-importlib-metadata 4.13.0 - Apache-2.0
+mmcv-full 1.7.1 - Apache-2.0
 
 
+Copyright 2019 Yan Yan
+Copyright (c) OpenMMLab
+Copyright (c) Open-MMLab
+Copyright (c) 2018 Microsoft
+Copyright (c) 2020 SenseTime
+Copyright (c) 2021 Cambricon
+Copyright (c) 2022 Cambricon
+Copyright (c) 2019, SenseTime
+Copyright (c) 2022 Apple Inc.
+Copyright 2018-2020 Open-MMLab
+Copyright (c) 2022 by Cambricon
+Copyright (c) Microsoft Corporation
+Copyright (c) 2018 Vladislav Sovrasov
+Copyright Louis Delacroix 2010 - 2014
+Copyright (c) 2019, NVIDIA Corporation
+Copyright (c) 2021, NVIDIA Corporation
+Copyright Huawei Technologies Co., Ltd.
+Copyright (c) 2019-2022 by Cambricon, Inc.
+Copyright (c) 2022 Huawei Technologies Co., Ltd
+Copyright (c) Facebook, Inc. and its affiliates
+Copyright (c) 2014-2017, the respective contributors
+Copyright (c) 2014-2017 The Regents of the University of California (Regents)
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1519,17 +1113,20 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-importlib-metadata 6.0.0 - Apache-2.0
+mmdet 2.28.2 - Apache-2.0
 
 
+Copyright (c) OpenMMLab
+Copyright (c) 2018, Alexander Kirillov
+Copyright (c) 2019 Western Digital Corporation
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1625,39 +1222,22 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-mmcv-full 1.7.1 - Apache-2.0
+mmtrack 0.14.0 - Apache-2.0
 
 
-Copyright 2019 Yan Yan
 Copyright (c) OpenMMLab
 Copyright (c) Open-MMLab
-Copyright (c) 2018 Microsoft
-Copyright (c) 2020 SenseTime
-Copyright (c) 2021 Cambricon
-Copyright (c) 2022 Cambricon
-Copyright (c) 2019, SenseTime
-Copyright (c) 2022 Apple Inc.
-Copyright 2018-2020 Open-MMLab
-Copyright (c) 2022 by Cambricon
-Copyright (c) Microsoft Corporation
-Copyright (c) 2018 Vladislav Sovrasov
-Copyright Louis Delacroix 2010 - 2014
-Copyright (c) 2019, NVIDIA Corporation
-Copyright (c) 2021, NVIDIA Corporation
-Copyright Huawei Technologies Co., Ltd.
-Copyright (c) 2019-2022 by Cambricon, Inc.
-Copyright (c) 2022 Huawei Technologies Co., Ltd
-Copyright (c) Facebook, Inc. and its affiliates
-Copyright (c) 2014-2017, the respective contributors
-Copyright (c) 2014-2017 The Regents of the University of California (Regents)
+Copyright (c) OpenMMLab. Modofied
+Copyright (c) Github URL Copied from https://github.com/youtubevos/cocoapi/blob/master/PythonAPI/pycocotools/ytvos.py
+Copyright (c) Github URL Copied from https://github.com/youtubevos/cocoapi/blob/master/PythonAPI/pycocotools/ytvoseval.py
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -1967,20 +1547,20 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-optimum 1.3.0 - Apache-2.0
+openmim 0.3.9 - Apache-2.0
 
 
-Copyright 2020 Optuna, Hugging Face
-Copyright 2021 The HuggingFace Team
-Copyright 2022 The HuggingFace Team
+Copyright (c) OpenMMLab
+Copyright 2021 OpenMMLab
+Copyright (c) https://github.com/pypa/pip Modified from https://github.com/pypa/pip/blob/main/src/pip/_internal/cli/progress_bars.py
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -2076,15 +1656,15 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyarrow 11.0.0 - Apache-2.0
+pyarrow 9.0.0 - Apache-2.0
 
 
 Copyright 2011 Kitware, Inc.
 Copyright 2012 Cloudera Inc.
 Copyright 2001-2009 Kitware, Inc.
 Copyright 2012 Continuum Analytics, Inc.
 Copyright 2012-2014 Continuum Analytics, Inc.
@@ -2187,22 +1767,41 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyarrow 9.0.0 - Apache-2.0
+pycryptodome 3.18.0 - Apache-2.0
 
 
-Copyright 2011 Kitware, Inc.
-Copyright 2012 Cloudera Inc.
-Copyright 2001-2009 Kitware, Inc.
-Copyright 2012 Continuum Analytics, Inc.
-Copyright 2012-2014 Continuum Analytics, Inc.
+copyright e (c)
+(c) Ban Quan Suo
+(c) Droits d'auteur
+Copyright Dave Gandy 2016
+copyright 2022, Helder Eijs
+(c) Autorioigus (copyright)s
+Copyright (c) 2019 ORGANIZATION
+Copyright 2007-2013 by the Sphinx team
+Copyright (c) 2014, Legrandin <helderijs@gmail.com>
+Copyright (c) 2015, Legrandin <helderijs@gmail.com>
+Copyright (c) 2016, Legrandin <helderijs@gmail.com>
+Copyright (c) 2019, Legrandin <helderijs@gmail.com>
+Copyright (c) 2021, Legrandin <helderijs@gmail.com>
+Copyright (c) 2022, Legrandin <helderijs@gmail.com>
+Copyright (c) 2017, Helder Eijs <helderijs@gmail.com>
+Copyright (c) 2018, Helder Eijs <helderijs@gmail.com>
+Copyright (c) 2019, Helder Eijs <helderijs@gmail.com>
+Copyright (c) 2021, Helder Eijs <helderijs@gmail.com>
+Copyright (c) 2022, Helder Eijs <helderijs@gmail.com>
+Copyright (c) 2001, 2002, 2003 Python Software Foundation
+Copyright (c) 2012-2014 Daniel J. Bernstein <djb@cr.yp.to>
+Copyright (c) 1995-2001 Corporation for National Research Initiatives
+Copyright (c) 2012-2016 Jean-Philippe Aumasson <jeanphilippe.aumasson@gmail.com>
+Copyright (c) 1991 - 1995, Stichting Mathematisch Centrum Amsterdam, The Netherlands
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -2449,15 +2048,15 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyopenssl 23.0.0 - Apache-2.0
+pyopenssl 23.2.0 - Apache-2.0
 
 
 copyright 2001
 Copyright (c) AB
 Copyright 2001-2023
 Copyright (c) Frederick Dean
 Copyright (c) Jean-Paul Calderone
@@ -2676,15 +2275,15 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-regex 2022.10.31 - Apache-2.0
+regex 2023.6.3 - Apache-2.0
 
 
 Copyright 2020 Matthew Barnett
 Copyright (c) 1997-2002 by Secret Labs AB
 copyright (c) 1998-2001 by Secret Labs AB
 Copyright (c) 1997-2001 by Secret Labs AB.
 Copyright (c) 1998-2001 by Secret Labs AB.
@@ -2787,15 +2386,15 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-requests 2.28.2 - Apache-2.0
+requests 2.31.0 - Apache-2.0
 
 
 Copyright Kenneth Reitz
 Copyright 2019 Kenneth Reitz
 copyright (c) 2012 by Kenneth Reitz
 copyright (c) 2017 by Kenneth Reitz
 
@@ -2897,128 +2496,31 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-responses 0.18.0 - Apache-2.0
-
-
-Copyright 2015 David Cramer
-copyright (c) 2015 David Cramer
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
-
-limitations under the License.
-
----------------------------------------------------------
-
----------------------------------------------------------
-
-sentencepiece 0.1.96 - Apache-2.0
+sentencepiece 0.1.99 - Apache-2.0
 
 
+Copyright 2008 Google Inc.
+Copyright 2012 Google Inc.
+Copyright 2014 Google Inc.
+Copyright 2016 Google Inc.
+Copyright 2016 Google LLC.
 Copyright 2018 Google Inc.
 copyright Archive Literary
-(c) (3) educational corporation
+Copyright (c) 2006, Google Inc.
+Copyright (c) 2008-2009 Yuta Mori
+Copyright 2017 The Abseil Authors
+Copyright (c) 2008-2011, Susumu Yata
+Copyright (c) 2010 Daisuke Okanohara
+Copyright 2020 Jan Tojnar https://github.com/jtojnar/cmake-snips
+Copyright (c) 2014, Bogdan Cristea and LTE Engineering Software, Kitware, Inc., Insight Software Consortium
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -3114,15 +2616,15 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-tokenizers 0.13.2 - Apache-2.0
+tokenizers 0.13.3 - Apache-2.0
 
 
 
 Apache License
 
 Version 2.0, January 2004
 
@@ -3220,338 +2722,18 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-transformers 4.25.1 - Apache-2.0
+yarl 1.9.2 - Apache-2.0
 
 
-Copyright 2022
-Copyright 2018 T5
-Copyright 2020 T5
-Copyright 2021 T5
-Copyright 2022 LongT5
-Copyright 2022 Salesforce
-Copyright 2020 Hugging Face
-Copyright 2020, Hugging Face
-Copyright (c) 2020 tanreinama
-Copyright 2022 Meta Platforms
-Copyright 2018 Mesh TensorFlow
-Copyright 2018 The OpenAI Team
-Copyright 2020 Mesh TensorFlow
-Copyright 2021 Mesh TensorFlow
-Copyright 2021 The Marian Team
-Copyright 2021 The OpenAI Team
-Copyright 2022 The OpenAI Team
-Copyright 2022 the Big Science
-Copyright The HuggingFace team
-Copyright 2018 The Open AI Team
-Copyright 2019 The Open AI Team
-Copyright 2021 The OFA-Sys Team
-Copyright 2021 The Open AI Team
-Copyright 2022 The OFA-Sys Team
-Copyright 2022 The Open AI Team
-Copyright 2022 SwitchTransformers
-Copyright 2022 Google LLC., LongT5
-Copyright (c) HuggingFace Inc. team
-Copyright 2018 The Google Flax Team
-Copyright 2020 Optuna, Hugging Face
-Copyright 2020 The HuggingFace Team
-Copyright 2021 The Google Flax Team
-Copyright 2021 The HuggingFace Team
-Copyright 2022 The HuggingFace Team
-Copyright The HuggingFace Inc. team
-Copyright (c) 2001-2020 NLTK Project
-Copyright 2021 AlQuraishi Laboratory
-Copyright 2022 HuggingFace Inc. team
-Copyright 2018, Hao Tan, Mohit Bansal
-Copyright 2018- The Hugging Face team
-Copyright (c) 2018, Alexander Kirillov
-Copyright (c) 2018, NVIDIA CORPORATION.
-Copyright (c) 2020, NVIDIA CORPORATION.
-Copyright (c) 20121, NVIDIA CORPORATION.
-Copyright (c) 2021-, NVIDIA CORPORATION.
-Copyright 2018 The HuggingFace Inc. team
-Copyright 2020 The HuggingFace Inc. team
-Copyright 2021 The HuggingFace Inc. team
-Copyright 2022 The HuggingFace Inc. team
-Copyright 2020, The HuggingFace Inc. team
-Copyright 2018 The Google AI Language Team
-Copyright 2019 The Google AI Language Team
-Copyright 2020 The Google AI Language Team
-Copyright 2022 The Google AI Language Team
-Copyright 2022 The Trajectory Transformers
-Copyright 2022, Google and HuggingFace Inc.
-Copyright (c) 2018-2021, NVIDIA CORPORATION.
-Copyright 2020 The Facebook AI Research Team
-Copyright 2021 DeepMind Technologies Limited
-Copyright 2021 The Facebook AI Research Team
-Copyright 2022 The Facebook AI Research Team
-Copyright 2022 NVIDIA and The HuggingFace Team
-Copyright (c) Facebook, Inc. and its affiliates
-Copyright 2021 NVIDIA The HuggingFace Inc. team
-Copyright 2022 NVIDIA The HuggingFace Inc. team
-Copyright 2020-present the HuggingFace Inc. team
-Copyright 2022 Facebook and The HuggingFace Team
-Copyright Deepmind and The HuggingFace Inc. team
-Copyright 2018 Amazon.com, Inc. or its affiliates
-Copyright 2018 DPR Authors, The Hugging Face Team
-Copyright 2022 Google AI and The HuggingFace Team
-Copyright 2022 Meta and The HuggingFace Inc. team
-Copyright 2022 WeChatAI The HuggingFace Inc. team
-Copyright Google AI and The HuggingFace Inc. team
-Copyright 2010, DPR authors, The Hugging Face Team
-Copyright 2021 Google AI The HuggingFace Inc. team
-Copyright 2022 KAIST and The HuggingFace Inc. team
-Copyright 2018 Salesforce and HuggingFace Inc. team
-Copyright 2020 Google and The HuggingFace Inc. team
-Copyright 2020, The T5 Authors and HuggingFace Inc.
-Copyright 2021 NVIDIA and The HuggingFace Inc. team
-Copyright 2021 The EleutherAI and HuggingFace Teams
-Copyright 2022 EleutherAI The HuggingFace Inc. team
-Copyright 2022 HuggingFace Inc. team and BigScience
-Copyright 2022 The EleutherAI and HuggingFace Teams
-Copyright 2022 UW-Madison The HuggingFace Inc. team
-Copyright 2021, Google and The HuggingFace Inc. team
-Copyright 2022, Google and The HuggingFace Inc. team
-Copyright Studio Ousia and The HuggingFace Inc. team
-Copyright Studio-Ouisa and The HuggingFace Inc. team
-Copyright 2021 Deepmind and The HuggingFace Inc. team
-Copyright 2022 SHI Labs and The HuggingFace Inc. team
-Copyright 2022 WeChatAI and The HuggingFace Inc. team
-Copyright 2020 Microsoft and the HuggingFace Inc. team
-Copyright 2021 Google AI and The HuggingFace Inc. team
-Copyright 2021 Microsoft and The HuggingFace Inc. team
-Copyright 2022 Google AI and The HuggingFace Inc. team
-Copyright 2022 SenseTime and The HuggingFace Inc. team
-Copyright Meta Platforms and The HuggingFace Inc. team
-Copyright 2018 Salesforce and The HuggingFace Inc. team
-Copyright 2018 The T5 authors and HuggingFace Inc. team
-Copyright 2020 Microsoft and the Hugging Face Inc. team
-Copyright 2020, Microsoft and the HuggingFace Inc. team
-Copyright 2021 ASAPP Inc. and The HuggingFace Inc. team
-Copyright 2021 ASAPP Inc. and the HuggingFace Inc. team
-Copyright 2021 The Eleuther AI and The Google Flax Team
-Copyright 2022 Apple Inc. and The HuggingFace Inc. team
-Copyright 2022 EleutherAI and The HuggingFace Inc. team
-Copyright 2022 Sea AI Lab and The HuggingFace Inc. team
-Copyright 2022 The Impira Team and the HuggingFace Team
-Copyright 2022 The OpenAI team and The HuggingFace Team
-Copyright 2022 The Salesforce authors, The Open AI Team
-Copyright 2022 UW-Madison and The HuggingFace Inc. team
-Copyright 2022, The LongT5 Authors and HuggingFace Inc.
-Copyright 2022, UCLA NLP, The Facebook AI Research Team
-Copyright Google Research and The HuggingFace Inc. team
-Copyright 2018 The Microsoft Research Asia LayoutLM Team
-Copyright 2021 Google Research The HuggingFace Inc. team
-Copyright 2021 The Eleuther AI and HuggingFace Inc. team
-Copyright 2022 ABEJA, Inc. and The HuggingFace Inc. team
-Copyright 2022 Facebook AI and The HuggingFace Inc. team
-Copyright 2022 Sea AI Labs and The HuggingFace Inc. team
-Copyright 2010, The Microsoft Research Asia LayoutLM Team
-Copyright 2021 Studio Ousia and the HuggingFace Inc. team
-Copyright 2021, Google Inc. and The HuggingFace Inc. team
-Copyright 2021, The Microsoft Research Asia MarkupLM Team
-Copyright 2021 NVIDIA Corporation and The HuggingFace Team
-Copyright 2022 Microsoft Research and The HuggingFace Team
-Copyright 2022 NAVER AI Labs and The HuggingFace Inc. team
-Copyright Microsoft Research and The HuggingFace Inc. team
-Copyright 2021 Microsoft Research The HuggingFace Inc. team
-Copyright 2021 The EleutherAI and The HuggingFace Inc. team
-Copyright 2021 The Fairseq Authors and The Google Flax Team
-Copyright 2021 VinAI Research and the HuggingFace Inc. team
-Copyright 2022 Meta Platforms and The HuggingFace Inc. team
-Copyright 2022 The Fairseq Authors and The Google Flax Team
-Copyright 2019 The TensorFlow Authors, The Hugging Face Team
-Copyright 2020 Google Research and The HuggingFace Inc. team
-Copyright 2020 The HuggingFace Team and the AllenNLP authors
-Copyright 2021 Google Research and The HuggingFace Inc. team
-Copyright 2021 The Fairseq Authors The HuggingFace Inc. team
-Copyright 2021 The OpenAI Team Authors, The Google Flax Team
-Copyright The HuggingFace Team and The HuggingFace Inc. team
-Copyright 2020 The Trax Authors and The HuggingFace Inc. team
-Copyright 2020, The RAG Authors and The HuggingFace Inc. team
-Copyright 2021 Facebook AI Research The HuggingFace Inc. team
-Copyright 2021 The HuggingFace Team The HuggingFace Inc. team
-Copyright 2022 The HuggingFace Team The HuggingFace Inc. team
-Copyright 2018 Hao Tan, Mohit Bansal, and the HuggingFace team
-Copyright 2021 The Facebook Inc. and The HuggingFace Inc. team
-Copyright 2021 The Facebook, Inc and The HuggingFace Inc. team
-Copyright 2022 The REALM authors and The HuggingFace Inc. team
-Copyright 2018 The HuggingFace Inc. team, Microsoft Corporation
-Copyright 2018 The HuggingFace Inc. team, The Hugging Face Team
-Copyright 2021 Microsoft Research and The HuggingFace Inc. team
-Copyright 2021 Microsoft Research and the HuggingFace Inc. team
-Copyright 2021 The Facebook, Inc. and The HuggingFace Inc. team
-Copyright 2022 Microsoft Research and The HuggingFace Inc. team
-Copyright 2022 The OpenAI Authors and The HuggingFace Inc. team
-Copyright (c) 2020, VinAI Research and the HuggingFace Inc. team
-Copyright 2020 Ecole Polytechnique and the HuggingFace Inc. team
-Copyright 2021 The Fairseq Authors and The HuggingFace Inc. team
-Copyright 2021 The Fairseq Authors and the HuggingFace Inc. team
-Copyright 2021, The Facebook, Inc. and The HuggingFace Inc. team
-Copyright 2021- NVIDIA Corporation and The HuggingFace Inc. team
-Copyright 2022 Meta Platforms Inc. and The HuggingFace Inc. team
-Copyright 2022 Meta Platforms, Inc.and The HuggingFace Inc. team
-Copyright 2022 The Fairseq Authors and The HuggingFace Inc. team
-Copyright 2022 The Fairseq Authors and the HuggingFace Inc. team
-Copyright 2022 The Metaseq Authors and The HuggingFace Inc. team
-Copyright 2019 Facebook AI Research and the HuggingFace Inc. team
-Copyright 2021 Facebook AI Research and The HuggingFace Inc. team
-Copyright 2021 The HuggingFace Team and The HuggingFace Inc. team
-Copyright 2021 The UCLA NLP Authors and The HuggingFace Inc. team
-Copyright 2022 Facebook AI Research and the HuggingFace Inc. team
-Copyright 2022 Meta Platforms, Inc. and The HuggingFace Inc. team
-Copyright 2022 The HuggingFace Team and The HuggingFace Inc. team
-Copyright 2020 The Microsoft Authors and The HuggingFace Inc. team
-Copyright 2020-present Google Brain and Carnegie Mellon University
-Copyright 2021 Google AI, Ross Wightman, The HuggingFace Inc. team
-Copyright 2022 Intel Labs, OpenMMLab and The HuggingFace Inc. team
-Copyright 2019-present, Facebook, Inc and the HuggingFace Inc. team
-Copyright 2018 Google AI, Google Brain and the HuggingFace Inc. team
-Copyright 2020 The SqueezeBert authors and The HuggingFace Inc. team
-Copyright 2021 Google AI, Google Brain and the HuggingFace Inc. team
-Copyright 2022 Microsoft Research Asia and The HuggingFace Inc. team
-Copyright 2022 Microsoft Research Asia and the HuggingFace Inc. team
-Copyright 2018 Google AI, Google Brain and Carnegie Mellon University
-Copyright 2022 Microsoft Research, Inc. and The HuggingFace Inc. team
-Copyright 2018 The Google AI Language Team Authors, Facebook AI Research
-Copyright 2019 Inria, Facebook AI Research and the HuggingFace Inc. team
-Copyright 2019-present CNRS, Facebook Inc. and the HuggingFace Inc. team
-Copyright 2020 The Google AI Language Team Authors, Facebook AI Research
-Copyright 2021 Facebook AI Research (FAIR) and The HuggingFace Inc. team
-Copyright 2022 Facebook AI Research (FAIR) and The HuggingFace Inc. team
-Copyright 2021 Tel AViv University, AllenAI and The HuggingFace Inc. team
-Copyright 2021, The Facebook AI Research Team and The HuggingFace Inc. team
-Copyright 2020 The Allen Institute for AI team and The HuggingFace Inc. team
-Copyright 2022 University of Wisconsin-Madison and The HuggingFace Inc. team
-Copyright 2021 The Google AI Flax Team Authors, and The HuggingFace Inc. team
-Copyright (c) 2020 The Google AI Language Team Authors, The HuggingFace Inc. team
-Copyright 2020 The Google AI Team, Stanford University and The HuggingFace Inc. team
-Copyright 2021 Facebook AI Research (FAIR), Ross Wightman, The HuggingFace Inc. team
-Copyright 2021 Google Research, Google AI, Google Brain and the HuggingFace Inc. team
-Copyright 2021 The Fairseq Authors, Microsoft Research, and The HuggingFace Inc. team
-Copyright 2022, UCLA NLP, The Facebook AI Research Team and The HuggingFace Inc. team
-Copyright 2021 Iz Beltagy, Matthew E. Peters, Arman Cohan and The HuggingFace Inc. team
-Copyright 2022 Multimedia Computing Group, Nanjing University and The HuggingFace Inc. team
-Copyright 2019-present, the HuggingFace Inc. team, The Google AI Language Team and Facebook, Inc.
-Copyright 2018 The Google AI Language Team Authors, The HuggingFace Inc. team, and the Lxmert Authors
-Copyright 2021 The I-BERT Authors Sehoon Kim, Amir Gholami, Zhewei Yao, Michael Mahoney, Kurt Keutzer
-Copyright 2022 BNRist (Tsinghua University), TKLNDST (Nankai University) and The HuggingFace Inc. team
-Copyright 2022 School of EIC, Huazhong University of Science & Technology and The HuggingFace Inc. team
-Copyright 2020 The Google AI Language Team Authors, Allegro.pl, Facebook Inc. and the HuggingFace Inc. team
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
-
-limitations under the License.
-
----------------------------------------------------------
-
----------------------------------------------------------
-
-websocket-client 1.5.1 - Apache-2.0
-
-
-Copyright 2022 engn33r
+copyright 2016-2018, Andrew Svetlov and aio-libs team
 
 Apache License
 
 Version 2.0, January 2004
 
 http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -3647,157 +2829,51 @@
 
 limitations under the License.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-yarl 1.8.2 - Apache-2.0
-
-
-Copyright 2016-2021, Andrew Svetlov and aio-libs team
-copyright 2016-2018, Andrew Svetlov and aio-libs team
-
-Apache License
-
-Version 2.0, January 2004
-
-http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      
-
-      "License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
-
-      
-
-      "Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
-
-      
-
-      "Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-
-      
-
-      "You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
-
-      
-
-      "Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
-
-      
-
-      "Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
-
-      
-
-      "Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
-
-      
-
-      "Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
-
-      
-
-      "Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
-
-      
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
-
-      (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability. END OF TERMS AND CONDITIONS
-
-APPENDIX: How to apply the Apache License to your work.
-
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
-
-Copyright [yyyy] [name of copyright owner]
-
-Licensed under the Apache License, Version 2.0 (the "License");
-
-you may not use this file except in compliance with the License.
-
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
+packaging 21.3 - Apache-2.0 OR (Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause)
 
-Unless required by applicable law or agreed to in writing, software
 
-distributed under the License is distributed on an "AS IS" BASIS,
-
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-
-See the License for the specific language governing permissions and
+copyright 2014-2019 s
+Copyright (c) Donald Stufft and individual contributors
 
-limitations under the License.
+Apache-2.0 OR (Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause)
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-cryptography 38.0.4 - Apache-2.0 AND BSD-3-Clause AND Python-2.0
+lit 16.0.6 - Apache-2.0 WITH LLVM-exception
 
 
-copyright 2013-2022, Individual
-Copyright (c) Individual contributors
-Copyright (c) 2005-2020, NumPy Developers
-Copyright 2001-2016 Python Software Foundation
-Copyright (c) 2001-2016 Python Software Foundation
-and individual contributors Copyright 2013-2022 .format
+Copyright (c) 2003-2019 University of Illinois at Urbana-Champaign
 
-Apache-2.0 AND BSD-3-Clause AND Python-2.0
+Apache-2.0 WITH LLVM-exception
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-packaging 21.3 - Apache-2.0 OR (Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause)
-
-
-copyright 2014-2019 s
-Copyright (c) Donald Stufft and individual contributors
+attributee 0.1.8 - BSD-2-Clause
 
-Apache-2.0 OR (Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause)
 
----------------------------------------------------------
+Copyright (c) 2020, Luka Cehovin Zajc
 
----------------------------------------------------------
+Copyright (c) <year> <owner> . All rights reserved.
 
-packaging 23.0 - Apache-2.0 OR (Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause)
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
+   1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-copyright 2014-2019 s
-Copyright (c) Donald Stufft and individual contributors
+   2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-Apache-2.0 OR (Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause)
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
 cloudpickle 2.2.1 - BSD-2-Clause
 
@@ -3817,18 +2893,18 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-isodate 0.6.1 - BSD-2-Clause
+enum34 1.1.10 - BSD-2-Clause
 
 
-Copyright 2009, Gerhard Weis
+Copyright (c) 2013, Ethan Furman.
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -3836,33 +2912,18 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-kiwisolver 1.4.4 - BSD-2-Clause
+isodate 0.6.1 - BSD-2-Clause
 
 
-copyright 2018-2021, Nucleic team
-Copyright (c) 2001. Addison-Wesley
-Copyright (c) 2019-2021 Martin Ankerl
-Copyright (c) 2001 by Andrei Alexandrescu
-Copyright (c) 2013, Nucleic Development Team
-Copyright (c) 2019, Nucleic Development Team
-Copyright (c) 2020, Nucleic Development Team
-Copyright (c) 2021, Nucleic Development Team
-Copyright (c) 2013-2017, Nucleic Development Team
-Copyright (c) 2013-2019, Nucleic Development Team
-Copyright (c) 2013-2021, Nucleic Development Team
-Copyright (c) 2013-2022, Nucleic Development Team
-Copyright (c) 2014-2021, Nucleic Development Team
-Copyright (c) 2014-2022, Nucleic Development Team
-Copyright 2000, 2004, 2005Adobe Systems Incorporated
-Copyright (c) 2019-2021 Martin Ankerl <martin.ankerl@gmail.com>
+Copyright 2009, Gerhard Weis
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -3870,19 +2931,20 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-mock 5.0.1 - BSD-2-Clause
+jinja2 3.1.2 - BSD-2-Clause
 
 
-Copyright (c) 2007-2012 Michael Foord
-Copyright (c) 2003-2013, Michael Foord & the mock team
+Copyright 2007 Pallets
+copyright 2007 Pallets
+(c) Copyright 2008 by http://domain.invalid/'>
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -3890,21 +2952,18 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-mpi4py 3.1.1 - BSD-2-Clause
+lap 0.4.0 - BSD-2-Clause
 
 
-Copyright 2009 Brian Quinlan.
-Copyright (c) 2015 Gunter Milde.
-(c) JS Foundation and other contributors
-Copyright JS Foundation and other contributors
+Copyright (c) 2012-2017, Tomas Kazmar
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -3912,22 +2971,19 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-ndg-httpsclient 0.5.1 - BSD-2-Clause
+mock 5.1.0 - BSD-2-Clause
 
 
-Copyright (c) 2012 STFC
-copyright (c) 2012 STFC
-copyright (c) 2011 Science and Technology Facilities Council
-copyright (c) 2012 Science and Technology Facilities Council
-Copyright (c) 2012, Science & Technology Facilities Council (STFC)
+Copyright (c) 2007-2012 Michael Foord
+Copyright (c) 2003-2013, Michael Foord & the mock team
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -3935,17 +2991,21 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-numpy 1.22.2 - BSD-2-Clause
+mpi4py 3.1.1 - BSD-2-Clause
 
 
+Copyright 2009 Brian Quinlan.
+Copyright (c) 2015 Gunter Milde.
+(c) JS Foundation and other contributors
+Copyright JS Foundation and other contributors
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -3953,96 +3013,22 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-numpy 1.24.2 - BSD-2-Clause
+ndg-httpsclient 0.5.1 - BSD-2-Clause
 
 
-Copyright (c) 2017
-(c) Convert Chebyshev
-(c) Multiply a Hermite
-(c) Multiply a Laguerre
-(c) Multiply a Legendre
-(c) Multiply a Chebyshev
-Copyright (c) 2010 - 2019
-Copyright Absoft Corporation
-(c), True, True, False, False
-Copyright 2000 Pearu Peterson
-Copyright 2002 Pearu Peterson
-(c), False, False, False, True
-(c), False, False, True, False
-Copyright (c) 2012 Google Inc.
-Copyright (c) 2014 Ryan Juckett
-Copyright 2011 by Enthought, Inc
-Copyright (c) 2011 Enthought, Inc
-Copyright (c) 2015 Pauli Virtanen
-Copyright (c) 2019 Kevin Sheppard
-Copyright 1999 2011 Pearu Peterson
-Copyright 1999,2000 Pearu Peterson
-Copyright 1999-2004 Pearu Peterson
-Copyright 2001-2005 Pearu Peterson
-Copyright (c) 2019 NumPy Developers
-Copyright (c) 2007 Cybozu Labs, Inc.
-Copyright (c) 2021 Intel Corporation
-Copyright 1999 - 2011 Pearu Peterson
-Copyright (c) 2011 by Enthought, Inc.
-Copyright (c) 2014 Mathjax Consortium
-Copyright (c) 2015 Melissa E. O'Neill
-Copyright (c) 2015-2017 Martin Hensel
-Copyright (c) 2018 Melissa E. O'Neill
-copyright 2008-2022, NumPy Developers
-copyright 2017-2018, NumPy Developers
-Copyright 2007-2018 by the Sphinx team
-Copyright (c) 2021 Microsoft Corporation
-Copyright 2010-2012, D. E. Shaw Research
-Copyright (c) 2005-2015, NumPy Developers
-Copyright (c) 2005-2017, NumPy Developers
-Copyright (c) 2005-2021, NumPy Developers
-Copyright (c) 2005-2022, NumPy Developers
-Copyright (c) 1993 by Sun Microsystems, Inc.
-Copyright (c) 2011-2014, The OpenBLAS Project
-Copyright (c) 2009-2017 The MathJax Consortium
-Copyright (c) 2010-2017 The MathJax Consortium
-Copyright (c) 2011-2015 The MathJax Consortium
-Copyright (c) 2011-2017 The MathJax Consortium
-Copyright (c) 2013-2017 The MathJax Consortium
-Copyright (c) 2014-2017 The MathJax Consortium
-Copyright (c) 2015-2017 The MathJax Consortium
-Copyright (c) 2016-2017 The MathJax Consortium
-Copyright (c) 2008 Ian Bicking and Contributors
-copyright 2010 David Wolever <david@wolever.net>
-Copyright (c) 2010 The Android Open Source Project
-Copyright 2015 Robert Kern <robert.kern@gmail.com>
-Copyright (c) 2002-2017 Free Software Foundation, Inc.
-Copyright 2014 Melissa O'Neill <oneill@pcg-random.org>
-Copyright (c) Donald Stufft and individual contributors
-Copyright (c) 2007, 2011 David Schultz <das@FreeBSD.ORG>
-Copyright (c) 2006-2013 The University of Colorado Denver
-Copyright Absoft Corporation 1994-2002 Absoft Pro FORTRAN
-Copyright (c) 1995, 1996, 1997 Jim Hugunin, hugunin@mit.edu
-Copyright (c) 2003-2005, Jean-Sebastien Roy (js@jeannot.org)
-Copyright (c) 2000-2013 The University of California Berkeley
-Copyright (c) 2016 - 2019 Kim Walisch, <kim.walisch@gmail.com>
-Copyright 2016-2021 Matthew Brett, Isuru Fernando, Matti Picus
-Copyright (c) 1997 - 2002, Makoto Matsumoto and Takuji Nishimura
-Copyright (c) 2004-2018 Max-Planck-Society author Martin Reinecke
-Copyright (c) 2012 Stephen Montgomery-Smith <stephen@FreeBSD.ORG>
-Copyright 1999, 2000, 2001 Regents of the University of California
-Copyright (c) 2007 Free Software Foundation, Inc. <http://fsf.org/>
-Copyright (c) 2009 Free Software Foundation, Inc. <http://fsf.org/>
-Copyright (c) 2006, University of Georgia and Pierre G.F. Gerard-Marchant
-Copyright Absoft Corporation 1994-1998 mV2 Cray Research, Inc. 1994-1996 CF90
-Copyright (c) 2010 by Mark Wiebe (mwwiebe@gmail.com) The University of British Columbia
-Copyright (c) 2011 by Mark Wiebe (mwwiebe@gmail.com) The University of British Columbia
-Copyright (c) 2010-2011 by Mark Wiebe (mwwiebe@gmail.com) The University of British Columbia
-Copyright (c) 2009-2019 Jeff Bezanson, Stefan Karpinski, Viral B. Shah, and other contributors
-Copyright (c) 1992-2013 The University of Tennessee and The University of Tennessee Research Foundation
+Copyright (c) 2012 STFC
+copyright (c) 2012 STFC
+copyright (c) 2011 Science and Technology Facilities Council
+copyright (c) 2012 Science and Technology Facilities Council
+Copyright (c) 2012, Science & Technology Facilities Council (STFC)
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -4050,20 +3036,17 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyasn1 0.4.8 - BSD-2-Clause
+numpy 1.22.2 - BSD-2-Clause
 
 
-copyright u'2005-2019, Ilya Etingof <etingof@gmail.com>
-Copyright (c) 2005-2019, Ilya Etingof <etingof@gmail.com>
-Copyright (c) 2005-2019, Ilya Etingof (mailto:etingof@gmail.com)
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -4071,138 +3054,21 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pygments 2.14.0 - BSD-2-Clause
+pyasn1 0.5.0 - BSD-2-Clause
 
 
-(c) 2014
-(c) FSF.
-(c) V End
-Copyright (c) 2003
-(c) Justin Fletcher
-copyright 2006. Text
-Copyright 2006-'+date
-(c) openEHR Foundation
-Copyright (c) 2005-2006
-Copyright 2013 Wikimedia
-copyright 2006. Uploaded
-(c) 2015 Andreas Rossberg
-(c) Justin Fletcher, 1998
-Copyright (c) 2006, Manni
-Copyright (c) 2008 Silken
-Copyright (c) Rich Hickey
-Copyright (c) 1998 Comment
-Copyright (c) INRIA - Serge
-Copyright 1999-2011 ( VV/ )
-Copyright 2005 Brian Alliet
-Copyright 2015 Ruben De Smet
-Copyright (c) 2006-2022 by the
-Copyright (c) 2007-2008 - INRIA
-Copyright (c) 2008 Slava Pestov
-Copyright (c) 2014 Fullstack.io
-Copyright (c) 2015 Georg Brandl
-(c) Copyright 1999, Artran, Inc.
-Copyright (c) 2009-2010, Gary L.
-Copyright (c) 2017 Johannes Holzl
-Copyright 2020 Microsoft Research
-copyright (c) 2004 by Andre Simon
-Copyright 2007-2012 LassoSoft Inc.
-Francisco Tolmasky. Copyright 2008
-Copyright 1999-2011 Comment Comment
-Copyright 2005 Brian Alliet Comment
-Copyright 2021 by the Pygments team
-Copyright (c) 2005-2007 Terence Parr
-Copyright (c) 2009 Benjamin Kowarsch
-Leaf Corcoran (leafot@gmail.com) 2011
-Copyright (C) 2015 DH electronics GmbH
-Copyright (c) 2004, 2005, 2006 Aelitis
-Copyright (c) 2015 DH electronics GmbH
-Copyright 1997 University of Cambridge
-Copyright 2007-2013 by the Sphinx team
-Copyright 2007-2021 by the Sphinx team
-Copyright (c) 2008 Slava Pestov Comment
-Copyright (c) 2009-2010, Gary L. Cutler
-Copyright (c) 2010, Gary L. Cutler, GPL
-Copyright (c) 2012-2013 Nenad Rakocevic
-Portions (c) International Organization
-Copyright (c) 1997 Borland International
-Copyright (c) 1998 the Initial Developer
-Copyright 2006-2019 by the Pygments team
-Copyright 2006-2020 by the Pygments team
-Copyright 2006-2022 by the Pygments team
-Copyright 2012 Nokia Siemens Networks Oyj
-(c) 2014 Comment.Multiline Text.Whitespace
-Copyright (c) 1993-2003 Yukihiro Matsumoto
-Copyright 2006-2022 by r'the Pygments team
-(c) 2000-2003 by cYcnus visit www.cYcnus.de
-(c) Copyright 2006 by http://mydomain.tld'>
-(c) 2010 Jeremy Ashkenas, DocumentCloud Inc.
-(c) opyright 2003, MetaQuotes Software Corp.
-Copyright (c) 2009-2010, Gary L. Cutler, GPL
-Copyright (c) 1998-2009, Modelica Association
-Copyright (c) 2008, Brian Frank and Andy Frank
-Copyright (c) 2018 Marek Vasut <marex@denx.de>
-Copyright 1997 University of Cambridge Comment
-Copyright 2006-2014, MetaQuotes Software Corp.
-Copyright 2009-2013, MetaQuotes Software Corp.
-Copyright 2012-2018 Manas Technology Solutions
-copyright 2006-2014, MetaQuotes Software Corp.
-(c) Name.Entity 1998-2009, Modelica Association
-Copyright (c) 2010, Gary L. Cutler, GPL Comment
-Copyright (c) 1995-2004 Functional Objects, Inc.
-Copyright 2004-2008 Jean Privat <jean@pryen.org>
-Copyright (c) 2005 Free Software Foundation, Inc.
-Copyright 2014 Lucas Bajolet <r4pass@hotmail.com>
-(c) Name.Entity Copyright 2006 by Text Punctuation
-Copyright (c) 1998,1999,2000,2001,2002 Tal Davidson
-Copyright (c) 2009-2010, Gary L. Cutler, GPL Comment
-Copyright (c) 1991, Jos van der Woude, jvdwoude@hut.nl
-(c) 2010 Jeremy Ashkenas, DocumentCloud Inc. Underscore
-Copyright 2013 Alexis Laferriere <alexis.laf@xymus.net>
-Copyright 2013 Matthieu Lucas <lucasmatthieu@gmail.com>
-Copyright 2014 Alexis Laferriere <alexis.laf@xymus.net>
-Copyright (c) 1991, 1992, Jos van de Woude, jvdwoude@hut.nl
-copyright 2006-2022, Georg Brandl and Pygments contributors
-Copyright 2012-2013 Alexis Laferriere <alexis.laf@xymus.net>
-Copyright (c) 2009 The R Foundation for Statistical Computing
-Copyright (c) 2008 The Regents of the University of California
-(c) Copyright 2006-2022, Georg Brandl and Pygments contributors
-(c) 2006-2022 by Georg Brandl, Matthaus Chajdas and contributors
-Copyright (c) 2011 Nokia Corporation and/or its subsidiary(-ies)
-Copyright (c) 2000 Information-technology Promotion Agency, Japan
-Copyright (c) 2000 Network Applied Communication Laboratory, Inc.
-Copyright (c) 1996-2016 by the PostgreSQL Global Development Group
-Copyright (c) 2009 The R Foundation for Statistical Computing ISBN
-Copyright 2009-2013, MetaQuotes Software Corp. http://www.mql4.com
-Copyright (c) 1994-5 by the Regents of the University of California
-Copyright (c) 2008-2011 The Regents of the University of California
-Murphy (c) 2000-2003 by cYcnus visit www.cYcnus.de licenser@cYcnus.de
-Copyright (c) 1984, 1985, 1988, 2010 Howard Trickey and Oren Patashnik
-Copyright 2006-2014, MetaQuotes Software Corp. http://www.metaquotes.net
-(c) Copyright 2006 Salvatore Filippone University of Rome Tor Vergata Comment
-Copyright 1996 Institut National de Recherche en Informatique et en Automatique
-Copyright (c) 1985-1986, 1992, 1994-1995, 1999-2015 Free Software Comment.Single
-Copyright (c) 2009-2010, Gary L. Cutler, GPL Literal.String.Double . Punctuation
-Copyright 1996 Institut National de Recherche en Informatique et Comment Comment
-copyright 2006-2014, MetaQuotes Software Corp. property link http://www.mql4.com
-Copyright (c) 1984, 1985, 1988, 2010 Howard Trickey and Oren Patashnik. Unlimited
-Copyright (c) 1996, 1997, 1998, 1999, 2000, 2001, 2003, 2004, 2005 Comment.Single
-Copyright (c) 1985-1986, 1992, 1994-1995, 1999-2015 Free Software Foundation, Inc.
-Copyright (c) 2006 Kashia Buch (kashia@vfemail.net), Fabian Buch (fabian@fabian-buch.de)
-Copyright content Knut Muller, Alexander Wolf, Uwe Ritzschke, Paul-Robert Achcenich, 2006
-Copyright (c) 1984, 1989, 1990, 2000, 2001, 2002, 2003, 2004 Free Software Foundation, Inc.
-Copyright (c) 1996, 1997, 1998, 1999, 2000, 2001, 2003, 2004, 2005 Free Software Foundation, Inc.
-Copyright (c) 1995, 1996, 1997, 1998, 1999, 2000, 2001, 2002, 2003, 2004 Free Software Foundation, Inc.
-(c) Copyright 2006 Salvatore Filippone University of Rome Tor Vergata Alfredo Buttari University of Rome Tor Vergata
-Copyright 2012 by Luis Majano and Ortus Solutions, Corp www.gocontentbox.org www.luismajano.com www.ortussolutions.com
-Platform Copyright 2012 by Luis Majano and Ortus Solutions, Corp www.gocontentbox.org www.luismajano.com www.ortussolutions.com
+copyright u'2005-2020, Ilya Etingof <etingof@gmail.com>
+Copyright (c) 2005-2019, Ilya Etingof <etingof@gmail.com>
+Copyright (c) 2005-2020, Ilya Etingof <etingof@gmail.com>
+Copyright (c) 2005-2020, Ilya Etingof (mailto:etingof@gmail.com)
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -4247,19 +3113,34 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-secretstorage 3.3.3 - BSD-2-Clause
+scikit-image 0.21.0 - BSD-2-Clause
 
 
-copyright 2022, Dmitry Shachnev
-Copyright 2012-2018 Dmitry Shachnev <mitya57@gmail.com>
+Copyright David Root
+Copyright 2014 2014 Dan Oneata
+Copyright 1994 Karel Zuiderveld
+Copyright (c) 2010, Matthew Brett
+Copyright 2009-2011 Pierre Raybaut
+Copyright 2015 Jon Lund Steffensen
+Copyright 2007-2010 the Sphinx team
+Copyright 2009-2022 the scikit-image team
+Copyright 2013 The IPython Development Team
+ImageJ (c) . https://imagej.net/Skeletonize3D
+copyright u'2010, Matthew Brett, Fernando Perez
+Copyright 2020 Broad Institute 2020 CellProfiler team
+copyright f'2013- date.today .year, the scikit-image team
+Copyright 2009-2015 Board of Regents of the University of Wisconsin-Madison, Broad Institute
+Copyright 2003-2009 Massachusetts Institute of Technology 2009-2011 Broad Institute 2003 Lee Kamentsky
+Copyright 2003-2009 Massachusetts Institute of Technology 2009-2011 Broad Institute 2003 Lee Kamentsky 2022 Gregory Lee
+Copyright 2003-2009 Massachusetts Institute of Technology 2009-2011 Broad Institute 2003 Lee Kamentsky 2003-2005 Peter J. Verveer
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -4267,24 +3148,19 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-traitlets 5.9.0 - BSD-2-Clause
+secretstorage 3.3.3 - BSD-2-Clause
 
 
-Copyright (c) Enthought, Inc.
-Copyright (c) 2010 Doug Hellmann
-Copyright (c) IPython Development Team
-Copyright (c) Jupyter Development Team
-Copyright 2007-2015 by the Sphinx team
-copyright 2015, The IPython Development Team
-Copyright (c) 2001-, IPython Development Team
+copyright 2022, Dmitry Shachnev
+Copyright 2012-2018 Dmitry Shachnev <mitya57@gmail.com>
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -4292,21 +3168,31 @@
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-xxhash 3.2.0 - BSD-2-Clause
+sympy 1.12 - BSD-2-Clause
 
 
-Copyright (c) 2014-2020 Yue
-Copyright (c) 2014-2020, Yue Du
-Copyright (c) 2012-2020 Yann Collet
-Copyright (c) 2019-2020 Yann Collet
+(c) A. B
+(c) A . B
+(c) Fix Qasm
+Copyright 2016, latex2sympy
+copyright SymPy Development
+Copyright (c) 2009-2023, PyDy
+Copyright (c) 2014 Matthew Rocklin
+copyright 2015, SymPy Development Team
+Copyright (c) 2006-2014 SymPy developers
+Copyright (c) 2001, 2002 Vasil Yaroshevich
+Copyright (c) 2006-2023 SymPy Development Team
+Copyright (c) 2008 Jens Rasch <jyr2000@gmail.com>
+Copyright (c) 2006-2018 SymPy Development Team, 2013-2023 Sergey B Kirpichev
+(c) Copyright 2000-2003 Symbolic Computation Laboratory, University of Western Ontario, London, Canada N6A
 
 Copyright (c) <year> <owner> . All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
@@ -4327,15 +3213,15 @@
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-contourpy 1.0.7 - BSD-2-Clause AND BSD-3-Clause
+contourpy 1.1.0 - BSD-2-Clause AND BSD-3-Clause
 
 
 copyright 2021-2023, ContourPy
 Copyright (c) 2021-2023, ContourPy Developers
 
 BSD-2-Clause AND BSD-3-Clause
 
@@ -4351,124 +3237,70 @@
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-joblib 1.2.0 - BSD-2-Clause AND BSD-3-Clause
+fsspec 2023.6.0 - BSD-2-Clause AND BSD-3-Clause
 
 
-Copyright 2009 Brian Quinlan
-Copyright 2017, Thomas Moreau
-Copyright 2010, Gael Varoquaux
-Copyright 2012, Olivier Grisel
-Copyright (c) 2008 Gael Varoquaux
-Copyright (c) 2009 Gael Varoquaux
-Copyright (c) 2010 Gael Varoquaux
-Copyright (c) 2008-2021, The joblib
-Copyright (c) 2010-2011 Gael Varoquaux
-copyright 2008-2021, Joblib developers
-Copyright (c) 2012, Regents of the University of California
-Copyright 2010, Gael Varoquaux 2001-2004, Fernando Perez 2001 Nathaniel Gray
-Copyright (c) 2009 PiCloud, Inc. <https://web.archive.org/web/20140626004012/http://www.picloud.com/>
+Copyright (c) 2018, Martin Durant
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-multiprocess 0.70.14 - BSD-2-Clause AND BSD-3-Clause
+mpmath 1.3.0 - BSD-2-Clause AND BSD-3-Clause
 
 
-Copyright (c) 2006-2008, R Oudkerk
-Copyright (c) 2008-2016 California Institute of Technology
-Copyright (c) 2022 The Uncertainty Quantification Foundation
-Copyright (c) 2016-2022 The Uncertainty Quantification Foundation
-Copyright (c) 2018-2022 The Uncertainty Quantification Foundation
+Copyright 2013 Timo Hartmann (thartmann15 at gmail.com)
+Copyright (c) 2005-2021 Fredrik Johansson and mpmath contributors
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-oauthlib 3.2.2 - BSD-2-Clause AND BSD-3-Clause
+networkx 3.1 - BSD-2-Clause AND BSD-3-Clause
 
 
-(c) Access Token
-(c) Redirection URI
-Copyright (c) 2019 The OAuthlib Community
-copyright (c) 2019 by The OAuthlib Community
+(c) Fcc Bcc None
+Copyright (c) 2015 - Thomson Licensing, SAS
+Copyright 2011 Alex Levenson <alex@isnotinvain.com>
+Copyright 2011 Reya Group <http://www.reyagroup.com>
+copyright f'2004- date.today .year, NetworkX Developers
+Copyright 2011 Diederik van Liere <diederik.vanliere@rotman.utoronto.ca>
+Copyright (c) 2004-2023 NetworkX Developers Aric Hagberg <hagberg@lanl.gov> Dan Schult <dschult@colgate.edu>
+Copyright (c) 2004-2023, NetworkX Developers Aric Hagberg <hagberg@lanl.gov> Dan Schult <dschult@colgate.edu>
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pandas 1.5.3 - BSD-2-Clause AND BSD-3-Clause
+oauthlib 3.2.2 - BSD-2-Clause AND BSD-3-Clause
 
 
-Copyright (c) 2009', join
-Copyright 2014-2019, xarray
-Copyright (c) 2012 Google Inc.
-Copyright (c) 2015 Jared Hobbs
-Copyright (c) 1994 David Burren
-Copyright (c) 2011 Szabolcs Nagy
-Copyright (c) 2011 Valentin Ochs
-Copyright (c) 2017 Anthony Sottile
-Copyright (c) 2005-2014 Rich Felker
-Copyright (c) 2010, Albert Sweigart
-Copyright (c) 2002 Michael Ringgaard
-Copyright (c) 2003-2011 David Schultz
-Copyright (c) 2008 Stephen L. Moshier
-Copyright (c) 2011 by Enthought, Inc.
-Copyright 2017- dateutil contributors
-Copyright (c) 2003-2009 Bruce D. Evans
-Copyright (c) 2001-2008 Ville Laurikari
-Copyright (c) 2003-2009 Steven G. Kargl
-Copyright (c) 1993,2004 Sun Microsystems
-Copyright (c) 2001, 2002 Enthought, Inc.
-Copyright (c) 2003-2012 SciPy Developers
-Copyright (c) 2012, Lambda Foundry, Inc.
-Copyright (c) 1994 Sun Microsystems, Inc.
-Copyright (c) 2005-2011, NumPy Developers
-Copyright (c) 2017 - dateutil contributors
-Copyright (c) 2015- - dateutil contributors
-Copyright (c) 2016, PyData Development Team
-Copyright (c) 2020, PyData Development Team
-Copyright 2017- Paul Ganssle <paul@ganssle.io>
-Copyright (c) 2011-2022, Open source contributors
-Copyright (c) 2008 The Android Open Source Project
-Copyright (c) 2015- - Paul Ganssle <paul@ganssle.io>
-Copyright (c) 2010-2012 Archipel Asset Management AB.
-Copyright (c) 2007 Nick Galbreath nickg at modp dot com
-Copyright (c) Donald Stufft and individual contributors
-Copyright (c) 2014-2016 - Yaron de Leeuw <me@jarondl.net>
-Copyright (c) 2019 Hadley Wickham RStudio and Evan Miller
-Copyright (c) 2008- Attractive Chaos <attractor@live.co.uk>
-Copyright (c) 2003-2011 - Gustavo Niemeyer <gustavo@niemeyer.net>
-Copyright (c) 1988-1993 The Regents of the University of California
-Copyright (c) 2011-2013, ESN Social Software AB and Jonas Tarnstrom
-Copyright (c) 2012-2014 - Tomi Pievilainen <tomi.pievilainen@iki.fi>
-Copyright (c) 1995-2001 Corporation for National Research Initiatives
-Copyright (c) 2008, 2009, 2011 by Attractive Chaos <attractor@live.co.uk>
-Copyright (c) 1991 - 1995, Stichting Mathematisch Centrum Amsterdam, The Netherlands
-Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010 Python Software Foundation
-Copyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team
+(c) Access Token
+(c) Redirection URI
+Copyright (c) 2019 The OAuthlib Community
+copyright (c) 2019 by The OAuthlib Community
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-psutil 5.9.4 - BSD-2-Clause AND BSD-3-Clause
+psutil 5.9.5 - BSD-2-Clause AND BSD-3-Clause
 
 
 copyright 2009- s, s
 Copyright (c) 2009, Giampaolo
 Copyright (c) 2017, Arnon Yaari
 Copyright (c) 2015, Ryo ONODERA.
 Copyright (c) 2009 Giampaolo Rodola
@@ -4498,786 +3330,2394 @@
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-scikit-learn 1.2.1 - BSD-2-Clause AND BSD-3-Clause
+pynvml 11.5.0 - BSD-2-Clause AND BSD-3-Clause
+
+
+Copyright (c) 2011-2021, NVIDIA Corporation
+Copyright (c) 2011-2023, NVIDIA Corporation
+
+BSD-2-Clause AND BSD-3-Clause
+
+---------------------------------------------------------
+
+---------------------------------------------------------
+
+scikit-learn 1.3.0 - BSD-2-Clause AND BSD-3-Clause
 
 
 (c) 2014
 (c) INRIA
 (c) INRIA 2010
 (c) INRIA 2011
 (c) INRIA 2014
 Copyright INRIA
-(c) 2011 import warnings
 Copyright (c) 2011, 2012
 Copyright (c) 2018, pandas
 Copyright 2014 Steven Loria
 Copyright 2011-2019 Twitter, Inc.
 (c) INRIA, University of Amsterdam
+Copyright (c) 2015, Leland McInnes
 Copyright 2015 Jon Lund Steffensen
 Copyright (c) 2003-2016 Paul T. McGuire
-Copyright (c) 2007-2022 The scikit-learn
+Copyright (c) 2007-2023 The scikit-learn
 Copyright 2011-2019 The Bootstrap Authors
 Copyright (c) 2011 Renato de Pontes Pereira
 (c) OpenJS Foundation and other contributors
 Copyright (c) 2007-2014 The LIBLINEAR Project
 copyrights by Aric Hagberg <hagberg@lanl.gov>
 Copyright (c) 2004-2017 Holger Krekel and others
 copyright f'2007 - datetime.now .year, scikit-learn
 Copyright (c) Donald Stufft and individual contributors
 Copyright (c) 2000-2009 Chih-Chung Chang and Chih-Jen Lin
+(c) 2011 import warnings from numbers import Integral, Real
 Copyright (c) 2011 Olivier Grisel <olivier.grisel@ensta.org>
 Copyright (c) 2011 David Warde-Farley <wardefar at iro dot umontreal dot ca>
 Copyright 2011-2019 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
 Copyright (c) 2007-2009 Cournapeau David <cournape@gmail.com> 2010 Fabian Pedregosa <fabian.pedregosa@inria.fr>
 Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018 Python Software Foundation
 Copyright (c) 2007 David Cournapeau <cournape@gmail.com> 2010 Fabian Pedregosa <fabian.pedregosa@inria.fr> 2010 Olivier Grisel <olivier.grisel@ensta.org>
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-threadpoolctl 3.1.0 - BSD-2-Clause AND BSD-3-Clause
+scipy 1.10.1 - BSD-2-Clause AND BSD-3-Clause
 
 
-Copyright (c) 2017, Intel Corporation
-(Copyright (c) 2017, Intel Corporation)
-Copyright (c) 2019, threadpoolctl contributors
+(c), (c)
+(c) . B' Both
+(c) B Whether
+Copyright 2001
+Copyright 2003
+Copyright 2008
+(c) 2003, C. Bond
+(c) Case 2 Caller
+(c) Copyright John
+Copyright 2014 LRI
+Copyright 2015 LRI
+(c) Date July, 1988
+Copyright 2018 Nico
+Gamma (c) Gamma (c)
+(c) Compute Hessian H
+Copyright 2014 LASMEA
+Copyright Jens Maurer
+copyright Cephes Math
+(c) David Abrahams 2002
+Copyright (c) 2010 Ilya
+Copyright Albert Steppi
+Copyright Gautam Sewani
+Copyright Nat Goodspeed
+(c) 2008 Gordon Woodhull
+(c) 2011 import warnings
+Copyright (c) 2018 Yi Ji
+Copyright 2012 IBM Corp.
+Copyright 2013 Kyle Lutz
+Copyright 2018 Ulf Adams
+Copyright Catch2 Authors
+Copyright Lingxi Li 2015
+copyright Boost Software
+copyright Xiaogang Zhang
+copyrighted by Alan Genz
+(c) Peter Kankowski, 2008
+Copyright (c) 2019 Damian
+Copyright 2003 Bruce Barr
+Copyright 2006 Johan Rade
+Copyright 2011 Simon West
+Copyright 2012 K R Walker
+Copyright Jaap Suter 2003
+Copyright Jan Langer 2002
+Copyright Paul A. Bristow
+Csp self.spmatrix (c) Dsp
+copyright Jason Rice 2016
+copyright Jason Rice 2017
+copyright by Renee Touzin
+Copyright 2000 Jens Maurer
+Copyright 2003 Jeremy Siek
+Copyright 2005 Dan Marsden
+Copyright 2005 Peter Dimov
+Copyright 2007 Peter Dimov
+Copyright 2008 Beman Dawes
+Copyright 2008 Peter Dimov
+Copyright 2009 Neil Groves
+Copyright 2010 Beman Dawes
+Copyright 2013 Ankur Sinha
+Copyright 2013 Peter Dimov
+Copyright 2014 Neil Groves
+Copyright 2014 Peter Dimov
+Copyright 2015 Peter Dimov
+Copyright 2016 Jorge Lodos
+Copyright 2017 Peter Dimov
+Copyright 2018 Peter Dimov
+Copyright 2019 Peter Dimov
+Copyright 2020 Peter Dimov
+Copyright Beman Dawes 2001
+Copyright Beman Dawes 2002
+Copyright Beman Dawes 2003
+Copyright Beman Dawes 2005
+Copyright Beman Dawes 2006
+Copyright Beman Dawes 2007
+Copyright Beman Dawes 2008
+Copyright Beman Dawes 2009
+Copyright Beman Dawes 2010
+Copyright Beman Dawes 2011
+Copyright Beman Dawes 2013
+Copyright Beman Dawes 2014
+Copyright Beman Dawes 2015
+Copyright Bruno Dutra 2015
+Copyright Evan Miller 2020
+Copyright Franz Detro 2014
+Copyright Jens Maurer 2000
+Copyright Jens Maurer 2002
+Copyright Jens Maurer 2006
+Copyright Joel Falcou 2015
+Copyright Neil Groves 2007
+Copyright Neil Groves 2009
+Copyright Neil Groves 2010
+Copyright Neil Groves 2014
+Copyright Peter Dimov 2001
+Copyright Peter Dimov 2019
+Copyright Rene Rivera 2013
+Copyright Rene Rivera 2014
+Copyright Rene Rivera 2015
+Copyright Rene Rivera 2017
+Copyright Thomas Mang 2012
+Copyright ohn Maddock 2012
+(c) 2011 import numpy as np
+(c) 2012 import numpy as np
+(c) 2014 import numpy as np
+(c) Copyright 2014 Jim Bell
+Copyright (c) 2011 Jamboree
+Copyright (c) 2013 Jamboree
+Copyright (c) 2014 Jamboree
+Copyright 2000 by Alan Genz
+Copyright 2001 John Maddock
+Copyright 2004 Eric Niebler
+Copyright 2005 Eric Niebler
+Copyright 2006 Eric Niebler
+Copyright 2006 John Maddock
+Copyright 2007 Eric Niebler
+Copyright 2008 Eric Niebler
+Copyright 2008 John Maddock
+Copyright 2009 Eric Niebler
+Copyright 2010 Eric Niebler
+Copyright 2010 John Maddock
+Copyright 2011 Eric Niebler
+Copyright 2011 John Maddock
+Copyright 2011, Andrew Ross
+Copyright 2012 Eric Niebler
+Copyright 2012 John Maddock
+Copyright 2013 John Maddock
+Copyright 2013 Paul Bristow
+Copyright 2014 John Maddock
+Copyright 2014 NumScale SAS
+Copyright 2014 Paul Bristow
+Copyright 2015 John Maddock
+Copyright 2015 NumScale SAS
+Copyright 2016 John Maddock
+Copyright 2017 Daniel James
+Copyright 2017 John Maddock
+Copyright 2017 Vinnie Falco
+Copyright 2018 John Maddock
+Copyright 2019 John Maddock
+Copyright 2020 John Maddock
+Copyright Beman Dawes, 2009
+Copyright Eric Niebler 2005
+Copyright Eric Niebler 2008
+Copyright Eric Niebler 2009
+Copyright Eric Niebler 2014
+Copyright John Maddock 2005
+Copyright John Maddock 2006
+Copyright John Maddock 2007
+Copyright John Maddock 2008
+Copyright John Maddock 2009
+Copyright John Maddock 2010
+Copyright John Maddock 2011
+Copyright John Maddock 2012
+Copyright John Maddock 2013
+Copyright John Maddock 2014
+Copyright John Maddock 2015
+Copyright John Maddock 2016
+Copyright John Maddock 2017
+Copyright John Maddock 2018
+Copyright Louis Dionne 2013
+Copyright Orson Peters 2017
+Copyright Paul Bristow 2007
+Copyright Paul Bristow 2014
+Copyright Robert Ramey 2007
+Copyright Robin Eckert 2015
+Copyright Timmo Stange 2007
+copyright Louis Dionne 2016
+(c) Copyright Francois Faure
+(c) Copyright Howard Hinnant
+Copyright (c) 2017 Dynatrace
+Copyright (c) 2018 ERGO-Code
+Copyright (c) 2021 ERGO-Code
+Copyright (c) 2022 ERGO-Code
+Copyright (c) Piers Lawrence
+Copyright 2002 Daryle Walker
+Copyright 2003 - 2011 LASMEA
+Copyright 2005 Ben Hutchings
+Copyright 2005 Daniel Egloff
+Copyright 2005 Daniel Wallin
+Copyright 2006 Andy Tompkins
+Copyright 2006 Ion Gaztanaga
+Copyright 2007 Aaron Windsor
+Copyright 2007 Andy Tompkins
+Copyright 2007 Baruch Zilber
+Copyright 2007 Boris Gubenko
+Copyright 2007 David Jenkins
+Copyright 2008 CodeRage, LLC
+Copyright 2008 David Jenkins
+Copyright 2008 Gautam Sewani
+Copyright 2009 Andy Tompkins
+Copyright 2010 Andy Tompkins
+Copyright 2012 Chung-Lin Wen
+Copyright 2012 Denis Demidov
+Copyright 2013 Andrea Gavana
+Copyright 2014 MetaScale SAS
+Copyright 2015 John Fletcher
+Copyright 2020 Ion Gaztanaga
+Copyright Andy Tompkins 2006
+Copyright Bryce Lelbach 2010
+Copyright Daniel Walker 2006
+Copyright Daniel Walker 2007
+Copyright Daniel Wallin 2005
+Copyright Daniel Wallin 2006
+Copyright Daniel Wallin 2007
+Copyright Dietmar Kuehl 2001
+Copyright Eric Friedman 2002
+Copyright Eric Friedman 2003
+Copyright Gautam Sewani 2008
+Copyright John Maddock, 2020
+Copyright Nat Goodspeed 2014
+Copyright Nick Thompson 2017
+Copyright Nick Thompson 2019
+Copyright Samuel Krempp 2003
+Copyright Vladimir Prus 2002
+Copyright Vladimir Prus 2004
+Copyright Yosef Meller, 2009
+(c) Copyright Bill Kempf 2001
+(c) Copyright Bill Kempf 2002
+(c) Copyright Brian Kuhl 2016
+(c) Copyright Jens Mauer 2001
+(c) Copyright Johan Rade 2006
+(c) Copyright Paul Moore 1999
+(c) Copyright Synge Todo 2003
+Copyright (c) 2002 Bill Kempf
+Copyright (c) 2004 Peder Holt
+Copyright (c) 2005 Peder Holt
+Copyright (c) 2006 Johan Rade
+Copyright (c) 2007 Peder Holt
+Copyright (c) 2010 Peder Holt
+Copyright (c) 2014 Eric Moore
+Copyright (c) 2014 Ian Forbed
+Copyright (c) 2015 Mario Lang
+Copyright (c) 2018 Fady Essam
+Copyright (c) 2018 agate-pris
+Copyright (c) 2019 Peter Bell
+Copyright (c) 2019 agate-pris
+Copyright (c) 2020 Jeff Trull
+Copyright 2002 Gary Strangman
+Copyright 2002 Pearu Peterson
+Copyright 2005 Douglas Gregor
+Copyright 2005 Jeremy G. Siek
+Copyright 2005 Joel de Guzman
+Copyright 2006 Douglas Gregor
+Copyright 2006 Roland Schwarz
+Copyright 2008 Hartmut Kaiser
+Copyright 2008 Howard Hinnant
+Copyright 2009, Andrew Sutton
+Copyright 2010 Mario Mulansky
+Copyright 2011 Karsten Ahnert
+Copyright 2011 Mario Mulansky
+Copyright 2012 Christoph Koke
+Copyright 2012 Karsten Ahnert
+Copyright 2012 Mario Mulansky
+Copyright 2013 Karsten Ahnert
+Copyright 2013 Mario Mulansky
+Copyright 2013 Nikhar Agrawal
+Copyright 2014 Anton Bikineev
+Copyright 2014 Bill Gallafent
+Copyright 2014, Eric W. Moore
+Copyright 2015 Mario Mulansky
+Copyright 2018 Hans Dembinski
+Copyright 2018 Stefan Seefeld
+Copyright 2019 Hans Dembinski
+Copyright 2019 Mateusz Loskot
+Copyright 2020 Hans Dembinski
+Copyright 2020 Madhur Chauhan
+Copyright Alain Miniussi 2014
+Copyright Andreas Schwab 2019
+Copyright Beman Dawes 1994-99
+Copyright Christian Lorentzen
+Copyright David Abrahams 2001
+Copyright David Abrahams 2002
+Copyright David Abrahams 2003
+Copyright David Abrahams 2004
+Copyright David Abrahams 2005
+Copyright David Abrahams 2006
+Copyright David Abrahams 2009
+Copyright Douglas Gregor 2003
+Copyright Douglas Gregor 2004
+Copyright Hans Dembinski 2020
+Copyright Jim Bosch 2010-2012
+Copyright John Maddock 2006-7
+Copyright John Maddock 2007-8
+Copyright Marco Guazzone 2014
+Copyright Nick Thompson, 2017
+Copyright Nick Thompson, 2018
+Copyright Nick Thompson, 2019
+Copyright Nick Thompson, 2020
+Copyright Oliver Kowalke 2009
+Copyright Oliver Kowalke 2013
+Copyright Oliver Kowalke 2014
+Copyright Oliver Kowalke 2015
+Copyright Oliver Kowalke 2016
+Copyright Oliver Kowalke 2017
+Copyright Oliver Kowalke 2018
+Copyright Ruslan Baratov 2017
+Copyright Shreyans Doshi 2017
+Copyright Stefan Seefeld 2005
+Copyright Stefan Seefeld 2016
+Copyright Steven J. Ross 2014
+Copyright Vladimir Prus, 2002
+Copyright Xiaogang Zhang 2006
+(c) Copyright Beman Dawes 1999
+(c) Copyright Beman Dawes 2000
+(c) Copyright Beman Dawes 2001
+(c) Copyright Beman Dawes 2002
+(c) Copyright Beman Dawes 2003
+(c) Copyright Boris Rasin 2014
+(c) Copyright Darin Adler 2000
+(c) Copyright Darin Adler 2001
+(c) Copyright Jens Maurer 2001
+(c) Copyright Jens Maurer 2003
+(c) Copyright Jeremy Siek 1999
+(c) Copyright Jeremy Siek 2000
+(c) Copyright Jeremy Siek 2001
+(c) Copyright Jeremy Siek 2002
+(c) Copyright Jeremy Siek 2004
+(c) Copyright Jeremy Siek 2006
+(c) Copyright Jim Douglas 2005
+(c) Copyright Jorge Lodos 2008
+(c) Copyright Peter Dimov 2001
+(c) Copyright Peter Dimov 2002
+(c) Copyright Peter Dimov 2008
+(c) Copyright Peter Dimov 2017
+(c) Copyright Peter Dimov 2019
+(c) Copyright Rene Rivera 2005
+(c) Copyright Thomas Witt 2002
+(c) Copyright Tobias Schwinger
+(c) Copyright Toon Knapen 2001
+(c) Copyright Toon Knapen 2003
+Copyright (c) 2001 Darin Adler
+Copyright (c) 2001 Doug Gregor
+Copyright (c) 2001 Peter Dimov
+Copyright (c) 2002 Beman Dawes
+Copyright (c) 2002 Jens Maurer
+Copyright (c) 2002 Peter Dimov
+Copyright (c) 2003 Daniel Frey
+Copyright (c) 2003 Peter Dimov
+Copyright (c) 2003 Thomas Witt
+Copyright (c) 2005 Dan Marsden
+Copyright (c) 2005 Peter Dimov
+Copyright (c) 2006 Dan Marsden
+Copyright (c) 2006 Peter Dimov
+Copyright (c) 2007 Dan Marsden
+Copyright (c) 2007 Peter Dimov
+Copyright (c) 2008 Beman Dawes
+Copyright (c) 2008 Damian Eads
+Copyright (c) 2008 Peter Dimov
+Copyright (c) 2009 Carl Barron
+Copyright (c) 2009 Peter Dimov
+Copyright (c) 2010 Neil Groves
+Copyright (c) 2012 David Stone
+Copyright (c) 2012 Google Inc.
+Copyright (c) 2013 Carl Barron
+Copyright (c) 2013 Peter Dimov
+Copyright (c) 2014 Lee Clagett
+Copyright (c) 2014 Peter Dimov
+Copyright (c) 2014 Tomoki Imai
+Copyright (c) 2015 Seth Heeren
+Copyright (c) 2016 Lee Clagett
+Copyright (c) 2016 Peter Dimov
+Copyright (c) 2018 Peter Dimov
+Copyright (c) 2019 Peter Dimov
+Copyright (c) 2020 Peter Dimov
+Copyright (c) Beman Dawes 2011
+Copyright (c) Beman Dawes 2015
+Copyright (c) Dan Watkins 2003
+Copyright (c) Jeremy Siek 2001
+Copyright (c) Thomas Witt 2002
+Copyright 1999 Travis Oliphant
+Copyright 2000 Maarten Keijzer
+Copyright 2005 Matthias Troyer
+Copyright 2005 Travis Oliphant
+Copyright 2008 Joaquin M Lopez
+Copyright 2009 Steven Watanabe
+Copyright 2010 Kenneth Riddile
+Copyright 2010 Paul A. Bristow
+Copyright 2011 Paul A. Bristow
+Copyright 2011 Steven Watanabe
+Copyright 2012 Andreas Pokorny
+Copyright 2012 Paul A. Bristow
+Copyright 2012 Steven Watanabe
+Copyright 2012-20 John Maddock
+Copyright 2013 Andrey Semashev
+Copyright 2013 Pascal Germroth
+Copyright 2014 Andrey Semashev
+Copyright 2014 Antony Polukhin
+Copyright 2015 Andrey Semashev
+Copyright 2015 Antony Polukhin
+Copyright 2015 Steven Watanabe
+Copyright 2016 Andrey Semashev
+Copyright 2016 Joaquin M Lopez
+Copyright 2017 Andrey Semashev
+Copyright 2017 Joaquin M Lopez
+Copyright 2018 Joaquin M Lopez
+Copyright 2018 Steven Watanabe
+Copyright 2019 Emil Dotchevski
+Copyright 2019 Henry Schreiner
+Copyright 2020 Andrey Semashev
+Copyright 2020 Samuel Debionne
+Copyright Adam D. Walling 2012
+Copyright Alexander Grund 2018
+Copyright Andrey Semashev 2013
+Copyright Andrey Semashev 2015
+Copyright Andrey Semashev 2016
+Copyright Andrey Semashev 2018
+Copyright Andrey Semashev 2019
+Copyright Andrey Semashev 2020
+Copyright Bertolt Mildner 2004
+Copyright Daniel Trebbien 2010
+Copyright Emil Dotchevski 2007
+Copyright Frank Mori Hess 2007
+Copyright Frank Mori Hess 2008
+Copyright Frank Mori Hess 2009
+Copyright John Maddock 2008-11
+Copyright John R. Bandela 2001
+Copyright Paul A. Bristow 2006
+Copyright Paul A. Bristow 2007
+Copyright Paul A. Bristow 2010
+Copyright Paul A. Bristow 2012
+Copyright Paul A. Bristow 2013
+Copyright Paul A. Bristow 2014
+Copyright Paul A. Bristow 2017
+Copyright Paul Mensonides 2003
+Copyright Sergey Krivonos 2017
+Copyright Steven Watanabe 2009
+Copyright Steven Watanabe 2010
+Copyright Steven Watanabe 2011
+Copyright Steven Watanabe 2014
+copyrighted by Enthought, Inc.
+(c) Copyright 2005 John Maddock
+(c) Copyright 2008 Robert Ramey
+(c) Copyright 2010 Daniel James
+(c) Copyright 2010 Robert Ramey
+(c) Copyright 2020 Robert Ramey
+(c) Copyright Daniel K. O. 2005
+(c) Copyright Hubert Holin 2001
+(c) Copyright Hubert Holin 2003
+(c) Copyright Jeremy Siek, 2001
+(c) Copyright John Maddock 2000
+(c) Copyright John Maddock 2001
+(c) Copyright John Maddock 2002
+(c) Copyright John Maddock 2003
+(c) Copyright John Maddock 2005
+(c) Copyright John Maddock 2006
+(c) Copyright John Maddock 2007
+(c) Copyright John Maddock 2008
+(c) Copyright John Maddock 2010
+(c) Copyright John Maddock 2011
+(c) Copyright John Maddock 2015
+(c) Copyright John Maddock 2017
+(c) Copyright John Maddock 2018
+(c) Copyright Lie-Quan Lee 2001
+(c) Copyright Martin Wille 2003
+(c) Copyright Orson Peters 2017
+(c) Copyright Rani Sharoni 2003
+(c) Copyright Robert Ramey 2004
+Copyright (c) 2002 John Maddock
+Copyright (c) 2003 John Maddock
+Copyright (c) 2003 Martin Wille
+Copyright (c) 2004 John Maddock
+Copyright (c) 2005 Eric Niebler
+Copyright (c) 2006 Eric Niebler
+Copyright (c) 2006 John Maddock
+Copyright (c) 2006 Stephen Nutt
+Copyright (c) 2007 John Maddock
+Copyright (c) 2007, Damian Eads
+Copyright (c) 2008 Eric Niebler
+Copyright (c) 2008 Roelof Naude
+Copyright (c) 2009 John Maddock
+Copyright (c) 2010 Eric Niebler
+Copyright (c) 2011 Aaron Graham
+Copyright (c) 2011 Brandon Kohn
+Copyright (c) 2011 Eric Niebler
+Copyright (c) 2011 John Maddock
+Copyright (c) 2012 Nathan Ridge
+Copyright (c) 2012 Oswin Krause
+Copyright (c) 2012 Robert Ramey
+Copyright (c) 2013 Eurodecision
+Copyright (c) 2014 Eric Niebler
+Copyright (c) 2014 Mageswaran.D
+Copyright (c) 2015 John Maddock
+Copyright (c) 2015 Orson Peters
+Copyright (c) 2015 Robert Ramey
+Copyright (c) 2016 Adrian Veres
+Copyright (c) 2017 John Maddock
+Copyright (c) 2017 Michel Morin
+Copyright (c) 2017 Robert Ramey
+Copyright (c) 2017 Vinnie Falco
+Copyright (c) 2020 John Maddock
+Copyright (c) 2021 Orson Peters
+Copyright (c) Tyler Reddy, 2016
+Copyright 2002-2018 Peter Dimov
+Copyright 2003-2005 Peter Dimov
+Copyright 2004-2005 Peter Dimov
+Copyright 2004-2006 Peter Dimov
+Copyright 2004-2008 Peter Dimov
+Copyright 2005-2013 Peter Dimov
+Copyright 2006 Thorsten Ottosen
+Copyright 2007 Tobias Schwinger
+Copyright 2008 Christophe Henry
+Copyright 2008,2012 Peter Dimov
+Copyright 2009-2014 Neil Groves
+Copyright 2011 Christophe Henry
+Copyright 2012 (c) Google, Inc.
+Copyright 2012 Lucanus Simonson
+Copyright 2012, Philipp Moeller
+Copyright 2013 Maciej Piechotka
+Copyright 2015-2017 Peter Dimov
+Copyright 2015-2019 Peter Dimov
+Copyright 2015-2020 Peter Dimov
+Copyright 2017-2019 Peter Dimov
+Copyright Aleksey Gurtovoy 2004
+Copyright Aleksey Gurtovoy 2006
+Copyright Aleksey Gurtovoy 2008
+Copyright Beman Dawes 1995-2001
+Copyright Beman Dawes 2002-2009
+Copyright Benjamin Sobotta 2012
+Copyright Benjamin Worpitz 2018
+Copyright Charly Chevalier 2015
+Copyright Jens Maurer 2000-2001
+Copyright Jessica Hamilton 2014
+Copyright Neil Groves 2003-2004
+Copyright Nikolay Mladenov 2007
+Copyright Pavol Droba 2002-2003
+Copyright Pavol Droba 2002-2004
+Copyright Pavol Droba 2002-2006
+Copyright Peter Dimov 2000-2002
+Copyright Peter Dimov 2000-2003
+Copyright Peter Dimov 2001-2002
+Copyright Peter Dimov 2001-2003
+Copyright Rene Rivera 2005-2016
+Copyright Rene Rivera 2008-2013
+Copyright Rene Rivera 2008-2015
+Copyright Rene Rivera 2008-2017
+Copyright Rene Rivera 2008-2019
+Copyright Rene Rivera 2011-2012
+Copyright Rene Rivera 2011-2015
+Copyright Rene Rivera 2012-2015
+Copyright Rene Rivera 2013-2015
+Copyright Rene Rivera 2014-2015
+Copyright Rene Rivera 2015-2016
+Copyright Rene Rivera 2015-2019
+Copyright Thorsten Ottosen 2006
+Copyright Thorsten Ottosen 2008
+(c) Copyright 2007 Andrew Sutton
+(c) Copyright 2007 David Deakins
+(c) Copyright 2008 CodeRage, LLC
+(c) Copyright 2012 Vicente Botet
+(c) Copyright 2013 Tim Blechmann
+(c) Copyright Andrew Sutton 2007
+(c) Copyright Artyom Beilis 2010
+(c) Copyright Balint Cserni 2017
+(c) Copyright Boris Gubenko 2007
+(c) Copyright Bruno Lalande 2008
+(c) Copyright Bryce Lelbach 2010
+(c) Copyright Bryce Lelbach 2011
+(c) Copyright Daniel Wallin 2004
+(c) Copyright Daryle Walker 2001
+(c) Copyright Edward Diener 2011
+(c) Copyright Edward Diener 2012
+(c) Copyright Edward Diener 2013
+(c) Copyright Edward Diener 2014
+(c) Copyright Edward Diener 2015
+(c) Copyright Edward Diener 2016
+(c) Copyright Edward Diener 2019
+(c) Copyright Edward Diener 2020
+(c) Copyright Gennaro Prota 2003
+(c) Copyright Ion Gaztanaga 2005
+(c) Copyright Ion Gaztanaga 2006
+(c) Copyright Ion Gaztanaga 2008
+(c) Copyright Ion Gaztanaga 2009
+(c) Copyright Ion Gaztanaga 2014
+(c) Copyright Milan Svoboda 2008
+(c) Copyright Nick Thompson 2017
+(c) Copyright Nick Thompson 2018
+(c) Copyright Nick Thompson 2019
+(c) Copyright Nick Thompson 2020
+(c) Copyright Noel Belcourt 2007
+(c) Copyright Pablo Halpern 2009
+(c) Copyright Ronald Garcia 2002
+Copyright (c) 2001 Bruce Florman
+Copyright (c) 2001 Daniel Nuffer
+Copyright (c) 2001 Daryle Walker
+Copyright (c) 2001 Dietmar Kuehl
+Copyright (c) 2002 Jeff Westfahl
+Copyright (c) 2003 Eric Friedman
+Copyright (c) 2003 Gennaro Prota
+Copyright (c) 2003 Giovanni Bajo
+Copyright (c) 2003 Vaclav Vesely
+Copyright (c) 2003 Vesa Karvonen
+Copyright (c) 2003 Vladimir Prus
+Copyright (c) 2004 Angus Leeming
+Copyright (c) 2004 Daniel Wallin
+Copyright (c) 2005 Aaron Windsor
+Copyright (c) 2005 Stefan Arentz
+Copyright (c) 2006 Daniel Wallin
+Copyright (c) 2006 Tomas Puverle
+Copyright (c) 2008 Ion Gaztanaga
+Copyright (c) 2009 Andrew Sutton
+Copyright (c) 2009 Helge Bahmann
+Copyright (c) 2009 Phil Endecott
+Copyright (c) 2010 Artyom Beilis
+Copyright (c) 2010 Bryce Lelbach
+Copyright (c) 2010 Helge Bahmann
+Copyright (c) 2010 Thomas Heller
+Copyright (c) 2010 Tim Blechmann
+Copyright (c) 2011 Bryce Lelbach
+Copyright (c) 2011 Helge Bahmann
+Copyright (c) 2011 Thomas Heller
+Copyright (c) 2011 Tim Blechmann
+Copyright (c) 2012 Artyom Beilis
+Copyright (c) 2012 Bruno Lalande
+Copyright (c) 2012 Paul Fultz II
+Copyright (c) 2012 Tim Blechmann
+Copyright (c) 2013 Agustin Berge
+Copyright (c) 2013 Bruno Lalande
+Copyright (c) 2013 Joaquim Duran
+Copyright (c) 2013 Kenneth L. Ho
+Copyright (c) 2013 Tim Blechmann
+Copyright (c) 2014 Agustin Berge
+Copyright (c) 2014 Ahmed Charles
+Copyright (c) 2014 Bruno Lalande
+Copyright (c) 2014 John Fletcher
+Copyright (c) 2014 Paul Fultz II
+Copyright (c) 2015 Artyom Beilis
+Copyright (c) 2015 Ion Gaztanaga
+Copyright (c) 2015 John Fletcher
+Copyright (c) 2015 Paul Fultz II
+Copyright (c) 2016 Barrett Adair
+Copyright (c) 2016 Paul Fultz II
+Copyright (c) 2018 Artyom Beilis
+Copyright (c) Aaron Windsor 2007
+Copyright (c) Chris Glover, 2016
+Copyright (c) Kevlin Henney 2001
+Copyright (c) Marshall Clow 2014
+Copyright (c) Marshall Clow 2017
+Copyright (c) Pablo Aguilar 2005
+Copyright (c) Vladimir Prus 2003
+Copyright 1991 Dieter Kraft, FHM
+Copyright 1997-2008 by Agner Fog
+Copyright 2002, 2009 Peter Dimov
+Copyright 2002, 2020 Peter Dimov
+Copyright 2002-2008 by Agner Fog
+Copyright 2002-2014 by Agner Fog
+Copyright 2004-2008 by Agner Fog
+Copyright 2004-2013 by Agner Fog
+Copyright 2005 Alexander Nasonov
+Copyright 2005, 2014 Peter Dimov
+Copyright 2005-2009 Daniel James
+Copyright 2005-2011 Daniel James
+Copyright 2005-2012 Daniel James
+Copyright 2005-2014 Daniel James
+Copyright 2006, 2020 Peter Dimov
+Copyright 2007 Christian Henning
+Copyright 2007, 2014 Peter Dimov
+Copyright 2007, 2019 Peter Dimov
+Copyright 2007, 2020 Peter Dimov
+Copyright 2008 Christian Henning
+Copyright 2008 Intel Corporation
+Copyright 2008, 2020 Peter Dimov
+Copyright 2009 Christian Henning
+Copyright 2010 Christian Henning
+Copyright 2010 Thomas Claveirole
+Copyright 2012 Christian Henning
+Copyright 2012 Olivier Tournaire
+Copyright 2012-2020 John Maddock
+Copyright 2013 Christian Henning
+Copyright 2013 Christian Shelton
+Copyright 2013 Cromwell D. Enage
+Copyright 2015, 2016 Peter Dimov
+Copyright 2015, 2019 Peter Dimov
+Copyright 2016, 2017 Peter Dimov
+Copyright 2017 James E. King III
+Copyright 2017, 2018 Peter Dimov
+Copyright 2017, 2019 Peter Dimov
+Copyright 2018, 2020 Peter Dimov
+Copyright 2019, 2020 Peter Dimov
+Copyright 2019-20 Madhur Chauhan
+Copyright Alexander Nasonov 2004
+Copyright Anne M. Archibald 2008
+Copyright Beman Dawes 2002, 2006
+Copyright Beman Dawes 2003, 2006
+Copyright Beman Dawes 2006, 2007
+Copyright Beman Dawes, 2002-2005
+Copyright Christopher Brown 2013
+Copyright Cromwell D. Enage 2013
+Copyright Cromwell D. Enage 2017
+Copyright Cromwell D. Enage 2018
+Copyright Cromwell D. Enage 2019
+Copyright Jason Rhinelander 2016
+Copyright John Maddock 2005-2006
+Copyright John Maddock 2005-2008
+Copyright Louis Dionne 2013-2017
+Copyright Nicholas Thompson 2018
+Copyright Nikhar Agrawal 2013-14
+Copyright Paul A. Bristow 2006-7
+Copyright Peter Dimov 2017, 2018
+Copyright Thorsten Ottosen, 2009
+copyright Louis Dionne 2013-2016
+copyright Louis Dionne 2013-2017
+(c) Copyright 2006 Douglas Gregor
+(c) Copyright 2009 Eric Bose-Wolf
+(c) Copyright 2013 Ruslan Baratov
+(c) Copyright Anton Bikineev 2014
+(c) Copyright David Abrahams 2000
+(c) Copyright David Abrahams 2001
+(c) Copyright David Abrahams 2002
+(c) Copyright David Abrahams 2003
+(c) Copyright David Abrahams 2004
+(c) Copyright Douglas Gregor 2001
+(c) Copyright Douglas Gregor 2002
+(c) Copyright Douglas Gregor 2010
+(c) Copyright Howard Hinnant 2004
+(c) Copyright Joel de Guzman 2003
+(c) Copyright John Maddock 2001-8
+(c) Copyright John Maddock 2006-7
+(c) Copyright John Maddock 2006-8
+(c) Copyright Juergen Hunold 2008
+(c) Copyright Roland Richter 2003
+(c) Copyright Stefan Slapeta 2004
+(c) Copyright Stephen Cleary 2000
+Copyright (c) 2000 David Abrahams
+Copyright (c) 2000 Stephen Cleary
+Copyright (c) 2001 David Abrahams
+Copyright (c) 2002 David Abrahams
+Copyright (c) 2002 Joel de Guzman
+Copyright (c) 2003 David Abrahams
+Copyright (c) 2003 Hartmut Kaiser
+Copyright (c) 2003 Howard Hinnant
+Copyright (c) 2003 Joel de Guzman
+Copyright (c) 2004 Hartmut Kaiser
+Copyright (c) 2004 Joel de Guzman
+Copyright (c) 2004 Ralf Mattethat
+Copyright (c) 2005 Douglas Gregor
+Copyright (c) 2005 Igor Chesnokov
+Copyright (c) 2006 Douglas Gregor
+Copyright (c) 2006 Piotr Wyderski
+Copyright (c) 2006 Xiaogang Zhang
+Copyright (c) 2006-7 John Maddock
+Copyright (c) 2007 Douglas Gregor
+Copyright (c) 2007 Hartmut Kaiser
+Copyright (c) 2007 Joel de Guzman
+Copyright (c) 2008 Michael Marcin
+Copyright (c) 2009 Chris Hoeppler
+Copyright (c) 2009 Francois Barel
+Copyright (c) 2009 Gunter Winkler
+Copyright (c) 2009 Hartmut Kaiser
+Copyright (c) 2009 Pauli Virtanen
+Copyright (c) 2009 Sebastian Redl
+Copyright (c) 2009, Motorola, Inc
+Copyright (c) 2010 Alfredo Correa
+Copyright (c) 2011 ! Brandon Kohn
+Copyright (c) 2011 Hartmut Kaiser
+Copyright (c) 2011 Thomas Bernard
+Copyright (c) 2012 Hartmut Kaiser
+Copyright (c) 2012 Martin Raspaud
+Copyright (c) 2012, Michele Caini
+Copyright (c) 2013 Anton Bikineev
+Copyright (c) 2013 Mateusz Loskot
+Copyright (c) 2013 Pauli Virtanen
+Copyright (c) 2013 Sebastian Redl
+Copyright (c) 2014 Erik Erlandson
+Copyright (c) 2014 Glen Fernandes
+Copyright (c) 2014 Joel de Guzman
+Copyright (c) 2014 Oliver Kowalke
+Copyright (c) 2014 Thomas Bernard
+Copyright (c) 2015 Sebastian Redl
+Copyright (c) 2016 Norbert Wenzel
+Copyright (c) 2016-2018 ERGO-Code
+Copyright (c) 2016-2019 ERGO-Code
+Copyright (c) 2017 Daniela Engert
+Copyright (c) 2018 Alain Miniussi
+Copyright (c) 2018 Evgeny Shulgin
+Copyright (c) 2018 Sergei Fedorov
+Copyright (c) 2018 Stefan Seefeld
+Copyright (c) 2018-2019 ERGO-Code
+Copyright (c) 2018-2021 ERGO-Code
+Copyright (c) 2019 Joel de Guzman
+Copyright (c) 2020 Nikita Kniazev
+Copyright (c) David Abrahams 2001
+Copyright (c) Douglas Gregor 2004
+Copyright (c) Douglas Gregor 2008
+Copyright 2001 Indiana University
+Copyright 2002 Indiana University
+Copyright 2006-2007 Boris Gubenko
+Copyright 2007 Alexandre Courpron
+Copyright 2007-2008 CodeRage, LLC
+Copyright 2007-2012 Ion Gaztanaga
+Copyright 2011 -2013 John Maddock
+Copyright 2011 Paul A. Bristow To
+Copyright 2017 James E. King, III
+Copyright Barrett Adair 2015-2017
+Copyright Barrett Adair 2015-2018
+Copyright Barrett Adair 2016-2017
+Copyright Dave Abrahams 2001-2002
+Copyright Eric Friedman 2002-2003
+Copyright James E. King III, 2017
+Copyright John Maddock 2006, 2007
+Copyright John Maddock 2006, 2010
+Copyright John Maddock 2006, 2011
+Copyright John Maddock 2006, 2012
+Copyright John Maddock 2007, 2014
+Copyright John Maddock 2008, 2012
+Copyright John Maddock 2010, 2012
+Copyright Paul Bristow 2006, 2007
+Copyright Paul Bristow 2007, 2011
+Copyright Thijs van den Berg 2014
+Copyright Vladimir Prus 2002-2004
+(c) Copyright 2004 Pavel Vozenilek
+(c) Copyright 2005 Matthias Troyer
+(c) Copyright 2007 Matthias Troyer
+(c) Copyright 2008 Matthias Troyer
+(c) Copyright 2013 Andrey Semashev
+(c) Copyright 2016 Raffi Enficiaud
+(c) Copyright 2017 Andrey Semashev
+(c) Copyright Andrey Semashev 2017
+(c) Copyright Antony Polukhin 2013
+(c) Copyright Antony Polukhin 2014
+(c) Copyright Craig Henderson 2002
+(c) Copyright Dustin Spicuzza 2009
+(c) Copyright Ignacy Gawedzki 2010
+(c) Copyright Jonathan Graehl 2004
+(c) Copyright Paul A. Bristow 2006
+(c) Copyright Paul A. Bristow 2011
+(c) Copyright Paul Mensonides 2002
+(c) Copyright Paul Mensonides 2003
+(c) Copyright Paul Mensonides 2005
+(c) Copyright Paul Mensonides 2011
+(c) Copyright Paul Mensonides 2012
+(c) Copyright Raffi Enficiaud 2017
+(c) Copyright Raffi Enficiaud 2018
+(c) Copyright Raffi Enficiaud 2019
+Copyright (c) 1995, Gerald Evenden
+Copyright (c) 2002 Travis Oliphant
+Copyright (c) 2003 Paul Mensonides
+Copyright (c) 2003-2008 Jan Gaspar
+Copyright (c) 2005-2007 Peder Holt
+Copyright (c) 2006 Steven Watanabe
+Copyright (c) 2006-2008 Johan Rade
+Copyright (c) 2007 Alexey Baskakov
+Copyright (c) 2007 Matthias Troyer
+Copyright (c) 2008 Frank Mori Hess
+Copyright (c) 2008 Steven Watanabe
+Copyright (c) 2008-2009 Ben Hanson
+Copyright (c) 2009 Boris Schaeling
+Copyright (c) 2009 Frank Mori Hess
+Copyright (c) 2009 Steven Watanabe
+Copyright (c) 2009, Gunter Winkler
+Copyright (c) 2009, Marco Guazzone
+Copyright (c) 2010 Paul A. Bristow
+Copyright (c) 2011 Emil Dotchevski
+Copyright (c) 2011 Julio Hoffimann
+Copyright (c) 2011 Paul A. Bristow
+Copyright (c) 2011 Steven Watanabe
+Copyright (c) 2012 Boris Schaeling
+Copyright (c) 2012 Kohei Takahashi
+Copyright (c) 2012 Paul A. Bristow
+Copyright (c) 2013 Antony Polukhin
+Copyright (c) 2013 Paul A. Bristow
+Copyright (c) 2014 Andrey Semashev
+Copyright (c) 2014 Christoph Weiss
+Copyright (c) 2014 Kohei Takahashi
+Copyright (c) 2015 Andrey Semashev
+Copyright (c) 2015 Kohei Takahashi
+Copyright (c) 2016 Kohei Takahashi
+Copyright (c) 2017 Andrey Semashev
+Copyright (c) 2017 Kohei Takahashi
+Copyright (c) 2017-2018 Chris Beck
+Copyright (c) 2018 Andrey Semashev
+Copyright (c) 2018 Kohei Takahashi
+Copyright (c) 2018, Quansight-Labs
+Copyright (c) 2018-2019 Cem Bassoy
+Copyright (c) 2019 Andrey Semashev
+Copyright (c) 2019-2020 Peter Bell
+Copyright (c) 2020 Alexander Grund
+Copyright (c) 2020 Andrey Semashev
+Copyright (c) Andrey Semashev 2017
+Copyright (c) Pauli Virtanen, 2010
+Copyright 2002, 2005 Daryle Walker
+Copyright 2003 Guillaume Melquiond
+Copyright 2005 Guillaume Melquiond
+Copyright 2007 Stanford University
+Copyright 2009-2011 Karsten Ahnert
+Copyright 2009-2011 Mario Mulansky
+Copyright 2009-2012 Karsten Ahnert
+Copyright 2009-2012 Mario Mulansky
+Copyright 2009-2013 Karsten Ahnert
+Copyright 2009-2013 Mario Mulansky
+Copyright 2009-2015 Mario Mulansky
+Copyright 2010-2011 Karsten Ahnert
+Copyright 2010-2011 Mario Mulansky
+Copyright 2010-2012 Karsten Ahnert
+Copyright 2010-2012 Mario Mulansky
+Copyright 2010-2013 Karsten Ahnert
+Copyright 2010-2013 Mario Mulansky
+Copyright 2010-2014 Mario Mulansky
+Copyright 2010-2015 Mario Mulansky
+Copyright 2011 - 2013 John Maddock
+Copyright 2011-2012 Karsten Ahnert
+Copyright 2011-2012 Mario Mulansky
+Copyright 2011-2013 Karsten Ahnert
+Copyright 2011-2013 Mario Mulansky
+Copyright 2011-2015 Mario Mulansky
+Copyright 2012-2013 Karsten Ahnert
+Copyright 2012-2013 Mario Mulansky
+Copyright 2012-2015 Mario Mulansky
+Copyright 2013-2014 Karsten Ahnert
+Copyright 2013-2014 Mario Mulansky
+Copyright 2015 Jon Lund Steffensen
+Copyright 2015 Klemens Morgenstern
+Copyright 2015-2016 Hans Dembinski
+Copyright 2015-2017 Hans Dembinski
+Copyright 2015-2018 Hans Dembinski
+Copyright 2015-2019 Hans Dembinski
+Copyright 2016 Klemens Morgenstern
+Copyright 2017 Two Blue Cubes Ltd.
+Copyright 2018-2019 Hans Dembinski
+Copyright 2019 Przemyslaw Bartosik
+Copyright Christoper Kohlhoff 2007
+Copyright David Abrahams 2000-2002
+Copyright David Abrahams 2001-2002
+Copyright David Abrahams 2002-2003
+Copyright David Abrahams 2003-2004
+Copyright Douglas Gregor 2001-2003
+Copyright Douglas Gregor 2001-2004
+Copyright Douglas Gregor 2001-2006
+Copyright Douglas Gregor 2002-2003
+Copyright Douglas Gregor 2002-2004
+Copyright Gottfried Ganssauge 2003
+Copyright Howard Hinnant 2007-2010
+Copyright Kevlin Henney, 2000-2005
+Copyright Michael Drexl 2005, 2006
+Copyright Sebastian Ramacher, 2007
+Copyright Thijs van den Berg, 2008
+(c) Copyright 2007 Anthony Williams
+(c) Copyright 2008 Anthony Williams
+(c) Copyright Aleksey Gurtovoy 2002
+(c) Copyright Aleksey Gurtovoy 2003
+(c) Copyright Beman Dawes 1995-2001
+(c) Copyright Beman Dawes 1999-2003
+(c) Copyright Daniel Frey 2002-2017
+(c) Copyright Herve Bronnimann 2004
+(c) Copyright Jeremy Siek 1999-2001
+(c) Copyright Jessica Hamilton 2014
+(c) Copyright Matthias Troyerk 2006
+(c) Copyright Peter Dimov 2004-2005
+(c) Copyright Reimar Doffinger 2018
+(c) Copyright Thorsten Ottosen 2005
+Copyright (c) 1988 by Theo Jurriens
+Copyright (c) 1993-2019 C.B. Barber
+Copyright (c) 2000, Frank Warmerdam
+Copyright (c) 2001 Daniel C. Nuffer
+Copyright (c) 2001-2003 Mac Murrett
+Copyright (c) 2001-2005 Peter Dimov
+Copyright (c) 2001-2008 Peter Dimov
+Copyright (c) 2002, Frank Warmerdam
+Copyright (c) 2003-2005 Peter Dimov
+Copyright (c) 2004 Arkadiy Vertleyb
+Copyright (c) 2005 Arkadiy Vertleyb
+Copyright (c) 2005-2006 Dan Marsden
+Copyright (c) 2005-2007 Dan Marsden
+Copyright (c) 2006 Arkadiy Vertleyb
+Copyright (c) 2006 Tobias Schwinger
+Copyright (c) 2007 Tobias Schwinger
+Copyright (c) 2012 Anthony Williams
+Copyright (c) 2012 Lorenzo Caminiti
+Copyright (c) 2013-2014 Damien Buhl
+Copyright (c) 2016 K. Noel Belcourt
+Copyright (c) 2019 T. Zachary Laine
+Copyright (c) Benjamin Sobotta 2012
+Copyright (c) Jeremy Siek 2001-2003
+Copyright (c) T. Zachary Laine 2018
+Copyright 2002 H Lohninger, TU Wein
+Copyright 2003-2008 Joaquin M Lopez
+Copyright 2003-2013 Joaquin M Lopez
+Copyright 2003-2014 Joaquin M Lopez
+Copyright 2003-2015 Joaquin M Lopez
+Copyright 2003-2016 Joaquin M Lopez
+Copyright 2003-2017 Joaquin M Lopez
+Copyright 2003-2018 Joaquin M Lopez
+Copyright 2003-2019 Joaquin M Lopez
+Copyright 2003-2020 Joaquin M Lopez
+Copyright 2006-2008 Joaquin M Lopez
+Copyright 2006-2009 Joaquin M Lopez
+Copyright 2006-2011 Joaquin M Lopez
+Copyright 2006-2013 Joaquin M Lopez
+Copyright 2006-2014 Joaquin M Lopez
+Copyright 2006-2015 Joaquin M Lopez
+Copyright 2006-2018 Joaquin M Lopez
+Copyright 2006-2019 Joaquin M Lopez
+Copyright 2006-2020 Joaquin M Lopez
+Copyright 2008 Andreas Huber Doenni
+Copyright 2008-2009 Frank Mori Hess
+Copyright 2008-2010 Gordon Woodhull
+Copyright 2011-2012 Steven Watanabe
+Copyright 2012-2013 Steven Watanabe
+Copyright 2012-2020 Antony Polukhin
+Copyright 2013 University of Warsaw
+Copyright 2013-2020 Antony Polukhin
+Copyright 2015-2018 Andrey Semashev
+Copyright 2015-2019 Antony Polukhin
+Copyright 2015-2020 Antony Polukhin
+Copyright 2016-2017 Joaquin M Lopez
+Copyright 2016-2018 Andrey Semashev
+Copyright 2016-2018 Joaquin M Lopez
+Copyright 2016-2019 Antony Polukhin
+Copyright 2016-2019 Joaquin M Lopez
+Copyright 2016-2020 Joaquin M Lopez
+Copyright 2017, NVIDIA CORPORATION.
+Copyright 2017-2018 Joaquin M Lopez
+Copyright 2018-2019 Antony Polukhin
+Copyright 2019-2020 Antony Polukhin
+Copyright Eric Niebler 2013-present
+Copyright Frank Mori Hess 2007,2009
+Copyright Frank Mori Hess 2007-2008
+Copyright Frank Mori Hess 2007-2009
+Copyright Frank Mori Hess 2007-2010
+Copyright John R. Bandela 2000-2002
+Copyright Kohei Takahashi 2012-2014
+Copyright Paul A. Bristow 2006-2011
+Copyright Shunsuke Sogame 2005-2006
+Copyright Steven Watanabe 2009-2011
+Copyright Steven Watanabe 2010-2011
+(c) Copyright 2002, 2003 Beman Dawes
+(c) Copyright 2002-4 Pavel Vozenilek
+(c) Copyright 2016 Ashish Sadanandan
+(c) Copyright Eric Niebler 2004-2005
+(c) Copyright Gennadiy Rozental 2001
+(c) Copyright Hubert Holin 2003-2005
+(c) Copyright Jeremiah Willcock 2004
+(c) Copyright John Maddock 2005-2006
+(c) Copyright Jonathan Turkanis 2003
+(c) Copyright Jonathan Turkanis 2004
+(c) Copyright Markus Schoepflin 2005
+(c) Copyright Markus Schoepflin 2007
+(c) Copyright Michael Glassford 2004
+(c) Copyright Peter Dimov 2001, 2002
+(c) Copyright Rani Sharoni 2003-2005
+(c) Copyright Thomas Claveirole 2010
+(c) Copyright Yuriy Krasnoschek 2009
+Copyright (c) 1998-2002 John Maddock
+Copyright (c) 1998-2004 John Maddock
+Copyright (c) 1998-2005 John Maddock
+Copyright (c) 1998-2009 John Maddock
+Copyright (c) 1999-2003 Jaakko Jarvi
+Copyright (c) 2001 Alexander Peslyak
+Copyright (c) 2001, 2002 Peter Dimov
+Copyright (c) 2001, Daniel C. Nuffer
+Copyright (c) 2001-2003 John Maddock
+Copyright (c) 2002, 2003 Peter Dimov
+Copyright (c) 2002-2003 Martin Wille
+Copyright (c) 2003 Gerald I. Evenden
+Copyright (c) 2003-2005 John Maddock
+Copyright (c) 2004 Gerald I. Evenden
+Copyright (c) 2005 Matthew Calabrese
+Copyright (c) 2005-2008 Daniel James
+Copyright (c) 2005-2009 Jongsoo Park
+Copyright (c) 2005-2011 Daniel James
+Copyright (c) 2005-2016 Daniel James
+Copyright (c) 2007 Cybozu Labs, Inc.
+Copyright (c) 2007 Marcin Kalicinski
+Copyright (c) 2007, 2008 Peter Dimov
+Copyright (c) 2007, 2013 Peter Dimov
+Copyright (c) 2007, 2014 Peter Dimov
+Copyright (c) 2007, Tobias Schwinger
+Copyright (c) 2008 Gerald I. Evenden
+Copyright (c) 2008, 2009 Peter Dimov
+Copyright (c) 2008, 2011 Peter Dimov
+Copyright (c) 2008, 2018 Peter Dimov
+Copyright (c) 2008-2011 Daniel James
+Copyright (c) 2008-2016 Daniel James
+Copyright (c) 2009, 2015 Peter Dimov
+Copyright (c) 2010-2011 David Bellot
+Copyright (c) 2011-2013 Andrew Hundt
+Copyright (c) 2013 Tim Blechmann ARM
+Copyright (c) 2015-2019 Vinnie Falco
+Copyright (c) 2016-2019 Damian Jarek
+Copyright (c) 2016-2019 Vinnie Falco
+Copyright (c) 2017 James E. King III
+Copyright (c) 2018 James E. King III
+Copyright (c) 2020 Michael Feldmeier
+Copyright (c) Christof Meerwald 2003
+Copyright (c) Damian Eads, 2007-2008
+Copyright (c) Intel Corporation 2008
+Copyright 1999-2003 Aleksey Gurtovoy
+Copyright 2011, 2012 Paul A. Bristow
+Copyright 2011-2013 Thorsten Ottosen
+Copyright 2013 Christopher Kormanyos
+Copyright 2013, 2017 Andrey Semashev
+Copyright 2013, 2017-2018 Cray, Inc.
+Copyright 2014 Christopher Kormanyos
+Copyright 2015, 2017 Andrey Semashev
+Copyright 2015, 2020 Andrey Semashev
+Copyright 2016, 2017 Andrey Semashev
+Copyright 2018, 2019 Andrey Semashev
+Copyright Aleksey Gurtovoy 2000-2002
+Copyright Aleksey Gurtovoy 2000-2003
+Copyright Aleksey Gurtovoy 2000-2004
+Copyright Aleksey Gurtovoy 2000-2006
+Copyright Aleksey Gurtovoy 2000-2008
+Copyright Aleksey Gurtovoy 2000-2009
+Copyright Aleksey Gurtovoy 2000-2010
+Copyright Aleksey Gurtovoy 2001-2004
+Copyright Aleksey Gurtovoy 2001-2006
+Copyright Aleksey Gurtovoy 2001-2007
+Copyright Aleksey Gurtovoy 2001-2008
+Copyright Aleksey Gurtovoy 2002-2004
+Copyright Aleksey Gurtovoy 2002-2006
+Copyright Aleksey Gurtovoy 2003-2004
+Copyright Aleksey Gurtovoy 2003-2007
+Copyright Andrii Sydorchuk 2010-2012
+Copyright Antony Polukhin, 2011-2020
+Copyright Antony Polukhin, 2013-2014
+Copyright Antony Polukhin, 2013-2020
+Copyright Antony Polukhin, 2016-2019
+Copyright Antony Polukhin, 2016-2020
+Copyright Christopher Kormanyos 2013
+Copyright Christopher Kormanyos 2014
+Copyright Matthew Pulver 2018 - 2019
+Copyright Paul A. Bristow 2006, 2007
+Copyright Paul A. Bristow 2007, 2009
+Copyright Paul A. Bristow 2007, 2010
+Copyright Paul A. Bristow 2007, 2012
+Copyright Paul A. Bristow 2008, 2009
+Copyright Paul A. Bristow 2008, 2010
+Copyright Paul A. Bristow 2008, 2014
+Copyright Paul A. Bristow 2009, 2011
+Copyright Paul A. Bristow 2011, 2012
+Copyright Steven J. Ross 2001 - 2009
+Copyright Steven J. Ross 2001 - 2014
+Copyright Thorsten Ottosen 2003-2004
+Copyright Thorsten Ottosen 2003-2005
+Copyright Thorsten Ottosen 2003-2006
+Copyright Thorsten Ottosen 2003-2007
+Copyright Thorsten Ottosen 2003-2008
+copyright 2004 Brian Ravnsgaard Riis
+(c) Copyright 2005-7 Anthony Williams
+(c) Copyright 2005-8 Anthony Williams
+(c) Copyright 2006-7 Anthony Williams
+(c) Copyright 2006-8 Anthony Williams
+(c) Copyright 2007-2009 Andrew Sutton
+(c) Copyright 2007-8 Anthony Williams
+(c) Copyright 2007-9 Anthony Williams
+(c) Copyright 2008-9 Anthony Williams
+(c) Copyright 2009-2011 Frederic Bron
+(c) Copyright Beman Dawes 2001 - 2003
+(c) Copyright Beman Dawes 2002 - 2003
+(c) Copyright Darin Adler 2001 - 2002
+(c) Copyright Daryle Walker 2000-2001
+(c) Copyright Daryle Walker 2001-2002
+(c) Copyright Edward Diener 2011,2012
+(c) Copyright Edward Diener 2011,2013
+(c) Copyright Edward Diener 2011,2014
+(c) Copyright Edward Diener 2011-2015
+(c) Copyright Edward Diener 2011-2020
+(c) Copyright Edward Diener 2012,2013
+(c) Copyright Edward Diener 2014,2019
+(c) Copyright Eric Friedman 2002-2003
+(c) Copyright Ion Gaztanaga 2004-2015
+(c) Copyright Ion Gaztanaga 2005-2012
+(c) Copyright Ion Gaztanaga 2005-2013
+(c) Copyright Ion Gaztanaga 2005-2014
+(c) Copyright Ion Gaztanaga 2005-2015
+(c) Copyright Ion Gaztanaga 2005-2016
+(c) Copyright Ion Gaztanaga 2006-2012
+(c) Copyright Ion Gaztanaga 2006-2013
+(c) Copyright Ion Gaztanaga 2006-2014
+(c) Copyright Ion Gaztanaga 2006-2015
+(c) Copyright Ion Gaztanaga 2007-2012
+(c) Copyright Ion Gaztanaga 2007-2013
+(c) Copyright Ion Gaztanaga 2007-2014
+(c) Copyright Ion Gaztanaga 2008-2012
+(c) Copyright Ion Gaztanaga 2008-2013
+(c) Copyright Ion Gaztanaga 2008-2015
+(c) Copyright Ion Gaztanaga 2009-2012
+(c) Copyright Ion Gaztanaga 2009-2013
+(c) Copyright Ion Gaztanaga 2010-2012
+(c) Copyright Ion Gaztanaga 2010-2013
+(c) Copyright Ion Gaztanaga 2010-2016
+(c) Copyright Ion Gaztanaga 2011-2012
+(c) Copyright Ion Gaztanaga 2011-2013
+(c) Copyright Ion Gaztanaga 2011-2014
+(c) Copyright Ion Gaztanaga 2012-2012
+(c) Copyright Ion Gaztanaga 2012-2013
+(c) Copyright Ion Gaztanaga 2012-2015
+(c) Copyright Ion Gaztanaga 2012-2016
+(c) Copyright Ion Gaztanaga 2013-2013
+(c) Copyright Ion Gaztanaga 2013-2014
+(c) Copyright Ion Gaztanaga 2014-2014
+(c) Copyright Ion Gaztanaga 2014-2015
+(c) Copyright Ion Gaztanaga 2014-2017
+(c) Copyright Ion Gaztanaga 2015-2015
+(c) Copyright Ion Gaztanaga 2015-2016
+(c) Copyright Ion Gaztanaga 2015-2017
+(c) Copyright Ion Gaztanaga 2016-2016
+(c) Copyright Ion Gaztanaga 2017-2017
+(c) Copyright Ion Gaztanaga 2017-2018
+(c) Copyright Ion Gaztanaga 2018-2018
+(c) Copyright Ion Gaztanaga 2019-2020
+(c) Copyright Jens Maurer 2001 - 2002
+(c) Copyright Jens Maurer 2001 - 2003
+(c) Copyright Jens Maurer 2002 - 2003
+(c) Copyright John Maddock 2006, 2015
+(c) Copyright Toon Knapen 2001 - 2003
+Copyright (c) 2001-2003 Daniel Nuffer
+Copyright (c) 2002 Raghavendra Satish
+Copyright (c) 2002-2003 Eric Friedman
+Copyright (c) 2003-2004 Gennaro Prota
+Copyright (c) 2004 Kristopher Beevers
+Copyright (c) 2005, 2014 Eric Niebler
+Copyright (c) 2005-2006 Joao Abecasis
+Copyright (c) 2006, Stephan Diederich
+Copyright (c) 2007 - Sebastien Fabbro
+Copyright (c) 2007, 2008, Damian Eads
+Copyright (c) 2007, 2013 John Maddock
+Copyright (c) 2007-8 Anthony Williams
+Copyright (c) 2007-9 Anthony Williams
+Copyright (c) 2008-2011 Bruno Lalande
+Copyright (c) 2008-2012 Bruno Lalande
+Copyright (c) 2008-2013 Bruno Lalande
+Copyright (c) 2008-2013 Tim Blechmann
+Copyright (c) 2008-2014 Bruno Lalande
+Copyright (c) 2008-2015 Bruno Lalande
+Copyright (c) 2008-2016 Tim Blechmann
+Copyright (c) 2008-2017 Bruno Lalande
+Copyright (c) 2009-2011 Artyom Beilis
+Copyright (c) 2009-2013 Tim Blechmann
+Copyright (c) 2010-2011 Bryce Lelbach
+Copyright (c) 2010-2011 Thomas Heller
+Copyright (c) 2010-2011 Tim Blechmann
+Copyright (c) 2011 Jan Frederick Eick
+Copyright (c) 2011 Paul A. Bristow To
+Copyright (c) 2011-2012 Bruno Lalande
+Copyright (c) 2012-2014 Bruno Lalande
+Copyright (c) 2013-2014 Agustin Berge
+Copyright (c) 2013-2014 Ion Gaztanaga
+Copyright (c) 2014 Mathjax Consortium
+Copyright (c) 2014-2015 Bruno Lalande
+Copyright (c) 2014-2015 John Fletcher
+Copyright (c) 2015-2017 Martin Hensel
+Copyright (c) 2016 2017 Felix Lenders
+Copyright (c) 2019 Max-Planck-Society
+Copyright (c) Marshall Clow 2008-2012
+Copyright (c) Marshall Clow 2010-2012
+Copyright (c) Marshall Clow 2011-2012
+Copyright (c) Marshall Clow 2012-2012
+Copyright (c) Marshall Clow 2012-2015
+Copyright 2007-2008 Christian Henning
+Copyright 2016 Klemens D. Morgenstern
+Copyright 2017 Valentin Noah Hartmann
+Copyright Andrey Semashev 2007 - 2013
+Copyright Andrey Semashev 2007 - 2014
+Copyright Andrey Semashev 2007 - 2015
+Copyright Andrey Semashev 2007 - 2016
+Copyright Andrey Semashev 2018 - 2020
+Copyright Beman Dawes 1994-2007, 2011
+Copyright Beman Dawes 2002-2005, 2009
+copyright Gonzalo Brito Gadeschi 2015
+(c) Copyright 2007-10 Anthony Williams
+(c) Copyright 2008-10 Anthony Williams
+(c) Copyright Benedek Thaler 2015-2016
+(c) Copyright Daryle Walker 2001, 2006
+(c) Copyright Guillaume Melquiond 2003
+(c) Copyright Howard Hinnant 2007-2010
+(c) Copyright John Maddock 2001 - 2002
+(c) Copyright John Maddock 2001 - 2003
+(c) Copyright John Maddock 2002 - 2003
+(c) Copyright Nicolai M. Josuttis 2001
+(c) Copyright Olaf Krzikalla 2004-2006
+(c) Copyright Vicente J. Botet Escriba
+(c) Rasmus Munk Larsen, Stanford, 2004
+Copyright (c) 1998-2003 Joel de Guzman
+Copyright (c) 1998-2008 Joel de Guzman
+Copyright (c) 2001-2002 Joel de Guzman
+Copyright (c) 2001-2003 Hartmut Kaiser
+Copyright (c) 2001-2003 Joel de Guzman
+Copyright (c) 2001-2007 Hartmut Kaiser
+Copyright (c) 2001-2007 Joel de Guzman
+Copyright (c) 2001-2008 Hartmut Kaiser
+Copyright (c) 2001-2008 Joel de Guzman
+Copyright (c) 2001-2009 Joel de Guzman
+Copyright (c) 2001-2010 Hartmut Kaiser
+Copyright (c) 2001-2010 Joel de Guzman
+Copyright (c) 2001-2011 Hartmut Kaiser
+Copyright (c) 2001-2011 Joel de Guzman
+Copyright (c) 2001-2011 Thomas Bernard
+Copyright (c) 2001-2012 Hartmut Kaiser
+Copyright (c) 2001-2012 Joel de Guzman
+Copyright (c) 2001-2013 Hartmut Kaiser
+Copyright (c) 2001-2013 Joel de Guzman
+Copyright (c) 2001-2014 Joel de Guzman
+Copyright (c) 2001-2015 Joel de Guzman
+Copyright (c) 2001-2019 Joel de Guzman
+Copyright (c) 2002-2003 David Abrahams
+Copyright (c) 2002-2003 Hartmut Kaiser
+Copyright (c) 2002-2003 Joel de Guzman
+Copyright (c) 2002-2006 Hartmut Kaiser
+Copyright (c) 2004 Jonathan Brandmeyer
+Copyright (c) 2005-2006 Alain Miniussi
+Copyright (c) 2005-2006 Douglas Gregor
+Copyright (c) 2005-2008 Hartmut Kaiser
+Copyright (c) 2005-2010 Joel de Guzman
+Copyright (c) 2005-2011 Joel de Guzman
+Copyright (c) 2005-2012 Joel de Guzman
+Copyright (c) 2005-2013 Joel de Guzman
+Copyright (c) 2007-2011 Hartmut Kaiser
+Copyright (c) 2008, 2016 Tim Blechmann
+Copyright (c) 2008-2011 Hartmut Kaiser
+Copyright (c) 2009 Christopher Schmidt
+Copyright (c) 2009, 2011 Helge Bahmann
+Copyright (c) 2009, 2016 Tim Blechmann
+Copyright (c) 2009-2010 Hartmut Kaiser
+Copyright (c) 2009-2020 Vladimir Batov
+Copyright (c) 2010 Christopher Schmidt
+Copyright (c) 2011, 2016 Tim Blechmann
+Copyright (c) 2011-2012 ! Brandon Kohn
+Copyright (c) 2011-2012 Thomas Bernard
+Copyright (c) 2012, Jaydeep P. Bardhan
+Copyright (c) 2012, Matthew G. Knepley
+Copyright (c) 2014 Riccardo Marcangelo
+Copyright (c) 2014, Janani Padmanabhan
+Copyright (c) 2015 Andrzej Krzemienski
+Copyright (c) 2016 Andrzej Krzemienski
+Copyright (c) 2016-2019 Viktor Kirilov
+Copyright (c) 2017 Andrzej Krzemienski
+Copyright (c) 2020 Krystian Stasiowski
+Copyright (c) 2022 Two Blue Cubes Ltd.
+Copyright (c) Christopher Diggins 2005
+Copyright 2002, 2009, 2014 Peter Dimov
+Copyright 2004-2005 by Enthought, Inc.
+Copyright 2007 University of Karlsruhe
+Copyright 2015, 2017, 2019 Peter Dimov
+Copyright 2016, 2018, 2019 Peter Dimov
+Copyright Alexander Nasonov, 2006-2010
+Copyright Beman Dawes 1994, 2006, 2008
+Copyright Beman Dawes 2003, 2006, 2008
+Copyright Beman Dawes 2003, 2006, 2010
+Copyright Beman Dawes 2003, 2006, 2011
+Copyright Beman Dawes 2010, 2011, 2014
+Copyright John Maddock 2005-2006, 2011
+Copyright John Maddock 2006-7, 2013-14
+Copyright Peter Dimov 2017, 2018, 2020
+copyright 2008- s, The SciPy community
+(c) Copyright 2005-2006 Matthias Troyer
+(c) Copyright 2005-2007 Matthias Troyer
+(c) Copyright Boris Gubenko 2006 - 2007
+(c) Copyright Gennaro Prota 2003 - 2004
+(c) Copyright Paul Mensonides 2002-2011
+Copyright (c) 1989-2004 Johannes Braams
+Copyright (c) 1994 by Xerox Corporation
+Copyright (c) 1996-2008 Rice University
+Copyright (c) 1998-2000 Dr John Maddock
+Copyright (c) 2000, 2001 Stephen Cleary
+Copyright (c) 2001-2009, Hartmut Kaiser
+Copyright (c) 2005, 2006 Douglas Gregor
+Copyright (c) 2007-2008 Steven Watanabe
+Copyright (c) 2007-2009 Steven Watanabe
+Copyright (c) 2007-2010 Steven Watanabe
+Copyright (c) 2008-2009 Frank Mori Hess
+Copyright (c) 2009-2010, Marco Guazzone
+Copyright (c) 2009-2012, Marco Guazzone
+Copyright (c) 2010 Thomas P. Robitaille
+Copyright (c) 2011-2015 Akira Takahashi
+Copyright (c) 2011-2020 Antony Polukhin
+Copyright (c) 2012 Pieter Bastiaan Ober
+Copyright (c) 2012-2014 Kohei Takahashi
+Copyright (c) 2012-2020 Antony Polukhin
+Copyright (c) 2013-2020 Antony Polukhin
+Copyright (c) 2014 Pieter Bastiaan Ober
+Copyright (c) 2014, Andrzej Krzemienski
+Copyright (c) 2014,2018 Kohei Takahashi
+Copyright (c) 2014-2015 Kohei Takahashi
+Copyright (c) 2014-2020 Andrey Semashev
+Copyright (c) 2014-2020 Antony Polukhin
+Copyright (c) 2015-2020 Antony Polukhin
+Copyright (c) 2016-2020 Antony Polukhin
+Copyright (c) 2018-2020 Antony Polukhin
+Copyright (c) 2019-2020 Alexander Grund
+Copyright (c) 2019-2020 Antony Polukhin
+Copyright 2000 University of Notre Dame
+Copyright 2001 University of Notre Dame
+Copyright 2002-2003 Guillaume Melquiond
+Copyright 2009 Vicente J. Botet Escriba
+Copyright 2010 Vicente J. Botet Escriba
+Copyright 2011 Vicente J. Botet Escriba
+Copyright 2012 Vicente J. Botet Escriba
+Copyright 2019-20 Christopher Kormanyos
+Copyright Christopher Kormanyos 2013-14
+Copyright Paul A. Bristow 2007, 2013-14
+Copyright Ralf W. Grosse-Kunstleve 2006
+Copyright Vicente J. Botet Escriba 2009
+Copyright Vicente J. Botet Escriba 2010
+Copyright Vicente J. Botet Escriba 2012
+(c) Copyright 2007-2010 Anthony Williams
+(c) Copyright 2009-2012 Anthony Williams
+(c) Copyright 2013, 2020 Andrey Semashev
+(c) Copyright Christopher Jefferson 2011
+(c) Copyright David Abrahams 2001 - 2002
+(c) Copyright David Abrahams 2002 - 2003
+(c) Copyright Jeremy William Murphy 2015
+(c) Copyright Jeremy William Murphy 2016
+(c) Copyright Microsoft Corporation 2014
+(c) Copyright R.W. Grosse-Kunstleve 2002
+(c) Copyright Thorsten Ottosen 2002-2003
+Copyright (arg) 2001-2014 Joel de Guzman
+Copyright (c) 2001, 2002 Enthought, Inc.
+Copyright (c) 2001-2003 William E. Kempf
+Copyright (c) 2003, 2007-14 Matteo Frigo
+Copyright (c) 2003-2005 Peter J. Verveer
+Copyright (c) 2004-2008 Rene Nyffenegger
+Copyright (c) 2006-2007 Matias Capeletto
+Copyright (c) 2006-2007 Tobias Schwinger
+Copyright (c) 2007-2008 Tobias Schwinger
+Copyright (c) 2008 Federico J. Fernandez
+Copyright (c) 2008-2012 Simonson Lucanus
+Copyright (c) 2008-2018 Lorenzo Caminiti
+Copyright (c) 2008-2019 Lorenzo Caminiti
+Copyright (c) 2009-2012 Lorenzo Caminiti
+Copyright (c) 2010 Athanasios Iliopoulos
+Copyright (c) 2011 Christopher Jefferson
+Copyright (c) 2012-2012 Andrii Sydorchuk
+Copyright (c) 2013 Christopher Kormanyos
+Copyright (c) 2014, 2019 Andrey Semashev
+Copyright (c) 2014, 2020 Andrey Semashev
+Copyright (c) 2015 Agustin K-ballo Berge
+Copyright (c) 2016-2018 T. Zachary Laine
+Copyright (c) Microsoft Corporation 2014
+Copyright 2001, 2004, 2011 Daryle Walker
+Copyright 2002-2006 Andreas Huber Doenni
+Copyright 2002-2007 Andreas Huber Doenni
+Copyright 2002-2008 Andreas Huber Doenni
+Copyright 2002-2010 Andreas Huber Doenni
+Copyright 2002-2016 The SciPy Developers
+Copyright 2005-2006 Andreas Huber Doenni
+Copyright 2005-2008 Andreas Huber Doenni
+Copyright 2010-2012, D. E. Shaw Research
+Copyright 2012-2013 Andreas Angelopoulos
+Copyright Gottfried Ganssauge 2003..2006
+(c) Copyright 2003-2007 Jonathan Turkanis
+(c) Copyright 2004-2007 Jonathan Turkanis
+(c) Copyright 2005-2007 Jonathan Turkanis
+(c) Copyright Jonathan Turkanis 2004-2005
+(c) Copyright Samuli-Petrus Korhonen 2017
+CNRS/Univ. Clermont II Copyright 2014 LRI
+Copyright (c) 1999-2003 Jeremiah Willcock
+Copyright (c) 2001 by Andrei Alexandrescu
+Copyright (c) 2001-2009, 2012 Peter Dimov
+Copyright (c) 2002 by Andrei Alexandrescu
+Copyright (c) 2002-2006 Marcin Kalicinski
+Copyright (c) 2002-2007 Marcin Kalicinski
+Copyright (c) 2004, 2005 Arkadiy Vertleyb
+Copyright (c) 2005-2022, NumPy Developers
+Copyright (c) 2007-2009 Joachim Faulhaber
+Copyright (c) 2007-2010 Joachim Faulhaber
+Copyright (c) 2007-2011 Joachim Faulhaber
+Copyright (c) 2007-2012 Joachim Faulhaber
+Copyright (c) 2008-2009 Joachim Faulhaber
+Copyright (c) 2008-2010 Joachim Faulhaber
+Copyright (c) 2008-2011 Joachim Faulhaber
+Copyright (c) 2008-2012 Joachim Faulhaber
+Copyright (c) 2009-2009 Joachim Faulhaber
+Copyright (c) 2009-2010 Joachim Faulhaber
+Copyright (c) 2009-2011 Joachim Faulhaber
+Copyright (c) 2010-2010 Joachim Faulhaber
+Copyright (c) 2010-2011 Joachim Faulhaber
+Copyright (c) 2011-2011 Joachim Faulhaber
+Copyright (c) 2012 - 2014 Andrey Semashev
+Copyright (c) 2013 - 2014 Andrey Semashev
+Copyright (c) 2013 - 2020 Andrey Semashev
+Copyright (c) 2014, Athanasios Iliopoulos
+Copyright (c) 2016 Klemens D. Morgenstern
+Copyright (c) 2017 - 2018 Andrey Semashev
+Copyright (c) 2017 Klemens D. Morgenstern
+Copyright (c) 2018 Klemens D. Morgenstern
+Copyright (c) 2019 - 2020 Alexander Grund
+Copyright (c) 2019 Klemens D. Morgenstern
+Copyright 2006 Eric Niebler, Olivier Gygi
+Copyright 2006 Michael van der Westhuizen
+Copyright 2008 Adobe Systems Incorporated
+Copyright Arno Schoedl & Neil Groves 2009
+Copyright Kevlin Henney, 2000, 2001, 2002
+copyright (c) 1995-2010 Geodan, Amsterdam
+(c) Copyright 2011Vicente J. Botet Escriba
+(c) Copyright Aleksey Gurtovoy 2002 - 2003
+(c) Copyright Beman Dawes 2006, 2009, 2014
+(c) Copyright Edward Diener 2011,2012,2013
+(c) Copyright Edward Diener 2011,2012,2019
+(c) Copyright Edward Diener 2011-2015,2019
+(c) Copyright Edward Diener 2012,2013,2019
+(c) Copyright Peter Dimov 2001, 2002, 2003
+Copyright (c) 1994 Hewlett-Packard Company
+Copyright (c) 2000 Cadenza New Zealand Ltd
+Copyright (c) 2001, 2002, 2003 Peter Dimov
+Copyright (c) 2001, 2002, 2012 Peter Dimov
+Copyright (c) 2002, 2008, 2013 Peter Dimov
+Copyright (c) 2002, 2009, 2014 Peter Dimov
+Copyright (c) 2002, 2018, 2019 Peter Dimov
+Copyright (c) 2003, 2006 Gerald I. Evenden
+Copyright (c) 2005-2015, Michele Simionato
+Copyright (c) 2006, 2009 Marcin Kalicinski
+Copyright (c) 2006-2008 Alexander Chemeris
+Copyright (c) 2007, 2008, 2012 Peter Dimov
+Copyright (c) 2010-2019 Max-Planck-Society
+Copyright (c) 2010-2020 Max-Planck-Society
+Copyright (c) 2017, 2018 James E. King III
+Copyright 1984, 1995 by Stephen L. Moshier
+Copyright 1984, 1996 by Stephen L. Moshier
+Copyright 2005 Daniel Egloff, Eric Niebler
+Copyright 2005 Daniel Egloff, Olivier Gygi
+Copyright 2005 Eric Niebler, Daniel Egloff
+Copyright 2006 Daniel Egloff, Olivier Gygi
+Copyright 2006 Olivier Gygi, Daniel Egloff
+Copyright 2006, Eric Niebler, Olivier Gygi
+Copyright 2010 Daniel Wallin, Eric Niebler
+Copyright 2015-2018 Klemens D. Morgenstern
+Copyright Nick Thompson, John Maddock 2020
+Copyright Paul A. Bristow 2006, 2007, 2012
+Copyright Paul A. Bristow 2006, 2012, 2017
+Copyright Paul A. Bristow 2016, 2017, 2018
+Portions Copyright (c) 2002 David Abrahams
+(c) Copyright 2010 Vicente J. Botet Escriba
+(c) Copyright 2011 Vicente J. Botet Escriba
+(c) Copyright 2012 Vicente J. Botet Escriba
+(c) Copyright 2013 Vicente J. Botet Escriba
+(c) Copyright 2014 Vicente J. Botet Escriba
+(c) Copyright Eric Ford & Hubert Holin 2001
+(c) Copyright Eric Ford 2001 & Hubert Holin
+(c) Copyright Markus Schoepflin 2002 - 2003
+(c) Copyright Vicente J. Botet Escriba 2010
+(c) Copyright Vicente J. Botet Escriba 2014
+(c) Rasmus Munk Larsen, Stanford University
+Copyright (c) 1993-2019 The Geometry Center
+Copyright (c) 2003-2004, 2008 Gennaro Prota
+Copyright (c) 2003-2006, 2008 Gennaro Prota
+Copyright (c) 2009-2010 Christopher Schmidt
+Copyright (c) 2009-2011 Christopher Schmidt
+Copyright (c) 2010-2011 Christopher Schmidt
+Copyright (c) 2011 Vicente J. Botet Escriba
+Copyright (c) 2011-2013, 2016 Tim Blechmann
+Copyright (c) 2012 Vicente J. Botet Escriba
+Copyright (c) 2013 Vicente J. Botet Escriba
+Copyright (c) 2014 Vicente J. Botet Escriba
+Copyright (c) 2014-2016 Andrzej Krzemienski
+Copyright (c) 2015 Vicente J. Botet Escriba
+Copyright (c) 2015-2018 Andrzej Krzemienski
+Copyright (c) 2017 Vicente J. Botet Escriba
+Copyright (c) 2019-2020 Krystian Stasiowski
+Copyright 1984 - 1994 by Stephen L. Moshier
+Copyright 1985 by Stephen L. Moshier Direct
+Copyright 2002 Brad King and Douglas Gregor
+Copyright 2012 (c) Jeffrey Lee Hellrung, Jr
+Copyright Christopher Kormanyos 2002 - 2011
+Copyright Christopher Kormanyos 2002 - 2013
+(c) Rasmus Munk Larsen, Stanford, 1999, 2004
+Copyright (c) 2001-2011 - Scilab Enterprises
+Copyright (c) 2002 Eric Friedman, Itay Maman
+Copyright (c) 2002 Juan Carlos Arevalo-Baeza
+Copyright (c) 2003 Eric Friedman, Itay Maman
+Copyright (c) 2008, 2009, 2016 Tim Blechmann
+Copyright (c) 2010 - Jordi Gutierrez Hermoso
+Copyright (c) 2012 Barend Gehrels, Amsterdam
+Copyright (c) 2013 Barend Gehrels, Amsterdam
+Copyright (c) 2014 Barend Gehrels, Amsterdam
+Copyright (c) 2014, 2015 Andrzej Krzemienski
+Copyright (c) 2014,2015,2018 Kohei Takahashi
+Copyright (c) 2015 Barend Gehrels, Amsterdam
+Copyright (c) 2017 Barend Gehrels, Amsterdam
+Copyright (c) 2019 Barend Gehrels, Amsterdam
+Copyright (c) 2020 Barend Gehrels, Amsterdam
+Copyright 1997-2001 University of Notre Dame
+Copyright 2009-2010 Vicente J. Botet Escriba
+Copyright 2009-2011 Vicente J. Botet Escriba
+Copyright 2009-2012 Vicente J. Botet Escriba
+Copyright Beman Dawes and Daryle Walker 1999
+Copyright Daniel Wallin, David Abrahams 2005
+Copyright Daniel Wallin, David Abrahams 2010
+Copyright David Abrahams, Daniel Wallin 2003
+Copyright David Abrahams, Daniel Wallin 2005
+Copyright Thorsten Ottosen, Neil Groves 2006
+Copyright Vicente J. Botet Escriba 2009-2011
+(c) Copyright Guillaume Melquiond 2002 - 2003
+(c) Copyright Joaquin M Lopez Munoz 2006-2013
+Copyright (c) 2011-2014, The OpenBLAS Project
+Copyright (c) 2013-2014, 2020 Andrey Semashev
+Copyright (c) 2014 - 2018 Andrzej Krzemienski
+Copyright (c) 2014-2018, 2020 Andrey Semashev
+Copyright (c) 2015 - 2017 Andrzej Krzemienski
+Copyright 2000 Jeremy Siek (jsiek@lsc.nd.edu)
+Copyright 2005 Eric Niebler, Michael Gauckler
+Copyright 2005 Trustees of Indiana University
+Copyright 2006 Trustees of Indiana University
+Copyright 2009 Trustees of Indiana University
+Copyright David Abrahams and Jeremy Siek 2003
+Copyright John Maddock 2006, 2007, 2012, 2014
+Copyright Peter Dimov and David Abrahams 2002
+Copyright (c) 2004 CrystalClear Software, Inc.
+Copyright (c) 2005 CrystalClear Software, Inc.
+Copyright (c) 2006 CrystalClear Software, Inc.
+Copyright (c) 2006, 2007 Julio M. Merino Vidal
+Copyright (c) 2009-2017 The MathJax Consortium
+Copyright (c) 2010-2017 The MathJax Consortium
+Copyright (c) 2011 Jeff Flinn, Boris Schaeling
+Copyright (c) 2011-2015 The MathJax Consortium
+Copyright (c) 2011-2017 The MathJax Consortium
+Copyright (c) 2012 Mateusz Loskot, London, UK.
+Copyright (c) 2013 Mateusz Loskot, London, UK.
+Copyright (c) 2013-2017 The MathJax Consortium
+Copyright (c) 2014 Mateusz Loskot, London, UK.
+Copyright (c) 2014-2017 The MathJax Consortium
+Copyright (c) 2015-2017 The MathJax Consortium
+Copyright (c) 2016 Modified Work Barrett Adair
+Copyright (c) 2016-2017 The MathJax Consortium
+Copyright 2001, 2003, 2004, 2012 Daryle Walker
+Copyright 2005-2007 Adobe Systems Incorporated
+Copyright 2011 Garmin Ltd. or its subsidiaries
+Copyright 2012 Chung-Lin Wen, Davide Anastasia
+Copyright J.S. Roy (js@jeannot.org), 2002-2005
+(c) Copyright Daniel Frey and Robert Ramey 2009
+Copyright (c) 1995 Maarten Hilferink, Amsterdam
+Copyright (c) 2002 Brad King and Douglas Gregor
+Copyright (c) 2003 Gunter Winkler, Joerg Walter
+Copyright (c) 2003-2011 Christopher M. Kohlhoff
+Copyright (c) 2003-2020 Christopher M. Kohlhoff
+Copyright (c) 2005 Arkadiy Vertleyb, Peder Holt
+Copyright (c) 2005 Voipster / Indrek dot Juhani
+Copyright (c) 2005-2020 Christopher M. Kohlhoff
+Copyright (c) 2006-2009, 2012 Alexander Nasonov
+Copyright (c) 2009, Pauli Virtanen <pav@iki.fi>
+Copyright (c) 2012 - 2014, 2017 Andrey Semashev
+Copyright (c) 2013 - 2018, 2020 Andrey Semashev
+Copyright (c) 2013 Tim Blechmann Linux-specific
+Copyright (c) 2015 Oracle and/or its affiliates
+Copyright (c) 2015, Pauli Virtanen <pav@iki.fi>
+Copyright (c) 2016 Oracle and/or its affiliates
+Copyright (c) 2017 Oracle and/or its affiliates
+Copyright (c) 2018 Oracle and/or its affiliates
+Copyright (c) 2019 Oracle and/or its affiliates
+Copyright (c) 2020 Oracle and/or its affiliates
+Copyright 2002 Rensselaer Polytechnic Institute
+Copyright 2004-9 Trustees of Indiana University
+Copyright 2010 Fabien Castan, Christian Henning
+Copyright 2010 Gaetano Mendola, 2011 Simon West
+copyright (c) 2014 Oracle and/or its affiliates
+copyright (c) 2015 Oracle and/or its affiliates
+copyright (c) 2016 Oracle and/or its affiliates
+copyright (c) 2017 Oracle and/or its affiliates
+copyright (c) 2018 Oracle and/or its affiliates
+copyright (c) 2019 Oracle and/or its affiliates
+copyright (c) 2020 Oracle and/or its affiliates
+(c) Copyright 2004 Robert Ramey and Martin Ecker
+(c) Copyright 2009-2012 Vicente J. Botet Escriba
+(c) Copyright 2010-2011 Vicente J. Botet Escriba
+(c) Copyright 2011-2012 Vicente J. Botet Escriba
+(c) Copyright 2011-2013 Vicente J. Botet Escriba
+(c) Copyright 2011-2015 Vicente J. Botet Escriba
+(c) Copyright 2013,2014 Vicente J. Botet Escriba
+(c) Copyright 2013,2015 Vicente J. Botet Escriba
+(c) Copyright David Abrahams, Vicente Botet 2009
+(c) Copyright Eric Jourdanneau, Joel Falcou 2010
+(c) Copyright John Maddock and Steve Cleary 2000
+(c) Copyright Vicente J. Botet Escriba 2013-2014
+(c) Copyright Vicente J. Botet Escriba 2013-2017
+(c) Copyright Vicente J. Botet Escriba 2014-2015
+CNRS/Univ. Clermont II Copyright 2009 - 2011 LRI
+Copyright (c) 2001, Thomas Flemming, tf@ttqv.com
+Copyright (c) 2003-2004 Jeremy B. Maitin-Shepard
+Copyright (c) 2008 Ilya Sokolov, Boris Schaeling
+Copyright (c) 2009, Spirent Communications, Inc.
+Copyright (c) 2010 Eric Jourdanneau, Joel Falcou
+Copyright (c) 2010 Felipe Tanus, Boris Schaeling
+Copyright (c) 2010 Nuovation System Designs, LLC
+Copyright (c) 2011-2012 Vicente J. Botet Escriba
+Copyright (c) 2011-2013 Vicente J. Botet Escriba
+Copyright (c) 2012-2013 Vicente J. Botet Escriba
+Copyright (c) 2013 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2013 John Maddock, Antony Polukhin
+Copyright (c) 2013,2014 Vicente J. Botet Escriba
+Copyright (c) 2013-2014 Vicente J. Botet Escriba
+Copyright (c) 2014 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2014, 2015, 2016, 2017 Jarryd Beck
+Copyright (c) 2014, Oracle and/or its affiliates
+Copyright (c) 2014-2015 Vicente J. Botet Escriba
+Copyright (c) 2014-2017 Vicente J. Botet Escriba
+Copyright (c) 2015, Oracle and/or its affiliates
+Copyright (c) 2016, Oracle and/or its affiliates
+Copyright (c) 2017 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2017, Oracle and/or its affiliates
+Copyright (c) 2018 Adam Butcher, Antony Polukhin
+Copyright (c) 2018 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2018, Oracle and/or its affiliates
+Copyright (c) 2019, Oracle and/or its affiliates
+Copyright (c) 2020, Oracle and/or its affiliates
+Copyright 1984, 1987, 1995 by Stephen L. Moshier
+Copyright 1984, 1987, 2000 by Stephen L. Moshier
+Copyright 1984, 1995, 2000 by Stephen L. Moshier
+Copyright 1985, 1987, 2000 by Stephen L. Moshier
+Copyright 2003 Guillaume Melquiond, Sylvain Pion
+Copyright Justinas Vygintas Daugmaudis 2010-2018
+Copyright Paul A. Bristow 2006, 2007, 2009, 2010
+Copyright Paul A. Bristow 2007, 2009, 2010, 2012
+Copyright Paul A. Bristow 2007, 2010, 2012, 2014
+copyright (c) 2013, Oracle and/or its affiliates
+copyright (c) 2014, Oracle and/or its affiliates
+copyright (c) 2015, Oracle and/or its affiliates
+copyright (c) 2016, Oracle and/or its affiliates
+copyright (c) 2017, Oracle and/or its affiliates
+copyright (c) 2018, Oracle and/or its affiliates
+copyright (c) 2020, Oracle and/or its affiliates
+(c) Rasmus Munk Larsen, Stanford University, 2000
+(c) Rasmus Munk Larsen, Stanford University, 2004
+Copyright (c) 2002-2003 Eric Friedman, Itay Maman
+Copyright (c) 2006 Trustees of Indiana University
+Copyright (c) 2007 Trustees of Indiana University
+Copyright (c) 2007-2011 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2012 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2013 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2014 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2015 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2016 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2017 Barend Gehrels, Amsterdam
+Copyright (c) 2007-2020 Barend Gehrels, Amsterdam
+Copyright (c) 2008-2012 Barend Gehrels, Amsterdam
+Copyright (c) 2008-2014 Barend Gehrels, Amsterdam
+Copyright (c) 2008-2015 Barend Gehrels, Amsterdam
+Copyright (c) 2009 Trustees of Indiana University
+Copyright (c) 2009-2012 Barend Gehrels, Amsterdam
+Copyright (c) 2009-2015 Barend Gehrels, Amsterdam
+Copyright (c) 2010-2012 Barend Gehrels, Amsterdam
+Copyright (c) 2011-2012 Barend Gehrels, Amsterdam
+Copyright (c) 2011-2015 Barend Gehrels, Amsterdam
+Copyright (c) 2012-2014 Barend Gehrels, Amsterdam
+Copyright (c) 2012-2015 Barend Gehrels, Amsterdam
+Copyright (c) 2012-2020 Barend Gehrels, Amsterdam
+Copyright (c) 2014-2015 Barend Gehrels, Amsterdam
+Copyright (c) 2015-2016 Barend Gehrels, Amsterdam
+Copyright (c) 2015-2020 Barend Gehrels, Amsterdam
+Copyright (c) 2017-2017 Barend Gehrels, Amsterdam
+Copyright (c) 2018-2019 Barend Gehrels, Amsterdam
+Copyright (c) 2019-2019 Barend Gehrels, Amsterdam
+Copyright 1984, 1987 by Stephen L. Moshier Direct
+Copyright 1984, 1991 by Stephen L. Moshier Direct
+Copyright 1985, 1987 by Stephen L. Moshier Direct
+Copyright 2002 The Trustees of Indiana University
+Copyright 2003 The Trustees of Indiana University
+Copyright 2004 The Trustees of Indiana University
+Copyright 2005 Felix Hofling, Guillaume Melquiond
+Copyright 2005 The Trustees of Indiana University
+Copyright 2006 The Trustees of Indiana University
+Copyright 2008 Christian Henning, Lubomir Bourdev
+Copyright 2009 The Trustees of Indiana University
+Copyright 2010 The Trustees of Indiana University
+Copyright 2012 Kenneth Riddile, Christian Henning
+Copyright 2012 The Trustees of Indiana University
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2010
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2011
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2012
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2013
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2014
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2015
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2016
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2017
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2018
+(c) Copyright Dave Abrahams and Daryle Walker 2001
+(c) Copyright Jeremy Siek and John R. Bandela 2001
+(c) Copyright John Maddock & Thorsten Ottosen 2005
+(c) Copyright Kevlin Henney and Dave Abrahams 1999
+Copyright (c) 2000-2002 Joerg Walter, Mathias Koch
+Copyright (c) 2000-2004 Joerg Walter, Mathias Koch
+Copyright (c) 2001 Vladimir Prus <ghost@cs.msu.su>
+Copyright (c) 2003-2008 Matthias Christian Schabel
+Copyright (c) 2003-2009 Matthias Christian Schabel
+Copyright (c) 2010 David Fong and Michael Saunders
+Copyright (c) 2019 Dario Menendez, Banco Santander
+Copyright 2005 David Abrahams and Aleksey Gurtovoy
+Copyright 2012 Fernando Vilas 2010 Daniel Trebbien
+Copyright 2014 Renato Tegon Forti, Antony Polukhin
+Copyright 2018 Mateusz Loskot <mateusz@loskot.net>
+Copyright Alexander Nasonov & Paul A. Bristow 2006
+Copyright David Abrahams and Nikolay Mladenov 2003
+Copyright (c) 2000 Gary Powell (powellg@amazon.com)
+Copyright (c) 2001 Peter Dimov and Multi Media Ltd.
+Copyright (c) 2001, 2002 Python Software Foundation
+Copyright (c) 2001-2007 Hartmut Kaiser Revised 2007
+Copyright (c) 2002 Peter Dimov and Multi Media Ltd.
+Copyright (c) 2002,2003 CrystalClear Software, Inc.
+Copyright (c) 2002-2004 CrystalClear Software, Inc.
+Copyright (c) 2002-2005 CrystalClear Software, Inc.
+Copyright (c) 2002-2020 CrystalClear Software, Inc.
+Copyright (c) 2003-2004 CrystalClear Software, Inc.
+Copyright (c) 2003-2005 CrystalClear Software, Inc.
+Copyright (c) 2004-2005 CrystalClear Software, Inc.
+Copyright (c) 2006, Systems Optimization Laboratory
+Copyright (c) 2007, John Travers <jtravs@gmail.com>
+Copyright (c) 2009-2011 Mateusz Loskot, London, UK.
+Copyright (c) 2009-2012 Mateusz Loskot, London, UK.
+Copyright (c) 2009-2013 Mateusz Loskot, London, UK.
+Copyright (c) 2009-2014 Mateusz Loskot, London, UK.
+Copyright (c) 2009-2015 Mateusz Loskot, London, UK.
+Copyright (c) 2009-2017 Mateusz Loskot, London, UK.
+Copyright (c) 2011-2012 Mateusz Loskot, London, UK.
+Copyright (c) 2012-2014 Mateusz Loskot, London, UK.
+Copyright (c) 2014-2015 Mateusz Loskot, London, UK.
+Copyright (c) 2018 Adeel Ahmad, Islamabad, Pakistan
+Copyright 2004, 2005 Trustees of Indiana University
+Copyright 2004-5 The Trustees of Indiana University
+Copyright 2012 Olivier Tournaire, Christian Henning
+Copyright 2016 Klemens Morgenstern, Antony Polukhin
+Copyright 2019 Miral Shah <miralshah2211@gmail.com>
+Copyright David Abrahams 2002, Joel de Guzman, 2002
+Copyright Thorsten Ottosen, Neil Groves 2006 - 2008
+(c) Copyright 2005 Matthias Troyer and Dave Abrahams
+(c) Copyright Greg Colvin and Beman Dawes 1998, 1999
+Copyright (c) 1998-2003 by the University of Florida
+Copyright (c) 2003, Fernando Luis Cacciola Carballal
+Copyright (c) 2005, Fernando Luis Cacciola Carballal
+Copyright (c) 2006 Xiaogang Zhang, 2015 John Maddock
+Copyright (c) 2011, 2012 Jeff Flinn, Boris Schaeling
+Copyright (c) 2013 Kyle Lutz <kyle.r.lutz@gmail.com>
+Copyright (c) 2014 Samuel Debionne, Grenoble, France
+Copyright (c) 2014-2016 Oracle and/or its affiliates
+Copyright (c) 2014-2018 Oracle and/or its affiliates
+Copyright (c) 2014-2020 Oracle and/or its affiliates
+Copyright (c) 2015 Jakub Pola <jakub.pola@gmail.com>
+Copyright (c) 2015 Jakub Szuppe <j.szuppe@gmail.com>
+Copyright (c) 2015-2016 Oracle and/or its affiliates
+Copyright (c) 2015-2018 Oracle and/or its affiliates
+Copyright (c) 2015-2020 Oracle and/or its affiliates
+Copyright (c) 2016 Jakub Szuppe <j.szuppe@gmail.com>
+Copyright (c) 2016-2018 Oracle and/or its affiliates
+Copyright (c) 2016-2019 Oracle and/or its affiliates
+Copyright (c) 2016-2020 Oracle and/or its affiliates
+Copyright (c) 2017-2018 Oracle and/or its affiliates
+Copyright (c) 2017-2019 Oracle and/or its affiliates
+Copyright (c) 2017-2020 Oracle and/or its affiliates
+Copyright (c) 2018 Jakub Szuppe <j.szuppe@gmail.com>
+Copyright (c) 2018, Cem Bassoy, cem.bassoy@gmail.com
+Copyright (c) 2018-2019 Oracle and/or its affiliates
+Copyright (c) 2018-2020 Oracle and/or its affiliates
+Copyright (c) 2020 Caian Benedicto, Campinas, Brazil
+Copyright 2000 John Maddock (john@johnmaddock.co.uk)
+Copyright 2013 Christian Henning and Juan V. Puertos
+Copyright 2015 Ontario Institute for Cancer Research
+Copyright David Abrahams 2002, Nikolay Mladenov 2007
+Copyright David Abrahams and Thomas Becker 2000-2006
+Copyright Peter Dimov and Multi Media Ltd 2001, 2002
+copyright (c) 2013-2017 Oracle and/or its affiliates
+copyright (c) 2013-2018 Oracle and/or its affiliates
+copyright (c) 2013-2019 Oracle and/or its affiliates
+copyright (c) 2013-2020 Oracle and/or its affiliates
+copyright (c) 2014-2015 Oracle and/or its affiliates
+copyright (c) 2014-2017 Oracle and/or its affiliates
+copyright (c) 2014-2018 Oracle and/or its affiliates
+copyright (c) 2014-2019 Oracle and/or its affiliates
+copyright (c) 2014-2020 Oracle and/or its affiliates
+copyright (c) 2015-2016 Oracle and/or its affiliates
+copyright (c) 2015-2017 Oracle and/or its affiliates
+copyright (c) 2015-2019 Oracle and/or its affiliates
+copyright (c) 2015-2020 Oracle and/or its affiliates
+copyright (c) 2016-2018 Oracle and/or its affiliates
+copyright (c) 2016-2020 Oracle and/or its affiliates
+copyright (c) 2017-2018 Oracle and/or its affiliates
+copyright (c) 2017-2020 Oracle and/or its affiliates
+copyright (c) 2018-2020 Oracle and/or its affiliates
+copyright (c) 2019-2020 Oracle and/or its affiliates
+(c) Copyright 2002 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2004 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2005 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2007 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2008-2009,2012 Vicente J. Botet Escriba
+(c) Copyright 2009 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2011,2012,2015 Vicente J. Botet Escriba
+(c) Copyright 2011-2012,2015 Vicente J. Botet Escriba
+(c) Copyright 2014 Robert Ramey - http://www.rrsd.com
+(c) Copyright Vicente J. Botet Escriba 2008-2009,2012
+Copyright (c) 2000 Gary Powell (gwpowell@hotmail.com)
+Copyright (c) 2001 Jeremy Siek <jsiek@cs.indiana.edu>
+Copyright (c) 2001-2002 Chuck Allison and Jeremy Siek
+Copyright (c) 2002 Gary Powell (gwpowell@hotmail.com)
+Copyright (c) 2002-2003 David Moore, William E. Kempf
+Copyright (c) 2004 The Trustees of Indiana University
+Copyright (c) 2006 The Trustees of Indiana University
+Copyright (c) 2007 Douglas Gregor and Matthias Troyer
+Copyright (c) 2007 The Trustees of Indiana University
+Copyright (c) 2011-2013 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2011-2014 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2011-2015 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2011-2016 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2011-2017 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2011-2018 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2011-2019 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2012-2013 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2012-2015 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2012-2020 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2013-2014 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2013-2015 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2013-2017 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2014-2015 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2014-2015, Oracle and/or its affiliates
+Copyright (c) 2014-2017 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2014-2017, Oracle and/or its affiliates
+Copyright (c) 2014-2018 Adam Wulkiewicz, Lodz, Poland
+Copyright (c) 2014-2018, Oracle and/or its affiliates
+Copyright (c) 2014-2019, Oracle and/or its affiliates
+Copyright (c) 2014-2020, Oracle and/or its affiliates
+Copyright (c) 2015-2017, Oracle and/or its affiliates
+Copyright (c) 2015-2018, Oracle and/or its affiliates
+Copyright (c) 2015-2020, Oracle and/or its affiliates
+Copyright (c) 2016, 2018 Oracle and/or its affiliates
+Copyright (c) 2016-2017, Oracle and/or its affiliates
+Copyright (c) 2016-2020, Oracle and/or its affiliates
+Copyright (c) 2017, 2019 Oracle and/or its affiliates
+Copyright (c) 2017-2018, Oracle and/or its affiliates
+Copyright (c) 2017-2019, Oracle and/or its affiliates
+Copyright (c) 2017-2020, Oracle and/or its affiliates
+Copyright (c) 2018-2019, Oracle and/or its affiliates
+Copyright (c) 2018-2020, Oracle and/or its affiliates
+Copyright (c) 2019-2020, Oracle and/or its affiliates
+Copyright (c) 2020 Digvijay Janartha, Hamirpur, India
+copyright (c) 2013, 2014 Oracle and/or its affiliates
+copyright (c) 2013-2014, Oracle and/or its affiliates
+copyright (c) 2013-2015, Oracle and/or its affiliates
+copyright (c) 2013-2017, Oracle and/or its affiliates
+copyright (c) 2013-2018, Oracle and/or its affiliates
+copyright (c) 2013-2019, Oracle and/or its affiliates
+copyright (c) 2013-2020, Oracle and/or its affiliates
+copyright (c) 2014-2017, Oracle and/or its affiliates
+copyright (c) 2014-2018, Oracle and/or its affiliates
+copyright (c) 2014-2019, Oracle and/or its affiliates
+copyright (c) 2014-2020, Oracle and/or its affiliates
+copyright (c) 2015-2016, Oracle and/or its affiliates
+copyright (c) 2015-2017, Oracle and/or its affiliates
+copyright (c) 2015-2018, Oracle and/or its affiliates
+copyright (c) 2015-2019, Oracle and/or its affiliates
+copyright (c) 2015-2020, Oracle and/or its affiliates
+copyright (c) 2016-2019, Oracle and/or its affiliates
+copyright (c) 2016-2020, Oracle and/or its affiliates
+copyright (c) 2017, 2019 Oracle and/or its affiliates
+copyright (c) 2017-2018, Oracle and/or its affiliates
+copyright (c) 2017-2019, Oracle and/or its affiliates
+copyright (c) 2017-2020, Oracle and/or its affiliates
+copyright (c) 2018-2019, Oracle and/or its affiliates
+copyright (c) 2018-2020, Oracle and/or its affiliates
+(c) Copyright Beman Dawes and Ullrich Koethe 1995-2001
+(c) Copyright David Abrahams 2001, Howard Hinnant 2001
+(c) Copyright Hubert Holin and Daryle Walker 2001-2002
+(c) Rasmus Munk Larsen, Stanford University, 2000,2004
+Copyright (c) 2002-2017 Free Software Foundation, Inc.
+Copyright (c) 2014, 2018, Oracle and/or its affiliates
+Copyright (c) 2014, 2019, Oracle and/or its affiliates
+Copyright (c) 2016 Wenzel Jakob <wenzel.jakob@epfl.ch>
+Copyright (c) 2020 Richard Hodges (hodges.r@gmail.com)
+Copyright (c) Jeremy Siek 2001, Marc Wintermantel 2002
+Copyright 1984, 1987, 1988, 2000 by Stephen L. Moshier
+Copyright 1984, 1987, 1989, 1995 by Stephen L. Moshier
+Copyright 1984, 1987, 1989, 2000 by Stephen L. Moshier
+Copyright 1984, 1987, 1992, 2000 by Stephen L. Moshier
+Copyright 2004-2006 The Trustees of Indiana University
+Copyright 2005-2009 The Trustees of Indiana University
+Copyright 2007-2008 Andreas Pokorny, Christian Henning
+Copyright 2007-2008 Christian Henning, Andreas Pokorny
+Copyright 2007-2012 Christian Henning, Andreas Pokorny
+Copyright 2007-2012 Christian Henning, Lubomir Bourdev
+Copyright 2010-2012 Kenneth Riddile, Christian Henning
+copyright (c) 2014, 2018, Oracle and/or its affiliates
+copyright (c) 2014, 2019, Oracle and/or its affiliates
+copyright (c) 2015, 2018, Oracle and/or its affiliates
+copyright (c) 2017, 2019, Oracle and/or its affiliates
+copyright (c) 2018, 2019, Oracle and/or its affiliates
+(c) 2020 Niall Douglas <http://www.nedproductions.biz/>
+(c) Copyright Boris Rasin and Antony Polukhin 2014-2019
+(c) Copyright Dave Abrahams and Daniel Walker 1999-2003
+(c) Copyright Robert Ramey 2003. Jonathan Turkanis 2004
+(c) Rasmus Munk Larsen, Stanford University, 1999, 2004
+(c) Rasmus Munk Larsen, Stanford University, 2000, 2004
+Copyright (c) 1995, 2007-2015 Barend Gehrels, Amsterdam
+Copyright (c) 1995-2013 Jean-loup Gailly and Mark Adler
+Copyright (c) 2000 Gary Powell (gary.powell@sierra.com)
+Copyright (c) 2001 Gary Powell (gary.powell@sierra.com)
+Copyright (c) 2002 Lars Gullik Bjonnes <larsbj@lyx.org>
+Copyright (c) 2011 Boris Schaeling (boris@highscore.de)
+Copyright (c) 2014 Roshan <thisisroshansmail@gmail.com>
+Copyright (c) 2015 Orson Peters <orsonpeters@gmail.com>
+Copyright (c) 2021 Orson Peters <orsonpeters@gmail.com>
+Copyright (c) Donald Stufft and individual contributors
+Copyright 1984, 1987, 1988 by Stephen L. Moshier Direct
+Copyright 1984, 1987, 1989 by Stephen L. Moshier Direct
+Copyright 1984, 1987, 1993 by Stephen L. Moshier Direct
+Copyright 1985, 1987, 1989 by Stephen L. Moshier Direct
+Copyright 2004, 2005 The Trustees of Indiana University
+Copyright 2014-2015 Renato Tegon Forti, Antony Polukhin
+Copyright 2019 Pranam Lashkari <plashkari628@gmail.com>
+(c) Copyright 2006 David Abrahams - http://www.boost.org
+(c) Copyright Daryle Walker and Stephen Cleary 2001-2002
+(c) Copyright Fernando Luis Cacciola Carballal 2000-2004
+Copyright (c) 2001 Jaakko Jarvi (jaakko.jarvi@cs.utu.fi)
+Copyright (c) 2001-2004 Peter Dimov and Multi Media Ltd.
+Copyright (c) 2002 Jaakko Jarvi (jaakko.jarvi@cs.utu.fi)
+Copyright (c) 2002,2003,2005 CrystalClear Software, Inc.
+Copyright (c) 2002,2003,2020 CrystalClear Software, Inc.
+Copyright (c) 2002-2003,2005 CrystalClear Software, Inc.
+Copyright (c) 2012 Massachusetts Institute of Technology
+Copyright (c) 2019 Vinnie Falco (vinnie.falco@gmail.com)
+Copyright (c) 2020 Vinnie Falco (vinnie.falco@gmail.com)
+Copyright 2008 CodeRage, LLC 2004-2007 Jonathan Turkanis
+Copyright 2014 Marco Guazzone (marco.guazzone@gmail.com)
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2009 - 2010
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2009 - 2011
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2009 - 2012
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2010 - 2011
+Copyright Abel Sinkovics (abel@sinkovics.hu) 2011 - 2012
+Copyright Ralf W. Grosse-Kunstleve & David Abrahams 2006
+(c) ACM, 2011. http://doi.acm.org/10.1145/1916461.1916469
+(c) Copyright 2002-2008, Fernando Luis Cacciola Carballal
+Copyright (c) 1999-2006 Cortex Software GmbH, Kantstrasse
+Copyright (c) 2001, 2002 Peter Dimov and Multi Media Ltd.
+Copyright (c) 2002, 2003 Peter Dimov and Multi Media Ltd.
+Copyright (c) 2002,2003, 2007 CrystalClear Software, Inc.
+Copyright (c) 2002,2003, 2020 CrystalClear Software, Inc.
+Copyright (c) 2003, 2008 Fernando Luis Cacciola Carballal
+Copyright (c) 2006-2013 The University of Colorado Denver
+Copyright (c) 2007 Douglas Gregor <doug.gregor@gmail.com>
+Copyright (c) 2009 Ben Hanson (http://www.benhanson.net/)
+Copyright (c) 2013-2014 Kyle Lutz <kyle.r.lutz@gmail.com>
+Copyright (c) 2013-2015 Kyle Lutz <kyle.r.lutz@gmail.com>
+Copyright (c) 2014-2015 Samuel Debionne, Grenoble, France
+Copyright (c) 2015 Francisco Jose Tapia fjtapia@gmail.com
+Copyright (c) 2016 Francisco Jose Tapia fjtapia@gmail.com
+Copyright (c) 2017 Francisco Jose Tapia fjtapia@gmail.com
+Copyright (c) 2018 Alain Miniussi <alain.miniussi@oca.eu>
+Copyright (c) 2018-2019, Cem Bassoy, cem.bassoy@gmail.com
+Copyright (c) 2019 Mika Fischer (mika.fischer@zoopnet.de)
+Copyright 1997, 1998, 1999, 2000 University of Notre Dame
+Copyright 2002 Aleksey Gurtovoy (agurtovoy@meta-comm.com)
+Copyright 2014 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2015 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2017 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2018 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2019 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2020 Glen Joseph Fernandes (glenjofe@gmail.com)
+(c) Copyright 2002-2009 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2002-2014 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2002-2020 Robert Ramey - http://www.rrsd.com
+(c) Copyright 2011-2012,2017-2018 Vicente J. Botet Escriba
+Copyright (c) 1996 Silicon Graphics Computer Systems, Inc.
+Copyright (c) 1998 Silicon Graphics Computer Systems, Inc.
+Copyright (c) 2004-2006 The Trustees of Indiana University
+Copyright (c) 2004-2008 The Trustees of Indiana University
+Copyright (c) 2004-2009 The Trustees of Indiana University
+Copyright (c) 2005-2006 The Trustees of Indiana University
+Copyright (c) 2005-2008 The Trustees of Indiana University
+Copyright (c) 2005-2010 The Trustees of Indiana University
+Copyright (c) 2006-2007, Robert Hetland <hetland@tamu.edu>
+Copyright (c) 2006-2010 The Trustees of Indiana University
+Copyright (c) 2011, 2012 Martin Lambers <marlam@marlam.de>
+Copyright (c) 2012 Flavio De Lorenzi (fdlorenzi@gmail.com)
+Copyright 1999, 2000 Jaakko Jarvi (jaakko.jarvi@cs.utu.fi)
+Copyright 2009 (c) Dean Michael Berris <me@deanberris.com>
+(c) 1995 Ernst Stadlober, Institut fuer Statistitk, TU Graz
+Copyright (c) 2001 Jeremy Siek, Douglas Gregor, Brian Osman
+Copyright (c) 2005, Rasmus Munk Larsen, Stanford University
+Copyright (c) 2006 Tiago de Paula Peixoto <tiago@forked.de>
+Copyright (c) 2006-2009 Dmitry Bufistov and Andrey Parfenov
+Copyright (c) 2014, 2019, 2020 Oracle and/or its affiliates
+Copyright (c) 2017 Denis Demidov <dennis.demidov@gmail.com>
+Copyright (c) 2017-2018 Alexandr Poltavsky, Antony Polukhin
+Copyright 2013 Juan V. Puertos G-Cluster, Christian Henning
+(c) 2015-2020 Niall Douglas <http://www.nedproductions.biz/>
+(c) 2017-2020 Niall Douglas <http://www.nedproductions.biz/>
+(c) 2018-2020 Niall Douglas <http://www.nedproductions.biz/>
+(c) 2019-2020 Niall Douglas <http://www.nedproductions.biz/>
+Copyright (c) 2001 Housemarque Oy http://www.housemarque.com
+Copyright (c) 2002-2005, Jean-Sebastien Roy (js@jeannot.org)
+Copyright (c) 2004-2005, Jean-Sebastien Roy (js@jeannot.org)
+Copyright (c) 2014, 2018, 2019, Oracle and/or its affiliates
+Copyright (c) Alexander Zaitsev <zamazan4ik@gmail.by> , 2017
+Copyright (c) Tobias Schwinger http://spirit.sourceforge.net
+Copyright 1984, 1987, 1988, 1992, 2000 by Stephen L. Moshier
+Copyright 1984, 1987, 1989, 1992, 2000 by Stephen L. Moshier
+(c) Copyright Runar Undheim, Robert Ramey & John Maddock 2008
+Copyright (c) 2000-2003 Brian McNamara and Yannis Smaragdakis
+Copyright (c) 2000-2013 The University of California Berkeley
+Copyright (c) 2002,2003,2005,2020 CrystalClear Software, Inc.
+Copyright (c) 2003 Martin Wille http://spirit.sourceforge.net
+Copyright (c) 2011 Aaron Graham http://spirit.sourceforge.net
+Copyright (c) 2014 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright (c) 2017 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright (c) 2020 Krystian Stasiowski (sdkrystian@gmail.com)
+Copyright (c) Alexander Zaitsev <zamazan4ik@gmail.com> , 2016
+Copyright (c) Alexander Zaitsev <zamazan4ik@gmail.com> , 2017
+Copyright (c) Charles Karney (2008-2017) <charles@karney.com>
+Copyright (c) Glen Joseph Fernandes 2019 (glenjofe@gmail.com)
+Copyright 1984, 1987, 1988, 1992 by Stephen L. Moshier Direct
+Copyright 1984, 1987, 1989, 1992 by Stephen L. Moshier Direct
+Copyright Daniel Walker, Eric Niebler, Michel Morin 2008-2012
+(c) 2018 - 2019 Niall Douglas <http://www.nedproductions.biz/>
+(c) 2018 - 2020 Niall Douglas <http://www.nedproductions.biz/>
+(c) Copyright 2002-2008 Robert Ramey and Joaquin M Lopez Munoz
+Copyright (c) 1999, 2000 Jaakko Jarvi (jaakko.jarvi@cs.utu.fi)
+Copyright (c) 1999, 2000, 2001 North Carolina State University
+Copyright (c) 2001 Bruce Florman http://spirit.sourceforge.net
+Copyright (c) 2001 Daniel Nuffer http://spirit.sourceforge.net
+Copyright (c) 2002 Jeff Westfahl http://spirit.sourceforge.net
+Copyright (c) 2003 Giovanni Bajo http://spirit.sourceforge.net
+Copyright (c) 2003 Vaclav Vesely http://spirit.sourceforge.net
+Copyright (c) 2005-2006 Douglas Gregor <doug.gregor@gmail.com>
+Copyright (c) 2006 Joao Abecasis http://spirit.sourceforge.net
+Copyright (c) 2007-2009 Ben Hanson (http://www.benhanson.net/)
+Copyright (c) 2008-2009 Ben Hanson (http://www.benhanson.net/)
+Copyright (c) 2010 2015 Francisco Jose Tapia fjtapia@gmail.com
+Copyright (c) 2010 Bryce Lelbach http://spirit.sourceforge.net
+Copyright (c) 2010 Matthias Walter (xammy@xammy.homelinux.net)
+Copyright (c) 2011 Bryce Lelbach http://spirit.sourceforge.net
+Copyright (c) 2013 Agustin Berge http://spirit.sourceforge.net
+Copyright (c) 2017 Kristian Popov <kristian.popov@outlook.com>
+Copyright (c) Tyler Reddy, Richard Gowers, and Max Linke, 2016
+Copyright 2012-2019 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2014,2018 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2014-2015 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2014-2016 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2014-2020 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2016-2021 Matthew Brett, Isuru Fernando, Matti Picus
+Copyright 2017-2018 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2017-2019 Glen Joseph Fernandes (glenjofe@gmail.com)
+Copyright 2019-2020 Glen Joseph Fernandes (glenjofe@gmail.com)
+(c) Copyright Andreas Huber Doenni 2002-2005, Eric Niebler 2006
+(c) Copyright Peter Dimov and Multi Media Ltd. 2001, 2002, 2003
+Copyright (c) 1996,1997 Silicon Graphics Computer Systems, Inc.
+Copyright (c) 1996-1998 Silicon Graphics Computer Systems, Inc.
+Copyright (c) 2001, 2002, 2003 Peter Dimov and Multi Media Ltd.
+Copyright (c) 2002 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2003 Gustavo Guerra http://spirit.sourceforge.net
+Copyright (c) 2003 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2003 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 2003 Jonathan de Halleux (dehalleux@pelikhan.com)
+Copyright (c) 2004 David M. Cooke <cookedm@physics.mcmaster.ca>
+Copyright (c) 2009 Francois Barel http://spirit.sourceforge.net
+Copyright (c) 2011 Thomas Bernard http://spirit.sourceforge.net
+Copyright (c) 2016 Frank Hein, maxence business consulting gmbh
+Copyright Daryle Walker, Hubert Holin, John Maddock 2006 - 2007
+(c) Copyright Mat Marcus, Jesse Jones and Adobe Systems Inc 2001
+Copyright (c) 2000-2010 Joerg Walter, Mathias Koch, David Bellot
+Copyright (c) 2000-2011 Joerg Walter, Mathias Koch, David Bellot
+Copyright (c) 2000-2013 Joerg Walter, Mathias Koch. David Bellot
+Copyright (c) 2003, Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2007 Matthias Troyer <troyer@boost-consulting.com>
+Copyright Neil Groves & Thorsten Ottosen & Pavol Droba 2003-2004
+copyrighted 2004 by David M. Cooke <cookedm@physics.mcmaster.ca>
+(c) 2000 W. Hoermann & J. Leydold, Institut f. Statistik, WU Wien
+(c) 2007 W. Hoermann & J. Leydold, Institut f. Statistik, WU Wien
+Copyright (c) 2002-2003 Toon Knapen, Kresimir Fresl, Joerg Walter
+Copyright (c) 2003, 2007-14 Massachusetts Institute of Technology
+Copyright (c) 2006 Tobias Schwinger http://spirit.sourceforge.net
+Copyright (c) 2006-2008 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2006-2009 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2006-2010 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2006-2013 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2008-2009 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2008-2016 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2008-2017 Emil Dotchevski and Reverge Studios, Inc.
+Copyright (c) 2018-2020 Emil Dotchevski and Reverge Studios, Inc.
+(c) Copyright David Abrahams, Jeremy Siek, Daryle Walker 1999-2001
+Copyright (c) 2000-2007 Joerg Walter, Mathias Koch, Gunter Winkler
+Copyright (c) 2000-2009 Joerg Walter, Mathias Koch, Gunter Winkler
+Copyright (c) 2001, Daniel C. Nuffer http://spirit.sourceforge.net
+Copyright (c) 2002-2003 Martin Wille http://spirit.sourceforge.net
+Copyright (c) 2018 Yaghyavardhan Singh Khangarot, Hyderabad, India
+Copyright 2002 Herve Bronnimann, Guillaume Melquiond, Sylvain Pion
+Copyright 2012 Christian Henning, Andreas Pokorny, Lubomir Bourdev
+Copyright (c) 2001-2002 Enthought, Inc. 2003-2022, SciPy Developers
+Copyright (c) 2001-2003 Daniel Nuffer http://spirit.sourceforge.net
+Copyright (c) 2001-2009 Daniel Nuffer http://spirit.sourceforge.net
+Copyright (c) 2002 Raghavendra Satish http://spirit.sourceforge.net
+Copyright (c) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+Copyright (c) 2009 Free Software Foundation, Inc. <http://fsf.org/>
+Copyright (c) 2020, Debabrata Mandal <mandaldebabrata123@gmail.com>
+Copyright 2019 Olzhas Zhumabek <anonymous.from.applecity@gmail.com>
+Copyright (c) 1998-2002 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 1998-2003 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 2001-2003 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2001-2003 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 2001-2007 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2001-2008 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2001-2010 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2001-2011 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2001-2011 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 2001-2012 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2001-2012 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 2001-2014 Joel de Guzman http://spirit.sourceforge.net
+Copyright (c) 2002-2003 Hartmut Kaiser http://spirit.sourceforge.net
+Copyright (c) 2002-2006 Hartmut Kaiser http://spirit.sourceforge.net
+(c) Copyright 2004-2009 Robert Ramey, Martin Ecker and Takatoshi Kondo
+Copyright (c) 1996, 1997, 1998, 1999, 2000 Gerard Jungman, Brian Gough
+Copyright (c) 2008 Rep Invariant Systems, Inc. (info@repinvariant.com)
+(c) Copyright 2007, 2008 Steven Watanabe, Joseph Gauterin, Niels Dekker
+Copyright (c) 2007, 2008 Steven Watanabe, Joseph Gauterin, Niels Dekker
+Copyright (c) 2015 Muhammad Junaid Muzammil <mjunaidmuzammil@gmail.com>
+Copyright 2002-2003 Herve Bronnimann, Guillaume Melquiond, Sylvain Pion
+Copyright 2007-2008 Christian Henning, Andreas Pokorny, Lubomir Bourdev
+Copyright 2007-2012 Christian Henning, Andreas Pokorny, Lubomir Bourdev
+Copyright (c) 1998-2000 Theodore C. Belding University of Michigan Center
+Copyright (c) 2000-2013 Joerg Walter, Mathias Koch, Athanasios Iliopoulos
+Copyright 2003-2013 Joaquin M Lopez Munoz. 2019 Mike Dev <mike.dev@gmx.de>
+(c) Copyright 2002 Rani Sharoni (rani_sharoni@hotmail.com) and Robert Ramey
+(c) Copyright 2003-4 Pavel Vozenilek and Robert Ramey - http://www.rrsd.com
+(c) Copyright Steve Cleary, Beman Dawes, Howard Hinnant & John Maddock 2000
+Copyright 2014 by P.-G. Martinsson, V. Rokhlin, Y. Shkolnisky, and M. Tygert
+Copyright (c) 2021-04-21 Stefan van der Walt https://github.com/stefanv/lloyd
+copyright A. Volgenant/Amsterdam School of Economics, University of Amsterdam
+Copyright (c) 2002-2003 Juan Carlos Arevalo-Baeza http://spirit.sourceforge.net
+(c) Copyright Steve Cleary, Beman Dawes, Howard Hinnant & John Maddock 2000-2005
+Copyright (c) 2000-2010 Joerg Walter, Mathias Koch, Gunter Winkler, David Bellot
+Copyright 1987-, A. Volgenant/Amsterdam School of Economics, University of Amsterdam
+(c) Copyright 2010 Just Software Solutions Ltd http://www.justsoftwaresolutions.co.uk
+copyright (c) 2005 troy d. straszheim <troy@resophonic.com> http://www.resophonic.com
+Copyright (c) 2002 Brad King (brad.king@kitware.com) Douglas Gregor (gregod@cs.rpi.edu)
+(c) Copyright 2009-2011 Frederic Bron, Robert Stewart, Steven Watanabe & Roman Perepelitsa
+(c) Copyright Dave Abrahams, Steve Cleary, Beman Dawes, Howard Hinnant & John Maddock 2000
+(c) Copyright Dave Abrahams, Steve Cleary, Beman Dawes, Howard Hinnant and John Maddock 2000
+Copyright (c) 2018 Sylvain Gubian <sylvain.gubian@pmi.com> , Yang Xiang <yang.xiang@pmi.com>
+(c) Copyright Steve Cleary, Beman Dawes, Aleksey Gurtovoy, Howard Hinnant & John Maddock 2000
+Copyright (c) 2003 Jonathan de Halleux (dehalleux@pelikhan.com) http://spirit.sourceforge.net
+(c) Copyright Dave Abrahams, Steve Cleary, Beman Dawes, Howard Hinnant & John Maddock 2000-2003
+(c) Copyright David Abrahams Steve Cleary, Beman Dawes, Howard Hinnant & John Maddock 2000-2002
+Copyright (c) 1999-2001 Jaakko Jarvi (jaakko.jarvi@cs.utu.fi) Gary Powell (gwpowell@hotmail.com)
+Copyright (c) Tyler Reddy, Ross Hemsley, Edd Edmondson, Nikolai Nowaczyk, Joe Pitt-Francis, 2015
+Copyright (c) 2013 Jakob Lykke Andersen, University of Southern Denmark (jlandersen@imada.sdu.dk)
+(c) Copyright Dave Abrahams, Steve Cleary, Beman Dawes, Howard Hinnant and John Maddock 2000, 2010
+Copyright (c) 2001 Jaakko Jarvi (jaakko.jarvi@cs.utu.fi) 2001 Gary Powell (gary.powell@sierra.com)
+Copyright (c) 2003 Jonathan de Halleux http://spirit.sourceforge.net http://www.boost.org/libs/spirit
+Copyright (c) 1992-2013 The University of Tennessee and The University of Tennessee Research Foundation
+(c) Copyright Dave Abrahams, Steve Cleary, Beman Dawes, Aleksey Gurtovoy, Howard Hinnant & John Maddock 2000
+Copyright (c) 1990-2004 by Johannes Braams texniek at braams.cistron.nl Kersengaarde 33 2723 BP Zoetermeer NL
+Copyright (c) 2003, The Regents of the University of California, through Lawrence Berkeley National Laboratory
+Copyright (c) 2008 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2009 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2010 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2003-2009, The Regents of the University of California, through Lawrence Berkeley National Laboratory
+Copyright (c) 2000-2010 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2000-2022 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2008-2010 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2009-2010 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2009-2011 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2009-2012 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2011-2012 Wolfgang Hoermann and Josef Leydold Institute for Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2000-2006 Wolfgang Hoermann and Josef Leydold Dept. for Statistics, University of Economics, Vienna, Austria
+Copyright (c) 2000-2006, 2010 Wolfgang Hoermann and Josef Leydold Department of Statistics and Mathematics, WU Wien, Austria
+Copyright (c) 2001 Ronald Garcia, Indiana University (garcia@osl.iu.edu) Andrew Lumsdaine, Indiana University (lums@osl.iu.edu)
+Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021 Python Software Foundation
+(c) KOKOKOKOKKuKyKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKxKyK KyKxKzKzKzKzKzKzKzKzKzKzKzKzKyKxKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzKzK K K KzK K
+Copyright 2002 Marc Wintermantel (wintermantel@even-ag.ch) ETH Zurich, Center of Structure Technologies (https://web.archive.org/web/20050307090307/http://www.structures.ethz.ch/)
 
 BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-requests-oauthlib 1.3.1 - BSD-2-Clause AND ISC
+seaborn 0.12.2 - BSD-2-Clause AND BSD-3-Clause
 
 
-copyright u'2014, Kenneth Reitz
-Copyright (c) 2014 Kenneth Reitz
+copyright f'2012- time.strftime
+Copyright (c) 2013 Eddy Petrisor
+Copyright (c) 2012 Alexei Boronine
+Copyright 2004-2005 by Enthought, Inc.
+Copyright (c) 2012-2021, Michael L. Waskom
+Copyright (c) 2010 ActiveState Software Inc.
+Copyright (c) 2005-2010 ActiveState Software Inc.
+Copyright , https://mwaskom.github.io/' Michael Waskom
+Copyright (c) Donald Stufft and individual contributors
+Copyright (c) 2001-2002 Enthought, Inc. 2003-2019, SciPy Developers
+Copyright (c) 2008 Stefan van der Walt <stefan@mentat.za.net> , Pauli Virtanen <pav@iki.fi>
+Copyright (c) 2015 Min RK, Florian Rathgeber, Michael McNeil Forbes 2019 Casper da Costa-Luis
 
-BSD-2-Clause AND ISC
+BSD-2-Clause AND BSD-3-Clause
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-matplotlib-inline 0.1.6 - BSD-3-Clause
+threadpoolctl 3.2.0 - BSD-2-Clause AND BSD-3-Clause
 
 
-Copyright (c) IPython Development Team
-Copyright (c) 2019-2022, IPython Development Team
+Copyright (c) 2017, Intel Corporation
+(Copyright (c) 2017, Intel Corporation)
+Copyright (c) 2019, threadpoolctl contributors
 
-Copyright (c) <year> <owner> . All rights reserved.
+BSD-2-Clause AND BSD-3-Clause
 
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+---------------------------------------------------------
 
-   1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+---------------------------------------------------------
 
-   2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+requests-oauthlib 1.3.1 - BSD-2-Clause AND ISC
 
-   3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+copyright u'2014, Kenneth Reitz
+Copyright (c) 2014 Kenneth Reitz
 
----------------------------------------------------------
+BSD-2-Clause AND ISC
 
 ---------------------------------------------------------
 
-ultralytics/yolov5 4fce0096fa2f2dc7db12b422200009362de9a056 - GPL-3.0 AND GPL-3.0-only
-
-
-Copyright (c) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+---------------------------------------------------------
 
-GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+protobuf 3.20.2 - BSD-3-Clause
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+Copyright 2007 Google Inc.
+Copyright 2008 Google Inc.
 
-Also add information on how to contact you by electronic and paper mail.
+Copyright (c) <year> <owner> . All rights reserved.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
+   1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+   2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
+   3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pillow 9.4.0 - HPND
+pillow 10.0.0 - HPND
 
 
 (c) Tavmjung Bah
 Copyright 2020 Google LLC
 Copyright 2014 Google Inc.
 Copyright 2016 Google Inc.
 Copyright (c) 2018 Google LLC
@@ -5420,24 +5860,24 @@
 Copyright International Color Consortium, 2009
 Portions Copyright 1988 Digital Equipment Corp.
 Copyright (c) 1998-2000 by Scriptics Corporation
 Copyright (c) 2020 Free Software Foundation, Inc.
 Copyright (c) 2016 Marcin Kurczewski <rr-@sakuya.pl>
 Portions Copyright 1988 Digital Equipment Corporation
 Copyright (c) 2010 Oliver Tonnhofer <olt@bogosoft.com>
-Copyright (c) 2010-2023 by Alex Clark and contributors
 Copyright (c) 2014 Dov Grobgeld <dov.grobgeld@gmail.com>
 Copyright 2013 Google Inc.Noto Color EmojiRegularVersion
 Copyright (c) 2018 Roel Nieskens, https://pixelambacht.nl
-Copyright (c) 2016-2022 Khaled Hosny <khaled@aliftype.com>
+Copyright (c) 2016-2023 Khaled Hosny <khaled@aliftype.com>
 copyright 2003 kevin_cazabon@hotmail.com kevin@cazabon.com
 Copyright (c) 1987-1994 The Regents of the University of California
-copyright 1995-2011 Fredrik Lundh, 2010-2023 Alex Clark and Contributors
+Copyright (c) 2010-2023 by Jeffrey A. Clark (Alex) and contributors
 Copyright 2002, 2003, 2005, 2008, 2009, 2010, 2012 GNU Freefont contributors
 Copyright (c) 2002-2003 Kevin Cazabon kevin@cazabon.com https://www.cazabon.com
+copyright 1995-2011 Fredrik Lundh, 2010-2023 Jeffrey A. Clark (Alex) and contributors
 Portions copyright 1997, 2009, 2011 American Mathematical Society <http://www.ams.org>
 Copyright 2002, 2003, 2005, 2008, 2009, 2010, 2012 GNU Freefont contributors. FreeMono FreeMono
 copyrighted by the Regents of the University of California, Sun Microsystems, Inc., Scriptics Corporation
 Copyright 2016 Adobe (http://www.adobe.com/).Adobe Variable Font PrototypeRegular1.004 ADBO AdobeVFPrototype-Default ADOBEVersion
 Copyright 2014, 2015 Adobe Systems Incorporated (http://www.adobe.com/).Noto Sans JP RegularRegular1.004 GOOG NotoSansJP-Regular ADOBEVersion
 copyright 2010-2011, Google Corporation.Open Sans Condensed LightItalic1.10 1ASC OpenSansCondensed-LightItalicOpen Sans Condensed Light ItalicVersion
 
@@ -5722,21 +6162,22 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-attrs 22.2.0 - MIT
+attrs 23.1.0 - MIT
 
 
 (c) N Revealed
 Hynek Schlawack copyright f'2015
 Copyright (c) 2015 Hynek Schlawack
 Copyright (c) 2015 Hynek Schlawack"
+Copyright (c) 2015 Hynek Schlawack" == mod.__copyright
 Copyright ..." is shown in the HTML footer. Default is True.
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -5745,18 +6186,17 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-azure-core 1.26.3 - MIT
+cffi 1.15.1 - MIT
 
 
-Copyright (c) Microsoft Corporation
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5764,17 +6204,25 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-cffi 1.15.1 - MIT
+charset-normalizer 3.2.0 - MIT
 
 
+COPYRIGHT (c) FOOBAR
+copyright 2019, Ahmed TAHRI
+Copyright (c) 2019 TAHRI Ahmed R.
+copyright (c) 2021 by Ahmed TAHRI
+Copyright (c) 2019 Ahmed TAHRI Ousret
+(c) 2012 Denny Vrandecic (http://simia.net/letters/)
+Copyright (c) Ahmed TAHRI Ousret (https://github.com/Ousret)
+(c) https://stackoverflow.com/questions/3041986/apt-command-line-interface-like-yes-no-input
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5782,15 +6230,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-dotnetcore2 3.1.23 - MIT
+coloredlogs 15.0.1 - MIT
 
 
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
@@ -5800,15 +6248,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-humanfriendly 10.0 - MIT
+dotnetcore2 3.1.23 - MIT
 
 
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
@@ -5818,19 +6266,17 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-jeepney 0.8.0 - MIT
+dotty-dict 1.3.1 - MIT
 
 
-copyright 2017, Thomas Kluyver
-Copyright (c) 2017 Thomas Kluyver
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5838,18 +6284,20 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-jmespath 0.10.0 - MIT
+humanfriendly 10.0 - MIT
 
 
-Copyright (c) 2013 Amazon.com, Inc.
+(c) 2021 Peter Odding
+copyright 2021, Peter Odding
+Copyright (c) 2021 Peter Odding
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5857,20 +6305,19 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-jsonschema 4.17.3 - MIT
+jeepney 0.8.0 - MIT
 
 
-Julian Berman copyright 2013
-Copyright (c) 2012 Julian Berman
-Copyright (c) 2013 Julian Berman
+copyright 2017, Thomas Kluyver
+Copyright (c) 2017 Thomas Kluyver
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5878,18 +6325,18 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-knack 0.10.1 - MIT
+jmespath 1.0.1 - MIT
 
 
-Copyright (c) Microsoft Corporation
+Copyright (c) 2013 Amazon.com, Inc. or its affiliates
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5897,18 +6344,20 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-msal 1.21.0 - MIT
+jsonschema 4.17.3 - MIT
 
 
-Copyright (c) Microsoft Corporation
+Julian Berman copyright 2013
+Copyright (c) 2012 Julian Berman
+Copyright (c) 2013 Julian Berman
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5916,15 +6365,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-msal-extensions 1.0.0 - MIT
+knack 0.10.1 - MIT
 
 
 Copyright (c) Microsoft Corporation
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
@@ -5935,17 +6384,21 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-msrest 0.7.1 - MIT
+markdown-it-py 3.0.0 - MIT
 
 
+Copyright 2021 Taneli Hukkinen
+Copyright (c) 2020 ExecutableBookProject
+Copyright (c) 2014 Vitaly Puzrin, Alex Kocharin
+Copyright 2014 Mathias Bynens <https://mathiasbynens.be/>
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5953,28 +6406,20 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pathlib2 2.3.7.post1 - MIT
+mdurl 0.1.2 - MIT
 
 
-Copyright 2007-2021 by the Sphinx team
-(c) JS Foundation and other contributors
-Copyright JS Foundation and other contributors
-Copyright (c) 2014-2017 Matthias C. M. Troffaes
-Copyright (c) 2014-2021 Matthias C. M. Troffaes
-Copyright (c) 2012-2014 Antoine Pitrou and contributors
-Copyright (c) 2014-2021 Matthias C. M. Troffaes and contributors
-(c) 2012-2014 Antoine Pitrou and contributors 2014-2021, Matthias C. M. Troffaes and contributors
-copyright 2012-2014 Antoine Pitrou and contributors 2014-2021, Matthias C. M. Troffaes and contributors
-copyright ^2012-2014 Antoine Pitrou and contributors 2014-2021, Matthias C. M. Troffaes and contributors
-(c) 2009-2021 Jeremy Ashkenas, Julian Gonggrijp, and DocumentCloud and Investigative Reporters & Editors Underscore
+Copyright (c) 2021 Taneli Hukkinen
+Copyright (c) 2015 Vitaly Puzrin, Alex Kocharin
+Copyright Joyent, Inc. and other Node contributors
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -5982,19 +6427,18 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pkginfo 1.9.6 - MIT
+msal 1.21.0 - MIT
 
 
-copyright u'2009-2013, Tres Seaver
-Copyright (c) 2009 Agendaless Consulting, Inc.
+Copyright (c) Microsoft Corporation
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6002,20 +6446,18 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyjwt 2.6.0 - MIT
+msal-extensions 1.0.0 - MIT
 
 
-Copyright 2015-2022 Jose Padilla
-copyright 2015-2022, Jose Padilla
-Copyright (c) 2015-2022 Jose Padilla
+Copyright (c) Microsoft Corporation
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6023,85 +6465,17 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyparsing 3.0.9 - MIT
+msrest 0.7.1 - MIT
 
 
-Copyright 2004-2010
-Copyright, Tom Coonan
-Copyright (c) 2021 Dot
-Copyright 2004, Paul McGuire
-Copyright 2006, Paul McGuire
-Copyright 2008 Chris Lambrou
-Copyright 2008, Paul McGuire
-Copyright 2010, Paul McGuire
-Copyright 2011, Paul McGuire
-Copyright 2015, Paul McGuire
-Copyright 2016, Paul McGuire
-Copyright 2018, Paul McGuire
-Copyright 2019, Paul McGuire
-Copyright 2020, Paul McGuire
-Copyright 2021, Paul McGuire
-Copyright Paul McGuire, 2019
-Copyright Paul McGuire, 2021
-copyright 2006, Paul McGuire
-Copyright, 2010, Paul McGuire
-Copyright 2007 by Paul McGuire
-Copyright, 2007 - Paul McGuire
-Copyright, 2012 - Paul McGuire
-Copyright 2006, by Paul McGuire
-Copyright 2008, by Paul McGuire
-Copyright 2012, Paul T. McGuire
-Copyright 2022, by Paul McGuire
-Copyright (c) 2003, Paul McGuire
-Copyright (c) 2004, Paul McGuire
-Copyright (c) 2006, Paul McGuire
-Copyright (c) 2009 Zarko Zivanov
-Copyright (c) 2016, Paul McGuire
-Copyright 2010,2019 Paul McGuire
-Copyright, 2006, by Paul McGuire
-Copyright (c) 2008, InformAsic AB
-Copyright 2002-2021, Paul McGuire
-Copyright 2005-2006, Paul McGuire
-Copyright 2009, 2011 Paul McGuire
-Copyright (c) 2018 Paul T. McGuire
-Copyright Ellis & Grant, Inc. 2005
-Copyright 2003-2019 by Paul McGuire
-Copyright 2011,2015 Paul T. McGuire
-Copyright (c) 2003,2019 Paul McGuire
-Copyright (c) 2006,2016 Paul McGuire
-Copyright 2003, 2019 by Paul McGuire
-Copyright 2004-2016, by Paul McGuire
-Copyright 2007-2011, by Paul McGuire
-Copyright 2010, 2019 by Paul McGuire
-Copyright 2012, 2019 Paul T. McGuire
-copyright 2018-2021, Paul T. McGuire
-Copyright (c) 2003,2016, Paul McGuire
-Copyright (c) 2004, 2006 Paul McGuire
-Copyright (c) 2004-2016, Paul McGuire
-Copyright copy 2003-2022 Paul McGuire
-Copyright (c) 2006, 2016, Paul McGuire
-Copyright (c) 2006, 2019, Paul McGuire
-Copyright (c) 2003-2019 Paul T. McGuire
-Copyright (c) 2003-2022 Paul T. McGuire
-Copyright (c) 2004-2011 Paul T. McGuire
-Copyright (c) 1992-1993 Jean-loup Gailly
-Copyright (c) 2006, Estrate, the Netherlands
-Copyright 1989 by Carnegie Mellon University
-Copyright (c) 2000 Rudolf Usselmann rudi@asics.ws
-Copyright (c) 2006 Tim Cera timcera@earthlink.net
-Copyright Petri Savolainen <firstname.lastname@iki.fi>
-copyright 1999, Kluwer Academic Publishers, Norwell, MA
-Copyright 2004, by Alberto Santini http://www.albertosantini.it/chess
-copyright 1998, Sutherland HDL Inc, Portland, Oregon, USA Contact www.sutherland.com
-Copyright (c) 1999 Fulvio Corno, Matteo Sonze Reorda, Giovanni Squillero Politecnico di Torino
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6109,18 +6483,18 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pytz 2022.7.1 - MIT
+msrestazure 0.6.4 - MIT
 
 
-Copyright (c) 2003-2019 Stuart Bishop <stuart@stuartbishop.net>
+Copyright (c) Microsoft Corporation.
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6128,19 +6502,18 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pyyaml 6.0 - MIT
+ordered-set 4.1.0 - MIT
 
 
-Copyright (c) 2017-2021 Ingy dot Net
-Copyright (c) 2006-2016 Kirill Simonov
+Copyright (c) 2012-2022 Elia Robyn Lake
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6148,17 +6521,28 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-qudida 0.0.4 - MIT
+pathlib2 2.3.7.post1 - MIT
 
 
+Copyright 2007-2021 by the Sphinx team
+(c) JS Foundation and other contributors
+Copyright JS Foundation and other contributors
+Copyright (c) 2014-2017 Matthias C. M. Troffaes
+Copyright (c) 2014-2021 Matthias C. M. Troffaes
+Copyright (c) 2012-2014 Antoine Pitrou and contributors
+Copyright (c) 2014-2021 Matthias C. M. Troffaes and contributors
+(c) 2012-2014 Antoine Pitrou and contributors 2014-2021, Matthias C. M. Troffaes and contributors
+copyright 2012-2014 Antoine Pitrou and contributors 2014-2021, Matthias C. M. Troffaes and contributors
+copyright ^2012-2014 Antoine Pitrou and contributors 2014-2021, Matthias C. M. Troffaes and contributors
+(c) 2009-2021 Jeremy Ashkenas, Julian Gonggrijp, and DocumentCloud and Investigative Reporters & Editors Underscore
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6166,17 +6550,19 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-recordclass 0.14.3 - MIT
+pkginfo 1.9.6 - MIT
 
 
+copyright u'2009-2013, Tres Seaver
+Copyright (c) 2009 Agendaless Consulting, Inc.
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6184,17 +6570,20 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-simplification 0.5.7 - MIT
+pyjwt 2.6.0 - MIT
 
 
+Copyright 2015-2022 Jose Padilla
+copyright 2015-2022, Jose Padilla
+Copyright (c) 2015-2022 Jose Padilla
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6202,19 +6591,19 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-six 1.16.0 - MIT
+pyrsistent 0.19.3 - MIT
 
 
-copyright u'2010-2020, Benjamin Peterson
-Copyright (c) 2010-2020 Benjamin Peterson
+Copyright (c) 2013 Matthew Rocklin
+Copyright (c) 2022 Tobias Gustafsson
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6222,18 +6611,18 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-tabulate 0.9.0 - MIT
+pytz 2023.3 - MIT
 
 
-Copyright (c) 2011-2020 Sergey Astanin and contributors
+Copyright (c) 2003-2019 Stuart Bishop <stuart@stuartbishop.net>
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6241,18 +6630,24 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-terminaltables 3.1.10 - MIT
+pywavelets 1.4.1 - MIT
 
 
-Copyright (c) 2017 Robpol86
+Copyright (c) 2016 Holger Nahrstaedt
+copyright 2006- s, The PyWavelets Developers
+Copyright (c) 2006-2012 Filip Wasilewski <http://en.ig.ma/>
+Copyright (c) 2017 The PyWavelets Developers <https://github.com/PyWavelets/pywt>
+Copyright (c) 2012-2016 The PyWavelets Developers <https://github.com/PyWavelets/pywt>
+Copyright (c) 2012-2018 The PyWavelets Developers <https://github.com/PyWavelets/pywt>
+Copyright (c) 2012-2020 The PyWavelets Developers <https://github.com/PyWavelets/pywt>
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6260,22 +6655,17 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-urllib3 1.26.14 - MIT
+qudida 0.0.4 - MIT
 
 
-Copyright 2015 Google Inc.
-Copyright (c) 2010-2020 Benjamin Peterson
-Copyright (c) 2015-2016 Will Bond <will@wbond.net>
-Copyright (c) 2008-2020 Andrey Petrov and contributors
-Copyright (c) 2012 Senko Rasic <senko.rasic@dobarkod.hr>
 
 MIT License
 
 Copyright (c) <year> <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
@@ -6283,194 +6673,170 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-certifi 2022.12.7 - MPL-2.0
-
-
-(c) 2006 Entrust, Inc.
-(c) 1999 Entrust.net Limited
-(c) 2009 Entrust, Inc. - for
-(c) 2012 Entrust, Inc. - for
-(c) 2015 Entrust, Inc. - for
-(c) 2006 Entrust, Inc. Label Entrust Root Certification
-(c) 1999 Entrust.net Limited Label Entrust.net Premium 2048 Secure Server CA Serial
-
-Mozilla Public License Version 2.0
-
-   1. Definitions
-
-      1.1. "Contributor" means each individual or legal entity that creates, contributes to the creation of, or owns Covered Software.
-
-      1.2. "Contributor Version" means the combination of the Contributions of others (if any) used by a Contributor and that particular Contributor's Contribution.
-
-      1.3. "Contribution" means Covered Software of a particular Contributor.
+recordclass 0.14.3 - MIT
 
-      1.4. "Covered Software" means Source Code Form to which the initial Contributor has attached the notice in Exhibit A, the Executable Form of such Source Code Form, and Modifications of such Source Code Form, in each case including portions thereof.
 
-      1.5. "Incompatible With Secondary Licenses" means
 
-         (a) that the initial Contributor has attached the notice described in Exhibit B to the Covered Software; or
+MIT License
 
-         (b) that the Covered Software was made available under the terms of version 1.1 or earlier of the License, but not also under the terms of a Secondary License.
+Copyright (c) <year> <copyright holders>
 
-      1.6. "Executable Form" means any form of the work other than Source Code Form.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-      1.7. "Larger Work" means a work that combines Covered Software with other material, in a separate file or files, that is not Covered Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-      1.8. "License" means this document.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-      1.9. "Licensable" means having the right to grant, to the maximum extent possible, whether at the time of the initial grant or subsequently, any and all of the rights conveyed by this License.
+---------------------------------------------------------
 
-      1.10. "Modifications" means any of the following:
+---------------------------------------------------------
 
-         (a) any file in Source Code Form that results from an addition to, deletion from, or modification of the contents of Covered Software; or
+rich 13.4.2 - MIT
 
-         (b) any new file in Source Code Form that contains any Covered Software.
 
-      1.11. "Patent Claims" of a Contributor means any patent claim(s), including without limitation, method, process, and apparatus claims, in any patent Licensable by such Contributor that would be infringed, but for the grant of the License, by the making, using, selling, offering for sale, having made, import, or transfer of either its Contributions or its Contributor Version.
+Copyright (c) 2020 Will McGugan
+Copyright (c) Sindre Sorhus <sindresorhus@gmail.com> (sindresorhus.com)
 
-      1.12. "Secondary License" means either the GNU General Public License, Version 2.0, the GNU Lesser General Public License, Version 2.1, the GNU Affero General Public License, Version 3.0, or any later versions of those licenses.
+MIT License
 
-      1.13. "Source Code Form" means the form of the work preferred for making modifications.
+Copyright (c) <year> <copyright holders>
 
-      1.14. "You" (or "Your") means an individual or a legal entity exercising rights under this License. For legal entities, "You" includes any entity that controls, is controlled by, or is under common control with You. For purposes of this definition, "control" means (a) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (b) ownership of more than fifty percent (50%) of the outstanding shares or beneficial ownership of such entity.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-   2. License Grants and Conditions
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-      2.1. Grants
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-      Each Contributor hereby grants You a world-wide, royalty-free, non-exclusive license:
+---------------------------------------------------------
 
-         (a) under intellectual property rights (other than patent or trademark) Licensable by such Contributor to use, reproduce, make available, modify, display, perform, distribute, and otherwise exploit its Contributions, either on an unmodified basis, with Modifications, or as part of a Larger Work; and
+---------------------------------------------------------
 
-         (b) under Patent Claims of such Contributor to make, use, sell, offer for sale, have made, import, and otherwise transfer either its Contributions or its Contributor Version.
+simplification 0.5.7 - MIT
 
-      2.2. Effective Date
 
-      The licenses granted in Section 2.1 with respect to any Contribution become effective for each Contribution on the date the Contributor first distributes such Contribution.
 
-      2.3. Limitations on Grant Scope
+MIT License
 
-      The licenses granted in this Section 2 are the only rights granted under this License. No additional rights or licenses will be implied from the distribution or licensing of Covered Software under this License. Notwithstanding Section 2.1(b) above, no patent license is granted by a Contributor:
+Copyright (c) <year> <copyright holders>
 
-         (a) for any code that a Contributor has removed from Covered Software; or
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-         (b) for infringements caused by: (i) Your and any other third party's modifications of Covered Software, or (ii) the combination of its Contributions with other software (except as part of its Contributor Version); or
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-         (c) under Patent Claims infringed by Covered Software in the absence of its Contributions.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-      This License does not grant any rights in the trademarks, service marks, or logos of any Contributor (except as may be necessary to comply with the notice requirements in Section 3.4).
+---------------------------------------------------------
 
-      2.4. Subsequent Licenses
+---------------------------------------------------------
 
-      No Contributor makes additional grants as a result of Your choice to distribute the Covered Software under a subsequent version of this License (see Section 10.2) or under the terms of a Secondary License (if permitted under the terms of Section 3.3).
+six 1.16.0 - MIT
 
-      2.5. Representation
 
-      Each Contributor represents that the Contributor believes its Contributions are its original creation(s) or it has sufficient rights to grant the rights to its Contributions conveyed by this License.
+copyright u'2010-2020, Benjamin Peterson
+Copyright (c) 2010-2020 Benjamin Peterson
 
-      2.6. Fair Use
+MIT License
 
-      This License is not intended to limit any rights You have under applicable copyright doctrines of fair use, fair dealing, or other equivalents.
+Copyright (c) <year> <copyright holders>
 
-      2.7. Conditions
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-      Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted in Section 2.1.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-   3. Responsibilities
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-      3.1. Distribution of Source Form
+---------------------------------------------------------
 
-      All distribution of Covered Software in Source Code Form, including any Modifications that You create or to which You contribute, must be under the terms of this License. You must inform recipients that the Source Code Form of the Covered Software is governed by the terms of this License, and how they can obtain a copy of this License. You may not attempt to alter or restrict the recipients' rights in the Source Code Form.
+---------------------------------------------------------
 
-      3.2. Distribution of Executable Form
+tabulate 0.9.0 - MIT
 
-      If You distribute Covered Software in Executable Form then:
 
-         (a) such Covered Software must also be made available in Source Code Form, as described in Section 3.1, and You must inform recipients of the Executable Form how they can obtain a copy of such Source Code Form by reasonable means in a timely manner, at a charge no more than the cost of distribution to the recipient; and
+Copyright (c) 2011-2020 Sergey Astanin and contributors
 
-         (b) You may distribute such Executable Form under the terms of this License, or sublicense it under different terms, provided that the license for the Executable Form does not attempt to limit or alter the recipients' rights in the Source Code Form under this License.
+MIT License
 
-      3.3. Distribution of a Larger Work
+Copyright (c) <year> <copyright holders>
 
-      You may create and distribute a Larger Work under terms of Your choice, provided that You also comply with the requirements of this License for the Covered Software. If the Larger Work is a combination of Covered Software with a work governed by one or more Secondary Licenses, and the Covered Software is not Incompatible With Secondary Licenses, this License permits You to additionally distribute such Covered Software under the terms of such Secondary License(s), so that the recipient of the Larger Work may, at their option, further distribute the Covered Software under the terms of either this License or such Secondary License(s).
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-      3.4. Notices
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-      You may not remove or alter the substance of any license notices (including copyright notices, patent notices, disclaimers of warranty, or limitations of liability) contained within the Source Code Form of the Covered Software, except that You may alter any license notices to the extent required to remedy known factual inaccuracies.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-      3.5. Application of Additional Terms
+---------------------------------------------------------
 
-      You may choose to offer, and to charge a fee for, warranty, support, indemnity or liability obligations to one or more recipients of Covered Software. However, You may do so only on Your own behalf, and not on behalf of any Contributor. You must make it absolutely clear that any such warranty, support, indemnity, or liability obligation is offered by You alone, and You hereby agree to indemnify every Contributor for any liability incurred by such Contributor as a result of warranty, support, indemnity or liability terms You offer. You may include additional disclaimers of warranty and limitations of liability specific to any jurisdiction.
+---------------------------------------------------------
 
-   4. Inability to Comply Due to Statute or Regulation
+terminaltables 3.1.10 - MIT
 
-   If it is impossible for You to comply with any of the terms of this License with respect to some or all of the Covered Software due to statute, judicial order, or regulation then You must: (a) comply with the terms of this License to the maximum extent possible; and (b) describe the limitations and the code they affect. Such description must be placed in a text file included with all distributions of the Covered Software under this License. Except to the extent prohibited by statute or regulation, such description must be sufficiently detailed for a recipient of ordinary skill to be able to understand it.
 
-   5. Termination
+Copyright (c) 2017 Robpol86
 
-      5.1. The rights granted under this License will terminate automatically if You fail to comply with any of its terms. However, if You become compliant, then the rights granted under this License from a particular Contributor are reinstated (a) provisionally, unless and until such Contributor explicitly and finally terminates Your grants, and (b) on an ongoing basis, if such Contributor fails to notify You of the non-compliance by some reasonable means prior to 60 days after You have come back into compliance. Moreover, Your grants from a particular Contributor are reinstated on an ongoing basis if such Contributor notifies You of the non-compliance by some reasonable means, this is the first time You have received notice of non-compliance with this License from such Contributor, and You become compliant prior to 30 days after Your receipt of the notice.
+MIT License
 
-      5.2. If You initiate litigation against any entity by asserting a patent infringement claim (excluding declaratory judgment actions, counter-claims, and cross-claims) alleging that a Contributor Version directly or indirectly infringes any patent, then the rights granted to You by any and all Contributors for the Covered Software under Section 2.1 of this License shall terminate.
+Copyright (c) <year> <copyright holders>
 
-      5.3. In the event of termination under Sections 5.1 or 5.2 above, all end user license agreements (excluding distributors and resellers) which have been validly granted by You or Your distributors under this License prior to termination shall survive termination.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-   6. Disclaimer of Warranty
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-   Covered Software is provided under this License on an "as is" basis, without warranty of any kind, either expressed, implied, or statutory, including, without limitation, warranties that the Covered Software is free of defects, merchantable, fit for a particular purpose or non-infringing. The entire risk as to the quality and performance of the Covered Software is with You. Should any Covered Software prove defective in any respect, You (not any Contributor) assume the cost of any necessary servicing, repair, or correction. This disclaimer of warranty constitutes an essential part of this License. No use of any Covered Software is authorized under this License except under this disclaimer.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-   7. Limitation of Liability
+---------------------------------------------------------
 
-   Under no circumstances and under no legal theory, whether tort (including negligence), contract, or otherwise, shall any Contributor, or anyone who distributes Covered Software as permitted above, be liable to You for any direct, indirect, special, incidental, or consequential damages of any character including, without limitation, damages for lost profits, loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses, even if such party shall have been informed of the possibility of such damages. This limitation of liability shall not apply to liability for death or personal injury resulting from such party's negligence to the extent applicable law prohibits such limitation. Some jurisdictions do not allow the exclusion or limitation of incidental or consequential damages, so this exclusion and limitation may not apply to You.
+---------------------------------------------------------
 
-   8. Litigation
+urllib3 1.26.15 - MIT
 
-   Any litigation relating to this License may be brought only in the courts of a jurisdiction where the defendant maintains its principal place of business and such litigation shall be governed by laws of that jurisdiction, without reference to its conflict-of-law provisions. Nothing in this Section shall prevent a party's ability to bring cross-claims or counter-claims.
 
-   9. Miscellaneous
+Copyright 2015 Google Inc.
+Copyright (c) 2010-2020 Benjamin Peterson
+Copyright (c) 2015-2016 Will Bond <will@wbond.net>
+Copyright (c) 2008-2020 Andrey Petrov and contributors
+Copyright (c) 2012 Senko Rasic <senko.rasic@dobarkod.hr>
 
-   This License represents the complete agreement concerning the subject matter hereof. If any provision of this License is held to be unenforceable, such provision shall be reformed only to the extent necessary to make it enforceable. Any law or regulation which provides that the language of a contract shall be construed against the drafter shall not be used to construe this License against a Contributor.
+MIT License
 
-   10. Versions of the License
+Copyright (c) <year> <copyright holders>
 
-      10.1. New Versions
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-      Mozilla Foundation is the license steward. Except as provided in Section 10.3, no one other than the license steward has the right to modify or publish new versions of this License. Each version will be given a distinguishing version number.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-      10.2. Effect of New Versions
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-      You may distribute the Covered Software under the terms of the version of the License under which You originally received the Covered Software, or under the terms of any subsequent version published by the license steward.
+---------------------------------------------------------
 
-      10.3. Modified Versions
+---------------------------------------------------------
 
-      If you create software not governed by this License, and you want to create a new license for such software, you may create and use a modified version of this License if you rename the license and remove any references to the name of the license steward (except to note that such modified license differs from this License).
+zipp 3.16.2 - MIT
 
-      10.4. Distributing Source Code Form that is Incompatible With Secondary Licenses
 
-      If You choose to distribute Source Code Form that is Incompatible With Secondary Licenses under the terms of this version of the License, the notice described in Exhibit B of this License must be attached. Exhibit A - Source Code Form License Notice
 
-This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
+MIT License
 
-If it is not possible or desirable to put the notice in a particular file, then You may include the notice in a location (such as a LICENSE file in a relevant directory) where a recipient would be likely to look for such a notice.
+Copyright (c) <year> <copyright holders>
 
-You may add additional accurate notices of copyright ownership.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-Exhibit B - "Incompatible With Secondary Licenses" Notice
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-This Source Code Form is "Incompatible With Secondary Licenses", as defined by the Mozilla Public License, v. 2.0.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pathspec 0.11.0 - MPL-2.0
+pathspec 0.11.1 - MPL-2.0
 
 
 Copyright (c) 2013-2023 Caleb P. Burns credits dahlia <https://github.com/dahlia>
 
 Mozilla Public License Version 2.0
 
    1. Definitions
@@ -6635,17 +7001,91 @@
 
 This Source Code Form is "Incompatible With Secondary Licenses", as defined by the Mozilla Public License, v. 2.0.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-pywin32 227 - PSF-2.0
+matplotlib 3.7.1 - PSF-2.0
 
 
+(c) Tavmjong Bah
+(c) Tavmjung Bah
+Copyright Font's
+Copyright xa9 2017
+b'Copyright xa9 2017
+(c) Frank Siegert 1996
+(c) 2003 by Bitstream, Inc.
+Copyright <http://www.ams.org>
+X11R4 release, copyright M.I.T.
+Copyright (c) 2010 Doug Hellmann
+Copyright 2010-2012, Google Inc.
+Copyright (c) 2002 Hansruedi Baer
+Copyright (c) 2003 Hansruedi Baer
+Copyright (c) 2009 Pierre Raybaut
+Copyright (c) 2006 by Tavmjong Bah
+Copyright (c) 2007-2008 Permission
+Copyright (c) 2011 Ethan Schoonover
+Copyright (c) 2002 by Kevin B. Kenny
+Copyright (c) 1994, Basil K. Malyshev
+Copyright (c) 2003 by Bitstream, Inc.
+Copyright (c) 2010, Bartosz Telenczuk
+copyright 2014, Matplotlib developers
+(c) 2001-2010 by the STI Pub Companies
+Copyright (c) 2002-2011 John D. Hunter
+ECopyright (c) 2003 by Bitstream, Inc.
+FCopyright (c) 2003 by Bitstream, Inc.
+Copyright (c) 2001-2004 by Fredrik Lundh
+Copyright (c) 2002-2005 Maxim Shemanarev
+Copyright 2004 John Gill and John Hunter
+Copyright The Matplotlib development team
+Copyright (c) 1993-1996 Lucent Technologies
+Copyright (c) 1994, 1995, Basil K. Malyshev
+Portions copyright (c) 1990 by Elsevier, Inc.
+Copyright (c) 1994-1998 Sun Microsystems, Inc.
+Copyright (c) 2012- Matplotlib Development Team
+Copyright (c) 1997 American Mathematical Society
+Copyright (c) 1998-2000 by Scriptics Corporation
+Copyright (c) 2001-2005 by the STI Pub Companies
+Copyright (c) 2001-2010 by the STI Pub Companies
+Copyright 1995, Trinity College Computing Center
+LCopyright (c) 2001-2010 by the STI Pub Companies
+Copyright (c) 1989, 1991 Adobe Systems Incorporated
+Copyright (c) 2010-2013 by tyPoland Lukasz Dziedzic
+Copyright (c) 2005 Tony Juricic (tonygeek@yahoo.com)
+Portions copyright (c) 1998-2003 by MicroPress, Inc.
+Copyright (c) Jeremy O'Donoghue & John Hunter, 2003-4
+Copyright (c) 1997, 2009 American Mathematical Society
+(c) Copyright 1989-1992, Bitstream Inc., Cambridge, MA.
+Copyright 1990 as an unpublished work by Bitstream Inc.
+Copyright (c) 1985, 1987, 1988 Adobe Systems Incorporated
+Copyright (c) 1989, 1990, 1991 Adobe Systems Incorporated
+Copyright (c) 1989, 1990, 1991, Adobe Systems Incorporated
+Copyright (c) 2009 John Horigan (http://www.antigrain.com)
+Copyright 2020- by the Matplotlib development team. :license
+Copyright (c) 1985, 1987, 1988, 1989 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1988, 1991 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1989, 1990 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1989, 1991 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1989, 1992 Adobe Systems Incorporated
+Copyright (c) 1996. The Regents of the University of California
+Copyright (c) 2002-2005 Maxim Shemanarev (http://antigrain.com/)
+Copyright (c) 2003-2004 Andrew Straw, Jeremy O'Donoghue and others
+Copyright (c) 1987-1994 The Regents of the University of California
+Copyright (c) 2002-2005 Maxim Shemanarev (http://www.antigrain.com)
+Copyright (c) 1985, 1987, 1988, 1989, 1997 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1989, 1990, 1991 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1989, 1990, 1997 Adobe Systems Incorporated
+Copyright (c) 1989, 1990, 1991, 1993, 1997 Adobe Systems Incorporated
+Copyright (c) 1985, 1987, 1989, 1990, 1993, 1997 Adobe Systems Incorporated
+Copyright (c) 1989, 1990, 1991, 1992, 1993, 1997 Adobe Systems Incorporated
+Copyright (c) 1997, 2009, American Mathematical Society (http://www.ams.org)
+Copyright (c) 2002 Cynthia Brewer, Mark Harrower, and The Pennsylvania State University
+copyrighted by the Regents of the University of California, Sun Microsystems, Inc., Scriptics Corporation
+copyright 2002-2012 John Hunter, Darren Dale, Eric Firing, Michael Droettboom and the Matplotlib development team f'2012- sourceyear The Matplotlib development team
 
 PSF-2.0
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
@@ -6927,76 +7367,18 @@
 
 STICHTING MATHEMATISCH CENTRUM DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS, IN NO EVENT SHALL STICHTING MATHEMATISCH CENTRUM BE LIABLE FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 ---------------------------------------------------------
 
 ---------------------------------------------------------
 
-typing-extensions 4.5.0 - Python-2.0
+typing-extensions 4.7.1 - Python-2.0.1
 
 
 Copyright (c) 1995-2001 Corporation for National Research Initiatives
 Copyright (c) 1991 - 1995, Stichting Mathematisch Centrum Amsterdam, The Netherlands
-Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022 Python Software Foundation
-
-PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
-
-   1. This LICENSE AGREEMENT is between the Python Software Foundation ("PSF"), and the Individual or Organization ("Licensee") accessing and otherwise using this software ("Python") in source or binary form and its associated documentation.
-
-   2. Subject to the terms and conditions of this License Agreement, PSF hereby grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce, analyze, test, perform and/or display publicly, prepare derivative works, distribute, and otherwise use Python alone or in any derivative version, provided, however, that PSF's License Agreement and PSF's notice of copyright, i.e., "Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006 Python Software Foundation; All Rights Reserved" are retained in Python alone or in any derivative version prepared by Licensee.
-
-   3. In the event Licensee prepares a derivative work that is based on or incorporates Python or any part thereof, and wants to make the derivative work available to others as provided herein, then Licensee hereby agrees to include in any such work a brief summary of the changes made to Python.
-
-   4. PSF is making Python available to Licensee on an "AS IS" basis. PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED. BY WAY OF EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
-
-   5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON, OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-   6. This License Agreement will automatically terminate upon a material breach of its terms and conditions.
+Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023 Python Software Foundation
 
-   7. Nothing in this License Agreement shall be deemed to create any relationship of agency, partnership, or joint venture between PSF and Licensee. This License Agreement does not grant permission to use PSF trademarks or trade name in a trademark sense to endorse or promote products or services of Licensee, or any third party.
-
-   8. By copying, installing or otherwise using Python, Licensee agrees to be bound by the terms and conditions of this License Agreement. BEOPEN.COM LICENSE AGREEMENT FOR PYTHON 2.0
-
-BEOPEN PYTHON OPEN SOURCE LICENSE AGREEMENT VERSION 1
-
-   1. This LICENSE AGREEMENT is between BeOpen.com ("BeOpen"), having an office at 160 Saratoga Avenue, Santa Clara, CA 95051, and the Individual or Organization ("Licensee") accessing and otherwise using this software in source or binary form and its associated documentation ("the Software").
-
-   2. Subject to the terms and conditions of this BeOpen Python License Agreement, BeOpen hereby grants Licensee a non-exclusive, royalty-free, world-wide license to reproduce, analyze, test, perform and/or display publicly, prepare derivative works, distribute, and otherwise use the Software alone or in any derivative version, provided, however, that the BeOpen Python License is retained in the Software, alone or in any derivative version prepared by Licensee.
-
-   3. BeOpen is making the Software available to Licensee on an "AS IS" basis. BEOPEN MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED. BY WAY OF EXAMPLE, BUT NOT LIMITATION, BEOPEN MAKES NO AND DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF THE SOFTWARE WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
-
-   4. BEOPEN SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF THE SOFTWARE FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT OF USING, MODIFYING OR DISTRIBUTING THE SOFTWARE, OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-   5. This License Agreement will automatically terminate upon a material breach of its terms and conditions.
-
-   6. This License Agreement shall be governed by and interpreted in all respects by the law of the State of California, excluding conflict of law provisions. Nothing in this License Agreement shall be deemed to create any relationship of agency, partnership, or joint venture between BeOpen and Licensee. This License Agreement does not grant permission to use BeOpen trademarks or trade names in a trademark sense to endorse or promote products or services of Licensee, or any third party. As an exception, the "BeOpen Python" logos available at http://www.pythonlabs.com/logos.html may be used according to the permissions granted on that web page.
-
-   7. By copying, installing or otherwise using the software, Licensee agrees to be bound by the terms and conditions of this License Agreement. CNRI OPEN SOURCE LICENSE AGREEMENT (for Python 1.6b1) IMPORTANT: PLEASE READ THE FOLLOWING AGREEMENT CAREFULLY.
-
-BY CLICKING ON "ACCEPT" WHERE INDICATED BELOW, OR BY COPYING, INSTALLING OR OTHERWISE USING PYTHON 1.6, beta 1 SOFTWARE, YOU ARE DEEMED TO HAVE AGREED TO THE TERMS AND CONDITIONS OF THIS LICENSE AGREEMENT.
-
-   1. This LICENSE AGREEMENT is between the Corporation for National Research Initiatives, having an office at 1895 Preston White Drive, Reston, VA 20191 ("CNRI"), and the Individual or Organization ("Licensee") accessing and otherwise using Python 1.6, beta 1 software in source or binary form and its associated documentation, as released at the www.python.org Internet site on August 4, 2000 ("Python 1.6b1").
-
-   2. Subject to the terms and conditions of this License Agreement, CNRI hereby grants Licensee a non-exclusive, royalty-free, world-wide license to reproduce, analyze, test, perform and/or display publicly, prepare derivative works, distribute, and otherwise use Python 1.6b1 alone or in any derivative version, provided, however, that CNRIs License Agreement is retained in Python 1.6b1, alone or in any derivative version prepared by Licensee.
-
-   Alternately, in lieu of CNRIs License Agreement, Licensee may substitute the following text (omitting the quotes): "Python 1.6, beta 1, is made available subject to the terms and conditions in CNRIs License Agreement. This Agreement may be located on the Internet using the following unique, persistent identifier (known as a handle): 1895.22/1011. This Agreement may also be obtained from a proxy server on the Internet using the URL:http://hdl.handle.net/1895.22/1011".
-
-   3. In the event Licensee prepares a derivative work that is based on or incorporates Python 1.6b1 or any part thereof, and wants to make the derivative work available to the public as provided herein, then Licensee hereby agrees to indicate in any such work the nature of the modifications made to Python 1.6b1.
-
-   4. CNRI is making Python 1.6b1 available to Licensee on an "AS IS" basis. CNRI MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED. BY WAY OF EXAMPLE, BUT NOT LIMITATION, CNRI MAKES NO AND DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON 1.6b1 WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
-
-   5. CNRI SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF THE SOFTWARE FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT OF USING, MODIFYING OR DISTRIBUTING PYTHON 1.6b1, OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-   6. This License Agreement will automatically terminate upon a material breach of its terms and conditions.
-
-   7. This License Agreement shall be governed by and interpreted in all respects by the law of the State of Virginia, excluding conflict of law provisions. Nothing in this License Agreement shall be deemed to create any relationship of agency, partnership, or joint venture between CNRI and Licensee. This License Agreement does not grant permission to use CNRI trademarks or trade name in a trademark sense to endorse or promote products or services of Licensee, or any third party.
-
-   8. By clicking on the "ACCEPT" button where indicated, or by copying, installing or otherwise using Python 1.6b1, Licensee agrees to be bound by the terms and conditions of this License Agreement. ACCEPT CWI LICENSE AGREEMENT FOR PYTHON 0.9.0 THROUGH 1.2
-
-Copyright (c) 1991 - 1995, Stichting Mathematisch Centrum Amsterdam, The Netherlands. All rights reserved.
-
-Permission to use, copy, modify, and distribute this software and its documentation for any purpose and without fee is hereby granted, provided that the above copyright notice appear in all copies and that both that copyright notice and this permission notice appear in supporting documentation, and that the name of Stichting Mathematisch Centrum or CWI not be used in advertising or publicity pertaining to distribution of the software without specific, written prior permission.
-
-STICHTING MATHEMATISCH CENTRUM DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS, IN NO EVENT SHALL STICHTING MATHEMATISCH CENTRUM BE LIABLE FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+Python-2.0.1
 
 ---------------------------------------------------------
```

## azureml/acft/image/components/_version.py

```diff
@@ -1,2 +1,2 @@
-ver = "0.0.9"
-selfver = "0.0.9"
+ver = "47.0.0"
+selfver = "47.0.0"
```

## azureml/acft/image/components/common/utils.py

```diff
@@ -1,20 +1,59 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """Common utils."""
 
+import base64
+import torch
+import urllib.request
+
+from io import BytesIO
+from PIL import Image
+
+from azureml.automl.core.automl_utils import retry_with_backoff
 from azureml.core import Workspace
 from azureml.core.run import Run
 
+from azureml.acft.common_components.utils.logging_utils import get_logger_app
+
+logger = get_logger_app(__name__)
+
 
 def get_workspace() -> Workspace:
     """Get current workspace either from Run or Config.
 
     :return: Current workspace
     :rtype: Workspace
     """
     try:
         ws = Run.get_context().experiment.workspace
         return ws
     except Exception:
         return Workspace.from_config()
+
+
+@retry_with_backoff(retries=3)
+def download_file(url: str, destination: str):
+    """Download file from url to destination.
+    :param url: Url to download from.
+    :type url: str
+    :param destination: Destination to download to.
+    :type destination: str
+    :raises Exception: If download fails.
+    """
+    urllib.request.urlretrieve(url, destination)
+    logger.info(f"Downloaded {url} to {destination}.")
+
+
+def get_random_base64_decoded_image() -> str:
+    """ get random base64 decoded image
+
+    :return: base64 decoded image
+    :rtype: string
+    """
+    buffered = BytesIO()
+    im = torch.rand((256, 256, 3))
+    image = Image.fromarray(im.numpy().astype('uint8'), 'RGB')
+    image.save(buffered, format="JPEG")
+    img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")
+    return img_str
```

## azureml/acft/image/components/finetune/__init__.py

```diff
@@ -1,6 +1,80 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """AzureML ACFT Image Components package - finetuning component."""
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
+
+
+# List of Huggingface models that are not supported by the fine-tuning component. The name of model should be
+# exactly same as model name specified in huggingface model repository.
+UNSUPPORTED_HF_MODEL = [
+
+]
+
+
+# List of MMDetection models that are not supported by the fine-tuning component. The name of model should be
+# exactly same as model name specified in mmdetection metafile.yaml
+# (https://github.com/open-mmlab/mmdetection/tree/v2.28.2/configs).
+UNSUPPORTED_MMDETECTION_MODEL = [
+    # *rcnn_convnext* models are failing due to ModuleNotFoundError: No module named 'mmcls' WI: 2503815
+    "mask-rcnn_convnext-t-p4-w7_fpn_amp-ms-crop-3x_coco",
+    "cascade-mask-rcnn_convnext-t-p4-w7_fpn_4conv1fc-giou_amp-ms-crop-3x_coco",
+    "cascade-mask-rcnn_convnext-s-p4-w7_fpn_4conv1fc-giou_amp-ms-crop-3x_coco",
+    # ga* models are failing with assert exception in evaluation loop. WI: 2500727
+    "ga-rpn_r50-caffe_fpn_1x_coco",
+    "ga-rpn_r101-caffe_fpn_1x_coco",
+    "ga-rpn_x101-32x4d_fpn_1x_coco",
+    "ga-rpn_x101-64x4d_fpn_1x_coco",
+    "ga-faster-rcnn_r50-caffe_fpn_1x_coco",
+    "ga-faster-rcnn_r101-caffe_fpn_1x_coco",
+    "ga-faster-rcnn_x101-32x4d_fpn_1x_coco",
+    "ga-faster-rcnn_x101-64x4d_fpn_1x_coco",
+    "ga-retinanet_r50-caffe_fpn_1x_coco",
+    "ga-retinanet_r101-caffe_fpn_1x_coco",
+    "ga-retinanet_x101-32x4d_fpn_1x_coco",
+    "ga-retinanet_x101-64x4d_fpn_1x_coco",
+
+    # crowddet models are failing due to dataset type mismatch. WI: 2679746
+    # they expect dataset type to be CrowdHumanDataset, but we are using COCODataset
+    "crowddet-rcnn_refine_r50_fpn_8xb2-30e_crowdhuman",
+    "crowddet-rcnn_r50_fpn_8xb2-30e_crowdhuman",
+    # 'InstanceData' object has no attribute 'masks'
+    "faster-rcnn_r50_fpn_carafe_1x_coco",
+    "mask-rcnn_r50_fpn_carafe_1x_coco",
+    # semantic - requires pairwisemasks
+    "htc_r50_fpn_1x_coco",
+    "htc_r101_fpn_20e_coco",
+    "htc_x101-32x4d_fpn_16xb1-20e_coco",
+    "htc_x101-64x4d_fpn_16xb1-20e_coco",
+    "htc_x101-64x4d-dconv-c3-c5_fpn_ms-400-1400-16xb1-20e_coco",
+
+    # maskformer models are not supported due to different format of model config yaml
+    "mask2former_r50_8xb2-lsj-50e_coco",
+    "mask2former_r101_8xb2-lsj-50e_coco",
+    "mask2former_swin-t-p4-w7-224_8xb2-lsj-50e_coco",
+    "mask2former_swin-s-p4-w7-224_8xb2-lsj-50e_coco",
+]
+
+
+UNSUPPORTED_MMTRACKING_MODEL = [
+    # currently do not support joint detection and tracking methods
+    "sort_faster-rcnn_fpn_4e_mot17-public-half",
+    "sort_faster-rcnn_fpn_4e_mot17-private-half",
+    "deepsort_faster-rcnn_fpn_4e_mot17-public-half",
+    "deepsort_faster-rcnn_fpn_4e_mot17-private-half",
+    "qdtrack_faster-rcnn_r50_fpn_4e_mot17-private-half",
+    "qdtrack_faster-rcnn_r50_fpn_4e_crowdhuman_mot17-private-half",
+    "qdtrack_faster-rcnn_r101_fpn_24e_lvis",
+    "qdtrack_faster-rcnn_r101_fpn_12e_tao",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot15-public-half",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot15-private-half",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot16-public-half",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot16-private-half",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot17-public-half",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot17-private-half",
+    "tracktor_faster-rcnn_r50_fpn_4e_mot17-public",
+    "tracktor_faster-rcnn_r50_fpn_8e_mot20-public-half",
+    "tracktor_faster-rcnn_r50_fpn_8e_mot20-public",
+    "tracktor_faster-rcnn_r50_fpn_fp16_4e_mot17-private-half"
+]
```

## azureml/acft/image/components/finetune/finetune_runner.py

```diff
@@ -15,52 +15,67 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """Finetune runner for image tasks."""
 
 import os
+import mlflow
 
 from argparse import Namespace
 from functools import partial
-
+from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 from azureml.acft.accelerator.constants import HfTrainerType
 from azureml.acft.accelerator.finetune import AzuremlDatasetArgs, AzuremlFinetuneArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
-
-from azureml.acft.common_components import get_logger_app
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTSystemError
+from azureml.acft.common_components import get_logger_app, ModelSelectorDefaults, ModelSelectorConstants
+from azureml.acft.common_components.image.runtime_common.common import distributed_utils
+from azureml.acft.common_components.utils.license_utils import save_license_file
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTSystemException
+from azureml.acft.common_components.utils.mlflow_utils import update_acft_metadata
+from azureml.acft.image.components.finetune.common.mlflow.mlflow_save_utils import hf_save_as_mlflow_model
+from azureml.acft.image.components.finetune.common.trainer.train_helper import save_pytorch_model
 from azureml.acft.image.components.finetune.factory.mappings import MODEL_FAMILY_CLS
 from azureml.acft.image.components.finetune.factory.model_factory import ModelFactory
+from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
 from azureml.acft.image.components.finetune.common.constants.constants import (
     SettingLiterals,
+    HfProcessorParamNames, SettingParameters,
 )
-from azureml.evaluate import mlflow
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MetricsLiterals
+# this is needed to handle mlflow tracking uri which startswith azureml
+import azureml.mlflow
 
 logger = get_logger_app(__name__)
 
 
 def finetune_runner(component_args: Namespace) -> None:
     """
     finetune runner for all image tasks
 
     :param component_args: args from the finetune component
     :type component_args: Namespace
     """
-    # importing here after common/mlfow is added to the path.
-    from azureml.acft.image.components.finetune.defaults.training_defaults import (
-        TrainingDefaults,
-    )
 
     logger.info("Starting finetune runner")
     logger.info(f"Task name: {component_args.task_name}")
+    component_args_dict = vars(component_args)
+
+    # fetch metadata to be dumped in MLmodel file/checkpoints
+    metadata = component_args_dict.get(ModelSelectorConstants.MODEL_METADATA, {})
+    metadata = update_acft_metadata(metadata=metadata,
+                                    finetuning_task=component_args.task_name)
+    component_args_dict[ModelSelectorConstants.MODEL_METADATA] = metadata
 
     model_factory = ModelFactory(
         component_args.model_family,
         component_args.model_name_or_path,
         task_name=component_args.task_name,
+        model_metadata=metadata
     )
     trainer_classes_obj = model_factory.get_trainer_classes()
 
     # set the trainer classes
     finetune_cls = trainer_classes_obj.finetune_cls
     image_processor = trainer_classes_obj.tokenizer_cls
     data_cls = trainer_classes_obj.dataset_cls
@@ -69,39 +84,84 @@
     trainer_callbacks = trainer_classes_obj.callbacks
 
     # call the interface
     finetune_obj = finetune_cls(vars(component_args))
 
     # get the component args dict
     custom_finetune_args = finetune_obj.get_finetune_args()
-    component_args_dict = vars(component_args)
     component_args_dict.update(custom_finetune_args)
 
-    # get the training defaults if auto hyperparameter selection is set
-    if component_args_dict.get(SettingLiterals.AUTO_HYPERPARAMETER_SELECTION, False):
-        training_defaults = TrainingDefaults(
-            task=component_args.task_name,
-            model_name_or_path=component_args.model_name_or_path,
-        )
-        component_args_dict.update(training_defaults.defaults_dict)
-
-    # log the component args dict
-    logger.info(f"Component args dict used for training: {component_args_dict}")
+    # Accelerator package uses argument "pytorch_model_folder" to store the model checkpoint and best model at the
+    # end of training. We want to store these models in job's "output" folder. Hence, overriding the value of
+    # "pytorch_model_folder" with job's output folder name. At the end of training, we will copy the best checkpoint
+    # from job's output to user specified pytorch model folder i.e., component_args.pytorch_model_folder before
+    # registering it as pytorch model asset.
+    component_args_dict["pytorch_best_model_folder"] = component_args.pytorch_model_folder if \
+        component_args.pytorch_model_folder != component_args.output_dir else SettingParameters.DEFAULT_PYTORCH_OUTPUT
+    component_args_dict["pytorch_model_folder"] = SettingParameters.DEFAULT_OUTPUT_DIR
 
     # get the custom trainer functions
     custom_trainer_functions = finetune_obj.get_custom_trainer_functions()
 
     # init the tokenizer
     tokenizer = (
         image_processor.from_pretrained(
             component_args.model_name_or_path, **component_args_dict
         )
         if image_processor
         else None
     )
+
+    # tokenizer image width and height would be used if user provided image width and height as -1
+    # This change is specifically for hugging face models.
+    if component_args.model_family == MODEL_FAMILY_CLS.HUGGING_FACE_IMAGE and (
+        component_args_dict[SettingLiterals.IMAGE_HEIGHT] == -1
+        or component_args_dict[SettingLiterals.IMAGE_WIDTH] == -1
+    ):
+        if HfProcessorParamNames.HEIGHT_KEY and HfProcessorParamNames.WIDTH_KEY in tokenizer.size:
+            component_args_dict[SettingLiterals.IMAGE_HEIGHT] = tokenizer.size[HfProcessorParamNames.HEIGHT_KEY]
+            component_args_dict[SettingLiterals.IMAGE_WIDTH] = tokenizer.size[HfProcessorParamNames.WIDTH_KEY]
+        elif (
+            HfProcessorParamNames.SHORTEST_EDGE_KEY in tokenizer.size
+            and HfProcessorParamNames.LONGEST_EDGE_KEY not in tokenizer.size
+        ):
+            component_args_dict[SettingLiterals.IMAGE_HEIGHT] = tokenizer.size[HfProcessorParamNames.SHORTEST_EDGE_KEY]
+            component_args_dict[SettingLiterals.IMAGE_WIDTH] = tokenizer.size[HfProcessorParamNames.SHORTEST_EDGE_KEY]
+        elif (
+            HfProcessorParamNames.LONGEST_EDGE_KEY in tokenizer.size
+            and HfProcessorParamNames.SHORTEST_EDGE_KEY not in tokenizer.size
+        ):
+            component_args_dict[SettingLiterals.IMAGE_HEIGHT] = tokenizer.size[HfProcessorParamNames.LONGEST_EDGE_KEY]
+            component_args_dict[SettingLiterals.IMAGE_WIDTH] = tokenizer.size[HfProcessorParamNames.LONGEST_EDGE_KEY]
+        elif (
+            HfProcessorParamNames.LONGEST_EDGE_KEY in tokenizer.size
+            and HfProcessorParamNames.SHORTEST_EDGE_KEY in tokenizer.size
+        ):
+            if (
+                tokenizer.size[HfProcessorParamNames.LONGEST_EDGE_KEY]
+                == tokenizer.size[HfProcessorParamNames.SHORTEST_EDGE_KEY]
+            ):
+                component_args_dict[SettingLiterals.IMAGE_HEIGHT] = tokenizer.size[
+                    HfProcessorParamNames.LONGEST_EDGE_KEY
+                ]
+                component_args_dict[SettingLiterals.IMAGE_WIDTH] = tokenizer.size[
+                    HfProcessorParamNames.LONGEST_EDGE_KEY
+                ]
+            else:
+                error_string = "Longest edge and shortest edge are not equal in the tokenizer."
+                raise ACFTSystemException._with_error(
+                    AzureMLError.create(ACFTSystemError, pii_safe_message=error_string)
+                )
+        else:
+            error_string = "Default image height and width are not available in the tokenizer."
+            raise ACFTSystemException._with_error(AzureMLError.create(ACFTSystemError, pii_safe_message=error_string))
+
+    # log the component args dict
+    logger.info(f"Component args dict used for training: {component_args_dict}")
+
     data_cls = data_cls(tokenizer=tokenizer, **component_args_dict)
     # set the dataset args
     dataset_args = AzuremlDatasetArgs(
         train_dataset=data_cls.get_train_dataset(),
         validation_dataset=data_cls.get_validation_dataset(),
         data_collator=data_cls.get_collation_function(),
     )
@@ -115,73 +175,89 @@
         **component_args_dict,
     )
 
     if isinstance(model, tuple):
         model, mismatch_info = model
         logger.info(f"Mismatch info: {mismatch_info}")
 
+    if component_args.task_name == Tasks.MM_OBJECT_DETECTION and model.lang_model:
+        component_args_dict[SettingLiterals.DDP_FIND_UNUSED_PARAMETERS] = False
     component_args_dict[SettingLiterals.NUM_LABELS] = len(data_cls.label2id)
 
     azml_finetune_args = AzuremlFinetuneArgs(
         finetune_args=component_args_dict, trainer_type=HfTrainerType.DEFAULT
     )
 
     # Define metric func, send the arguments to the metric function
-    compute_metric_func = (
-        partial(calculate_metrics, **component_args_dict) if calculate_metrics else None
-    )
+    compute_metric_func = None
+    if calculate_metrics:
+        # metric computer is only available for OD and IS models.
+        metrics_computer = model.metrics_computer if hasattr(model, 'metrics_computer') else None
+        calculate_metrics_kwargs = {
+            MetricsLiterals.METRICS_COMPUTER: metrics_computer, **component_args_dict
+        } if metrics_computer else component_args_dict
+        compute_metric_func = partial(calculate_metrics, **calculate_metrics_kwargs)
 
     # init trainer
     azml_trainer = AzuremlTrainer(
         finetune_args=azml_finetune_args,
         dataset_args=dataset_args,
         model=model,
         tokenizer=tokenizer,
         metric_func=compute_metric_func,
         custom_trainer_callbacks=trainer_callbacks,
         custom_trainer_functions=custom_trainer_functions,
         new_initalized_layers=None,
     )
-    azml_trainer.train()
+    master_process = distributed_utils.master_process()
+    try:
+        azml_trainer.train()
+    except Exception:
+        # Let the exception propagate to catch in exception swallow wrapper.
+        raise
+    finally:
+        # Upload local output to job's mlflow run artifact
+        if master_process:
+            mlflow.log_artifacts(component_args.output_dir, SettingParameters.DEFAULT_OUTPUT_DIR)
 
     # saving the mlflow model
-    if component_args.save_as_mlflow_model:
+    if component_args.save_as_mlflow_model and master_process:
         logger.info("saving the mlflow model")
         if component_args.model_family == MODEL_FAMILY_CLS.HUGGING_FACE_IMAGE:
-
-            # In new version azureml_evaluate_mlflow 0.1.0.86769376 package infer the tokenizer class.
-            # Now, we don't need to pass "hf_tokenizer_class": AutoImageProcessor.__name__,
-
-            # In train_label_list, use id2label to get label list. Avoid using label2id as label2id can be
-            # inconsistent if there are two labels with same name (very rare condition). It's observed in google vit
-            # model's default config.
-
-            hf_conf = {
-                "task_type": component_args.task_name,
-                "train_label_list": sorted(list(model.config.id2label.values())),
-                "hf_predict_module": "hf_test_predict",
-            }
-            mlflow_dir = os.path.join(os.path.dirname(__file__), "common", "mlflow")
-            files_to_include = ['common_constants.py', 'common_utils.py', 'hf_test_predict.py']
-            code_paths = [os.path.join(mlflow_dir, x) for x in files_to_include]
-            from mlflow_save_utils import get_mlflow_signature
-            mlflow.hftransformers.save_model(
-                model,
-                component_args.mlflow_model_folder,
-                tokenizer=tokenizer,
-                config=model.config,
-                hf_conf=hf_conf,
-                code_paths=code_paths,
-                signature=get_mlflow_signature(component_args.task_name)
-            )
-        elif component_args.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            hf_save_as_mlflow_model(component_args, model, tokenizer, metadata)
+        elif component_args.model_family in (MODEL_FAMILY_CLS.MMDETECTION_IMAGE, MODEL_FAMILY_CLS.MMTRACKING_VIDEO):
+            # Saving the model artifacts in the output folder
+            # Please note model.state_dict() would not work for ds stage 3. We need to use
+            # state_dict = self.accelerator.get_state_dict(self.deepspeed)
+            # https://github.com/huggingface/transformers/blob/fc63914399b6f60512c720959f9182b02ae4a45c/src/transformers/
+            # trainer.py#L2753C17-L2753C77
+            state_dict = model.state_dict()
+            model.save_pretrained(component_args.output_dir,
+                                  state_dict=state_dict)
             # importing directly from acft package is resulting in our package dependencies.
             from mlflow_save_utils import save_mmdet_mlflow_pyfunc_model
+            if component_args.model_name.endswith(".py"):
+                component_args.model_name = component_args.model_name[:-3]
             save_mmdet_mlflow_pyfunc_model(
-                model_output_dir=component_args.pytorch_model_folder,
+                model_output_dir=component_args.output_dir,
                 mlflow_output_dir=component_args.mlflow_model_folder,
-                model_name=os.path.basename(component_args.model_name).split('.')[0],
+                model_name=os.path.basename(component_args.model_name),
                 task_type=component_args.task_name,
+                metadata=metadata
             )
         else:
             raise NotImplementedError(f"Saving mlflow model is not implemented for this model family\
                 : {component_args.model_family}")
+        logger.info("mlflow model saved successfully.")
+    if master_process:
+        # saving the pytorch model
+        save_pytorch_model(job_output_dir=component_args.output_dir,
+                           pytorch_model_folder=component_args.pytorch_best_model_folder)
+
+        # save the license file in the pytorch, job output and mlflow model folders
+        if MODEL_FAMILY_CLS.MMDETECTION_IMAGE == component_args.model_family:
+            component_args.model_name_or_path = os.path.dirname(component_args.model_name_or_path)
+        save_license_file(
+            model_name_or_path=component_args.model_name_or_path,
+            license_file_name=ModelSelectorDefaults.LICENSE_FILE_NAME,
+            destination_paths=[component_args.pytorch_best_model_folder, component_args.mlflow_model_folder]
+        )
```

## azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py

```diff
@@ -227,14 +227,21 @@
             else:
                 # update img_scale and keep_ratio parameters from model's config.
                 # This is required for MMdetection constraint resize transformation.
                 constraint_resize_params_dict = self.get_image_scale_from_model_preproc_params(
                     phase_name=phase_name
                 )
             return constraint_resize_params_dict
+        elif (
+            augmentation_function_name.lower()
+            == self.augmentation_param_names_cls.PAD_IF_NEEDED_FUNC_NAME.lower()
+        ):
+            # update pad size divisor
+            pad_size_divisor = self.get_pad_size_divisor_from_model_preproc_params()
+            return pad_size_divisor
 
         return dict()
 
 
 class HfModelPreProcExtractor(ModelPreProcExtractor):
     """Helper class to extract parameter update (dict) from model preprocessing config for HF"""
 
@@ -455,18 +462,24 @@
         """Get model preprocessing params for MMDetection
         :param phase_name: Name of the phase - train/valid.
         :type phase_name: str
 
         :return: A dictionary containing model preprocessing params
         :rtype: dict
         """
+        # to handle circular dependency
+        from azureml.acft.image.components.finetune.mmdetection.common.constants import (
+            MmDetectionConfigLiterals
+        )
+
         phase_name_mapping = {
-            AugmentationConfigKeys.TRAINING_PHASE_KEY: AugmentationConfigKeys.TRAINING_PHASE_KEY,
-            AugmentationConfigKeys.VALIDATION_PHASE_KEY: "val",
-            "val": "val"
+            AugmentationConfigKeys.TRAINING_PHASE_KEY: MmDetectionConfigLiterals.TRAIN_PIPELINE,
+            AugmentationConfigKeys.VALIDATION_PHASE_KEY: MmDetectionConfigLiterals.TEST_PIPELINE,
+            "val": "val",
+            AugmentationConfigKeys.MODEL_KEY: MmDetectionConfigLiterals.MODEL
         }
         if phase_name in phase_name_mapping:
             mapped_phase = phase_name_mapping[phase_name]
             return self.model_preprocessing_params.get(mapped_phase, None)
         return None
 
     def _get_step_by_name(self, pipeline: List, step_name: str) -> Dict:
@@ -478,44 +491,64 @@
 
         :return: A dictionary containing the step
         :rtype: Dict
         """
         if not pipeline:
             return {}
         for step in pipeline:
-            if step['type'] == step_name:
+            if isinstance(step, list):
+                for item in step:
+                    if item.get('type', None) == step_name:
+                        return item
+            elif isinstance(step, dict) and step['type'] == step_name:
                 return step
             else:
                 transforms = step.get(MmDetectionPreprocessorParamNames.TRANSFORMS, [])
                 if transforms:
                     normalization_step = self._get_step_by_name(transforms, step_name)
                     if normalization_step:
                         return normalization_step
         return {}
 
+    def get_pad_size_divisor_from_model_preproc_params(self) -> Dict[str, int]:
+        """ Get pad_size_divisor from model's preprocessing params
+
+        :return: A integer denoting the required pad size divisor for the model.
+        :rtype: dict
+        """
+        model_preprocessing_params = self.get_model_preprocessing_params(AugmentationConfigKeys.MODEL_KEY)
+        if model_preprocessing_params:
+            data_preprocess = model_preprocessing_params[MmDetectionPreprocessorParamNames.DATA_PREPROCESSOR]
+            if not data_preprocess or MmDetectionPreprocessorParamNames.PAD_SIZE_DIVISOR not in data_preprocess:
+                return {}
+            pad_size_divisor = data_preprocess.get(MmDetectionPreprocessorParamNames.PAD_SIZE_DIVISOR)
+            pad_size_divisor_dict = {
+                self.augmentation_param_names_cls.PAD_HEIGHT_DIVISOR_KEY: pad_size_divisor,
+                self.augmentation_param_names_cls.PAD_WIDTH_DIVISOR_KEY: pad_size_divisor,
+            }
+            return pad_size_divisor_dict
+        return {}
+
     def get_mean_std_from_model_preproc_params(self, **kwargs) -> Dict[str, List[float]]:
         """ Get mean/std for normalization from model config for MMDetection
 
         :param phase_name: Whether it is training phase or test
         :param type: str
 
         :return: A dictionary containing mean and std extracted from model config
         :rtype: dict
         """
-        phase_name = kwargs[AugmentationConfigKeys.PHASE_NAME]
-        model_preprocessing_params = self.get_model_preprocessing_params(phase_name)
-        if model_preprocessing_params and \
-           MmDetectionPreprocessorParamNames.PIPELINE in model_preprocessing_params:
-            pipeline = model_preprocessing_params[MmDetectionPreprocessorParamNames.PIPELINE]
-            normalization_step = self._get_step_by_name(pipeline, MmDetectionPreprocessorParamNames.NORMALIZE)
-            if not normalization_step:
+        model_preprocessing_params = self.get_model_preprocessing_params(AugmentationConfigKeys.MODEL_KEY)
+        if model_preprocessing_params:
+            data_preprocess = model_preprocessing_params[MmDetectionPreprocessorParamNames.DATA_PREPROCESSOR]
+            if not data_preprocess or MmDetectionPreprocessorParamNames.MEAN_KEY not in data_preprocess:
                 return {}
-            mean = normalization_step.get(MmDetectionPreprocessorParamNames.MEAN_KEY)
-            std = normalization_step.get(MmDetectionPreprocessorParamNames.STD_KEY)
-            to_rgb = normalization_step.get(MmDetectionPreprocessorParamNames.TO_RGB_KEY, True)
+            mean = data_preprocess.get(MmDetectionPreprocessorParamNames.MEAN_KEY)
+            std = data_preprocess.get(MmDetectionPreprocessorParamNames.STD_KEY)
+            to_rgb = data_preprocess.get(MmDetectionPreprocessorParamNames.TO_RGB_KEY, True)
             if not to_rgb:
                 # Whether to convert the image from BGR to RGB
                 mean = mean[::-1]
                 std = std[::-1]
 
             if max(mean) > 1:
                 # If mean and std values are > 1, normalize them to get them on scale between 0 and 1.
@@ -548,18 +581,16 @@
 
         :return: A dictionary containing img_scale and/or keep_ratio extracted from
          feature extractor / preprocess_config
         :rtype: dict
         """
 
         model_preprocessing_params = self.get_model_preprocessing_params(phase_name)
-        if model_preprocessing_params and \
-                MmDetectionPreprocessorParamNames.PIPELINE in model_preprocessing_params:
-            pipeline = model_preprocessing_params[MmDetectionPreprocessorParamNames.PIPELINE]
-            resize_step = self._get_step_by_name(pipeline, MmDetectionPreprocessorParamNames.RESIZE)
+        if model_preprocessing_params:
+            resize_step = self._get_step_by_name(model_preprocessing_params, MmDetectionPreprocessorParamNames.RESIZE)
             aug_constants = self.augmentation_param_names_cls
             if not resize_step:
                 # return empty dict if resize step is not present.
                 return {}
             constraint_resize_params_dict = {}
 
             if aug_constants.KEEP_RATIO in resize_step:
@@ -573,15 +604,15 @@
                 constraint_resize_params_dict = {
                     **constraint_resize_params_dict,
                     aug_constants.CONSTRAINT_RESIZE_KEY: resize_step.get(aug_constants.CONSTRAINT_RESIZE_KEY)
                 }
             else:
                 # Get img_scale from MULTISCALE_FLIP_AUG step
                 multiscale_aug_step = self._get_step_by_name(
-                    pipeline, MmDetectionPreprocessorParamNames.MULTISCALE_FLIP_AUG
+                    model_preprocessing_params, MmDetectionPreprocessorParamNames.MULTISCALE_FLIP_AUG
                 )
                 if aug_constants.CONSTRAINT_RESIZE_KEY in multiscale_aug_step:
                     constraint_resize_params_dict = {
                         **constraint_resize_params_dict,
                         aug_constants.CONSTRAINT_RESIZE_KEY: multiscale_aug_step.get(
                             aug_constants.CONSTRAINT_RESIZE_KEY
                         )
```

## azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml

```diff
@@ -6,14 +6,17 @@
 
 train:
   # # Current set of augmentations for Classification in dnn-vision
   # 1. Random Resize and crop 
   # 2. Horizontal flip 
   # 3. color jitter (brightness=0.4, contrast=0.4, saturation=0.4, hue=0.4) - 50%
   # 4. normalisation using channel wise imagenet's mean and std. 
+  - ToFloat:
+      p: 1
+      always_apply: True
 
   - RandomResizedCrop:
       height: 256 # will be overwritten with "height" from preprocess_config.json from HF
       width: 256  # will be overwritten with "width" from preprocess_config.json from HF
       scale: [0.08, 1.0]
       ratio: [0.75, 1.3333333333333333]
       interpolation: 1 # cv2.INTER aka bilinear
@@ -28,27 +31,31 @@
       contrast: 0.4
       saturation: 0.4
       hue: 0.4
       always_apply: False
       p: 0.5
 
   - Normalize:
-      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preproessing config
-      std: [0.229, 0.224, 0.225]  # will be overwritten with values from model preproessing config
-      max_pixel_value: 255.0
+      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preprocessing config
+      std: [0.229, 0.224, 0.225]  # will be overwritten with values from model preprocessing config
+      max_pixel_value: 1.0
       always_apply: True
       p: 1.0
 
 validation:
+  - ToFloat:
+      p: 1
+      always_apply: True
+
   - Resize:
       height: 256 # will be overwritten with "height" from preprocess_config.json from HF
       width: 256  # will be overwritten with "width" from preprocess_config.json from HF
       interpolation: 1 # cv2.INTER aka bilinear
       always_apply: True
       p: 1
 
   - Normalize:
-      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preproessing config
-      std: [0.229, 0.224, 0.225]  # will be overwritten with values from model preproessing config
-      max_pixel_value: 255.0
+      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preprocessing config
+      std: [0.229, 0.224, 0.225]  # will be overwritten with values from model preprocessing config
+      max_pixel_value: 1.0
       always_apply: True
       p: 1.0
```

## azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml

```diff
@@ -22,61 +22,64 @@
             p: 0.5
         - RandomExpand:
             p: 0.5
 
   - HorizontalFlip:
       p: 0.5
 
+  - Normalize:
+      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preprocessing config
+      # Range of mean and std is [0,1]. In case of MMDetection, if it is more than 1, divide
+      # the values by 255.
+      std: [0.229, 0.224, 0.225] # will be overwritten with values from model preprocessing config
+      max_pixel_value: 1.0
+      always_apply: True
+      p: 1
+
   - ConstraintResize:
       img_scale: [600, 800] # will be overwritten with "img_scale" from model preprocessing config file
       always_apply: True
       p: 1
 
   - PadIfNeeded:
       min_height: null
       min_width: null
       pad_height_divisor: 32
       pad_width_divisor: 32
       border_mode: 0 # cv2.BORDER_CONSTANT
       value: 0      # Value to be used for padding the image
       mask_value: 0 # Value to be used for padding the mask
+      position: top_left # Pad towards the bottom of the image. Postion of the image is top left.
       always_apply: True
       p: 1
 
+
+validation:
+  - ToFloat:
+      p: 1
+      always_apply: True
+
   - Normalize:
-      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preproessing config
+      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preprocessing config 
       # Range of mean and std is [0,1]. In case of MMDetection, if it is more than 1, divide
       # the values by 255.
-      std: [0.229, 0.224, 0.225] # will be overwritten with values from model preproessing config
+      std: [0.229, 0.224, 0.225] # will be overwritten with values from model preprocessing config
       max_pixel_value: 1.0
       always_apply: True
       p: 1
 
-validation:
-  - ToFloat:
-      p: 1
-      always_apply: True
-
   - ConstraintResize:
       img_scale: [600, 800] # will be overwritten with "height" from preprocess_config.json from HF
       always_apply: True
       p: 1
 
   - PadIfNeeded:
       min_height: null
       min_width: null
       pad_height_divisor: 32
       pad_width_divisor: 32
       border_mode: 0 # cv2.BORDER_CONSTANT
       value: 0      # Value to be used for padding the image
       mask_value: 0 # Value to be used for padding the mask
-      always_apply: True
-      p: 1
-
-  - Normalize:
-      mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preproessing config 
-      # Range of mean and std is [0,1]. In case of MMDetection, if it is more than 1, divide
-      # the values by 255.
-      std: [0.229, 0.224, 0.225] # will be overwritten with values from model preproessing config
-      max_pixel_value: 1.0
+      position: top_left # Pad towards the bottom of the image. Postion of the image is top left.
       always_apply: True
       p: 1
```

## azureml/acft/image/components/finetune/common/constants/augmentation_constants.py

```diff
@@ -9,14 +9,16 @@
 
 @dataclass
 class AugmentationConfigKeys:
     """Keys in augmentation configs"""
 
     TRAINING_PHASE_KEY = "train"
     VALIDATION_PHASE_KEY = "validation"
+    VALID_PHASE_KEY = "val"
+    MODEL_KEY = "model"
     AUGMENTATION_LIBRARY_NAME = "augmentation_library_name"
     FUNC_NAME = "augmentation_function_name"
     FUNC_PARAMS_DICT = "augmentation_function_params_dict"
     PHASE_NAME = "phase_name"
     TASK_PARAM_DICT = "task_input_params_dict"
 
 
@@ -24,26 +26,34 @@
 class AugmentationConfigFileNames:
     """Augmentation configs inside config folder at
     src/azureml-acpt-image-components/azureml/train/vision/components/finetune/common/augmentation/
     """
 
     CLASSIFICATION_ALBUMENTATIONS_CONFIG = "configs/albumentations_classification.yaml"
     OD_IS_ALBUMENTATIONS_CONFIG = "configs/albumentations_od_is.yaml"
-    HF_CLASSIFICATION_ALBUMENTATIONS_CONFIG = (
-        "configs/hf_albumentations_classification.yaml"
-    )
 
 
 @dataclass
 class AlbumentationParamNames:
     """Albumentations parameter and function names"""
 
     LIB_NAME = "albumentations"
 
     HEIGHT_KEY = "height"
     WIDTH_KEY = "width"
 
     NORMALIZE_FUNC_NAME = "Normalize"
     MEAN_KEY = "mean"
     STD_KEY = "std"
+    PAD_HEIGHT_DIVISOR_KEY = "pad_height_divisor"
+    PAD_WIDTH_DIVISOR_KEY = "pad_width_divisor"
     CONSTRAINT_RESIZE_KEY = "img_scale"
     KEEP_RATIO = "keep_ratio"
+    PAD_IF_NEEDED_FUNC_NAME = "PadIfNeeded"
+
+
+@dataclass
+class OpenmmlabAugmentationNames:
+    """Openmmlab data augmentation names"""
+    LOAD_ANNOTATIONS = "LoadAnnotations"
+    LOAD_TRACK = "LoadTrack"
+    VIDEO_COLLECT_FOR_MODELS = "VideoCollectForModel"
```

## azureml/acft/image/components/finetune/common/constants/constants.py

```diff
@@ -107,14 +107,26 @@
     IGNORE_DATA_ERRORS = "ignore_data_errors"
     IOU_THRESHOLD = "iou_threshold"
     NUM_LABELS = "num_labels"
     BOX_SCORE_THRESHOLD = "box_score_threshold"
     LABEL_COLUMN_NAME = "label_column_name"
     STREAM_IMAGE_FILES = "stream_image_files"
 
+    # Optimizer
+    WEIGHT_DECAY = "weight_decay"
+    LR = "lr"
+    OPTIMIZER = "optim"
+    EXTRA_OPTIMIZER_ARGS = "extra_optim_args"
+    PARAMS = "params"
+    NESTEROV = "nesterov"
+    MOMENTUM = "momentum"
+
+    # trainer
+    DDP_FIND_UNUSED_PARAMETERS = "ddp_find_unused_parameters"
+
 
 @dataclass
 class HfProcessorParamNames:
     """Hugging face parameter names, primariy in preprocessing_config.json for models"""
 
     # Size related params from preprocess_config.json / FeatureExtractor
     DO_CENTER_CROP_KEY = "do_center_crop"
@@ -147,15 +159,17 @@
     MEAN_KEY = "mean"
     STD_KEY = "std"
     TO_RGB_KEY = "to_rgb"
     PIPELINE = "pipeline"
     NORMALIZE = "Normalize"
     TRANSFORMS = "transforms"
     RESIZE = "Resize"
+    PAD_SIZE_DIVISOR = "pad_size_divisor"
     MULTISCALE_FLIP_AUG = "MultiScaleFlipAug"
+    DATA_PREPROCESSOR = "data_preprocessor"
 
 
 class DetectionDatasetLiterals:
     """Literals for detection dataset"""
 
     HEIGHT = "height"
     WIDTH = "width"
```

## azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py

```diff
@@ -60,15 +60,21 @@
         :type index: int
         :return: Image tensor in de-normalized form [0-255], training labels
         :rtype: Tuple[Tensor, dict]
         """
         image, training_labels = super().__getitem__(index)
 
         if image is None:
-            return None, {}
+            logger.info("Image was not found for a data point in the batch, the data point is marked as invalid.")
+            return None
+        if training_labels is None:
+            logger.info(
+                "Labels were not found for a data point in the batch, the data point is marked as invalid."
+            )
+            return None
 
         if self.transform is not None:
             image = self._apply_transform(image=np.array(image))
 
         example = {
             ImageDataItemLiterals.DEFAULT_IMAGE_KEY: np.asarray(image),
             ImageDataItemLiterals.DEFAULT_LABEL_KEY: training_labels,
```

## azureml/acft/image/components/finetune/common/mlflow/common_constants.py

```diff
@@ -1,14 +1,15 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Mlflow PythonModel wrapper helper constants."""
 
 from dataclasses import dataclass
+from mlflow.types import DataType
 
 
 @dataclass
 class AugmentationConfigKeys:
     """Keys in augmentation configs"""
 
     TRAINING_PHASE_KEY = "train"
@@ -19,16 +20,30 @@
 
 
 @dataclass
 class AlbumentationParameterNames:
     """ keys for Albumentations parameters"""
     TRANSFORMS_KEY = "transforms"
     BBOX_PARAMS = "bbox_params"
-    PASCAL_VOC = 'pascal_voc'
-    CLASS_LABELS = 'class_labels'
+    PASCAL_VOC = "pascal_voc"
+    CLASS_LABELS = "class_labels"
+    IMAGE = "image"
+    BBOX = "bbox"
+    MASK = "mask"
+    IMAGE_METADATA = "image_metadata"
+    ORIGINAL_WIDTH = "original_width"
+    ORIGINAL_HEIGHT = "original_height"
+    NEW_WIDTH = "new_width"
+    NEW_HEIGHT = "new_height"
+    NEW_LEFT = "new_left"
+    NEW_TOP = "new_top"
+    WIDTH_SCALE = "width_scale"
+    HEIGHT_SCALE = "height_scale"
+    RESIZED_WIDTH = "resized_width"
+    RESIZED_HEIGHT = "resized_height"
 
 
 @dataclass
 class AugmentationConfigFileExts:
     """Various Augmentation Config file types supported"""
 
     YAML = ".yaml"
@@ -37,40 +52,43 @@
 class Tasks:
     "Tasks supported for All Frameworks"
 
     HF_MULTI_CLASS_IMAGE_CLASSIFICATION = "image-classification"
     HF_MULTI_LABEL_IMAGE_CLASSIFICATION = "image-classification-multilabel"
     MM_OBJECT_DETECTION = "image-object-detection"
     MM_INSTANCE_SEGMENTATION = "image-instance-segmentation"
+    MM_MULTI_OBJECT_TRACKING = "video-multi-object-tracking"
 
 
 class HFMiscellaneousLiterals:
     """HF miscellaneous constants"""
 
     PIXEL_VALUES = "pixel_values"
     DEFAULT_IMAGE_KEY = "image"
     IMAGE_FOLDER = "imagefolder"
     VAL = "val"
     ID2LABEL = "id2label"
     LABEL2ID = "label2id"
 
 
-class HFMiscellaneousConstants:
-    """HF miscellaneous constants."""
+class HFConstants:
+    """HF constants"""
 
-    DEFAULT_THRESHOLD = 0.5
+    DEFAULT_DATALOADER_NUM_WORKERS = 6
 
 
 class MLFlowSchemaLiterals:
     """MLFlow model signature related schema"""
 
     INPUT_IMAGE_KEY = "image_base64"
-    INPUT_COLUMN_IMAGE_DATA_TYPE = "string"
+    INPUT_COLUMN_IMAGE_DATA_TYPE = DataType.binary
     INPUT_COLUMN_IMAGE = "image"
-    OUTPUT_COLUMN_DATA_TYPE = "string"
+    INPUT_COLUMN_VIDEO_DATA_TYPE = DataType.string
+    INPUT_COLUMN_VIDEO = "video"
+    OUTPUT_COLUMN_DATA_TYPE = DataType.string
     OUTPUT_COLUMN_FILENAME = "filename"
     OUTPUT_COLUMN_PROBS = "probs"
     OUTPUT_COLUMN_LABELS = "labels"
     OUTPUT_COLUMN_BOXES = "boxes"
 
     BATCH_SIZE_KEY = "batch_size"
     SCHEMA_SIGNATURE = "signature"
@@ -80,30 +98,60 @@
 
 
 class MMDetLiterals:
     """MMDetection constants"""
     CONFIG_PATH = "config_path"
     WEIGHTS_PATH = "weights_path"
     AUGMENTATIONS_PATH = "augmentations_path"
-    METAFILE_PATH = "model_metafile"
+    METAFILE_PATH = "model_metadata"
+    MODEL_DEFAULTS_PATH = "model_defaults_path"
+
+
+class MMdetModes:
+    """ MMDetection forward mode constants"""
+    LOSS = "loss"
+    PREDICT = "predict"
 
 
 class MmDetectionDatasetLiterals:
     """MMDetection dataset constants"""
 
     IMG = "img"
     IMG_METAS = "img_metas"
     GT_BBOXES = "gt_bboxes"
     GT_LABELS = "gt_labels"
     GT_CROWDS = "gt_crowds"
     GT_MASKS = "gt_masks"
     MASKS = "masks"
     BBOXES = "bboxes"
     LABELS = "labels"
+    IMAGE_SHAPE = "img_shape"
     IMAGE_ORIGINAL_SHAPE = "ori_shape"
+    PAD_SHAPE = "pad_shape"
+    RAW_DIMENSIONS = "raw_dimensions"
+    RAW_MASK_DIMENSIONS = "raw_mask_dimensions"
+    SCALE_FACTOR = "scale_factor"
+    DUMMY_LABELS = "dummy_labels"
+    BATCH_DATA_SAMPLES = "batch_data_samples"
+    ORIGINAL_GT_BBOXES = "original_gt_bboxes"
+    ORIGINAL_GT_MASKS = "original_gt_masks"
+
+
+class MmTrackingDatasetLiterals(MmDetectionDatasetLiterals):
+    """MMTracking dataset constants"""
+
+    DET_BBOXES = "det_bboxes"
+    DET_LABELS = "det_labels"
+    TRACK_BBOXES = "track_bboxes"
+    TRACK_LABELS = "track_labels"
+    INSTANCE_ID = "instance_id"
+
+    IMG_INFO = "img_info"
+    FRAME_ID = "frame_id"
+    VIDEO_URL = "video_url"
 
 
 class ODLiterals:
     """OD constants"""
 
     LABEL = "label"
     BOXES = "boxes"
@@ -117,7 +165,28 @@
 
 
 class MmDetectionConfigLiterals:
     """MMDetection config constants"""
 
     NUM_CLASSES = "num_classes"
     BOX_SCORE_THRESHOLD = "score_thr"
+    LANG_MODEL_NAME = "lang_model_name"
+
+
+class MetricsLiterals:
+    """ Azureml Metrics Literals"""
+
+    SCORES = "scores"
+    CLASSES = "classes"
+    METRICS_COMPUTER = "metrics_computer"
+    METRICS = "metrics"
+
+
+class TrainingDefaultsConstants:
+    """Training Defaults Constants"""
+
+    MODEL_DEFAULTS_FILE = "model_defaults.json"
+
+
+class DistributedConstants:
+    """Distributed Constants"""
+    LOCAL_RANK = "LOCAL_RANK"
```

## azureml/acft/image/components/finetune/common/mlflow/common_utils.py

```diff
@@ -1,22 +1,26 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Mlflow PythonModel wrapper helper scripts."""
 
 import logging
+import os
 import tempfile
 import pandas as pd
 import base64
 import io
 import re
 import requests
+import torch
 
-from PIL import Image
+from PIL import Image, UnidentifiedImageError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTSystemException
+from common_constants import DistributedConstants
 
 logger = logging.getLogger(__name__)
 
 # Uncomment the following line for mlflow debug mode
 # logging.getLogger("mlflow").setLevel(logging.DEBUG)
 
 
@@ -29,15 +33,19 @@
     :type parent_dir: str
     :return: Path to the file
     :rtype: str
     """
     with tempfile.NamedTemporaryFile(dir=parent_dir, mode="wb", delete=False) as image_file_fp:
         # image_file_fp.write(request_body)
         img_path = image_file_fp.name + ".png"
-        img = Image.open(io.BytesIO(request_body))
+        try:
+            img = Image.open(io.BytesIO(request_body))
+        except UnidentifiedImageError as e:
+            logger.error("Invalid image format. Please use base64 encoding for input images.")
+            raise e
         img.save(img_path)
         return img_path
 
 
 def process_image(img: pd.Series) -> pd.Series:
     """If input image is in base64 string format, decode it to bytes. If input image is in url format,
     download it and return bytes.
@@ -45,21 +53,45 @@
 
     :param img: pandas series with image in base64 string format or url.
     :type img: pd.Series
     :return: decoded image in pandas series format.
     :rtype: Pandas Series
     """
     image = img[0]
-    if _is_valid_url(image):
-        image = requests.get(image).content
-        return pd.Series(image)
-    try:
-        return pd.Series(base64.b64decode(image))
-    except Exception:
-        raise ValueError("Invalid image format")
+    if isinstance(image, bytes):
+        return img
+    elif isinstance(image, str):
+        if _is_valid_url(image):
+            image = requests.get(image).content
+            return pd.Series(image)
+        else:
+            try:
+                return pd.Series(base64.b64decode(image))
+            except ValueError:
+                raise ValueError("The provided image string cannot be decoded."
+                                 "Expected format is base64 string or url string.")
+    else:
+        raise ValueError(f"Image received in {type(image)} format which is not supported."
+                         "Expected format is bytes, base64 string or url string.")
+
+
+def process_video(vid: pd.Series) -> str:
+    """If input video is in url format, return the video url.
+       This function called for each row in the input data, i.e one video a time.
+
+    :param vid: pandas series with valid video url.
+    :type vid: pd.Series
+    :return: video link str.
+    :rtype: str
+    """
+    video = vid[0]
+    if isinstance(video, str):
+        if _is_valid_url(video):
+            return video
+    raise ValueError("Video received is not in valid format. Expected format is url string.")
 
 
 def _is_valid_url(text: str) -> bool:
     """check if text is url or base64 string
     :param text: text to validate
     :type text: str
     :return: True if url else false
@@ -81,7 +113,26 @@
 
     # Return if the string
     # matched the ReGex
     if re.search(p, text):
         return True
     else:
         return False
+
+
+def get_current_device() -> torch.device:
+    """Get current cuda device
+    :return: current device
+    :rtype: torch.device
+    """
+
+    # check if GPU is available
+    if torch.cuda.is_available():
+        if os.environ.get(DistributedConstants.LOCAL_RANK) is None:
+            msg = "LOCAL_RANK parameter is missing from environment variables."
+            logger.warning(f"{msg}")
+
+        # get the current device index
+        device_idx = int(os.environ.get(DistributedConstants.LOCAL_RANK, "0"))
+        return torch.device(type="cuda", index=device_idx)
+    else:
+        return torch.device(type="cpu")
```

## azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py

```diff
@@ -4,130 +4,180 @@
 
 """Custom albumentation augmentations."""
 
 import albumentations
 import torch
 import random
 import numpy as np
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Tuple, Union, Callable
 from albumentations.pytorch import transforms
 from albumentations import DualTransform
+from common_constants import AlbumentationParameterNames
 
 BoxInternalType = Tuple[float, float, float, float]
 
 
 class RandomExpand(DualTransform):
     """ Expand the image, bbox and mask by a random ratio and fill the surrounding space with the mean of ImageNet.
         This is intended to detect smaller objects.
     """
-    def apply(self, img: np.ndarray, **params) -> np.ndarray:
-        """ Overrides the DualTransform.apply method. This would apply the
-        transformation to the input image.
-        :param image: image
-        :type image: np.ndarray
-        :return: transformed image
-        :rtype: np.ndarray
-        """
 
-        return self._expand_image(img)
-
-    def apply_to_bbox(self, bbox: BoxInternalType, **params) -> BoxInternalType:
-        """ Overrides the DualTransform.apply_to_bbox method. This would apply
-        the transformations to each bounding box separately.
-        :param image: bbox
-        :type image: Tuple[float, float, float, float]
-        :return: transformed bounding box
-        :rtype: Tuple[float, float, float, float]
+    @property
+    def targets_as_params(self):
+        """ targets which are required for the transformation as parameters.
+        These targets are passed to get_params_dependent_on_targets method as params.
+        """
+        return [AlbumentationParameterNames.IMAGE]
+
+    def get_params_dependent_on_targets(self, params: Dict) -> Tuple:
+        """ Calcuate the parameters for the transformation which are dependent on the input image.
+        :params: Dict of input image
+        :type params: Dict
+        :return: Tuple of parameters
+        :rtype: Tuple
         """
+        img = params[AlbumentationParameterNames.IMAGE]
+        height, width, _ = img.shape
 
-        return self._expand_bbox(bbox)
-
-    def apply_to_masks(self, masks: List[np.ndarray], **params) -> List[np.ndarray]:
-        """ Overrides the DualTransform.apply_to_masks method. This would apply
-        the transformations to the masks.
-        :param masks: list of masks
-        :type image: List[np.ndarray]
-        :return: transformed masks
-        :rtype: List[np.ndarray]
-        """
-
-        return self._expand_masks(masks)
-
-    def get_transform_init_args_names(self) -> Tuple:
-        """ Returns a tuple of arguments which are expected in the init method of the
-        transformations.
-        """
-
-        return ()
-
-    def _expand_image(self, image: np.ndarray) -> np.ndarray:
-        """
+        ratio = random.uniform(1, 2)
+        new_height = int(height * ratio)
+        new_width = int(width * ratio)
+        top = random.randint(0, new_height - height)
+        left = random.randint(0, new_width - width)
+        return {
+            AlbumentationParameterNames.ORIGINAL_WIDTH: width,
+            AlbumentationParameterNames.ORIGINAL_HEIGHT: height,
+            AlbumentationParameterNames.NEW_WIDTH: new_width,
+            AlbumentationParameterNames.NEW_HEIGHT: new_height,
+            AlbumentationParameterNames.NEW_LEFT: left,
+            AlbumentationParameterNames.NEW_TOP: top
+        }
+
+    def apply(self,
+              img: np.ndarray,
+              original_width: int,
+              original_height: int,
+              new_width: int,
+              new_height: int,
+              new_left: int,
+              new_top: int,
+              **params) -> np.ndarray:
+        """ Overrides the DualTransform.apply method. This would apply the
+        transformation to the input image.
         :param image: image
         :type image: np.ndarray
-        :return: expanded image
+        :param original_width: Original width of the image
+        :type original_width: int
+        :param original_height: Original height of the image
+        :type original_height: int
+        :param new_width: New width after expanding the image
+        :type new_width: int
+        :param new_height: New height after expanding the image
+        :type new_height: int
+        :param new_left: New left of the image after expansion
+        :type new_left: int
+        :param new_top: New top of the image after expansion
+        :type new_top: int
+        :return: transformed image
         :rtype: np.ndarray
         """
-
         # Todo: Replace imagenet mean read from model's config file
         imagenet_mean = [0.485, 0.456, 0.406]
 
-        tensor_image = transforms.img_to_tensor(image)
-        depth, self.height, self.width = tensor_image.size()
-
-        ratio = random.uniform(1, 2)
-        self.new_height = int(self.height * ratio)
-        self.new_width = int(self.width * ratio)
-        self.top = random.randint(0, self.new_height - self.height)
-        self.left = random.randint(0, self.new_width - self.width)
+        tensor_image = transforms.img_to_tensor(img)
 
         # place an image in a larger mean image
-        new_image = torch.ones((3, self.new_height, self.new_width), dtype=torch.float)
+        new_image = torch.ones((3, new_height, new_width), dtype=torch.float)
         new_image[:, :, :] *= torch.FloatTensor(imagenet_mean).unsqueeze(1).unsqueeze(2)
-        new_image[:, self.top: self.top + self.height, self.left:self.left + self.width] = tensor_image
+        new_image[:, new_top: new_top + original_height, new_left:new_left + original_width] = tensor_image
         # convert image(C, H, W) to (H, W, C)
         return new_image.numpy().transpose(1, 2, 0)
 
-    def _expand_bbox(self, bbox: BoxInternalType) -> BoxInternalType:
-        """
-        expand the bounding box to the same dimension as the image
-        :param box: bounding box in (x_min, y_min, x_max, y_max)
-        :type boxe: Tuple[torch.Tensor]
-        :return: expanded bounding box
-        :rtype: Tuple[torch.Tensor]
+    def apply_to_bbox(self,
+                      bbox: BoxInternalType,
+                      original_width: int,
+                      original_height: int,
+                      new_width: int,
+                      new_height: int,
+                      new_left: int,
+                      new_top: int,
+                      **params) -> BoxInternalType:
+        """ Overrides the DualTransform.apply_to_bbox method. This would apply
+        the transformations to each bounding box separately.
+        :param image: bbox
+        :type image: Tuple[float, float, float, float]
+        :param original_width: Original width of the image
+        :type original_width: int
+        :param original_height: Original height of the image
+        :type original_height: int
+        :param new_width: New width after expanding the image
+        :type new_width: int
+        :param new_height: New height after expanding the image
+        :type new_height: int
+        :param new_left: New left of the image after expansion
+        :type new_left: int
+        :param new_top: New top of the image after expansion
+        :type new_top: int
+        :return: transformed bounding box
+        :rtype: Tuple[float, float, float, float]
         """
-
-        # Albumentation normalizes the input bboxes to keep the scale in range[0,1].
+        # Note: Albumentation normalizes the input bboxes to keep the scale in range[0,1].
         denormalized_bbox = (
-            bbox[0] * self.width, bbox[1] * self.height,
-            bbox[2] * self.width, bbox[3] * self.height
+            bbox[0] * original_width, bbox[1] * original_height,
+            bbox[2] * original_width, bbox[3] * original_height
         )
         new_bbox = torch.Tensor(denormalized_bbox)
-        new_bbox += torch.FloatTensor([self.left, self.top, self.left, self.top])
+        new_bbox += torch.FloatTensor([new_left, new_top, new_left, new_top])
         new_bbox = tuple(new_bbox)
         normalized_box = (
-            new_bbox[0] / self.new_width, new_bbox[1] / self.new_height,
-            new_bbox[2] / self.new_width, new_bbox[3] / self.new_height
+            new_bbox[0] / new_width, new_bbox[1] / new_height,
+            new_bbox[2] / new_width, new_bbox[3] / new_height
         )
         return normalized_box
 
-    def _expand_masks(self, masks: Optional[List[np.ndarray]]) -> Optional[List[np.ndarray]]:
-        """
-        :param masks: NxHxW pixel array masks for the object
-        :type masks: List[np.ndarray]
-        :return: expanded mask if present
-        :rtype: Optional[List[np.ndarray]]
+    def apply_to_masks(self, masks: List[np.ndarray],
+                       original_width: int,
+                       original_height: int,
+                       new_width: int,
+                       new_height: int,
+                       new_left: int,
+                       new_top: int,
+                       **params) -> List[np.ndarray]:
+        """ Overrides the DualTransform.apply_to_masks method. This would apply
+        the transformations to the masks.
+        :param masks: list of masks
+        :type image: List[np.ndarray]
+        :param original_width: Original width of the image
+        :type original_width: int
+        :param original_height: Original height of the image
+        :type original_height: int
+        :param new_width: New width after expanding the image
+        :type new_width: int
+        :param new_height: New height after expanding the image
+        :type new_height: int
+        :param new_left: New left of the image after expansion
+        :type new_left: int
+        :param new_top: New top of the image after expansion
+        :type new_top: int
+        :return: transformed masks
+        :rtype: List[np.ndarray]
         """
-
         # if there are masks, align them with the image
         new_masks = None
         if masks is not None:
-            new_masks = np.zeros((len(masks), self.new_height, self.new_width), dtype=np.float32)
-            new_masks[:, self.top:self.top + self.height, self.left:self.left + self.width] = masks
+            new_masks = np.zeros((len(masks), new_height, new_width), dtype=np.float32)
+            new_masks[:, new_top:new_top + original_height, new_left:new_left + original_width] = masks
         return new_masks
 
+    def get_transform_init_args_names(self) -> Tuple:
+        """ Returns a tuple of arguments which are expected in the init method of the
+        transformations.
+        """
+        return ()
+
 
 class ConstraintResize(DualTransform):
     """
     Given the scale<min_size, max_size>, the image will be rescaled as large as possible within the scale.
     The image size will be constraint so that the max edge is no longer than max_size and
     short edge is no longer than min_size.
     """
@@ -145,16 +195,14 @@
         :type p: float
         """
         super(ConstraintResize, self).__init__(always_apply, p)
         self.img_scale = img_scale
         self.min_size = min(img_scale)
         self.max_size = max(img_scale)
         self.keep_ratio = keep_ratio
-        self.new_h = None
-        self.new_w = None
 
     def _random_select(self):
         """Randomly select an img_scale from given candidates.
         Args:
             img_scales (list[tuple]): Images scales for selection.
         Returns:
             (tuple, int): Returns a tuple ``(img_scale, scale_dix)``, \
@@ -162,106 +210,189 @@
                 ``scale_idx`` is the selected index in the given candidates.
         """
 
         scale_idx = np.random.randint(len(self.img_scale))
         selected_img_scale = self.img_scale[scale_idx]
         return selected_img_scale, scale_idx
 
-    def _set_new_size(self, img: np.ndarray, keep_ratio=True) -> None:
+    def _get_new_size(self, img: np.ndarray) -> Tuple[int, int, int, int, float, float]:
         """
         Calcuate the final size of the output image
         :param img: Input image
         :type img: np.ndarray
-        :param keep_ratio: Whether to keep the aspect ratio.
-        :type keep_ratio: Boolean
+        :return a tuple of (current_height, current width,
+                            new_height, new_width,
+                            width_scale_factor, height_scale_factor)
         """
 
-        self.h, self.w = img.shape[:2]
-        if type(self.img_scale[0]) == list or type(self.img_scale[0]) == tuple:
+        h, w = img.shape[:2]
+        if isinstance(self.img_scale[0], list) or isinstance(self.img_scale[0], tuple):
             randomly_selected_scale, _ = self._random_select()
             self.min_size = min(randomly_selected_scale)
             self.max_size = max(randomly_selected_scale)
 
-        if keep_ratio:
+        if self.keep_ratio:
             img_min_size = min(img.shape[:2])
             img_max_size = max(img.shape[:2])
             # Todo: Add support for min_size and max_size as a list also
             scale_factor = min(self.min_size / img_min_size, self.max_size / img_max_size)
-            self.new_h = int(self.h * scale_factor)
-            self.new_w = int(self.w * scale_factor)
+            new_h = int(h * scale_factor)
+            new_w = int(w * scale_factor)
         else:
-            self.new_h = self.max_size if self.h > self.w else self.min_size
-            self.new_w = self.min_size if self.h > self.w else self.max_size
-        self.w_scale = self.new_w / self.w
-        self.h_scale = self.new_h / self.h
-
-    def apply(self, img: np.ndarray, **params) -> np.ndarray:
+            new_h = self.max_size if h > w else self.min_size
+            new_w = self.min_size if h > w else self.max_size
+        w_scale = new_w / w
+        h_scale = new_h / h
+        return w, h, new_w, new_h, w_scale, h_scale
+
+    @property
+    def targets_as_params(self):
+        """ targets which are required for the transformation as parameters.
+        Overrides the DualTransform.targets_as_params property.
+        These targets are passed to get_params_dependent_on_targets method as params.
+        """
+        return [AlbumentationParameterNames.IMAGE]
+
+    @property
+    def targets(self) -> Dict[str, Callable]:
+        """ targets for the augmentation such as image, mask, bbox, keypoints etc.
+        Overrides the DualTransform.targets property.
+        """
+        super_targets = super().targets
+        return {
+            **super_targets,
+            AlbumentationParameterNames.IMAGE_METADATA: self.apply_to_metadata
+        }
+
+    def get_params_dependent_on_targets(self, params: Dict) -> Tuple:
+        """ Calcuate the parameters for the transformation which are dependent on the input image.
+        Overrides the DualTransform.get_params_dependent_on_targets method. This would apply
+        :params: Dict of input image
+        :type params: Dict
+        :return: Tuple of parameters
+        :rtype: Tuple
+        """
+        img = params[AlbumentationParameterNames.IMAGE]
+        width, height, new_w, new_h, w_scale, h_scale = self._get_new_size(img)
+        return {
+            AlbumentationParameterNames.ORIGINAL_WIDTH: width,
+            AlbumentationParameterNames.ORIGINAL_HEIGHT: height,
+            AlbumentationParameterNames.NEW_WIDTH: new_w,
+            AlbumentationParameterNames.NEW_HEIGHT: new_h,
+            AlbumentationParameterNames.WIDTH_SCALE: w_scale,
+            AlbumentationParameterNames.HEIGHT_SCALE: h_scale
+        }
+
+    def apply(self,
+              img: np.ndarray,
+              new_width: int,
+              new_height: int,
+              **params) -> np.ndarray:
         """ Overrides the DualTransform.apply method. This would apply the
         transformation to the input image.
         :param image: image
         :type image: np.ndarray
+        :param new_w: New width after resizing the image
+        :param new_w: int
+        :param new_h: New height after resizing the image
+        :param new_h: int
         :return: transformed image
         :rtype: np.ndarray
         """
 
-        # Todo: This resizes all the images to a fixed size which is the size
-        # of the first image. Remove this and add resizing of all the images
-        # in current batch to the same size in collate method. This should
-        # resize the bboxes, masks as well.
-
-        if not self.new_h or not self.new_w:
-            self._set_new_size(img, self.keep_ratio)
-        new_image = albumentations.resize(img, self.new_h, self.new_w)
-        return new_image
+        return albumentations.resize(img, new_height, new_width)
 
-    def apply_to_bbox(self, bbox: BoxInternalType, **params) -> BoxInternalType:
+    def apply_to_metadata(self,
+                          metadata: Dict,
+                          new_width: int,
+                          new_height: int,
+                          **params) -> Dict:
+        """ Capture the resized image shape in the metadata
+        :param metadata: Image metadata
+        :type metadata: Dict
+        :param new_w: New width after resizing the image
+        :param new_w: int
+        :param new_h: New height after resizing the image
+        :param new_h: int
+        :return: transformed metadata
+        :rtype: Dict
+        """
+        resize_shape = {
+            AlbumentationParameterNames.RESIZED_WIDTH: new_width,
+            AlbumentationParameterNames.RESIZED_HEIGHT: new_height
+        }
+        return {**metadata, **resize_shape}
+
+    def apply_to_bbox(self, bbox: BoxInternalType,
+                      original_width: int,
+                      original_height: int,
+                      new_width: int,
+                      new_height: int,
+                      width_scale: float,
+                      height_scale: float,
+                      **params) -> BoxInternalType:
         """ Overrides the DualTransform.apply_to_bbox method. This would apply
         the transformations to each bounding box separately.
         :param image: bbox
         :type image: Tuple[float, float, float, float]
         :return: transformed bounding box
         :rtype: Tuple[float, float, float, float]
         """
 
         denormalized_bbox = (
-            bbox[0] * self.w, bbox[1] * self.h,
-            bbox[2] * self.w, bbox[3] * self.h
+            bbox[0] * original_width, bbox[1] * original_height,
+            bbox[2] * original_width, bbox[3] * original_height
         )
-        new_bbox = torch.Tensor(denormalized_bbox)
-        new_bbox *= torch.FloatTensor([self.w_scale, self.h_scale, self.w_scale, self.h_scale])
+        new_bbox = self.resize_bbox(denormalized_bbox, width_scale, height_scale)
         new_bbox = tuple(new_bbox)
         normalized_box = (
-            new_bbox[0] / self.new_w, new_bbox[1] / self.new_h,
-            new_bbox[2] / self.new_w, new_bbox[3] / self.new_h
+            new_bbox[0] / new_width, new_bbox[1] / new_height,
+            new_bbox[2] / new_width, new_bbox[3] / new_height
         )
         return normalized_box
 
-    def apply_to_masks(self, masks: List[np.ndarray], **params) -> List[np.ndarray]:
+    def resize_bbox(cls, bbox: BoxInternalType,
+                    w_scale: float, h_scale: float) -> Tuple[float, float, float, float]:
+        """ Resize the bounding box
+        :param bbox: bbox
+        :type bbox: Tuple[float, float, float, float]
+        :param w_scale: width scale factor
+        :type w_scale: float
+        :param h_scale: height scale factor
+        :type h_scale: float
+        :return: transformed bounding box
+        :rtype: Tuple[float, float, float, float]
+        """
+        scale_multiplier = np.array([w_scale, h_scale, w_scale, h_scale])
+        np_bbox = np.array(bbox)
+        return np_bbox * scale_multiplier
+
+    def apply_to_masks(self, masks: List[np.ndarray], new_width: int,
+                       new_height: int, **params) -> List[np.ndarray]:
         """ Overrides the DualTransform.apply_to_masks method. This would apply
         the transformations to the masks.
         :param masks: list of masks
         :type image: List[np.ndarray]
         :return: transformed masks
         :rtype: List[np.ndarray]
         """
 
         if masks is None:
             return masks
         rescaled_masks = []
         for mask in masks:
-            rescaled_masks.append(albumentations.resize(mask, self.new_h, self.new_w))
+            rescaled_masks.append(albumentations.resize(mask, new_height, new_width))
         return rescaled_masks
 
     def get_transform_init_args_names(self) -> Tuple:
         """ Returns a tuple of arguments which are expected in the init method of the
         transformations.
         """
 
         return (
             "img_scale",
             "keep_ratio"
         )
 
 
-# Todo: Move this file to inference folder for model export
 albumentations.RandomExpand = RandomExpand
 albumentations.ConstraintResize = ConstraintResize
```

## azureml/acft/image/components/finetune/common/mlflow/masktools.py

```diff
@@ -64,15 +64,16 @@
         # Convert to [x, y, x, y, ....] coordinates and correct for padding
         unwrapped_contour = [0] * (2 * len(contour))
         unwrapped_contour[::2] = numpy.ceil(contour[:, 1]) - edge_safety_padding
         unwrapped_contour[1::2] = numpy.ceil(contour[:, 0]) - edge_safety_padding
 
         simplified_contours.append(unwrapped_contour)
 
-    return _normalize_contour(simplified_contours, image_shape)
+    contours = _normalize_contour(simplified_contours, image_shape)
+    return _remove_invalid_contours(contours)
 
 
 def _normalize_contour(contours: List, image_shape: Tuple[int, int]) -> List:
     """Normalize the contour coordinates to be between 0 and 1.
 
     :param contours: List of contours
     :type: contours: list
@@ -86,7 +87,15 @@
     height, width = image_shape[0], image_shape[1]
 
     for contour in contours:
         contour[::2] = [x * 1.0 / width for x in contour[::2]]
         contour[1::2] = [y * 1.0 / height for y in contour[1::2]]
 
     return contours
+
+
+def _remove_invalid_contours(contours: List[List[float]]) -> List[List[float]]:
+    """Remove invalid contours. Contours is valid if it contains more than or equal to 6 co-ordinates (triangle).
+    :param contours: List of contours.
+    :return: List of contours.
+    """
+    return [contour for contour in contours if len(contour) >= 6]
```

## azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py

```diff
@@ -1,54 +1,78 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Mlflow save utils."""
 
+# Note: Make Sure not add any imports from image package as this is being
+# used in evaluate-mlflow pacakge for testing.
 import mlflow
 import os
-
+import torch
+import transformers
+from argparse import Namespace
+
+from mlflow.models import infer_signature
+from mlflow.transformers import generate_signature_output
+from transformers.image_processing_utils import BaseImageProcessor
+from transformers.modeling_utils import PreTrainedModel
 from typing import Dict, Optional, List, Any
 
 from azureml._common._error_definition.azureml_error import AzureMLError
 from azureml.acft.common_components import get_logger_app, ModelSelectorDefaults
 from azureml.acft.common_components.utils.error_handling.error_definitions import TaskNotSupported
 from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
+from azureml.acft.image.components.common.utils import get_random_base64_decoded_image
 from mlflow.models.signature import ModelSignature
 from mlflow.types.schema import ColSpec, Schema
 
+from mmdet_mlflow_model_wrapper import ImagesMLFlowModelWrapper as DetImagesMLFlowModelWrapper
+from mmtrack_mlflow_model_wrapper import ImagesMLFlowModelWrapper as TrackImagesMLFlowModelWrapper
+
 from common_constants import (
     AugmentationConfigKeys,
     Tasks,
     MLFlowSchemaLiterals,
-    MMDetLiterals
+    MMDetLiterals,
+    TrainingDefaultsConstants
 )
-from mmdet_mlflow_model_wrapper import ImagesMLFlowModelWrapper
+from mlflow.utils.requirements_utils import _get_pinned_requirement
+
 
 logger = get_logger_app(__name__)
 
 
 def get_mlflow_signature(task_type: str) -> ModelSignature:
     """
     Return mlflow model signature with input and output schema given the input task type.
 
     :param task_type: Task type used in training.
     :type task_type: str
     :return: mlflow model signature.
     :rtype: mlflow.models.signature.ModelSignature
     """
-
-    input_schema = Schema(
-        [
-            ColSpec(
-                MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE_DATA_TYPE,
-                MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE,
-            )
-        ]
-    )
+    if task_type == Tasks.MM_MULTI_OBJECT_TRACKING:
+        input_schema = Schema(
+            [
+                ColSpec(
+                    MLFlowSchemaLiterals.INPUT_COLUMN_VIDEO_DATA_TYPE,
+                    MLFlowSchemaLiterals.INPUT_COLUMN_VIDEO,
+                )
+            ]
+        )
+    else:
+        input_schema = Schema(
+            [
+                ColSpec(
+                    MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE_DATA_TYPE,
+                    MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE,
+                )
+            ]
+        )
 
     # For classification
     if task_type in [
         Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
         Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION,
     ]:
 
@@ -61,18 +85,19 @@
                 ColSpec(
                     MLFlowSchemaLiterals.OUTPUT_COLUMN_DATA_TYPE,
                     MLFlowSchemaLiterals.OUTPUT_COLUMN_LABELS,
                 ),
             ]
         )
 
-    # for object detection and instance segmentation mlflow signature remains same
+    # for object detection and instance segmentation and multi-object tracking mlflow signature remains same
     elif task_type in [
         Tasks.MM_OBJECT_DETECTION,
-        Tasks.MM_INSTANCE_SEGMENTATION
+        Tasks.MM_INSTANCE_SEGMENTATION,
+        Tasks.MM_MULTI_OBJECT_TRACKING,
     ]:
         output_schema = Schema(
             [
                 ColSpec(
                     MLFlowSchemaLiterals.OUTPUT_COLUMN_DATA_TYPE,
                     MLFlowSchemaLiterals.OUTPUT_COLUMN_BOXES,
                 ),
@@ -82,106 +107,207 @@
         raise ACFTValidationException._with_error(
             AzureMLError.create(TaskNotSupported, TaskName=task_type)
         )
 
     return ModelSignature(inputs=input_schema, outputs=output_schema)
 
 
+def get_extra_pip_requirements(task_name: str) -> List[str]:
+    """ Return extra pip packages required to loading the model in mlflow.
+    :param task_name: Task name used in training.
+    :type task_name: str
+    :return: extra pip packages.
+    :rtype: List[str]
+    """
+    extra_packages_list = []
+    extra_package_names = []
+    if task_name in [Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
+                     Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION]:
+        extra_package_names = [("torchvision", ">=0.0.14")]
+    for (package_name, default_version) in extra_package_names:
+        try:
+            # Take the pinned version from the current environment if available
+            # else use the default version provided.
+            package_with_version = _get_pinned_requirement(package_name)
+            extra_packages_list.append(package_with_version)
+        except ModuleNotFoundError:
+            msg = f"Failed to get requirement for {package_name} in the current environment. \
+                Pinning the default version {default_version} for {package_name}."
+            logger.info(msg)
+            extra_packages_list.append(f"{package_name}{default_version}")
+
+    return extra_packages_list
+
+
 def _save_mmdet_mlflow_model(
     model_output_dir: str,
     mlflow_output_dir: str,
     options: Dict[str, Any],
     model_name: str,
-    task_type: str
+    task_type: str,
+    metadata: dict
 ) -> None:
     """
     Save the mmdetection model in mlflow format.
 
     :param model_output_dir: Output directory where the HF trainer model files are stored.
     :type model_output_dir: str
     :param mlflow_output_dir: Output directory where mlflow model will be stored.
     :type mlflow_output_dir: str
     :param options: Dictionary of MLflow settings/wrappers for model saving process.
     :type options: Dict
     :param model_name: Name of the model.
     :type model_name: str
     :param task_type: Task type used in training.
     :type task_type: str
+    :param metadata: metadata to be added to MLmodel file
+    :type metadata: dict
     :return: None
     """
 
     config_path = os.path.join(model_output_dir, model_name + ".py")
     model_weights_path = os.path.join(model_output_dir, ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME)
     augmentations_path = os.path.join(model_output_dir, AugmentationConfigKeys.OUTPUT_AUG_FILENAME)
     metafile_path = os.path.join(model_output_dir, MMDetLiterals.METAFILE_PATH + ".json")
+    model_defaults_path = os.path.join(model_output_dir, TrainingDefaultsConstants.MODEL_DEFAULTS_FILE)
     artifacts_dict = {
         MMDetLiterals.CONFIG_PATH : config_path,
         MMDetLiterals.WEIGHTS_PATH : model_weights_path,
         MMDetLiterals.AUGMENTATIONS_PATH: augmentations_path,
         MMDetLiterals.METAFILE_PATH: metafile_path,
     }
+    if os.path.isfile(model_defaults_path):
+        artifacts_dict[MMDetLiterals.MODEL_DEFAULTS_PATH] = model_defaults_path
 
-    files_to_include = ['common_constants.py', 'common_utils.py', 'mmdet_mlflow_model_wrapper.py',
-                        'mmdet_modules.py', 'mmdet_utils.py', 'augmentation_helper.py',
-                        'custom_augmentations.py']
+    files_to_include_mmd = ['common_constants.py', 'common_utils.py', 'mmdet_mlflow_model_wrapper.py',
+                            'mmdet_modules.py', 'mmdet_utils.py', 'augmentation_helper.py',
+                            'custom_augmentations.py']
+    files_to_include_mmt = ['common_constants.py', 'common_utils.py', 'mmtrack_mlflow_model_wrapper.py',
+                            'mmtrack_module.py', 'mmtrack_utils.py']
+    if task_type == Tasks.MM_OBJECT_DETECTION:
+        files_to_include = files_to_include_mmd
     if task_type == Tasks.MM_INSTANCE_SEGMENTATION:
-        files_to_include.append('masktools.py')
+        files_to_include_mmd.append('masktools.py')
+        files_to_include = files_to_include_mmd
+    if task_type == Tasks.MM_MULTI_OBJECT_TRACKING:
+        files_to_include = files_to_include_mmt
     directory = os.path.dirname(__file__)
     code_path = [os.path.join(directory, x) for x in files_to_include]
 
+    logger.info(f"Saving mlflow pyfunc model to {mlflow_output_dir}.")
+
     pip_requirements = None
+    conda_env = None
     if task_type == Tasks.MM_OBJECT_DETECTION:
         pip_requirements = os.path.join(os.path.dirname(__file__), "mmdet-od-requirements.txt")
     elif task_type == Tasks.MM_INSTANCE_SEGMENTATION:
         pip_requirements = os.path.join(os.path.dirname(__file__), "mmdet-is-requirements.txt")
-
-    logger.info(f"Saving mlflow pyfunc model to {mlflow_output_dir}.")
+    elif task_type == Tasks.MM_MULTI_OBJECT_TRACKING:
+        conda_env = os.path.join(os.path.dirname(__file__), "mmtrack-mot-conda.yaml")
 
     try:
         mlflow.pyfunc.save_model(
             path=mlflow_output_dir,
             python_model=options[MLFlowSchemaLiterals.WRAPPER],
             artifacts=artifacts_dict,
             pip_requirements=pip_requirements,
+            conda_env=conda_env,
             signature=options[MLFlowSchemaLiterals.SCHEMA_SIGNATURE],
-            code_path=code_path
+            code_path=code_path,
+            metadata=metadata
         )
         logger.info("Saved mlflow model successfully.")
     except Exception as e:
         logger.error(f"Failed to save the mlflow model {str(e)}")
         raise Exception(f"failed to save the mlflow model {str(e)}")
 
 
 def save_mmdet_mlflow_pyfunc_model(
     task_type: str,
     model_output_dir: str,
     mlflow_output_dir: str,
     model_name: str,
+    metadata: dict,
 ) -> None:
     """
     Save the mlflow model.
 
     :param task_type: Task type used in training.
     :type task_type: str
     :param model_output_dir: Output directory where the HF trainer model files are stored.
     :type model_output_dir: str
     :param mlflow_output_dir: Output directory where mlflow model will be stored.
     :type mlflow_output_dir: str
     :param model_name: Name of the model.
     :type model_name: str
+    :param metadata: metadata to be added to MLmodel file
+    :type metadata: dict
     """
 
     logger.info("Saving the model in MLFlow format.")
-    mlflow_model_wrapper = ImagesMLFlowModelWrapper(task_type=task_type)
+    if task_type == Tasks.MM_MULTI_OBJECT_TRACKING:
+        mlflow_model_wrapper = TrackImagesMLFlowModelWrapper(task_type=task_type)
+    else:
+        mlflow_model_wrapper = DetImagesMLFlowModelWrapper(task_type=task_type)
 
     # Upload files to artifact store
     mlflow_options = {
         MLFlowSchemaLiterals.WRAPPER: mlflow_model_wrapper,
         MLFlowSchemaLiterals.SCHEMA_SIGNATURE: get_mlflow_signature(task_type),
     }
     _save_mmdet_mlflow_model(
         model_output_dir=model_output_dir,
         mlflow_output_dir=mlflow_output_dir,
         options=mlflow_options or {},
         model_name=model_name,
-        task_type=task_type
+        task_type=task_type,
+        metadata=metadata
+    )
+
+
+def hf_save_as_mlflow_model(component_args: Namespace,
+                            model: PreTrainedModel,
+                            image_processor: BaseImageProcessor,
+                            metadata: dict):
+    """
+    save hugging face mlflow
+
+    :param component_args: args from the finetune component
+    :type component_args: Namespace
+    :param model: transformers model object
+    :type model: PreTrainedModel
+    :param image_processor: transformers image processor object
+    :type image_processor: BaseImageProcessor
+    :param metadata: metadata to be added to MLmodel file
+    :type metadata: dict
+    """
+    output_model_metafile_path = os.path.join(component_args.output_dir,
+                                              ModelSelectorDefaults.MODEL_METADATA_PATH)
+    output_model_defaults_path = os.path.join(component_args.output_dir,
+                                              ModelSelectorDefaults.MODEL_DEFAULTS_PATH)
+    code_paths = []
+    if os.path.isfile(output_model_defaults_path):
+        code_paths.append(output_model_defaults_path)
+    if os.path.isfile(output_model_metafile_path):
+        code_paths.append(output_model_metafile_path)
+    transformers_model = {"model": model, "image_processor": image_processor}
+    # float16 models won't work when model is on cpu. hence converting
+    # the model to float32 for generating the signature.
+    vision_model = transformers.pipeline(
+        task="image-classification",
+        model=model.to(torch.float32),
+        image_processor=image_processor,
+    )
+
+    img_str = get_random_base64_decoded_image()
+    signature = infer_signature(
+        img_str, generate_signature_output(vision_model, img_str),
+    )
+    mlflow.transformers.save_model(
+        transformers_model=transformers_model,
+        path=component_args.mlflow_model_folder,
+        code_paths=code_paths,
+        signature=signature,
+        metadata=metadata,
+        task=Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
+        conda_env=mlflow.transformers.get_default_conda_env(model)
     )
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt

```diff
@@ -1,10 +1,12 @@
-mlflow
-cloudpickle==2.2.0
-datasets==2.3.2
-openmim
-torch==1.11.0
-torchvision
-transformers==4.25.1
+mlflow==2.9.2
+cloudpickle==2.2.1
+datasets==2.15.0
+openmim==0.3.9
+torch==2.0.1
+torchvision==0.15.2
+transformers==4.38.2
+accelerate==0.27.2
 albumentations==1.3.0
 scikit-image==0.19.3
-simplification==0.5.7
+simplification==0.7.10
+fairscale==0.4.13
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt

```diff
@@ -1,8 +1,10 @@
-mlflow
-cloudpickle==2.2.0
-datasets==2.3.2
-openmim
-torch==1.11.0
-torchvision
-transformers==4.25.1
-albumentations==1.3.0
+mlflow==2.9.2
+cloudpickle==2.2.1
+datasets==2.15.0
+openmim==0.3.9
+torch==2.0.1
+torchvision==0.15.2
+transformers==4.38.2
+accelerate==0.27.2
+albumentations==1.3.0
+fairscale==0.4.13
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py

```diff
@@ -4,39 +4,56 @@
 
 """Mlflow PythonModel wrapper class that loads the Mlflow model, preprocess inputs and performs inference."""
 
 import logging
 import subprocess
 import sys
 import tempfile
+import math
+import albumentations
 
 import mlflow
 import pandas as pd
 import torch
 from transformers import TrainingArguments
 
 from augmentation_helper import (
     load_augmentation_dict_from_config,
     get_transform
 )
 from common_constants import (AugmentationConfigKeys,
-                              HFMiscellaneousLiterals, Tasks,
+                              HFMiscellaneousLiterals,
+                              HFConstants, Tasks,
                               MMDetLiterals,
                               MLFlowSchemaLiterals)
-from common_utils import process_image, create_temp_file
+from common_utils import process_image, create_temp_file, get_current_device
 
 logger = logging.getLogger(__name__)
 
 
-def get_device() -> str:
-    """Returns the currently existing device type.
-    Returns:
-        str: cuda | cpu.
+def get_max_image_size(transforms_list: albumentations.Compose) -> int:
+    """ For MMD model, read the transforms list and return the max image size that the image
+        could be resized to by the ConstraintResize transformation.
+        This is calculated from the img_scale attribute of the ConstraintResize
+        and the pad_factor attribute of the PadIfNeeded transforms.
+
+        :param transforms_list: list of transforms
+        :type transforms_list: list
+        :return: max image size
+        :rtype: int
     """
-    return "cuda" if torch.cuda.is_available() else "cpu"
+    max_size, max_pad_divisor = 0, 1
+    for transform in transforms_list.transforms:
+        if transform.__class__.__name__ == "ConstraintResize":
+            max_size = max(transform.img_scale)
+        elif transform.__class__.__name__ == "PadIfNeeded":
+            max_pad_divisor = max(transform.pad_width_divisor, transform.pad_height_divisor)
+
+    max_img_size = math.ceil(max_size / max_pad_divisor) * max_pad_divisor
+    return max_img_size
 
 
 class ImagesMLFlowModelWrapper(mlflow.pyfunc.PythonModel):
     """MLFlow model wrapper for AutoML for Images models."""
 
     def __init__(
         self,
@@ -61,55 +78,48 @@
         :param context: Mlflow context containing artifacts that the model can use for inference.
         :type context: mlflow.pyfunc.PythonModelContext
         """
         logger.info("Inside load_context()")
 
         if self._task_type in [Tasks.MM_OBJECT_DETECTION, Tasks.MM_INSTANCE_SEGMENTATION]:
             # Install mmcv and mmdet using mim, with pip installation is not working
-            subprocess.check_call([sys.executable, "-m", "mim", "install", "mmcv-full==1.7.1"])
-            subprocess.check_call([sys.executable, "-m", "mim", "install", "mmdet==2.28.2"])
+            subprocess.check_call([sys.executable, "-m", "mim", "install", "mmdet==3.3.0"])
 
             # importing mmdet/mmcv after installing using mim
-            from mmdet.models import build_detector
-            from mmcv import Config
-            from mmcv.runner import load_checkpoint
+            from mmengine.config import Config
+            from mmengine.runner import load_checkpoint
+            from mmdet.apis import init_detector
             from mmdet_modules import ObjectDetectionModelWrapper, InstanceSegmentationModelWrapper
             from mmdet_utils import mmdet_run_inference_batch
             self.mmdet_run_inference_batch = mmdet_run_inference_batch
 
             try:
+                current_device = get_current_device()
                 model_config_path = context.artifacts[MMDetLiterals.CONFIG_PATH]
                 model_weights_path = context.artifacts[MMDetLiterals.WEIGHTS_PATH]
                 self._config = Config.fromfile(model_config_path)
-                self._model = build_detector(self._config.model)
+                self._model = init_detector(self._config, device=current_device)
                 if self._task_type == Tasks.MM_INSTANCE_SEGMENTATION:
                     self._model = InstanceSegmentationModelWrapper(self._model, self._config, model_weights_path)
                 elif self._task_type == Tasks.MM_OBJECT_DETECTION:
                     self._model = ObjectDetectionModelWrapper(self._model, self._config, model_weights_path)
-                load_checkpoint(self._model, model_weights_path, map_location=get_device())
+                load_checkpoint(self._model, model_weights_path, map_location=current_device)
                 logger.info("Model loaded successfully")
             except Exception:
                 logger.warning("Failed to load the the model.")
                 raise
 
             aug_config_path = context.artifacts[MMDetLiterals.AUGMENTATIONS_PATH]
             aug_config_dict = load_augmentation_dict_from_config(aug_config_path)
             self.test_transforms = get_transform(AugmentationConfigKeys.VALIDATION_PHASE_KEY,
                                                  aug_config_dict,
                                                  # Bbox is not required at test time
                                                  is_bbox_required=False)
-            # arguments for Trainer
-            self.test_args = TrainingArguments(
-                output_dir=".",
-                do_train=False,
-                do_predict=True,
-                per_device_eval_batch_size=1,
-                dataloader_drop_last=False,
-                remove_unused_columns=False
-            )
+            max_image_size = get_max_image_size(self.test_transforms)
+            self._model.max_image_size = max_image_size
         else:
             raise ValueError(f"invalid task type {self._task_type}."
                              f"Supported tasks: {Tasks.MM_OBJECT_DETECTION, Tasks.MM_INSTANCE_SEGMENTATION}")
 
     def predict(
         self, context: mlflow.pyfunc.PythonModelContext, input_data: pd.DataFrame
     ) -> pd.DataFrame:
@@ -122,29 +132,46 @@
         image is in base64 String format.
         :return: Output of inferencing
         :rtype: Pandas DataFrame with columns ["probs", "labels"] for classification and
         ["boxes"] for object detection, instance segmentation
         """
         task = self._task_type
 
+        ngpus = torch.cuda.device_count()
+        batch_size = len(input_data)
+        if ngpus > 1:
+            batch_size = int(math.ceil(batch_size // ngpus))
+
+        logger.info(f"evaluating with batch_size: {batch_size} and n_gpus: {ngpus}")
+        # arguments for Trainer
+        test_args = TrainingArguments(
+            output_dir=".",
+            do_train=False,
+            do_predict=True,
+            per_device_eval_batch_size=batch_size,
+            dataloader_num_workers=HFConstants.DEFAULT_DATALOADER_NUM_WORKERS,
+            dataloader_drop_last=False,
+            remove_unused_columns=False
+        )
+
         # process the images in image column
         processed_images = input_data.loc[:, [MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE]]\
             .apply(axis=1, func=process_image)
 
         # To Do: change image height and width based on kwargs.
 
         with tempfile.TemporaryDirectory() as tmp_output_dir:
             image_path_list = (
                 processed_images.iloc[:, 0]
                 .map(lambda row: create_temp_file(row, tmp_output_dir))
                 .tolist()
             )
 
             result = self.mmdet_run_inference_batch(
-                self.test_args,
+                test_args,
                 model=self._model,
                 id2label=self._config[HFMiscellaneousLiterals.ID2LABEL],
                 image_path_list=image_path_list,
                 task_type=task,
                 test_transforms=self.test_transforms,
             )
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py

```diff
@@ -1,44 +1,61 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """MMDetection modules."""
 
+import logging
 import torch
 import numpy as np
 
 from dataclasses import dataclass
-from mmcv import Config, concat_list
+from mmengine.config import Config
+from mmengine.utils import concat_list
+from mmengine.structures import InstanceData
+try:
+    # mmdet = 3.x
+    from mmdet.structures import DetDataSample
+except ImportError:
+    # mmdet = 2.x
+    DetDataSample = None
 from pathlib import Path
 from torch import nn, Tensor
 from torch.nn.utils.rnn import pad_sequence
 from typing import Dict, List, Union, Any, Tuple
+from common_constants import MmDetectionDatasetLiterals, MMdetModes, MmDetectionConfigLiterals
+from common_utils import get_current_device
 
-from common_constants import MmDetectionDatasetLiterals
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ImageMetadata:
     """Dataclass for maintaining the metadata dictionary as required for MM detection models.
     The keys of metadata dictionary is same as the property name."""
 
-    ori_shape: Tuple[int, int, int]
-    img_shape: Tuple[int, int, int] = None
-    pad_shape: Tuple[int, int, int] = None
-    scale_factor: np.ndarray = np.array([1, 1, 1, 1])
+    ori_shape: Tuple[int, int, int]         # Dimension of the transformed image H x W x C. This is the shape of the
+    # image after resizing and padding. If we set it to the original image shape i.e. shape before transformation
+    # then the MMD model is not able to learn and the eval_mAP is always 0.0.
+    img_shape: Tuple[int, int, int] = None  # Dimension of the image after ConstraintResize transformation.
+    pad_shape: Tuple[int, int, int] = None  # Dimension of the tranformed image after padding. Please note that padding
+    # is applied after ConstraintResize transformation, so pad_shape is always greater than or equal to img_shape.
+    raw_dimensions: Tuple[int, int] = None   # Dimension of the raw image H x W. This is used to resize the predicted
+    # mask to the original image size.
+    scale_factor: np.ndarray = np.array([1, 1])
     flip: bool = False
     flip_direction: str = None
     filename: str = None
     ori_filename: str = None
+    border: Tuple[int, int, int, int] = (0, 0, 0, 0)
 
     def __post_init__(self):
         """If image shape after resizing and padding is not provided then assign it with original shape"""
-        self.img_shape = self.ori_shape or self.img_shape
-        self.pad_shape = self.ori_shape or self.pad_shape
+        self.img_shape = self.img_shape or self.ori_shape
+        self.pad_shape = self.pad_shape or self.ori_shape
 
 
 class ObjectDetectionModelWrapper(nn.Module):
     """Wrapper class over object detection model of MMDetection."""
     def __init__(
         self,
         mm_object_detection_model: nn.Module,
@@ -55,89 +72,126 @@
         :type model_name_or_path: str
         """
 
         super().__init__()
         self.model = mm_object_detection_model
         self.config = config
         self.model_name = Path(model_name_or_path).stem
-
-    @classmethod
-    def _get_bboxes_and_labels(
-            cls, predicted_bbox: List[np.ndarray], img_meta: Dict
-    ) -> Tuple[Tensor, Tensor]:
-        """
-        Map the MM detection model"s predicted label to the bbox and labels
-        :param predicted_bbox: bbox of shape [Number of labels, Number of boxes, 5 [tl_x, tl_y, br_x, br_y,
-        box_score]] format.
-        :type predicted_bbox: List[np.ndarray]
-        :param img_meta: Image metadata
-        :type img_meta: Dict
-        :return: bounding boxes of shape [Number of boxes, 5 [tl_x, tl_y, br_x, br_y, box_score]] and labels of
-        shape [Number of boxes, label id]
-        :rtype: Tuple[Tensor, Tensor]
-        """
-        bboxes = torch.as_tensor(np.vstack(predicted_bbox))
-        height, width, _ = img_meta[MmDetectionDatasetLiterals.IMAGE_ORIGINAL_SHAPE]
-        for bbox in bboxes:
-            # Normalize bounding box
-            bbox[0] = bbox[0] / width
-            bbox[1] = bbox[1] / height
-            bbox[2] = bbox[2] / width
-            bbox[3] = bbox[3] / height
-
-        labels = [
-            np.full(bbox.shape[0], i, dtype=np.int32)
-            for i, bbox in enumerate(predicted_bbox)
-        ]
-        labels = torch.as_tensor(np.concatenate(labels))
-        return bboxes, labels
+        self.lang_model = hasattr(self.config, MmDetectionConfigLiterals.LANG_MODEL_NAME)
+        self.text = None
+        if self.lang_model:
+            try:
+                classes = self.config.test_dataloader.dataset.metainfo.CLASSES
+                self.text = ". ".join(classes)
+            except Exception as e:
+                logger.error("Unable to fetch classes information from config file")
+                raise e
 
     @classmethod
     def _pad_sequence(cls, sequences: Tensor, padding_value: float = -1, batch_first: bool = True) -> Tensor:
         """
         It stacks a list of Tensors sequences, and pads them to equal length.
         :param sequences: list of variable length sequences.
         :type sequences: Tensor
         :param padding_value: value for padded elements
         :type padding_value: float
         :param batch_first: output will be in B x T x * if True, or in T x B x * otherwise
         :type batch_first: bool
         :return: Tensor of size ``B x T x *`` if batch_first is True
         :rtype: Tensor
         """
-        return pad_sequence(sequences, padding_value=padding_value, batch_first=batch_first)
+        rt_tensor = pad_sequence(sequences, padding_value=padding_value, batch_first=batch_first)
+        rt_tensor = rt_tensor.to(device=get_current_device())
+        return rt_tensor
+
+    def _get_bboxes_and_labels(self, predictions):
+        """
+        Get bounding boxes and labels from the predictions.
+        :param predictions: predictions from the model
+        :type predictions: mmdet.structures.DetDataSample
+        :return: bounding boxes and labels
+        :rtype: Tensor, Tensor
+        """
+        predictions = predictions.detach()
+        pred = predictions.pred_instances
+        height, width = predictions.img_shape
+
+        scores = pred.scores.unsqueeze(dim=1)
+        img_box = torch.tensor([width, height, width, height], device=scores.device)
+        bboxes = pred.bboxes / img_box
+        bboxes = torch.concat((bboxes, scores), dim=1)
+
+        return bboxes, pred.labels
 
-    @classmethod
     def _organize_predictions_for_trainer(
-        cls, batch_predictions: List[List[np.ndarray]], img_metas: List[Dict]
+        self, batch_predictions: List[DetDataSample]
     ) -> Dict[str, Tensor]:
         """
         Transform the batch of predicted labels as required by the HF trainer.
         :param batch_predictions: batch of predicted labels
         :type batch_predictions: List of bbox list for each image
-        :param img_metas: batch of predicted labels
-        :type img_metas: List of image metadata dictionary
         :return: Dict of predicted labels in tensor format
         :rtype: Dict[str, Tensor]
 
         Note: Same reasoning like _organize_ground_truth_for_trainer function but for predicted label
         """
         batch_bboxes, batch_labels = [], []
-        for prediction, img_meta in zip(batch_predictions, img_metas):
-            bboxes, labels = ObjectDetectionModelWrapper._get_bboxes_and_labels(
-                prediction, img_meta
-            )
+        for predictions in batch_predictions:
+            bboxes, labels = self._get_bboxes_and_labels(predictions)
             batch_bboxes.append(bboxes)
             batch_labels.append(labels)
 
         output = dict()
         output[MmDetectionDatasetLiterals.BBOXES] = ObjectDetectionModelWrapper._pad_sequence(batch_bboxes)
         output[MmDetectionDatasetLiterals.LABELS] = ObjectDetectionModelWrapper._pad_sequence(batch_labels)
         return output
 
+    @classmethod
+    def prepare_inputs_for_model_forward(cls, data, is_train=False, text=None):
+        """ Prepare inputs as required for mmdetection.
+
+        :param data: list of dictionaries from od collate func
+        :type data: list of Dict
+        :param is_train: whether the data is for training or not
+        :type is_train: bool
+        :param text: str representing all the classes of the data joined by ". ".
+        :type text: str
+        :return: image tensor and list of datasamples
+        :rtype: Tensor, List[mmdet.structures.DetDataSample]
+        """
+
+        inputs = data.get(MmDetectionDatasetLiterals.IMG)
+        batch_data_samples = []
+        for i in range(len(inputs)):
+            img_metainfo = data[MmDetectionDatasetLiterals.IMG_METAS][i]
+            img_metainfo[MmDetectionDatasetLiterals.IMAGE_SHAPE] = \
+                img_metainfo[MmDetectionDatasetLiterals.IMAGE_SHAPE][:2]
+            img_metainfo.update({"batch_input_shape": inputs.shape[2:]})
+            if DetDataSample is None:
+                raise SystemError("DetDataSample is set to be None. "
+                                  "For detection tasks, please check installation of mmdet 3.x installation. "
+                                  "This function should not be called n video-multi-object-tracking tasks.")
+            data_sample = DetDataSample(metainfo=img_metainfo)
+
+            if is_train:
+                gt_instances = InstanceData(metainfo=img_metainfo)
+                if MmDetectionDatasetLiterals.GT_BBOXES in data:
+                    gt_instances.bboxes = data[MmDetectionDatasetLiterals.GT_BBOXES][i]
+                    gt_instances.labels = data[MmDetectionDatasetLiterals.GT_LABELS][i]
+                # gt_masks would be present for instance segmentation.
+                if MmDetectionDatasetLiterals.GT_MASKS in data:
+                    gt_instances.masks = data[MmDetectionDatasetLiterals.GT_MASKS][i]
+                data_sample.gt_instances = gt_instances
+            if text:
+                data_sample.text = text
+                data_sample.custom_entities = True
+            batch_data_samples.append(data_sample)
+
+        return inputs, batch_data_samples
+
     def forward(
         self, **data
     ) -> Union[Dict[str, Any], Tuple[Tensor, Dict[str, Tensor]]]:
         """
         Model forward pass for training and validation mode
         :param data: Input data to model
         :type data: Dict
@@ -152,24 +206,22 @@
              of these keys see `mmdet/datasets/pipelines/formatting.py:Collect`.
             gt_bboxes - Ground truth bboxes for each image with shape (num_gts, 4) in [tl_x, tl_y, br_x, br_y] format.
             gt_labels - List of class indices corresponding to each box
             gt_crowds - List of "is crowds" (boolean) to each box
             gt_masks - List of masks (type BitmapMasks) for each image if task is instance_segmentation
         """
         # test mode
-        img = data[MmDetectionDatasetLiterals.IMG]
-        img_metas = data[MmDetectionDatasetLiterals.IMG_METAS]
-        batch_predictions = self.model(
-            img=[img], img_metas=[img_metas], return_loss=False
-        )
+        inputs, batch_data_samples = ObjectDetectionModelWrapper.prepare_inputs_for_model_forward(data, text=self.text)
+        batch_predictions = self.model(inputs, batch_data_samples, mode=MMdetModes.PREDICT)
+
         output: dict = self._organize_predictions_for_trainer(
-            batch_predictions, img_metas
+            batch_predictions
         )
 
-        return torch.asarray([]), output
+        return torch.asarray([], device=get_current_device()), output
 
 
 class InstanceSegmentationModelWrapper(ObjectDetectionModelWrapper):
     """Wrapper class over mm instance segmentation model of MMDetection framework."""
     def __init__(
         self,
         mm_instance_segmentation_model: nn.Module,
@@ -181,70 +233,53 @@
         :param mm_instance_segmentation_model: MM instance segmentation model
         :type mm_instance_segmentation_model: nn.Module
         :param config: MM Instance segmentation model configuration
         :type config: MMCV Config
         :param model_name_or_path: model name or path
         :type model_name_or_path: str
         """
+        self.max_image_size = 0
         super(InstanceSegmentationModelWrapper, self).__init__(
             mm_instance_segmentation_model, config, model_name_or_path
         )
 
-    @classmethod
-    def _get_segmentation_masks(cls, mask_result: List[np.ndarray]) -> Tensor:
-        """
-        Map the model's predicted segmentation masks to the format required by the HF trainer
-        :param mask_result:
-        :type mask_result: List of masks
-        :return: mask in tensor format
-        :rtype: Tensor
-        """
-        mask = concat_list(
-            mask_result
-        )  # Concatenate a list of list into a single list.
-        if isinstance(mask[0], torch.Tensor):
-            mask = torch.stack(mask, dim=0)
-        else:
-            mask = torch.as_tensor(np.stack(mask, axis=0))
-        return mask
-
-    @classmethod
     def _organize_predictions_for_trainer(
-            cls,
-            batch_predictions: List[Tuple[List[np.ndarray], List[np.ndarray]]],
-            img_metas: List[Dict],
+        self, batch_predictions: List[DetDataSample]
     ) -> Dict[str, Tensor]:
         """
         Transform the batch of predicted labels as required by the HF trainer.
-
         :param batch_predictions: batch of predicted labels
-        :type batch_predictions: List of tuple containing list of bboxes and masks
-        :param img_metas: batch of predicted labels
-        :type img_metas: List of image metadata dictionary
+        :type batch_predictions: List of bbox list for each image
         :return: Dict of predicted labels in tensor format
         :rtype: Dict[str, Tensor]
+
+        Note: Same reasoning like _organize_ground_truth_for_trainer function but for predicted label
         """
         batch_bboxes, batch_labels, batch_masks = [], [], []
-        for (predicted_bbox, predicted_mask), img_meta in zip(batch_predictions, img_metas):
-            if isinstance(predicted_mask, tuple):
-                predicted_mask = predicted_mask[0]  # ms rcnn
-
-            bboxes, labels = super()._get_bboxes_and_labels(predicted_bbox, img_meta)
-            if predicted_mask is not None and len(labels) > 0:
-                masks = InstanceSegmentationModelWrapper._get_segmentation_masks(
-                    predicted_mask
-                )
-            else:
-                # The case when all predictions are below the box score threshold. Add empty mask tensor to satisfy
-                # the pad_sequence criteria.
-                height, width, _ = img_meta[MmDetectionDatasetLiterals.IMAGE_ORIGINAL_SHAPE]
-                masks = torch.empty(0, height, width)
+        batch_original_mask_shapes, batch_original_img_shapes = [], []
+        for predictions in batch_predictions:
+            bboxes, labels = self._get_bboxes_and_labels(predictions)
+            pred_instances = predictions.pred_instances
+
+            # HF Trainer stack the predictions of all batches together. Since prediction masks could be of
+            # different size, We are padding the masks to the max possible image size and we are removing the
+            # padding when we parse the instance segmentation outputs.
+            masks = pred_instances.masks
+            padded_masks = torch.empty(len(masks), self.max_image_size, self.max_image_size, dtype=torch.bool)
+            padded_masks[:, :masks.shape[-2], :masks.shape[-1]] = masks
+            original_mask_shape = masks.shape
+            batch_masks.append(padded_masks)
 
             batch_bboxes.append(bboxes)
             batch_labels.append(labels)
-            batch_masks.append(masks)
+            batch_original_mask_shapes.append(original_mask_shape)
+            batch_original_img_shapes.append(predictions.raw_dimensions)
 
         output = dict()
         output[MmDetectionDatasetLiterals.BBOXES] = super()._pad_sequence(batch_bboxes)
         output[MmDetectionDatasetLiterals.LABELS] = super()._pad_sequence(batch_labels)
         output[MmDetectionDatasetLiterals.MASKS] = super()._pad_sequence(batch_masks)
+        output[MmDetectionDatasetLiterals.RAW_DIMENSIONS] = \
+            torch.tensor(batch_original_img_shapes, device=get_current_device())
+        output[MmDetectionDatasetLiterals.RAW_MASK_DIMENSIONS] = \
+            torch.tensor(batch_original_mask_shapes, device=get_current_device())
         return output
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py

```diff
@@ -7,28 +7,31 @@
 import logging
 import numpy as np
 import torch
 
 from datasets import load_dataset
 from dataclasses import asdict
 from transformers import Trainer, TrainingArguments
-from typing import Dict, List, Callable
+from typing import Dict, List, Callable, Tuple
 
 from common_constants import (HFMiscellaneousLiterals,
                               Tasks,
                               MmDetectionDatasetLiterals,
-                              ODLiterals)
+                              ODLiterals,
+                              AlbumentationParameterNames)
 from mmdet_modules import ImageMetadata
+from custom_augmentations import ConstraintResize
 
 logger = logging.getLogger(__name__)
 
 
 def _parse_object_detection_output(output: Dict[str, np.ndarray], id2label: Dict[int, str]) -> List[Dict]:
     proc_op = []
-    for bboxes, labels in zip(output[MmDetectionDatasetLiterals.BBOXES], output[MmDetectionDatasetLiterals.LABELS]):
+    for bboxes, labels in zip(output[MmDetectionDatasetLiterals.BBOXES],
+                              output[MmDetectionDatasetLiterals.LABELS]):
         curimage_preds = {ODLiterals.BOXES: []}
         for bbox, label in zip(bboxes, labels):
             if label >= 0:
                 curimage_preds[ODLiterals.BOXES].append({
                     ODLiterals.BOX: {
                         ODLiterals.TOP_X: float(bbox[0]),
                         ODLiterals.TOP_Y: float(bbox[1]),
@@ -41,18 +44,27 @@
         proc_op.append(curimage_preds)
     return proc_op
 
 
 def _parse_instance_segmentation_output(output: Dict[str, np.ndarray], id2label: Dict[int, str]) -> List[Dict]:
     from masktools import convert_mask_to_polygon
     proc_op = []
-    for bboxes, labels, masks in zip(output[MmDetectionDatasetLiterals.BBOXES],
-                                     output[MmDetectionDatasetLiterals.LABELS],
-                                     output[MmDetectionDatasetLiterals.MASKS]):
+    for bboxes, labels, masks, raw_image_dimension, raw_mask_dimension in zip(
+        output[MmDetectionDatasetLiterals.BBOXES],
+        output[MmDetectionDatasetLiterals.LABELS],
+        output[MmDetectionDatasetLiterals.MASKS],
+        output[MmDetectionDatasetLiterals.RAW_DIMENSIONS],
+        output[MmDetectionDatasetLiterals.RAW_MASK_DIMENSIONS]
+    ):
         curimage_preds = {ODLiterals.BOXES: []}
+        _, h, w = raw_mask_dimension
+        # Remove the padding added to the masks to make them of equal size.
+        masks = masks[:, :h, :w]
+        # Postprocess predictions to resize masks to match original image dimensions
+        masks = resize_masks(masks=masks, raw_image_dimension=raw_image_dimension)
         for bbox, label, mask in zip(bboxes, labels, masks):
             if label >= 0:
                 box = {
                     ODLiterals.BOX: {
                         ODLiterals.TOP_X: float(bbox[0]),
                         ODLiterals.TOP_Y: float(bbox[1]),
                         ODLiterals.BOTTOM_X: float(bbox[2]),
@@ -105,45 +117,62 @@
                 num_invalid_examples = len(examples) - len(valid_examples)
                 logger.info(f"{num_invalid_examples} invalid images found.")
                 logger.info("Replacing invalid images with randomly selected valid images from the current batch")
                 new_example_indices = np.random.choice(np.arange(len(valid_examples)), num_invalid_examples)
                 for ind in new_example_indices:
                     # Padding the batch with valid examples
                     valid_examples.append(valid_examples[ind])
+        # Capture original image size in format (height, width)
+        original_image_sizes = [example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY].size[::-1] for example in examples]
 
+        resized_image_shapes = []
         # Pre processing Image
         if test_transforms is not None:
             for example in valid_examples:
-                example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY] = test_transforms(
-                    image=np.array(example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY])
-                )[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY]
+                transformed_inputs = test_transforms(
+                    image=np.array(example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY]),
+                    image_metadata=dict()
+                )
+                example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY] = transformed_inputs[
+                    HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY]
+                resized_width = transformed_inputs[AlbumentationParameterNames.IMAGE_METADATA][
+                    AlbumentationParameterNames.RESIZED_WIDTH
+                ]
+                resized_height = transformed_inputs[AlbumentationParameterNames.IMAGE_METADATA][
+                    AlbumentationParameterNames.RESIZED_HEIGHT
+                ]
+                resized_image_shapes.append((resized_height, resized_width))
 
         def to_tensor_fn(img):
             return torch.from_numpy(img.transpose(2, 0, 1)).to(dtype=torch.float)
 
-        pixel_values = torch.stack([
-            to_tensor_fn(example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY])
-            for example in valid_examples
-        ])
+        tensor_images = [to_tensor_fn(example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY])
+                         for example in valid_examples]
+        # Create a batch of images of equal size which is equal to [N, C, H_max, W_max] where
+        # H_max is the maximum height of the image in the current batch.
+        # W_max is the maximum width of the image in the current batch.
+        batched_images = make_batch(tensor_images)
 
         img_metas = []
         for i, example in enumerate(valid_examples):
             image = example[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY]
             if test_transforms:
-                width, height, no_ch = image.shape
+                height, width, no_ch = image.shape
             else:
                 width, height = image.size
                 no_ch = len(image.getbands())
             img_metas.append(
-                asdict(ImageMetadata(ori_shape=(width, height, no_ch), filename=f"test_{i}.jpg"))
+                asdict(ImageMetadata(ori_shape=(height, width, no_ch),
+                                     img_shape=resized_image_shapes[i] if test_transforms else None,
+                                     raw_dimensions=tuple(original_image_sizes[i]),
+                                     filename=f"test_{i}.jpg"))
             )
-
         # input to mmdet model should contain image and image meta data
         output = {
-            MmDetectionDatasetLiterals.IMG: pixel_values,
+            MmDetectionDatasetLiterals.IMG: batched_images,
             MmDetectionDatasetLiterals.IMG_METAS: img_metas
         }
 
         return output
 
     inference_dataset = load_dataset(
         HFMiscellaneousLiterals.IMAGE_FOLDER,
@@ -159,7 +188,81 @@
     )
     results = trainer.predict(inference_dataset)
     output = results.predictions[1]
     if task_type == Tasks.MM_OBJECT_DETECTION:
         return _parse_object_detection_output(output, id2label)
     elif task_type == Tasks.MM_INSTANCE_SEGMENTATION:
         return _parse_instance_segmentation_output(output, id2label)
+
+
+def make_batch(images: List[torch.Tensor]) -> torch.Tensor:
+    """Make batch for object detection and instance segmentation
+    Hf Trainer expects a torch tensor for input images. For OD and IS, the images in the current batch can have
+    different dimensions(due to constraintResize and other transformations applied at train time), we need to pad
+    the images to make them of equal size. To create a batch of images, we first find the maximum height and
+    maximum width of the images in the current batch. We then pad the images to match the maximum height and
+    maximum width. We then stack the images to create a batch of images.
+
+    :param images: list of Images
+    :type images: List[torch.Tensor]
+    :return: batch of Images of size [channels, height_max, width_max] where height_max and width_max are the maximum
+    height and width of the images in the current batch
+    :rtype: torch.Tensor
+    """
+    batch_width, batch_height = 0, 0
+    for img in images:
+        img_height, img_width = img.shape[-2:]
+        batch_width = max(img_width, batch_width)
+        batch_height = max(img_height, batch_height)
+
+    padded_images = []
+    for img in images:
+        img_height, img_width = img.shape[-2:]
+        if img_height != batch_height or img_width != batch_width:
+            # Only pad images when the image height or width is not equal to batch height or width respectively.
+            padded_images.append(pad_img(img, batch_width, batch_height))
+        else:
+            # No need to pad if the image height and width is equal to batch height and width respectively.
+            padded_images.append(img)
+    pixel_values = torch.stack(padded_images)
+    return pixel_values
+
+
+def pad_img(img: torch.Tensor,
+            new_width: int,
+            new_height: int) -> torch.Tensor:
+    """Pad image and to match the new width and height
+    :param img: input image
+    :type img: torch.Tensor
+    :param new_width: new width
+    :type new_width: int
+    :param new_height: new height
+    :param new_height: int
+    :return: padded image
+    :rtype: torch.Tensor
+    """
+    img_height, img_width = img.shape[-2:]
+    padded_img = torch.zeros((3, new_height, new_width), dtype=img.dtype)
+    padded_img[:, :img_height, :img_width] = img
+    return padded_img
+
+
+def resize_masks(masks: List[np.ndarray], raw_image_dimension: List) -> np.ndarray:
+    """Postprocess predictions to resize the masks to match original image dimensions
+    :masks: instance segmentation masks
+    :type masks: List[np.ndarray]
+    :img_shape: image shape after resizing
+    :type img_shape: List
+    :raw_image_dimension: Dimensions of the original image before preprocessing
+    :type raw_image_dimension: List
+    :return: resized masks
+    :return: np.ndarray
+    """
+
+    resizer = ConstraintResize(img_scale=(-1, -1))
+    h_original, w_original = raw_image_dimension
+    resized_masks = None
+    if masks is not None:
+        if masks.dtype != np.uint8:
+            masks.dtype = np.uint8
+        resized_masks = resizer.apply_to_masks(masks, w_original, h_original)
+    return resized_masks
```

## azureml/acft/image/components/finetune/defaults/constants.py

```diff
@@ -3,63 +3,85 @@
 # ---------------------------------------------------------
 
 """Finetuning component default contants."""
 
 
 from dataclasses import dataclass
 from azureml.acft.image.components.finetune.defaults.task_defaults import (
-    ClassificationDefaults,
+    MultiClassClassificationDefaults,
+    MultiLabelClassificationDefaults,
     InstanceSegmentationDefaults,
     ObjectDetectionDefaults,
+    MultiObjectTrackingDefaults,
 )
-from azureml.acft.image.components.finetune.defaults.classification_models_defaults import (
-    BEITDefaults,
-    DEITDefaults,
-    MobileVITDefaults,
-    SWINV2Defaults,
-    VITDefaults,
+from azureml.acft.image.components.finetune.defaults.multiclass_classification_models_defaults import (
+    MultiClassBEITDefaults,
+    MultiClassDEITDefaults,
+    MultiClassVITDefaults,
+    MultiClassSWINV2Defaults,
+    MultiClassMobileVITDefaults,
 )
-from azureml.acft.image.components.finetune.defaults.object_detection_models_defaults import (
-    YOLODefaults,
+from azureml.acft.image.components.finetune.defaults.multilabel_classification_models_defaults import (
+    MultiLabelBEITDefaults,
+    MultiLabelDEITDefaults,
+    MultiLabelMobileVITDefaults,
+    MultiLabelSWINV2Defaults,
+    MultiLabelVITDefaults,
 )
-from azureml.acft.image.components.finetune.defaults.instance_segmentation_models_defaults import (
-    RCNNDefaults,
-)
-from azureml.acft.image.components.finetune.huggingface.common.constants import (
-    HfProblemType,
+from azureml.acft.image.components.model_selector.constants import ImageModelSelectorConstants
+from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
+from azureml.acft.image.components.finetune.defaults.multi_object_tracking_models_defaults import (
+    ByteTrackDefaults,
 )
 
 
 @dataclass
 class TrainingDefaultsConstants:
     """
     This class contains constants for the TrainingDefaults class.
     Note: Provide mapping of model name to dataclass and task to dataclass.
     """
 
+    # model name to model family mapping
+    # if a model name matches to multiple model families, then provide a dict of task to model family
+    # mapping for that model name else provide a single model family directly
     MODEL_NAME_TO_DATACLASS_MAPPING = {
-        "yolov5": YOLODefaults,
-        "google/vit-base-patch16-224": VITDefaults,
-        "bitmodel": BEITDefaults,
-        "maskrcnn": RCNNDefaults,
-        "microsoft/beit-base-patch16-224-pt22k-ft22k": BEITDefaults,
-        "microsoft/swinv2-base-patch4-window12-192-22k": SWINV2Defaults,
-        "facebook/deit-base-patch16-224": DEITDefaults,
-        "apple/mobilevit-small": MobileVITDefaults,
+        "google/vit-base-patch16-224": {
+            Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION: MultiClassVITDefaults,
+            Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION: MultiLabelVITDefaults,
+        },
+        "microsoft/beit-base-patch16-224-pt22k-ft22k": {
+            Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION: MultiClassBEITDefaults,
+            Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION: MultiLabelBEITDefaults,
+        },
+        "microsoft/swinv2-base-patch4-window12-192-22k": {
+            Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION: MultiClassSWINV2Defaults,
+            Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION: MultiLabelSWINV2Defaults,
+        },
+        "facebook/deit-base-patch16-224": {
+            Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION: MultiClassDEITDefaults,
+            Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION: MultiLabelDEITDefaults,
+        },
+        "apple/mobilevit-small": {
+            Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION: MultiClassMobileVITDefaults,
+            Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION: MultiLabelMobileVITDefaults,
+        },
+        "bytetrack_yolox_x_crowdhuman_mot17-private-half": ByteTrackDefaults,
     }
 
     TASK_TO_DATACLASS_MAPPING = {
-        HfProblemType.MULTI_LABEL_CLASSIFICATION: ClassificationDefaults,
-        HfProblemType.SINGLE_LABEL_CLASSIFICATION: ClassificationDefaults,
-        HfProblemType.INSTANCE_SEGMENTATION: InstanceSegmentationDefaults,
-        HfProblemType.OBJECT_DETECTION: ObjectDetectionDefaults,
+        Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION: MultiClassClassificationDefaults,
+        Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION: MultiLabelClassificationDefaults,
+        Tasks.MM_INSTANCE_SEGMENTATION: InstanceSegmentationDefaults,
+        Tasks.MM_OBJECT_DETECTION: ObjectDetectionDefaults,
+        Tasks.MM_MULTI_OBJECT_TRACKING: MultiObjectTrackingDefaults,
     }
 
     MODEL_DEFAULTS_FILE = "model_defaults.json"
-    MODEL_METADATA_FILE = "model_metadata.json"
+    MODEL_METADATA_FILE = ImageModelSelectorConstants.MODEL_METAFILE_NAME
     MODEL_NAME_KEY = "model_name"
 
 
 @dataclass
 class HFTrainerDefaultsKeys:
     """
     This class contains the keys for the Hugging Face trainer defaults.
@@ -69,34 +91,38 @@
     NUM_TRAIN_EPOCHS = "num_train_epochs"
     PER_DEVICE_TRAIN_BATCH_SIZE = "per_device_train_batch_size"
     PER_DEVICE_EVAL_BATCH_SIZE = "per_device_eval_batch_size"
     LEARNING_RATE = "learning_rate"
     OPTIM = "optim"
     GRADIENT_ACCUMULATION_STEPS = "gradient_accumulation_steps"
     MAX_STEPS = "max_steps"
-    AUTO_FIND_BATCH_SIZE = "auto_find_batch_size"
-    EVALUATION_STRATEGY = "evaluation_strategy"
-    EVAL_STEPS = "eval_steps"
-    SAVE_STRATEGY = "save_strategy"
-    SAVE_STEPS = "save_steps"
-    LOGGING_STRATEGY = "logging_strategy"
-    LOGGING_STEPS = "logging_steps"
     WARMUP_STEPS = "warmup_steps"
     WEIGHT_DECAY = "weight_decay"
     ADAM_BETA1 = "adam_beta1"
     ADAM_BETA2 = "adam_beta2"
     ADAM_EPSILON = "adam_epsilon"
     LR_SCHEDULING_TYPE = "lr_scheduler_type"
-    DATALOADER_NUM_WORKERS = "dataloader_num_workers"
-    SEED = "seed"
-    SAVE_TOTAL_LIMIT = "save_total_limit"
+    METRIC_FOR_BEST_MODEL = "metric_for_best_model"
+    LABEL_SMOOTHING_FACTOR = "label_smoothing_factor"
+    MAX_GRAD_NORM = "max_grad_norm"
+    SAVE_SAFETENSORS = "save_safetensors"
 
 
 @dataclass
 class NonHfTrainerDefaultsKeys:
     """
     This class contains the keys for the non Hugging Face trainer defaults.
 
     """
 
     IMAGE_WIDTH = "image_width"
     IMAGE_HEIGHT = "image_height"
+    IMAGE_MIN_SIZE = "image_min_size"
+    IMAGE_MAX_SIZE = "image_max_size"
+    # adamw hyperparameters are not part of HF Training Arguments but part of Namespace
+    ADAM_BETA1 = "adam_beta1"
+    ADAM_BETA2 = "adam_beta2"
+    ADAM_EPSILON = "adam_epsilon"
+    IOU_THRESHOLD = "iou_threshold"
+    BOX_SCORE_THRESHOLD = "box_score_threshold"
+    APPLY_ORT = "apply_ort"
+    APPLY_DEEPSPEED = "apply_deepspeed"
```

## azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py

```diff
@@ -19,26 +19,18 @@
     _num_train_epochs: int = 3
     _per_device_train_batch_size: int = 8
     _per_device_eval_batch_size: int = 8
     _learning_rate: float = 5e-5
     _optim: str = "adamw_hf"
     _gradient_accumulation_steps: int = 1
     _max_steps: int = -1
-    _auto_find_batch_size: bool = False
-    _evaluation_strategy: str = "steps"
-    _eval_steps: int = 500
-    _save_strategy: str = "steps"
-    _save_steps: int = 500
-    _logging_strategy: str = "steps"
-    _logging_steps: int = 500
     _warmup_steps: int = 0
     _weight_decay: float = 0.0
     _adam_beta1: float = 0.9
     _adam_beta2: float = 0.999
     _adam_epsilon: float = 1e-8
     _lr_scheduler_type: str = "linear"
-    _dataloader_num_workers: int = 0
-    _seed: int = 42
-    _save_total_limit: int = 1
     _metric_for_best_model: str = "loss"
     _label_smoothing_factor: float = 0.0
     _max_grad_norm: float = 1.0
+    _apply_deepspeed: bool = False
+    _apply_ort: bool = False
```

## azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py

```diff
@@ -16,10 +16,8 @@
     """
     This class contain trainer defaults specific to RCNN models.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    _per_device_train_batch_size: int = 4
-    _per_device_eval_batch_size: int = 4
-    _learning_rate: float = 5e-4
+    # todo: add the defaults for RCNN model family
```

## azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py

```diff
@@ -16,10 +16,8 @@
     """
     This class contain trainer defaults specific to YOLO models.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    _per_device_train_batch_size: int = 4
-    _per_device_eval_batch_size: int = 4
-    _learning_rate: float = 5e-4
+    # todo: add the defaults for YOLO model family
```

## azureml/acft/image/components/finetune/defaults/task_defaults.py

```diff
@@ -7,55 +7,107 @@
 from dataclasses import dataclass
 from azureml.acft.image.components.finetune.defaults.hf_trainer_defaults import (
     HFTrainerDefaults,
 )
 
 
 @dataclass
-class ClassificationDefaults(HFTrainerDefaults):
+class MultiClassClassificationDefaults(HFTrainerDefaults):
     """
-    This class contain trainer defaults specific to classification models.
+    This class contain trainer defaults specific to multiclass classification models.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    _image_width: int = 224
-    _image_height: int = 224
     _num_train_epochs: int = 15
-    _evaluation_strategy: str = "epoch"
-    _save_strategy: str = "epoch"
-    _logging_strategy: str = "epoch"
     _lr_scheduler_type: str = "cosine"
-    _dataloader_num_workers: int = 6
-    _seed: int = 43
-    _save_total_limit: int = -1
+    _metric_for_best_model: str = "accuracy"
+
+
+@dataclass
+class MultiLabelClassificationDefaults(HFTrainerDefaults):
+    """
+    This class contain trainer defaults specific to multilabel classification models.
+
+    Note: This class is not meant to be used directly.
+    Provide the defaults name consistently with the Hugging Face Trainer class.
+    """
+
+    _num_train_epochs: int = 15
+    _lr_scheduler_type: str = "cosine"
+    _metric_for_best_model: str = "iou"
+    _label_smoothing_factor: float = 0.0
+    # Setting it to 0.0 as label_smoothing_factor is not supported for multi-label classification.
 
 
 @dataclass
 class ObjectDetectionDefaults(HFTrainerDefaults):
     """
     This class contain trainer defaults specific to object detection models.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    # todo: updated defaults for object detection after benchmarking
-    _per_device_train_batch_size: int = 4
-    _per_device_eval_batch_size: int = 4
-    _learning_rate: float = 5e-4
+    _image_max_size: int = -1
+    _image_min_size: int = -1
+    _num_train_epochs: int = 10
+    _per_device_train_batch_size: int = 2
+    _per_device_eval_batch_size: int = 2
+    _optim: str = "adamw_torch"
+    _learning_rate: float = 1e-5
+    _warmup_steps: int = 1
+    _weight_decay: float = 1.4679630586541725e-05
+    _lr_scheduler_type: str = "cosine"
+    _metric_for_best_model: str = "mean_average_precision"
+    _iou_threshold: float = 0.5
+    _box_score_threshold: float = 0.3
 
 
 @dataclass
 class InstanceSegmentationDefaults(HFTrainerDefaults):
     """
     This class contain trainer defaults specific to instance segmentation models.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    # todo: updated defaults for instance segmentation after benchmarking
-    _per_device_train_batch_size: int = 4
-    _per_device_eval_batch_size: int = 4
-    _learning_rate: float = 5e-4
+    _image_max_size: int = -1
+    _image_min_size: int = -1
+    _num_train_epochs: int = 10
+    _per_device_train_batch_size: int = 1
+    _per_device_eval_batch_size: int = 1
+    _optim: str = "adamw_torch"
+    _learning_rate: float = 9.674567440430093e-05
+    _warmup_steps: int = 1
+    _weight_decay: float = 6.335073210739572e-06
+    _lr_scheduler_type: str = "cosine"
+    _metric_for_best_model: str = "mean_average_precision"
+    _iou_threshold: float = 0.5
+    _box_score_threshold: float = 0.3
+
+
+@dataclass
+class MultiObjectTrackingDefaults(HFTrainerDefaults):
+    """
+    This class contain trainer defaults specific to multi-object tracking models.
+
+    Note: This class is not meant to be used directly.
+    Provide the defaults name consistently with the Hugging Face Trainer class.
+    """
+
+    # todo: updated defaults for object tracking after benchmarking
+    _per_device_train_batch_size: int = 1
+    _per_device_eval_batch_size: int = 1
+    _learning_rate: float = 1e-4
+    _optim: str = "sgd"
+    _num_train_epochs: int = 10
+    _warmup_steps: int = 1
+    _weight_decay: float = 1.4679630586541725e-05
+    _lr_scheduler_type: str = "cosine"
+    _metric_for_best_model: str = "MOTA"
+    _iou_threshold: float = 0.5
+    _box_score_threshold: float = 0.3
+    _image_width: int = -1
+    _image_height: int = -1
```

## azureml/acft/image/components/finetune/defaults/training_defaults.py

```diff
@@ -23,14 +23,15 @@
 from typing import Optional, Union
 from transformers import TrainingArguments
 
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.image.components.finetune.defaults.hf_trainer_defaults import (
     HFTrainerDefaults,
 )
+from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
 from azureml.acft.image.components.finetune.defaults.constants import (
     TrainingDefaultsConstants,
     NonHfTrainerDefaultsKeys,
 )
 
 logger = get_logger_app(__name__)
 
@@ -64,49 +65,48 @@
         :rtype: None
         """
         self.task = task
         self.model_path = None
         self.model_name = None
         self.defaults_dict = None
 
-        if model_name_or_path is not None and os.path.isdir(model_name_or_path):
-            self.model_path = model_name_or_path
-            model_metadata_file = os.path.join(
-                self.model_path, TrainingDefaultsConstants.MODEL_METADATA_FILE
-            )
+        if model_name_or_path is not None and (
+            os.path.isdir(model_name_or_path)
+            or (os.path.isfile(model_name_or_path) and model_name_or_path.endswith(".py"))
+        ):
+            if os.path.isdir(model_name_or_path):
+                self.model_path = model_name_or_path
+            else:
+                self.model_path = os.path.dirname(model_name_or_path)
+            model_metadata_file = os.path.join(self.model_path, TrainingDefaultsConstants.MODEL_METADATA_FILE)
             data_dict = self._get_data_from_file(model_metadata_file)
-            if TrainingDefaultsConstants.MODEL_NAME_KEY in data_dict:
+            if data_dict is not None and TrainingDefaultsConstants.MODEL_NAME_KEY in data_dict:
                 self.model_name = data_dict[TrainingDefaultsConstants.MODEL_NAME_KEY]
+            else:
+                logger.info("Unable to read model name from model metadata file.")
         elif model_name_or_path is not None:
             self.model_name = model_name_or_path
 
         # get the dataclass defaults based on the task and model family
         self.dataclass_defaults = self._get_training_defaults_dataclass()
         self.defaults_dict = self._get_dict_from_dataclass(self.dataclass_defaults)
 
         # If the model architecture is supported, then the defaults are selected based on the model architecture.
         if self.model_path is not None:
-            model_defaults_file = os.path.join(
-                self.model_path, TrainingDefaultsConstants.MODEL_DEFAULTS_FILE
-            )
+            model_defaults_file = os.path.join(self.model_path, TrainingDefaultsConstants.MODEL_DEFAULTS_FILE)
             model_defaults_dict = self._get_data_from_file(model_defaults_file)
             # take the union of dictionaries model defaults dict and defaults dict with precedence
             # given to model defaults dict
             if model_defaults_dict is not None:
-                logger.info(
-                    f"Using the defaults from {TrainingDefaultsConstants.MODEL_DEFAULTS_FILE}"
-                )
+                logger.info(f"Using the defaults from {TrainingDefaultsConstants.MODEL_DEFAULTS_FILE}")
                 self.defaults_dict.update(model_defaults_dict)
 
         # validate and update the default dictionary
         self.defaults_dict = self._validate_and_update_defaults_dict(self.defaults_dict)
 
-        # log the defaults
-        logger.info(f"Training defaults used: {self.defaults_dict}")
-
     @staticmethod
     def _get_data_from_file(file_path: str) -> dict:
         """This method returns the data from the file.
 
         :param file_path: The path to the file.
         :type file_path: str
         :return: The data from the file.
@@ -143,41 +143,48 @@
     def _get_training_defaults_dataclass(self) -> object:
         """This method returns the training defaults dataclass.
 
         :return: The training defaults dataclass.
         :rtype: object
         """
 
-        task_defaults = TrainingDefaultsConstants.TASK_TO_DATACLASS_MAPPING.get(
-            self.task, HFTrainerDefaults
-        )
-        model_defaults = TrainingDefaultsConstants.MODEL_NAME_TO_DATACLASS_MAPPING.get(
-            self.model_name, task_defaults
-        )
+        task_defaults = TrainingDefaultsConstants.TASK_TO_DATACLASS_MAPPING.get(self.task, HFTrainerDefaults)
+
+        # get the model family defaults
+        # identify the model family defaults or model families defaults from the model name
+        # as single model could match to multiple model families depending on the task
+        matched_model_families = TrainingDefaultsConstants.MODEL_NAME_TO_DATACLASS_MAPPING.get(self.model_name, None)
+
+        if matched_model_families is None:
+            # if model family is not supported, then use the task defaults
+            model_family_defaults = task_defaults
+        elif isinstance(matched_model_families, dict):
+            # if model name matches to multiple model families, then use the task defaults
+            # to identify the model family defaults
+            model_family_defaults = matched_model_families.get(self.task, task_defaults)
+        else:
+            # if model name matches to single model family, then use the model family defaults
+            model_family_defaults = matched_model_families
 
-        return model_defaults()
+        return model_family_defaults()
 
     @staticmethod
     def _validate_and_update_defaults_dict(defaults_dict: dict) -> dict:
         """This method validates the default dictionary.
 
         :param defaults_dict: The default dictionary.
         :type defaults_dict: dict
         :return: The updated default dictionary.
         :rtype: dict
         """
         updated_defaults_dict = {}
         for key, value in defaults_dict.items():
             # check is key is present in TrainingArguments dataclass
             # and value has the same type as the dataclass attribute
-            if key in NonHfTrainerDefaultsKeys.__dict__.values() or hasattr(
-                TrainingArguments, key
-            ):
+            if key in NonHfTrainerDefaultsKeys.__dict__.values() or hasattr(TrainingArguments, key):
                 # add key value in updated defaults dict
                 updated_defaults_dict[key] = value
             else:
                 # log warning if the key is not present in TrainingArguments dataclass
-                logger.warning(
-                    f"{key} is not a valid training argument. It cannot be used for training defaults."
-                )
+                logger.warning(f"{key} is not a valid training argument. It cannot be used for training defaults.")
 
         return updated_defaults_dict
```

## azureml/acft/image/components/finetune/factory/mappings.py

```diff
@@ -8,13 +8,16 @@
 
 
 @dataclass
 class MODEL_FAMILY_CLS:
     """A class to represent model family constants."""
     HUGGING_FACE_IMAGE = "HuggingFaceImage"
     MMDETECTION_IMAGE = "MmDetectionImage"
+    MMTRACKING_VIDEO = "MmTrackingVideo"
 
 
 MODEL_FAMILY_MODULE_IMPORT_PATH_MAP = OrderedDict([
     (MODEL_FAMILY_CLS.HUGGING_FACE_IMAGE, "azureml.acft.image.components.finetune.huggingface"),
     (MODEL_FAMILY_CLS.MMDETECTION_IMAGE, "azureml.acft.image.components.finetune.mmdetection"),
+    (MODEL_FAMILY_CLS.MMTRACKING_VIDEO, "azureml.acft.image.components.finetune.mmtracking"),
+
 ])
```

## azureml/acft/image/components/finetune/factory/model_factory.py

```diff
@@ -20,15 +20,16 @@
 logger = get_logger_app(__name__)
 
 
 class ModelFactory:
     """Class for fetching and returning model."""
 
     def __init__(self, model_family: MODEL_FAMILY_CLS, model_id: str,
-                 task_name: str=Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION):
+                 task_name: str=Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
+                 model_metadata: dict={}):
         """
         init function for ModelFactory
         """
         if model_family not in MODEL_FAMILY_MODULE_IMPORT_PATH_MAP:
             raise ACFTValidationException._with_error(
                 AzureMLError.create(
                     ModelFamilyNotSupported,
@@ -41,14 +42,14 @@
         try:
             module = importlib.import_module(MODEL_FAMILY_MODULE_IMPORT_PATH_MAP[model_family])
         except ImportError as e:
             logger.error(f"Unable to import the module. model family: {model_family}. Error: {e}")
             raise ImportError(f"Unable to import the module. model family: {model_family}. Error: {e}")
 
         # Set the model factory output
-        trainer_classes_obj = getattr(module, "TrainerClasses")(model_family, model_id, task_name)
+        trainer_classes_obj = getattr(module, "TrainerClasses")(model_family, model_id, task_name, model_metadata)
         self.trainer_classes = trainer_classes_obj.get_trainer_classes_mapping()
 
     @property
     def get_trainer_classes(self):
         """Get trainer classes."""
         return self.trainer_classes
```

## azureml/acft/image/components/finetune/factory/task_definitions.py

```diff
@@ -8,7 +8,8 @@
 class Tasks:
     "Tasks supported for All Frameworks"
 
     HF_MULTI_CLASS_IMAGE_CLASSIFICATION = "image-classification"
     HF_MULTI_LABEL_IMAGE_CLASSIFICATION = "image-classification-multilabel"
     MM_OBJECT_DETECTION = "image-object-detection"
     MM_INSTANCE_SEGMENTATION = "image-instance-segmentation"
+    MM_MULTI_OBJECT_TRACKING = "video-multi-object-tracking"
```

## azureml/acft/image/components/finetune/huggingface/__init__.py

```diff
@@ -15,30 +15,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """AzureML ACFT Image Components package - finetuning component huggingface."""
 
 import os
+import inspect
 
 from collections import OrderedDict
 from typing import Union
-from transformers import AutoConfig
+from transformers import AutoConfig, AutoModelForImageClassification
 from transformers.models.auto.modeling_auto import (
     MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING_NAMES,
 )
 
 from azureml.acft.image.components.finetune.factory.mappings import MODEL_FAMILY_CLS
 from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
-from azureml.acft.image.components.finetune.common.constants.constants import HfConstants
+from azureml.acft.image.components.finetune.common.constants.constants import HfConstants, ImageDataItemLiterals
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
-from azureml.acft.common_components.utils.error_handling.error_definitions import ModelIncompatibleWithTask
+from azureml.acft.common_components.utils.error_handling.error_definitions import (
+    ModelIncompatibleWithTask,
+    NotSupported
+)
 from azureml.acft.image.components.finetune.huggingface.classification.trainer_classes import (
     ImageClassificationTrainerClasses,
 )
 
 logger = get_logger_app(__name__)
 
 
@@ -49,29 +53,36 @@
     ]
 )
 
 
 class TrainerClasses:
     """Class for fetching and returning trainer classes."""
     def __init__(
-        self, model_family: MODEL_FAMILY_CLS, model_name_or_path: Union[str, os.PathLike], task_name: Tasks
+        self,
+        model_family: MODEL_FAMILY_CLS,
+        model_name_or_path: Union[str, os.PathLike],
+        task_name: Tasks,
+        model_metadata: dict = {},
     ) -> None:
         """ init function for TrainerClasses
         :param model_family: related model_family to which current task belongs
         :type model_family: azureml.acft.accelerator.mappings.MODEL_FAMILY_CLS
         :param model_name_or_path: Hugging face image model name or path
         :type model_name_or_path: Union[str, os.PathLike]
         :param task_name: related task_name
         :type task_name: azureml.acft.accelerator.constants.task_definitions.Tasks
+        :param model_metafile_path: path to model metafile
+        :type model_metafile_path: Union[str, os.PathLike]
         """
         self.model_family = model_family
         self.task_name = task_name
         self.model_name_or_path = model_name_or_path
         self.model_type = TrainerClasses.get_hf_model_type(self.model_name_or_path)
         self._check_task_model_family_compatibility()
+        self._is_finetuning_supported()
 
     @staticmethod
     def get_hf_model_type(model_name_or_path: Union[str, os.PathLike]) -> Union[str, None]:
         """Get model_type from model_name or model_path
 
         :param model_name_or_path: Hugging face image model name or path
         :type model_name_or_path: Union[str, os.PathLike]
@@ -110,16 +121,55 @@
             raise ACFTValidationException._with_error(
                 AzureMLError.create(
                     ModelIncompatibleWithTask,
                     TaskName=self.task_name,
                     ModelName=self.model_name_or_path,
                 )
             )
-        else:
-            return
+        return
+
+    def _is_finetuning_supported(self):
+        """Check if finetuning is supported for the given model and task."""
+        if self.task_name in [
+                Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
+                Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION
+        ]:
+            try:
+                model = AutoModelForImageClassification.from_pretrained(self.model_name_or_path)
+            except Exception as e:
+                error_str = f"Finetuning is not supported for the given model. The model \
+                {self.model_name_or_path} cannot be loaded. Only models that can be loaded \
+                with transformers.AutoModelForImageClassification are supported for finetuning."
+                logger.error(f"{error_str}. {e}")
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(
+                        NotSupported,
+                        TaskName=self.task_name,
+                        ModelName=self.model_name_or_path,
+                        scenario_name=error_str,
+                    )
+                )
+
+            # finetuning is supported only when forward has labels param.
+            signature = inspect.signature(model.forward)
+            params = signature.parameters.keys()
+            if ImageDataItemLiterals.HF_LABELS_KEY not in params:
+                error_str = f"Finetuning is not supported for the given model. \
+                Could not find {ImageDataItemLiterals.HF_LABELS_KEY} in signature parameters of model.forward. \
+                Finetuning is supported only when forward method has labels param."
+                logger.error(error_str)
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(
+                        NotSupported,
+                        TaskName=self.task_name,
+                        ModelName=self.model_name_or_path,
+                        scenario_name=error_str
+                    )
+                )
+        return
 
     def get_trainer_classes_mapping(self):
         """Cet trainer class based on task_name."""
         if self.task_name in [
             Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
             Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION,
         ]:
```

## azureml/acft/image/components/finetune/huggingface/classification/data_cls.py

```diff
@@ -45,14 +45,15 @@
     HfProblemType,
 )
 from azureml.acft.image.components.finetune.interfaces.azml_interface import AzmlDataInterface
 
 from azureml.acft.image.components.finetune.common.data.runtime_classification_dataset import (
     get_classification_dataset,
 )
+from azureml.acft.image.components.finetune.common.data.data_utils import filter_invalid_images
 
 logger = get_logger_app(__name__)
 
 
 class AzmlHfImageDataInterface(AzmlDataInterface):
     """Data interface for Hf Image Models"""
 
@@ -79,38 +80,41 @@
     def _get_train_valid_augmentation_transforms(self, **kwargs) -> Tuple[Optional[Callable], Optional[Callable]]:
         """Get train and/or validation transforms
 
         :return: A tuple with train and validation transform
         :rtype: Tuple[Optional[Callable], Optional[Callable]]
         """
         train_transform, valid_transform = None, None
-        if not self.apply_augmentations:
-            return train_transform, valid_transform
 
         logger.info(f"Feature Extractor config as dict: {self.model_preprocessing_param_dict}")
 
         # Note/Todo: read config_path from the params once the option is open to user.
         config_path = os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
             "..",
             "..",
             "common/augmentation",
-            AugmentationConfigFileNames.HF_CLASSIFICATION_ALBUMENTATIONS_CONFIG,
+            AugmentationConfigFileNames.CLASSIFICATION_ALBUMENTATIONS_CONFIG,
         )
         augmentation_class_obj = AlbumAugmentations(
             config_path=config_path,
             model_preprocessing_params_dict=self.model_preprocessing_param_dict,
             **kwargs,
         )
         # Note/Todo: Output augmentation_class_obj.augmentations_dict to one of the output ports.
 
-        # Get train and valid transforms
-        train_transform = augmentation_class_obj.get_train_transform()
+        # Get valid transforms
         valid_transform = augmentation_class_obj.get_valid_transform()
 
+        if not self.apply_augmentations:
+            # If no augmentations are applied, we only want to apply the validation transformations.
+            return valid_transform, valid_transform
+
+        # Get train transforms
+        train_transform = augmentation_class_obj.get_train_transform()
         return train_transform, valid_transform
 
     def _set_dataset_classes(self, **kwargs) -> None:
         """Set dataset classes
 
         :return: None
         :rtype: None
@@ -154,45 +158,53 @@
         """get validation dataset
 
         :return : validation dataset
         :rtype: BaseDataset
         """
         return self.validation_ds
 
+    def image_classification_collate_func(self, data_list: List[Dict[str, Any]]) -> Dict[str, torch.tensor]:
+        """
+        Collate function for image classification.
+
+        :param data_list: A list of dictionaries with image and label keys.
+        :type data_list: List[Dict[str, Any]]
+
+        :return: A dictionary with images and labels.
+        :rtype: Dict[str, torch.Tensor]
+        """
+        valid_data_list = filter_invalid_images(data_list, ImageDataItemLiterals.DEFAULT_IMAGE_KEY)
+        if self.multi_label:
+            labels = np.zeros((len(data_list), len(self.label2id)), dtype=np.float64)
+            for idx, data in enumerate(valid_data_list):
+                for label in data[ImageDataItemLiterals.DEFAULT_LABEL_KEY]:
+                    labels[idx][label] = 1
+        else:
+            labels = np.array(
+                [data[ImageDataItemLiterals.DEFAULT_LABEL_KEY] for data in valid_data_list],
+                dtype=np.int64,
+            )
+        labels_tensor = torch.tensor(labels)
+
+        images = [data[ImageDataItemLiterals.DEFAULT_IMAGE_KEY] for data in valid_data_list]
+
+        output_dict = dict()
+
+        def to_tensor_fn(img):
+            # Converting to torch tensor(CHW format) from numpy array(HWC format)
+            return torch.from_numpy(img.transpose(2, 0, 1)).to(dtype=torch.float)
+
+        output_dict[ImageDataItemLiterals.HF_PIXEL_VALUES_KEY] = torch.stack([to_tensor_fn(img) for img in images])
+        output_dict.update({ImageDataItemLiterals.HF_LABELS_KEY: labels_tensor})
+        return output_dict
+
     def get_collation_function(
         self,
     ) -> Callable[[List[Dict[str, Any]]], Dict[str, torch.tensor]]:
         """
-        collate function for hugging face image classification
+        Get the collate function for Hugging Face image classification.
 
-        return: callable function
-        rtype: Callable[[List[Dict[str, Any]]], Dict[str, torch.tensor]]
+        :return: A callable collate function.
+        :rtype: Callable[[List[Dict[str, Any]]], Dict[str, torch.Tensor]]
         """
 
-        def image_classification_collate_func(data_list: List[Dict[str, Any]]) -> Dict[str, torch.tensor]:
-            """
-            param data_list: list of dict with image and label key
-            type data_list: list[Dict]
-            return: dict with images and labels key
-            rtype: Dict[str, torch.tensor]
-            """
-            if self.multi_label:
-                labels = np.zeros((len(data_list), len(self.label2id)), dtype=np.float64)
-                for idx, data in enumerate(data_list):
-                    for label in data[ImageDataItemLiterals.DEFAULT_LABEL_KEY]:
-                        labels[idx][label] = 1
-            else:
-                labels = np.array(
-                    [data[ImageDataItemLiterals.DEFAULT_LABEL_KEY] for data in data_list],
-                    dtype=np.int64,
-                )
-            labels_tensor = torch.tensor(labels)
-
-            images = [data[ImageDataItemLiterals.DEFAULT_IMAGE_KEY] for data in data_list]
-
-            # When apply_augmentations is set to true, the dataset will return transformed images.
-            # use the basic preprocessing from HF feature extractor at the end.
-            output_dict = self.image_processor(images, return_tensors="pt")
-            output_dict.update({ImageDataItemLiterals.HF_LABELS_KEY: labels_tensor})
-            return output_dict
-
-        return image_classification_collate_func
+        return self.image_classification_collate_func
```

## azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py

```diff
@@ -1,24 +1,28 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Hf image classification finetune class."""
 
 from typing import Any, Dict
+from functools import partial
 
+from transformers.training_args import OptimizerNames
+from azureml.acft.accelerator.constants import HfTrainerMethodsConstants
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
 from azureml.acft.image.components.finetune.common.constants.constants import SettingLiterals, SettingParameters
 from azureml.acft.image.components.finetune.huggingface.common.constants import (
     HfImageInterfaceConstants,
     HfImageModelConstants,
     HfProblemType,
 )
 from azureml.acft.image.components.finetune.interfaces.azml_interface import AzmlFinetuneInterface
+from azureml.acft.image.components.finetune.common.trainer.train_helper import get_custom_optimizer
 
 logger = get_logger_app(__name__)
 
 
 class AzmlHfImageClsFinetune(AzmlFinetuneInterface):
     """Hf image classification finetune class."""
 
@@ -53,8 +57,16 @@
 
     def get_custom_trainer_functions(self) -> Dict[str, Any]:
         """Customizable methods for trainer class
 
         :return: dictionary of custom trainer methods needed for image models
         :rtype: Dict[str, Any]
         """
+        if self.params.get(SettingLiterals.OPTIMIZER, None) == OptimizerNames.SGD \
+           and self.params.get(SettingLiterals.EXTRA_OPTIMIZER_ARGS, None):
+            sgd_optimizer = partial(get_custom_optimizer,
+                                    optimizer_name=self.params[SettingLiterals.OPTIMIZER],
+                                    extra_optim_args=self.params[SettingLiterals.EXTRA_OPTIMIZER_ARGS],
+                                    weight_decay=self.params.get(SettingLiterals.WEIGHT_DECAY, 0.0))
+
+            return {HfTrainerMethodsConstants.AZUREML_OPTIMIZER: sgd_optimizer}
         return {}
```

## azureml/acft/image/components/finetune/huggingface/common/constants.py

```diff
@@ -26,7 +26,8 @@
 class HfProblemType:
     """problem types used by hugging face models internally"""
 
     SINGLE_LABEL_CLASSIFICATION = "single_label_classification"
     MULTI_LABEL_CLASSIFICATION = "multi_label_classification"
     OBJECT_DETECTION = "object_detection"
     INSTANCE_SEGMENTATION = "instance_segmentation"
+    MULTI_OBJECT_TRACKING = "multi_object_tracking"
```

## azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py

```diff
@@ -273,45 +273,48 @@
         # RGB -> resize -> center_crop -> rescale -> normalize
         do_center_crop = hasattr(
             image_processor, HfProcessorParamNames.DO_CENTER_CROP_KEY
         ) and getattr(image_processor, HfProcessorParamNames.DO_CENTER_CROP_KEY)
         do_resize = hasattr(
             image_processor, HfProcessorParamNames.DO_RESIZE_KEY
         ) and getattr(image_processor, HfProcessorParamNames.DO_RESIZE_KEY)
-        if do_center_crop and do_resize:
-            image_processor.size = AzmlHfImageFeatureExtractor.update_resize_size_dict(
-                image_processor=image_processor,
-                image_height=kwargs[SettingLiterals.IMAGE_HEIGHT],
-                image_width=kwargs[SettingLiterals.IMAGE_WIDTH],
-                do_center_crop=do_center_crop,
-            )
-            image_processor.crop_size = {
-                HfProcessorParamNames.HEIGHT_KEY: kwargs[
-                    SettingLiterals.IMAGE_HEIGHT
-                ],
-                HfProcessorParamNames.WIDTH_KEY: kwargs[
-                    SettingLiterals.IMAGE_WIDTH
-                ],
-            }
-        elif do_center_crop:
-            image_processor.crop_size = {
-                HfProcessorParamNames.HEIGHT_KEY: kwargs[
-                    SettingLiterals.IMAGE_HEIGHT
-                ],
-                HfProcessorParamNames.WIDTH_KEY: kwargs[
-                    SettingLiterals.IMAGE_WIDTH
-                ],
-            }
-        elif do_resize:
-            image_processor.size = AzmlHfImageFeatureExtractor.update_resize_size_dict(
-                image_processor=image_processor,
-                image_height=kwargs[SettingLiterals.IMAGE_HEIGHT],
-                image_width=kwargs[SettingLiterals.IMAGE_WIDTH],
-                do_center_crop=False,
-            )
+
+        if kwargs[SettingLiterals.IMAGE_HEIGHT] != -1 and kwargs[SettingLiterals.IMAGE_WIDTH] != -1:
+            # User has provided image height and width, Updating feature extractor values for height and width
+            if do_center_crop and do_resize:
+                image_processor.size = AzmlHfImageFeatureExtractor.update_resize_size_dict(
+                    image_processor=image_processor,
+                    image_height=kwargs[SettingLiterals.IMAGE_HEIGHT],
+                    image_width=kwargs[SettingLiterals.IMAGE_WIDTH],
+                    do_center_crop=do_center_crop,
+                )
+                image_processor.crop_size = {
+                    HfProcessorParamNames.HEIGHT_KEY: kwargs[
+                        SettingLiterals.IMAGE_HEIGHT
+                    ],
+                    HfProcessorParamNames.WIDTH_KEY: kwargs[
+                        SettingLiterals.IMAGE_WIDTH
+                    ],
+                }
+            elif do_center_crop:
+                image_processor.crop_size = {
+                    HfProcessorParamNames.HEIGHT_KEY: kwargs[
+                        SettingLiterals.IMAGE_HEIGHT
+                    ],
+                    HfProcessorParamNames.WIDTH_KEY: kwargs[
+                        SettingLiterals.IMAGE_WIDTH
+                    ],
+                }
+            elif do_resize:
+                image_processor.size = AzmlHfImageFeatureExtractor.update_resize_size_dict(
+                    image_processor=image_processor,
+                    image_height=kwargs[SettingLiterals.IMAGE_HEIGHT],
+                    image_width=kwargs[SettingLiterals.IMAGE_WIDTH],
+                    do_center_crop=False,
+                )
         logger.info(
             f"Updating Feature Extractor with: {image_processor.to_dict()}"
         )
         # Todo - if we find a better way, update it.
         # Get the feature extractor using the updated dict. This way save_pretrained will save the right values.
         image_processor = AutoImageProcessor.from_pretrained(
             hf_image_model_name_or_path, **image_processor.to_dict()
@@ -336,63 +339,18 @@
     ) -> PretrainedConfig:
         """
         :param hf_image_model_name_or_path: Hugging face image model name or path
         :type hf_image_model_name_or_path: Union[str, os.PathLike]
         :return: config object containing information about the model.
         :rtype: PretrainedConfig
         """
-        config = AutoConfig.from_pretrained(hf_image_model_name_or_path, **kwargs,)
-        # Update the image size in the model
-        if hasattr(config, HfImageModelConstants.HF_MODEL_CONFIG_IMAGE_SIZE_KEY):
-            image_size = getattr(
-                config, HfImageModelConstants.HF_MODEL_CONFIG_IMAGE_SIZE_KEY
-            )
-            if isinstance(image_size, int):
-                if (
-                    kwargs[SettingLiterals.IMAGE_WIDTH]
-                    != kwargs[SettingLiterals.IMAGE_HEIGHT]
-                ):
-                    error_string = (
-                        f"The model expects same values for image height and width. "
-                        f"Inputs given, height: {kwargs[SettingLiterals.IMAGE_HEIGHT]}, "
-                        f"width: {kwargs[SettingLiterals.IMAGE_WIDTH]}"
-                    )
-
-                    raise ACFTValidationException._with_error(
-                        AzureMLError.create(
-                            ACFTUserError, pii_safe_message=error_string
-                        )
-                    )
-                image_size_update = {
-                    HfImageModelConstants.HF_MODEL_CONFIG_IMAGE_SIZE_KEY: kwargs[
-                        SettingLiterals.IMAGE_HEIGHT
-                    ]
-                }
-            else:
-                assert isinstance(image_size, list) or isinstance(
-                    image_size, tuple
-                ), f"Models' image size is of type {type(image_size)}, not supported."
-                image_size_update = {
-                    HfImageModelConstants.HF_MODEL_CONFIG_IMAGE_SIZE_KEY: [
-                        kwargs[SettingLiterals.IMAGE_WIDTH],
-                        kwargs[SettingLiterals.IMAGE_HEIGHT],
-                    ]
-                }
-            logger.info(
-                f"Original Model {HfImageModelConstants.HF_MODEL_CONFIG_IMAGE_SIZE_KEY}: {image_size}"
-            )
-            config.update(image_size_update)
-
-            # Todo - if we find a better way, update it.
-            # Get the model config using the updated dict. This way save_pretrained will save the right values.
-            config = AutoConfig.from_pretrained(
-                hf_image_model_name_or_path, **config.to_dict()
-            )
-
-            logger.info(f"Updated Model Config: {config}")
+        config = AutoConfig.from_pretrained(hf_image_model_name_or_path, **kwargs)
+        # No need to manipulate the image_size in model config since the image_size is used to
+        # construct the positional embeddings layer of the network, manipulating it will lead to
+        # suboptimal performance for model families such as DinoV2 which uses positional embeddings.
         return config
 
 
 class AzmlHfImageModel(AzmlModelInterface):
     """Get model based on the model_name or path."""
     @classmethod
     def from_pretrained(
```

## azureml/acft/image/components/finetune/mmdetection/__init__.py

```diff
@@ -1,55 +1,159 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """AzureML ACFT Image Components package - finetuning component MMDetection."""
 
 import os
+import json
 from typing import Union
 
+from mmengine import Config
+from mmdet.apis import init_detector
+from mmdet.models.detectors.two_stage import TwoStageDetector
+
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 from azureml.acft.common_components import get_logger_app
-from azureml.acft.common_components.utils.error_handling.error_definitions import TaskNotSupported
-from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
+from azureml.acft.common_components.model_selector.constants import (
+    ModelRepositoryURLs
+)
+from azureml.acft.common_components.utils.error_handling.error_definitions import (
+    TaskNotSupported,
+    ModelIncompatibleWithTask,
+    InvalidData,
+    NotSupported,
+    ValidationError
+)
+from azureml.acft.common_components.utils.error_handling.exceptions import (
+    ACFTValidationException,
+    ACFTSystemException
+)
 
 from azureml.acft.image.components.finetune.factory.mappings import MODEL_FAMILY_CLS
 from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
+from azureml.acft.image.components.finetune.common.mlflow.common_utils import get_current_device
 from azureml.acft.image.components.finetune.mmdetection.common.trainer_classes import (
     DetectionTrainer,
 )
+from azureml.acft.image.components.finetune.mmdetection.common.constants import (
+    MmDetectionModelLiterals
+)
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MmDetectionDatasetLiterals
+
+from azureml.acft.image.components.model_selector.constants import MMDSupportedTasks
+from azureml.acft.common_components.model_selector.constants import (
+    ModelSelectorConstants
+)
 
 logger = get_logger_app(__name__)
 
+MMDTaskMap = {
+    MMDSupportedTasks.OBJECT_DETECTION: Tasks.MM_OBJECT_DETECTION,
+    MMDSupportedTasks.INSTANCE_SEGMENTATION: Tasks.MM_INSTANCE_SEGMENTATION,
+}
+
 
 class TrainerClasses:
     """Trainer classes."""
     def __init__(
         self,
         model_family: MODEL_FAMILY_CLS,
         model_name_or_path: Union[str, os.PathLike],
         task_name: Tasks,
+        model_metadata: dict = {},
     ) -> None:
         """
         :param model_family: related model_family to which current task belongs
         :type model_family: azureml.acft.accelerator.mappings.MODEL_FAMILY_CLS
         :param model_name_or_path: Hugging face image model name or path
         :type model_name_or_path: Union[str, os.PathLike]
         :param task_name: related task_name
         :type task_name: azureml.acft.accelerator.constants.task_definitions.Tasks
+        :param model_metafile_path: path to model metadata file
+        :type model_metafile_path: str
         """
         self.model_family = model_family
         self.task_name = task_name
         self.model_name_or_path = model_name_or_path
-        # self.model_type = TrainerClasses.get_hf_model_type(self.model_name_or_path)
+        self.model_metadata = model_metadata
+        self._is_finetuning_supported()
 
     def get_trainer_classes_mapping(self):
         """get trainer class based on task_name"""
         if self.task_name in [
             Tasks.MM_OBJECT_DETECTION,
             Tasks.MM_INSTANCE_SEGMENTATION,
         ]:
             return DetectionTrainer
         else:
             raise ACFTValidationException._with_error(
                 AzureMLError.create(TaskNotSupported,
                                     TaskName=self.task_name))
+
+    def _is_finetuning_supported(self):
+        """check if model is supported for current task"""
+
+        model_tasks = [MMDTaskMap[task.lower()] for task in
+                       self.model_metadata[ModelSelectorConstants.FINETUNING_TASKS]]
+        model_name = self.model_name_or_path.split("/")[-1][:-3]
+
+        # raise if selected task is not in model tasks
+        if self.task_name not in model_tasks:
+            error_str = f"Model {self.model_name_or_path} is not compatible with task {self.task_name}. "\
+                        f"Provided Model supports these tasks: {model_tasks}."
+            logger.error(error_str)
+
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ModelIncompatibleWithTask,
+                                    pii_safe_message=error_str,
+                                    ModelName=model_name,
+                                    TaskName=self.task_name))
+
+        try:
+            config = Config.fromfile(self.model_name_or_path)
+        except Exception as e:
+            error_str = f"Error while reading config file for model {model_name}."
+            logger.error(error_str + f"Error: {e}")
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_str))
+
+        teacher_config = config.model.get(MmDetectionModelLiterals.TEACHER_CONFIG)
+        if teacher_config:
+            error_str = "Teacher models are not yet supported for image finetuning tasks "
+            logger.error(error_str)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(NotSupported,
+                                    ModelName=model_name,
+                                    scenario_name=error_str))
+        try:
+            model = init_detector(config, device=get_current_device())
+        except Exception as e:
+            error_str = f"Error while initializing model {model_name}. {e}"
+            logger.error(error_str)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError,
+                                    error=error_str))
+        # semantic segmentation is not yet supported.
+        with_semantic = hasattr(model, MmDetectionModelLiterals.ROI_HEAD)\
+            and hasattr(model.roi_head, MmDetectionModelLiterals.WITH_SEMANTIC)\
+            and model.roi_head.with_semantic
+        with_panoptic = (hasattr(model, MmDetectionModelLiterals.WITH_SEMANTIC) and model.with_semantic)\
+            and (hasattr(model, MmDetectionModelLiterals.PANOPTIC_HEAD))
+        if with_semantic or with_panoptic:
+            error_str = f"Model-{model_name} with semantic/panoptic segmentation is not yet supported"\
+                        "for image finetuning tasks."
+            logger.error(error_str)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_str))
+
+        # Models like fast rcnn needs a proposal file to be sent along since it doesn't
+        # have a rpn network. They are currently not supported for finetuning.
+        if isinstance(model, TwoStageDetector) and \
+           hasattr(model, MmDetectionModelLiterals.WITH_RPN) and not model.with_rpn:
+            error_str = "Two-stage models without rpn are not yet supported."\
+                        f"please select other models from {ModelRepositoryURLs.MMDETECTION} for finetuning."
+            logger.error(error_str)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_str))
+
+        return
```

## azureml/acft/image/components/finetune/mmdetection/common/constants.py

```diff
@@ -1,25 +1,34 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """File for adding all the constants required for MMDetection."""
 
 
-class MmDetectionDatasetLiterals:
-    """Constants for MMDetection dataset."""
-    IMG = "img"
-    IMG_METAS = "img_metas"
-    GT_BBOXES = 'gt_bboxes'
-    GT_LABELS = 'gt_labels'
-    GT_CROWDS = 'gt_crowds'
-    GT_MASKS = "gt_masks"
-    MASKS = "masks"
-    BBOXES = "bboxes"
-    LABELS = "labels"
-    IMAGE_ORIGINAL_SHAPE = "ori_shape"
-
-
 class MmDetectionConfigLiterals:
     """Constants for MMDetection config."""
     NUM_CLASSES = "num_classes"
     BOX_SCORE_THRESHOLD = "score_thr"
+    IOU_THRESHOLD = "iou_threshold"
+    TRAIN_PIPELINE = "train_pipeline"
+    TEST_PIPELINE = "test_pipeline"
+    COLLECT = "Collect"
+    TYPE = "type"
+    KEYS = "keys"
+    CLASSES = "CLASSES"
+    META = "meta"
+    STATE_DICT = "state_dict"
+    MODEL = "model"
+
+
+class MmDetectionModelLiterals:
+    """Constants for MMDetection model."""
+    WITH_SEMANTIC = "with_semantic"
+    WITH_RPN = "with_rpn"
+    ROI_HEAD = "roi_head"
+    PANOPTIC_HEAD = "panoptic_head"
+    TEACHER_CONFIG = "teacher_config"
+    LANG_MODEL_NAME = "lang_model_name"
+    BBOX_HEAD = "bbox_head"
+    LOSS_CLS = "loss_cls"
+    CLASS_WEIGHT = "class_weight"
```

## azureml/acft/image/components/finetune/mmdetection/common/data_class.py

```diff
@@ -19,27 +19,26 @@
 from azureml.acft.image.components.finetune.common.constants.augmentation_constants import (
     AugmentationConfigFileNames,
 )
 from azureml.acft.image.components.finetune.common.constants.constants import (
     SettingLiterals, SettingParameters
 )
 from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
-from azureml.acft.image.components.finetune.mmdetection.common.constants import (
-    MmDetectionDatasetLiterals,
-)
 from azureml.acft.image.components.finetune.mmdetection.common.dataset import (
     MmObjectDetectionDataset
 )
 from azureml.acft.image.components.finetune.common.data.runtime_detection_dataset_adapter import (
     get_object_detection_dataset
 )
 from azureml.acft.image.components.finetune.interfaces.azml_interface import AzmlDataInterface
 
 from azureml.acft.image.components.finetune.mmdetection.common.model import DetectionConfigBuilder
-
+from azureml.acft.image.components.finetune.common.mlflow.mmdet_utils import make_batch
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MmDetectionDatasetLiterals
+from azureml.acft.image.components.finetune.common.data.data_utils import filter_invalid_images
 logger = get_logger_app(__name__)
 
 
 class AzmlMMDImageDataClass(AzmlDataInterface):
     """Data Class for MMDetection Image Models"""
 
     def __init__(self, tokenizer=None, **kwargs) -> None:
@@ -76,15 +75,15 @@
         :param type: str
 
         :return: MMdetcetion model configuration related to dataset preprocessing
                  such as transformations to apply.
         :rtype: Dict
         """
         config = DetectionConfigBuilder(model_name_or_path).build()
-        return config.data
+        return config
 
     def _get_train_valid_augmentation_transforms(
         self, **kwargs
     ) -> Tuple[Optional[Callable], Optional[Callable]]:
         """Get train and/or validation transforms
 
         :return: A tuple with train and validation transform
@@ -148,22 +147,14 @@
 
         # set train transform
         self.train_ds.set_transform(transform=train_transform)
         if self.validation_ds:
             # set valid transform
             self.validation_ds.set_transform(transform=valid_transform)
 
-        # log the augmented image size
-        train_image_shape = self.train_ds[0][MmDetectionDatasetLiterals.IMG].shape
-        logger.info(f"Augmented train image shape: {train_image_shape}")
-
-        if self.validation_ds:
-            valid_image_shape = self.validation_ds[0][MmDetectionDatasetLiterals.IMG].shape
-            logger.info(f"Augmented validation image shape: {valid_image_shape}")
-
     def _set_classes_metadata(self) -> None:
         """copy the label mappings from train_dataset"""
         dataset = self.train_ds.dataset
         self.label2id = {c: dataset.label_to_index_map(c) for c in dataset.classes}
         self.id2label = {v: k for k, v in self.label2id.items()}
 
     def get_train_dataset(self) -> MmObjectDetectionDataset:
@@ -178,60 +169,60 @@
         """get validation dataset
 
         :return : validation dataset
         :rtype: MmObjectDetectionDataset
         """
         return self.validation_ds
 
-    def get_collation_function(
-        self,
-    ) -> Callable[[List[Dict[str, Dict]]], Dict[str, Dict]]:
+    def object_detection_collate_func(self, examples: List[Dict[str, Dict]]) -> Dict[str, Dict]:
         """
-        collate function for MMDetection Object Detection/Instace Segmentation
+        Collate function for MMDetection Object Detection/Instance Segmentation.
 
-        return: callable function
-        rtype: Callable[[List[Dict[str, Dict]]], Dict[str, Dict]]
-        """
+        :param examples: A list of dictionaries containing example data.
+        :type examples: List[Dict[str, Dict]]
+
+        :return: A dictionary containing batched data.
+        :rtype: Dict[str, Dict]
+        """
+        # Filter out invalid examples
+        valid_examples = filter_invalid_images(examples, MmDetectionDatasetLiterals.IMG)
+
+        batched_images = make_batch([example[MmDetectionDatasetLiterals.IMG] for example in valid_examples])
+        img_metas = [example[MmDetectionDatasetLiterals.IMG_METAS] for example in valid_examples]
+        gt_bboxes = [example[MmDetectionDatasetLiterals.GT_BBOXES] for example in valid_examples]
+        gt_labels = [example[MmDetectionDatasetLiterals.GT_LABELS] for example in valid_examples]
+        gt_crowds = [example[MmDetectionDatasetLiterals.GT_CROWDS] for example in valid_examples]
+        original_gtbboxes = [example[MmDetectionDatasetLiterals.ORIGINAL_GT_BBOXES] for example in valid_examples]
+        # dummy_labels are added since hf_trainer expects same size tensors in
+        # distributed gather step in evaluation loop
+        dummy_labels = [torch.tensor(1)] * len(gt_labels)
+        output = {
+            MmDetectionDatasetLiterals.IMG: batched_images,
+            MmDetectionDatasetLiterals.IMG_METAS: img_metas,
+            MmDetectionDatasetLiterals.GT_BBOXES: gt_bboxes,
+            MmDetectionDatasetLiterals.GT_LABELS: gt_labels,
+            MmDetectionDatasetLiterals.GT_CROWDS: gt_crowds,
+            MmDetectionDatasetLiterals.DUMMY_LABELS: dummy_labels,
+            MmDetectionDatasetLiterals.ORIGINAL_GT_BBOXES: original_gtbboxes
+        }
 
-        def object_detection_collate_func(
-            examples: List[Dict[str, Dict]]
-        ) -> Dict[str, Dict]:
-
-            # Filter out invalid examples
-            valid_examples = [example for example in examples if example is not None]
-            if len(valid_examples) != len(examples):
-                if len(valid_examples) == 0:
-                    raise ACFTDataException._with_error(
-                        AzureMLError.create(ACFTUserError,
-                                            pii_safe_message="All images in the current batch are invalid.")
-                    )
-                else:
-                    num_invalid_examples = len(examples) - len(valid_examples)
-                    logger.info(f"{num_invalid_examples} invalid images found.")
-                    logger.info("Replacing invalid images with randomly selected valid images from the current batch")
-                    new_example_indices = np.random.choice(np.arange(len(valid_examples)), num_invalid_examples)
-                    for ind in new_example_indices:
-                        # Padding the batch with valid examples
-                        valid_examples.append(valid_examples[ind])
-
-            pixel_values = torch.stack([example[MmDetectionDatasetLiterals.IMG].to(torch.float) for example in
-                                       valid_examples])
-            # pixel_values = [example[MmDetectionDatasetLiterals.IMG].to(torch.float) for example in valid_examples]
-            img_metas = [example[MmDetectionDatasetLiterals.IMG_METAS] for example in valid_examples]
-            gt_bboxes = [example[MmDetectionDatasetLiterals.GT_BBOXES] for example in valid_examples]
-            gt_labels = [example[MmDetectionDatasetLiterals.GT_LABELS] for example in valid_examples]
-            gt_crowds = [example[MmDetectionDatasetLiterals.GT_CROWDS] for example in valid_examples]
+        if self.masks_required:
+            gt_masks = [example[MmDetectionDatasetLiterals.GT_MASKS] for example in valid_examples]
+            original_gtmasks = [example[MmDetectionDatasetLiterals.ORIGINAL_GT_MASKS] for example in valid_examples]
             output = {
-                MmDetectionDatasetLiterals.IMG: pixel_values,
-                MmDetectionDatasetLiterals.IMG_METAS: img_metas,
-                MmDetectionDatasetLiterals.GT_BBOXES: gt_bboxes,
-                MmDetectionDatasetLiterals.GT_LABELS: gt_labels,
-                MmDetectionDatasetLiterals.GT_CROWDS: gt_crowds
+                **output,
+                MmDetectionDatasetLiterals.GT_MASKS: gt_masks,
+                MmDetectionDatasetLiterals.ORIGINAL_GT_MASKS: original_gtmasks
             }
 
-            if self.masks_required:
-                gt_masks = [example[MmDetectionDatasetLiterals.GT_MASKS] for example in valid_examples]
-                output = {**output, MmDetectionDatasetLiterals.GT_MASKS: gt_masks}
+        return output
 
-            return output
+    def get_collation_function(
+        self,
+    ) -> Callable[[List[Dict[str, Dict]]], Dict[str, Dict]]:
+        """
+        Get the collate function for MMDetection Object Detection/Instance Segmentation.
 
-        return object_detection_collate_func
+        :return: A callable collate function.
+        :rtype: Callable[[List[Dict[str, Dict]]], Dict[str, Dict]]
+        """
+        return self.object_detection_collate_func
```

## azureml/acft/image/components/finetune/mmdetection/common/dataset.py

```diff
@@ -20,37 +20,44 @@
 
 import torch
 import numpy as np
 import albumentations
 
 from PIL.Image import Image
 from dataclasses import asdict
-from mmdet.core.mask import BitmapMasks
+try:
+    # mmdet version 3.x
+    from mmdet.structures.mask import BitmapMasks
+except ImportError:
+    # mmdet version 2.x
+    # temp hack to solve version discrepency in mmdet package
+    from mmdet.core.mask import BitmapMasks
 from typing import Union, Dict, Any, Callable, Tuple, Optional, List
-
+from azureml.acft.common_components import get_logger_app
 from azureml.acft.image.components.finetune.common.constants.augmentation_constants import (
     AlbumentationParamNames,
 )
 from azureml.acft.image.components.finetune.common.mlflow.common_constants import (
     AlbumentationParameterNames
 )
 from azureml.acft.image.components.finetune.common.constants.constants import (
     DetectionDatasetLiterals,
     ImageDataItemLiterals
 )
 from azureml.acft.image.components.finetune.common.data.runtime_detection_dataset_adapter import (
     RuntimeDetectionDatasetAdapter,
 )
-from azureml.acft.image.components.finetune.mmdetection.common.constants import (
-    MmDetectionDatasetLiterals,
-)
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MmDetectionDatasetLiterals
+
 from azureml.acft.image.components.finetune.mmdetection.common.image_metadata import (
     ImageMetadata,
 )
 
+logger = get_logger_app(__name__)
+
 
 class MmObjectDetectionDataset(RuntimeDetectionDatasetAdapter):
     """ Dataset for Object Detection Models from MMDetection """
 
     SUPPORTED_TRANSFORM_LIB_NAME_MAPPING = {
         albumentations.core.composition.Compose: AlbumentationParamNames.LIB_NAME
     }
@@ -64,30 +71,52 @@
         :rtype: dict, None
         """
         image, training_labels, image_info = super(
             MmObjectDetectionDataset, self
         ).__getitem__(index)
 
         if image is None:
+            logger.info("Image was not found for a data point in the batch, the data point is marked as invalid.")
+            return None
+
+        if training_labels[DetectionDatasetLiterals.BOXES].shape[0] == 0:
+            # empty training labels tensor
+            logger.info(
+                "Bounding boxes were not found for a data point in the batch, the data point is marked as invalid."
+            )
             return None
 
         gtbboxes = training_labels[DetectionDatasetLiterals.BOXES]
+        original_gtbboxes = gtbboxes.clone()
         gtlabels = training_labels[DetectionDatasetLiterals.LABELS]
         gtmasks = [mask for mask in training_labels[DetectionDatasetLiterals.MASKS].numpy()] \
             if DetectionDatasetLiterals.MASKS in training_labels else None
+        original_gtmasks = gtmasks or None
+        c, h, w = image.shape
+        ori_shape = (h, w, c)
+        resized_image_height, resized_image_width = ori_shape[0], ori_shape[1]
         # Convert np.ndarray to List[np.ndarray] since albumentation expects list[np.ndarray]
         if hasattr(self, DetectionDatasetLiterals.TRANSFORM) and self.transform is not None:
             transformed = self._apply_transform(
                 # Move channel to last dimension. i.e. (C,H,W) to (H,W,C)
                 image=image.numpy().transpose(1, 2, 0),
                 bboxes=gtbboxes,
                 labels=gtlabels,
                 masks=gtmasks
             )
             image = transformed[ImageDataItemLiterals.ALBUMENTATIONS_IMAGE_KEY]
+            # The transformed image is first resized(using constraint resize) and then padded to make divisible by
+            # stride(32 by default).
+            # The resized_width and resized_height is the image size after resizing(before padding).
+            resized_image_width = transformed[AlbumentationParameterNames.IMAGE_METADATA][
+                AlbumentationParameterNames.RESIZED_WIDTH
+            ]
+            resized_image_height = transformed[AlbumentationParameterNames.IMAGE_METADATA][
+                AlbumentationParameterNames.RESIZED_HEIGHT
+            ]
             if isinstance(image, np.ndarray):
                 # Move channel to first dimension. i.e. (H,W,C) to (C,H,W)
                 image = torch.from_numpy(image.transpose(2, 0, 1))
 
             gtbboxes = transformed[ImageDataItemLiterals.ALBUMENTATIONS_BBOXES_KEY]
             if not torch.is_tensor(gtbboxes):
                 gtbboxes = torch.as_tensor(gtbboxes, dtype=torch.float32)
@@ -95,34 +124,43 @@
             if not torch.is_tensor(gtlabels):
                 gtlabels = torch.as_tensor(gtlabels, dtype=torch.long)
             gtmasks = transformed[DetectionDatasetLiterals.MASKS]
 
         channels, height, width = image.shape
 
         img_metas = ImageMetadata(ori_shape=(height, width, channels),
+                                  img_shape=(resized_image_height, resized_image_width),
                                   filename=image_info[DetectionDatasetLiterals.IMAGEFILENAME],
-                                  ori_filename=image_info[DetectionDatasetLiterals.IMAGEFILENAME])
+                                  ori_filename=image_info[DetectionDatasetLiterals.IMAGEFILENAME],
+                                  raw_dimensions=ori_shape)
 
         example = {
             MmDetectionDatasetLiterals.IMG: image,
             MmDetectionDatasetLiterals.IMG_METAS: asdict(img_metas),
             MmDetectionDatasetLiterals.GT_BBOXES: gtbboxes,
             MmDetectionDatasetLiterals.GT_LABELS: gtlabels,
             MmDetectionDatasetLiterals.GT_CROWDS: torch.tensor(
                 [bool(is_crowd) for is_crowd in image_info[DetectionDatasetLiterals.ISCROWD]]
             ),
+            # Untransformed ground truth bounding boxes. Used for validation metrics calculation.
+            MmDetectionDatasetLiterals.ORIGINAL_GT_BBOXES: original_gtbboxes
         }
 
         if DetectionDatasetLiterals.MASKS in training_labels:
             masks = BitmapMasks(
                 gtmasks,
                 height=height,
                 width=width,
             )
             example[MmDetectionDatasetLiterals.GT_MASKS] = masks
+            example[MmDetectionDatasetLiterals.ORIGINAL_GT_MASKS] = BitmapMasks(
+                original_gtmasks,
+                height=ori_shape[0],
+                width=ori_shape[1],
+            )
 
         return example
 
     def _apply_transform(self,
                          image: np.ndarray,
                          bboxes: torch.Tensor,
                          labels, masks: torch.Tensor = None) -> \
@@ -203,8 +241,8 @@
         :param masks: List of mask if present
         :type labels: Optional[List[torch.Tensor]]
 
         :return: A dictonary containing the transformed image, transformed bbox, transformed mask and
         transformed labels.
         :rtype: Dict[str, Any]
         """
-        return self.transform(image=image, bboxes=bboxes, class_labels=labels, masks=masks)
+        return self.transform(image=image, bboxes=bboxes, class_labels=labels, masks=masks, image_metadata=dict())
```

## azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py

```diff
@@ -9,20 +9,26 @@
 
 
 @dataclass
 class ImageMetadata:
     """ Dataclass for maintaining the metadata dictionary as required for MM detection models.
     The keys of metadata dictionary is same as the property name."""
 
-    ori_shape: Tuple[int, int, int]
-    img_shape: Tuple[int, int, int] = None
-    pad_shape: Tuple[int, int, int] = None
-    scale_factor: np.ndarray = np.array([1, 1, 1, 1])
+    ori_shape: Tuple[int, int, int]         # Dimension of the transformed image H x W x C. This is the shape of the
+    # image after resizing and padding. If we set it to the original image shape i.e. shape before transformation
+    # then the MMD model is not able to learn and the eval_mAP is always 0.0.
+    img_shape: Tuple[int, int, int] = None  # Dimension of the image after ConstraintResize transformation.
+    pad_shape: Tuple[int, int, int] = None  # Dimension of the tranformed image after padding. Please note that padding
+    # is applied after ConstraintResize transformation, so pad_shape is always greater than or equal to img_shape.
+    raw_dimensions: Tuple[int, int] = None   # Dimension of the raw image H x W. This is used to resize the predicted
+    # mask to the original image size.
+    scale_factor: np.ndarray = np.array([1, 1])
     flip: bool = False
     flip_direction: str = None
     filename: str = None
     ori_filename: str = None
+    border: Tuple[int, int, int, int] = (0, 0, 0, 0)
 
     def __post_init__(self):
         """If image shape after resizing and padding is not provided then assign it with original shape"""
-        self.img_shape = self.ori_shape or self.img_shape
-        self.pad_shape = self.ori_shape or self.pad_shape
+        self.img_shape = self.img_shape or self.ori_shape
+        self.pad_shape = self.pad_shape or self.ori_shape
```

## azureml/acft/image/components/finetune/mmdetection/common/inference.py

```diff
@@ -21,49 +21,45 @@
 from typing import Dict, Any
 from transformers import (
     TrainerCallback,
     TrainingArguments,
     TrainerState,
     TrainerControl,
 )
-
+from mmengine import MessageHub
 from azureml.acft.image.components.finetune.common.constants.constants import (
     SettingLiterals,
 )
 from azureml.acft.image.components.finetune.interfaces.azml_interface import (
     AzmlInferenceInterface,
 )
 
 
 class DetectionInference(AzmlInferenceInterface):
     """Inference class for MMDetection image OD and IS tasks"""
+
     def __init__(self, params: Dict[str, Any]) -> None:
         """
         :param params: parameters used for inference
         :type params: dict
         :param trainer_classes_cls: trainer interface class
         :type trainer_classes_cls: AzmlTrainerClassesInterface
         """
         self.inference_params = params
 
     # other required methods to be implemented as part of mlflow_save task.
 
 
 class SaveMlflowModel(TrainerCallback):
     """MMDetection image OD and IS save mlflow model callback."""
+
     # finetune-core has implemented save mlflow model directly in the driver without an interface and
     # they are using mlflow.hftransformers flavor. Till the interface is exposed we can have a TrainerCallback
     # on_train_end and save the mlflow model
-    def on_train_end(
-        self,
-        args: TrainingArguments,
-        state: TrainerState,
-        control: TrainerControl,
-        **kwargs
-    ) -> None:
+    def on_train_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
         """Callback called at the end of training.
         :param args: training arguments
         :type args: TrainingArguments (transformers.TrainingArguments)
         :param state: trainer state
         :type state: TrainerState (transformers.TrainerState)
         :param control: trainer control
         :type control: TrainerControl (transformers.TrainerControl)
@@ -73,7 +69,32 @@
         :return: None
         :rtype: None
         """
         if not getattr(args, SettingLiterals.SAVE_AS_MLFLOW_MODEL, False):
             return
 
         raise NotImplementedError()
+
+
+class MMDetectionMessageHubUpdateCallback(TrainerCallback):
+    """MMDetection image OD and IS message hub update callback class."""
+
+    # messagehub for MMD is not available in finetune-core. This is a placeholder to update the epoch
+    # information in the messagehub. Please add any other training details in MessageHub as needed.
+    def on_epoch_begin(self, args, state, control, **kwargs) -> None:
+        """Callback called at the beginning of each epoch.
+        :param args: training arguments
+        :type args: TrainingArguments (transformers.TrainingArguments)
+        :param state: trainer state
+        :type state: TrainerState (transformers.TrainerState)
+        :param control: trainer control
+        :type control: TrainerControl (transformers.TrainerControl)
+        :param kwargs: additional arguments
+        :type kwargs: dict
+
+        :return: None
+        :rtype: None
+        """
+        # Get the current instance of MessageHub
+        message_hub = MessageHub.get_current_instance()
+        # Update the epoch information in MessageHub
+        message_hub.update_info("epoch", state.epoch)
```

## azureml/acft/image/components/finetune/mmdetection/common/metrics.py

```diff
@@ -14,229 +14,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """MMDetection image OD and IS evaluation related functions."""
 
-import numpy as np
-import torch
-
 from transformers import EvalPrediction
-from typing import Dict, List, Tuple
-
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
-from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
-from azureml.acft.image.components.finetune.common.constants.constants import (
-    SettingLiterals,
-    InferenceParameters,
-)
-from azureml.acft.image.components.finetune.common import masktools
-from azureml.acft.image.components.finetune.mmdetection.common.constants import (
-    MmDetectionDatasetLiterals,
-)
-from azureml.acft.image.components.finetune.mmdetection.object_detection.model_wrapper import (
-    ObjectDetectionModelWrapper as od_model_wrapper,
-)
-from azureml.acft.image.components.finetune.mmdetection.instance_segmentation.model_wrapper import (
-    InstanceSegmentationModelWrapper as is_model_wrapper,
-)
-from azureml.metrics import compute_metrics
-from azureml.metrics import list_metrics
-from azureml.metrics.constants import Tasks as MetricsTasks
-
-# TODO Compute metrics package is yet to define constants for literals like "boxes", "metrics" which are
-#  used in this file. Replace these with constants from metrics package when it'll be available.
-
-
-def _get_valid_index(
-    labels: np.ndarray, box_scores: np.ndarray = None, box_score_threshold: float = None
-) -> List:
-    """
-    Get the index of valid labels i.e, id >= 0 and box score above box score threshold
-    :param labels: classification labels of image
-    :param labels: nd-array
-    :param box_scores: Optional, prediction score of bounding box
-    :param box_scores: nd-array
-    :param box_score_threshold: Optional, box score threshold
-    :param box_score_threshold: float
-    :return: index of valid labels
-    :rtype: List
-
-    Note: This helper function is used for preparing the model output and ground truth labels before
-    feeding to compute_metrics. (It returns the valid indices of predictions, we then filtered out the invalid labels,
-    bbox and masks).
-    1. For prediction, It will only keep those indices which satisfy the following 2 conditions:
-        1.1 label id >= 0 (basically, remove the padding that we intentially added for HF trainer.)
-        1.2 the box scoring confidence >= box score threshold
-        i.e., lbl >=0 and box_scores[index] >= box_score_threshold
-    2. For ground truth, we don't have the box score. Hence, we only remove the padding.
-    i.e., lbl >=0 and box_score is None
-    """
-    valid_index = []
-    for index, lbl in enumerate(labels):
-        if lbl >= 0 and (
-            box_scores is None or box_scores[index] >= box_score_threshold
-        ):
-            valid_index.append(index)
-    return valid_index
-
-
-def _convert_masks_to_rle(masks: np.ndarray) -> List[Dict]:
-    """
-    Convert masks to rle as required by metrics functions
-    :param masks: Binary masks
-    :type masks: np.ndarray
-    :return: List of masks in rle format
-    :rtype: List of rle dict
-    """
-    rle_mask = list()
-    for mask in masks:
-        rle_mask.append(masktools.encode_mask_as_rle(torch.tensor(mask)))
-    return rle_mask
-
-
-def _prepare_prediction_labels(
-    predictions: Tuple,
-    box_score_threshold: float,
-    output_keys_to_index_mapping: Dict[MmDetectionDatasetLiterals, int],
-) -> List[Dict[str, np.ndarray]]:
-    """
-    This function transforms the predictions from HF trainer as required by the metrics functions.
-    It also removes the padded (dummy) predictions added in model forward function.
-    :param predictions: model prediction containing bboxes, labels and masks
-    :type predictions: Tuple
-    :param box_score_threshold: threshold for bounding box score
-    :type box_score_threshold: float
-    :param output_keys_to_index_mapping: mapping of keys to index in prediction tuple
-    :type output_keys_to_index_mapping: dict
-    :return: Transformed predictions as required by metrics compute function
-    :rtype: List of prediction dictionary List[Dict[str, np.ndarray]]
-    """
-    batch_bboxes = predictions[
-        output_keys_to_index_mapping[MmDetectionDatasetLiterals.BBOXES]
-    ]
-    batch_labels = predictions[
-        output_keys_to_index_mapping[MmDetectionDatasetLiterals.LABELS]
-    ]
-
-    outputs: List[Dict] = list()
-    for index, (bboxes, labels) in enumerate(zip(batch_bboxes, batch_labels)):
-        keep_index = _get_valid_index(
-            labels, box_scores=bboxes[:, 4], box_score_threshold=box_score_threshold
-        )
-        output = {
-            "boxes": bboxes[keep_index][:, :4],
-            "classes": labels[keep_index],
-            "scores": bboxes[keep_index][:, 4],
-        }
-
-        # if len of prediction is greater than 5, then it will have mask information.
-        if len(predictions) > 5:
-            image_masks = predictions[
-                output_keys_to_index_mapping[MmDetectionDatasetLiterals.MASKS]
-            ][index]
-            valid_masks = image_masks[keep_index]
-            output["masks"] = _convert_masks_to_rle(valid_masks)
-
-        outputs.append(output)
-    return outputs
-
-
-def _prepare_ground_truth_labels(
-    ground_truths: Tuple,
-    output_keys_to_index_mapping: Dict[MmDetectionDatasetLiterals, int],
-) -> Tuple[List[Dict], List[Dict]]:
-    """
-    This function transforms the ground truth labels as required by the metrics functions.
-    It also removes the padded (dummy) labels added in model forward function.
-    :param ground_truths: Ground truth labels
-    :type ground_truths: Tuple of ground truth
-    :param output_keys_to_index_mapping: mapping of keys to index in prediction tuple
-    :type output_keys_to_index_mapping: dict
-    :return: Dictionaries of transformed ground truth and image_metadata
-    :rtype: Tuple of Lists having gt and metadata dictionaries
-    """
-    batch_gt_bboxes = ground_truths[
-        output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_BBOXES]
-    ]
-    batch_gt_labels = ground_truths[
-        output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_LABELS]
-    ]
-    batch_gt_crowds = ground_truths[
-        output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_CROWDS]
-    ]
-
-    gts: List[Dict] = list()
-    meta_infos: List[Dict] = list()
-    for index, (gt_bboxes, gt_labels, gt_crowds) in enumerate(
-        zip(batch_gt_bboxes, batch_gt_labels, batch_gt_crowds)
-    ):
-        keep_index = _get_valid_index(gt_labels)
-
-        ground_truth = {
-            "boxes": gt_bboxes[keep_index],
-            "classes": gt_labels[keep_index],
-        }
-
-        if len(ground_truths) > 5:
-            gt_image_masks = ground_truths[
-                output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_MASKS]
-            ][index]
-            gt_valid_masks = gt_image_masks[keep_index]
-            ground_truth["masks"] = _convert_masks_to_rle(gt_valid_masks)
-
-        image_metadata = {"iscrowd": gt_crowds[keep_index]}
-
-        gts.append(ground_truth)
-        meta_infos.append(image_metadata)
-    return gts, meta_infos
+from typing import Dict
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MetricsLiterals
 
 
 def calculate_detection_metrics(eval_prediction: EvalPrediction, **kwargs) -> Dict:
     """
-    compute and return metrics for Object Detection task
+    compute and return metrics for Object Detection or instance segmentation task
     :param eval_prediction: eval_prediction containing predictions and labels
     :type eval_prediction: Huggingface EvalPrediction
-    :param kwargs: A dictionary of additional configuration parameters.
+    :param kwargs: A dictionary of additional configuration parameters including the metric
+    computer method.
     :type kwargs: dict
     :return: Dictionary containing all metrics.
     :rtype: Dict
     """
-    num_classes = kwargs[SettingLiterals.NUM_LABELS]
-    task_name = kwargs[SettingLiterals.TASK_NAME]
-    box_score_threshold = kwargs.get(
-        SettingLiterals.BOX_SCORE_THRESHOLD,
-        InferenceParameters.DEFAULT_BOX_SCORE_THRESHOLD,
-    )
-    iou_threshold = kwargs.get(
-        SettingLiterals.IOU_THRESHOLD, InferenceParameters.DEFAULT_IOU_THRESHOLD
-    )
-
-    if task_name == Tasks.MM_INSTANCE_SEGMENTATION:
-        metrics_list = list_metrics(MetricsTasks.IMAGE_INSTANCE_SEGMENTATION)
-        task_type = MetricsTasks.IMAGE_INSTANCE_SEGMENTATION
-        model_output_keys_ordering = is_model_wrapper.MODEL_OUTPUT_KEY_ORDERING
-    else:
-        metrics_list = list_metrics(MetricsTasks.IMAGE_OBJECT_DETECTION)
-        task_type = MetricsTasks.IMAGE_OBJECT_DETECTION
-        model_output_keys_ordering = od_model_wrapper.MODEL_OUTPUT_KEY_ORDERING
-    output_keys_to_index_mapping = {
-        value: index for index, value in enumerate(model_output_keys_ordering)
-    }
-    predictions = _prepare_prediction_labels(
-        eval_prediction.predictions, box_score_threshold, output_keys_to_index_mapping
-    )
-    gts, img_meta_infos = _prepare_ground_truth_labels(
-        eval_prediction.predictions, output_keys_to_index_mapping
-    )
+    metrics_computer = kwargs[MetricsLiterals.METRICS_COMPUTER]
+    # Calculate metrics at the end of the epoch
+    metrics = metrics_computer.aggregate_compute()[MetricsLiterals.METRICS]
+    # Reset the metric computation after batch is over.
+    metrics_computer.reset()
 
-    metrics = compute_metrics(
-        task_type=task_type,
-        y_test=gts,
-        image_meta_info=img_meta_infos,
-        y_pred=predictions,
-        num_classes=num_classes,
-        iou_threshold=iou_threshold,
-        metrics=metrics_list,
-    )["metrics"]
     return metrics
```

## azureml/acft/image/components/finetune/mmdetection/common/model.py

```diff
@@ -15,131 +15,187 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """MMDetection model related classes."""
 
 from __future__ import annotations
+
+import torch
+
 from typing import Dict, Any, List
 
-from mmcv import Config
-from mmcv.runner import load_checkpoint
-from mmdet.models import build_detector
+try:
+    # mmcv-full under 2.0
+    from mmcv import Config
+except ImportError:
+    # mmcv version >= 2.0
+    from mmengine.config import Config
+from mmengine.runner import load_checkpoint
+from mmdet.apis import init_detector
 from torch import nn
 
+from azureml._common._error_definition.azureml_error import AzureMLError
+
 from azureml.acft.common_components import get_logger_app
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTSystemError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTSystemException
 from azureml.acft.image.components.finetune.common.constants.constants import (
     SettingLiterals,
     InferenceParameters,
 )
+from azureml.acft.image.components.finetune.common.mlflow.common_utils import (
+    get_current_device
+)
 from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
 from azureml.acft.image.components.finetune.mmdetection.common.constants import (
     MmDetectionConfigLiterals,
 )
 from azureml.acft.image.components.finetune.mmdetection.instance_segmentation.model_wrapper import (
     InstanceSegmentationModelWrapper,
 )
 from azureml.acft.image.components.finetune.mmdetection.object_detection.model_wrapper import (
     ObjectDetectionModelWrapper,
 )
 from azureml.acft.image.components.finetune.interfaces.azml_interface import (
     AzmlModelInterface,
 )
 from azureml.acft.image.components.model_selector.constants import ImageModelSelectorConstants
+from azureml.metrics.constants import Tasks as MetricsTasks
+
 
 logger = get_logger_app(__name__)
 
 
 class DetectionConfigBuilder:
     """ Builder class to build the MM Detection config."""
     def __init__(self, config_file_path):
         """ Builder class to build the MM Detection config.
         :param config_file_path: parameters used for inference
         :type config_file_path: str
         """
         self.config: Config = Config.fromfile(config_file_path)
+        self._flag = False  # Internal flag to track if model config is updated with key-val or not
 
-    @staticmethod
     def _find_key_and_set_value(
-        config: Dict, search_field: str, value: Any, stack: List
+            self, config: Dict, search_field: str, value: Any, stack: List
     ) -> None:
         """
         Recursively find the search field and update it with value in given config dictionary
         :param config: mm detection model configuration
         :type config: Dict
         :param search_field: field to update
         :type search_field: str
         :param value: value to update
         :type value: Any
         :param stack: The stack to maintain the path of the search field
         :type stack: List
         """
+        if not isinstance(config, Dict):
+            return
         for key in config:
             stack.append(key)
             if isinstance(config[key], dict):
-                DetectionConfigBuilder._find_key_and_set_value(
+                self._find_key_and_set_value(
                     config[key], search_field, value, stack
                 )
             elif isinstance(key, str) and key == search_field:
                 config[key] = value
+                self._flag = True
                 logger.info(f"Setting {value} at {'.'.join(stack)} in config.")
+            elif isinstance(config[key], list) or isinstance(config[key], tuple):
+                for item in config[key]:
+                    self._find_key_and_set_value(
+                        item, search_field, value, stack
+                    )
             stack.pop()
 
     def set_num_labels(self, num_labels: int) -> DetectionConfigBuilder:
         """
         Set number of labels/ classes in the model config
         :param num_labels: number of labels
         :type num_labels: int
         :return: config builder
         :rtype: DetectionConfigBuilder
         """
         if num_labels > 0:
+            self._flag = False
             self._find_key_and_set_value(
                 self.config.model,
                 MmDetectionConfigLiterals.NUM_CLASSES,
                 num_labels,
                 stack=["model"],
             )
+            if not self._flag:
+                raise ACFTSystemException._with_error(
+                    AzureMLError.create(ACFTSystemError, pii_safe_message="Number of labels are not updated in model"
+                                                                          "config")
+                )
         return self
 
-    def set_box_scoring_threshold(
-        self, box_score_threshold: float
+    def set_box_scoring_or_iou_threshold(
+            self, threshold: float, is_iou_threshold: bool = False
     ) -> DetectionConfigBuilder:
         """
-        Set box scoring threshold in the model config
-        :param box_score_threshold: threshold for bounding box score
-        :type box_score_threshold: float
+        Set threshold in the model config
+        :param threshold: threshold for bounding box score or iou_threshols
+        :type threshold: float
+        :param is_iou_threshold: flag to indicate if threshold is iou threshold or not
+        :type is_iou_threshold: bool
         :return: config builder
         :rtype: DetectionConfigBuilder
         """
+        threshold_name = MmDetectionConfigLiterals.IOU_THRESHOLD if is_iou_threshold else \
+            MmDetectionConfigLiterals.BOX_SCORE_THRESHOLD
         try:
-            self._find_key_and_set_value(
-                self.config.model.test_cfg,
-                MmDetectionConfigLiterals.BOX_SCORE_THRESHOLD,
-                box_score_threshold,
-                stack=["model", "test_cfg"],
-            )
+            self._flag = False
+            # find and replace threshold in model.test_cfg.rcnn for two stage models
+            if "rcnn" in self.config.model.test_cfg:
+                self._find_key_and_set_value(
+                    self.config.model.test_cfg.rcnn,
+                    threshold_name,
+                    threshold,
+                    stack=["model", "test_cfg", "rcnn"],
+                )
+            else:
+                if "rpn" in self.config.model.test_cfg:
+                    error_str = "rpn should not be present, if rcnn is not present in config"
+                    logger.error(error_str)
+                    raise ACFTSystemException._with_error(
+                        AzureMLError.create(ACFTSystemError, pii_safe_message=error_str)
+                    )
+
+                # find and replace threshold in model.test_cfg for ssd models
+                self._find_key_and_set_value(
+                    self.config.model.test_cfg,
+                    threshold_name,
+                    threshold,
+                    stack=["model", "test_cfg"],
+                )
+            if not self._flag:
+                logger.warning("Box scoring threshold is not updated in model config.")
         except Exception as ex:
             logger.warning(
                 f"Exception {ex} when calling set_box_scoring_threshold. "
             )
-            # If test_cfg or score_threshold is not present in config, then this thresholding
+            # If test_cfg or score_threshold or iou_threshold is not present in config, then this thresholding
             # is handled while calculating the metrics.
         return self
 
     def build(self) -> Config:
         """ Return the built MM Detection config.
         :return: MM Detection config
         :rtype: MMCV Config
         """
         return self.config
 
 
 class DetectionModel(AzmlModelInterface):
     """MM Detection models."""
+
     def from_pretrained(self, model_name_or_path: str, **kwargs) -> nn.Module:
         """ Load the model config and weights if weight path specified.
         :param model_name_or_path: parameters used for inference
         :type model_name_or_path: str
         :param kwargs: A dictionary of additional configuration parameters.
         :type kwargs: dict
         :return: MM Detection model
@@ -149,33 +205,55 @@
         task_name = kwargs.get(SettingLiterals.TASK_NAME, Tasks.MM_OBJECT_DETECTION)
         num_labels = kwargs.get(SettingLiterals.NUM_LABELS, 0)
         box_score_threshold = kwargs.get(
             SettingLiterals.BOX_SCORE_THRESHOLD,
             InferenceParameters.DEFAULT_BOX_SCORE_THRESHOLD,
         )
 
+        iou_threshold = kwargs.get(SettingLiterals.IOU_THRESHOLD,
+                                   InferenceParameters.DEFAULT_IOU_THRESHOLD)
+
         config = (
             DetectionConfigBuilder(model_name_or_path)
             .set_num_labels(num_labels)
-            .set_box_scoring_threshold(box_score_threshold)
+            .set_box_scoring_or_iou_threshold(box_score_threshold, is_iou_threshold=False)
+            .set_box_scoring_or_iou_threshold(iou_threshold, is_iou_threshold=True)
             .build()
         )
 
         # copy the label2id mapping from kwargs to config. To be used in mlflow export
         config.id2label = kwargs.get(SettingLiterals.ID2LABEL, None)
         model_meta_file_path = kwargs.get(ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_PATH)
-        model = build_detector(config.model)
+        model = init_detector(config, model_weights_path, device=get_current_device())
         logger.info(f"Successfully loaded model config and with {num_labels} labels.")
-        if model_weights_path:
+        model_state_dict = torch.load(model_weights_path, map_location="cpu")
+        if 'state_dict' in model_state_dict:
+            model_state_dict = model_state_dict['state_dict']
+        # state_dict starts with model.* for the case of aml models.
+        # need to load the checkpint to wrapped model for the case of aml models.
+        load_after_wrapping = list(model_state_dict.keys())[0].startswith('model.')
+
+        if model_weights_path and not load_after_wrapping:
             load_checkpoint(model, model_weights_path)
             logger.info(f"Successfully loaded model weight from {model_weights_path}.")
 
         model_wrapper = None
         if task_name == Tasks.MM_OBJECT_DETECTION:
             model_wrapper = ObjectDetectionModelWrapper(
-                model, config, model_name_or_path, model_meta_file_path
+                model, config, model_name_or_path,
+                task_type=MetricsTasks.IMAGE_OBJECT_DETECTION,
+                num_labels=num_labels, box_score_threshold=box_score_threshold,
+                iou_threshold=iou_threshold,
+                meta_file_path=model_meta_file_path
             )
         elif task_name == Tasks.MM_INSTANCE_SEGMENTATION:
             model_wrapper = InstanceSegmentationModelWrapper(
-                model, config, model_name_or_path, model_meta_file_path
+                model, config, model_name_or_path,
+                task_type=MetricsTasks.IMAGE_INSTANCE_SEGMENTATION,
+                num_labels=num_labels, box_score_threshold=box_score_threshold,
+                iou_threshold=iou_threshold,
+                meta_file_path=model_meta_file_path
             )
+        if model_weights_path and load_after_wrapping:
+            load_checkpoint(model_wrapper, model_weights_path)
+            logger.info(f"Successfully loaded model weight from {model_weights_path}.")
         return model_wrapper
```

## azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py

```diff
@@ -1,27 +1,31 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """MMDetection trainer arguments"""
 
 from typing import Any, Dict
+from functools import partial
 
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.image.components.finetune.common.constants.constants import (
     SettingLiterals,
     SettingParameters,
 )
 
+from transformers.training_args import OptimizerNames
+from transformers import TrainingArguments
+from azureml.acft.accelerator.constants import HfTrainerMethodsConstants
 from azureml.acft.image.components.finetune.interfaces.azml_interface import (
     AzmlFinetuneInterface,
 )
-from azureml.acft.image.components.finetune.mmdetection.common.constants import (
-    MmDetectionDatasetLiterals,
-)
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MmDetectionDatasetLiterals
+from azureml.acft.image.components.finetune.defaults.constants import HFTrainerDefaultsKeys
+from azureml.acft.image.components.finetune.common.trainer.train_helper import get_custom_optimizer
 
 logger = get_logger_app(__name__)
 
 
 class DetectionTrainerArguments(AzmlFinetuneInterface):
     """MM Detection trainer arguments."""
     def __init__(self, params: Dict[str, Any]) -> None:
@@ -37,18 +41,32 @@
 
         :return: dictionary of custom args which are not supported by core
                  and needed for image models
         :rtype: Dict[str, Any]
         """
         custom_args_dict = {
             SettingLiterals.REMOVE_UNUSED_COLUMNS: SettingParameters.REMOVE_UNUSED_COLUMNS,
-            SettingLiterals.LABEL_NAMES: [MmDetectionDatasetLiterals.GT_LABELS],
+            # dummy_labels are added since hf_trainer expects same size tensors in
+            # distributed gather step in evaluation loop
+            SettingLiterals.LABEL_NAMES: [MmDetectionDatasetLiterals.DUMMY_LABELS],
         }
+
+        if hasattr(TrainingArguments, HFTrainerDefaultsKeys.SAVE_SAFETENSORS):
+            custom_args_dict[HFTrainerDefaultsKeys.SAVE_SAFETENSORS] = False
+
         return custom_args_dict
 
     def get_custom_trainer_functions(self) -> Dict[str, Any]:
         """Customizable methods for trainer class
 
         :return: dictionary of custom trainer methods needed for image models
         :rtype: Dict[str, Any]
         """
+        if self.params.get(SettingLiterals.OPTIMIZER, None) == OptimizerNames.SGD \
+           and self.params.get(SettingLiterals.EXTRA_OPTIMIZER_ARGS, None):
+            sgd_optimizer = partial(get_custom_optimizer,
+                                    optimizer_name=self.params[SettingLiterals.OPTIMIZER],
+                                    extra_optim_args=self.params[SettingLiterals.EXTRA_OPTIMIZER_ARGS],
+                                    weight_decay=self.params.get(SettingLiterals.WEIGHT_DECAY, 0.0))
+
+            return {HfTrainerMethodsConstants.AZUREML_OPTIMIZER: sgd_optimizer}
         return {}
```

## azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py

```diff
@@ -9,14 +9,15 @@
 from azureml.acft.image.components.finetune.interfaces.azml_interface import (
     AzmlTrainerClassesInterface,
 )
 from azureml.acft.image.components.finetune.mmdetection.common.data_class import AzmlMMDImageDataClass
 from azureml.acft.image.components.finetune.mmdetection.common.inference import (
     SaveMlflowModel,
     DetectionInference,
+    MMDetectionMessageHubUpdateCallback,
 )
 from azureml.acft.image.components.finetune.mmdetection.common.model import (
     DetectionModel,
     DetectionConfigBuilder,
 )
 from azureml.acft.image.components.finetune.mmdetection.common.trainer_arguments import (
     DetectionTrainerArguments,
@@ -36,10 +37,10 @@
         self.dataset_cls = AzmlMMDImageDataClass
         # MMDetection framework don't have tokenizer. Preprocessing is handled in augmentation.
         self.tokenizer_cls = None
         self.model_cls = DetectionModel
 
         self.finetune_cls = DetectionTrainerArguments
         self.config_cls = DetectionConfigBuilder
-        self.callbacks = [SaveMlflowModel]
+        self.callbacks = [SaveMlflowModel, MMDetectionMessageHubUpdateCallback]
         self.metrics_function = calculate_detection_metrics
         self.inference_cls = DetectionInference
```

## azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py

```diff
@@ -18,160 +18,201 @@
 
 """MMdetection instance segmentation model wrapper class."""
 
 import mmcv
 import numpy as np
 import torch
 
-from mmcv import Config
+from mmengine.config import Config
+try:
+    # mmdet version 3.x
+    from mmdet.structures import DetDataSample
+    from mmdet.structures.mask import BitmapMasks
+except ImportError:
+    # mmdet version 2.x
+    from mmdet.core.mask import BitmapMasks
+    DetDataSample = None
 from torch import nn, Tensor
-from typing import List, Dict, Tuple
+from typing import List, Dict, Tuple, Union
 
-from azureml.acft.image.components.finetune.common.utils import get_current_device
-from azureml.acft.image.components.finetune.mmdetection.common.constants import (
-    MmDetectionDatasetLiterals,
+from azureml.acft.image.components.finetune.common import masktools
+from azureml.acft.image.components.finetune.common.constants.constants import DetectionDatasetLiterals
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import (
+    MetricsLiterals,
+    MmDetectionDatasetLiterals
 )
+from azureml.acft.image.components.finetune.common.mlflow.mmdet_utils import resize_masks
 from azureml.acft.image.components.finetune.mmdetection.object_detection.model_wrapper import (
     ObjectDetectionModelWrapper,
 )
 
 
 class InstanceSegmentationModelWrapper(ObjectDetectionModelWrapper):
     """Wrapper class over mm instance segmentation model of MMDetection framework."""
-    MODEL_OUTPUT_KEY_ORDERING = [
-        MmDetectionDatasetLiterals.GT_BBOXES,
-        MmDetectionDatasetLiterals.GT_LABELS,
-        MmDetectionDatasetLiterals.GT_CROWDS,
-        MmDetectionDatasetLiterals.GT_MASKS,
-        MmDetectionDatasetLiterals.BBOXES,
-        MmDetectionDatasetLiterals.LABELS,
-        MmDetectionDatasetLiterals.MASKS,
-    ]
 
     def __init__(
         self,
         mm_instance_segmentation_model: nn.Module,
         config: Config,
         model_name_or_path: str,
+        task_type: str,
+        num_labels: int,
+        box_score_threshold: int,
+        iou_threshold: int,
         meta_file_path: str = None,
     ):
         """Wrapper class over mm instance segmentation model of MMDetection framework.
         :param mm_instance_segmentation_model: MM instance segmentation model
         :type mm_instance_segmentation_model: nn.Module
         :param config: MM Instance segmentation model configuration
         :type config: MMCV Config
         :param model_name_or_path: model name or path
         :type model_name_or_path: str
+        :param task_type: Name of the Task(Instance Segmentation)
+        :type task_type: str
+        :param num_labels: Number of ground truth classes in the dataset
+        :type num_labels: int
+        :param box_score_threshold: Threshold for bounding box score
+        :type box_score_threshold: float
+        :param iou_threshold: Threshold for IoU(inetersection over union)
+        :type iou_threshold: float
         :param meta_file_path: path to meta file
         :type meta_file_path: str
         """
         super(InstanceSegmentationModelWrapper, self).__init__(
-            mm_instance_segmentation_model, config, model_name_or_path, meta_file_path
+            mm_instance_segmentation_model,
+            config,
+            model_name_or_path,
+            task_type,
+            num_labels,
+            box_score_threshold,
+            iou_threshold,
+            meta_file_path
         )
 
     @classmethod
-    def _get_segmentation_masks(cls, mask_result: List[List[np.ndarray]]) -> Tensor:
+    def _convert_masks_to_rle(cls, masks: Union[List[torch.Tensor], torch.Tensor]) -> List[Dict]:
         """
-        Map the model's predicted segmentation masks to the format required by the HF trainer
-        :param mask_result:
-        :type mask_result: List of masks
-        :return: mask in tensor format
-        :rtype: Tensor
-        """
-        mask = mmcv.concat_list(
-            mask_result
-        )  # Concatenate a list of list into a single list.
-        if isinstance(mask[0], torch.Tensor):
-            mask = torch.stack(mask, dim=0)
-        else:
-            mask = torch.as_tensor(np.stack(mask, axis=0))
-        return mask
+        Convert masks to rle as required by metrics functions
+        :param masks: Binary masks
+        :type masks: np.ndarray
+        :return: List of masks in rle format
+        :rtype: List of rle dict
+        sample input: [[0, 0, 1, 1], [2, 2, 3, 3]]
+        sample output: [{"size": [5, 5], "counts": "0311090E"}, {"size": [5, 5], "counts": "0b01@01"}]
+        """
+        rle_mask = list()
+        for mask in masks:
+            rle_mask.append(masktools.encode_mask_as_rle(mask))
+        return rle_mask
 
-    @classmethod
-    def _organize_predictions_for_trainer(
-        cls,
-        batch_predictions: List[Tuple[List[np.ndarray], List[np.ndarray]]],
-        img_metas: List[Dict],
-    ) -> Dict[str, Tensor]:
-        """
-        Transform the batch of predicted labels as required by the HF trainer.
-        :param batch_predictions: batch of predicted labels
-        :type batch_predictions: List of tuple containing list of bboxes and masks
-        :param img_metas: batch of predicted labels
-        :type img_metas: List of image metadata dictionary
-        :return: Dict of predicted labels in tensor format
-        :rtype: Dict[str, Tensor]
-
-        Note: Same reasoning like _organize_ground_truth_for_trainer function but for predicted label
-        """
-        batch_bboxes, batch_labels, batch_masks = [], [], []
-        for (predicted_bbox, predicted_mask), img_meta in zip(
-            batch_predictions, img_metas
-        ):
-            if isinstance(predicted_mask, tuple):
-                predicted_mask = predicted_mask[0]  # ms rcnn
-
-            bboxes, labels = super()._get_bboxes_and_labels(predicted_bbox)
-            if predicted_mask is not None and len(labels) > 0:
-                masks = InstanceSegmentationModelWrapper._get_segmentation_masks(
-                    predicted_mask
-                )
-            else:
-                # The case when all predictions are below the box score threshold. Add empty mask tensor to satisfy
-                # the pad_sequence criteria.
-                height, width, channel = img_meta[
-                    MmDetectionDatasetLiterals.IMAGE_ORIGINAL_SHAPE
-                ]
-                masks = torch.empty(0, height, width)
-
-            batch_bboxes.append(bboxes)
-            batch_labels.append(labels)
-            batch_masks.append(masks)
-
-        output = dict()
-        output[MmDetectionDatasetLiterals.BBOXES] = super()._pad_sequence(batch_bboxes)
-        output[MmDetectionDatasetLiterals.LABELS] = super()._pad_sequence(batch_labels)
-        output[MmDetectionDatasetLiterals.MASKS] = super()._pad_sequence(batch_masks)
-        return output
+    def _organize_predictions_for_evaluation(
+        self,
+        batch_predictions: List[DetDataSample]
+    ) -> List[Dict[str, np.ndarray]]:
+        """
+        This function transforms the predictions from HF trainer as required by the metrics functions.
+        It also filters out the predictions which are under the threshold.
+        :param predictions: list of model prediction with attributes bboxes, labels and masks
+        :type predictions: List[mmdet.structures.DetDataSample]
+        :return: Transformed predictions as required by metrics compute function
+        :rtype: List of prediction dictionary List[Dict[str, np.ndarray]]
+
+        Sample output:
+        [{
+            # List of bounding boxes for first input image
+            DetectionDatasetLiterals.BOXES: np.array([[0, 0, 1, 1], [2, 2, 3, 3]]),
+            # List of predicetd classes for first input image
+            MetricsLiterals.CLASSES: np.array([0, 1]),
+            # List of predicetd rle masks for first input image
+            MmDetectionDatasetLiterals.MASKS: [
+                {"size": [5, 5], "counts": "0311090E"}, {"size": [5, 5], "counts": "0b01@01"}
+            ]
+        }, {
+            # List of bounding boxes for second input image
+            DetectionDatasetLiterals.BOXES: np.array([[0, 1, 3, 4]]),
+            # List of predicetd classes for second input image
+            MetricsLiterals.CLASSES: np.array([0]),
+            # List of predicetd rle masks for second input image
+            MmDetectionDatasetLiterals.MASKS: [
+                [{"size": [5, 5], "counts": "0=1L0H"}]
+            ]
+        }]
+        """
+        outputs = []
+        for prediction in batch_predictions:
+            prediction = prediction.detach()
+            pred_instances = prediction.pred_instances
+            indices = pred_instances.scores >= self.box_score_threshold
+            output = {
+                DetectionDatasetLiterals.BOXES: pred_instances.bboxes[indices].cpu().numpy(),
+                MetricsLiterals.CLASSES: pred_instances.labels[indices].cpu().numpy(),
+                MetricsLiterals.SCORES: pred_instances.scores[indices].cpu().numpy(),
+                DetectionDatasetLiterals.MASKS: [],
+            }
+            h_original, w_original, _ = prediction.raw_dimensions
+            h_resized, w_resized = prediction.img_shape
+            output[DetectionDatasetLiterals.BOXES] = [
+                self.adjust_boundingbox_scale(bbox,
+                                              h_resized,
+                                              w_resized,
+                                              h_original,
+                                              w_original) for bbox in output[DetectionDatasetLiterals.BOXES]]
+
+            for idx in range(len(indices)):
+                if not indices[idx]:
+                    continue
+                pred_mask = pred_instances.masks[idx].cpu().numpy()
+                pred_masks = np.array([pred_mask[:h_resized, :w_resized]])
+                resized_masks = resize_masks(pred_masks, [h_original, w_original])
+                resized_masks[0].dtype = np.bool8
+                output[DetectionDatasetLiterals.MASKS].append(
+                    self._convert_masks_to_rle(torch.from_numpy(np.array(resized_masks)))[0])
+            outputs.append(output)
+        return outputs
 
-    @classmethod
-    def _organize_ground_truth_for_trainer(
-        cls,
+    def _organize_ground_truths_for_evaluation(
+        self,
         gt_bboxes: List[Tensor],
         gt_labels: List[Tensor],
         gt_crowds: List[Tensor],
-        **kwargs
-    ) -> Dict[str, Tensor]:
+        gt_masks: List[BitmapMasks] = None,
+    ) -> Tuple[List[Dict], List[Dict]]:
         """
-        Transform the batch of ground truth as required by the HF trainer.
+        Organize the batch of ground truth as required by the azureml-metrics package for mAP calculations.
         :param gt_bboxes: batch of ground truth bounding boxes
         :type gt_bboxes: list of tensor
         :param gt_labels: batch of ground truth class labels
         :type gt_labels: list of tensor
         :param gt_crowds: batch of ground truth crowds flag
         :type gt_crowds: list of tensor
-        :param kwargs: A dictionary of additional configuration parameters. For instance segmentation taak,
-        it should contain the ground truth masks (bitmask type) in MmDetectionDatasetLiterals.GT_MASKS key.
-        :type kwargs: dict
-        :return: Dict of ground truth labels in Tensor type
-        :rtype: Dict[str, Tensor]
-
-        Note: The model needs the ground truth in dict of List of tensor format. List for batch and tensor for per
-         image labels. But, the HF trainer need the dictionary of tensor, otherwise it will fail while concatenating
-         the batches to form full dataset before passing to evaluation function.
-         We will need to convert these Dict[List] to Dict[tensors]. List can have different size; for example,
-         1st image can have 2 bbox and 2nd image can have 1 bbox. Hence, we need to pad the labels
-         to have same dimension so that it can be converted to tensor.
-        """
-        output = super()._organize_ground_truth_for_trainer(
-            gt_bboxes, gt_labels, gt_crowds
-        )
-        gt_masks = kwargs[MmDetectionDatasetLiterals.GT_MASKS]
-
-        # convert from bitmap to tensor
-        gt_masks_in_tensor = [
-            mask.to_tensor(dtype=torch.bool, device=get_current_device())
-            for mask in gt_masks
-        ]
-
-        output[MmDetectionDatasetLiterals.GT_MASKS] = super()._pad_sequence(gt_masks_in_tensor)
-        return output
+        :param gt_masks: batch of ground truth masks(bitmask type)
+        :type gt_masks: list of BitmapMasks
+        :return: Tuple of Dict of ground truth labels and Dict of image metadata information
+        :rtype: Tuple[List[Dict], List[Dict]]
+
+        sample output: (
+        [{
+            DetectionDatasetLiterals.BOXES: np.array([[0, 0, 1, 1], [2, 2, 3, 3]]),
+            MetricsLiterals.CLASSES: np.array([0, 1]),
+            DetectionDatasetLiterals.MASKS:
+                [{"size": [5, 5], "counts": "0311090E"}, {"size": [5, 5], "counts": "0b01@01"}]
+        }, {
+            DetectionDatasetLiterals.BOXES: np.array([[0, 1, 3, 4]]),
+            MetricsLiterals.CLASSES: np.array([0]),
+            DetectionDatasetLiterals.MASKS: [{"size": [5, 5], "counts": "0=1L0H"}]
+        }],
+        "image_metas": [
+            { DetectionDatasetLiterals.ISCROWD: np.array([False, False]) },
+            { DetectionDatasetLiterals.ISCROWD: np.array([True]) }
+        ])
+        """
+
+        gts, meta_infos = super()._organize_ground_truths_for_evaluation(gt_bboxes=gt_bboxes,
+                                                                         gt_labels=gt_labels,
+                                                                         gt_crowds=gt_crowds)
+        if gt_masks:
+            for i, gt_mask in enumerate(gt_masks):
+                gt_image_mask = gt_mask.to_tensor(dtype=torch.bool, device="cpu")
+                gt_rle_masks = self._convert_masks_to_rle(gt_image_mask)
+                gts[i].update({MmDetectionDatasetLiterals.MASKS: gt_rle_masks})
+        return gts, meta_infos
```

## azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py

```diff
@@ -20,220 +20,393 @@
 
 
 import numpy as np
 import os
 import shutil
 import torch
 
-from mmcv import Config
+from mmengine.config import Config, ConfigDict
+from mmengine.structures import InstanceData
+from mmdet.models.detectors.deformable_detr import DeformableDETR
+try:
+    from mmdet.structures import DetDataSample
+except ImportError:
+    DetDataSample = None
 from pathlib import Path
 from torch import nn, Tensor
-from torch.nn.utils.rnn import pad_sequence
 from typing import Dict, List, Union, Any, Tuple, OrderedDict
 
 from azureml.acft.common_components import get_logger_app, ModelSelectorDefaults
-from azureml.acft.image.components.finetune.common.utils import get_current_device
+from azureml.acft.image.components.finetune.common.mlflow.common_utils import get_current_device
+from azureml.acft.image.components.finetune.defaults.constants import TrainingDefaultsConstants
 from azureml.acft.image.components.finetune.mmdetection.common.constants import (
+    MmDetectionConfigLiterals,
+    MmDetectionModelLiterals
+)
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import (
     MmDetectionDatasetLiterals,
+    MMdetModes
+)
+from azureml.acft.image.components.finetune.common.mlflow.mmdet_modules import (
+    ObjectDetectionModelWrapper as mlflow_obj_det_wrapper
+)
+
+from azureml.acft.image.components.finetune.common.constants.constants import (
+    DetectionDatasetLiterals,
 )
+from azureml.acft.image.components.finetune.mmdetection.common.model_config_rules import MODEL_RULES_MAP
+from azureml.acft.image.components.finetune.common.mlflow.common_constants import MetricsLiterals
 from azureml.acft.image.components.model_selector.constants import ImageModelSelectorConstants
+from azureml.metrics.vision.od_is_eval.azureml_od_is_metrics import AzureMLODISMetrics
+from azureml.metrics.constants import Tasks as MetricsTasks
+from azureml.metrics import list_metrics
+
 
 logger = get_logger_app(__name__)
 
 
 class ObjectDetectionModelWrapper(nn.Module):
     """Wrapper class over object detection model of MMDetection framework."""
-    MODEL_OUTPUT_KEY_ORDERING = [
-        MmDetectionDatasetLiterals.GT_BBOXES,
-        MmDetectionDatasetLiterals.GT_LABELS,
-        MmDetectionDatasetLiterals.GT_CROWDS,
-        MmDetectionDatasetLiterals.BBOXES,
-        MmDetectionDatasetLiterals.LABELS,
-    ]
 
     def __init__(
         self,
         mm_object_detection_model: nn.Module,
         config: Config,
         model_name_or_path: str,
-        meta_file_path: str,
+        task_type: str,
+        num_labels: int,
+        box_score_threshold: int,
+        iou_threshold: int,
+        meta_file_path: str = None,
     ):
         """Wrapper class over object detection model of MMDetection.
         :param mm_object_detection_model: MM object detection model
         :type mm_object_detection_model: nn.Module
         :param config: MM Detection model configuration
         :type config: MMCV Config
         :param model_name_or_path: model name or path
         :type model_name_or_path: str
+        :param task_type: Task type either of Object Detection or Instance Segmentation
+        :type task_type: str
+        :param num_labels: Number of ground truth classes in the dataset
+        :type num_labels: int
+        :param box_score_threshold: Threshold for bounding box score
+        :type box_score_threshold: float
+        :param iou_threshold: Threshold for IoU(intersection over union)
+        :type iou_threshold: float
         :param meta_file_path: path to meta file
         :type meta_file_path: str
         """
         super().__init__()
         self.model = mm_object_detection_model
         self.config = config
         self.model_name = Path(model_name_or_path).stem
-        self.meta_file_path = meta_file_path
+        self.box_score_threshold = box_score_threshold
+        self.classes = list(self.config.id2label.values())
+        self.lang_model = hasattr(self.config, MmDetectionModelLiterals.LANG_MODEL_NAME)
+        self.text = ". ".join(self.classes) if self.lang_model else None
+
+        metrics_list = list_metrics(task_type)
+        self.metrics_computer = AzureMLODISMetrics(
+            task_is_detection=bool(task_type == MetricsTasks.IMAGE_OBJECT_DETECTION),
+            num_classes=num_labels,
+            iou_threshold=iou_threshold,
+            metrics=metrics_list,
+        )
+
+    def _organize_predictions_for_evaluation(
+        self,
+        batch_predictions: List
+    ) -> List[Dict[str, np.ndarray]]:
+        """
+        This function transforms the predictions from HF trainer as required by the metrics functions.
+        It also filters out the predictions which are under the threshold.
+        :param batch_predictions: list of model prediction with attributes bboxes, labels and masks
+        :type batch_predictions: List[mmdet.structures.DetDataSample]
+        :return: Transformed predictions as required by metrics compute function
+        :rtype: List of prediction dictionary List[Dict[str, np.ndarray]]
+
+        Sample output:
+        [{
+            # List of bounding boxes for first input image
+            DetectionDatasetLiterals.BOXES: np.array([[0, 0, 1, 1], [2, 2, 3, 3]]),
+            # List of predicetd classes for first input image
+            MetricsLiterals.CLASSES: np.array([0, 1]),
+            # List of predicetd rle masks for first input image
+            MmDetectionDatasetLiterals.MASKS: [
+                {"size": [5, 5], "counts": "0311090E"}, {"size": [5, 5], "counts": "0b01@01"}
+            ]
+        }, {
+            # List of bounding boxes for second input image
+            DetectionDatasetLiterals.BOXES: np.array([[0, 1, 3, 4]]),
+            # List of predicetd classes for second input image
+            MetricsLiterals.CLASSES: np.array([0]),
+            # List of predicetd rle masks for second input image
+            MmDetectionDatasetLiterals.MASKS: [
+                [{"size": [5, 5], "counts": "0=1L0H"}]
+            ]
+        }]
+        """
+        outputs = []
+        for prediction in batch_predictions:
+            prediction = prediction.detach()
+            pred_instances = prediction.pred_instances
+            indices = pred_instances.scores >= self.box_score_threshold
+            output = {
+                DetectionDatasetLiterals.BOXES: pred_instances.bboxes[indices].cpu().numpy(),
+                MetricsLiterals.CLASSES: pred_instances.labels[indices].cpu().numpy(),
+                MetricsLiterals.SCORES: pred_instances.scores[indices].cpu().numpy(),
+                DetectionDatasetLiterals.MASKS: [],
+            }
+            # Raw dimension is the original image size before resizing. img_shape is the resized image size.
+            # The predicted bounding boxes are w.r.t. the resized image size.
+            # Since the validation labels have bounding boxes w.r.t to the original image size, we are rescaling
+            # the predicted bounding boxes w.r.t. the original image size as well.
+            h_original, w_original, _ = prediction.raw_dimensions
+            h_resized, w_resized = prediction.img_shape
+            output[DetectionDatasetLiterals.BOXES] = [
+                self.adjust_boundingbox_scale(bbox,
+                                              h_resized,
+                                              w_resized,
+                                              h_original,
+                                              w_original) for bbox in output[DetectionDatasetLiterals.BOXES]]
+            outputs.append(output)
+        return outputs
 
-    @classmethod
-    def _get_bboxes_and_labels(
-        cls, predicted_bbox: List[List[np.ndarray]]
-    ) -> Tuple[Tensor, Tensor]:
-        """
-        Map the MM detection model's predicted label to the bbox and labels
-        :param predicted_bbox: bbox of shape [Number of labels, Number of boxes, 5 [tl_x, tl_y, br_x, br_y,
-        box_score]] format.
-        :type predicted_bbox: List[List[np.ndarray]]
-        :return: bounding boxes of shape [Number of boxes, 5 [tl_x, tl_y, br_x, br_y, box_score]] and labels of
-        shape [Number of boxes, label id]
-        :rtype: Tuple[Tensor, Tensor]
-        """
-        bboxes = torch.as_tensor(np.vstack(predicted_bbox))
-        labels = [
-            np.full(bbox.shape[0], i, dtype=np.int32)
-            for i, bbox in enumerate(predicted_bbox)
-        ]
-        labels = torch.as_tensor(np.concatenate(labels))
-        return bboxes, labels
-
-    @classmethod
-    def _pad_sequence(cls, sequences: Tensor, padding_value: float = -1, batch_first: bool = True) -> Tensor:
-        """
-        It stacks a list of Tensors sequences, and pads them to equal length.
-        :param sequences: list of variable length sequences.
-        :type sequences: Tensor
-        :param padding_value: value for padded elements
-        :type padding_value: float
-        :param batch_first: output will be in B x T x * if True, or in T x B x * otherwise
-        :type batch_first: bool
-        :return: Tensor of size ``B x T x *`` if batch_first is True
-        :rtype: Tensor
-        """
-        return pad_sequence(
-            sequences, padding_value=padding_value, batch_first=batch_first
-        ).to(get_current_device())
-
-    @classmethod
-    def _organize_ground_truth_for_trainer(
-        cls,
+    def _organize_ground_truths_for_evaluation(
+        self,
         gt_bboxes: List[Tensor],
         gt_labels: List[Tensor],
-        gt_crowds: List[Tensor],
-        **kwargs,
-    ) -> Dict[str, Tensor]:
+        gt_crowds: List[Tensor]
+    ) -> Tuple[List[Dict], List[Dict]]:
         """
-        Transform the batch of ground truth as required by the HF trainer.
+        Organize the batch of ground truth as required by the azureml-metrics package for mAP calculations.
         :param gt_bboxes: batch of ground truth bounding boxes
         :type gt_bboxes: list of tensor
         :param gt_labels: batch of ground truth class labels
         :type gt_labels: list of tensor
         :param gt_crowds: batch of ground truth crowds flag
         :type gt_crowds: list of tensor
-        :param kwargs: A dictionary of additional configuration parameters.
-        :type kwargs: dict
-        :return: Dict of ground truth labels
+        :return: Dict of ground truth labels in Tensor type
         :rtype: Dict[str, Tensor]
 
-        Note: The model needs the ground truth in dict of List of tensor format. List for batch and tensor for per
-         image labels. But, the HF trainer need the dictionary of tensor, otherwise it will fail while concatenating
-         the batches to form full dataset before passing to evaluation function.
-         We will need to convert these Dict[List] to Dict[tensors]. List can have different size; for example,
-         1st image can have 2 bbox and 2nd image can have 1 bbox. Hence, we need to pad the labels
-         to have same dimension so that it can be converted to tensor.
-        """
-        output = dict()
-        output[MmDetectionDatasetLiterals.GT_BBOXES] = ObjectDetectionModelWrapper._pad_sequence(gt_bboxes)
-        output[MmDetectionDatasetLiterals.GT_LABELS] = ObjectDetectionModelWrapper._pad_sequence(gt_labels)
-        output[MmDetectionDatasetLiterals.GT_CROWDS] = ObjectDetectionModelWrapper._pad_sequence(gt_crowds)
-        return output
-
-    @classmethod
-    def _organize_predictions_for_trainer(
-        cls, batch_predictions: List[List[np.ndarray]], img_metas: List[Dict]
-    ) -> Dict[str, Tensor]:
-        """
-        Transform the batch of predicted labels as required by the HF trainer.
-        :param batch_predictions: batch of predicted labels
-        :type batch_predictions: List of bbox list for each image
-        :param img_metas: batch of predicted labels
-        :type img_metas: List of image metadata dictionary
-        :return: Dict of predicted labels in tensor format
-        :rtype: Dict[str, Tensor]
+        Sample input:
+            gt_bboxes: [
+                torch.tensor([[0, 0, 1, 1], [2, 2, 3, 3]]),
+                torch.tensor([[0, 1, 3, 4]])
+            ]
+            gt_labels: torch.tensor([[0, 1], [0]])
+            gt_crowds: torch.tensor([[False, False], [True]])
+
+        Sample output: ([
+            {
+                DetectionDatasetLiterals.BOXES: np.array([[0, 0, 1, 1], [2, 2, 3, 3]]),
+                MetricsLiterals.CLASSES: np.array([0, 1]),
+            }, {
+                DetectionDatasetLiterals.BOXES: np.array([[0, 1, 3, 4]]),
+                MetricsLiterals.CLASSES: np.array([0]),
+            }
+        ],
+        [   # Image Metas
+            {DetectionDatasetLiterals.ISCROWD: np.array([False, False])},
+            {DetectionDatasetLiterals.ISCROWD: np.array([True])}
+        ])
+        """
+        batch_gt_bboxes = [gt_bbox.cpu().numpy() for gt_bbox in gt_bboxes]
+        batch_gt_labels = [gt_label.cpu().numpy() for gt_label in gt_labels]
+        batch_gt_crowds = [gt_crowd.cpu().numpy() for gt_crowd in gt_crowds]
+
+        gts: List[Dict] = list()
+        meta_infos: List[Dict] = list()
+        for gt_bboxes, gt_labels, gt_crowds in zip(
+            batch_gt_bboxes, batch_gt_labels, batch_gt_crowds
+        ):
+            ground_truth = {
+                DetectionDatasetLiterals.BOXES: gt_bboxes,
+                MetricsLiterals.CLASSES: gt_labels,
+            }
+            image_metadata = {DetectionDatasetLiterals.ISCROWD: gt_crowds}
+
+            gts.append(ground_truth)
+            meta_infos.append(image_metadata)
+        return gts, meta_infos
+
+    def _handle_anchor_outside_image_boundary_in_rpn(
+        self, inputs: torch.tensor, batch_data_samples: List["DetDataSample"], mode: MMdetModes  # type: ignore
+    ) -> Union[Dict, List["DetDataSample"]]:  # type: ignore
+        """
+        Handles anchors that fall outside the image boundary during the Region Proposal Network (RPN) stage.
+
+        This function temporarily allows anchors to be outside the image boundary by setting the 'allowed_border'
+        parameter to -1. It then performs a forward pass through the model. After the forward pass, it restores
+        the original value of 'allowed_border'.
+
+        :param inputs: The input tensor for the forward pass.
+        :type inputs: torch.tensor
+        :param batch_data_samples: A list of data samples for the batch.
+        :type batch_data_samples: List["DetDataSample"]
+        :param mode: The mode for the forward pass.
+        :type mode: MMdetModes
+        :return: The output of the forward pass, which could be a dictionary or a list of data samples,
+                depending on the mode.
+        :rtype: Union[Dict, List["DetDataSample"]]
+        """
+        try:
+            prev_val = self.model.train_cfg.rpn["allowed_border"]
+            self.model.train_cfg.rpn["allowed_border"] = -1
+        except Exception as ex:
+            logger.warning(f'Error while setting model.train_cfg.rpn["allowed_border"]: {str(ex)}')
 
-        Note: Same reasoning like _organize_ground_truth_for_trainer function but for predicted label
-        """
-        batch_bboxes, batch_labels = [], []
-        for prediction in batch_predictions:
-            bboxes, labels = ObjectDetectionModelWrapper._get_bboxes_and_labels(
-                prediction
-            )
-            batch_bboxes.append(bboxes)
-            batch_labels.append(labels)
-        output = dict()
-        output[MmDetectionDatasetLiterals.BBOXES] = ObjectDetectionModelWrapper._pad_sequence(batch_bboxes)
-        output[MmDetectionDatasetLiterals.LABELS] = ObjectDetectionModelWrapper._pad_sequence(batch_labels)
+        output = self.model(inputs, batch_data_samples, mode=mode)
+        self.model.train_cfg.rpn["allowed_border"] = prev_val
         return output
 
-    @classmethod
-    def _convert_output_to_tuple(cls, output: Dict) -> Tuple:
-        """Convert model output from dict to tuple to make it suitable for trainer distirubeted_concat method
-        :param output: model output containing predictions and ground truth
-        :type output: dict
-        :return: output formatted in tuple
-        :rtype: tuple
-        """
-        return tuple(output[key] for key in cls.MODEL_OUTPUT_KEY_ORDERING)
+    def _robust_forward(
+        self, inputs: torch.tensor, batch_data_samples: List["DetDataSample"], mode: MMdetModes  # type: ignore
+    ) -> Union[Dict, List["DetDataSample"]]:  # type: ignore
+        """This function performs a forward pass through the model, with additional error handling.
+
+        :param inputs: The input data for the forward pass.
+        :type inputs: torch.Tensor
+        :batch_data_samples: The batch data samples.
+        :type batch_data_samples: List[DetDataSample]
+        :mode: The mode for the forward pass.
+        :type mode: MMdetModes
+        :return: The output of the forward pass, which could be a dictionary or a list of data samples,
+                depending on the mode.
+        :rtype: Union[Dict, List["DetDataSample"]]
+        """
+        try:
+            return self.model(inputs, batch_data_samples, mode=mode)
+        except ValueError as ex:
+            error_message = (
+                "There is no valid anchor inside the image boundary. "
+                "Please check the image size and anchor sizes, or set "
+                "``allowed_border`` to -1 to skip the condition."
+            )
+            if error_message.lower() in str(ex).lower():
+                return self._handle_anchor_outside_image_boundary_in_rpn(inputs, batch_data_samples, mode)
+            else:
+                raise
 
-    def forward(self, **data) -> Union[Dict[str, Any], Tuple[Tensor, Tuple]]:
+    def forward(self, **data) -> Union[Dict[str, Any], Tuple[Tensor, Tensor]]:
         """
         Model forward pass for training and validation mode
         :param data: Input data to model
         :type data: Dict
         :return: A dictionary of loss components in training mode OR Tuple of dictionary of predicted and ground
         labels in validation mode
-        :rtype: Dict[str, Any] in training mode; Tuple[Tensor, Dict[str, Tensor]] in validation mode;
+        :rtype: Dict[str, Any] in training mode; Tuple[Tensor, Tensor] in validation mode;
 
         Note: Input data dictionary consist of
             img: Tensor of shape (N, C, H, W) encoding input images.
             img_metas: list of image info dict where each dict has: 'img_shape', 'scale_factor', 'flip',
              and may also contain 'filename', 'ori_shape', 'pad_shape', and 'img_norm_cfg'. For details on the values
              of these keys see `mmdet/datasets/pipelines/formatting.py:Collect`.
             gt_bboxes - Ground truth bboxes for each image with shape (num_gts, 4) in [tl_x, tl_y, br_x, br_y] format.
             gt_labels - List of class indices corresponding to each box
             gt_crowds - List of "is crowds" (boolean) to each box
             gt_masks - List of masks (type BitmapMasks) for each image if task is instance_segmentation
         """
-        if self.model.training:
-            # GT_CROWDS is not required for training
-            data.pop(MmDetectionDatasetLiterals.GT_CROWDS)
-            return self.model.train_step(data, optimizer=None)
+        # removing dummy_labels for forward calls
+        dummy_labels = data.pop(MmDetectionDatasetLiterals.DUMMY_LABELS, None)
+        is_train = self.model.training
+        inputs, batch_data_samples = \
+            mlflow_obj_det_wrapper.prepare_inputs_for_model_forward(data, is_train=is_train, text=self.text)
+        if is_train:
+            losses = self._robust_forward(inputs, batch_data_samples, mode=MMdetModes.LOSS)
+            parsed_losses, log_vars = self.model.parse_losses(losses)
+            op = {"loss" : parsed_losses}
+            return op  # type: ignore
         else:
-            img = data[MmDetectionDatasetLiterals.IMG]
-            img_metas = data[MmDetectionDatasetLiterals.IMG_METAS]
-            batch_predictions = self.model(
-                img=[img], img_metas=[img_metas], return_loss=False
-            )
-            output: dict = self._organize_predictions_for_trainer(
-                batch_predictions, img_metas
-            )
-            ground_truth: dict = self._organize_ground_truth_for_trainer(**data)
-            output.update(ground_truth)
+            data.pop(MmDetectionDatasetLiterals.IMG)
+            data.pop(MmDetectionDatasetLiterals.IMG_METAS)
+            batch_predictions = self._robust_forward(inputs, batch_data_samples, mode=MMdetModes.PREDICT)
+            gt_bboxes = data.pop(MmDetectionDatasetLiterals.ORIGINAL_GT_BBOXES)
+            gt_masks = data.pop(MmDetectionDatasetLiterals.ORIGINAL_GT_MASKS, None)
+            data.pop(MmDetectionDatasetLiterals.GT_BBOXES)
+            data.pop(MmDetectionDatasetLiterals.GT_MASKS, None)
+            mask_args = {MmDetectionDatasetLiterals.GT_MASKS: gt_masks} if gt_masks is not None else {}
+
+            predictions = self._organize_predictions_for_evaluation(batch_predictions)
+            gts, img_meta_infos = self._organize_ground_truths_for_evaluation(gt_bboxes=gt_bboxes, **data, **mask_args)
+            self.metrics_computer.update_states(y_test=gts, image_meta_info=img_meta_infos, y_pred=predictions)
 
+            # Returning dummy_loss, dummy_labels since HF-trainer eval step expects two outputs.
             dummy_loss = torch.asarray([]).to(get_current_device())
-
-            return dummy_loss, self._convert_output_to_tuple(output)
+            dummy_labels = torch.asarray([]).to(get_current_device())
+            return dummy_loss, dummy_labels
 
     def save_pretrained(self, output_dir: os.PathLike, state_dict: OrderedDict) -> None:
         """
         Save finetuned weights and model configuration
         :param output_dir: Output directory to store the model
         :type output_dir: os.PathLike
         :param state_dict: Model state dictionary
-        :return state_dict: Dict
+        :type state_dict: Dict
         """
         # TODO: Revisit the logic for resuming training from checkpoint. Taking user input in python script
         #  may not be a good idea from security perspective. Or, it may not affect as user machine is individual.
         os.makedirs(output_dir, exist_ok=True)
         torch.save(state_dict, os.path.join(output_dir, ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME))
+        # saving the unwrapped version that can be directly used with mmd repo
+        MMD_PATH = os.path.join(output_dir, ImageModelSelectorConstants.MMD_MODEL_CHECKPOINT_FILE_NAME)
+        torch.save(
+            {
+                MmDetectionConfigLiterals.STATE_DICT : self.model.state_dict(),
+                MmDetectionConfigLiterals.META : {
+                    MmDetectionConfigLiterals.CLASSES : self.classes}
+            }, MMD_PATH)
+        # dumping the class names in test_dataloader to be used with mmd repo
+        # for mmtracking, config doens't have test_dataloader, thus we skip this step. id2label will be in config
+        if hasattr(self.config, "test_dataloader") and hasattr(self.config.test_dataloader, "dataset"):
+            self.config.test_dataloader.dataset.metainfo = {
+                MmDetectionConfigLiterals.CLASSES : self.classes
+            }
+        model_type = self.config.model.type if hasattr(self.config, "model") \
+            and hasattr(self.config.model, "type") else None
+        if isinstance(self.model, DeformableDETR) and hasattr(self.config.model, "bbox_head"):
+            # Removing the following keys due to a bug in mmdetection for DeformableDETR model.
+            # https://github.com/open-mmlab/mmdetection/issues/10281. init_detector will fail if
+            # these keys are present.
+            # These keys are not present in the original config of the model, but init_detector adds
+            # these keys to the config after first load and we need to remove it before saving.
+            keys_to_remove = ["share_pred_layer", "num_pred_layer", "as_two_stage"]
+            for key in keys_to_remove:
+                if key in self.config.model.bbox_head:
+                    print(f"Removing {key} from model's bbox_head since it is not supported for DeformableDETR model.")
+                    del self.config.model.bbox_head[key]
+
+            # delete num_classes in dn_cfg since re loading the config file is failing
+            if hasattr(self.config.model, "dn_cfg"):
+                self.config.model.dn_cfg.pop("num_classes")
+
+        if model_type and model_type in MODEL_RULES_MAP:
+            MODEL_RULES_MAP[model_type]().apply(self.config.model)
+
         self.config.dump(os.path.join(output_dir, self.model_name + ".py"))
-        shutil.copy(self.meta_file_path,
-                    os.path.join(output_dir, ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME))
         logger.info(f"Model saved at {output_dir}")
+        Config.fromfile(os.path.join(output_dir, self.model_name + ".py"))
+        logger.info("Validated the Saved Model configuration.")
+
+    @staticmethod
+    def adjust_boundingbox_scale(bbox: List, h_cur: int, w_cur: int, h_raw: int, w_raw: int) -> List:
+        """ Adjusts the bounding box coordinates to the original image size.
+        :bbox: list of bounding box coordinates
+        :type bbox: list
+        :h_cur: Height of the input image after transformation. This is
+        the height of the image after constraint resize and not the final image height which
+        has additional padding as well.
+        :type h_cur: int
+        :w_cur: Width of the input image after transformation. This is
+        the width of the image after constraint resize and not the final image width which
+        has additional padding as well.
+        :type w_cur: int
+        :h_raw: Original height of the image
+        :type h_raw: int
+        :w_raw: Original width of the image
+
+        : return: list of bounding box coordinates adjusted to the original image size.
+        : rtype: list
+        """
+        adjusted_bbox = (bbox / [w_cur, h_cur, w_cur, h_cur]) * [w_raw, h_raw, w_raw, h_raw]
+        return adjusted_bbox
```

## azureml/acft/image/components/model_selector/component.py

```diff
@@ -1,38 +1,42 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """AzureML ACFT Image Components - model selector component code."""
 import glob
 import json
 import os
-from pathlib import Path
-import shutil
-from typing import Union
-import urllib
+from azureml.acft.common_components.utils.license_utils import save_license_file
+from azureml.acft.image.components.common.utils import download_file
 import yaml
 from os.path import dirname
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
-from azureml.acft.accelerator.utils.error_handling.error_definitions import (
-    LLMInternalError,
-)
-from azureml.acft.accelerator.utils.error_handling.exceptions import LLMException
+
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.common_components.model_selector.component import ModelSelector
 from azureml.acft.common_components.model_selector.constants import (
     ModelSelectorDefaults,
     ModelSelectorConstants,
+    ModelRepositoryURLs
+)
+from azureml.acft.common_components.utils.constants import MlflowMetaConstants
+from azureml.acft.common_components.utils.error_handling.error_definitions import (
+    ACFTUserError,
+    ACFTSystemError,
+    ValidationError,
 )
-from azureml.acft.common_components.utils.error_handling.error_definitions \
-    import ACFTUserError, ACFTSystemError, InvalidMlflowModelFormat
 from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException, ACFTSystemException
 from azureml.acft.image.components.finetune.factory.mappings import MODEL_FAMILY_CLS
+from azureml.acft.image.components.finetune.factory.task_definitions import Tasks
+from azureml.acft.image.components.finetune import UNSUPPORTED_HF_MODEL, UNSUPPORTED_MMDETECTION_MODEL, \
+    UNSUPPORTED_MMTRACKING_MODEL
 from azureml.acft.image.components.model_selector.constants import (
     ImageModelSelectorConstants,
     MMDetectionModelZooConfigConstants,
+    MMDSupportedTasks, MMTSupportedTasks
 )
 
 
 logger = get_logger_app(__name__)
 
 
 class ImageModelSelector(ModelSelector):
@@ -40,14 +44,15 @@
     def __init__(
         self,
         pytorch_model: str = None,
         mlflow_model: str = None,
         model_family: str = None,
         model_name: str = None,
         output_dir: str = None,
+        download_from_source: bool = False,
         **kwargs,
     ) -> None:
         """Implementation for image model selector.
 
         :param pytorch_model: asset path of pytorch model, defaults to None
         :type pytorch_model: str, optional
         :param mlflow_model: asset path of mlflow model, defaults to None
@@ -55,64 +60,81 @@
         :param model_family: model family (like HuggingFace, MMDetection), defaults to None
         :type model_family: str, optional
         :param model_name: model name from the framework (i.e., HF), defaults to None
         :type model_name: str, optional
         :param output_dir: path to store arguments and model, defaults to None
         :type output_dir: str, optional
         """
+        unsupported_model_list = []
+        if model_family == MODEL_FAMILY_CLS.HUGGING_FACE_IMAGE:
+            unsupported_model_list = UNSUPPORTED_HF_MODEL
+        elif model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            unsupported_model_list = UNSUPPORTED_MMDETECTION_MODEL
+        elif model_family == MODEL_FAMILY_CLS.MMTRACKING_VIDEO:
+            unsupported_model_list = UNSUPPORTED_MMTRACKING_MODEL
         super().__init__(
             pytorch_model=pytorch_model,
             mlflow_model=mlflow_model,
             model_name=model_name,
             output_dir=output_dir,
+            model_family=model_family,
+            unsupported_model_list=unsupported_model_list,
+            download_from_source=download_from_source,
             **kwargs,
         )
-        self.model_family = model_family
 
-    def _download_mlflow_model_from_registry(self) -> None:
-        """Download mlflow model from AzureML registry"""
-        model_path = os.path.join(
-            self.output_dir, ModelSelectorDefaults.MLFLOW_MODEL_DIRECTORY
-        )
-        if self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
-            ImageModelSelector.convert_pyfunc_mlflow_model_to_pytorch_model(self.mlflow_model, Path(model_path))
-        else:
-            ModelSelector.convert_mlflow_model_to_pytorch_model(self.mlflow_model, Path(model_path))
-        logger.info(
-            f"Downloaded mlflow model from {self.mlflow_model} to {model_path}."
-        )
+    def _is_acft_model(self):
+        """ Check whether i/p model is an acft model"""
+        is_acft_model = False
+        if self.mlflow_model:
+            is_acft_model = self.metadata.get(MlflowMetaConstants.IS_ACFT_MODEL, False)
+        elif self.pytorch_model:
+            # pytorch models that are produced by finetuning components(hf trainer) contain pytorch_model.bin
+            model_path = os.path.join(
+                self.output_dir, ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY
+            )
+            checkpoint_file = os.path.join(model_path, ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME)
+            is_acft_model = os.path.isfile(checkpoint_file)
+
+        model_type = "acft_model" if is_acft_model else "non_acft_model"
+        logger.info(f"Input model type: {model_type}")
+        return is_acft_model
+
+    def _is_mmd_2x_model(self, config_file_path) -> None:
+        """ Validate if it is MMD 2.x model."""
+        if os.path.exists(config_file_path) and self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            # Check and warn if it is MMD 2.x model.
+            with open(config_file_path, "r") as f:
+                config_data = f.read()
+                # In MMD 3.x model config, img_norm_cfg is moved to data_preprocessor.
+                # Source: https://mmdetection.readthedocs.io/en/latest/migration/config_migration.html
+                if "img_norm_cfg" in config_data and "data_preprocessor" not in config_data:
+                    error_string = (
+                        f"Model {self.model_name} is a MMDetection 2.x model and this component"
+                        " only supports MMDectection 3.x models. We strongly recommend MMD 3.x models from the"
+                        " model zoo but if 2.x models need be finetuned, use finetuning component version <=0.0.8"
+                    )
+                    raise ACFTValidationException._with_error(
+                        AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
+                    )
+
+    def raise_relevant_error(self, error_string):
+        """ raise system/user error based on model_type.
 
-    def convert_pyfunc_mlflow_model_to_pytorch_model(
-            mlflow_model_path: Union[str, Path],
-            download_dir: Path) -> None:
-        """
-        Download the mlflow model assets(in artifacts dir)
-        in the download directory to have similar directory structure as the pytorch model.
-
-        :param mlflow_model_path: Path of the mlflow model
-        :type mlflow_model_path: Union[str, Path]
-        :param download_dir: Destination directory to download the model
-        :type download_dir: Path
-        """
-
-        os.makedirs(download_dir, exist_ok=True)
-        try:
-            ARTIFACT_DIR = ImageModelSelectorConstants.ARTIFACTS_DIR
-            artifact_dir = Path(mlflow_model_path, f"{ARTIFACT_DIR}")
-
-            # copy the model artifacts to the download directory
-            shutil.copytree(artifact_dir, download_dir, dirs_exist_ok=True)
-
-        except Exception:
-            shutil.rmtree(download_dir, ignore_errors=True)
-            directories = f" '{artifact_dir}' "
+        :param error_string: error string to be logged
+        :type error_string: str
+        """
+        logger.error(error_string)
+        if not self.is_acft_model:
             raise ACFTValidationException._with_error(
-                AzureMLError.create(
-                    InvalidMlflowModelFormat, directories
-                )
+                AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
+            )
+        else:
+            raise ACFTSystemException._with_error(
+                AzureMLError.create(ACFTSystemError, pii_safe_message=error_string)
             )
 
     def _prepare_mmlab_arguments_from_input_model(self) -> dict:
         """Prepare arguments for MMLAB/MMDetection models.
 
         :return: A dictinary conatining argument name to value mapping to update.
         :rtype: dictionary
@@ -123,101 +145,160 @@
         elif self.mlflow_model is not None:
             input_model_path = self.mlflow_model
 
         abs_input_model_path = os.path.join(self.output_dir, input_model_path)
 
         model_metafile_json_path = os.path.join(
             abs_input_model_path,
-            ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME
+            ImageModelSelectorConstants.MODEL_METAFILE_NAME
         )
         if os.path.exists(model_metafile_json_path):
+            # If model_metafile.json exists, then read the model name from it.
             with open(model_metafile_json_path, "r") as jsonFile:
                 model_metadata = json.load(jsonFile)
+
+            for name in [ModelSelectorConstants.FINETUNING_TASKS, ModelSelectorConstants.MODEL_NAME]:
+                if name not in model_metadata:
+                    error_string = (
+                        f"Ensure provided model path {input_model_path} contains "
+                        f"{ImageModelSelectorConstants.MODEL_METAFILE_NAME} with "
+                        f"{name} in it."
+                    )
+                    self.raise_relevant_error(error_string)
             if self.model_name is not None and self.model_name != model_metadata[ModelSelectorConstants.MODEL_NAME]:
                 error_string = (
                     f"Ensure provided model_name ({self.model_name}) matches with what's in "
-                    f"{ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME} - "
+                    f"{ImageModelSelectorConstants.MODEL_METAFILE_NAME} - "
                     f"{model_metadata[ModelSelectorConstants.MODEL_NAME]}."
                 )
-                raise LLMException._with_error(
-                    AzureMLError.create(LLMInternalError, error=error_string)
-                )
+                self.raise_relevant_error(error_string)
             else:
                 self.model_name = model_metadata[ModelSelectorConstants.MODEL_NAME]
+        else:
+            error_string = (
+                f"Input model path {input_model_path} does not contain "
+                f"{ImageModelSelectorConstants.MODEL_METAFILE_NAME}."
+            )
+            self.raise_relevant_error(error_string)
 
         self.model_name = self.model_name if not self.model_name.endswith(".py") else self.model_name[:-3]
 
         if self.model_name is None:
             error_string = (
-                f"We could not indentify {ModelSelectorConstants.MODEL_NAME}'s value {self.model_name}. "
+                f"We could not identify {ModelSelectorConstants.MODEL_NAME}'s value {self.model_name}. "
                 f"Ensure to either pass model name in {ModelSelectorConstants.MODEL_NAME}, or in "
-                f"{ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME} as "
+                f"{ImageModelSelectorConstants.MODEL_METAFILE_NAME} as "
                 f"{{{ModelSelectorConstants.MODEL_NAME}: <NAME_OF_MODEL>}}"
             )
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
-            )
+            self.raise_relevant_error(error_string)
+        self.model_name = self.model_name if not self.model_name.endswith(".py") else self.model_name[:-3]
 
         abs_mmlab_config_path = os.path.join(abs_input_model_path, f"{self.model_name}.py")
         # Assume that model config is in the parent folder
         mmlab_config_path = abs_mmlab_config_path.replace(abs_input_model_path, input_model_path)
         # Check existance of mmlab config python file
         if not os.path.exists(abs_mmlab_config_path):
             error_string = (
                 f"Ensure that {self.model_name}.py exists in your registered input model folder. "
                 f"Found list of files: {os.listdir(abs_input_model_path)}"
             )
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
-            )
-
+            self.raise_relevant_error(error_string)
+        self._is_mmd_2x_model(abs_mmlab_config_path)
         # Get the model weight file path
         checkpoint_files = glob.glob(os.path.join(abs_input_model_path, "*.pth"), recursive=True)
         if len(checkpoint_files) == 0:
             checkpoint_files = glob.glob(os.path.join(abs_input_model_path,
                                                       ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME),
                                          recursive=True)
         if len(checkpoint_files) != 1:
             error_string = (
                 f"Ensure that you have only one .pth or {ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME} "
                 f"checkpoint file in your registered model. Found {len(checkpoint_files)}"
             )
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
-            )
+            self.raise_relevant_error(error_string)
         # Assume checkpoint is in the parent folder
         checkpoint_file_name = checkpoint_files[0].replace(abs_input_model_path, input_model_path)
-        model_metafile_json_path = model_metafile_json_path.replace(abs_input_model_path, input_model_path)
 
         if self.pytorch_model is not None:
             self.pytorch_model = mmlab_config_path
         elif self.mlflow_model is not None:
             self.mlflow_model = mmlab_config_path
 
+        # copy license file
+        save_license_file(
+            model_name_or_path=input_model_path,
+            license_file_name=ModelSelectorDefaults.LICENSE_FILE_NAME,
+            destination_paths=[abs_input_model_path]
+        )
+
+        self.metadata.update(**model_metadata)
         return {
             ModelSelectorConstants.MODEL_NAME: self.model_name,
             ModelSelectorConstants.MLFLOW_MODEL_PATH: self.mlflow_model,
             ModelSelectorConstants.PYTORCH_MODEL_PATH: self.pytorch_model,
             ImageModelSelectorConstants.MMLAB_MODEL_WEIGHTS_PATH_OR_URL: checkpoint_file_name,
-            ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_PATH: model_metafile_json_path
+            ModelSelectorConstants.MODEL_METADATA: self.metadata,
         }
 
     def _load_and_save_mm_config_file(self, mm_config_file: str) -> str:
         """Load and save MMLAB/MMDetection config file
         :param mm_config_file: path to MMLAB/MMDetection config file in repository
         :type mm_config_file: str
         :return: config file name
         :rtype: str
         """
-        from mmcv import Config
+        from mmengine.config import Config
         config = Config.fromfile(mm_config_file)
         file_name = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY, self.model_name + ".py")
         config.dump(os.path.join(self.output_dir, file_name))
         return file_name
 
+    def _fetch_finetuning_tasks(self, model_data: dict) -> list:
+        """Fetch finetuning tasks from model_data
+
+        :param model_data: model_data
+        :type model_data: dict
+        :return: list of finetuning tasks
+        :rtype: list
+        """
+        finetuning_tasks = [result[MMDetectionModelZooConfigConstants.TASK].lower() for result in
+                            model_data[MMDetectionModelZooConfigConstants.RESULTS]]
+
+        # supporting object detection and instance segmentation
+        if self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            for task in finetuning_tasks:
+                if task not in [MMDSupportedTasks.OBJECT_DETECTION, MMDSupportedTasks.INSTANCE_SEGMENTATION]:
+                    error_string = (
+                        f"Finetuning for {MMDSupportedTasks.OBJECT_DETECTION}/"
+                        f"{MMDSupportedTasks.INSTANCE_SEGMENTATION} is supported."
+                        f"Provided Model: {self.model_name} supports {task}"
+                    )
+                    logger.error(error_string)
+                    raise ACFTValidationException._with_error(
+                        AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
+                    )
+        elif self.model_family == MODEL_FAMILY_CLS.MMTRACKING_VIDEO:
+            for task in finetuning_tasks:
+                if task not in [MMTSupportedTasks.MULTI_OBJECT_TRACKING]:
+                    error_string = (
+                        f"Finetuning for {MMTSupportedTasks.MULTI_OBJECT_TRACKING}  is supported."
+                        f"Provided Model: {self.model_name} supports {task}"
+                    )
+                    logger.error(error_string)
+                    raise ACFTValidationException._with_error(
+                        AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
+                    )
+
+        # models which support instance_segmentation always expects gt_masks from the data.
+        # results in model_data contain od but finetuning for od is not supported.
+        if MMDSupportedTasks.INSTANCE_SEGMENTATION in finetuning_tasks:
+            finetuning_tasks = [MMDSupportedTasks.INSTANCE_SEGMENTATION]
+
+        return finetuning_tasks
+
     def _prepare_mmlab_arguments_from_model_zoo_config(self) -> dict:
         """Prepared arguments for MMLAB/MMDetection models using the model name as in MMDetection model zoo.
 
         :return: A dictinary conatining argument name to value mapping to update.
         :rtype: dictionary
         """
         if (
@@ -227,75 +308,100 @@
         ):
             error_string = (
                 "All, model_name, mlflow_model, pytorch_model can not be None at the same time."
                 "Please provide either a model via pytorch_model or mlflow_model port; Or, "
                 "provide name of the model from MMDetection model zoo, as specified in respective model"
                 "family's metafile.yaml."
             )
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_string)
             )
 
-        meta_file = ImageModelSelector._search_model_name_in_mmd_model_zoo(self.model_name)
+        abs_config_folder_path = self._get_config_path()
+
+        meta_file = ImageModelSelector._search_model_name_in_mmd_model_zoo(self.model_name,
+                                                                           abs_config_folder_path,
+                                                                           self._get_model_zoo_link())
         model_data = None
         if meta_file is not None:
             # read yml file and get the model data
             with open(meta_file, "r") as f:
-                data = yaml.safe_load(f)
-                for model in data[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODELS]:
-                    if self.model_name in model[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODEL_NAME]:
+                metafile_dict = yaml.safe_load(f)
+                models_dict_list = metafile_dict if isinstance(metafile_dict, list) \
+                    else metafile_dict[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODELS]
+                for model in models_dict_list:
+                    if self.model_name == model[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODEL_NAME]:
                         model_data = model
                         break
         else:
             error_string = f"Not able to find the meta file {meta_file}."
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_string)
             )
 
         if model_data is None:
             error_string = f"Ensure that {self.model_name} data exists in the meta file."
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_string)
             )
-        abs_config_folder_path = ImageModelSelector._get_mmdet_config_path()
         abs_mmlab_config_path = os.path.join(
             dirname(abs_config_folder_path),
             model_data[MMDetectionModelZooConfigConstants.MODEL_ZOO_CONFIG],
         )
 
         if not os.path.exists(abs_mmlab_config_path):
-            error_string = f"Ensure that {self.model_name}.py exists in the model zoo configs folder."
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=error_string)
+            error_string = f"Ensure that {self.model_name}.py exists in the model zoo configs folder. \
+                The model zoo used is the following:{self._get_model_zoo_link()}."
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_string)
             )
 
+        if self.model_name.endswith(".py"):
+            self.model_name = self.model_name[:-3]
+
         os.makedirs(os.path.join(self.output_dir, ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY), exist_ok=True)
+
+        self.pytorch_model = self._load_and_save_mm_config_file(abs_mmlab_config_path)
+        self._is_mmd_2x_model(os.path.join(self.output_dir, self.pytorch_model))
+
         # Get the model weight file path
-        url = model_data[MMDetectionModelZooConfigConstants.MODEL_ZOO_WEIGHTS]
+        url = model_data.get(MMDetectionModelZooConfigConstants.MODEL_ZOO_WEIGHTS, None)
+        if not url:
+            error_str = f"{MMDetectionModelZooConfigConstants.MODEL_ZOO_WEIGHTS} key is not found in the"\
+                        f"metafile: {meta_file}. please select any other model for image finetuning."
+            logger.error(error_str)
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ValidationError, error=error_str))
         weights_file_name = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY,
                                          self.model_name + "_weights.pth")
         # download the file
-        urllib.request.urlretrieve(
-            url,
-            os.path.join(self.output_dir, weights_file_name),
-        )
+        download_file(url, os.path.join(self.output_dir, weights_file_name))
 
-        self.pytorch_model = self._load_and_save_mm_config_file(abs_mmlab_config_path)
-        model_metafile_json_path = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY,
-                                                ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME)
-        with open(os.path.join(self.output_dir, model_metafile_json_path), "w") as f:
-            model_metadata = {"model_name": self.model_name}
-            json.dump(model_metadata, f)
+        # fetch fine tuning tasks to dump in the model_metafile
+        finetuning_tasks = self._fetch_finetuning_tasks(model_data)
+        self.metadata.update({ModelSelectorConstants.FINETUNING_TASKS : finetuning_tasks})
+
+        model_metadata_path = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY,
+                                           ModelSelectorDefaults.MODEL_METADATA_PATH)
+        model_metadata_dict = {
+            ModelSelectorConstants.MODEL_NAME: self.model_name,
+            ModelSelectorConstants.FINETUNING_TASKS: finetuning_tasks,
+        }
+        if not os.path.exists(os.path.join(self.output_dir, model_metadata_path)):
+            # only dump the model metadata if it does not exist
+            with open(os.path.join(self.output_dir, model_metadata_path), 'w') as fp:
+                json.dump(model_metadata_dict, fp)
 
         return {
             ModelSelectorConstants.MODEL_NAME: self.model_name,
             ModelSelectorConstants.MLFLOW_MODEL_PATH: self.mlflow_model,
             ModelSelectorConstants.PYTORCH_MODEL_PATH: self.pytorch_model,
             ImageModelSelectorConstants.MMLAB_MODEL_WEIGHTS_PATH_OR_URL: weights_file_name,
-            ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_PATH: model_metafile_json_path
+            ModelSelectorConstants.MODEL_METADATA: self.metadata,
+            ModelSelectorConstants.MODEL_METAFILE_PATH: model_metadata_path,
         }
 
     def _prepare_mmlab_arguments(self) -> dict:
         """Prepare an update for the keyword arguments (if present) with required key-val items for MMLab/MMDetection
         models.
 
         :return: A dictinary conatining argument name to value mapping to update.
@@ -307,22 +413,34 @@
         else:
             return self._prepare_mmlab_arguments_from_model_zoo_config()
 
     def _prepare_and_logs_arguments(self) -> None:
         """Update the keyword arguments (if present) with required key-val items and
         Store the model selector arguments to json file.
         """
+
+        self.is_acft_model = self._is_acft_model()
+        if self.is_acft_model:
+            task_type = self.metadata.get(MlflowMetaConstants.FINETUNING_TASK, None)
+            # check if the input model supports image finetuning tasks
+            if task_type and task_type not in [i for i in Tasks.__dict__.values()]:
+                error_string = "Input model does not support finetuning of image tasks"
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
+                )
+
         arguments = {
             ModelSelectorConstants.MLFLOW_MODEL_PATH: self.mlflow_model,
             ModelSelectorConstants.PYTORCH_MODEL_PATH: self.pytorch_model,
             ModelSelectorConstants.MODEL_NAME: self.model_name,
-            ImageModelSelectorConstants.MODEL_FAMILY: self.model_family
+            ImageModelSelectorConstants.MODEL_FAMILY: self.model_family,
+            ModelSelectorConstants.MODEL_METADATA: self.metadata
         }
 
-        if self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+        if self.model_family in (MODEL_FAMILY_CLS.MMDETECTION_IMAGE, MODEL_FAMILY_CLS.MMTRACKING_VIDEO):
             arguments.update(self._prepare_mmlab_arguments())
 
         if self.keyword_arguments:
             self.keyword_arguments.update(arguments)
         else:
             self.keyword_arguments = arguments
 
@@ -333,34 +451,90 @@
         logger.info(
             f"Saving the model selector args to {model_selector_args_save_path}"
         )
         with open(model_selector_args_save_path, "w") as output_file:
             json.dump(self.keyword_arguments, output_file, indent=2)
 
     @staticmethod
-    def _search_model_name_in_mmd_model_zoo(model_name):
+    def _search_model_name_in_mmd_model_zoo(model_name, config_path=None, model_zoo_link=None):
         """
         Search for model name in all the metafile.yaml files present in model zoo configs folder
         """
-        for dirpath, _, filenames in os.walk(ImageModelSelector._get_mmdet_config_path()):
+        if config_path is None:  # set mmd path as default
+            config_path = ImageModelSelector._get_mmdet_config_path()
+        for dirpath, _, filenames in os.walk(config_path):
             for file_name in filenames:
                 file_path = os.path.abspath(os.path.join(dirpath, file_name))
                 if file_path.endswith("metafile.yml"):
-                    with open(file_path, "r") as f:
-                        if model_name in f.read():
-                            return file_path
-        error_string = f"Model {model_name} was not found in the metafile.yml files of the model zoo configs folder."
-        raise LLMException._with_error(
-            AzureMLError.create(LLMInternalError, error=error_string)
+                    with open(file_path, "r") as metafile:
+                        metafile_dict = yaml.safe_load(metafile)
+                        models_dict_list = metafile_dict if isinstance(metafile_dict, list) \
+                            else metafile_dict[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODELS]
+                        for model_config in models_dict_list:
+                            if model_config[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODEL_NAME] \
+                                and model_config[MMDetectionModelZooConfigConstants.MODEL_ZOO_MODEL_NAME].lower() == \
+                                    model_name.lower():
+                                return file_path
+
+        if model_name.startswith(ModelSelectorDefaults.FAST_RCNN_MODEL_PREFIX):
+            error_string = f"{model_name} seems to be fast-rcnn model since the model name starts with " \
+                f"{ModelSelectorDefaults.FAST_RCNN_MODEL_PREFIX} " \
+                "The fast-rcnn family of models should be trained with RPN family of models, therefore " \
+                "please use a model name from the RPN family of models. For more details, please refer to " \
+                f"{ModelRepositoryURLs.MMDETECTION}/fast_rcnn#introduction"
+        else:
+            error_string = f"Model {model_name} was not found in the metafile.yml files of the model zoo \
+                configs folder. Please use a valid model name from the model zoo."
+            if model_zoo_link is not None:
+                error_string += f" The model zoo used is the following:{model_zoo_link}.To find the correct \
+                model name, go to {model_zoo_link}, click on the model type, and you will find the \
+                model name in the metafile.yml file which is present at configs/<MODEL_TYPE>/metafile.yml location."
+
+        raise ACFTValidationException._with_error(
+            AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
         )
 
     @staticmethod
     def _get_mmdet_config_path() -> str:
         """Get the path to the MMDetection config file.
 
         :return: Path to the MMDetection config file.
         :rtype: str
         """
         import mmdet
         # Note: mmdet should be installed via mim to access the model zoo config folder.
         CONFIG_FOLDER_PATH = os.path.join(mmdet.__path__[0], ".mim", "configs")
         return CONFIG_FOLDER_PATH
+
+    @staticmethod
+    def _get_mmtrack_config_path() -> str:
+        """Get the path to the MmTracking config file.
+
+        :return: Path to the MmTracking config file.
+        :rtype: str
+        """
+        import mmtrack
+        # Note: mmtrack should be installed via mim to access the model zoo config folder.
+        CONFIG_FOLDER_PATH = os.path.join(mmtrack.__path__[0], ".mim", "configs")
+        return CONFIG_FOLDER_PATH
+
+    def _get_config_path(self) -> str:
+        """Get the path to the config file by model family
+
+        :return: Path to config file by model_family
+        :rtype: str
+        """
+        if self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            return ImageModelSelector._get_mmdet_config_path()
+        elif self.model_family == MODEL_FAMILY_CLS.MMTRACKING_VIDEO:
+            return ImageModelSelector._get_mmtrack_config_path()
+
+    def _get_model_zoo_link(self) -> str:
+        """Get the model zoo link by model family
+
+        :return: model zoo link by model_family
+        :rtype: str
+        """
+        if self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            return ModelRepositoryURLs.MMDETECTION
+        elif self.model_family == MODEL_FAMILY_CLS.MMTRACKING_VIDEO:
+            return ModelRepositoryURLs.MMTRACKING
```

## azureml/acft/image/components/model_selector/constants.py

```diff
@@ -1,27 +1,42 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """Constants used for image model selector component."""
-import os
 
 
 class ImageModelSelectorConstants:
     """String constants for model selector component."""
 
     ARTIFACTS_DIR = "artifacts"
     MODEL_FAMILY = "model_family"
+    MODEL_METAFILE_NAME = "model_metadata.json"
 
     MMLAB_MODEL_WEIGHTS_PATH_OR_URL = "model_weights_path_or_url"
     MMLAB_MODEL_METAFILE_PATH = "model_metafile_path"
-    MMLAB_MODEL_METAFILE_NAME = "model_metafile.json"
+    MMD_MODEL_CHECKPOINT_FILE_NAME = "mmd_pytorch_model.pth"
+    MODEL_DEFAULTS_PATH = "model_defaults_path"
 
 
 class MMDetectionModelZooConfigConstants:
     """
     Constants for MMDetection model zoo config.
     """
 
     MODEL_ZOO_MODELS = "Models"
     MODEL_ZOO_MODEL_NAME = "Name"
     MODEL_ZOO_CONFIG = "Config"
     MODEL_ZOO_WEIGHTS = "Weights"
+    RESULTS = "Results"
+    TASK = "Task"
+
+
+class MMDSupportedTasks:
+    """Supported tasks for MMDetection."""
+
+    OBJECT_DETECTION = "object detection"
+    INSTANCE_SEGMENTATION = "instance segmentation"
+
+
+class MMTSupportedTasks:
+    """Supported tasks for MMTracking"""
+    MULTI_OBJECT_TRACKING = "multiple object tracking"
```

## Comparing `azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py` & `azureml/acft/image/components/finetune/common/mlflow/mmtrack_mlflow_model_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,167 +1,141 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-"""Huggingface classification predict file for mlflow."""
+"""Mlflow PythonModel wrapper class that loads the Mlflow model, preprocess inputs and performs inference."""
 
 import logging
-
-import numpy as np
-import pandas as pd
+import subprocess
+import sys
 import tempfile
+import math
 
+import mlflow
+import pandas as pd
 import torch
-
-from datasets import load_dataset
-from transformers import (
-    AutoImageProcessor,
-    AutoModelForImageClassification,
-    TrainingArguments,
-    Trainer
-)
-from typing import List, Dict, Any, Optional, Tuple
-
-from common_constants import (HFMiscellaneousLiterals, HFMiscellaneousConstants, Tasks,
+from transformers import TrainingArguments
+from common_constants import (HFMiscellaneousLiterals,
+                              HFConstants, Tasks,
+                              MMDetLiterals,
                               MLFlowSchemaLiterals)
-from common_utils import create_temp_file, process_image
+from common_utils import process_video, create_temp_file, get_current_device
 
 logger = logging.getLogger(__name__)
 
 
-def predict(input_data: pd.DataFrame, task, model, tokenizer, **kwargs) -> pd.DataFrame:
-    """Perform inference on the input data.
+class ImagesMLFlowModelWrapper(mlflow.pyfunc.PythonModel):
+    """MLFlow model wrapper for AutoML for Images models."""
 
-    :param input_data: Input images for prediction.
-    :type input_data: Pandas DataFrame with a first column name ["image"] of images where each
-    image is in base64 String format.
-    :param task: Task type of the model.
-    :type task: HFTaskLiterals
-    :param tokenizer: Preprocessing configuration loader.
-    :type tokenizer: transformers.AutoImageProcessor
-    :param model: Pytorch model weights.
-    :type model: transformers.AutoModelForImageClassification
-    :return: Output of inferencing
-    :rtype: Pandas DataFrame with columns ["filename", "probs", "labels"] for classification and
-    ["filename", "boxes"] for object detection, instance segmentation
-    """
-    # Decode the base64 image column
-    decoded_images = input_data.loc[
-        :, [MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE]
-    ].apply(axis=1, func=process_image)
-
-    # arguments for Trainer
-    test_args = TrainingArguments(
-        output_dir=".",
-        do_train=False,
-        do_predict=True,
-        per_device_eval_batch_size=kwargs.get(MLFlowSchemaLiterals.BATCH_SIZE_KEY, 1),
-        dataloader_drop_last=False,
-        remove_unused_columns=False,
-    )
-
-    # To Do: change image height and width based on kwargs.
-
-    with tempfile.TemporaryDirectory() as tmp_output_dir:
-        image_path_list = (
-            decoded_images.iloc[:, 0]
-            .map(lambda row: create_temp_file(row, tmp_output_dir))
-            .tolist()
-        )
-        predicted_indexes, conf_scores = run_inference_batch(
-            test_args,
-            image_processor=tokenizer,
-            model=model,
-            image_path_list=image_path_list,
-            task_type=task,
-            threshold=kwargs.get(MLFlowSchemaLiterals.THRESHOLD, None)
-        )
+    def __init__(
+        self,
+        task_type: str,
+    ) -> None:
+        """This method is called when the python model wrapper is initialized.
 
-    df_result = pd.DataFrame(
-        columns=[
-            MLFlowSchemaLiterals.OUTPUT_COLUMN_PROBS,
-            MLFlowSchemaLiterals.OUTPUT_COLUMN_LABELS,
-        ]
-    )
-
-    labels = kwargs.get(MLFlowSchemaLiterals.TRAIN_LABEL_LIST)
-
-    if task == Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION:
-        predicted_labels = [labels[index] for index in predicted_indexes]
-    else:
-        predicted_labels = []
-        for predicted_index in predicted_indexes:
-            image_labels = []
-            for index, pred in enumerate(predicted_index):
-                if pred == 1:
-                    image_labels.append(labels[index])
-            predicted_labels.append(image_labels)
-
-    df_result[MLFlowSchemaLiterals.OUTPUT_COLUMN_PROBS], df_result[MLFlowSchemaLiterals.OUTPUT_COLUMN_LABELS]\
-        = (conf_scores.tolist(), predicted_labels)
-    return df_result
-
-
-def run_inference_batch(
-    test_args: TrainingArguments,
-    image_processor: AutoImageProcessor,
-    model: AutoModelForImageClassification,
-    image_path_list: List,
-    task_type: Tasks,
-    threshold: Optional[float] = None
-) -> Tuple[torch.tensor, torch.tensor]:
-    """Perform inference on batch of input images.
-
-    :param test_args: Training arguments path.
-    :type test_args: transformers.TrainingArguments
-    :param image_processor: Preprocessing configuration loader.
-    :type image_processor: transformers.AutoImageProcessor
-    :param model: Pytorch model weights.
-    :type model: transformers.AutoModelForImageClassification
-    :param image_path_list: list of image paths for inferencing.
-    :type image_path_list: List
-    :param task_type: Task type of the model.
-    :type task_type: Tasks
-    :param threshold: threshold for multi_label_classification
-    :type threshold: optional, float
-    :return: Predicted labels index, Predicted probabilities,
-    :rtype: Tuple of torch.tensor, torch.tensor
-    """
-
-    def collate_fn(examples: List[Dict[str, Any]]) -> Dict[str, torch.tensor]:
-        """Collator function for eval dataset.
-
-        :param examples: List of input images.
-        :type examples: List
-        :return: Dictionary of pixel values in torch tensor format.
-        :rtype: Dict
+        :param task_type: Task type used in training.
+        :type task_type: str
         """
-        images = [data[HFMiscellaneousLiterals.DEFAULT_IMAGE_KEY] for data in examples]
-        return image_processor(images, return_tensors="pt")
+        super().__init__()
+        self.test_args = None
+        self.test_transforms = None
+        self.mmtrack_run_inference_batch = None
+        self._config = None
+        self._model = None
+        self._task_type = task_type
+
+    def load_context(self, context: mlflow.pyfunc.PythonModelContext) -> None:
+        """This method is called when loading a Mlflow model with pyfunc.load_model().
 
-    inference_dataset = load_dataset(
-        "imagefolder",
-        data_files={"val": image_path_list}
-    )
-    inference_dataset = inference_dataset["val"]
-
-    # Initialize the trainer
-    trainer = Trainer(
-        model=model,
-        args=test_args,
-        tokenizer=image_processor,
-        data_collator=collate_fn,
-    )
-    results = trainer.predict(inference_dataset)
-    if task_type == Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION:
-        probs = torch.nn.functional.softmax(torch.from_numpy(results.predictions), dim=1).numpy()
-        y_pred = np.argmax(probs, axis=1)
-    elif task_type == Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION:
-        sigmoid = torch.nn.Sigmoid()
-        threshold = threshold or HFMiscellaneousConstants.DEFAULT_THRESHOLD
-
-        probs = sigmoid(torch.from_numpy(results.predictions)).numpy()
-        y_pred = np.zeros(probs.shape)
-        # next, use threshold to turn them into integer predictions
-        y_pred[np.where(probs >= threshold)] = 1
+        :param context: Mlflow context containing artifacts that the model can use for inference.
+        :type context: mlflow.pyfunc.PythonModelContext
+        """
+        logger.info("Inside load_context()")
+
+        if self._task_type in [Tasks.MM_MULTI_OBJECT_TRACKING]:
+            """
+            Install mmtrack, mmcv and mmdet using mim, with pip installation is not working
+            1. for mmtrack, one of its dependency is mmcv 1.6.2, which will trigger cuda related issues.
+                to mitigate, we use no dependency install for mmtrack, and put other dependencies in pip requirement
+            2. for opencv, the default installed by mmcv is opencv-python. however, it's installing unwanted UI,
+                which causes problems for stability. thus we force reinstall opencv-python-headless.
+            3. for numpy, we are reinstalling numpy to older version to be compatible to opencv. more info:
+                https://stackoverflow.com/questions/20518632/importerror-numpy-core-multiarray-failed-to-import
+            """
+            subprocess.check_call([sys.executable, "-m", "mim", "install", "mmcv-full==1.7.1"])
+            subprocess.check_call([sys.executable, "-m", "mim", "install", "mmdet==2.28.2"])
+            subprocess.check_call([sys.executable, "-m", "mim", "install", "--no-deps", "mmtrack==0.14.0"])
+            subprocess.check_call([sys.executable, "-m", "pip", "install",
+                                   "opencv-python-headless==4.7.0.72", "--force-reinstall"])
+            subprocess.check_call([sys.executable, "-m", "pip", "install", "numpy==1.19.3", "--force-reinstall"])
+
+            # importing mmdet/mmcv after installing using mim
+            from mmtrack.apis import init_model
+            from mmcv import Config
+            from mmcv.runner import load_checkpoint
+            from mmdet.datasets.pipelines import Compose
+            from mmtrack_module import MultiObjectTrackingModelWrapper
+            from mmtrack_utils import mmtrack_run_inference_batch
+            self.mmtrack_run_inference_batch = mmtrack_run_inference_batch
+
+            try:
+                model_config_path = context.artifacts[MMDetLiterals.CONFIG_PATH]
+                model_weights_path = context.artifacts[MMDetLiterals.WEIGHTS_PATH]
+                self._config = Config.fromfile(model_config_path)
+                self._model = init_model(self._config)
+                if self._task_type == Tasks.MM_MULTI_OBJECT_TRACKING:
+                    self._model = MultiObjectTrackingModelWrapper(self._model, self._config, model_weights_path)
+                load_checkpoint(self._model, model_weights_path, map_location=get_current_device())
+                logger.info("Model loaded successfully")
+            except Exception:
+                logger.warning("Failed to load the the model.")
+                raise
+
+            test_pipeline = self._config.data.test.pipeline
+            test_pipeline[0].type = 'LoadImageFromWebcam'
+            self.test_transforms = Compose(test_pipeline)
+        else:
+            raise ValueError(f"invalid task type {self._task_type}."
+                             f"Supported tasks: {Tasks.MM_MULTI_OBJECT_TRACKING}")
+
+    def predict(
+        self, context: mlflow.pyfunc.PythonModelContext, input_data: pd.DataFrame
+    ) -> pd.DataFrame:
+        """This method performs inference on the input data.
+
+        :param context: Mlflow context containing artifacts that the model can use for inference.
+        :type context: mlflow.pyfunc.PythonModelContext
+        :param input_data: Input images for prediction.
+        :type input_data: Pandas DataFrame with a first column name ["image"] of images where each
+        image is in base64 String format.
+        :return: Output of inferencing
+        :rtype: Pandas DataFrame with columns ["probs", "labels"] for classification and
+        ["boxes"] for object detection, instance segmentation
+        """
+        task = self._task_type
+        logger.info(f"evaluating with batch_size: {1}")
+
+        # arguments for Trainer
+        test_args = TrainingArguments(
+            output_dir=".",
+            do_train=False,
+            do_predict=True,
+            per_device_eval_batch_size=1,
+            dataloader_num_workers=HFConstants.DEFAULT_DATALOADER_NUM_WORKERS,
+            dataloader_drop_last=False,
+            remove_unused_columns=False
+        )
+
+        # process the videos in video column
+        processed_videos = input_data.loc[:, [MLFlowSchemaLiterals.INPUT_COLUMN_VIDEO]]\
+            .apply(axis=1, func=process_video)
+
+        result = self.mmtrack_run_inference_batch(
+            test_args=test_args,
+            model=self._model,
+            id2label=self._config[HFMiscellaneousLiterals.ID2LABEL],
+            processed_videos=processed_videos,
+            task_type=task,
+            test_transforms=self.test_transforms,
+        )
 
-    return y_pred, probs
+        return pd.DataFrame(result)
```

## Comparing `azureml/acft/image/components/finetune/defaults/classification_models_defaults.py` & `azureml/acft/image/components/finetune/defaults/multiclass_classification_models_defaults.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-"""Finetuning component classification model family defaults."""
+"""Finetuning component multiclass classification model family defaults."""
 
 from dataclasses import dataclass
 from azureml.acft.image.components.finetune.defaults.task_defaults import (
-    ClassificationDefaults,
+    MultiClassClassificationDefaults,
 )
 
 
 @dataclass
-class VITDefaults(ClassificationDefaults):
+class MultiClassVITDefaults(MultiClassClassificationDefaults):
     """
-    This class contain trainer defaults specific to VIT model family.
+    This class contain trainer defaults specific to VIT model family for multiclass classification.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
     _per_device_train_batch_size: int = 72
     _per_device_eval_batch_size: int = 72
     _learning_rate: float = 5.0249077359786836e-05
     _optim: str = "adamw_torch"
     _weight_decay: float = 6.933735771405163e-07
+    _metric_for_best_model: str = "loss"
 
 
 @dataclass
-class BEITDefaults(ClassificationDefaults):
+class MultiClassBEITDefaults(MultiClassClassificationDefaults):
     """
-    This class contain trainer defaults specific to BEIT model family.
+    This class contain trainer defaults specific to BEIT model family for multiclass classification.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
     _per_device_train_batch_size: int = 72
     _per_device_eval_batch_size: int = 72
     _learning_rate: float = 9.973114624235077e-05
     _weight_decay: float = 1.1847040694703787e-07
+    _metric_for_best_model: str = "loss"
 
 
 @dataclass
-class SWINV2Defaults(ClassificationDefaults):
+class MultiClassSWINV2Defaults(MultiClassClassificationDefaults):
     """
-    This class contain trainer defaults specific to SwinV2 model family.
+    This class contain trainer defaults specific to SwinV2 model family for multiclass classification.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    _image_width: int = 256
-    _image_height: int = 256
     _num_train_epochs: int = 5
     _per_device_train_batch_size: int = 12
     _per_device_eval_batch_size: int = 12
     _learning_rate: float = 3.388822145881516e-05
     _optim: str = "adafactor"
     _weight_decay: float = 1.6496304960471456e-08
+    _metric_for_best_model: str = "loss"
 
 
 @dataclass
-class DEITDefaults(ClassificationDefaults):
+class MultiClassDEITDefaults(MultiClassClassificationDefaults):
     """
-    This class contain trainer defaults specific to Deit model family.
+    This class contain trainer defaults specific to Deit model family for multiclass classification.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
     _per_device_train_batch_size: int = 60
     _per_device_eval_batch_size: int = 60
     _learning_rate: float = 5e-5
     _metric_for_best_model: str = "accuracy"
 
 
 @dataclass
-class MobileVITDefaults(ClassificationDefaults):
+class MultiClassMobileVITDefaults(MultiClassClassificationDefaults):
     """
-    This class contain trainer defaults specific to mobile vit model family.
+    This class contain trainer defaults specific to mobile vit model family for multiclass classification.
 
     Note: This class is not meant to be used directly.
     Provide the defaults name consistently with the Hugging Face Trainer class.
     """
 
-    _image_width: int = 448
-    _image_height: int = 448
     _per_device_train_batch_size: int = 16
     _per_device_eval_batch_size: int = 16
     _learning_rate: float = 6.605687285815252e-05
     _weight_decay: float = 1.3211374571630504e-05
     _lr_scheduler_type: str = "constant"
     _label_smoothing_factor: float = 0.1
+    _metric_for_best_model: str = "loss"
```

## Comparing `azureml_acft_image_components-0.0.9.dist-info/LICENSE.txt` & `azureml_acft_image_components-47.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_acft_image_components-0.0.9.dist-info/METADATA` & `azureml_acft_image_components-47.0.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1
-Name: azureml-acft-image-components
-Version: 0.0.9
-Summary: Contains the code for vision model's components.
-Home-page: https://msdata.visualstudio.com/Vienna/_git/sdk-cli-v2?version=GBtraining_finetune
-Author: Microsoft Corp
-License: inline_license
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8,<3.9
-Description-Content-Type: text/x-rst
-Requires-Dist: albumentations (==1.3.0)
-Requires-Dist: azureml-evaluate-mlflow
-Provides-Extra: all
-Requires-Dist: transformers (==4.26.1) ; extra == 'all'
-Provides-Extra: hf
-Requires-Dist: transformers (==4.26.1) ; extra == 'hf'
-Provides-Extra: mmd
-
-The azureml-acft-image-components package contains functionality used by the components for training image
-models available on various frameworks like hugging face, torchvision, MMDetection. This package is not designed to be installed by end-user directly.
-
-
+Metadata-Version: 2.1
+Name: azureml-acft-image-components
+Version: 47.0.0
+Summary: Contains the code for vision model's components.
+Home-page: https://msdata.visualstudio.com/Vienna/_git/sdk-cli-v2?version=GBtraining_finetune
+Author: Microsoft Corp
+License: inline_license
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8,<3.11
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: albumentations ==1.3.0
+Requires-Dist: azureml-mlflow
+Requires-Dist: peft ==0.4.0
+Provides-Extra: all
+Requires-Dist: transformers ==4.33.0 ; extra == 'all'
+Provides-Extra: hf
+Requires-Dist: transformers ==4.33.0 ; extra == 'hf'
+Provides-Extra: mmd
+
+The azureml-acft-image-components package contains functionality used by the components for training image
+models available on various frameworks like hugging face, torchvision, MMDetection. This package is not designed to be installed by end-user directly.
```

## Comparing `azureml_acft_image_components-0.0.9.dist-info/RECORD` & `azureml_acft_image_components-47.0.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,115 @@
 azureml/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/acft/__init__.py,sha256=qqupVla6VEo6r82whlPnifStK1J2C4O_mvyitUj6Gtk,295
 azureml/acft/image/__init__.py,sha256=WGGwHkYOREBwKsKBoq01dly26dZbULYG-kEjJllgnD4,822
-azureml/acft/image/components/NOTICE.txt,sha256=EQf8zdNpXgRtMJBAPCxdMMmqBLxxbRMbufcg3O2Yi_s,600282
+azureml/acft/image/components/NOTICE.txt,sha256=7QyQ2T7B9FM2GCp6HhCYAGnQAkOlVu0YGosCQJPbne0,552837
 azureml/acft/image/components/__init__.py,sha256=TyldUBdbBo69wJIzXzocmuvyEhS4v6wIBVXjk7SecE8,498
-azureml/acft/image/components/_version.py,sha256=GEQLI_HpmoMBfahlay2eatCORC4cSw-U1d_alMy5g14,34
+azureml/acft/image/components/_version.py,sha256=6tbwTfcvkL7u8i_rkvzyeWb_6rwSOsoLFvfhWf89WZM,36
 azureml/acft/image/components/common/__init__.py,sha256=67NkDhf7k9I_TLGAq1Bc3h3_EHkorbP9cthI9SlxOZk,312
-azureml/acft/image/components/common/utils.py,sha256=DAhC43RDSFpU4t90x4BxlFlz-lXh6IstJnuKM8IFcDM,583
-azureml/acft/image/components/finetune/__init__.py,sha256=zdA-QvDl7dTfTAapxHHMdHstIVbe-2WdgP7HPmhugMY,320
-azureml/acft/image/components/finetune/finetune_runner.py,sha256=DtIUtYSe-s5CrDzS3QzJhvrr5Uel02LO-IVKRenzX54,7753
+azureml/acft/image/components/common/constants.py,sha256=Gz7WR07FeG8ZQFhTr3jPuK7rHpkbtlEXr9B7teusrAk,1656
+azureml/acft/image/components/common/utils.py,sha256=YYOD44m5WjFjZVkYHTpv9Z7ieQUMZjEL33HNiRv28r0,1712
+azureml/acft/image/components/finetune/__init__.py,sha256=bHuK5rawYDh_1i-k55Ur_X3XTVaUN0RghHN8EVNbjp4,3810
+azureml/acft/image/components/finetune/finetune_runner.py,sha256=Ei7nz9vy9qCoh0c_mZA47MNFZYifZ9q0YsdGCuChZ2E,13407
 azureml/acft/image/components/finetune/common/__init__.py,sha256=fcxQ6oUUCqx3FVtqkf64D_C6G3fLv4sKP63jDTA4P3c,464
-azureml/acft/image/components/finetune/common/utils.py,sha256=1sWQMassg4tJ-HXTXz7MGB38oOrHVp-nPOoVVIt2UoM,1052
 azureml/acft/image/components/finetune/common/augmentation/__init__.py,sha256=XzmI_8D7RLFYFYhIHWlQEzNoidm6vueDIhVYs23Ltk4,313
 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py,sha256=adVNzRTXCQWJCqk_W0xkYEkFmQS16lbOHRRjKOUhuLQ,6267
 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py,sha256=s09P7WtXdeOZNXlqZ6AFhSATZ6LLz44GTwnmcXhda5Q,14648
 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py,sha256=HAsPVKQzoVn0CIWYycpUtWy6-wxXe7LE1rhQ58f1QgA,3152
-azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py,sha256=JbvuvwIPC6KCeRR9qnT8Y3mb-2nrPNzpZ0h2BX6XjiE,27652
+azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py,sha256=z-Yx_ZtSVSbbw2AMUhgH2MsSQNqJ1_uwDaH9MmtjZB8,29218
+azureml/acft/image/components/finetune/common/augmentation/openmmlab_augmentation.py,sha256=wqdkGGMWAHEvOeByeEVI1sTPpphzl3yrVQgxgrRfH_M,5379
 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py,sha256=JG43IYmXg2fXS1FNoebLt63IkV2hypGITnXUcz8dfCc,320
-azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml,sha256=4Uo-vR8XQSNcMO2C3Eaj-vMfa7JuJ0Zlx9VyTBdqtFM,1929
-azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml,sha256=sOmd_0GXkJO2OdNKoHnGbeGX016aBfMHKi-gkrRDZjs,2580
-azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml,sha256=Ai-zj88CJDxFR1rj9OkdoI5yx8nMH46dIsp57e7etiY,1314
+azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml,sha256=QlppohsD-7yLRRGnr40i0hVR7CW9Ue_lGE-7_zesB-w,2035
+azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml,sha256=ylXhFlIa9-tr56v25oaxdUnZOJljYwthgmXY9_R6Wi8,2784
 azureml/acft/image/components/finetune/common/constants/__init__.py,sha256=c9AETSCQhjx9UqOeXZvZ6DVap4R3qW-FxMJ39HCsO_8,309
-azureml/acft/image/components/finetune/common/constants/augmentation_constants.py,sha256=E1dGL46EIvm9S7JgNeHZ3l4HKYxrYrNcmGoSDJx3O4s,1550
-azureml/acft/image/components/finetune/common/constants/constants.py,sha256=D01E0e3zkwXwi99kBvBOhq1cEHAzFlecWFXCakTJw84,4628
+azureml/acft/image/components/finetune/common/constants/augmentation_constants.py,sha256=JKmCvvp3pD_dM3qtO5cRJVdhFRUR1WIM_VpWQbXTPtM,1859
+azureml/acft/image/components/finetune/common/constants/constants.py,sha256=q8XUz8Ri_jrSZ_gbgqcmD5BLjl9I0R6FM--WabB20n4,5014
 azureml/acft/image/components/finetune/common/data/__init__.py,sha256=Iqha0pV_7OWQ1pBcLUeBZW-Yo_GGxSzRRUvjZsW27Hw,304
 azureml/acft/image/components/finetune/common/data/base_dataset.py,sha256=DnvZM-dCQL6coxbE1blL-bsSnNaDPJUE2-YBILyO0_Y,5216
 azureml/acft/image/components/finetune/common/data/classification_dataset.py,sha256=DRPXxk3rAu3LiBLxHgPu8qhfTZyL8NlALiFPIh__fzw,9513
 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py,sha256=lKqSOy60LPU9dbvv2woj0xZxhsoQ5seoPwt-n3uVtCk,5469
+azureml/acft/image/components/finetune/common/data/data_utils.py,sha256=9VF57c41a67DCEu9I2gW5E_Pd-VdYopQXQfiV8IUBvM,7240
 azureml/acft/image/components/finetune/common/data/download_manager.py,sha256=0-rYQlv_q_xNRpCGI3oPuZHnzall0LIZLaJexDh3x-M,10779
-azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py,sha256=nPhPmEI9Z_HbYYbDkD9zVJLOsJ8CnWbJBXUcSO-ITWE,10729
+azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py,sha256=lEkXr7w5tvw-cR0ZEZ_CgsWbu1Ze8nBWBLvduFRHiYc,11053
 azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py,sha256=xqlVmqKVy9crg3fMTn1qfC2w120ORQiMfjKagAHpqkQ,7557
 azureml/acft/image/components/finetune/common/mlflow/__init__.py,sha256=D1Fxlq34-Arr84Ey1nucvWPYmkjmcrelBuwOvQVDSF4,338
 azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py,sha256=6k05-IRBeTQqKFFmXLHkcjvf1N_Of37oimaOLMwfxqo,8813
-azureml/acft/image/components/finetune/common/mlflow/common_constants.py,sha256=Ig9KdME_Ebfj0gK0-5N81WTb99NCFBCQfvukFLjY44g,3158
-azureml/acft/image/components/finetune/common/mlflow/common_utils.py,sha256=qPJaqKnz5YORxzuUhXju_UP81TutOtpNkOOnrQ50FRQ,2546
-azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py,sha256=q4A7_ySMa6SjDLNPhlkeNNnbzWGJeE4pqSkZ8AhOmVA,10883
-azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py,sha256=8s4d99ltap3BkArCfdQDQfGgJASc72cv7NdLSmrdI3U,6194
-azureml/acft/image/components/finetune/common/mlflow/hf_utils.py,sha256=E729Bkb19eO2tYLquLvK2zyJL6NMLs7ROS15a8jzntA,3222
-azureml/acft/image/components/finetune/common/mlflow/masktools.py,sha256=he6_slEVDNYwbWYLE_Q7G_9JsUJL1vGq4MXilep6L3A,3677
-azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py,sha256=2koLV_Cpbvz6Sdc4EVA46xoABkqPUhu0aduyN-vYEJE,6780
-azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt,sha256=jH_Wvn289w7ojmzOEuWcvePieKe1jD41qXdZ6x4y4OQ,170
-azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt,sha256=tZ15cmof2eQEB9M74a2c7Gn0MRFiATxaHGreraYBMLw,125
-azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py,sha256=1IiSByY-wRYQUvgwHOeyAQKxNhzuQzvHY6I2lSrtJ6s,6549
-azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py,sha256=aTsH0MiCyCb7HEr7kzn3iv4XmgkDYoX6qoj2vvzjQAU,10790
-azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py,sha256=u9gq-05bsUwI-uRsjOWhoNB1Qq-WPZHCAoUgiKJopZs,7009
+azureml/acft/image/components/finetune/common/mlflow/common_constants.py,sha256=bjVEnl_WLWfaiLIPRI7x6XvJ6jDtXGFSH8nBXX6ihnU,5099
+azureml/acft/image/components/finetune/common/mlflow/common_utils.py,sha256=J1VUR6IPT6edjdiBxtVTFuLolCoRo-B778CFHwosSek,4537
+azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py,sha256=SmGfStk12o9MNvK75R-qGEYUdBgi9vm3xZf5bakiNGU,16659
+azureml/acft/image/components/finetune/common/mlflow/custom_augmentations_openmm.py,sha256=3dFkSVuKP3_oit5U6ernlbbD6tg7v__rYI7tbfofdrk,5143
+azureml/acft/image/components/finetune/common/mlflow/masktools.py,sha256=1wnbX5vqxG3q23dVrczeNe9tFIxmq6uOfbfzaT4Hmi0,4076
+azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py,sha256=vdeGtIDFKd7YrLLSchEBD2XiJvfEokSAg3Wfcbo7tbA,12582
+azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt,sha256=1kwEWlwuVxzSUIt9WbRwRYmYxA1AOxYr23P6QUGGEdY,234
+azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt,sha256=HB9TnJ3gsIS0oPTw-Twcy_jXENfTV3ApGL9BRid_hzQ,188
+azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py,sha256=iuy0esHjzQjU4DPpr6W-G96vFpQhZXxfU_5LB8Rms90,7876
+azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py,sha256=4--usYV7diHIBtv8O3v1AmV9wk6N3FiQvSw4RmHEQ4U,13526
+azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py,sha256=pY78pozwemTlf4036H2GCL3pthGLKY0zlfb41JT4bjs,12062
+azureml/acft/image/components/finetune/common/mlflow/mmtrack-mot-conda.yaml,sha256=JH88ASNYrcaUk-Fcny5-KhHpYN0W6KyAZreJ85cosY4,444
+azureml/acft/image/components/finetune/common/mlflow/mmtrack_mlflow_model_wrapper.py,sha256=KjgZ-i-BIYMJRKNMKrke21bbZ2MRw7dLnOXt3xs-j-U,6619
+azureml/acft/image/components/finetune/common/mlflow/mmtrack_module.py,sha256=fPYUiQr4TMBzuE_ak4yRxGOoG68JWTrsJw-nIjfkL4o,5253
+azureml/acft/image/components/finetune/common/mlflow/mmtrack_utils.py,sha256=Ah5u_GOX5d5bR4ILufih6qyLs22IXsZ_r9xD3cb3zw0,5985
+azureml/acft/image/components/finetune/common/trainer/__init__.py,sha256=3fv1UZeGDRYic4LVNIG3T1BxyRvltJ7FefCO9QYJ1Zk,307
+azureml/acft/image/components/finetune/common/trainer/train_helper.py,sha256=ER0MBAsBCl15diskBKq19PyXBpT48Fu7iFgOXy7Kr6g,6883
 azureml/acft/image/components/finetune/defaults/__init__.py,sha256=lwuuzJJAKaTscSfrN5IK4YYV45l1Nllq1MM7CUkGx3M,329
-azureml/acft/image/components/finetune/defaults/classification_models_defaults.py,sha256=NoyWIeXGqCRGkKmdySOQWHlGkZZRWf4W9TTOszDIlHQ,3091
-azureml/acft/image/components/finetune/defaults/constants.py,sha256=M2MihYAofHs9k6NA3n0tzqs-2xxds4uZ-AIBDbl_Pqk,3507
-azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py,sha256=yOUlcDsdnLmbmm3LPTwltT38SQrMdrrOvg_ZWVenjZs,1430
-azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py,sha256=hgPHsBVbRxUZJzqUEK0yBujO-Obg7goqez6bcDv1pyM,823
-azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py,sha256=a8Halx2uj6JZuGQWDMlmEBkyTlpg6cfr_WoKyhosITE,808
-azureml/acft/image/components/finetune/defaults/task_defaults.py,sha256=2VEBUYVE8nalnRt6QjaJ3UqanxHhcP7DaM59kIe1IpM,2021
-azureml/acft/image/components/finetune/defaults/training_defaults.py,sha256=oXyJaeeTg6hMpV50exL6veIMRQTGDqqpsUApP0sBYVU,7761
+azureml/acft/image/components/finetune/defaults/constants.py,sha256=ACURRnEnrgkPDdmLg4SWkLCQQOFBRoFv7LQvW84saJE,5195
+azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py,sha256=Ci9a2npny2DDSZXOPmk40iyhVgm0llBGr-uDFT6xwh4,1163
+azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py,sha256=1fd2XwnHQXrivIy03zkL4gKAO1UI7aXw2HnOKQxYavA,756
+azureml/acft/image/components/finetune/defaults/multi_object_tracking_models_defaults.py,sha256=p6y5y2g-jWV8-h44kf3DRnwhhlbOfqUEul3lQbxvkt0,750
+azureml/acft/image/components/finetune/defaults/multiclass_classification_models_defaults.py,sha256=IiXX9hgt2WeCOgsTLpDMTLpSoeeIvdCVWwU10gOt05A,3412
+azureml/acft/image/components/finetune/defaults/multilabel_classification_models_defaults.py,sha256=c2nA-vXYLmRZi8hC0h8llMLz4c5dUwkIbxoEoUyPmYY,4006
+azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py,sha256=duZ-6Vyu2eYWraHoI_r5McRSKlTJbXO4YnNS2DFsfH4,741
+azureml/acft/image/components/finetune/defaults/task_defaults.py,sha256=w0aqnp-uCaSHRHYws-OK_BCyUhSt44jlYTRn6bngHz8,3879
+azureml/acft/image/components/finetune/defaults/training_defaults.py,sha256=qp_2jNLpxFtZHjcqtelSSs00Ky52qLl0cFjr3HpJ4kE,8777
 azureml/acft/image/components/finetune/factory/__init__.py,sha256=Ht92Ed5qLyCM4oyG7VsOAIDo-KhSxtXzeqJzFCnL8vw,333
-azureml/acft/image/components/finetune/factory/mappings.py,sha256=StW_tjTrsjhHo3cmlQNqQaEIT7iOaehAQ0HTgPAWUfk,764
-azureml/acft/image/components/finetune/factory/model_factory.py,sha256=vDw01IgHjV5a8z3gAProiSVkpeLQuBfvJYd5Hs3iuaI,2253
-azureml/acft/image/components/finetune/factory/task_definitions.py,sha256=xrpwIttCpexwQeUeq1PNURJcyKsiFtv5rqJmSK_7iPw,548
-azureml/acft/image/components/finetune/huggingface/__init__.py,sha256=iBl14XpvoQpEuXuLYgoel3QoEbV_XCJUyVE6RodoKzk,5944
+azureml/acft/image/components/finetune/factory/mappings.py,sha256=QhfonLZnoQxe7SlX1T9tqJBwcCcnW7OvGNGJPJQ6Io8,903
+azureml/acft/image/components/finetune/factory/model_factory.py,sha256=kxgNcZI12-GfisjPfVPYnIWiCU1bUiXt1PdUC_ML5RM,2312
+azureml/acft/image/components/finetune/factory/task_definitions.py,sha256=Lm4Slp0D4Ag_9lJfhNzXdMFpM39gozmZ1u2Mj23kC5s,610
+azureml/acft/image/components/finetune/huggingface/__init__.py,sha256=kVNVDW29ogrIjzoJPrZCXIvNWUU9M137dm6F-we0ns0,8297
 azureml/acft/image/components/finetune/huggingface/classification/__init__.py,sha256=zn62FtSZn05t8m69tj0WxP6XVYqKjv6ZGkbCzEkWuh0,347
-azureml/acft/image/components/finetune/huggingface/classification/data_cls.py,sha256=ZiEkUJp44dBgUWQIBipsVYhwSBPZ7cQtH3DLhZBvsKg,7964
-azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py,sha256=rNhwvyUb5H9PdxsqDT2uJKgmeEY5V51vAJXbuNwa3OE,2367
+azureml/acft/image/components/finetune/huggingface/classification/data_cls.py,sha256=VvE_VqZZNDOR-eSBWXH6mbY-eURSZrhWuC6FjuSlC84,8430
+azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py,sha256=gOe9XZrNyk5QugrVRiRzgEWTKefWysTqW3vt-p_4fEI,3231
 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py,sha256=AwfXL1apBCtLRB_HxQcvEypgzbzt5qAjbSzk5xfumDE,5178
 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py,sha256=bTnSEyJhXU9XJgLMKKieMbyNb99qbcZx490aE524Cxg,1706
 azureml/acft/image/components/finetune/huggingface/common/__init__.py,sha256=dV1ARKal1bfCgWCrBdxsbYnWi-P93vInIXCkw32IzWY,339
-azureml/acft/image/components/finetune/huggingface/common/constants.py,sha256=P2JWfLsSPUXenUOlhMoMtrCVAgKwvPSElMGfUpjTK8g,951
-azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py,sha256=Z1cV27VSvtDPBzlm6CklLhAQCL6yyEPqP_FTsRI1VbI,18943
+azureml/acft/image/components/finetune/huggingface/common/constants.py,sha256=11W4S1sPN8ysajzaWOlhobktC227NyDp-VI4M0c3QWo,1004
+azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py,sha256=DLUroJt3idN_87XM3yL4OD0eedYDtntAUorM6d9zEEA,17297
 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py,sha256=DJU_AOCFlm8r_D-7nloUhNg2WjRwdextrnprtKLFbzo,350
 azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py,sha256=b70-zfc7uxbYVpaPD8KkmsofqCRM4CaTwV1HAX14p28,8760
 azureml/acft/image/components/finetune/interfaces/__init__.py,sha256=u68Sh6HeK2tX3EWq4aLftcM84RH5fJC0I7h5mGJOsm4,265
 azureml/acft/image/components/finetune/interfaces/azml_interface.py,sha256=-N8_ryynhz94xmdTTmHLLhU1Aht35PhyYnLlmNwB3nA,10706
-azureml/acft/image/components/finetune/mmdetection/__init__.py,sha256=GspVcHM5uoSi1hjTkxnqsAFzoqZfxxxP-y-5xxPMuyI,2327
+azureml/acft/image/components/finetune/mmdetection/__init__.py,sha256=XBjKPz9a4W0P-UsNCJBLnMIpP4o6voBxsDRkEmaRnPA,7225
 azureml/acft/image/components/finetune/mmdetection/common/__init__.py,sha256=2hE4bBrLwd8UgBHayiYE1IfNgiGL7T-e-bC4fGDT4Qk,249
-azureml/acft/image/components/finetune/mmdetection/common/constants.py,sha256=GUZlQPJZ9cduoJ_7GDdKBObQqH3IMBKZHjofKu-yjNg,759
-azureml/acft/image/components/finetune/mmdetection/common/data_class.py,sha256=u_tcYFHfIXY-Zjh7V5ML9n1FMMFEyQnbBGk-95R1Psw,10253
-azureml/acft/image/components/finetune/mmdetection/common/dataset.py,sha256=1C-j_Zejv0B4f2Ys_CwIdjGVB06MLwAkA7u2G8Kga3s,8739
-azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py,sha256=8U9HcJA8D1-S4aAGqKIA6UTZuwizCmLRkv8Gt-gHZGc,1083
-azureml/acft/image/components/finetune/mmdetection/common/inference.py,sha256=_tgfaxwkaTNbQuGOQaGdJpTN8CSLlHLujGaKaD06H6k,3015
-azureml/acft/image/components/finetune/mmdetection/common/metrics.py,sha256=CytJSGTjp22N-QrDS_6PJpz9yjXNFBUcecADvttH2VM,10152
-azureml/acft/image/components/finetune/mmdetection/common/model.py,sha256=PatGaZdjp5JkQFwq9fPG2sWnUE51z6MkR7XtfMHwzWs,7374
-azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py,sha256=u8hgY4HMuN4dDUdnaJMk9ow_okoki3_wxgwwg7ok0dk,1832
-azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py,sha256=PG5Dn91CGMFPWXde1PM8QumhDy_o6Y25wjLY7AOTBs4,1784
+azureml/acft/image/components/finetune/mmdetection/common/constants.py,sha256=4RGzQJ_-Y79c0VUk5OJu4FnI9UHyDdnLP1phniCPobo,1059
+azureml/acft/image/components/finetune/mmdetection/common/data_class.py,sha256=YyWpo41IYRFzOkhAyHxAMNQkFuSOd-36Df4WAq4tsKg,9849
+azureml/acft/image/components/finetune/mmdetection/common/dataset.py,sha256=_67_EJ_Q9HrL2JmstXSEEJ4z9lUrYswj8Pcf17MAJTk,10821
+azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py,sha256=KRoRViVVbiwzyAhtbYxicxsEzr1rto8PneP0Pd31buI,1823
+azureml/acft/image/components/finetune/mmdetection/common/inference.py,sha256=pivqi3s9DQXyccs5Rsz70vY7_ZdQDPVsOFRkWFB9bAI,4146
+azureml/acft/image/components/finetune/mmdetection/common/metrics.py,sha256=CedBCn8naZoYq52V5YyPuVCliS0b7fk5urzLDwJ88jU,1932
+azureml/acft/image/components/finetune/mmdetection/common/model.py,sha256=96bSRjz9xB6ETnSTTMOZVJu6jw4KcECATEvklivZgEs,11461
+azureml/acft/image/components/finetune/mmdetection/common/model_config_rules.py,sha256=eR9MX8e49_drebjf6waHsWPbO5cuh113Uy0qxaTJ2Ds,1888
+azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py,sha256=t9KwyD83dRLQpj74f0iC4QGak3AJD6An0wWIEKmuWUc,3131
+azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py,sha256=B8yZm0eGHzp_zpNvN9d9TLnx9zU3-mIe594ob9EEgUA,1863
 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py,sha256=71dEttL5_De4UI9esPQaS80moyIqM5sZQKf8AqC6rmE,264
-azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py,sha256=U3WAKFGFQ0_LicEbjKyej1p9XqfnbAmHEpRH4qdsFC8,7724
+azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py,sha256=HhyhmCBN3p2iHhwyazPaIoks0QRNmQhGHMibOcDGwtY,9981
 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py,sha256=VT7-OMmae4eekALgF2a3PWe_xKoeTTGMg2U6ShgXDTE,259
-azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py,sha256=-67169F1UdQHgV9uizzUt0sFodkX5YAYxrzwNVDan4M,11273
+azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py,sha256=5E6HAHD9j5P_RHmlwFxbvBVck_2WXsaCYtawP_8vuy8,20894
+azureml/acft/image/components/finetune/mmtracking/__init__.py,sha256=8mYvmf5pCGDCGdROiKsf76zoJcj1S0NL3ijyWAZ5jdY,2293
+azureml/acft/image/components/finetune/mmtracking/common/__init__.py,sha256=4CO4HfSpUppBw-dWN2q1GuNXicCOKNQ_CqEMR5Rp-ik,248
+azureml/acft/image/components/finetune/mmtracking/common/constants.py,sha256=IWbBe-cGRFtV12hy8voWkL9akDzzJBTkTzuIssfYTfQ,1563
+azureml/acft/image/components/finetune/mmtracking/common/data_class.py,sha256=BXJjcBlWmmu9K6Yvfuh2F7mpJ8wzQ0Ntcu2FNQnZPWs,14240
+azureml/acft/image/components/finetune/mmtracking/common/dataset.py,sha256=c81Refam1QFF16H_wHmRr4f3CKCCxw43tvzO6XtFj8U,27756
+azureml/acft/image/components/finetune/mmtracking/common/image_metadata.py,sha256=BAzc25fVNWZ9V764sy0KXtpizgsQ-NESm3-kVnwJhCs,1082
+azureml/acft/image/components/finetune/mmtracking/common/inference.py,sha256=AFbhQWYtkVC-2pKrYjVSv0413cD5XPTCyzXB9ihqF9w,3000
+azureml/acft/image/components/finetune/mmtracking/common/metrics.py,sha256=cyPBZO0otozPj43FZ0o3B5NVmBLmvftK0VVZQMT9x4U,1911
+azureml/acft/image/components/finetune/mmtracking/common/model.py,sha256=jRzUltx_VkxBd-ZL9Vl9HxSjFB3igoMITNBqH1p1YRE,7291
+azureml/acft/image/components/finetune/mmtracking/common/trainer_arguments.py,sha256=DdgkarpvlERajovPVusTVvmxhjuYyj6Ygtv_SImca6M,780
+azureml/acft/image/components/finetune/mmtracking/common/trainer_classes.py,sha256=E5G7nGdvRAmZ6Xwd2ZMEcu0Q-ctRmmzp8UlM8bgkKs0,1767
+azureml/acft/image/components/finetune/mmtracking/mot/__init__.py,sha256=R4tnY3kgiMAW5h1ERVfBCCjVQpyJPPK6Q4jZxqBGwAo,263
+azureml/acft/image/components/finetune/mmtracking/mot/model_wrapper.py,sha256=ZNcr09-5EmkP4y9TbMwrCv1N_D5FMuQkoXvBmnbJIws,18350
 azureml/acft/image/components/model_selector/__init__.py,sha256=Beo_K6DsSl7BGWXFdQGv9B8qo9oY-qWKJmNJvmsvZpo,321
-azureml/acft/image/components/model_selector/component.py,sha256=uzsF7n564NFG1dDjvN-NiIVTZL_ERtoLUqyEmlik0dw,17200
-azureml/acft/image/components/model_selector/constants.py,sha256=pjQicLRnDP0PuuKelIHyOxMpfjZm1m7Y2MJmj8caV4E,851
-azureml_acft_image_components-0.0.9.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_acft_image_components-0.0.9.dist-info/METADATA,sha256=ipgHeZQMnlHgvABnSUML8CMB7hYB9ydRYgeOBn3uoMA,1315
-azureml_acft_image_components-0.0.9.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-azureml_acft_image_components-0.0.9.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
-azureml_acft_image_components-0.0.9.dist-info/RECORD,,
+azureml/acft/image/components/model_selector/component.py,sha256=NvLdstBpe6fIKxgV2ec3mSVpU2_0ewddlgkg7sF6Lm8,27217
+azureml/acft/image/components/model_selector/constants.py,sha256=_QlOtK6V9VulE8lTJG_Krw5rHHmek3z8lpoRS5lPzEo,1289
+azureml_acft_image_components-47.0.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_acft_image_components-47.0.0.dist-info/METADATA,sha256=2Sg6ujj9gv5ihk3_CKMr6msiFARU_PUd6XqaTeJBXQk,1469
+azureml_acft_image_components-47.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+azureml_acft_image_components-47.0.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml_acft_image_components-47.0.0.dist-info/RECORD,,
```

