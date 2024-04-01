# Comparing `tmp/azureml_acft_common_components-0.0.9-py3-none-any.whl.zip` & `tmp/azureml_acft_common_components-47.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,78 +1,87 @@
-Zip file size: 162262 bytes, number of entries: 76
--rw-rw-rw-  2.0 fat      251 b- defN 23-May-17 17:31 azureml/__init__.py
--rw-rw-rw-  2.0 fat      317 b- defN 23-May-17 17:31 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat     1226 b- defN 23-May-17 17:31 azureml/acft/common_components/__init__.py
--rw-rw-rw-  2.0 fat       34 b- defN 23-May-17 17:36 azureml/acft/common_components/_version.py
--rw-rw-rw-  2.0 fat      309 b- defN 23-May-17 17:31 azureml/acft/common_components/image/__init__.py
--rw-rw-rw-  2.0 fat      337 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/__init__.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/__init__.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/common/__init__.py
--rw-rw-rw-  2.0 fat    27157 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/common/classification_utils.py
--rw-rw-rw-  2.0 fat     7505 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/common/constants.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/common/transforms.py
--rw-rw-rw-  2.0 fat      210 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/io/__init__.py
--rw-rw-rw-  2.0 fat      398 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/io/read/__init__.py
--rw-rw-rw-  2.0 fat     4953 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/io/read/dataloader.py
--rw-rw-rw-  2.0 fat    22521 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/io/read/dataset_wrappers.py
--rw-rw-rw-  2.0 fat     5611 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/io/read/utils.py
--rw-rw-rw-  2.0 fat      429 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/models/__init__.py
--rw-rw-rw-  2.0 fat    11546 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/classification/models/base_model_wrapper.py
--rw-rw-rw-  2.0 fat      331 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/__init__.py
--rw-rw-rw-  2.0 fat     1903 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/aml_dataset_base_wrapper.py
--rw-rw-rw-  2.0 fat    10436 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py
--rw-rw-rw-  2.0 fat     2025 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/average_meter.py
--rw-rw-rw-  2.0 fat     2229 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/base_model_factory.py
--rw-rw-rw-  2.0 fat     1231 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/base_model_settings.py
--rw-rw-rw-  2.0 fat    22490 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/constants.py
--rw-rw-rw-  2.0 fat     2826 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/data_utils.py
--rw-rw-rw-  2.0 fat     3200 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/dataloaders.py
--rw-rw-rw-  2.0 fat    18973 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/dataset_helper.py
--rw-rw-rw-  2.0 fat    21069 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/distributed_utils.py
--rw-rw-rw-  2.0 fat      672 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/errors.py
--rw-rw-rw-  2.0 fat     2379 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/exceptions.py
--rw-rw-rw-  2.0 fat     2528 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/logging_utils.py
--rw-rw-rw-  2.0 fat    25060 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/model_export_utils.py
--rw-rw-rw-  2.0 fat    14782 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/parameters.py
--rw-rw-rw-  2.0 fat    10346 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/prediction_dataset.py
--rw-rw-rw-  2.0 fat    37090 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/pretrained_model_utilities.py
--rw-rw-rw-  2.0 fat     3033 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/sku_validation.py
--rw-rw-rw-  2.0 fat     9850 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/system_meter.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/tiling_dataset_element.py
--rw-rw-rw-  2.0 fat     6591 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/tiling_utils.py
--rw-rw-rw-  2.0 fat     1039 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/torch_utils.py
--rw-rw-rw-  2.0 fat    65435 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/common/utils.py
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/__init__.py
--rw-rw-rw-  2.0 fat      311 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/__init__.py
--rw-rw-rw-  2.0 fat     9651 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/augmentations.py
--rw-rw-rw-  2.0 fat     7382 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/boundingbox.py
--rw-rw-rw-  2.0 fat     3068 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/coco_eval_box_converter.py
--rw-rw-rw-  2.0 fat    11008 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py
--rw-rw-rw-  2.0 fat    11945 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/masktools.py
--rw-rw-rw-  2.0 fat    27533 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/object_detection_utils.py
--rw-rw-rw-  2.0 fat     4995 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/parameters.py
--rw-rw-rw-  2.0 fat    25959 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/common/tiling_helper.py
--rw-rw-rw-  2.0 fat      306 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/__init__.py
--rw-rw-rw-  2.0 fat     4664 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/dataset_wrappers.py
--rw-rw-rw-  2.0 fat    39856 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py
--rw-rw-rw-  2.0 fat     6162 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/loaders.py
--rw-rw-rw-  2.0 fat    11899 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py
--rw-rw-rw-  2.0 fat     5037 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/tiling_distributed_sampler.py
--rw-rw-rw-  2.0 fat    11332 b- defN 23-May-17 17:31 azureml/acft/common_components/image/runtime_common/object_detection/data/utils.py
--rw-rw-rw-  2.0 fat      325 b- defN 23-May-17 17:31 azureml/acft/common_components/model_selector/__init__.py
--rw-rw-rw-  2.0 fat     7131 b- defN 23-May-17 17:31 azureml/acft/common_components/model_selector/component.py
--rw-rw-rw-  2.0 fat      854 b- defN 23-May-17 17:31 azureml/acft/common_components/model_selector/constants.py
--rw-rw-rw-  2.0 fat      236 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/__init__.py
--rw-rw-rw-  2.0 fat    12226 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/logging_utils.py
--rw-rw-rw-  2.0 fat     1649 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
--rw-rw-rw-  2.0 fat      226 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/error_handling/__init__.py
--rw-rw-rw-  2.0 fat     6864 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/error_handling/error_definitions.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/error_handling/error_strings.py
--rw-rw-rw-  2.0 fat     3650 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/error_handling/exceptions.py
--rw-rw-rw-  2.0 fat     5786 b- defN 23-May-17 17:31 azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
--rw-rw-rw-  2.0 fat      859 b- defN 23-May-17 17:36 azureml_acft_common_components-0.0.9.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1271 b- defN 23-May-17 17:36 azureml_acft_common_components-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-17 17:36 azureml_acft_common_components-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-17 17:36 azureml_acft_common_components-0.0.9.dist-info/namespace_packages.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 17:36 azureml_acft_common_components-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9959 b- defN 23-May-17 17:36 azureml_acft_common_components-0.0.9.dist-info/RECORD
-76 files, 592481 bytes uncompressed, 145084 bytes compressed:  75.5%
+Zip file size: 179706 bytes, number of entries: 85
+-rw-rw-rw-  2.0 fat      251 b- defN 24-Mar-22 10:04 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      317 b- defN 24-Mar-22 10:04 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat     1314 b- defN 24-Mar-22 10:04 azureml/acft/common_components/__init__.py
+-rw-rw-rw-  2.0 fat       36 b- defN 24-Mar-22 10:09 azureml/acft/common_components/_version.py
+-rw-rw-rw-  2.0 fat      309 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/__init__.py
+-rw-rw-rw-  2.0 fat      337 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/common/__init__.py
+-rw-rw-rw-  2.0 fat    27157 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/common/classification_utils.py
+-rw-rw-rw-  2.0 fat     7505 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/common/constants.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/common/transforms.py
+-rw-rw-rw-  2.0 fat      210 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/io/__init__.py
+-rw-rw-rw-  2.0 fat      398 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/io/read/__init__.py
+-rw-rw-rw-  2.0 fat     4953 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/io/read/dataloader.py
+-rw-rw-rw-  2.0 fat    22521 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/io/read/dataset_wrappers.py
+-rw-rw-rw-  2.0 fat     5611 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/io/read/utils.py
+-rw-rw-rw-  2.0 fat      429 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/models/__init__.py
+-rw-rw-rw-  2.0 fat    11546 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/classification/models/base_model_wrapper.py
+-rw-rw-rw-  2.0 fat      331 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/__init__.py
+-rw-rw-rw-  2.0 fat     1903 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/aml_dataset_base_wrapper.py
+-rw-rw-rw-  2.0 fat    11717 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py
+-rw-rw-rw-  2.0 fat     2025 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/average_meter.py
+-rw-rw-rw-  2.0 fat     2229 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/base_model_factory.py
+-rw-rw-rw-  2.0 fat     1231 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/base_model_settings.py
+-rw-rw-rw-  2.0 fat    22490 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/constants.py
+-rw-rw-rw-  2.0 fat     2826 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/data_utils.py
+-rw-rw-rw-  2.0 fat     3200 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/dataloaders.py
+-rw-rw-rw-  2.0 fat    19103 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/dataset_helper.py
+-rw-rw-rw-  2.0 fat    21069 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/distributed_utils.py
+-rw-rw-rw-  2.0 fat      672 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/errors.py
+-rw-rw-rw-  2.0 fat     2379 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/exceptions.py
+-rw-rw-rw-  2.0 fat     2528 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/logging_utils.py
+-rw-rw-rw-  2.0 fat    25060 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/model_export_utils.py
+-rw-rw-rw-  2.0 fat    14782 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/parameters.py
+-rw-rw-rw-  2.0 fat    10346 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/prediction_dataset.py
+-rw-rw-rw-  2.0 fat    37090 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/pretrained_model_utilities.py
+-rw-rw-rw-  2.0 fat     3033 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/sku_validation.py
+-rw-rw-rw-  2.0 fat     9850 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/system_meter.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/tiling_dataset_element.py
+-rw-rw-rw-  2.0 fat     6591 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/tiling_utils.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/torch_utils.py
+-rw-rw-rw-  2.0 fat    66311 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/common/utils.py
+-rw-rw-rw-  2.0 fat      302 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/__init__.py
+-rw-rw-rw-  2.0 fat      311 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/__init__.py
+-rw-rw-rw-  2.0 fat     9651 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/augmentations.py
+-rw-rw-rw-  2.0 fat     7382 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/boundingbox.py
+-rw-rw-rw-  2.0 fat     3068 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/coco_eval_box_converter.py
+-rw-rw-rw-  2.0 fat    11041 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py
+-rw-rw-rw-  2.0 fat    11945 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/masktools.py
+-rw-rw-rw-  2.0 fat    27533 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/object_detection_utils.py
+-rw-rw-rw-  2.0 fat     4995 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/parameters.py
+-rw-rw-rw-  2.0 fat    25959 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/common/tiling_helper.py
+-rw-rw-rw-  2.0 fat      306 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/__init__.py
+-rw-rw-rw-  2.0 fat     4664 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/dataset_wrappers.py
+-rw-rw-rw-  2.0 fat    40176 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py
+-rw-rw-rw-  2.0 fat     6162 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/loaders.py
+-rw-rw-rw-  2.0 fat    13798 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py
+-rw-rw-rw-  2.0 fat     5037 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/tiling_distributed_sampler.py
+-rw-rw-rw-  2.0 fat    11332 b- defN 24-Mar-22 10:04 azureml/acft/common_components/image/runtime_common/object_detection/data/utils.py
+-rw-rw-rw-  2.0 fat      325 b- defN 24-Mar-22 10:04 azureml/acft/common_components/model_selector/__init__.py
+-rw-rw-rw-  2.0 fat    26691 b- defN 24-Mar-22 10:04 azureml/acft/common_components/model_selector/component.py
+-rw-rw-rw-  2.0 fat     3499 b- defN 24-Mar-22 10:04 azureml/acft/common_components/model_selector/constants.py
+-rw-rw-rw-  2.0 fat      236 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1075 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/arg_utils.py
+-rw-rw-rw-  2.0 fat     5300 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/callbacks.py
+-rw-rw-rw-  2.0 fat     3618 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/constants.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/hf_hub_utils.py
+-rw-rw-rw-  2.0 fat     3623 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/license_utils.py
+-rw-rw-rw-  2.0 fat    15400 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/logging_utils.py
+-rw-rw-rw-  2.0 fat     1358 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/mlflow_utils.py
+-rw-rw-rw-  2.0 fat     2260 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/run_utils.py
+-rw-rw-rw-  2.0 fat     3742 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
+-rw-rw-rw-  2.0 fat      529 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/torch_utils.py
+-rw-rw-rw-  2.0 fat      700 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/transformer_utils.py
+-rw-rw-rw-  2.0 fat      226 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/error_handling/__init__.py
+-rw-rw-rw-  2.0 fat     8410 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/error_handling/error_definitions.py
+-rw-rw-rw-  2.0 fat     4677 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/error_handling/error_strings.py
+-rw-rw-rw-  2.0 fat     4588 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/error_handling/exceptions.py
+-rw-rw-rw-  2.0 fat     8013 b- defN 24-Mar-22 10:04 azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
+-rw-rw-rw-  2.0 fat      859 b- defN 24-Mar-22 10:09 azureml_acft_common_components-47.0.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1550 b- defN 24-Mar-22 10:09 azureml_acft_common_components-47.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 10:09 azureml_acft_common_components-47.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-22 10:09 azureml_acft_common_components-47.0.0.dist-info/namespace_packages.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-22 10:09 azureml_acft_common_components-47.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    10939 b- defN 24-Mar-22 10:09 azureml_acft_common_components-47.0.0.dist-info/RECORD
+85 files, 651783 bytes uncompressed, 160910 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -183,20 +183,47 @@
 
 Filename: azureml/acft/common_components/model_selector/constants.py
 Comment: 
 
 Filename: azureml/acft/common_components/utils/__init__.py
 Comment: 
 
+Filename: azureml/acft/common_components/utils/arg_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/callbacks.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/constants.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/hf_hub_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/license_utils.py
+Comment: 
+
 Filename: azureml/acft/common_components/utils/logging_utils.py
 Comment: 
 
+Filename: azureml/acft/common_components/utils/mlflow_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/run_utils.py
+Comment: 
+
 Filename: azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
 Comment: 
 
+Filename: azureml/acft/common_components/utils/torch_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/utils/transformer_utils.py
+Comment: 
+
 Filename: azureml/acft/common_components/utils/error_handling/__init__.py
 Comment: 
 
 Filename: azureml/acft/common_components/utils/error_handling/error_definitions.py
 Comment: 
 
 Filename: azureml/acft/common_components/utils/error_handling/error_strings.py
@@ -204,26 +231,26 @@
 
 Filename: azureml/acft/common_components/utils/error_handling/exceptions.py
 Comment: 
 
 Filename: azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.9.dist-info/LICENSE.txt
+Filename: azureml_acft_common_components-47.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.9.dist-info/METADATA
+Filename: azureml_acft_common_components-47.0.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.9.dist-info/WHEEL
+Filename: azureml_acft_common_components-47.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.9.dist-info/namespace_packages.txt
+Filename: azureml_acft_common_components-47.0.0.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.9.dist-info/top_level.txt
+Filename: azureml_acft_common_components-47.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.9.dist-info/RECORD
+Filename: azureml_acft_common_components-47.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/acft/common_components/__init__.py

```diff
@@ -7,30 +7,33 @@
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)  # type: ignore
 
 import sys
 
 from azureml.automl.core.shared import logging_utilities, log_server
 
 from .model_selector.component import ModelSelector
-from .model_selector.constants import ModelSelectorConstants, ModelSelectorDefaults
+from .model_selector.constants import ModelSelectorConstants, ModelSelectorDefaults, ModelSelectorAPIConstants
 
 from .utils.logging_utils import set_logging_parameters, get_logger_app, LoggingLiterals
 
 try:
     from ._version import ver as VERSION, selfver as SELFVERSION
     __version__ = VERSION
 except ImportError:
     VERSION = '0.0.0+dev'
     SELFVERSION = VERSION
     __version__ = VERSION
 
+PROJECT_NAME = __name__
+
 __all__ = [
     "ModelSelector",
     "ModelSelectorConstants",
     "ModelSelectorDefaults",
+    "ModelSelectorAPIConstants",
     "set_logging_parameters",
     "get_logger_app",
     "LoggingLiterals",
 ]
 
 # Mark this package as being allowed to log certain built-in types
 module = sys.modules[__name__]
```

## azureml/acft/common_components/_version.py

```diff
@@ -1,2 +1,2 @@
-ver = "0.0.9"
-selfver = "0.0.9"
+ver = "47.0.0"
+selfver = "47.0.0"
```

## azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py

```diff
@@ -17,20 +17,21 @@
 from azureml.acft.common_components.image.runtime_common.common.constants import ArtifactLiterals, \
     SettingsLiterals, CommonSettings
 from azureml.acft.common_components.image.runtime_common.common.exceptions import \
     AutoMLVisionValidationException, AutoMLVisionRuntimeUserException
 from azureml.acft.common_components.image.runtime_common.common.model_export_utils import prepare_model_export
 from azureml.acft.common_components.image.runtime_common.common.torch_utils import intersect_dicts
 from azureml.acft.common_components.image.runtime_common.common.utils import _set_train_run_properties, \
-    _distill_run_from_experiment
+    _distill_run_from_experiment, should_log_metrics_to_parent
 from azureml.acft.common_components.image.runtime_common.object_detection.common.constants import ModelNames
 from azureml.acft.common_components.image.runtime_common.object_detection.models.object_detection_model_wrappers \
     import BaseObjectDetectionModelWrapper
 from azureml.core.run import Run
 from typing import Union, Any, Dict, Optional, List
+from azureml.exceptions import AzureMLAggregatedException
 
 logger = get_logger_app(__name__)
 
 
 def write_artifacts(model_wrapper: Union[BaseObjectDetectionModelWrapper, Module],
                     best_model_weights: Dict[str, Any], labels: List[str],
                     output_dir: str, run: Run, best_metric: float,
@@ -79,22 +80,49 @@
     label_file_path = os.path.join(output_dir, ArtifactLiterals.LABEL_FILE_NAME)
     with open(label_file_path, 'w') as f:
         json.dump(labels, f)
 
     _set_train_run_properties(run, model_wrapper.model_name, best_metric)
 
     folder_name = os.path.basename(output_dir)
-    run.upload_folder(name=folder_name, path=output_dir)
+    try:
+        run.upload_folder(name=folder_name, path=output_dir)
+    except AzureMLAggregatedException as e:
+        if "Resource Conflict" in e.message:
+            parsed_message = e.message.replace("UserError: ", "")
+            logger.warning("Resource conflict when uploading artifacts to run.")
+            logger.warning(parsed_message)
+        else:
+            raise
+    parent_run = should_log_metrics_to_parent(run)
+    if parent_run:
+        try:
+            parent_run.upload_folder(name=folder_name, path=output_dir)
+        except AzureMLAggregatedException as e:
+            if "Resource Conflict" in e.message:
+                parsed_message = e.message.replace("UserError: ", "")
+                logger.warning("Resource conflict when uploading artifacts to parent run.")
+                logger.warning(parsed_message)
+            else:
+                raise
     model_settings.update(model_wrapper.inference_settings)
-    prepare_model_export(run=run,
-                         output_dir=output_dir,
-                         task_type=task_type,
-                         model_settings=model_settings,
-                         save_as_mlflow=save_as_mlflow,
-                         is_yolo=is_yolo)
+    try:
+        prepare_model_export(run=run,
+                             output_dir=output_dir,
+                             task_type=task_type,
+                             model_settings=model_settings,
+                             save_as_mlflow=save_as_mlflow,
+                             is_yolo=is_yolo)
+    except AzureMLAggregatedException as e:
+        if "Resource Conflict" in e.message:
+            parsed_message = e.message.replace("UserError: ", "")
+            logger.warning("Resource conflict when preparing model export.")
+            logger.warning(parsed_message)
+        else:
+            raise
 
 
 def upload_model_checkpoint(run: Run, model_location: str) -> None:
     """Uploads the model checkpoints to workspace.
 
     :param run: azureml run object
     :type run: azureml.core.Run
```

## azureml/acft/common_components/image/runtime_common/common/dataset_helper.py

```diff
@@ -7,14 +7,15 @@
 import json
 import os
 import shutil
 import tempfile
 import time
 import uuid
 from typing import Any, List, cast
+from urllib.parse import unquote
 from azureml.data.abstract_dataset import AbstractDataset
 
 import pandas
 
 import azureml.dataprep as dprep
 
 from azureml.acft.common_components import get_logger_app
@@ -132,15 +133,16 @@
         :param image_file_name: The image file name with path within the datastore.
         :type image_file_name: str
         :param confidence: Label confidence values between 0.0 and 1.0
         :type confidence: List[float]
         :param label: The label names.
         :type label: List[str]
         """
-        image_full_path = AmlDatasetHelper.DATASTORE_PREFIX + image_file_name
+        # unquote to convert the replace(%3A and %2F ...) in the url
+        image_full_path = AmlDatasetHelper.DATASTORE_PREFIX + unquote(image_file_name)
 
         fw.write(
             json.dumps(
                 {
                     AmlDatasetHelper.DEFAULT_IMAGE_COLUMN_NAME: image_full_path,
                     AmlDatasetHelper.DEFAULT_LABEL_CONFIDENCE_COLUMN_NAME: confidence,
                     AmlDatasetHelper.DEFAULT_LABEL_COLUMN_NAME: label
@@ -304,15 +306,15 @@
             # The first call (using on_error="fail") raises an exception if there's an error in the Dataset.
             # We can't use on_error="fail" together with extended_types=True because if extended_types=True is
             # part of the call, the on_error="fail" parameter is ignored. The extended_types=True parameter
             # is helpful because the resulting DataFrame contains structured information about the Datastore
             # and handler protocol (used below).)
             ds._dataflow.to_pandas_dataframe(on_error="fail")
             df = ds._dataflow.to_pandas_dataframe(extended_types=True)
-        except (ExecutionError, UserErrorException) as e:
+        except (ExecutionError, UserErrorException, ValidationError) as e:
             raise AutoMLVisionDataException(
                 f"Could not convert the dataset to a pandas data frame. "
                 f"Please check the logs for more details. Error Code: {e}")
         AmlDatasetHelper._validate_image_column(ds, image_column_name)
         # Find all datastores referenced by the dataset.
         datastore_names = set()
         for image_stream_info in df[image_column_name]:
```

## azureml/acft/common_components/image/runtime_common/common/utils.py

```diff
@@ -688,14 +688,36 @@
         if metric_name_stem not in METRICS_WITH_CUSTOM_LOGGING:
             if is_verbose:
                 azureml_run.log_row("verbose_metrics", metric_name=metric_name, value=value)
             else:
                 azureml_run.log(metric_name, value)
 
 
+def should_log_metrics_to_parent(run: Run) -> Run:
+    """
+    Log metrics to the run history if a run is a pipeline job.
+
+    :param run: The run object.
+    :type run: azureml.core.run
+    :return: Parent run if we should log else None.
+    :rtype: azureml.core.run
+    """
+
+    # Get the parent run id and check if its a pipeline run.
+    # If pipeline run, log all metrics to parent pipeline as well.
+    parent_run = run.parent
+    child_run = None
+    while parent_run and (parent_run.type == "azureml.PipelineRun"
+                          or parent_run.type == "azureml.StepRun"):
+        child_run = parent_run
+        parent_run = parent_run.parent
+    logger.info("Logging to run: {}".format(child_run))
+    return child_run
+
+
 def log_detailed_object_detection_metrics(
     metrics: Dict[str, Any], azureml_run: Run, class_names: List[str] = []
 ) -> None:
     """
     Log detailed metrics for object detection to the run history of a run.
 
     The detailed metrics are the per label, image level and confusion matrix metrics.
@@ -732,17 +754,21 @@
 
         if metric_name_stem == MetricsLiterals.CONFUSION_MATRICES_PER_SCORE_THRESHOLD:
             confusion_matrices_per_score_threshold = metrics[metric_name]
 
             # Go through sorted score thresholds and log the corresponding confusion matrices.
             sorted_score_thresholds = sorted(confusion_matrices_per_score_threshold.keys())
             for st in sorted_score_thresholds:
+                # Skip empty confusion matrices.
+                cm = confusion_matrices_per_score_threshold[st]
+                if len(cm) == 0:
+                    continue
+
                 # Format the confusion matrix in scikit format, ie append a row to make it square and add a class. The
                 # matrix ends up being (C+1)x(C+1), with the last class called 'Missed'.
-                cm = confusion_matrices_per_score_threshold[st]
                 fcm = {
                     "schema_type": "confusion_matrix",
                     "schema_version": "1.0.0",
                     "data": {
                         "class_labels": class_names + [MISSED_CLASS_NAME],
                         "matrix": cm + [[NO_VALUE for _ in range(len(cm[0]))]]
                     }
```

## azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py

```diff
@@ -45,14 +45,15 @@
     IMAGE_URL = "imageUrl"
     IMAGE_DETAILS = "imageDetails"
     IMAGE_LABEL = "label"
     CLASS_LABEL = "label"
     WIDTH = "width"
     HEIGHT = "height"
     POLYGON = "polygon"
+    INSTANCE_ID = "instance_id"
 
 
 class ModelNames:
     """String names for models."""
     FASTER_RCNN_RESNET152_FPN = "fasterrcnn_resnet152_fpn"
     FASTER_RCNN_RESNET101_FPN = "fasterrcnn_resnet101_fpn"
     FASTER_RCNN_RESNET50_FPN = "fasterrcnn_resnet50_fpn"
```

## azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py

```diff
@@ -814,14 +814,20 @@
             image_elements.add(image_element)
             self._annotations[image_element].extend(cur_img_object_infos)
             object_classes.update(cur_object_classes)
 
         if not image_elements:
             raise AutoMLVisionDataException("All annotations provided are ill-formed.", has_pii=False)
 
+        # Check that at least an image in the dataset has at least an object.
+        if num_background_images == len(image_elements):
+            raise AutoMLVisionDataException(
+                "No objects in dataset. Please ensure that at least one image has one or more objects.", has_pii=False
+            )
+
         # Log number of background images.
         logger.info(f"{num_background_images} background images.")
 
         self._object_classes, self._image_elements, self._class_to_index_map, self._labels = \
             self._prepare_images_and_labels(image_elements, self._annotations, object_classes,
                                             self._use_bg_label, self._label_compute_func)
         self._generate_tile_elements()
```

## azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py

```diff
@@ -275,7 +275,56 @@
         if invalid_segment_indices:
             logger.warning(f"Removed {len(invalid_segment_indices)} invalid segments from polygon.")
             self._update_box_percentages_from_normalized_mask_poly()
             # depending on the model, this will be overridden by fill_box_properties
             self._bounding_box = [self._label,
                                   self._x0_percentage, self._y0_percentage,
                                   self._x1_percentage, self._y1_percentage]
+
+
+class VideoObjectAnnotation(ObjectAnnotation):
+    """Class that contains all of the information associated with
+    a single bounding box in a video frame."""
+
+    _instance_id: Optional[int] = None
+
+    def _init_labels(self, labels):
+        super()._init_labels(labels)
+        has_valid_track_id = DatasetFieldLabels.INSTANCE_ID in labels and \
+            isinstance(labels[DatasetFieldLabels.INSTANCE_ID], int)
+
+        if not has_valid_track_id:
+            raise AutoMLVisionDataException("Found invalid type. "
+                                            "Expected instance_id in labels to be an integer.", has_pii=False)
+
+        self._instance_id = labels[DatasetFieldLabels.INSTANCE_ID]
+
+    @property
+    def instance_id(self):
+        """Get bounding box instance id
+
+        :return: Instance id for bounding box object
+        :rtype: str
+        """
+        return self._instance_id
+
+    def _validate(self):
+        """Check if the annotation is a valid one. we are overriding this function for od,
+        because it is okay for boxes to be out of bounds in video scenario.
+
+        :return: Valid or not
+        :rtype: bool
+        """
+        if self._normalized_mask_poly and self._normalized_mask_poly[0]:
+            self._remove_invalid_segments_from_normalized_mask_poly()
+            # Invalid if polygon is empty after removing invalid segments.
+            if bool(self._normalized_mask_poly) is False:
+                return False
+
+        # Invalid if masks is required, and polygon is empty after removing invalid segments.
+        if self._masks_required and bool(self._normalized_mask_poly) is False:
+            return False
+
+        valid_normalized_bbox = \
+            self._x0_percentage < self._x1_percentage and \
+            self._y0_percentage < self._y1_percentage
+        return valid_normalized_bbox
```

## azureml/acft/common_components/model_selector/component.py

```diff
@@ -2,57 +2,89 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """For model selector component."""
 
 import json
 import os
 import shutil
+import random
+import time
+import yaml
 from pathlib import Path
-from typing import Union
-
+from typing import Union, Callable, List
 from azureml._common._error_definition.azureml_error import AzureMLError
-
-from azureml.acft.common_components.utils.error_handling.error_definitions import InvalidMlflowModelFormat, \
-    ModelInputEmpty
-from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
+from azureml.acft.common_components.utils.error_handling.error_definitions import (
+    ModelInputEmpty, ACFTSystemError, ACFTUserError)
+from azureml.acft.common_components.utils.error_handling.exceptions import (
+    ACFTValidationException,
+    ACFTSystemException,
+)
 from azureml.acft.common_components.utils.logging_utils import get_logger_app
+from azureml.acft.common_components.utils.constants import MlflowMetaConstants
 from .constants import (
+    ModelRepositoryURLs,
     ModelSelectorConstants,
-    ModelSelectorDefaults
+    ModelSelectorDefaults,
+    ModelSelectorAPIConstants,
+    ModelFamily,
+    RunDetailsConstants
 )
+from ..utils.hf_hub_utils import check_if_model_present_in_hf_hub
+from ..utils.license_utils import save_license_file
+from azureml.core.run import Run
+import requests
+from azureml.dataprep.rslex import Copier, PyIfDestinationExists, PyLocationInfo
+from azureml.dataprep.api._rslex_executor import ensure_rslex_environment
 
 logger = get_logger_app(__name__)
 
 
 class ModelSelector:
     """Model selector class to select the model and store the arguments to json file."""
     def __init__(
         self,
         pytorch_model: str = None,
         mlflow_model: str = None,
         model_name: str = None,
         output_dir: str = None,
+        model_family: str = None,
+        download_from_source: bool = False,
+        unsupported_model_list: List[str] = [],
         **kwargs,
     ) -> None:
         """Default implementation for model selector. Override the functions for custom implementation.
 
         :param pytorch_model: asset path of pytorch model, defaults to None
         :type pytorch_model: str, optional
         :param mlflow_model: asset path of mlflow model, defaults to None
         :type mlflow_model: str, optional
         :param model_name: model name from the framework (i.e., HF), defaults to None
         :type model_name: str, optional
         :param output_dir: path to store arguments and model, defaults to None
         :type output_dir: str, optional
+        :param model_family: model family, defaults to None
+        :type model_family: str, optional
+        :param unsupported_model_list: list of blocked models used to validate model name, defaults to None
+        :type unsupported_model_list: List[str], optional
         """
         self.pytorch_model = pytorch_model
         self.mlflow_model = mlflow_model
         self.output_dir = output_dir
         self.model_name = model_name
         self.keyword_arguments = kwargs
+        self.model_family = model_family
+        self.download_from_source = download_from_source
+        self.unsupported_model_list = unsupported_model_list
+        self.base_model_asset_id = None
+        self.metadata = {}
+        self.model_through_input_port = self.pytorch_model or self.mlflow_model
+        if self.model_through_input_port:
+            is_mlflow_model = self.mlflow_model is not None
+            self.base_model_asset_id = self.get_model_asset_id(is_mlflow_model=is_mlflow_model)
+            logger.info(f"asset id of input model: {self.base_model_asset_id}")
 
     def _download_pytorch_model_from_registry(self) -> None:
         """Download pytorch model from AzureML registry"""
         model_path = os.path.join(
             self.output_dir, ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY
         )
         ModelSelector._copy_directories(self.pytorch_model, model_path)
@@ -66,22 +98,65 @@
             self.output_dir, ModelSelectorDefaults.MLFLOW_MODEL_DIRECTORY
         )
         ModelSelector.convert_mlflow_model_to_pytorch_model(self.mlflow_model, Path(model_path))
         logger.info(
             f"Downloaded mlflow model from {self.mlflow_model} to {model_path}."
         )
 
+    def _fetch_metadata(self) -> None:
+        """ fetch metadata from i/p model. """
+        if self.mlflow_model:
+            model_path = os.path.join(
+                self.output_dir, ModelSelectorDefaults.MLFLOW_MODEL_DIRECTORY
+            )
+            mlmodel_path = os.path.join(model_path, ModelSelectorConstants.MLMODEL)
+            try:
+                with open(mlmodel_path, "r") as f:
+                    yaml_dict = yaml.safe_load(f)
+                self.metadata = yaml_dict.get("metadata", {})
+                logger.info(f"Fetched metadata from {ModelSelectorConstants.MLMODEL}: {self.metadata}")
+            except Exception as e:
+                logger.warning(f"Failed while fetching metadata from {ModelSelectorConstants.MLMODEL}\
+                               with err: {str(e)}")
+        elif self.pytorch_model:
+            model_path = os.path.join(
+                self.output_dir, ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY
+            )
+            model_metadata_file = os.path.join(model_path,
+                                               ModelSelectorDefaults.MODEL_METADATA_PATH)
+            if os.path.isfile(model_metadata_file):
+                with open(model_metadata_file, "r") as f:
+                    self.metadata = json.load(f)
+                    logger.info(f"Fetched metadata from {model_metadata_file} file: {self.metadata}")
+            else:
+                logger.warning("unable to fetch metadata from the model provided through the"
+                               f"input port since {ModelSelectorDefaults.MODEL_METADATA_PATH} is not found")
+
+        if not self.model_name:
+            if MlflowMetaConstants.BASE_MODEL_NAME in self.metadata:
+                self.model_name = self.metadata.get(MlflowMetaConstants.BASE_MODEL_NAME)
+            else:
+                self.model_name = self.metadata.get(ModelSelectorConstants.MODEL_NAME, None)
+
+        if ModelSelectorConstants.BASE_MODEL_ASSET_ID not in self.metadata and self.base_model_asset_id:
+            self.metadata.update({ModelSelectorConstants.BASE_MODEL_ASSET_ID : self.base_model_asset_id})
+        if self.model_name and MlflowMetaConstants.BASE_MODEL_NAME not in self.metadata:
+            self.metadata.update({MlflowMetaConstants.BASE_MODEL_NAME : self.model_name})
+
+        return
+
     def _prepare_and_logs_arguments(self) -> None:
         """Update the keyword arguments (if present) with required key-val items and
         Store the model selector arguments to json file.
         """
         arguments = {
             ModelSelectorConstants.MLFLOW_MODEL_PATH: self.mlflow_model,
             ModelSelectorConstants.PYTORCH_MODEL_PATH: self.pytorch_model,
             ModelSelectorConstants.MODEL_NAME: self.model_name,
+            ModelSelectorConstants.MODEL_METADATA: self.metadata
         }
 
         if self.keyword_arguments:
             self.keyword_arguments.update(arguments)
         else:
             self.keyword_arguments = arguments
 
@@ -103,14 +178,30 @@
         :type asset_path: str
         :param destination: destination path
         :type destination: str
         """
         os.makedirs(destination, exist_ok=True)
         shutil.copytree(asset_path, destination, dirs_exist_ok=True)
 
+    @staticmethod
+    def flatten_and_copy_directories(src_dir, dest_dir):
+        """Recursively copy from source to destination
+
+        :param src_dir: source directory path
+        :type asset_path: str
+        :param dest_dir: destination path
+        :type dest_dir: str
+        """
+        for subdir in os.listdir(src_dir):
+            subdir_or_file = os.path.join(src_dir, subdir)
+            if os.path.isdir(subdir_or_file):
+                ModelSelector.flatten_and_copy_directories(subdir_or_file, dest_dir)
+            else:
+                shutil.copy2(subdir_or_file, dest_dir)
+
     def convert_mlflow_model_to_pytorch_model(
             mlflow_model_path: Union[str, Path],
             download_dir: Path) -> None:
         """
         Download the mlflow model assets(model, config and proprocessor.json file)
         in the download directory to have similar directory structure as the pytorch model.
 
@@ -118,50 +209,328 @@
         :type mlflow_model_path: Union[str, Path]
         :param download_dir: Destination directory to download the model
         :type download_dir: Path
         """
 
         os.makedirs(download_dir, exist_ok=True)
         try:
-            DATA_DIR = ModelSelectorConstants.MLFLOW_MODEL_DATA_PATH
-            model_dir = Path(mlflow_model_path, f'{DATA_DIR}/model')
-            config_dir = Path(mlflow_model_path, f'{DATA_DIR}/config')
-            tokenizer_dir = Path(mlflow_model_path, f'{DATA_DIR}/tokenizer')
-
-            # copy the model
-            shutil.copytree(model_dir, download_dir, dirs_exist_ok=True)
-
-            # copy the config files
-            shutil.copytree(config_dir, download_dir, dirs_exist_ok=True)
-
-            # copy tokenizer files
-            shutil.copytree(tokenizer_dir, download_dir, dirs_exist_ok=True)
-        except Exception:
+            # flatten and copy to download dir
+            ModelSelector.flatten_and_copy_directories(src_dir=mlflow_model_path, dest_dir=download_dir)
+
+            # copy license file
+            save_license_file(
+                model_name_or_path=mlflow_model_path,
+                license_file_name=ModelSelectorDefaults.LICENSE_FILE_NAME,
+                destination_paths=[str(download_dir)]
+            )
+            # mlflow models should contains MLmodel file
+            if not os.path.isfile(os.path.join(download_dir, ModelSelectorConstants.MLMODEL)):
+                error_string = f"{ModelSelectorConstants.MLMODEL} missing in the input mlflow model"
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(ACFTUserError, pii_safe_message=error_string)
+                )
+        except Exception as e:
             shutil.rmtree(download_dir, ignore_errors=True)
-            directories = f" '{model_dir}', '{config_dir}', '{tokenizer_dir}' "
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ACFTUserError, pii_safe_message=str(e))
+            )
+
+    def _call_api_with_retries(self, request_method: Callable[..., requests.Response],
+                               uri: str, **kwargs: dict) -> requests.Response:
+        """
+        Submit a REST API request to the given uri using the given request method. Retries failed requests
+        and either fails with error reporting or returns the request reponse.
+
+        :param request_method: request method to call
+        :type request_method: Callable[..., requests.Response]
+        :param uri: REST API uri
+        :type uri: str
+        :param **kwargs: keyword args to pass to request method
+        :type **kwargs: dict
+        """
+
+        for i in range(ModelSelectorAPIConstants.API_RETRY_COUNT - 1):
+            try:
+                return request_method(uri, **kwargs)
+            except requests.exceptions.RequestException as e:
+                logger.warning(
+                    f"Encountered {e.__class__.__name__} error while calling REST API "
+                    f"Retries left: {ModelSelectorAPIConstants.API_RETRY_COUNT - i - 1}. Error details: {e}"
+                )
+
+                wait_time = ((2 ** i) * ModelSelectorAPIConstants.BACKOFF_IN_SECONDS + random.uniform(0, 1))
+                logger.info(f"Waiting {wait_time:.2f} seconds before attempting call to {uri} again.")
+                time.sleep(wait_time)
+
+        # Attempt to load the call REST API one more time. Warn and advise to run again in case of new failure.
+        logger.warning("Attempting to call REST API one last time. If this fails, please submit a new run.")
+        try:
+            return request_method(uri, **kwargs)
+        except requests.exceptions.RequestException as e:
+            error_string = (
+                f"Encountered {e.__class__.__name__} error while calling REST API "
+                f"Failed with exception {e}"
+            )
+            raise ACFTSystemException._with_error(
+                AzureMLError.create(ACFTSystemError, pii_safe_message=error_string)
+            )
+
+    def _get_model_info_from_registry(self) -> requests.Response:
+        """
+        Retrieve model metadata from registry using REST API call.
+        :return API call response
+        :type requests.Response
+        """
+        if self.service_endpoint is None:
+            logger.info(f"{ModelSelectorAPIConstants.SERVICE_ENDPOINT} environment variable is not set")
+            return
+        if not self.base_model_asset_id:
+            self.base_model_asset_id = ModelSelectorAPIConstants.MODEL_ASSET_ID.format(
+                ModelSelectorDefaults.MODEL_REGISTRY, self.registry_model_name)
+        registry_uri = ModelSelectorAPIConstants.REGISTRY_URI.format(self.service_endpoint, self.base_model_asset_id)
+
+        # make API call to get model info from registry
+        logger.info(f"Calling REST API to get model metadata for {self.registry_model_name} from registry")
+        request_args = {"headers" : self.auth_header}
+        return self._call_api_with_retries(requests.get, registry_uri, **request_args)
+
+    def _get_blobstore_sas_credential(self, model_info: dict) -> requests.Response:
+        """
+        Retrieve SaS credential for blob url specified in model_info using REST API call.
+        :param model_info: model metadata including blob url
+        :type model_info: dict
+        :return API call response
+        :type requests.Response
+        """
+        model_url = model_info[ModelSelectorAPIConstants.URL]
+        self.base_model_asset_id = model_info[ModelSelectorAPIConstants.ASSET_ID]
+
+        # get SaS credential because we cannot access blob store with AML Run Token
+        sas_uri = ModelSelectorAPIConstants.SAS_URI.format(self.service_endpoint)
+        blob_reference_sas_request_dto = {
+            ModelSelectorAPIConstants.BLOB_REF_ASSET_ID: self.base_model_asset_id,
+            ModelSelectorAPIConstants.BLOB_REF_BLOB_URI: model_url
+        }
+
+        # make API call to get SaS credential from registry
+        logger.info("Calling REST API to get SaS credential for model artifacts blob")
+        request_args = {"json" : blob_reference_sas_request_dto, "headers" : self.auth_header}
+        return self._call_api_with_retries(requests.post, sas_uri, **request_args)
+
+    def _download_blobstore_model_artifacts(self, sas_info: dict) -> os.PathLike:
+        """
+        Download model artifacts from blobstore with SaS credential.
+        :param sas_info: SaS credential
+        :type model_info: dict
+        :return model_download_path: path that model artifacts are downloaded to
+        :type os.Path
+        """
+        model_download_path = os.path.join(self.output_dir, ModelSelectorConstants.REGISTRY_DOWNLOAD_DIR)
+        os.makedirs(model_download_path, exist_ok=True)
+        download_location = PyLocationInfo('Local', model_download_path, {})
+        if_exists = PyIfDestinationExists.MERGE_WITH_OVERWRITE
+        credential = sas_info[ModelSelectorAPIConstants.BLOB_REF][ModelSelectorAPIConstants.CREDENTIAL]
+        wasbs_uri = credential[ModelSelectorAPIConstants.WASBS_URI]
+        try:
+            logger.info("Downloading model artifacts from blobstore")
+            ensure_rslex_environment()
+            Copier.copy_uri(download_location, wasbs_uri, if_exists, "")
+        except Exception as e:
+            error_string = (
+                f"Unable to download model artifacts from blobstore."
+                f"Failed with exception {e}"
+            )
+            raise ACFTSystemException._with_error(
+                AzureMLError.create(ACFTSystemError, pii_safe_message=error_string)
+            )
+
+        logger.info(f"Model {self.registry_model_name} is downloaded to folder {model_download_path}")
+        return model_download_path
+
+    def _model_name_download_from_registry(self) -> bool:
+        """
+        Search for model name in ModelSelectorDefaults.MODEL_REGISTRY.
+        Download model and set model asset path (self.pytorch_model or self.mlflow_model)
+        if the model is successfully downloaded from the registry.
+
+        :return: True if model is downloaded from registry, False otherwise
+        :rtype: bool
+        """
+
+        # convert HF id to registry model name
+        self.registry_model_name = self.model_name.replace("/", "-")
+        self._add_mmd_model_prefix()
+        logger.info(f"Searching for model {self.registry_model_name} in registry")
+
+        # get AML run token and service endpoint
+        context = Run.get_context()
+        self.auth_header = context.experiment.workspace._auth_object.get_authentication_header()
+        self.service_endpoint = os.getenv(ModelSelectorAPIConstants.SERVICE_ENDPOINT)
+
+        model_info_response = self._get_model_info_from_registry()
+
+        # if the model was found, get sas credential and download model artifacts
+        if model_info_response.status_code == 200:
+            logger_str = f"Model {self.registry_model_name} was found in registry "\
+                         f"{ModelSelectorDefaults.MODEL_REGISTRY}"
+            logger.info(logger_str)
+            model_info = model_info_response.json()
+            logger.info(f"model_info: {model_info}")
+
+            # get SaS credential for accessing blobstore
+            sas_info_response = self._get_blobstore_sas_credential(model_info)
+            if sas_info_response.status_code != 200:
+                error_string = "Unable to retrieve SaS token for model download from registry"
+                raise ACFTSystemException._with_error(
+                    AzureMLError.create(ACFTSystemError, pii_safe_message=error_string)
+                )
+            sas_info = sas_info_response.json()
+            logger.info("SaS token retrieved to download model")
+
+            # download model artifacts from blobstore using sas credential
+            model_download_path = self._download_blobstore_model_artifacts(sas_info)
+
+            # set the asset path for the downloaded model, replace model_name with registry_model_name
+            model_format = model_info[ModelSelectorAPIConstants.MODEL_FORMAT]
+            if model_format == ModelSelectorAPIConstants.CUSTOM_MODEL:
+                self.pytorch_model = Path(model_download_path, ModelSelectorConstants.PYTORCH_MODEL_ROOT)
+                self.model_name = self.registry_model_name
+                self._remove_mmd_model_prefix()
+
+            elif model_format == ModelSelectorAPIConstants.MLFLOW_MODEL:
+                self.mlflow_model = Path(model_download_path, ModelSelectorConstants.MLFLOW_MODEL_ROOT)
+                self.model_name = self.registry_model_name
+                self._remove_mmd_model_prefix()
+            else:
+                logger.warning(f'Model {self.registry_model_name} is not \
+                            of type {ModelSelectorAPIConstants.CUSTOM_MODEL} or \
+                            {ModelSelectorAPIConstants.MLFLOW_MODEL}')
+            return True
+        else:
+            logger.warning(f'Model {self.model_name} was not found in registry '
+                           f'{ModelSelectorDefaults.MODEL_REGISTRY}. Received response with status code'
+                           f' {model_info_response.status_code} and error message: {model_info_response.content}')
+            return False
+
+    def _add_mmd_model_prefix(self) -> None:
+        """ Add mmd-3x prefix to model name for MMDetection Models if not present.
+        """
+        if self.model_family == ModelFamily.MMDETECTION_IMAGE:
+            # MMD 3.x models are prefix with mmd-3x in the model registry
+            if self.registry_model_name.startswith(ModelSelectorDefaults.MMD_MODELS_PREFIX):
+                msg = f"Model {self.registry_model_name} is already prefixed with "\
+                      f"{ModelSelectorDefaults.MMD_MODELS_PREFIX}"
+                logger.info(msg)
+            else:
+                self.registry_model_name = f"{ModelSelectorDefaults.MMD_MODELS_PREFIX}{self.registry_model_name}"
+
+    def _remove_mmd_model_prefix(self) -> None:
+        """Remove mmd-3x prefix from model name if present."""
+        if self.model_name.startswith(ModelSelectorDefaults.MMD_MODELS_PREFIX):
+            msg = (
+                f"Model {self.model_name} is prefixed with {ModelSelectorDefaults.MMD_MODELS_PREFIX}"
+                f" Removing prefix."
+            )
+            logger.info(msg)
+            self.model_name = self.model_name[len(ModelSelectorDefaults.MMD_MODELS_PREFIX) :]
+
+    def _validate_hf_model_name(self) -> None:
+        """Validate if model name is present in hugging face model repository.
+        :raises ACFTValidationException: if model name is not present in hugging face model repository
+        """
+        model_info_list = check_if_model_present_in_hf_hub(self.model_name)
+        if len(model_info_list) == 0:
             raise ACFTValidationException._with_error(
                 AzureMLError.create(
-                    InvalidMlflowModelFormat, directories
+                    ACFTUserError,
+                    pii_safe_message=f"Model name {self.model_name} is not present in hugging face model repository. "
+                                     f"Please check {ModelRepositoryURLs.HF_TRANSFORMER_IMAGE_CLASSIFIFCATION} for "
+                                     f"valid model name."
                 )
             )
 
-    def run_workflow(self):
+    def _validate_if_model_supported(self) -> None:
+        """Validate if model is supported by ACFT.
+        :raises ACFTValidationException: if model is not supported by ACFT
+        """
+        error_message = f"{self.model_name} is not supported. " \
+                        f"Please select different model from AzureML Model catalog "
+        if self.model_family == ModelFamily.HUGGING_FACE_IMAGE:
+            error_message += f"or check {ModelRepositoryURLs.HF_TRANSFORMER_IMAGE_CLASSIFIFCATION}"
+        elif self.model_family == ModelFamily.MMDETECTION_IMAGE:
+            error_message += f"or check {ModelRepositoryURLs.MMDETECTION}"
+        elif self.model_family == ModelFamily.MMTRACKING_VIDEO:
+            error_message += f"or check {ModelRepositoryURLs.MMTRACKING}"
+        if self.model_name in self.unsupported_model_list:
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(ACFTUserError, pii_safe_message=error_message)
+            )
+
+    def get_model_asset_id(self, is_mlflow_model: bool) -> str:
+        """Read the model asset id from the run context.
+
+        :param is_mlflow_model: whether the model is provided through mlflow i/p port
+        :type is_mlflow_model: bool
+
+        :return asset id of the i/p model
+        :rtype str
+        """
+        try:
+            run_ctx = Run.get_context()
+            if isinstance(run_ctx, Run):
+                run_details = run_ctx.get_details()
+                model_path = RunDetailsConstants.MLFLOW_MODEL if is_mlflow_model else RunDetailsConstants.PYTORCH_MODEL
+                return run_details[RunDetailsConstants.RUN_DEFINITION][
+                    RunDetailsConstants.INPUT_ASSETS][model_path][
+                    RunDetailsConstants.ASSET][RunDetailsConstants.ASSET_ID]
+            else:
+                logger.info("Found offline run")
+                return ModelSelectorConstants.ASSET_ID_NOT_FOUND
+        except Exception as e:
+            logger.warning(f"Could not fetch the model asset id: {e}")
+            return ModelSelectorConstants.ASSET_ID_NOT_FOUND
+
+    def run_workflow(self) -> None:
         """If model asset path is provided then it will download the model. Pytorch model will take preference
-        over mlflow model. If model name is provided then, it will not download model from framework hub.
+        over mlflow model. If model name is provided then, it will download the model from the registry. If the
+        model is not found in the registry, it will download model from framework hub.
         It's responsibility of downstream component (e.g., finetune) to load the model.
 
         :raises ArgumentException._with_error: Raise exception if model ports or model name is not provided.
         """
+
+        # If model_name is provided and asset paths are not specified, download the model from the registry.
+        # If the model is found in the registry, the asset path will be set for the next if/elif block
+        if ((self.model_name is not None) and (self.pytorch_model is None) and (self.mlflow_model is None)):
+
+            if not self.download_from_source:
+                model_found_in_registry = self._model_name_download_from_registry()
+            else:
+                model_found_in_registry = False
+                # remove mmd prefix from model name if present when downloading from source
+                self._remove_mmd_model_prefix()
+                logger.info("Retrieving model from source instead of registry.")
+
+            # If model is not found in the registry, validate model_name before downloading from framework hub
+            if not model_found_in_registry:
+                self.base_model_asset_id = None
+                self._validate_if_model_supported()
+
+                if self.model_family == ModelFamily.HUGGING_FACE_IMAGE:
+                    self._validate_hf_model_name()
+
         if self.pytorch_model is not None:
             self._download_pytorch_model_from_registry()
             self.pytorch_model = ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY
             self.mlflow_model = None
         elif self.mlflow_model is not None:
             self._download_mlflow_model_from_registry()
             self.mlflow_model = ModelSelectorDefaults.MLFLOW_MODEL_DIRECTORY
         elif self.model_name is None:
             raise ACFTValidationException._with_error(
                 AzureMLError.create(
                     ModelInputEmpty, argument_name="Model ports and model_name"
                 )
             )
+        self._fetch_metadata()
+
         self._prepare_and_logs_arguments()
```

## azureml/acft/common_components/model_selector/constants.py

```diff
@@ -9,18 +9,95 @@
 class ModelSelectorConstants:
     """String constants for model selector component."""
 
     PYTORCH_MODEL_PATH = "pytorch_model_path"
     MLFLOW_MODEL_PATH = "mlflow_model_path"
     MODEL_NAME = "model_name"
     MLFLOW_MODEL_DATA_PATH = "data"
+    LICENSE_PATH = "license_path"
+    MLFLOW_MODEL_ROOT = "mlflow_model_folder"
+    PYTORCH_MODEL_ROOT = "pytorch_model_folder"
+    REGISTRY_DOWNLOAD_DIR = "registry_model_download"
+    FINETUNING_TASKS = "finetuning_tasks"
+    MODEL_METAFILE_PATH = "model_metafile_path"
+    MODEL_DEFAULTS_PATH = "model_defaults_path"
+    BASE_MODEL_ASSET_ID = "base_model_asset_id"
+    BASE_MODEL_TASK = "base_model_task"
+    ASSET_ID_NOT_FOUND = "ASSET_ID_NOT_FOUND"
+    MODEL_NAME_NOT_FOUND = "MODEL_NAME_NOT_FOUND"
+    MODEL_METADATA = "model_metadata"
+    MLMODEL = "MLmodel"
+
+
+class ModelSelectorAPIConstants:
+    """String constants for API calls in model selector component"""
+
+    REGISTRY_URI = "{}/modelregistry/v1.0/registry/models?assetIdOrReference={}"
+    SERVICE_ENDPOINT = "AZUREML_SERVICE_ENDPOINT"
+    MODEL_ASSET_ID = "azureml://registries/{}/models/{}/labels/latest"
+    SAS_URI = "{}/assetstore/v1.0/dataReference/getBlobReferenceSAS"
+    CUSTOM_MODEL = "CUSTOM"
+    MLFLOW_MODEL = "MLFLOW"
+    URL = "url"
+    MODEL_FORMAT = "modelFormat"
+    ASSET_ID = "assetId"
+    BLOB_REF = "blobReferenceForConsumption"
+    CREDENTIAL = "credential"
+    WASBS_URI = "wasbsUri"
+    BLOB_REF_ASSET_ID = "AssetId"
+    BLOB_REF_BLOB_URI = "BlobUri"
+    API_RETRY_COUNT = 5
+    BACKOFF_IN_SECONDS = 1
+    KVTAGS = "kvTags"
+    TASK = "task"
 
 
 @dataclass
 class ModelSelectorDefaults:
     """Data class for model selector defaults."""
 
     MODEL_SELECTOR_ARGS_SAVE_PATH = "model_selector_args.json"
     MLFLOW_MODEL_DIRECTORY = "model"
     PYTORCH_MODEL_DIRECTORY = "model"
+    MODEL_METADATA_PATH = "model_metadata.json"
+    MODEL_DEFAULTS_PATH = "model_defaults.json"
     # Mandetory name for HF trainer.
     MODEL_CHECKPOINT_FILE_NAME = "pytorch_model.bin"
+    # License file for HF
+    LICENSE_FILE_NAME = "LICENSE"
+    MODEL_REGISTRY = "azureml"
+    MMD_MODELS_PREFIX = "mmd-3x-"
+    FAST_RCNN_MODEL_PREFIX = "fast-rcnn"
+
+
+class RunDetailsConstants:
+    """ Run details constants"""
+
+    MLFLOW_MODEL = "mlflow_model"
+    PYTORCH_MODEL = "pytorch_model"
+    RUN_DEFINITION = "runDefinition"
+    INPUT_ASSETS = "inputAssets"
+    ASSET = "asset"
+    ASSET_ID = "assetId"
+    NODE_COUNT = "nodeCount"
+    PROCESS_COUNT = "processCount"
+    PYTORCH_DISTRIBUTION = "pyTorch"
+
+
+@dataclass
+class ModelFamily:
+    """A class to represent model family constants."""
+
+    HUGGING_FACE_IMAGE = "HuggingFaceImage"
+    MMDETECTION_IMAGE = "MmDetectionImage"
+    MMTRACKING_VIDEO = "MmTrackingVideo"
+
+
+@dataclass
+class ModelRepositoryURLs:
+    """A class to represent model repository URLs."""
+
+    MMDETECTION = "https://github.com/open-mmlab/mmdetection/tree/v3.1.0/configs"
+    HF_TRANSFORMER_IMAGE_CLASSIFIFCATION = (
+        "https://huggingface.co/models?pipeline_tag=image-classification&library=transformers"
+    )
+    MMTRACKING = "https://github.com/open-mmlab/mmtracking/tree/v0.14.0/configs/mot"
```

## azureml/acft/common_components/utils/logging_utils.py

```diff
@@ -1,21 +1,22 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """
 This file defines the util functions used for logging
 """
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional, cast, List
 import logging
 import os
 import sys
 
 from dataclasses import dataclass, asdict
 
+from azureml.acft.common_components.utils.constants import AzuremlRunType
 from azureml.acft.common_components.utils.telemetry_pii_stripping_formatter import (
     AppInsightsPIIStrippingAllMessagesFormatter,
 )
 from azureml.automl.core.shared import log_server
 from azureml.automl.core.shared.logging_fields import camel_to_snake_case
 from azureml.core import Run
 from azureml.core.run import _OfflineRun
@@ -38,14 +39,15 @@
     TASK_TYPE = "task_type"
     LOG_FOLDER = "log_folder"
     LOG_FILENAME = "log_filename"
     RANK = "rank"
     PROPERTIES = "properties"
     STDOUT = "stdout"
     APP_NAME = "app_name"
+    COMPONENT_NAME = "component_name"
 
 
 class SystemSettings:
     """System settings."""
 
     LOG_FILENAME = "azureml_acft.log"
     LOG_FOLDER = "logs"
@@ -53,14 +55,15 @@
     DEFAULT_COMPUTE_TARGETS = "AmlCompute"
     DEFAULT_CLIENT_TYPE = "sdk"
 
 
 @dataclass
 class AzuremlAcftSettings:
     """AzureAcftSettings class to configure logging."""
+
     task_type: str
     subscription_id: str
     region: str
     parent_run_id: str
     run_id: str
     child_run_id: str
     app_name: str = SystemSettings.DEFAULT_APP_NAME
@@ -114,72 +117,100 @@
 
 def set_logging_parameters(
     task_type: str,
     output_dir: Optional[str] = None,
     output_file: Optional[str] = None,
     acft_custom_dimensions: Optional[Dict] = None,
     hf_logs_to_app_insight: Optional[bool] = True,
+    azureml_pkg_denylist_logging_patterns: Optional[List] = None,
+    non_azureml_packages_to_disable_logs: Optional[List] = None,
+    log_level: int = logging.DEBUG,
 ) -> None:
     """Sets the logging parameters so that we can track all the training runs from
     a given project.
 
     :param task_type: task type
     :type task_type: str
     :param output_dir: output directory of log file
     :type output_dir: Optional[str]
     :param output_file: name of the file for logging
     :type output_file: Optional[str]
     :param acft_custom_dimensions: custom information to add in log messages
     :type acft_custom_dimensions: Optional[Dict]
     :param hf_logs_to_app_insight: add app insight handler to HF trainer logger, if true
     :type hf_logs_to_app_insight: Optional[bool]
+    :param azureml_pkg_denylist_logging_patterns: Substrings patterns that would be used to identify the logs to
+                                                exclude from Azure ML package logs.
+    :type azureml_pkg_denylist_logging_patterns: Optional[List]
+    :param disable_non_azureml_package_logs: List of non-Azure ML package names to disable logs for.
+    :type disable_non_azureml_package_logs: Optional[List]
     """
 
     output_dir = output_dir or SystemSettings.LOG_FOLDER
     logging_file = output_file or SystemSettings.LOG_FILENAME
 
     azureml_run = Run.get_context()
-    _set_default_custom_dimensions_and_handlers(task_type, output_dir, logging_file, azureml_run)
+    _set_default_custom_dimensions_and_handlers(task_type, output_dir, logging_file, azureml_run, log_level)
 
     _set_acft_custom_dimensions(acft_custom_dimensions)
 
-    _set_formatter_to_handlers(log_server.handlers, azureml_run.id, hf_logs_to_app_insight)
+    _set_formatter_to_handlers(
+        log_server.handlers,
+        azureml_run.id,
+        hf_logs_to_app_insight,
+        azureml_pkg_denylist_logging_patterns,
+        non_azureml_packages_to_disable_logs,
+    )
     if hf_logs_to_app_insight:
         _add_app_insights_handler_to_hf_logger(log_server.handlers)
 
 
 def _set_formatter_to_handlers(
-    handlers: Dict[str, logging.Handler], run_id: str, hf_logs_to_app_insight: bool
+    handlers: Dict[str, logging.Handler],
+    run_id: str,
+    hf_logs_to_app_insight: bool,
+    azureml_pkg_denylist_logging_patterns: Optional[List] = None,
+    non_azureml_packages_to_disable_logs: Optional[List] = None,
 ) -> None:
     """Set formatter to the handlers
     :param handlers: handlers added in logger
     :type handlers: Dict[str, logging.Handler]
     :param run_id: run id
     :type run_id: str
     :param hf_logs_to_app_insight: flag to indicate whether to add app insights handler to HuggingFace logger. If
     true, then add AppInsightsPIIStrippingAllMessagesFormatter which strip PII information from all logs messages (
     info, warning, error, exceptions) else use AppInsightsPIIStrippingFormatter which strips exception messages.
     :type hf_logs_to_app_insight: bool
+    :param azureml_pkg_denylist_logging_patterns: Substring patterns that would be used to identify the logs to exclude
+                                               from Azure ML package logs.
+    :type azureml_pkg_denylist_logging_patterns: Optional[List]
+    :param disable_non_azureml_package_logs: List of non-Azure ML package names to disable logs for.
+    :type disable_non_azureml_package_logs: Optional[List]
     """
 
     fmt = (
         "%(asctime)s.%(msecs)03d - {} - {} - %(levelname)s - %(process)d - %(name)s.%(funcName)s:%(lineno)d - %("
         "message)s".format(SystemSettings.DEFAULT_APP_NAME, run_id)
     )
     datefmt = "%Y-%m-%d %H:%M:%S"
     for key, handler in handlers.items():
         if isinstance(handler, AppInsightsLoggingHandler):
             if hf_logs_to_app_insight:
-                formatter = AppInsightsPIIStrippingAllMessagesFormatter
+                formatter = AppInsightsPIIStrippingAllMessagesFormatter(
+                    fmt=fmt,
+                    datefmt=datefmt,
+                    azureml_pkg_denylist_logging_patterns=azureml_pkg_denylist_logging_patterns,
+                    non_azureml_packages_to_disable_logs=non_azureml_packages_to_disable_logs,
+                )
             else:
-                formatter = AppInsightsPIIStrippingFormatter
+                formatter = AppInsightsPIIStrippingFormatter(fmt=fmt, datefmt=datefmt)
         else:
-            formatter = logging.Formatter
+            formatter = logging.Formatter(fmt=fmt, datefmt=datefmt)
 
-        handler.setFormatter(formatter(fmt=fmt, datefmt=datefmt))
+        handler.setFormatter(formatter)
 
 
 def _set_acft_custom_dimensions(acft_custom_dimensions: Dict) -> None:
     """Add acft custom dimensions to the log server's custom dimensions.
     :param acft_custom_dimensions: custom dimensions related to the acft project
     :type acft_custom_dimensions: Dict
     """
@@ -187,14 +218,18 @@
         project_name = acft_custom_dimensions[LoggingLiterals.PROJECT_NAME]
         log_server.update_custom_dimensions({LoggingLiterals.PROJECT_NAME: project_name})
 
     if acft_custom_dimensions and LoggingLiterals.PROJECT_VERSION_NUMBER in acft_custom_dimensions:
         project_version_number = acft_custom_dimensions[LoggingLiterals.PROJECT_VERSION_NUMBER]
         log_server.update_custom_dimensions({LoggingLiterals.PROJECT_VERSION_NUMBER: project_version_number})
 
+    if acft_custom_dimensions and LoggingLiterals.COMPONENT_NAME in acft_custom_dimensions:
+        component_name = acft_custom_dimensions[LoggingLiterals.COMPONENT_NAME]
+        log_server.update_custom_dimensions({LoggingLiterals.COMPONENT_NAME: component_name})
+
 
 def _get_azureml_acft_common_components_version() -> str:
     """Get version of azureml.acft.common_components package"""
     try:
         from azureml.acft import common_components
 
         return common_components.VERSION
@@ -208,30 +243,51 @@
         from azureml.acft import accelerator
 
         return accelerator.VERSION
     except Exception:
         return UNKNOWN_VALUE
 
 
+def _get_root_pipeline_run(azureml_run: Run):
+    """
+    Get root pipeline run. Root pipeline run is the pipeline/step run which is at the root in the run hierarchy
+    or is child of a non-pipeline/step run (for example, when pipeline run is child of HyperDrive run).
+
+    :param azureml_run: Current run.
+    :type azureml_run: azureml.core.Run
+    :return: Root pipeline run if exists else None.
+    :rtype: azureml.core.Run
+    """
+    parent_run = azureml_run.parent
+    child_run = None
+    while parent_run is not None and (
+        parent_run.type == AzuremlRunType.PIPELINE_RUN or parent_run.type == AzuremlRunType.STEP_RUN
+    ):
+        child_run = parent_run
+        parent_run = parent_run.parent
+    return child_run
+
+
 def _set_default_custom_dimensions_and_handlers(
-    task_type: str, output_dir: str, logging_file: str, azureml_run: Run
+    task_type: str, output_dir: str, logging_file: str, azureml_run: Run, log_level: int = logging.DEBUG
 ) -> None:
     """Add current run custom dimensions information and handlers (file, stream and app insights) to log server
 
     :param task_type: task type
     :type task_type: str
     :param output_dir: output directory of log file
     :type output_dir: str
     :param logging_file: name of the file for logging
     :type logging_file: str
     """
     if not isinstance(azureml_run, _OfflineRun):
         subscription_id = azureml_run.experiment.workspace.subscription_id
         region = azureml_run.experiment.workspace.location
-        parent_run_id = azureml_run.parent.id if azureml_run.parent is not None else None
+        root_pipeline_run = _get_root_pipeline_run(azureml_run=azureml_run)
+        parent_run_id = root_pipeline_run.id if root_pipeline_run is not None else None
     else:
         subscription_id = "not_available_offline"
         region = "not_available_offline"
         parent_run_id = "not_available_offline"
     child_run_id = azureml_run.id
 
     # Build the acft settings expected by the logger
@@ -239,46 +295,48 @@
         task_type=task_type,
         subscription_id=subscription_id,
         region=region,
         parent_run_id=parent_run_id,
         run_id=child_run_id,
         child_run_id=child_run_id,
         azureml_acft_common_components_version=_get_azureml_acft_common_components_version(),
-        azureml_acft_accelerator_version=_get_azureml_acft_accelerator_version()
-    )
-    log_server.update_custom_dimensions(
-        asdict(acft_settings)
+        azureml_acft_accelerator_version=_get_azureml_acft_accelerator_version(),
     )
+    log_server.update_custom_dimensions(asdict(acft_settings))
 
     component_name_literal = camel_to_snake_case(RequiredFieldKeys.COMPONENT_NAME_KEY)
     algorithm_type_literal = camel_to_snake_case(StandardFieldKeys.ALGORITHM_TYPE_KEY)
     subscription_id_literal = camel_to_snake_case(RequiredFieldKeys.SUBSCRIPTION_ID_KEY)
 
     log_server.update_custom_dimensions(
         {
             component_name_literal: TELEMETRY_AZUREML_ACFT_COMPONENT_KEY,
             algorithm_type_literal: task_type,
             subscription_id_literal: subscription_id,
         }
     )
 
     os.makedirs(output_dir, exist_ok=True)
+    # :func set_log_file - adds a file handler to handlers global variable
     log_server.set_log_file(os.path.join(output_dir, logging_file))
-    _add_stream_handler()
+    # Setting the log level for the file handler
+    if "file" in log_server.handlers and isinstance(log_server.handlers["file"], logging.FileHandler):
+        log_server.handlers["file"].setLevel(log_level)
+    _add_stream_handler(log_level)
     send_telemetry, level = get_diagnostics_collection_info(component_name=TELEMETRY_AZUREML_ACFT_COMPONENT_KEY)
     if send_telemetry:
         log_server.enable_telemetry(INSTRUMENTATION_KEY, component_name=TELEMETRY_AZUREML_ACFT_COMPONENT_KEY)
     log_server.set_verbosity(level)
 
 
-def _add_stream_handler() -> None:
+def _add_stream_handler(log_level: int = logging.DEBUG) -> None:
     """Add console handler i.e., stream handler"""
 
     stdout_handler = logging.StreamHandler(sys.stdout)
-    stdout_handler.setLevel(logging.DEBUG)
+    stdout_handler.setLevel(log_level)
     log_server.add_handler(LoggingLiterals.STDOUT, stdout_handler)
 
 
 def _add_app_insights_handler_to_hf_logger(handlers: Dict) -> None:
     """Set the app insight handler to all hf logger
 
     :param handlers: The dictionary of handlers attached to log server
```

## azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py

```diff
@@ -1,36 +1,79 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """This file contains telemetry PII stripping formatter."""
 
 from logging import LogRecord
-
+from typing import Dict, Tuple, List, Optional
 from azureml.automl.core.shared.exceptions import NON_PII_MESSAGE
 from azureml.automl.core.shared.telemetry_formatter import AppInsightsPIIStrippingFormatter
+from azureml.acft.common_components.utils.constants import (
+    NonAzureMLLoggingLibsAllowedPatterns,
+    LoggingLibsIdentifier,
+)
 
 
 class AppInsightsPIIStrippingAllMessagesFormatter(AppInsightsPIIStrippingFormatter):
     """Formatter that will prevent any PII debug/info/warning/exception from getting logged"""
 
-    # Following is the allow-list of messages to log in app-insight if they are generating outside the azureml
-    # packages.
-    # Dev Notes: Add only PII-free messages to whitelist from non azureml packages.
-    ALLOWED_PATTERN_TO_LOG_IN_APPINSIGHTS = []
+    def __init__(
+        self,
+        *args,
+        azureml_pkg_denylist_logging_patterns: Optional[List] = None,
+        non_azureml_packages_to_disable_logs: Optional[List] = None,
+        **kwargs
+    ):
+        """
+        Initialize a new instance of AppInsightsPIIStrippingAllMessagesFormatter.
+
+        :param azureml_pkg_denylist_logging_patterns: Substring patterns that would be used to identify the logs to
+                                                        exclude from Azure ML package logs.
+        :type azureml_pkg_denylist_logging_patterns: Optional[List]
+        :param disable_non_azureml_package_logs: List of non-Azure ML package names to disable logs for.
+        :type disable_non_azureml_package_logs: Optional[List]
+        """
+        super().__init__(*args, **kwargs)
+
+        self.azureml_pkg_denylist_logging_patterns = azureml_pkg_denylist_logging_patterns or []
+        self.non_azureml_packages_to_disable_logs = non_azureml_packages_to_disable_logs or []
+
+        self.non_azureml_pkg_allowlist_logging_patterns = self._prepare_allowlist_patterns_for_non_azureml_packages()
+
+    def _prepare_allowlist_patterns_for_non_azureml_packages(self) -> Dict[str, Tuple[str]]:
+        """Prepare allowlist patterns for non-AzureML packages
+
+        :return: Dict of allowlist patterns
+        :rtype: Dict[str, Tuple[str]]
+        """
+
+        lib_to_allowlist_patterns = {}
+
+        for lib, patterns in NonAzureMLLoggingLibsAllowedPatterns.NON_AZUREML_PKGS_IDENTIFIER_PATTERNS_MAPPING.items():
+            if lib not in self.non_azureml_packages_to_disable_logs:
+                lib_to_allowlist_patterns[lib] = patterns
+        return lib_to_allowlist_patterns
 
     def format(self, record: LogRecord) -> str:
         """
         Modify the log record to strip log messages if they originate from a non-AzureML packages and not matches
-        the ALLOWED_PATTERN_TO_LOG_IN_APPINSIGHTS
+        the allowed pattern to log in appinsights for corresponding non-AzureML package or if they originate from
+        AzureML packages and not matches the denylist pattern to log in appinsights for AzureML package.
 
         :param record: Logging record.
         :return: Formatted record message.
         """
-        message = record.getMessage()
+        message = record.getMessage().lower()
+        is_azureml_package = record.name.startswith(LoggingLibsIdentifier.AZUREML)
 
-        if record.name.startswith("azureml.") or any(allowed_patern in message for allowed_patern in
-                                                     self.ALLOWED_PATTERN_TO_LOG_IN_APPINSIGHTS):
-            return super().format(record)
-        else:
-            record.message = NON_PII_MESSAGE
-            record.msg = NON_PII_MESSAGE
+        if (
+            is_azureml_package
+            and not any(pattern.lower() in message for pattern in self.azureml_pkg_denylist_logging_patterns)
+        ) or any(
+            (record.name.startswith(non_azureml_pkg) and any(pattern.lower() in message for pattern in patterns))
+            for non_azureml_pkg, patterns in self.non_azureml_pkg_allowlist_logging_patterns.items()
+        ):
             return super().format(record)
+
+        record.message = NON_PII_MESSAGE
+        record.msg = NON_PII_MESSAGE
+        return super().format(record)
```

## azureml/acft/common_components/utils/error_handling/error_definitions.py

```diff
@@ -314,7 +314,73 @@
     @property
     def message_format(self) -> str:
         """
         Message Format
         """
 
         return ACFTErrorStrings.GENERIC_ERROR
+
+
+class LossScaleAtMinimum(UserError):
+    """
+    Deepspeed Loss scale at minimum error
+    """
+
+    @property
+    def message_format(self) -> str:
+        """
+        Message Format
+        """
+        return ACFTErrorStrings.LOSS_SCALE_AT_MINIMUM
+
+
+class SKUNotSupported(NotSupported):
+    """
+    SKU Not Supported Error
+    """
+
+    @property
+    def message_format(self) -> str:
+        """
+        Message Format
+        """
+
+        return ACFTErrorStrings.SKU_NOT_SUPPORTED
+
+
+@error_decorator(
+    use_parent_error_code=True, details_uri="https://docs.microsoft.com/en-us/azure/virtual-machines/sizes-gpu"
+)
+class InsufficientGPUMemoryAutoFindBatchSize(Memory):
+    """
+    Insufficient GPU memory error
+    """
+    @property
+    def message_format(self) -> str:
+        """
+        Message Format
+        """
+        return ACFTErrorStrings.INSUFFICIENT_GPU_MEMORY_AUTO_FIND_BATCH_SIZE
+
+
+class FP16TrainingNotSupportedForModel(NotSupported):
+    """
+    FP16 training not supported for specified model error
+    """
+
+    @property
+    def message_format(self) -> str:
+        """
+        Message Format
+        """
+        return ACFTErrorStrings.FP16_TRAINING_NOT_SUPPORTED_FOR_MODEL
+
+
+class CudaErrorInvalidDeviceOrdinal(NotSupported):
+    """Error definition for invalid device ordinal."""
+
+    @property
+    def message_format(self) -> str:
+        """
+        Message Format
+        """
+        return ACFTErrorStrings.INVALID_PARAM_NUMBER_OF_GPU_TO_USE_FINETUNING
```

## azureml/acft/common_components/utils/error_handling/error_strings.py

```diff
@@ -1,12 +1,13 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Error strings for custom errors"""
+from azureml.acft.common_components.utils.constants import AzuremlSKUType
 
 
 class ACFTErrorStrings:
     """Error strings for ACFT errors"""
 
     INTERNAL_ERROR = (
         "Encountered an internal ACFT error. Error Message/Code: {error_details}. Traceback: "
@@ -26,14 +27,18 @@
         "The selected Model [{ModelName:log_safe}] doesn't support the current Task [{TaskName:log_safe}], "
         "Please select a different model"
     )
     TOKENIZER_NOT_SUPPORTED = (
         "The selected Tokenizer [{Tokenizer:log_safe}] doesn't support the current Task [{TaskName:log_safe}], "
         "Please select a different tokenizer or tokenizer type"
     )
+    SKU_NOT_SUPPORTED = (
+        "The selected compute does not meet minimum compute requirements, "
+        f"Please use {AzuremlSKUType.STANDARD_NC24s_V3} SKU."
+    )
     VALIDATION_ERROR = "Error while validating parameters [{error:log_safe}]"
     RESOURCE_NOT_FOUND = "Resource [{ResourceName:log_safe}] not found"
     INVALID_CHECKPOINT_DIRECTORY = "Provide a valid checkpoint directory. Got [{dir:log_safe}]"
     PATH_NOT_FOUND = "Path [{path:log_safe}] was not found"
     ML_CLIENT_NOT_CREATED = (
         "Failed to create ML Client. This is likely because you didn't create a managed identity and assign it to "
         "your compute cluster."
@@ -44,14 +49,40 @@
     INVALID_DATASET = "Only one label found in training and validation data combined"
     INSUFFICIENT_SHM_MEMORY = (
         "There is not enough shared memory on the machine to do the operation. "
         "Please try running the experiment with a smaller batch size."
     )
     INSUFFICIENT_GPU_MEMORY = (
         "There is not enough GPU memory on the machine to do the operation. "
-        "Please try running the experiment on a VM with higher GPU memory, decrease the batch "
-        "size or image size."
+        "Please try:\n"
+        "1. Running the experiment on a VM with higher GPU memory.\n"
+        "2. Decreasing the `per_device_train_batch_size`.\n"
+        "3. Enabling LoRA or Deepspeed or ORT or any combinations of these.\n"
+        "4. Setting the `pad_to_max_length` to false for Language tasks.\n"
+        "5. Decreasing the `image_size` for Image tasks.\n"
+        "6. Decreasing the `lora_r` if `apply_lora` is set to true.\n"
     )
     INVALID_MLFLOW_MODEL_FORMAT = (
         "Please make sure that the mlflow model has the following directories: \n [{directories:log_safe}] "
     )
     ARGUMENT_BLANK_OR_EMPTY = "An empty value for argument [{argument_name:log_safe}] is provided."
+    INSUFFICIENT_GPU_MEMORY_AUTO_FIND_BATCH_SIZE = (
+        "Auto find batch size couldn't find the right batch size to do the operation. Encountered error [{error}]. "
+        "You could try:\n"
+        "1. Running the experiment on Standard_NC24s_v3 SKU.\n"
+        "2. Enabling LoRA.\n"
+        "3. Enabling deepspeed optimization\n"
+        "4. Enabling deepspeed and ORT optimization.\n"
+    )
+    LOSS_SCALE_AT_MINIMUM = (
+        "Encountered an error while training with Deepspeed [{error}]"
+        "Try with fp32 precision or provide a different Deepspeed config"
+    )
+    FP16_TRAINING_NOT_SUPPORTED_FOR_MODEL = (
+        "An error occurred while attempting to train with fp16 precision for the specified model [{error}]. "
+        "Please consider using fp32 precision or selecting a different model."
+    )
+    INVALID_PARAM_NUMBER_OF_GPU_TO_USE_FINETUNING = (
+        "The selected value for number_of_gpu_to_use_finetuning [{number_of_gpu_to_use_finetuning:log_safe}] is "
+        "higher than gpus present in the node [{maximum_number_of_gpu_to_use_finetuning:log_safe}]. Please fix "
+        "the value and try again."
+    )
```

## azureml/acft/common_components/utils/error_handling/exceptions.py

```diff
@@ -1,13 +1,13 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """Exceptions for the acft package."""
 import json
-from typing import Optional
+from typing import Any, Optional
 
 from azureml._common._error_definition import AzureMLError
 from azureml._common._error_response._error_response_constants import ErrorCodes
 from azureml._common.exceptions import AzureMLException
 from azureml.exceptions import UserErrorException
 
 
@@ -72,14 +72,30 @@
 
 
 class ACFTDataException(ACFTValidationException):
     """Exception related to data validations."""
 
     _error_code = ErrorCodes.INVALIDDATA_ERROR
 
+    def __init__(self, message: str = "", **kwargs: Any) -> None:
+        """Init function that accepts message argument.
+
+        In the case of torch.utils.data.DataLoader with num_workers > 0, any exceptions raised in
+        worker processes is reraised using this function
+        https://github.com/pytorch/pytorch/blob/v2.1.0/torch/_utils.py#L674.
+        If an exception raised in worker process has "message" in its properties,
+        this function expects the __init__ method
+        to have message argument. Adding it here as we raise ACFTDataException and it has "message" parameter.
+        Please note that this behavior in torch can be changed in future versions
+        and this __init__ method needs to be updated accordingly.
+        """
+        if "exception_message" in kwargs:
+            message = kwargs.pop("exception_message")
+        super().__init__(exception_message=message, **kwargs)
+
 
 # System Exception
 class ACFTSystemException(ACFTException):
     """Exception for internal errors that happen within the SDK."""
 
     _error_code = ErrorCodes.SYSTEM_ERROR
```

## azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py

```diff
@@ -15,26 +15,43 @@
 from azureml.automl.core._run import run_lifecycle_utilities
 from azureml.automl.core.shared import logging_utilities
 from azureml.automl.core.shared.exceptions import NON_PII_MESSAGE
 from azureml.core.run import Run  # type: ignore
 from azureml.exceptions import ServiceException as AzureMLServiceException
 
 from azureml.acft.common_components.utils.logging_utils import get_logger_app
-from .error_definitions import ACFTInternalError, InsufficientGPUMemory, InsufficientSHMMemory
+from .error_definitions import (
+    ACFTInternalError,
+    InsufficientGPUMemory,
+    InsufficientSHMMemory,
+    InsufficientGPUMemoryAutoFindBatchSize,
+    LossScaleAtMinimum,
+    FP16TrainingNotSupportedForModel,
+    CudaErrorInvalidDeviceOrdinal
+)
 from .exceptions import ACFTSystemException
+from ..torch_utils import get_node_gpu_count
+from ..run_utils import calculate_per_node_process_count
+
 
 logger = get_logger_app(__name__)
 
 
 CUDA_OUT_OF_MEMORY_ERROR = "CUDA out of memory"
 SHARED_MEMORY_ERROR = "shared memory"
+AUTO_FIND_BATCH_SIZE_MEMORY_ERROR = "No executable batch size found, reached zero"
+LOSS_SCALE_AT_MINIMUM = "Current loss scale already at minimum - cannot decrease scale anymore"
 CUDA_ERROR = "CUDA error:"
+CUDA_ERROR_INVALID_DEVICE_ORDINAL = "CUDA error: invalid device ordinal"
 CUDNN_ERROR = "cuDNN error:"
 CUDA_ERROR_EXCEPTION_MESSAGE = "Potential temporary hardware failure - please resubmit the run. If that does not " \
                                "solve the problem, please file a support ticket for further investigation."
+MMDETECTION_FP16_TRAINING_NOT_SUPPORTED_ERROR_1 = "expected scalar type Half but found Float"
+MMDETECTION_FP16_TRAINING_NOT_SUPPORTED_ERROR_2 = "got Half for the destination and Float for the source"
+MMDETECTION_FP16_TRAINING_NOT_SUPPORTED_ERROR_3 = "not implemented for 'Half'"
 
 
 def swallow_all_exceptions(fail_run: bool = True, time_delay: int = 0) -> Callable[..., Any]:
     """This decorates a function to handle uncaught exceptions and fail the run with System Error.
 
     :param fail_run: if True, fail the run. If False, just log the exception and raise it further.
         Note: This is useful when an exception is raised from a child process, because the exception details might not
@@ -53,17 +70,37 @@
                 str_e = str(e)
 
                 if isinstance(e, (AzureMLException, AzureMLServiceException)):
                     interpreted_exception = e
                 elif CUDA_OUT_OF_MEMORY_ERROR in str_e:
                     azureml_error = AzureMLError.create(InsufficientGPUMemory)
                     raise AzureMLException._with_error(azureml_error)
+                elif AUTO_FIND_BATCH_SIZE_MEMORY_ERROR in str_e:
+                    azureml_error = AzureMLError.create(InsufficientGPUMemoryAutoFindBatchSize, error=e)
+                    raise AzureMLException._with_error(azureml_error)
+                elif CUDA_ERROR_INVALID_DEVICE_ORDINAL in str_e:
+                    azureml_error = AzureMLError.create(
+                        CudaErrorInvalidDeviceOrdinal,
+                        number_of_gpu_to_use_finetuning=calculate_per_node_process_count(),
+                        maximum_number_of_gpu_to_use_finetuning=get_node_gpu_count()
+                    )
+                    raise AzureMLException._with_error(azureml_error)
+                elif LOSS_SCALE_AT_MINIMUM in str_e:
+                    azureml_error = AzureMLError.create(LossScaleAtMinimum, error=e)
+                    raise AzureMLException._with_error(azureml_error)
                 elif SHARED_MEMORY_ERROR in str_e:
                     azureml_error = AzureMLError.create(InsufficientSHMMemory)
                     raise AzureMLException._with_error(azureml_error)
+                elif (
+                    MMDETECTION_FP16_TRAINING_NOT_SUPPORTED_ERROR_1 in str_e
+                    or MMDETECTION_FP16_TRAINING_NOT_SUPPORTED_ERROR_2 in str_e
+                    or MMDETECTION_FP16_TRAINING_NOT_SUPPORTED_ERROR_3 in str_e
+                ):
+                    azureml_error = AzureMLError.create(FP16TrainingNotSupportedForModel, error=e)
+                    raise AzureMLException._with_error(azureml_error)
                 else:
                     # This is an unknown exception - try to log as much non PII info in telemetry
                     # in case logging is not yet initialized or not working
                     error_details = str_e
 
                     # If CUDA related error, direct user to file a ticket.
                     if (CUDA_ERROR in str_e) or (CUDNN_ERROR in str_e):
@@ -113,11 +150,12 @@
     """Get pii free message for ACFT exceptions.
     :param exception: Exception object
     :type exception: BaseException
     :return: PII free message
     :rtype: str
     """
     get_pii_free_exception_msg_format = getattr(exception, "get_pii_free_exception_msg_format", None)
-    if get_pii_free_exception_msg_format and callable(get_pii_free_exception_msg_format):
+    if get_pii_free_exception_msg_format and callable(get_pii_free_exception_msg_format) and \
+       getattr(exception, "_azureml_error", None):
         return get_pii_free_exception_msg_format()
     else:
         return NON_PII_MESSAGE
```

## Comparing `azureml_acft_common_components-0.0.9.dist-info/LICENSE.txt` & `azureml_acft_common_components-47.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_acft_common_components-0.0.9.dist-info/METADATA` & `azureml_acft_common_components-47.0.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-Metadata-Version: 2.1
-Name: azureml-acft-common-components
-Version: 0.0.9
-Summary: Basic implementation of common components and         utility functions that can be used by all verticals (image/video/nlp/multi-modal).
-Home-page: https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py
-Author: Microsoft Corp
-License: https://aka.ms/azureml-sdk-license
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7,<3.10
-Description-Content-Type: text/x-rst
-Requires-Dist: azureml-core (>=1.50.0)
-Requires-Dist: azureml-automl-core (>=1.50.0)
-Provides-Extra: image
-Requires-Dist: pynvml ; extra == 'image'
-Requires-Dist: numpy (~=1.22.0) ; extra == 'image'
-Requires-Dist: opencv-python-headless (>=4.1.1) ; extra == 'image'
-Requires-Dist: simplification (==0.5.7) ; extra == 'image'
-Requires-Dist: recordclass (~=0.14.3) ; extra == 'image'
-
-
-Basic implementation of common components and utility functions that can be used by all verticals - 
-image/video/nlp/multi-modal.
-
-
-
-
+Metadata-Version: 2.1
+Name: azureml-acft-common-components
+Version: 47.0.0
+Summary: Basic implementation of common components and         utility functions that can be used by all verticals (image/video/nlp/multi-modal).
+Home-page: https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py
+Author: Microsoft Corp
+License: https://aka.ms/azureml-sdk-license
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7,<3.12
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: azureml-core >=1.50.0
+Requires-Dist: azureml-automl-core >=1.50.0
+Requires-Dist: azure-ai-ml >=1.5.0
+Provides-Extra: image
+Requires-Dist: pynvml ; extra == 'image'
+Requires-Dist: numpy >=1.22.0 ; extra == 'image'
+Requires-Dist: opencv-python-headless >=4.1.1 ; extra == 'image'
+Requires-Dist: simplification ==0.7.10 ; extra == 'image'
+Requires-Dist: recordclass ~=0.21.1 ; extra == 'image'
+Requires-Dist: torchvision >=0.14.1 ; extra == 'image'
+Requires-Dist: scikit-image ==0.19.3 ; extra == 'image'
+
+
+Basic implementation of common components and utility functions that can be used by all verticals - 
+image/video/nlp/multi-modal.
+
+
```

## Comparing `azureml_acft_common_components-0.0.9.dist-info/RECORD` & `azureml_acft_common_components-47.0.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 azureml/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/acft/__init__.py,sha256=uR25VVAK6AdsLS8H2EQKoLKr3inwv9tYSp_Omp0DefA,317
-azureml/acft/common_components/__init__.py,sha256=hr3oefrzgarg0fejNfPkarGwvWUg-jJixOvV_4wA4rc,1226
-azureml/acft/common_components/_version.py,sha256=GEQLI_HpmoMBfahlay2eatCORC4cSw-U1d_alMy5g14,34
+azureml/acft/common_components/__init__.py,sha256=qq5zvNTTkW03t2vWuKMg3xFH9r53TnO5ktToGynZrpM,1314
+azureml/acft/common_components/_version.py,sha256=6tbwTfcvkL7u8i_rkvzyeWb_6rwSOsoLFvfhWf89WZM,36
 azureml/acft/common_components/image/__init__.py,sha256=j8yOgBjCbm6UmIGPBpZPTcXntwmylDCnLJPC3SX7pPI,309
 azureml/acft/common_components/image/runtime_common/__init__.py,sha256=94ATB0UuQmPx5JO6mE1JO0Na87EYOpIsQY53HVYc8RQ,337
 azureml/acft/common_components/image/runtime_common/classification/__init__.py,sha256=uaENFv98jd-IaiMr1-mR9heLMwMpvUyh1KVSxJhy3E0,298
 azureml/acft/common_components/image/runtime_common/classification/common/__init__.py,sha256=uaENFv98jd-IaiMr1-mR9heLMwMpvUyh1KVSxJhy3E0,298
 azureml/acft/common_components/image/runtime_common/classification/common/classification_utils.py,sha256=6cZOX7TXbz7N5_NbeRcKlTbA4UXiUpJhJ6LIxGBX44A,27157
 azureml/acft/common_components/image/runtime_common/classification/common/constants.py,sha256=kwaawgEYNHXdAheuixirOSsQTEVKG9DS_JrlYjBSoMk,7505
 azureml/acft/common_components/image/runtime_common/classification/common/transforms.py,sha256=0bl02l6e0_Wfw0xGDC_aS6gLZhesYMtsAJuVtLvGwKY,2599
@@ -14,63 +14,72 @@
 azureml/acft/common_components/image/runtime_common/classification/io/read/dataloader.py,sha256=sNOpydt7UmhzcEKrUfNKNpJGOZ7wtDFnfGKF9MyVURE,4953
 azureml/acft/common_components/image/runtime_common/classification/io/read/dataset_wrappers.py,sha256=GP0XK1ikkz3YpNUBrJ_s6ns0292MPo8J43JAfm6Hr7Q,22521
 azureml/acft/common_components/image/runtime_common/classification/io/read/utils.py,sha256=zGvJrqBjwtei07GMsW9ATUG6Nf3oGTG5cAEBmiMWWW0,5611
 azureml/acft/common_components/image/runtime_common/classification/models/__init__.py,sha256=aJJrit8a_1sLTCOlpPkw4glIgbQRiqO2O2Xrur3KyGU,429
 azureml/acft/common_components/image/runtime_common/classification/models/base_model_wrapper.py,sha256=uahSZlAohNNVHQ0J_42XzjUj5ECwGUzphUbrZ7E8PAE,11546
 azureml/acft/common_components/image/runtime_common/common/__init__.py,sha256=pFEEmYGBIZY3ewu0pxR0RSD2HbCGaxmvdZcGtc5KD-4,331
 azureml/acft/common_components/image/runtime_common/common/aml_dataset_base_wrapper.py,sha256=V7UYkdN1d5tIUij4DWyJnG9RS-jDX6fd7YWku99X8N4,1903
-azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py,sha256=fa5DyEBRqhwfTUZeq9IT4alvsCd2lWWzRX6HHpI8xsg,10436
+azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py,sha256=9w7ejzXTVHWoUyVJpfD8ZIGfXEKeLCpo55lbw8J3qnk,11717
 azureml/acft/common_components/image/runtime_common/common/average_meter.py,sha256=jgLAM2T4sqzcYwkqyZPonA-PzjTo22u_FkgjSXELJz4,2025
 azureml/acft/common_components/image/runtime_common/common/base_model_factory.py,sha256=CPOhl-GYEFym44H27nwYHlCZJqQ1HmITib-KnPrq0_M,2229
 azureml/acft/common_components/image/runtime_common/common/base_model_settings.py,sha256=vjFc2VjnItGtNFI6GO_5RyY8TTh3nFMRciIM-darIws,1231
 azureml/acft/common_components/image/runtime_common/common/constants.py,sha256=S1sv1EC3iaSWIG-KYclsycXq2g7IbOXzVN2f7FwCIZQ,22490
 azureml/acft/common_components/image/runtime_common/common/data_utils.py,sha256=qdg2SmmN-0BJkaut0XtjhNGbNm7zvhabolJcnxJbDxM,2826
 azureml/acft/common_components/image/runtime_common/common/dataloaders.py,sha256=vmcWBwbzqfvuggQAv-Bygh1k67y6W9X43_EwwDiaZq4,3200
-azureml/acft/common_components/image/runtime_common/common/dataset_helper.py,sha256=5NnIEciNp89brKd-r46ADK1yZo_mjEUcQY0G2y71r9c,18973
+azureml/acft/common_components/image/runtime_common/common/dataset_helper.py,sha256=ifAbPd0Hh2TzkeCzx7A5Mg6Zwnw6TzAorFImOXnw_OU,19103
 azureml/acft/common_components/image/runtime_common/common/distributed_utils.py,sha256=gFEAucPiA2xXj6-CdYQrO7EUJHBwlK9VVMyKCWxzdDQ,21069
 azureml/acft/common_components/image/runtime_common/common/errors.py,sha256=9knV7WI1paVWHLXGTSIa-AxYMq0s2RtrrsyEXxVbqH0,672
 azureml/acft/common_components/image/runtime_common/common/exceptions.py,sha256=eDxs4p3tI7JZG4Fv60rIehayqAO751xELLPGozsWuig,2379
 azureml/acft/common_components/image/runtime_common/common/logging_utils.py,sha256=LldRV06kWtaI16snaGVgyH6rpMhWAnTy2SHBex0_R6A,2528
 azureml/acft/common_components/image/runtime_common/common/model_export_utils.py,sha256=Waqd9i5zbM0qjlE6xQ_aLf34bg4aVIvipQr7SzPFGmY,25060
 azureml/acft/common_components/image/runtime_common/common/parameters.py,sha256=LeK68JJUAybs2T8liQ6HslL116crfKahsuFifoRscEM,14782
 azureml/acft/common_components/image/runtime_common/common/prediction_dataset.py,sha256=4ZGAXSq7anMb_imjrT11evZ_DzWsv5RTlwqDN8JgPsg,10346
 azureml/acft/common_components/image/runtime_common/common/pretrained_model_utilities.py,sha256=ObueTqclBkrQknkfEDd-fa1EX524yNyRmx3qN89IIdI,37090
 azureml/acft/common_components/image/runtime_common/common/sku_validation.py,sha256=slsTvUhJAdE3rWgdSdIVgqVT8MP41YEisOeiZ6mxG_o,3033
 azureml/acft/common_components/image/runtime_common/common/system_meter.py,sha256=CdeRQMMPmZTaTzZpgvIVQqZuMSg5KGwTMxyIGWDV9kQ,9850
 azureml/acft/common_components/image/runtime_common/common/tiling_dataset_element.py,sha256=zAWpfNwokX_EnDFDEPZHPn-1HrkC4kjRwMJRydJ7HcA,5469
 azureml/acft/common_components/image/runtime_common/common/tiling_utils.py,sha256=AsBF80uAO5RhHBFAODgYVVjny7JYHC9E3banFrCOsl4,6591
 azureml/acft/common_components/image/runtime_common/common/torch_utils.py,sha256=LgCIEUaJLj4vvGRPLFzW71G1kj5BdDW4hh2yYZpzhGk,1039
-azureml/acft/common_components/image/runtime_common/common/utils.py,sha256=KkqtybpCDed1b2ZLrGMqnqEKDZy9bB7HoT-pQUe6WDo,65435
+azureml/acft/common_components/image/runtime_common/common/utils.py,sha256=hX6DzSob6wkcQd11Yli7mQ5xPeGhr2RZnXws66d5euA,66311
 azureml/acft/common_components/image/runtime_common/object_detection/__init__.py,sha256=4HLxQJGWo9Pyuo72Y_NfWgBFEtzAE3ZX6qtcvFoQgJ4,302
 azureml/acft/common_components/image/runtime_common/object_detection/common/__init__.py,sha256=RumyOi_96w6tL_An0_TyagRmE038Y85xtCPncBDDHtM,311
 azureml/acft/common_components/image/runtime_common/object_detection/common/augmentations.py,sha256=vdTMyk8D9vxs3umy74KYqEXab0ynDcXoSyTEAEImgfk,9651
 azureml/acft/common_components/image/runtime_common/object_detection/common/boundingbox.py,sha256=eoq3on9xZj6KS1-3AV1AHJ50DWaJwjjEpdFYDbLhQgc,7382
 azureml/acft/common_components/image/runtime_common/object_detection/common/coco_eval_box_converter.py,sha256=La7QuM5X87pHBse4WVnAVwDezYgPS9KWTXy2bpLhImo,3068
-azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py,sha256=6O_mWOeXyUkWljwLYZWTTRYI21U9TgcvdwIkInLQlMA,11008
+azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py,sha256=hKoc9_H4-S9dzk6ZYn_r_8Hr0qAMi4v7Zbetn_uHMY0,11041
 azureml/acft/common_components/image/runtime_common/object_detection/common/masktools.py,sha256=bl9jPxVuNjpG7qdUd3jkhx_xABtctk1qUqHme6CJ1m0,11945
 azureml/acft/common_components/image/runtime_common/object_detection/common/object_detection_utils.py,sha256=2RRAksFAG4HmU_2_yTiEOKSHL2zBCXejwymvWnhYQZw,27533
 azureml/acft/common_components/image/runtime_common/object_detection/common/parameters.py,sha256=rwrL2-Y7bui62w9mnm5QZlHVS6LOTtyqbCqjVHoby5E,4995
 azureml/acft/common_components/image/runtime_common/object_detection/common/tiling_helper.py,sha256=q9THTSjwQW0OmvOTIGuROTRJV09spo-3gELmHaZ_35g,25959
 azureml/acft/common_components/image/runtime_common/object_detection/data/__init__.py,sha256=ou8vwg4U9jTYFXZKTfWOY5JNXCMZuwo95zPNbXoT2yo,306
 azureml/acft/common_components/image/runtime_common/object_detection/data/dataset_wrappers.py,sha256=LNgHGRaWw1XT_Q0PgxKSGNQJa9cKg6Mco7A1Jt5kLUA,4664
-azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py,sha256=nM7Bedarcj7Ql79ykVFWgVkGB2pj1yFLzjopyk2qPZg,39856
+azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py,sha256=5JEZkoB7yIrT3T2PuUKXrHACZjXjL2UziqPJmr_L_x4,40176
 azureml/acft/common_components/image/runtime_common/object_detection/data/loaders.py,sha256=apVXxFYHTu8BuKNg3fG2TSpLZahHFOvSCmTYz-jaV3I,6162
-azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py,sha256=AaVaYo2ajG7FVgSGEJAOlzDr9xFBreSARnmkRipXkpw,11899
+azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py,sha256=oYE7MNnJAzEvjMMwbkZLEvgwlmZIn_EjdLk5i3Dgc0w,13798
 azureml/acft/common_components/image/runtime_common/object_detection/data/tiling_distributed_sampler.py,sha256=4_hG1bTjjpqzx0ZlP_IJKZsXg1s92B7YQwHA4GBsjTk,5037
 azureml/acft/common_components/image/runtime_common/object_detection/data/utils.py,sha256=-nUlyASqUsGWsDWghB3AGHg1MxssAs08qiQYz5sgRiw,11332
 azureml/acft/common_components/model_selector/__init__.py,sha256=jRvS3fBIHo1tVbO4tyF1yGeLWjG1XdbayHyXalLatIw,325
-azureml/acft/common_components/model_selector/component.py,sha256=hfCtFXxVwPMj6buKnqlU6y0NIvk7xTBWVGFtlmiFxtI,7131
-azureml/acft/common_components/model_selector/constants.py,sha256=p5JSgAEOyg0GvrcmXBDOWsU6wlKG61fWT96Eq7oO1lk,854
+azureml/acft/common_components/model_selector/component.py,sha256=LuhfprY-mGss3RRxfy5sCnKZtpMffBxwUa5LpAxDY_s,26691
+azureml/acft/common_components/model_selector/constants.py,sha256=pNvgWvjhdfc33t11mThyf_Y6giz1ek6i7JIpWiBxWB0,3499
 azureml/acft/common_components/utils/__init__.py,sha256=eCFvAjyFUk4n1AshMP_Dhgy1z71GEEFIQ6BpCkH76_Y,236
-azureml/acft/common_components/utils/logging_utils.py,sha256=atIjOyW8sMRPu9t29i4NtwNNYpHXpHo1zVXVCUwIPn0,12226
-azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py,sha256=B3yl0YTg-A-l17BdMKKqgSRyKGKFAjJ4KV6aEm4bskk,1649
+azureml/acft/common_components/utils/arg_utils.py,sha256=Gu-GVPr-gim-0vHd3bOGG3Q65RreaTp47RYrKEPCR4o,1075
+azureml/acft/common_components/utils/callbacks.py,sha256=tzhM9Y4FCoyVO1HXB-3TSuvZCOEGnyrQf2mSAMttVlU,5300
+azureml/acft/common_components/utils/constants.py,sha256=AOt56QVdD2yzAQlF3Vb4x52c_V2MwMeiQsUFtO8TwcA,3618
+azureml/acft/common_components/utils/hf_hub_utils.py,sha256=QeJGHwN0b1YAg71drxBW6UcxvHhZIktbjf-t0RYG4Oo,1039
+azureml/acft/common_components/utils/license_utils.py,sha256=Z9nbUwDtKgk13D_H8-0KnOsXBJ0FgJhInHfzm7pgdaU,3623
+azureml/acft/common_components/utils/logging_utils.py,sha256=qMs7EWTyeVBpqNmA1wnOYazfhu0-CkeoPsdzHY6odKM,15400
+azureml/acft/common_components/utils/mlflow_utils.py,sha256=N_53H9KYyXGY2BNWcQVo410nhtQ_B5FpnfXDqFjgR_s,1358
+azureml/acft/common_components/utils/run_utils.py,sha256=rQ5OhLm9pxIF_AfdHiUyeESwdEH3qAWypgUoyYAlinA,2260
+azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py,sha256=4eIccJ8jn_GanNGx4NKpv71inuW3bngrSIYzbHJJAVc,3742
+azureml/acft/common_components/utils/torch_utils.py,sha256=QEZoEKQzDghywYzMiexU1yP2nPkpDnFkg2H3QQfl_mc,529
+azureml/acft/common_components/utils/transformer_utils.py,sha256=nzyw9DU1KGUQ_kBxUpGQzfMYBQgsX-Fhg8b2iynBBFM,700
 azureml/acft/common_components/utils/error_handling/__init__.py,sha256=jnEZ1NnBpIuFYVEWASuWOJVIW3z837TlbgYlw0tL6uU,226
-azureml/acft/common_components/utils/error_handling/error_definitions.py,sha256=5VQX8ce1r9sOAKOtE9zIxhJXKLFTO7u2-UXw2jXHKiw,6864
-azureml/acft/common_components/utils/error_handling/error_strings.py,sha256=j6GiNf5KoHBrGM8YC9hXewMdxXVPp5k5xt5DgZBiSHc,2943
-azureml/acft/common_components/utils/error_handling/exceptions.py,sha256=sXd93TFqllxPfvZAgjf6iZsEmSKRMG6cKxoq0UKX5vo,3650
-azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py,sha256=g__vT7-kizKoutNafkl7xIpGbtq9tY1nGGEAYw6Noog,5786
-azureml_acft_common_components-0.0.9.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_acft_common_components-0.0.9.dist-info/METADATA,sha256=7Oukois4NQpDLR_kaaNiconpC9_GU7qQPLXxIHfPglQ,1271
-azureml_acft_common_components-0.0.9.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-azureml_acft_common_components-0.0.9.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-azureml_acft_common_components-0.0.9.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
-azureml_acft_common_components-0.0.9.dist-info/RECORD,,
+azureml/acft/common_components/utils/error_handling/error_definitions.py,sha256=bvoMxTF5ttHH0ztEUPZFLUGrpqRi4r_GFNn4TF0GvXs,8410
+azureml/acft/common_components/utils/error_handling/error_strings.py,sha256=clzOplV0wm8Z0SZAaE4mu5iAZjnYg3igwCjS5gdIWHQ,4677
+azureml/acft/common_components/utils/error_handling/exceptions.py,sha256=XGrxlMYF0yvXGWkwHWEjJacYeflvuBrIXgggw4QTuEg,4588
+azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py,sha256=DtHWArfRsg8xB72K2uoqCx_DKB3ON3Gq4tLdX4B0nbA,8013
+azureml_acft_common_components-47.0.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_acft_common_components-47.0.0.dist-info/METADATA,sha256=j0k-FoPiL31dbLNHV9-mP4QMMVtaAqQZhOT-880R7xY,1550
+azureml_acft_common_components-47.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+azureml_acft_common_components-47.0.0.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+azureml_acft_common_components-47.0.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml_acft_common_components-47.0.0.dist-info/RECORD,,
```

