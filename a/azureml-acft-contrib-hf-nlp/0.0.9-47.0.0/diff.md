# Comparing `tmp/azureml_acft_contrib_hf_nlp-0.0.9-py3-none-any.whl.zip` & `tmp/azureml_acft_contrib_hf_nlp-47.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,101 +1,128 @@
-Zip file size: 297452 bytes, number of entries: 99
--rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 17:31 azureml/__init__.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 17:31 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 17:31 azureml/acft/contrib/__init__.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/__init__.py
--rw-rw-rw-  2.0 fat   869245 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/NOTICE
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/__init__.py
--rw-rw-rw-  2.0 fat     4929 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/base_runner.py
--rw-rw-rw-  2.0 fat     2555 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/task_factory.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/constants/__init__.py
--rw-rw-rw-  2.0 fat     8213 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/constants/constants.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/nlp_auto/__init__.py
--rw-rw-rw-  2.0 fat     3265 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/nlp_auto/config.py
--rw-rw-rw-  2.0 fat    14065 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/nlp_auto/model.py
--rw-rw-rw-  2.0 fat     4358 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/nlp_auto/tokenizer.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/__init__.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/__init__.py
--rw-rw-rw-  2.0 fat     2520 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/__init__.py
--rw-rw-rw-  2.0 fat    10105 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    16173 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/base.py
--rw-rw-rw-  2.0 fat    15582 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat     2552 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_inference.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/__init__.py
--rw-rw-rw-  2.0 fat     3126 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/finetune/__init__.py
--rw-rw-rw-  2.0 fat     9751 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    13206 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/base.py
--rw-rw-rw-  2.0 fat    14826 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat     4000 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_inference.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/__init__.py
--rw-rw-rw-  2.0 fat     2487 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/finetune/__init__.py
--rw-rw-rw-  2.0 fat     9596 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    12965 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/base.py
--rw-rw-rw-  2.0 fat    12150 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/__init__.py
--rw-rw-rw-  2.0 fat     2494 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/finetune/__init__.py
--rw-rw-rw-  2.0 fat    10143 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    12067 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/base.py
--rw-rw-rw-  2.0 fat    12464 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/__init__.py
--rw-rw-rw-  2.0 fat     2380 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/finetune/__init__.py
--rw-rw-rw-  2.0 fat     9649 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/__init__.py
--rw-rw-rw-  2.0 fat     9985 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/base.py
--rw-rw-rw-  2.0 fat    11434 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/__init__.py
--rw-rw-rw-  2.0 fat     2453 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/finetune/__init__.py
--rw-rw-rw-  2.0 fat    14466 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    28677 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/base.py
--rw-rw-rw-  2.0 fat    13059 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat     2561 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_inference.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/__init__.py
--rw-rw-rw-  2.0 fat     2534 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/__init__.py
--rw-rw-rw-  2.0 fat     9843 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    10429 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/base.py
--rw-rw-rw-  2.0 fat    15153 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat     2561 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_inference.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/__init__.py
--rw-rw-rw-  2.0 fat     2583 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/__init__.py
--rw-rw-rw-  2.0 fat     9515 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    11203 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/base.py
--rw-rw-rw-  2.0 fat    16583 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat     2284 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_inference.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/__init__.py
--rw-rw-rw-  2.0 fat     2546 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/runner.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/finetune/__init__.py
--rw-rw-rw-  2.0 fat    10788 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/finetune/finetune.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/__init__.py
--rw-rw-rw-  2.0 fat    11537 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/base.py
--rw-rw-rw-  2.0 fat    17727 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_finetune.py
--rw-rw-rw-  2.0 fat     2284 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_inference.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/__init__.py
--rw-rw-rw-  2.0 fat    16029 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/data_utils.py
--rw-rw-rw-  2.0 fat    19641 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/hf_argparser.py
--rw-rw-rw-  2.0 fat     1167 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/mlflow_preprocess.py
--rw-rw-rw-  2.0 fat     8105 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/mlflow_utils.py
--rw-rw-rw-  2.0 fat     8208 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/model_selector_utils.py
--rw-rw-rw-  2.0 fat      801 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/preprocess.py
--rw-rw-rw-  2.0 fat     5409 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/preprocess_utils.py
--rw-rw-rw-  2.0 fat     9380 b- defN 23-May-17 17:31 azureml/acft/contrib/hf/nlp/utils/validation_utils.py
--rw-rw-rw-  2.0 fat   869245 b- defN 23-May-17 17:31 azureml_acft_contrib_hf_nlp-0.0.9.data/data/azureml-acft-contrib-hf-nlp/NOTICE
--rw-rw-rw-  2.0 fat      859 b- defN 23-May-17 17:36 azureml_acft_contrib_hf_nlp-0.0.9.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1502 b- defN 23-May-17 17:36 azureml_acft_contrib_hf_nlp-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-17 17:36 azureml_acft_contrib_hf_nlp-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 17:36 azureml_acft_contrib_hf_nlp-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    11514 b- defN 23-May-17 17:36 azureml_acft_contrib_hf_nlp-0.0.9.dist-info/RECORD
-99 files, 2257640 bytes uncompressed, 278026 bytes compressed:  87.7%
+Zip file size: 363777 bytes, number of entries: 126
+-rw-rw-rw-  2.0 fat      267 b- defN 24-Mar-22 10:04 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      267 b- defN 24-Mar-22 10:04 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat      267 b- defN 24-Mar-22 10:04 azureml/acft/contrib/__init__.py
+-rw-rw-rw-  2.0 fat      792 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/__init__.py
+-rw-rw-rw-  2.0 fat       36 b- defN 24-Mar-22 10:09 azureml/acft/contrib/hf/_version.py
+-rw-rw-rw-  2.0 fat   869245 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/NOTICE
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/__init__.py
+-rw-rw-rw-  2.0 fat     7317 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/base_runner.py
+-rw-rw-rw-  2.0 fat     2710 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/task_factory.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/constants/__init__.py
+-rw-rw-rw-  2.0 fat    11035 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/constants/constants.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/data_import/__init__.py
+-rw-rw-rw-  2.0 fat     4513 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/data_import/data_import.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    50782 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/finetune.py
+-rw-rw-rw-  2.0 fat    11993 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/finetune_config.py
+-rw-rw-rw-  2.0 fat    15159 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/model_selector.py
+-rw-rw-rw-  2.0 fat    14043 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/preprocess.py
+-rw-rw-rw-  2.0 fat    11694 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/register_model.py
+-rw-rw-rw-  2.0 fat    18143 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/register_presets_model.py
+-rw-rw-rw-  2.0 fat     4526 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/validate_lora_weights.py
+-rw-rw-rw-  2.0 fat     1166 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/zero2.json
+-rw-rw-rw-  2.0 fat     1726 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/entry_point/finetune/zero3.json
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/metrics/__init__.py
+-rw-rw-rw-  2.0 fat     1303 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/metrics/load_metric.py
+-rw-rw-rw-  2.0 fat     5968 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/metrics/rouge.py
+-rw-rw-rw-  2.0 fat     8001 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/metrics/sacrebleu.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/nlp_auto/__init__.py
+-rw-rw-rw-  2.0 fat     3289 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/nlp_auto/config.py
+-rw-rw-rw-  2.0 fat    20805 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/nlp_auto/model.py
+-rw-rw-rw-  2.0 fat     4514 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/nlp_auto/tokenizer.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/base/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/base/finetune/__init__.py
+-rw-rw-rw-  2.0 fat     4385 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/base/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/__init__.py
+-rw-rw-rw-  2.0 fat     2857 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    10875 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    16318 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/base.py
+-rw-rw-rw-  2.0 fat    15987 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     2349 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/__init__.py
+-rw-rw-rw-  2.0 fat     3540 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    10482 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    13300 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/base.py
+-rw-rw-rw-  2.0 fat    15263 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     3994 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/__init__.py
+-rw-rw-rw-  2.0 fat     2541 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    11026 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/base.py
+-rw-rw-rw-  2.0 fat    12497 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/__init__.py
+-rw-rw-rw-  2.0 fat     2464 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    14453 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/base.py
+-rw-rw-rw-  2.0 fat    13481 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/__init__.py
+-rw-rw-rw-  2.0 fat     2409 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    11377 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/base.py
+-rw-rw-rw-  2.0 fat    11633 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/__init__.py
+-rw-rw-rw-  2.0 fat     2833 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    14953 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    29454 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/base.py
+-rw-rw-rw-  2.0 fat    13450 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     2349 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/__init__.py
+-rw-rw-rw-  2.0 fat     2954 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    10430 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    10646 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/base.py
+-rw-rw-rw-  2.0 fat    15579 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     2349 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/__init__.py
+-rw-rw-rw-  2.0 fat     2973 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    10356 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    11009 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/base.py
+-rw-rw-rw-  2.0 fat    16560 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     2278 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/__init__.py
+-rw-rw-rw-  2.0 fat     2919 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/finetune/__init__.py
+-rw-rw-rw-  2.0 fat     8611 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    15549 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/base.py
+-rw-rw-rw-  2.0 fat    15448 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     2391 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/__init__.py
+-rw-rw-rw-  2.0 fat     2936 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/runner.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/finetune/__init__.py
+-rw-rw-rw-  2.0 fat    11683 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/finetune/finetune.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/__init__.py
+-rw-rw-rw-  2.0 fat    11342 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/base.py
+-rw-rw-rw-  2.0 fat    17779 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_finetune.py
+-rw-rw-rw-  2.0 fat     2278 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_inference.py
+-rw-rw-rw-  2.0 fat      298 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/__init__.py
+-rw-rw-rw-  2.0 fat     5477 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/common_utils.py
+-rw-rw-rw-  2.0 fat    19817 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/data_utils.py
+-rw-rw-rw-  2.0 fat    21628 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/hf_argparser.py
+-rw-rw-rw-  2.0 fat     3516 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/io_utils.py
+-rw-rw-rw-  2.0 fat     1167 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/mlflow_preprocess.py
+-rw-rw-rw-  2.0 fat    16226 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/mlflow_utils.py
+-rw-rw-rw-  2.0 fat    11706 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/model_selector_utils.py
+-rw-rw-rw-  2.0 fat      801 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/preprocess.py
+-rw-rw-rw-  2.0 fat     7729 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/preprocess_utils.py
+-rw-rw-rw-  2.0 fat    15039 b- defN 24-Mar-22 10:04 azureml/acft/contrib/hf/nlp/utils/validation_utils.py
+-rw-rw-rw-  2.0 fat   869245 b- defN 24-Mar-22 10:04 azureml_acft_contrib_hf_nlp-47.0.0.data/data/azureml-acft-contrib-hf-nlp/NOTICE
+-rw-rw-rw-  2.0 fat     1166 b- defN 24-Mar-22 10:04 azureml_acft_contrib_hf_nlp-47.0.0.data/data/deepspeed/zero2.json
+-rw-rw-rw-  2.0 fat     1726 b- defN 24-Mar-22 10:04 azureml_acft_contrib_hf_nlp-47.0.0.data/data/deepspeed/zero3.json
+-rw-rw-rw-  2.0 fat      859 b- defN 24-Mar-22 10:09 azureml_acft_contrib_hf_nlp-47.0.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1631 b- defN 24-Mar-22 10:09 azureml_acft_contrib_hf_nlp-47.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 10:09 azureml_acft_contrib_hf_nlp-47.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Mar-22 10:09 azureml_acft_contrib_hf_nlp-47.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    14683 b- defN 24-Mar-22 10:09 azureml_acft_contrib_hf_nlp-47.0.0.dist-info/RECORD
+126 files, 2493741 bytes uncompressed, 339053 bytes compressed:  86.4%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: azureml/acft/contrib/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/__init__.py
 Comment: 
 
+Filename: azureml/acft/contrib/hf/_version.py
+Comment: 
+
 Filename: azureml/acft/contrib/hf/nlp/NOTICE
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/base_runner.py
@@ -24,14 +27,65 @@
 
 Filename: azureml/acft/contrib/hf/nlp/constants/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/constants/constants.py
 Comment: 
 
+Filename: azureml/acft/contrib/hf/nlp/entry_point/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/data_import/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/data_import/data_import.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/finetune.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/finetune_config.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/model_selector.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/preprocess.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/register_model.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/register_presets_model.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/validate_lora_weights.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/zero2.json
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/entry_point/finetune/zero3.json
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/metrics/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/metrics/load_metric.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/metrics/rouge.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/metrics/sacrebleu.py
+Comment: 
+
 Filename: azureml/acft/contrib/hf/nlp/nlp_auto/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/nlp_auto/config.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/nlp_auto/model.py
@@ -39,14 +93,23 @@
 
 Filename: azureml/acft/contrib/hf/nlp/nlp_auto/tokenizer.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/__init__.py
 Comment: 
 
+Filename: azureml/acft/contrib/hf/nlp/tasks/base/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/base/finetune/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/base/finetune/finetune.py
+Comment: 
+
 Filename: azureml/acft/contrib/hf/nlp/tasks/multi_label/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/multi_label/runner.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/__init__.py
@@ -93,20 +156,14 @@
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/runner.py
 Comment: 
 
-Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/finetune/__init__.py
-Comment: 
-
-Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/finetune/finetune.py
-Comment: 
-
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/base.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/preprocess_for_finetune.py
@@ -114,20 +171,14 @@
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/runner.py
 Comment: 
 
-Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/finetune/__init__.py
-Comment: 
-
-Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/finetune/finetune.py
-Comment: 
-
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/base.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/preprocess_for_finetune.py
@@ -135,20 +186,14 @@
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/runner.py
 Comment: 
 
-Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/finetune/__init__.py
-Comment: 
-
-Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/finetune/finetune.py
-Comment: 
-
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/base.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/preprocess_for_finetune.py
@@ -222,14 +267,38 @@
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_finetune.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_inference.py
 Comment: 
 
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/runner.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/finetune/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/finetune/finetune.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/__init__.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/base.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/preprocess_for_finetune.py
+Comment: 
+
+Filename: azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/preprocess_for_inference.py
+Comment: 
+
 Filename: azureml/acft/contrib/hf/nlp/tasks/translation/__init__.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/translation/runner.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/translation/finetune/__init__.py
@@ -249,20 +318,26 @@
 
 Filename: azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_inference.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/utils/__init__.py
 Comment: 
 
+Filename: azureml/acft/contrib/hf/nlp/utils/common_utils.py
+Comment: 
+
 Filename: azureml/acft/contrib/hf/nlp/utils/data_utils.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/utils/hf_argparser.py
 Comment: 
 
+Filename: azureml/acft/contrib/hf/nlp/utils/io_utils.py
+Comment: 
+
 Filename: azureml/acft/contrib/hf/nlp/utils/mlflow_preprocess.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/utils/mlflow_utils.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/utils/model_selector_utils.py
@@ -273,26 +348,32 @@
 
 Filename: azureml/acft/contrib/hf/nlp/utils/preprocess_utils.py
 Comment: 
 
 Filename: azureml/acft/contrib/hf/nlp/utils/validation_utils.py
 Comment: 
 
-Filename: azureml_acft_contrib_hf_nlp-0.0.9.data/data/azureml-acft-contrib-hf-nlp/NOTICE
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.data/data/azureml-acft-contrib-hf-nlp/NOTICE
+Comment: 
+
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.data/data/deepspeed/zero2.json
+Comment: 
+
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.data/data/deepspeed/zero3.json
 Comment: 
 
-Filename: azureml_acft_contrib_hf_nlp-0.0.9.dist-info/LICENSE.txt
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_acft_contrib_hf_nlp-0.0.9.dist-info/METADATA
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_acft_contrib_hf_nlp-0.0.9.dist-info/WHEEL
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_acft_contrib_hf_nlp-0.0.9.dist-info/top_level.txt
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_acft_contrib_hf_nlp-0.0.9.dist-info/RECORD
+Filename: azureml_acft_contrib_hf_nlp-47.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/acft/contrib/hf/__init__.py

```diff
@@ -1,5 +1,24 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)  # type: ignore
+
+import sys
+
+from azureml.automl.core.shared import logging_utilities, log_server
+
+try:
+    from ._version import ver as VERSION, selfver as SELFVERSION
+    __version__ = VERSION
+except ImportError:
+    VERSION = '0.0.0+dev'
+    SELFVERSION = VERSION
+    __version__ = VERSION
+
+PROJECT_NAME = __name__
+
+# Mark this package as being allowed to log certain built-in types
+module = sys.modules[__name__]
+logging_utilities.mark_package_exceptions_as_loggable(module)
+log_server.install_sockethandler(__name__)
```

## azureml/acft/contrib/hf/nlp/base_runner.py

```diff
@@ -15,83 +15,126 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 """
 Base runner
 """
 
+import os
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from argparse import Namespace
 from pathlib import Path
+from typing import Optional
 
 from transformers.models.auto.modeling_auto import (
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING_NAMES,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING_NAMES,
     MODEL_FOR_QUESTION_ANSWERING_MAPPING_NAMES,
+    MODEL_FOR_CAUSAL_LM_MAPPING_NAMES,
 )
+from transformers import PretrainedConfig
 
 from .nlp_auto.config import AzuremlAutoConfig
 from .constants.constants import Tasks
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException, LLMException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import (
-    ModelIncompatibleWithTask,
-)
+from azureml.acft.accelerator.constants import SaveFileConstants
+from azureml.acft.accelerator.utils.checkpoint_utils import get_checkpoint_step
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ModelIncompatibleWithTask
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 TASK_SUPPORTED_MODEL_TYPES_MAP = OrderedDict([
     (Tasks.SINGLE_LABEL_CLASSIFICATION, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES),
     (Tasks.MULTI_LABEL_CLASSIFICATION, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES),
     (Tasks.REGRESSION, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES),
     (Tasks.NAMED_ENTITY_RECOGNITION, MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING_NAMES),
     (Tasks.SUMMARIZATION, MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING_NAMES),
     (Tasks.TRANSLATION, MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING_NAMES),
     (Tasks.QUESTION_ANSWERING, MODEL_FOR_QUESTION_ANSWERING_MAPPING_NAMES),
+    (Tasks.TEXT_GENERATION, MODEL_FOR_CAUSAL_LM_MAPPING_NAMES),
     (Tasks.NLP_NER, MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING_NAMES),
     (Tasks.NLP_MULTICLASS, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES),
-    (Tasks.NLP_MULTILABEL, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES)
+    (Tasks.NLP_MULTILABEL, MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING_NAMES),
+])
+
+
+ACFT_TASK_AUTO_TASK_MAP = OrderedDict([
+    (Tasks.SINGLE_LABEL_CLASSIFICATION, "AutoModelForSequenceClassification"),
+    (Tasks.MULTI_LABEL_CLASSIFICATION, "AutoModelForSequenceClassification"),
+    (Tasks.NAMED_ENTITY_RECOGNITION, "AutoModelForTokenClassification"),
+    (Tasks.QUESTION_ANSWERING, "AutoModelForQuestionAnswering"),
+    (Tasks.SUMMARIZATION, "AutoModelForSeq2SeqLM"),
+    (Tasks.TRANSLATION, "AutoModelForSeq2SeqLM"),
+    (Tasks.TEXT_GENERATION, "AutoModelForCausalLM"),
 ])
 
 
 class BaseRunner(ABC):
 
-    def check_model_task_compatibility(self, model_name_or_path: str, task_name: str) -> None:
+    def check_model_task_compatibility(self, model_name_or_path: str, task_name: str, **kwargs) -> None:
         """
         Check if the given model supports the given task in the case of Hugging Face Models
         """
         supported_model_types = TASK_SUPPORTED_MODEL_TYPES_MAP[task_name]
-        model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=model_name_or_path)
+        model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=model_name_or_path, **kwargs)
 
         if model_type not in supported_model_types:
-            raise ValidationException._with_error(
-                AzureMLError.create(
-                    ModelIncompatibleWithTask, TaskName=task_name, ModelName=model_name_or_path
+            config_dict, _ = PretrainedConfig.get_config_dict(model_name_or_path, **kwargs)
+            if "auto_map" in config_dict and ACFT_TASK_AUTO_TASK_MAP[task_name] in config_dict["auto_map"]:
+                logger.info(
+                    f"Task {task_name} is supported with external class - "
+                    f"{config_dict['auto_map'][ACFT_TASK_AUTO_TASK_MAP[task_name]]}"
+                )
+            else:
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(
+                        ModelIncompatibleWithTask, TaskName=task_name, ModelName=model_name_or_path
+                    )
                 )
-            )
 
     def resolve_resume_from_checkpoint(self, component_plus_preprocess_args: Namespace) -> None:
-        # if :param `resume_from_checkpoint` is set to True
-        #   - only load the weights using config while creating model object
-        #   - update the `resume_from_checkpoint` to the model_name_or_path to load the model, and optimizer and
-        #     scheduler states if exist
-        resume_from_checkpoint = getattr(component_plus_preprocess_args, "resume_from_checkpoint", False)
-        if hasattr(component_plus_preprocess_args, "resume_from_checkpoint"):
-            delattr(component_plus_preprocess_args, "resume_from_checkpoint")
-        if resume_from_checkpoint and isinstance(component_plus_preprocess_args.model_name_or_path, Path) \
-            and component_plus_preprocess_args.model_name_or_path.is_dir():
-            component_plus_preprocess_args.resume_from_checkpoint = str(component_plus_preprocess_args.model_name_or_path)
-        else:
-            component_plus_preprocess_args.resume_from_checkpoint = None
+        """
+        Resolve resume_from_checkpoint path to allow Auto-resuming from checkpoint in case of singularity preemption.
+        """
+        resume_from_checkpoint = None
+        if component_plus_preprocess_args.resume_from_checkpoint:
+            last_valid_checkpoint = self._get_last_valid_checkpoint(component_plus_preprocess_args.pytorch_model_folder)
+            if last_valid_checkpoint:
+                logger.info(f"Found a valid checkpoint in pytorch_model_folder: {last_valid_checkpoint}")
+                resume_from_checkpoint = last_valid_checkpoint
+            else:
+                logger.info("No valid checkpoint found in pytorch_model_folder. Will not resume from checkpoint")
+        logger.info(f"Set resume_from_checkpoint path to: {resume_from_checkpoint}")
+        component_plus_preprocess_args.resume_from_checkpoint = resume_from_checkpoint
+
+    def _get_last_valid_checkpoint(self, pytorch_model_folder: Path) -> Optional[str]:
+        """
+        Get the last (latest) checkpoint from pytorch_model_folder that contains checkpoint_done.txt
+        checkpoint_done.txt marks whether a checkpoint is safe to use.
+        """
+        contents = os.listdir(pytorch_model_folder)
+        logger.info(f"pytorch_model_folder contents: {contents}")
+        checkpoint_steps = []
+        for name in contents:
+            checkpoint_step = get_checkpoint_step(name)
+            if Path(pytorch_model_folder, name).is_dir() and checkpoint_step is not None:
+                checkpoint_steps.append(checkpoint_step)
+        for checkpoint_step in sorted(checkpoint_steps, reverse=True):
+            checkpoint_path = Path(pytorch_model_folder, f"checkpoint-{checkpoint_step}")
+            checkpoint_done_filepath = checkpoint_path / SaveFileConstants.CHECKPOINT_DONE_PATH
+            logger.info(f"Checking if {SaveFileConstants.CHECKPOINT_DONE_PATH} exists: {checkpoint_done_filepath}")
+            if checkpoint_done_filepath.exists():
+                return str(checkpoint_path)
 
     @abstractmethod
     def run_preprocess_for_finetune(self, *args, **kwargs) -> None:
         pass
 
     @abstractmethod
     def run_finetune(self, *args, **kwargs) -> None:
```

## azureml/acft/contrib/hf/nlp/task_factory.py

```diff
@@ -48,14 +48,18 @@
         from .tasks.translation.runner import TranslationRunner
         return TranslationRunner
 
     if task_name == Tasks.QUESTION_ANSWERING:
         from .tasks.qna.runner import QnARunner
         return QnARunner
 
+    if task_name == Tasks.TEXT_GENERATION:
+        from .tasks.text_generation.runner import TextGenerationRunner
+        return TextGenerationRunner
+
     if task_name == Tasks.NLP_NER:
         from .tasks.nlp_ner.runner import NLPNerRunner
         return NLPNerRunner
 
     if task_name == Tasks.NLP_MULTICLASS:
         from .tasks.nlp_multiclass.runner import NLPMulticlassRunner
         return NLPMulticlassRunner
```

## azureml/acft/contrib/hf/nlp/constants/constants.py

```diff
@@ -14,38 +14,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """File for adding all the constants"""
 
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+from azureml._common._error_definition.azureml_error import AzureMLError
+
 from dataclasses import dataclass, field
 from typing import Optional, List
 
 
 @dataclass
 class DatasetSplit:
     TEST = "test"
     TRAIN = "train"
     VALIDATION = "validation"
 
 
 @dataclass
+class DataSliceConstants:
+    """
+    Constants related to slice specification in class NLPMulticlassDataset
+    """
+    NO_SPLIT = "train"
+
+
+@dataclass
 class SaveFileConstants:
     """
     A class to represent constants for metadata related to saving the model.
     """
 
     PREPROCESS_ARGS_SAVE_PATH = "preprocess_args.json"
     FINETUNE_ARGS_SAVE_PATH = "finetune_args.json"
     CLASSES_SAVE_PATH = "class_names.json"
     ID2LABEL_SAVE_PATH = "id2label.json"
     LABEL2ID_SAVE_PATH = "label2id.json"
     CLASSES_SAVE_KEY = "class_names"
     MODEL_SELECTOR_ARGS_SAVE_PATH = "model_selector_args.json"
+    ACFT_CONFIG_SAVE_PATH = "finetune_config.json"
+
 
 @dataclass
 class HfConstants:
     """
     A class to represent constants for hugging face files.
     """
     LARGE_MODEL_MAX_LENGTH = 1e6
@@ -63,54 +77,66 @@
     # NOTE ONLY used for Summarization and Translation tasks
     PREFIX_AND_TASK_FILE_SAVE_NAME_WITH_EXT = "azureml_tokenizer_prefix_mlflow_task.json"
     PREFIX_SAVE_KEY = "tokenizer_prefix"
     #
     TASK_SAVE_KEY = "mlflow_task"
     INFERENCE_PARAMS_SAVE_NAME_WITH_EXT = "azureml_mlflow_inference_params.json"
     INFERENCE_PARAMS_SAVE_KEY = "tokenizer_config"
+    INFERENCE_PARAMS_SAVE_KEY_TEXTGEN = "tokenizer_hf_load_kwargs"
     MISC_CONFIG_FILE = "MLmodel"
+    CONDA_YAML_FILE = "conda.yaml"
     MODEL_ROOT_DIRECTORY = "mlflow_model_folder"
     HUGGINGFACE_ID = "huggingface_id"
     LICENSE_FILE = "LICENSE"
+    DEFAULT_MODEL_NAME = "default_model_name"
 
 
 @dataclass
 class AzuremlConstants:
     """
     General constants
     """
     DATASET_COLUMN_PREFIX = "Azureml_"
+    AZUREML_URL_PREFIX = "azureml://"
 
 
 @dataclass
 class HfModelTypes:
     GPT2 = "gpt2"
     ROBERTA = "roberta"
     DEBERTA = "deberta"
     DISTILBERT = "distilbert"
     BERT = "bert"
     BART = "bart"
     MBART = "mbart"
     T5 = "t5"
     CAMEMBERT = "camembert"
     LLAMA = "llama"
+    GPT_NEOX = "gpt_neox"
+    FALCON = "falcon"
+    REFINEDWEBMODEL = "RefinedWebModel"
+    REFINED_WEB = "RefinedWeb"
+    MIXFORMER_SEQUENTIAL = "mixformer-sequential"   # Phi models
+    MISTRAL = "mistral"
+    MIXTRAL = "mixtral"
 
 
 @dataclass
 class Tasks:
     """Supported Tasks"""
     SINGLE_LABEL_CLASSIFICATION = "SingleLabelClassification"
     MULTI_LABEL_CLASSIFICATION = "MultiLabelClassification"
     REGRESSION = "regression"
     NAMED_ENTITY_RECOGNITION = "NamedEntityRecognition"
     PARTS_OF_SPEECH_TAGGING = "PartsOfSpeechTagging"
     CHUNKING = "Chunking"
     SUMMARIZATION = "Summarization"
     TRANSLATION = "Translation"
     QUESTION_ANSWERING = "QuestionAnswering"
+    TEXT_GENERATION = "TextGeneration"
     NLP_NER = "NLPNER"
     NLP_MULTICLASS = "NLPMulticlass"
     NLP_MULTILABEL = "NLPMultilabel"
 
 
 class MLFlowHFFlavourTasks:
     """
@@ -118,14 +144,15 @@
     """
     SINGLE_LABEL_CLASSIFICATION = "text-classification"
     MULTI_LABEL_CLASSIFICATION = "text-classification"
     NAMED_ENTITY_RECOGNITION = "token-classification"
     QUESTION_ANSWERING = "question-answering"
     SUMMARIZATION = "summarization"
     TRANSLATION = "translation"
+    TEXT_GENERATION = "text-generation"
     REGRESSION = "regression"
     CHUNKING = "chunking"
     PARTS_OF_SPEECH_TAGGING = "pos-tagging"
 
 
 # Pyarrow ref
 # https://github.com/huggingface/datasets/blob/9f9f0b536e128710115c486b0b9c319c3f0a570f/src/datasets/features/features.py#L404
@@ -211,20 +238,32 @@
             "help": (
                 "Number of examples to batch before calling the tokenization function. "
                 "This also controls the number of examples to batch while writing to cache and saving to the json file."
             )
         }
     )
 
+    def validate_required_columns(self):
+        if len(self.required_columns) != len(set(self.required_columns)):
+             raise ACFTDataException._with_error(
+                    AzureMLError.create(
+                        ACFTUserError,
+                        pii_safe_message=(
+                            f"Duplicate column name passed:  {(','.join(self.required_columns))}"
+                        )
+                    )
+                )
+
 
 @dataclass
 class TaskConstants:
     NER_IGNORE_INDEX = -100
     TRANSLATION_IGNORE_INDEX = -100
     SUMMARIZATION_IGNORE_INDEX = -100
+    TEXT_GENERATION_IGNORE_INDEX = -100
     MULTI_LABEL_THRESHOLD = 0.5
     MULTI_LABEL_NEW_COLUMN_SUFFIX = "_list"
 
 
 @dataclass
 class DataConstants:
     ENCODING = 'utf-8'
@@ -237,7 +276,53 @@
     LONG_RANGE_MAX = 256
     MIN_PROPORTION_LONG_RANGE = 0.1
     TEXT_CLASSIFICATION_COLUMN_NAME = "sentences"
     TEXT_NER_TOKEN_KEY = "tokens"
     TEXT_NER_TAG_KEY = "ner_tags_str"
     NER_IGNORE_TOKENS = ["", " ", "\n"]
     BATCH_SIZE = 32
+
+
+class ValidationConstants:
+    """All constants related to data validation."""
+    MIN_TRAINING_SAMPLE = 50
+    MIN_TRAINING_SAMPLE_GENERATIVE_TASKS = 10
+
+
+# Following is the deny-list of messages to avoid logging in app-insight.
+# Dev Notes: Add only PII messages to denylist from azureml packages.
+LOGS_TO_BE_FILTERED_IN_APPINSIGHTS = [
+        "Dataset columns after pruning",
+        "loading configuration file",
+        "Model config",
+        "loading file",
+        "Namespace(",
+        "output type to python objects for",
+        "class Names:",
+        "Class names : ",
+        "Metrics calculator:",
+        "The following columns in the training set",
+        # validation filter strings
+        "Dataset Columns: ",
+        "Data formating",
+        "dtype mismatch for feature",
+        "Removing label_column",
+        "Removed columns:",
+        "Converting column:",
+        "Component Args:",
+        "Using client id:"
+    ]
+
+class MLFLOW_FLAVORS:
+    """
+    A class to represent constants for mlflow flavours.
+    """
+    TRANSFORMERS = "transformers"
+    HFTRANSFORMERSV2 = "hftransformersv2"
+    HFTRANSFORMERS = "hftransformers"
+
+
+@dataclass
+class SaveStrategy:
+    EVALUATION_STRATEGY = "evaluation_strategy"
+    EPOCH = "epoch"
+    STEPS = "steps"
```

## azureml/acft/contrib/hf/nlp/nlp_auto/config.py

```diff
@@ -11,20 +11,20 @@
 from __future__ import annotations
 
 import os
 from typing import Optional, Union
 import copy
 from ..constants.constants import HfModelTypes
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from azureml.acft.common_components import get_logger_app
 
 from transformers import AutoConfig, PretrainedConfig
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class AzuremlAutoConfig(AutoConfig):
 
     @classmethod
     def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> PretrainedConfig:
 
@@ -68,18 +68,19 @@
             config.use_cache = False
 
         return config
 
     @staticmethod
     def get_model_type(
         config: Optional[PretrainedConfig] = None,
-        hf_model_name_or_path: Optional[Union[str, os.PathLike]] = None
+        hf_model_name_or_path: Optional[Union[str, os.PathLike]] = None,
+        **kwargs,
     ) -> str:
 
         # PreTrainedConfig has an attribute model_type
         if config is not None:
             return getattr(config, "model_type")
         elif hf_model_name_or_path is not None:
-            config = super(AzuremlAutoConfig, AzuremlAutoConfig).from_pretrained(hf_model_name_or_path)
+            config = super(AzuremlAutoConfig, AzuremlAutoConfig).from_pretrained(hf_model_name_or_path, **kwargs)
             return getattr(config, "model_type")
         else:
             raise ValueError("Pretrained config or model_name_or_path should be present")
```

## azureml/acft/contrib/hf/nlp/nlp_auto/model.py

```diff
@@ -1,166 +1,229 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """
 File containing HF model related functions
 """
+import os
 from pathlib import Path
-from dataclasses import dataclass
 
-from typing import Union, Optional, List, Tuple
+from typing import List, Tuple
 
 import torch
 
 from transformers.models.auto.modeling_auto import (
     AutoModelForSequenceClassification,
     AutoModelForTokenClassification,
     AutoModelForSeq2SeqLM,
-    AutoModelForQuestionAnswering
+    AutoModelForQuestionAnswering,
+    AutoModelForCausalLM,
 )
-from transformers.utils import WEIGHTS_NAME
+from transformers.utils import CONFIG_NAME
 from transformers.modeling_utils import PreTrainedModel
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from transformers import BitsAndBytesConfig
+
+from azureml.acft.common_components import get_logger_app
 
 from .config import AzuremlAutoConfig
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
+
+
+class AzuremlAutoModelBase():
+    @classmethod
+    def get_model_path(cls, hf_model_name_or_path, resume_from_checkpoint):
+        model_path = hf_model_name_or_path
+        if resume_from_checkpoint:
+            if Path(resume_from_checkpoint, CONFIG_NAME).exists():
+                logger.info(f"Found config.json present under resume_from_checkpoint. Will assume resume_from_checkpoint contains full model weights.")
+                model_path = resume_from_checkpoint
+            else:
+                logger.info("No config.json present under resume_from_checkpoint. Will assume lora+peft case where resume_from_checkpoint contains just lora weights (adapter_model.bin).")
+        return model_path
 
 
-class AzuremlAutoModelForSequenceClassification(AutoModelForSequenceClassification):
+# not using Inheritance for Azureml class as while loading auto classes for `trust_remote_code=True` the
+# huggingface classes checks for the parent class name and they must be pre-defined Auto classes of transformers
+# library not any other unknown custom classes
+class AzuremlAutoModelForSequenceClassification(AzuremlAutoModelBase):
 
     @classmethod
     def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> Tuple[PreTrainedModel, str, List[str]]:
         """Apply model specific hacks before calling the Base tokenizer"""
 
         # Initialize the config
         problem_type = kwargs.pop("problem_type", None)
         num_labels = kwargs.pop("num_labels", None)
         label2id = kwargs.pop("label2id", None)
         id2label = kwargs.pop("id2label", None)
-
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
+        ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
+        load_in_8bit = kwargs.pop("load_in_8bit", False)
+        load_in_4bit = kwargs.pop("load_in_4bit", False)
+        if load_in_8bit or load_in_4bit:
+            # Setting device_map to None or {"": torch.cuda.current_device()} is trying to load
+            # the model in GPU 0 always. To avoid that and load the model in all GPUs, :env
+            # variable LOCAL_RANK is passed explicitly
+            kwargs["device_map"] = {"": int(os.environ["LOCAL_RANK"])}
+            logger.info(f'Setting the device map to use the current device GPU: {kwargs["device_map"]}')
+
+        resume_from_checkpoint = kwargs.pop("resume_from_checkpoint", None)
+        model_path = cls.get_model_path(hf_model_name_or_path, resume_from_checkpoint)
+        logger.info(f"Loading config and model from: {model_path}")
         config = AzuremlAutoConfig.from_pretrained(
-            hf_model_name_or_path,
+            model_path,
             problem_type=problem_type,
             num_labels=num_labels,
             id2label=id2label,
             label2id=label2id,
             output_attentions=False,
             output_hidden_states=False,
+            **load_config_kwargs,
         )
-
-        # Initialize the model
-        resume_from_checkpoint = kwargs.get("resume_from_checkpoint", None)
-        model_type = AzuremlAutoConfig.get_model_type(config)
-        if resume_from_checkpoint:
-            # First load the state dictionary to find the keys of pretrained weights
-            # and delete it so that the memory is efficiently used
-            weights_path = Path(hf_model_name_or_path, WEIGHTS_NAME)
-            pretrained_weights_state_dict = torch.load(weights_path, map_location="cpu")
-            pretrained_weights_keys = set(pretrained_weights_state_dict.keys())
-            del pretrained_weights_state_dict
-
-            # will load the model using resume_from_checkpoint of HF TrainingArgs
-            # so instantiating model with random weights for now
-            model = super().from_config(config=config)
-
-            # find the newly initialized layers in the model
-            missing_keys = set(model.state_dict().keys()).difference(pretrained_weights_keys)
-
-            return model, model_type, list(missing_keys)
-        else:
-            model, model_loading_metadata = super().from_pretrained(
-                hf_model_name_or_path,
-                config=config,
-                ignore_mismatched_sizes=kwargs.pop("ignore_mismatched_sizes", False),
-                output_loading_info=True,
+        bnb_config = None
+        if load_in_4bit:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_compute_dtype=torch.bfloat16,
             )
 
-            return model, model_type, model_loading_metadata["missing_keys"]
+        # Initialize the model
+        model_type = AzuremlAutoConfig.get_model_type(config, **load_config_kwargs)
+        model, model_loading_metadata = AutoModelForSequenceClassification.from_pretrained(
+            model_path,
+            config=config,
+            quantization_config=bnb_config,
+            ignore_mismatched_sizes=ignore_mismatched_sizes,
+            output_loading_info=True,
+            **kwargs,
+        )
+        return model, model_type, model_loading_metadata["missing_keys"]
 
 
-class AzuremlAutoModelForTokenClassification(AutoModelForTokenClassification):
+# not using Inheritance for Azureml class as while loading auto classes for `trust_remote_code=True` the 
+# huggingface classes checks for the parent class name and they must be pre-defined Auto classes of transformers 
+# library not any other unknown custom classes
+class AzuremlAutoModelForTokenClassification(AzuremlAutoModelBase):
 
     @classmethod
     def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> Tuple[PreTrainedModel, str, List[str]]:
         """Apply model specific hacks before calling the Base tokenizer"""
 
         # Initialize the config
         problem_type = kwargs.pop("problem_type", None)
         num_labels = kwargs.pop("num_labels", None)
         label2id = kwargs.pop("label2id", None)
         id2label = kwargs.pop("id2label", None)
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
+        ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
+        load_in_8bit = kwargs.pop("load_in_8bit", False)
+        load_in_4bit = kwargs.pop("load_in_4bit", False)
+        if load_in_8bit or load_in_4bit:
+            # Setting device_map to None or {"": torch.cuda.current_device()} is trying to load
+            # the model in GPU 0 always. To avoid that and load the model in all GPUs, :env
+            # variable LOCAL_RANK is passed explicitly
+            kwargs["device_map"] = {"": int(os.environ["LOCAL_RANK"])}
+            logger.info(f'Setting the device map to use the current device GPU: {kwargs["device_map"]}')
+        bnb_config = None
+        if load_in_4bit:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_compute_dtype=(
+                    torch.bfloat16
+                    if torch.cuda.is_bf16_supported() else
+                    torch.float16
+                ),
+            )
 
+        resume_from_checkpoint = kwargs.pop("resume_from_checkpoint", None)
+        model_path = cls.get_model_path(hf_model_name_or_path, resume_from_checkpoint)
+        logger.info(f"Loading config and model from: {model_path}")
         config = AzuremlAutoConfig.from_pretrained(
-            hf_model_name_or_path,
+            model_path,
             problem_type=problem_type,
             num_labels=num_labels,
             id2label=id2label,
             label2id=label2id,
             output_attentions=False,
             output_hidden_states=False,
+            **load_config_kwargs,
         )
 
         # Initialize the model
-        resume_from_checkpoint = kwargs.get("resume_from_checkpoint", None)
-        model_type = AzuremlAutoConfig.get_model_type(config)
-        if resume_from_checkpoint:
-            # First load the state dictionary to find the keys of pretrained weights
-            # and delete it so that the memory is efficiently used
-            weights_path = Path(hf_model_name_or_path, WEIGHTS_NAME)
-            pretrained_weights_state_dict = torch.load(weights_path, map_location="cpu")
-            pretrained_weights_keys = set(pretrained_weights_state_dict.keys())
-            del pretrained_weights_state_dict
-
-            # will load the model using resume_from_checkpoint of HF TrainingArgs
-            # so instantiating model with random weights for now
-            model = super().from_config(config=config)
-
-            # find the newly initialized layers in the model
-            missing_keys = set(model.state_dict().keys()).difference(pretrained_weights_keys)
-
-            return model, model_type, list(missing_keys)
-        else:
-            model, model_loading_metadata = super().from_pretrained(
-                hf_model_name_or_path,
-                config=config,
-                ignore_mismatched_sizes=kwargs.pop("ignore_mismatched_sizes", False),
-                output_loading_info=True,
-            )
-            return model, model_type, model_loading_metadata["missing_keys"]
+        model_type = AzuremlAutoConfig.get_model_type(config, **load_config_kwargs)
+        model, model_loading_metadata = AutoModelForTokenClassification.from_pretrained(
+            model_path,
+            config=config,
+            quantization_config=bnb_config,
+            ignore_mismatched_sizes=ignore_mismatched_sizes,
+            output_loading_info=True,
+            **kwargs,
+        )
+        return model, model_type, model_loading_metadata["missing_keys"]
 
 
-class AzuremlAutoModelForSummarization(AutoModelForSeq2SeqLM):
+# not using Inheritance for Azureml class as while loading auto classes for `trust_remote_code=True` the 
+# huggingface classes checks for the parent class name and they must be pre-defined Auto classes of transformers 
+# library not any other unknown custom classes
+class AzuremlAutoModelForSummarization(AzuremlAutoModelBase):
 
     @classmethod
     def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> Tuple[PreTrainedModel, str, List[str]]:
         """Apply model specific hacks before calling the Base tokenizer"""
 
         # Initialize the config
         problem_type = kwargs.pop("problem_type", None)
         label2id = kwargs.pop("label2id", None)
         id2label = kwargs.pop("id2label", None)
         # not None for t5 models
         tok_prefix = kwargs.pop("tok_prefix", None)
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
+        ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
+        load_in_8bit = kwargs.pop("load_in_8bit", False)
+        load_in_4bit = kwargs.pop("load_in_4bit", False)
+        if load_in_8bit or load_in_4bit:
+            # Setting device_map to None or {"": torch.cuda.current_device()} is trying to load
+            # the model in GPU 0 always. To avoid that and load the model in all GPUs, :env
+            # variable LOCAL_RANK is passed explicitly
+            kwargs["device_map"] = {"": int(os.environ["LOCAL_RANK"])}
+            logger.info(f'Setting the device map to use the current device GPU: {kwargs["device_map"]}')
+
+        bnb_config = None
+        if load_in_4bit:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_compute_dtype=torch.bfloat16,
+            )
 
         config_params = {
             "problem_type": problem_type,
             "id2label": id2label,
             "label2id": label2id,
             "output_attentions": False,
             "output_hidden_states": False,
+            **load_config_kwargs,
         }
 
         if tok_prefix is not None:
             config_params["prefix"] = tok_prefix
 
-        config = AzuremlAutoConfig.from_pretrained(hf_model_name_or_path, **config_params)
+        resume_from_checkpoint = kwargs.pop("resume_from_checkpoint", None)
+        model_path = cls.get_model_path(hf_model_name_or_path, resume_from_checkpoint)
+        logger.info(f"Loading config and model from: {model_path}")
+        config = AzuremlAutoConfig.from_pretrained(model_path, **config_params)
 
         # summarization task specific params
         task_specific_key = "summarization"
         task_specific_params = {
             "early_stopping": False,
             "length_penalty": 1.0,
             "min_length": 0,
@@ -173,43 +236,30 @@
 
         if task_specific_key in config.task_specific_params:
             config.task_specific_params[task_specific_key].update(task_specific_params)
         else:
             config.task_specific_params[task_specific_key] = task_specific_params
 
         # Initialize the model
-        resume_from_checkpoint = kwargs.get("resume_from_checkpoint", None)
-        model_type = AzuremlAutoConfig.get_model_type(config)
-        if resume_from_checkpoint:
-            # First load the state dictionary to find the keys of pretrained weights
-            # and delete it so that the memory is efficiently used
-            weights_path = Path(hf_model_name_or_path, WEIGHTS_NAME)
-            pretrained_weights_state_dict = torch.load(weights_path, map_location="cpu")
-            pretrained_weights_keys = set(pretrained_weights_state_dict.keys())
-            del pretrained_weights_state_dict
-
-            # will load the model using resume_from_checkpoint of HF TrainingArgs
-            # so instantiating model with random weights for now
-            model = super().from_config(config=config)
-
-            # find the newly initialized layers in the model
-            missing_keys = set(model.state_dict().keys()).difference(pretrained_weights_keys)
-
-            return model, model_type, list(missing_keys)
-        else:
-            model, model_loading_metadata = super().from_pretrained(
-                hf_model_name_or_path,
-                config=config,
-                ignore_mismatched_sizes=kwargs.pop("ignore_mismatched_sizes", False),
-                output_loading_info=True,
-            )
-            return model, model_type, model_loading_metadata["missing_keys"]
+        model_type = AzuremlAutoConfig.get_model_type(config, **load_config_kwargs)
+        model, model_loading_metadata = AutoModelForSeq2SeqLM.from_pretrained(
+            model_path,
+            config=config,
+            quantization_config=bnb_config,
+            ignore_mismatched_sizes=ignore_mismatched_sizes,
+            output_loading_info=True,
+            **kwargs,
+        )
+        return model, model_type, model_loading_metadata["missing_keys"]
 
 
-class AzuremlAutoModelForTranslation(AutoModelForSeq2SeqLM):
+# not using Inheritance for Azureml class as while loading auto classes for `trust_remote_code=True` the 
+# huggingface classes checks for the parent class name and they must be pre-defined Auto classes of transformers 
+# library not any other unknown custom classes
+class AzuremlAutoModelForTranslation(AzuremlAutoModelBase):
 
     @classmethod
     def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> Tuple[PreTrainedModel, str, List[str]]:
         """Apply model specific hacks before calling the Base tokenizer"""
 
         # Initialize the config
         problem_type = kwargs.pop("problem_type", None)
@@ -217,29 +267,52 @@
         id2label = kwargs.pop("id2label", None)
         source_lang = kwargs.pop("source_lang", None)
         target_lang = kwargs.pop("target_lang", None)
         # not None for t5 models
         tok_prefix = kwargs.pop("tok_prefix", None)
         # not None for Mbart models
         decoder_start_token_id = kwargs.pop("decoder_start_token_id", None)
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
+        ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
+        load_in_8bit = kwargs.pop("load_in_8bit", False)
+        load_in_4bit = kwargs.pop("load_in_4bit", False)
+        if load_in_8bit or load_in_4bit:
+            # Setting device_map to None or {"": torch.cuda.current_device()} is trying to load
+            # the model in GPU 0 always. To avoid that and load the model in all GPUs, :env
+            # variable LOCAL_RANK is passed explicitly
+            kwargs["device_map"] = {"": int(os.environ["LOCAL_RANK"])}
+            logger.info(f'Setting the device map to use the current device GPU: {kwargs["device_map"]}')
+
+        bnb_config = None
+        if load_in_4bit:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_compute_dtype=torch.bfloat16,
+            )
 
         config_params = {
             "problem_type": problem_type,
             "id2label": id2label,
             "label2id": label2id,
             "output_attentions": False,
             "output_hidden_states": False,
+            **load_config_kwargs,
         }
 
         if tok_prefix is not None:
             config_params["prefix"] = tok_prefix
         if decoder_start_token_id is not None:
             config_params["decoder_start_token_id"] = decoder_start_token_id
 
-        config = AzuremlAutoConfig.from_pretrained(hf_model_name_or_path, **config_params)
+        resume_from_checkpoint = kwargs.pop("resume_from_checkpoint", None)
+        model_path = cls.get_model_path(hf_model_name_or_path, resume_from_checkpoint)
+        logger.info(f"Loading config and model from: {model_path}")
+        config = AzuremlAutoConfig.from_pretrained(model_path, **config_params)
 
         task_specific_key = f"translation_{source_lang}_to_{target_lang}"
         task_specific_params = {
             "early_stopping": False,
             "num_beams": 1,
         }
 
@@ -248,82 +321,130 @@
 
         if task_specific_key in config.task_specific_params:
             config.task_specific_params[task_specific_key].update(task_specific_params)
         else:
             config.task_specific_params[task_specific_key] = task_specific_params
 
         # Initialize the model
-        resume_from_checkpoint = kwargs.get("resume_from_checkpoint", None)
-        model_type = AzuremlAutoConfig.get_model_type(config)
-        if resume_from_checkpoint:
-            # First load the state dictionary to find the keys of pretrained weights
-            # and delete it so that the memory is efficiently used
-            weights_path = Path(hf_model_name_or_path, WEIGHTS_NAME)
-            pretrained_weights_state_dict = torch.load(weights_path, map_location="cpu")
-            pretrained_weights_keys = set(pretrained_weights_state_dict.keys())
-            del pretrained_weights_state_dict
-
-            # will load the model using resume_from_checkpoint of HF TrainingArgs
-            # so instantiating model with random weights for now
-            model = super().from_config(config=config)
-
-            # find the newly initialized layers in the model
-            missing_keys = set(model.state_dict().keys()).difference(pretrained_weights_keys)
-
-            return model, model_type, list(missing_keys)
-        else:
-            model, model_loading_metadata = super().from_pretrained(
-                hf_model_name_or_path,
-                config=config,
-                ignore_mismatched_sizes=kwargs.pop("ignore_mismatched_sizes", False),
-                output_loading_info=True,
-            )
-            return model, model_type, model_loading_metadata["missing_keys"]
+        model_type = AzuremlAutoConfig.get_model_type(config, **load_config_kwargs)
+        model, model_loading_metadata = AutoModelForSeq2SeqLM.from_pretrained(
+            model_path,
+            config=config,
+            quantization_config=bnb_config,
+            ignore_mismatched_sizes=ignore_mismatched_sizes,
+            output_loading_info=True,
+            **kwargs,
+        )
+        return model, model_type, model_loading_metadata["missing_keys"]
 
 
-class AzuremlAutoModelForQnA(AutoModelForQuestionAnswering):
+# not using Inheritance for Azureml class as while loading auto classes for `trust_remote_code=True` the 
+# huggingface classes checks for the parent class name and they must be pre-defined Auto classes of transformers 
+# library not any other unknown custom classes
+class AzuremlAutoModelForQnA(AzuremlAutoModelBase):
 
     @classmethod
     def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> Tuple[PreTrainedModel, str, List[str]]:
         """Apply model specific hacks before calling the Base tokenizer"""
 
         # Initialize the config
         problem_type = kwargs.pop("problem_type", None)
-        label2id = kwargs.pop("label2id", None)
-        id2label = kwargs.pop("id2label", None)
+        # Extractive QnA predicts the start and end logits => number of labels to be 2
+        # The class names is hardcoded here to allow finetuning models that were trained with classes != 2
+        # Refer to this issue for more information https://github.com/huggingface/transformers/issues/22601
+        num_labels = 2
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
+        ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
+        load_in_8bit = kwargs.pop("load_in_8bit", False)
+        load_in_4bit = kwargs.pop("load_in_4bit", False)
+        if load_in_8bit or load_in_4bit:
+            # Setting device_map to None or {"": torch.cuda.current_device()} is trying to load
+            # the model in GPU 0 always. To avoid that and load the model in all GPUs, :env
+            # variable LOCAL_RANK is passed explicitly
+            kwargs["device_map"] = {"": int(os.environ["LOCAL_RANK"])}
+            logger.info(f'Setting the device map to use the current device GPU: {kwargs["device_map"]}')
+        bnb_config = None
+        if load_in_4bit:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_compute_dtype=torch.bfloat16,
+            )
 
+        resume_from_checkpoint = kwargs.pop("resume_from_checkpoint", None)
+        model_path = cls.get_model_path(hf_model_name_or_path, resume_from_checkpoint)
+        logger.info(f"Loading config and model from: {model_path}")
         config = AzuremlAutoConfig.from_pretrained(
-            hf_model_name_or_path,
+            model_path,
             problem_type=problem_type,
-            # id2label=id2label,
-            # label2id=label2id,
+            num_labels=num_labels,
             output_attentions=False,
             output_hidden_states=False,
+            **load_config_kwargs,
         )
 
         # Initialize the model
-        resume_from_checkpoint = kwargs.get("resume_from_checkpoint", None)
-        model_type = AzuremlAutoConfig.get_model_type(config)
-        if resume_from_checkpoint:
-            # First load the state dictionary to find the keys of pretrained weights
-            # and delete it so that the memory is efficiently used
-            weights_path = Path(hf_model_name_or_path, WEIGHTS_NAME)
-            pretrained_weights_state_dict = torch.load(weights_path, map_location="cpu")
-            pretrained_weights_keys = set(pretrained_weights_state_dict.keys())
-            del pretrained_weights_state_dict
-
-            # will load the model using resume_from_checkpoint of HF TrainingArgs
-            # so instantiating model with random weights for now
-            model = super().from_config(config=config)
+        model_type = AzuremlAutoConfig.get_model_type(config, **load_config_kwargs)
+        model, model_loading_metadata = AutoModelForQuestionAnswering.from_pretrained(
+            model_path,
+            config=config,
+            ignore_mismatched_sizes=ignore_mismatched_sizes,
+            quantization_config=bnb_config,
+            output_loading_info=True,
+            **kwargs,
+        )
+        return model, model_type, model_loading_metadata["missing_keys"]
 
-            # find the newly initialized layers in the model
-            missing_keys = set(model.state_dict().keys()).difference(pretrained_weights_keys)
 
-            return model, model_type, list(missing_keys)
-        else:
-            model, model_loading_metadata = super().from_pretrained(
-                hf_model_name_or_path,
-                config=config,
-                ignore_mismatched_sizes=kwargs.pop("ignore_mismatched_sizes", False),
-                output_loading_info=True,
+# not using Inheritance for Azureml class as while loading auto classes for `trust_remote_code=True` the 
+# huggingface classes checks for the parent class name and they must be pre-defined Auto classes of transformers 
+# library not any other unknown custom classes
+class AzuremlAutoModelForCausalLM(AzuremlAutoModelBase):
+
+    @classmethod
+    def from_pretrained(cls, hf_model_name_or_path: str, **kwargs) -> Tuple[PreTrainedModel, str, List[str]]:
+        """Apply model specific hacks before calling the Base tokenizer"""
+
+        # Initialize the config
+        problem_type = kwargs.pop("problem_type", None)
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
+        ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
+        load_in_8bit = kwargs.pop("load_in_8bit", False)
+        load_in_4bit = kwargs.pop("load_in_4bit", False)
+        if load_in_8bit or load_in_4bit:
+            # Setting device_map to None or {"": torch.cuda.current_device()} is trying to load
+            # the model in GPU 0 always. To avoid that and load the model in all GPUs, :env
+            # variable LOCAL_RANK is passed explicitly
+            kwargs["device_map"] = {"": int(os.environ["LOCAL_RANK"])}
+            logger.info(f'Setting the device map to use the current device GPU: {kwargs["device_map"]}')
+        bnb_config = None
+        if load_in_4bit:
+            bnb_config = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_quant_type="nf4",
+                bnb_4bit_use_double_quant=True,
+                bnb_4bit_compute_dtype=torch.bfloat16,
             )
-            return model, model_type, model_loading_metadata["missing_keys"]
+
+        resume_from_checkpoint = kwargs.pop("resume_from_checkpoint", None)
+        model_path = cls.get_model_path(hf_model_name_or_path, resume_from_checkpoint)
+        logger.info(f"Loading config and model from: {model_path}")
+        config = AzuremlAutoConfig.from_pretrained(
+            model_path,
+            problem_type=problem_type,
+            output_attentions=False,
+            output_hidden_states=False,
+            **load_config_kwargs,
+        )
+
+        # Initialize the model
+        model_type = AzuremlAutoConfig.get_model_type(config, **load_config_kwargs)
+        model, model_loading_metadata = AutoModelForCausalLM.from_pretrained(
+            model_path,
+            config=config,
+            quantization_config=bnb_config,
+            ignore_mismatched_sizes=ignore_mismatched_sizes,
+            output_loading_info=True,
+            **kwargs,
+        )
+        return model, model_type, model_loading_metadata["missing_keys"]
```

## azureml/acft/contrib/hf/nlp/nlp_auto/tokenizer.py

```diff
@@ -9,30 +9,30 @@
 from typing import Dict, Any
 
 from transformers import AutoTokenizer, PreTrainedTokenizerBase
 
 from ..constants.constants import HfModelTypes, HfConstants
 from .config import AzuremlAutoConfig
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from azureml.acft.common_components import get_logger_app
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class AzuremlAutoTokenizer(AutoTokenizer):
 
     @staticmethod
-    def pre_init(hf_model_name_or_path: str) -> Dict[str, Any]:
+    def pre_init(hf_model_name_or_path: str, **kwargs) -> Dict[str, Any]:
         """Apply model adjustments before calling the Base tokenizer"""
 
         model_specific_args = {}
 
         # GPT2 specific adjustments for all tasks
-        model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=hf_model_name_or_path)
+        model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=hf_model_name_or_path, **kwargs)
         if model_type == HfModelTypes.GPT2:
             # adding eos_token as pad_token. The value of eos_token is taken from tokenization_gpt2.py file
             model_specific_args["pad_token"] = "<|endoftext|>"
             logger.info(f'Adding pad token to tokenizer init: {model_specific_args["pad_token"]}')
         elif model_type == HfModelTypes.LLAMA:
             # adding eos_token as pad_token. The value of eos_token is taken from tokenization_llama.py file
             model_specific_args["pad_token"] = "</s>"
@@ -47,44 +47,45 @@
         :param kwargs
             The kwargs can't contain arbitrary key-value pairs as most of the kwargs will be sent to tokenizer
             during initialization
         """
 
         apply_adjust = kwargs.pop("apply_adjust", True)
         max_sequence_length = kwargs.pop("max_sequence_length", -1)
+        load_config_kwargs = kwargs.pop("load_config_kwargs", {})
         model_specific_args = kwargs
         if apply_adjust:
             logger.info("Applying model adjustments")
-            model_specific_args.update(AzuremlAutoTokenizer.pre_init(hf_model_name_or_path))
+            model_specific_args.update(AzuremlAutoTokenizer.pre_init(hf_model_name_or_path, **load_config_kwargs))
 
         logger.info(f"Tokenizer initialized with args {model_specific_args}")
+        # fast tokenizer is loaded by default, if not slow tokenizer is loaded
         try:
             # fast tokenizer
             tokenizer = super().from_pretrained(
                 hf_model_name_or_path,
                 use_fast=True,
                 **model_specific_args,
             )
         except Exception as e:
             logger.warning(f"Fast tokenizer not supported: {e}")
             logger.info("Trying default tokenizer.")
             # slow tokenizer
             tokenizer = super().from_pretrained(
-               hf_model_name_or_path,
+                hf_model_name_or_path,
                 **model_specific_args,
             )
         logger.debug("Loaded tokenizer : {}".format(tokenizer))
 
-        if apply_adjust:
-            AzuremlAutoTokenizer.set_model_max_length(tokenizer, max_sequence_length)
+        AzuremlAutoTokenizer.set_model_max_length(tokenizer, max_sequence_length)
 
         return tokenizer
 
     @staticmethod
-    def set_model_max_length(tokenizer: PreTrainedTokenizerBase, max_sequence_length: int=-1) -> None:
+    def set_model_max_length(tokenizer: PreTrainedTokenizerBase, max_sequence_length: int = -1) -> None:
         """Set the model max length to a default value to avoid integer out of bounds error"""
 
         if (
             hasattr(tokenizer, HfConstants.MODEL_MAX_LENGTH_KEY) and
             getattr(tokenizer, HfConstants.MODEL_MAX_LENGTH_KEY) > HfConstants.LARGE_MODEL_MAX_LENGTH
         ):
             logger.info(
```

## azureml/acft/contrib/hf/nlp/tasks/multi_label/runner.py

```diff
@@ -17,46 +17,56 @@
 # ---------------------------------------------------------
 
 from argparse import Namespace
 from typing import List
 
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
-from .preprocess.base import MultiLabelPreprocessArgs
+from .preprocess.base import MultiLabelPreprocessArgs, MultiLabelDataset
 
-# from .preprocess.preprocess_for_inference import MultiLabelPreprocessForInfer
 from ...utils.hf_argparser import HfArgumentParser
 
+from azureml.acft.common_components import get_logger_app
+
+
+logger = get_logger_app(__name__)
+
 
 class MultiLabelRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
         from .preprocess.preprocess_for_finetune import MultiLabelPreprocessForFinetune
 
+        load_config_kwargs = getattr(component_args, "finetune_config", {}).get("load_config_kwargs", {})
         self.check_model_task_compatibility(
-            model_name_or_path=component_args.model_name_or_path, task_name=Tasks.MULTI_LABEL_CLASSIFICATION
+            model_name_or_path=component_args.model_name_or_path,
+            task_name=Tasks.MULTI_LABEL_CLASSIFICATION,
+            **load_config_kwargs,
         )
 
         preprocess_arg_parser = HfArgumentParser([MultiLabelPreprocessArgs])
-        preprocess_args: MultiLabelPreprocessArgs = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args)[0]
+        output_args = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args, return_remaining_strings=True)
+        preprocess_args: MultiLabelPreprocessArgs = output_args[0]
+
+        logger.info(f"unused args - {output_args[1]}")
 
         preprocess_obj = MultiLabelPreprocessForFinetune(component_args, preprocess_args)
         preprocess_obj.preprocess()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         pass
 
     def run_finetune(self, component_plus_preprocess_args: Namespace) -> None:
 
         from .finetune.finetune import MultiLabelFinetune
 
         self.resolve_resume_from_checkpoint(component_plus_preprocess_args)
 
-        finetune_obj = MultiLabelFinetune(vars(component_plus_preprocess_args))
+        finetune_obj = MultiLabelFinetune(vars(component_plus_preprocess_args), MultiLabelDataset)
         finetune_obj.finetune()
 
     def run_modelselector(self, *args, **kwargs) -> None:
 
         from ...utils.model_selector_utils import model_selector
 
         model_selector(kwargs)
```

## azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/finetune.py

```diff
@@ -15,82 +15,87 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 import json
 import numpy as np
 from pathlib import Path
+import shutil
 
 from typing import Any, Dict, List, Tuple, Optional
 
+from ...base.finetune.finetune import FinetuneBase
 from ....constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, TaskConstants, Tasks
 from ....nlp_auto.model import AzuremlAutoModelForSequenceClassification
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ..preprocess.base import MultiLabelDataset
-from ....utils.mlflow_utils import SaveMLflowModelCallback, replace_deepspeed_zero3_mlflow_pytorch_weights
+from ....utils.common_utils import write_dict_to_json_file
 
 import torch.nn as nn
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-
 from azureml.acft.accelerator.finetune import AzuremlFinetuneArgs, AzuremlDatasetArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
 from azureml.acft.accelerator.constants import HfTrainerType
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_utils import EvalPrediction
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 
 import torch
 from sklearn.metrics import (
     f1_score,
     accuracy_score,
     roc_auc_score,
     precision_score,
     recall_score
 )
 
+from peft import TaskType
+
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
-class MultiLabelFinetune:
+class MultiLabelFinetune(FinetuneBase):
 
-    def __init__(self, finetune_params: Dict[str, Any]) -> None:
+    def __init__(self, finetune_params: Dict[str, Any], dataset_class) -> None:
         # finetune params is finetune component args + args saved as part of preprocess
         self.finetune_params = finetune_params
+        self.dataset_class = dataset_class
+        self.ft_config = finetune_params.get("finetune_config", {})
 
         logger.info(f"Task name: {Tasks.MULTI_LABEL_CLASSIFICATION}")
 
         # Load class names
         class_names_load_path = Path(self.finetune_params["preprocess_output"], SaveFileConstants.CLASSES_SAVE_PATH)
         with open(class_names_load_path, 'r') as rptr:
             self.finetune_params["class_names"] = json.load(rptr)[SaveFileConstants.CLASSES_SAVE_KEY]
             self.finetune_params["num_labels"] = len(self.finetune_params["class_names"])
 
         # set log_metrics_at_root=False to not to log to parent
-        self.finetune_params["log_metrics_at_root"] = False
+        self.finetune_params["log_metrics_at_root"] = True
 
     def _get_finetune_args(self, model_type: str) -> AzuremlFinetuneArgs:
 
         self.finetune_params["model_type"] = model_type
+        self.finetune_params["peft_task_type"] = TaskType.SEQ_CLS
         azml_trainer_finetune_args = AzuremlFinetuneArgs(
             self.finetune_params,
-            trainer_type=HfTrainerType.DEFAULT
+            trainer_type=HfTrainerType.DEFAULT,
         )
 
         return azml_trainer_finetune_args
 
     def _get_dataset_args(self, tokenizer: Optional[PreTrainedTokenizerBase] = None) -> AzuremlDatasetArgs:
 
-        encoded_train_ds = MultiLabelDataset(
+        encoded_train_ds = self.dataset_class(
             Path(self.finetune_params["preprocess_output"], self.finetune_params["encoded_train_data_fname"]),
             tokenizer=tokenizer
         )
-        encoded_validation_ds = MultiLabelDataset(
+        encoded_validation_ds = self.dataset_class(
             Path(self.finetune_params["preprocess_output"], self.finetune_params["encoded_validation_data_fname"]),
         )
         azml_trainer_dataset_args = AzuremlDatasetArgs(
             train_dataset=encoded_train_ds.dataset,
             validation_dataset=encoded_validation_ds.dataset,
             data_collator=encoded_train_ds.get_collation_function()
         )
@@ -105,88 +110,96 @@
         model_params = {
             "problem_type": "multi_label_classification",
             "num_labels": self.finetune_params["num_labels"],
             "id2label": id2label,
             "label2id": label2id,
             "ignore_mismatched_sizes": self.finetune_params["ignore_mismatched_sizes"],
             "resume_from_checkpoint": self.finetune_params["resume_from_checkpoint"],
+            "load_in_8bit": self.finetune_params["finetune_in_8bit"],
+            "load_in_4bit": self.finetune_params["finetune_in_4bit"],
         }
 
+        model_params.update(self.ft_config.get("load_model_kwargs", {}))
+        model_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading model with following args: {model_params}")
+
         model, model_type, new_initalized_layers = AzuremlAutoModelForSequenceClassification.from_pretrained(
             self.finetune_params["model_name_or_path"], **model_params)
 
         return model, model_type, new_initalized_layers
 
     def _get_tokenizer(self) -> PreTrainedTokenizerBase:
         """This method loads the tokenizer as is w/o any modifications to it"""
 
         tokenizer_params = {
             "apply_adjust": False,
             "task_name": self.finetune_params["task_name"],
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading tokenizer with following params: {tokenizer_params}")
+
         return AzuremlAutoTokenizer.from_pretrained(self.finetune_params["preprocess_output"], **tokenizer_params)
 
     def finetune(self) -> None:
 
-        # configure MLflow save callback
-        mlflow_infer_params_file_path = Path(
-            self.finetune_params["preprocess_output"], MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT
-        )
-        save_mlflow_callback = SaveMLflowModelCallback(
-            mlflow_infer_params_file_path=mlflow_infer_params_file_path,
-            mlflow_model_save_path=self.finetune_params["mlflow_model_folder"],
-            mlflow_task_type=self.finetune_params["mlflow_task_type"],
-            class_names=self.finetune_params["class_names"],
-            model_name=self.finetune_params["model_name"],
-            model_name_or_path=self.finetune_params["model_name_or_path"],
-        )
-
+        # Initializing the finetune args with dummy_model_type to enable the
+        # deepspeed stage3 which is used in :meth _load_model
+        finetune_args = self._get_finetune_args("dummy_model_type")
         model, model_type, new_initialized_params = self._load_model()
+        # Replacing the dummy_model_type -> original model_type information
+        setattr(finetune_args.optimization_args, "model_type", model_type)
+        self.finetune_params["model_type"] = model_type
         tokenizer = self._get_tokenizer()
         trainer = AzuremlTrainer(
-            finetune_args=self._get_finetune_args(model_type),
+            finetune_args=finetune_args,
             dataset_args=self._get_dataset_args(tokenizer),
             model=model,
             tokenizer=tokenizer,
             metric_func=multi_label_metrics_func,
             new_initalized_layers=new_initialized_params,
-            custom_trainer_callbacks=[save_mlflow_callback],
         )
 
+        self._save_mininum_finetune_args(finetune_args)
+
         # Torch barrier is used to complete the training on a distributed setup
         # Use callbacks for adding steps to be done at the end of training
         # NOTE Avoid adding any logic after trainer.train()
         # Test the distributed scenario in case you add any logic beyond trainer.train()
         trainer.train()
 
-        # replace pytorch weights for lora / deep speed zero3 optimization
-        if trainer.should_save and (self.finetune_params["apply_lora"] or is_deepspeed_zero3_enabled()):
-            logger.info("Replacing dummy MLflow weights ")
-            replace_deepspeed_zero3_mlflow_pytorch_weights(
-                self.finetune_params["pytorch_model_folder"],
-                self.finetune_params["mlflow_model_folder"]
-            )
-
         # save files only once by Rank-0 process
         if trainer.should_save:
-            # save finetune args
-            Path(self.finetune_params["pytorch_model_folder"]).mkdir(exist_ok=True, parents=True)
-            finetune_args_path = Path(self.finetune_params["pytorch_model_folder"], \
-                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
             self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
-            with open(finetune_args_path, 'w') as rptr:
-                json.dump(self.finetune_params, rptr, indent=2)
+            # save if model is trained via deepspeed stage 3
+            self.finetune_params["is_deepspeed_zero3_enabled"] = is_deepspeed_zero3_enabled()
+            # save finetune args
+            finetune_args_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH))
+            write_dict_to_json_file(self.finetune_params, finetune_args_path)
             # save the classes list for azmlft inference compatability
-            classes_save_path = Path(self.finetune_params["pytorch_model_folder"], SaveFileConstants.CLASSES_SAVE_PATH)
+            classes_save_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.CLASSES_SAVE_PATH))
             class_names_json = {SaveFileConstants.CLASSES_SAVE_KEY: self.finetune_params["class_names"]}
-            with open(classes_save_path, "w") as wptr:
-                json.dump(class_names_json, wptr)
+            write_dict_to_json_file(class_names_json, classes_save_path)
             logger.info(f"Classes file saved at {classes_save_path}")
 
+            # save finetune_config file
+            ft_config_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.ACFT_CONFIG_SAVE_PATH))
+            write_dict_to_json_file(self.ft_config, ft_config_path)
+
+            # copy mlflow inference params file to pytorch output for model converter
+            mlflow_infer_params_file_path = Path(
+                self.finetune_params["preprocess_output"],
+                MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT,
+            )
+            shutil.copy(mlflow_infer_params_file_path, self.finetune_params["pytorch_model_folder"])
+
 
 def multi_label_metrics_func(eval_pred: EvalPrediction) -> Dict[str, Any]:
     """
     compute and return metrics for sequence classification
     # source: https://jesusleal.io/2021/04/21/Longformer-multilabel-classification/
     """
```

## azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/base.py

```diff
@@ -19,38 +19,41 @@
 import ast
 from pathlib import Path
 
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 from sklearn.preprocessing import MultiLabelBinarizer
 
-from ....constants.constants import DatasetSplit, SaveFileConstants, AzuremlConstants, MLFlowHFFlavourConstants, PreprocessArgsTemplate
-from ....constants.constants import Tasks, MLFlowHFFlavourTasks, HfModelTypes
-from ....constants.constants  import STRING_DTYPES
-from ....base_runner import BaseRunner
+from ....constants.constants import (
+    AzuremlConstants,
+    MLFlowHFFlavourTasks,
+    PreprocessArgsTemplate,
+    TaskConstants,
+    Tasks,
+    STRING_DTYPES
+)
 
-from ....utils.data_utils import AzuremlDataset
+from ....utils.data_utils import AzuremlDataset, clean_column_name
 from ....utils.validation_utils import AzuremlValidatorMixin
-from ....constants.constants import TaskConstants
 
 from datasets.arrow_dataset import Dataset
 from datasets import Sequence
 
-import transformers
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorWithPadding
-from transformers.hf_argparser import HfArgumentParser
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.contrib.hf.nlp.constants.constants import DataSliceConstants
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class MultiLabelPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of MultiLabelPreprocessArgs +
     # inhertied attributes from _PreprocessArgsTemplate here.
     # Otherwise, there will be issues related to ordering of default and
@@ -105,32 +108,34 @@
             STRING_DTYPES, STRING_DTYPES, STRING_DTYPES
         ]
         #
         if self.placeholder_required_columns is not None:
             for idx, col_name in enumerate(self.placeholder_required_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
-                    self.required_columns.append(decoded_arg)
+                    cleaned_name = clean_column_name(decoded_arg)
+                    setattr(self, col_name, cleaned_name)  # reset with cleaned name for further use
+                    self.required_columns.append(cleaned_name)
                     self.required_column_dtypes.append(self.placeholder_required_column_dtypes[idx])
-
+        self.validate_required_columns()
         self.label_column = getattr(self, self.placeholder_label_column)
 
 
 class MultiLabelDataset(AzuremlDataset, AzuremlValidatorMixin):
 
     def __init__(
         self,
         path_or_dict: Union[str, Path],
         dataset_args: Optional[Dict[str, Any]] = None,
         required_columns: Optional[List[str]] = None,
         required_column_dtypes: Optional[List[List[str]]] = None,
         label_column: Optional[str] = None,
         label_column_optional: bool = False,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
-        slice: str = "train",
+        slice: str = DataSliceConstants.NO_SPLIT,
     ) -> None:
         # required_columns, required_column_dtypes are made optional to support loading the dataset
         # without the need for validation
 
         # special column is added for multi-label after the label_data is decoded and converted to list of string
         new_label_column = None
         if label_column is not None and dataset_args is not None and required_columns is not None and required_column_dtypes is not None:
@@ -234,18 +239,18 @@
             return examples
 
         item_decode_list = []
         for item in examples[self.old_label_column]:
             try:
                 item_decode = ast.literal_eval(item)
             except Exception as e:
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=f"Data is incorrectly formatted. Error while using ast eval: {e}"
+                        ACFTUserError,
+                        pii_safe_message=f"Data is incorrectly formatted. Error while using ast eval: {e}"
                     )
                 )
 
             if not (
                 isinstance(item_decode, List) and
                 (item_decode and isinstance(item_decode[0], str))
             ):
@@ -264,20 +269,20 @@
             if self.dataset_args["sentence2_key"] is not None:
                 self.dataset_args["sentence2_key"] = AzuremlConstants.DATASET_COLUMN_PREFIX + self.dataset_args["sentence2_key"]
             if self.dataset_args["label_key"] is not None:
                 self.dataset_args["label_key"] = AzuremlConstants.DATASET_COLUMN_PREFIX + self.dataset_args["label_key"]
 
         return super().update_dataset_columns_with_prefix()
 
-    def load(self) -> Dataset:
+    def load(self, slice: str = DataSliceConstants.NO_SPLIT) -> Dataset:
         """
         Load the dataset and add a dummy column for the new column
         new column will a list of strings which will be a decoded column of string input
         """
-        dataset = super().load()
+        dataset = super().load(slice)
 
         # add a dummy column with list of strings dtype
         dataset = dataset.add_column(
             name=self.label_column,
             column=[[""]] * len(dataset)
         )
 
@@ -306,18 +311,18 @@
             filter_lambda,
             batch_size=self.dataset_args["batch_size"],
             writer_batch_size=self.dataset_args["batch_size"]
         )
         post_filter_rows = self.dataset.num_rows
         logger.info(f"Multilabel data filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
                 )
             )
 
     def check_column_dtypes(self) -> None:
         """
         check the keep columns with keep column dtypes and raise error otherwise
         """
@@ -329,53 +334,49 @@
                     f"{column_name} not present in column to dtypes map file."
                     f"The following columns are present: {list(datset_features.keys())}"
                 )
 
             if column_name == self.label_column:
                 sequence_column_type = isinstance(datset_features[column_name], Sequence)
                 if not sequence_column_type:
-                    raise ValidationException._with_error(
+                    raise ACFTDataException._with_error(
                         AzureMLError.create(
-                            ValidationError,
-                            error=(
+                            ACFTUserError,
+                            pii_safe_message=(
                                 f"File path or data: {self.path_or_dict}\n"
                                 f"type mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                                 f"Found type: {type(datset_features[column_name])}\n"
                                 f"Expected type: {Sequence}"
                             )
                         )
                     )
                 column_dtype = datset_features[column_name].feature.dtype
             else:
                 column_dtype = datset_features[column_name].dtype
             if column_dtype not in valid_dtypes:
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"File path or data: {self.path_or_dict}\n"
                             f"dtype mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                             f"Found dtype: {column_dtype}\n"
                             f"Expected dtypes: {valid_dtypes}"
                         )
                     )
                 )
 
-    def validate(self):
-
+    def validate(self, split: Optional[str] = None):
         if self.dataset_args is None:
             logger.info(f"Dataset args is {self.dataset_args}. Skipping multilabel validate")
             return
 
-        # Remove the extra columns and match the remaining columns
-        self.remove_extra_columns()
-        self.match_columns()
-
-        # filter data
-        # null filter
-        self.remove_null_examples(batch_size=self.dataset_args["batch_size"])
+        self.apply_common_validations(split, batch_size=self.dataset_args["batch_size"])
+
+        # check if feature columns are identical
+        self.check_column_contents(self.dataset_args["sentence1_key"], self.dataset_args["sentence2_key"])
         # check dtypes
         # NOTE doing dtype check before task specific data filter because :meth multi_label_data_filter
         # assumes the dtypes for columns
         self.check_column_dtypes()
         # remove empty sentence1 or sentence2
         self.multi_label_data_filter()
```

## azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_finetune.py

```diff
@@ -25,51 +25,58 @@
 import json
 
 from .base import MultiLabelPreprocessArgs, MultiLabelDataset
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....constants.constants import Tasks, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class MultiLabelPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: MultiLabelPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
         #  - model_name arg from model selector
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
+        self.ft_config = getattr(component_args, "finetune_config", {})
 
         logger.info(f"Task name: {Tasks.MULTI_LABEL_CLASSIFICATION}")
 
-        self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
+        self.model_type = AzuremlAutoConfig.get_model_type(
+            hf_model_name_or_path=component_args.model_name_or_path,
+            **self.ft_config.get("load_config_kwargs", {}),
+        )
         logger.info(self.preprocess_args)
 
         self.tokenizer = self._init_tokenizer()
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.MULTI_LABEL_CLASSIFICATION,
             "apply_adjust": True,
-            "max_sequence_length": self.preprocess_args.max_seq_length
+            "max_sequence_length": self.preprocess_args.max_seq_length,
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+
         return AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
 
     def _get_encode_dataset_params(self) -> Dict[str, Any]:
 
         encode_params = {}
         # padding and truncation
         encode_params["padding"] = "max_length" if self.preprocess_args.pad_to_max_length else False
@@ -211,34 +218,34 @@
     def _validate_data_splits(self):
         """
         1. validate the datasets
         2. Identify the classnames and do some validations on them
         """
         # validate the datasets
         logger.info("Validating the train dataset")
-        self.train_ds.validate()
+        self.train_ds.validate(DatasetSplit.TRAIN)
         logger.info("Validating the validation dataset")
-        self.valid_ds.validate()
+        self.valid_ds.validate(DatasetSplit.VALIDATION)
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             logger.info("Validating the test dataset")
-            self.test_ds.validate()
+            self.test_ds.validate(DatasetSplit.TEST)
 
         # Identify the class names - combination of train and validation datasets
         # class names are list of strings
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))  # type: ignore
         # few classes to do classification
         if len(self.class_names_train_plus_valid) < 2:
-            raise ValidationException._with_error(AzureMLError.create(InvalidDataset))
+            raise ACFTDataException._with_error(AzureMLError.create(InvalidDataset))
         logger.info(f"Identified class names: {self.class_names_train_plus_valid}")
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             self.class_names_test= self.test_ds.class_names
             # test ds has extra classes that are not in train and valid
             test_ds_extra_labels = set(self.class_names_test).difference(set(self.class_names_train_plus_valid))  # type: ignore
             if test_ds_extra_labels:
-                raise ValidationException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
+                raise ACFTDataException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset(class_names_train_plus_valid=self.class_names_train_plus_valid)
```

## azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_inference.py

```diff
@@ -18,22 +18,20 @@
 
 from argparse import Namespace
 
 from .base import NerPreprocessArgs
 from ...constants.constants import Tasks
 from ...nlp_auto.tokenizer import AzuremlAutoTokenizer
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForInfer():
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
```

## azureml/acft/contrib/hf/nlp/tasks/ner/runner.py

```diff
@@ -21,31 +21,43 @@
 """
 
 from argparse import Namespace
 from typing import List
 
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
-from .preprocess.base import NerPreprocessArgs
+from .preprocess.base import NerPreprocessArgs, NerDataset
 from .preprocess.preprocess_for_inference import NerPreprocessForInfer
 
 from transformers.hf_argparser import HfArgumentParser
 
+from azureml.acft.common_components import get_logger_app
+
+
+logger = get_logger_app(__name__)
+
 
 class NerRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
         from .preprocess.preprocess_for_finetune import NerPreprocessForFinetune
 
+        load_config_kwargs = getattr(component_args, "finetune_config", {}).get("load_config_kwargs", {})
         self.check_model_task_compatibility(
-            model_name_or_path=component_args.model_name_or_path, task_name=Tasks.NAMED_ENTITY_RECOGNITION)
+            model_name_or_path=component_args.model_name_or_path,
+            task_name=Tasks.NAMED_ENTITY_RECOGNITION,
+            **load_config_kwargs,
+        )
 
         preprocess_arg_parser = HfArgumentParser([NerPreprocessArgs])
-        preprocess_args: NerPreprocessArgs = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args)[0]
+        output_args = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args, return_remaining_strings=True)
+        preprocess_args: NerPreprocessArgs = output_args[0]
+
+        logger.info(f"unused args - {output_args[1]}")
 
         preprocess_obj = NerPreprocessForFinetune(component_args, preprocess_args)
         preprocess_obj.preprocess()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         data = [x.split() for x in kwargs["data"]]
         model_name_or_path = kwargs["tokenizer_path"]
@@ -61,15 +73,15 @@
 
     def run_finetune(self, component_plus_preprocess_args: Namespace) -> None:
 
         from .finetune.finetune import NerFinetune
 
         self.resolve_resume_from_checkpoint(component_plus_preprocess_args)
 
-        finetune_obj = NerFinetune(vars(component_plus_preprocess_args))
+        finetune_obj = NerFinetune(vars(component_plus_preprocess_args), NerDataset)
         finetune_obj.finetune()
 
     def run_modelselector(self, *args, **kwargs) -> None:
 
         from ...utils.model_selector_utils import model_selector
 
         model_selector(kwargs)
```

## azureml/acft/contrib/hf/nlp/tasks/ner/finetune/finetune.py

```diff
@@ -20,75 +20,81 @@
 NER
 """
 
 import json
 import numpy as np
 from pathlib import Path
 from functools import partial
+import shutil
 
 from typing import Any, Dict, List, Tuple, Optional
 
-from ..preprocess.base import NerDataset
+from ...base.finetune.finetune import FinetuneBase
 from ....constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, TaskConstants, Tasks
 from ....nlp_auto.model import AzuremlAutoModelForTokenClassification
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ....utils.mlflow_utils import SaveMLflowModelCallback, replace_deepspeed_zero3_mlflow_pytorch_weights
+from ....utils.common_utils import write_dict_to_json_file
 
 import torch.nn as nn
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-
 from azureml.acft.accelerator.finetune import AzuremlFinetuneArgs, AzuremlDatasetArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
 from azureml.acft.accelerator.constants import HfTrainerType
 
+from azureml.acft.common_components import get_logger_app
+
 from datasets.load import load_metric
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_utils import EvalPrediction
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 
+from peft import TaskType
 
-logger = get_logger_app()
 
+logger = get_logger_app(__name__)
 
-class NerFinetune:
 
-    def __init__(self, finetune_params: Dict[str, Any]) -> None:
+class NerFinetune(FinetuneBase):
+
+    def __init__(self, finetune_params: Dict[str, Any], dataset_class) -> None:
         # finetune params is finetune component args + args saved as part of preprocess
         self.finetune_params = finetune_params
+        self.dataset_class = dataset_class
+        self.ft_config = finetune_params.get("finetune_config", {})
 
         logger.info(f"Task name: {Tasks.NAMED_ENTITY_RECOGNITION}")
 
         # Load class names
         class_names_load_path = Path(self.finetune_params["preprocess_output"], SaveFileConstants.CLASSES_SAVE_PATH)
         with open(class_names_load_path, 'r') as rptr:
             self.finetune_params["class_names"] = json.load(rptr)[SaveFileConstants.CLASSES_SAVE_KEY]
             self.finetune_params["num_labels"] = len(self.finetune_params["class_names"])
 
         # set log_metrics_at_root=False to not to log to parent
-        self.finetune_params["log_metrics_at_root"] = False
+        self.finetune_params["log_metrics_at_root"] = True
 
     def _get_finetune_args(self, model_type: str) -> AzuremlFinetuneArgs:
 
         self.finetune_params["model_type"] = model_type
+        self.finetune_params["peft_task_type"] = TaskType.TOKEN_CLS
         azml_trainer_finetune_args = AzuremlFinetuneArgs(
             self.finetune_params,
-            trainer_type=HfTrainerType.DEFAULT
+            trainer_type=HfTrainerType.DEFAULT,
         )
 
         return azml_trainer_finetune_args
 
     def _get_dataset_args(self, tokenizer: Optional[PreTrainedTokenizerBase] = None) -> AzuremlDatasetArgs:
 
-        encoded_train_ds = NerDataset(
+        encoded_train_ds = self.dataset_class(
             str(Path(self.finetune_params["preprocess_output"], self.finetune_params["encoded_train_data_fname"])),
             tokenizer=tokenizer
         )
-        encoded_validation_ds = NerDataset(
+        encoded_validation_ds = self.dataset_class(
             str(Path(self.finetune_params["preprocess_output"], self.finetune_params["encoded_validation_data_fname"])),
         )
         azml_trainer_dataset_args = AzuremlDatasetArgs(
             train_dataset=encoded_train_ds.dataset,
             validation_dataset=encoded_validation_ds.dataset,
             data_collator=encoded_train_ds.get_collation_function()
         )
@@ -103,91 +109,99 @@
         model_params = {
             "problem_type": "single_label_classification",
             "num_labels": self.finetune_params["num_labels"],
             "id2label": id2label,
             "label2id": label2id,
             "ignore_mismatched_sizes": self.finetune_params["ignore_mismatched_sizes"],
             "resume_from_checkpoint": self.finetune_params["resume_from_checkpoint"],
+            "load_in_8bit": self.finetune_params["finetune_in_8bit"],
+            "load_in_4bit": self.finetune_params["finetune_in_4bit"],
         }
 
+        model_params.update(self.ft_config.get("load_model_kwargs", {}))
+        model_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading model with following args: {model_params}")
+
         model, model_type, new_initalized_layers = AzuremlAutoModelForTokenClassification.from_pretrained(
             self.finetune_params["model_name_or_path"], **model_params)
 
         return model, model_type, new_initalized_layers
 
     def _get_tokenizer(self) -> PreTrainedTokenizerBase:
         """This method loads the tokenizer as is w/o any modifications to it"""
 
         tokenizer_params = {
             "apply_adjust": False,
             "task_name": self.finetune_params["task_name"],
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading tokenizer with following params: {tokenizer_params}")
+
         return AzuremlAutoTokenizer.from_pretrained(self.finetune_params["preprocess_output"], **tokenizer_params)
 
     def finetune(self) -> None:
 
-        # configure MLflow save callback
-        mlflow_infer_params_file_path = Path(
-            self.finetune_params["preprocess_output"], MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT
-        )
-        save_mlflow_callback = SaveMLflowModelCallback(
-            mlflow_infer_params_file_path=mlflow_infer_params_file_path,
-            mlflow_model_save_path=self.finetune_params["mlflow_model_folder"],
-            mlflow_task_type=self.finetune_params["mlflow_task_type"],
-            class_names=self.finetune_params["class_names"],
-            model_name=self.finetune_params["model_name"],
-            model_name_or_path=self.finetune_params["model_name_or_path"],
-        )
-
+        # Initializing the finetune args with dummy_model_type to enable the
+        # deepspeed stage3 which is used in :meth _load_model
+        finetune_args = self._get_finetune_args("dummy_model_type")
         model, model_type, new_initialized_params = self._load_model()
+        # Replacing the dummy_model_type -> original model_type information
+        setattr(finetune_args.optimization_args, "model_type", model_type)
+        self.finetune_params["model_type"] = model_type
         tokenizer = self._get_tokenizer()
         trainer = AzuremlTrainer(
-            finetune_args=self._get_finetune_args(model_type),
+            finetune_args=finetune_args,
             dataset_args=self._get_dataset_args(tokenizer),
             model=model,
             tokenizer=tokenizer,
             metric_func=partial(
                 ner_metrics_func,
                 class_names=self.finetune_params["class_names"]
             ),
             new_initalized_layers=new_initialized_params,
-            custom_trainer_callbacks=[save_mlflow_callback],
         )
 
+        self._save_mininum_finetune_args(finetune_args)
+
         # Torch barrier is used to complete the training on a distributed setup
         # Use callbacks for adding steps to be done at the end of training
         # NOTE Avoid adding any logic after trainer.train()
         # Test the distributed scenario in case you add any logic beyond trainer.train()
         trainer.train()
 
-        # replace pytorch weights for lora / deep speed zero3 optimization
-        if trainer.should_save and (self.finetune_params["apply_lora"] or is_deepspeed_zero3_enabled()):
-            logger.info("Replacing dummy MLflow weights ")
-            replace_deepspeed_zero3_mlflow_pytorch_weights(
-                self.finetune_params["pytorch_model_folder"],
-                self.finetune_params["mlflow_model_folder"]
-            )
-
         # save files only once by Rank-0 process
         if trainer.should_save:
-            # saving the args before the finetune to avoid issues related to distributed training
-            Path(self.finetune_params["pytorch_model_folder"]).mkdir(exist_ok=True, parents=True)
-            finetune_args_path = Path(
-                self.finetune_params["pytorch_model_folder"], SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
             self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
-            with open(finetune_args_path, 'w') as rptr:
-                json.dump(self.finetune_params, rptr, indent=2)
+            # save if model is trained via deepspeed stage 3
+            self.finetune_params["is_deepspeed_zero3_enabled"] = is_deepspeed_zero3_enabled()
+            # save finetune args
+            finetune_args_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH))
+            write_dict_to_json_file(self.finetune_params, finetune_args_path)
             # save the classes list for azmlft inference compatability
-            classes_save_path = Path(self.finetune_params["pytorch_model_folder"], SaveFileConstants.CLASSES_SAVE_PATH)
+            classes_save_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.CLASSES_SAVE_PATH))
             class_names_json = {SaveFileConstants.CLASSES_SAVE_KEY: self.finetune_params["class_names"]}
-            with open(classes_save_path, "w") as wptr:
-                json.dump(class_names_json, wptr)
+            write_dict_to_json_file(class_names_json, classes_save_path)
             logger.info(f"Classes file saved at {classes_save_path}")
 
+            # save finetune_config file
+            ft_config_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.ACFT_CONFIG_SAVE_PATH))
+            write_dict_to_json_file(self.ft_config, ft_config_path)
+
+            # copy mlflow inference params file to pytorch output for model converter
+            mlflow_infer_params_file_path = Path(
+                self.finetune_params["preprocess_output"],
+                MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT,
+            )
+            shutil.copy(mlflow_infer_params_file_path, self.finetune_params["pytorch_model_folder"])
+
 
 def ner_metrics_func(eval_pred: EvalPrediction, class_names: List[str]) -> Dict:
     """Compute and return metrics for Named Entity Recognition"""
 
     metric = load_metric("seqeval")
 
     predictions, labels = eval_pred
```

## azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/base.py

```diff
@@ -21,32 +21,38 @@
 """
 
 from pathlib import Path
 
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 
+from ....constants.constants import (
+    AzuremlConstants,
+    MLFlowHFFlavourTasks,
+    PreprocessArgsTemplate,
+    TaskConstants,
+    Tasks,
+    STRING_DTYPES
+)
 
-from ....constants.constants import AzuremlConstants, PreprocessArgsTemplate
-from ....constants.constants import Tasks, MLFlowHFFlavourTasks, STRING_DTYPES, TaskConstants
-
-from ....utils.data_utils import AzuremlDataset
+from ....utils.data_utils import AzuremlDataset, clean_column_name
 from ....utils.validation_utils import AzuremlValidatorMixin
 
 from datasets import Sequence
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorForTokenClassification
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class NerPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of NerPreprocessArgs + inhertied attributes from
     # _PreprocessArgsTemplate here. Otherwise, there will be issues related to ordering of default and
     # non-default attributes
@@ -97,17 +103,19 @@
         self.placeholder_required_columns = ["token_key", "tag_key"]
         self.placeholder_required_column_dtypes = [STRING_DTYPES, STRING_DTYPES]
         #
         if self.placeholder_required_columns is not None:
             for idx, col_name in enumerate(self.placeholder_required_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
-                    self.required_columns.append(decoded_arg)
+                    cleaned_name = clean_column_name(decoded_arg)
+                    setattr(self, col_name, cleaned_name)  # reset with cleaned name for further use
+                    self.required_columns.append(cleaned_name)
                     self.required_column_dtypes.append(self.placeholder_required_column_dtypes[idx])
-
+        self.validate_required_columns()
         self.label_column = getattr(self, self.placeholder_label_column)
 
 
 class NerDataset(AzuremlDataset, AzuremlValidatorMixin):
 
     def __init__(
         self,
@@ -239,18 +247,18 @@
             filter_lambda,
             batch_size=self.dataset_args["batch_size"],
             writer_batch_size=self.dataset_args["batch_size"]
         )
         post_filter_rows = self.dataset.num_rows
         logger.info(f"Ner data filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
                 )
             )
 
     def check_column_dtypes(self) -> None:
         """
         check the keep columns with keep column dtypes and raise error otherwise
         """
@@ -261,47 +269,41 @@
                 raise ValueError(
                     f"{column_name} not present in column to dtypes map file."
                     f"The following columns are present: {list(datset_features.keys())}"
                 )
 
             sequence_column_type = isinstance(datset_features[column_name], Sequence)
             if not sequence_column_type:
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"File path or data: {self.path_or_dict}\n"
                             f"type mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                             f"Found type: {type(datset_features[column_name])}\n"
                             f"Expected type: {Sequence}"
                         )
                     )
                 )
             column_dtype = datset_features[column_name].feature.dtype
             if column_dtype not in valid_dtypes:
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"File path or data: {self.path_or_dict}\n"
                             f"dtype mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                             f"Found dtype: {column_dtype}\n"
                             f"Expected dtypes: {valid_dtypes}"
                         )
                     )
                 )
 
-    def validate(self):
+    def validate(self, split: Optional[str] = None):
+        self.apply_common_validations(split, batch_size=self.dataset_args["batch_size"])
 
-        # Remove the extra columns and match the remaining columns
-        self.remove_extra_columns()
-        self.match_columns()
-
-        # filter data
-        # null filter
-        self.remove_null_examples(batch_size=self.dataset_args["batch_size"])
         # check dtypes
         # NOTE doing dtype check before task specific data filter because :meth ner_data_filter
         # assumes the dtypes for columns
         self.check_column_dtypes()
         # using ner specific filter
         self.ner_data_filter()
```

## azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_finetune.py

```diff
@@ -27,63 +27,71 @@
 import json
 
 from .base import NerPreprocessArgs, NerDataset
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....constants.constants import Tasks, HfModelTypes, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import TokenizerNotSupported, InvalidLabel, InvalidDataset
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException, ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import TokenizerNotSupported, InvalidLabel, InvalidDataset
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.tokenization_utils_fast import PreTrainedTokenizerFast
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
         #  - model_name arg from model selector
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
+        self.ft_config = getattr(component_args, "finetune_config", {})
 
         logger.info(f"Task name: {Tasks.NAMED_ENTITY_RECOGNITION}")
 
-        self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
+        self.model_type = AzuremlAutoConfig.get_model_type(
+            hf_model_name_or_path=component_args.model_name_or_path,
+            **self.ft_config.get("load_config_kwargs", {}),
+        )
         logger.info(self.preprocess_args)
 
         self.tokenizer = self._init_tokenizer()
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.NAMED_ENTITY_RECOGNITION,
             "apply_adjust": True,
-            "max_sequence_length": self.preprocess_args.max_seq_length
+            "max_sequence_length": self.preprocess_args.max_seq_length,
         }
         if self.model_type in [HfModelTypes.GPT2, HfModelTypes.ROBERTA, HfModelTypes.DEBERTA]:
             tokenizer_params.update(
                 {
-                    "add_prefix_space": True
+                    "add_prefix_space": True,
                 }
             )
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+
         tokenizer = AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
         # Only FastTokenizer is supported for TokenClassification
         # The python based tokenizer doesn't support `tokenizer.word_ids(<idx>)`
         if not isinstance(tokenizer, PreTrainedTokenizerFast):
-            raise ValidationException._with_error(
+            raise ACFTValidationException._with_error(
                 AzureMLError.create(
                     TokenizerNotSupported, Tokenizer=tokenizer, TaskName=Tasks.NAMED_ENTITY_RECOGNITION
                 )
             )
 
         return tokenizer
 
@@ -206,34 +214,34 @@
     def _validate_data_splits(self):
         """
         1. validate the datasets
         2. Identify the classnames and do some validations on them
         """
         # validate the datasets
         logger.info("Validating the train dataset")
-        self.train_ds.validate()
+        self.train_ds.validate(DatasetSplit.TRAIN)
         logger.info("Validating the validation dataset")
-        self.valid_ds.validate()
+        self.valid_ds.validate(DatasetSplit.VALIDATION)
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             logger.info("Validating the test dataset")
-            self.test_ds.validate()
+            self.test_ds.validate(DatasetSplit.TEST)
 
         # Identify the class names - combination of train and validation datasets
         # class names are list of strings
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))  # type: ignore
         # few classes to do classification
         if len(self.class_names_train_plus_valid) < 2:
-            raise ValidationException._with_error(AzureMLError.create(InvalidDataset))
+            raise ACFTDataException._with_error(AzureMLError.create(InvalidDataset))
         logger.info(f"Identified class names: {self.class_names_train_plus_valid}")
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             self.class_names_test = self.test_ds.class_names
             # test ds has extra classes that are not in train and valid
             test_ds_extra_labels = set(self.class_names_test).difference(set(self.class_names_train_plus_valid))
             if test_ds_extra_labels:
-                raise ValidationException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
+                raise ACFTDataException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset(class_names_train_plus_valid=self.class_names_train_plus_valid)
```

## azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_inference.py

```diff
@@ -27,19 +27,19 @@
 from .base import NerPreprocessArgs, NerDataset
 from ....constants.constants import Tasks
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 
 from datasets.arrow_dataset import Dataset
 import pandas as pd
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForInfer():
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/runner.py

```diff
@@ -17,15 +17,15 @@
 # ---------------------------------------------------------
 
 from argparse import Namespace
 from typing import List
 
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
-from .preprocess.base import NLPMulticlassPreprocessArgs
+from .preprocess.base import NLPMulticlassPreprocessArgs, NLPMulticlassDataset
 # from .preprocess.preprocess_for_inference import SingleLabelPreprocessForInfer
 
 from transformers.hf_argparser import HfArgumentParser
 
 
 class NLPMulticlassRunner(BaseRunner):
 
@@ -47,14 +47,14 @@
 
         from ...utils.model_selector_utils import model_selector
 
         model_selector(kwargs)
 
     def run_finetune(self, component_plus_preprocess_args: Namespace) -> None:
 
-        from .finetune.finetune import NLPMulticlassFinetune
+        from ..single_label.finetune.finetune import SingleLabelFinetune
 
-        finetune_obj = NLPMulticlassFinetune(vars(component_plus_preprocess_args))
+        finetune_obj = SingleLabelFinetune(vars(component_plus_preprocess_args), NLPMulticlassDataset)
         finetune_obj.finetune()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         raise NotImplementedError
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/base.py

```diff
@@ -12,16 +12,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
+"""
+NLP Multiclass
+"""
+
 from pathlib import Path
-from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 from datasets.arrow_dataset import Dataset
 
 from ....constants.constants import (
     AzuremlConstants,
     PreprocessArgsTemplate,
@@ -29,33 +32,31 @@
     MLFlowHFFlavourTasks,
     STRING_DTYPES,
     INT_DTYPES,
     AutomlConstants
 )
 
 from ....utils.data_utils import AzuremlDataset
-from ....utils.preprocess_utils import concat_text_columns
 from ....utils.validation_utils import AzuremlValidatorMixin
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorWithPadding
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import ValidationError
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
+from azureml.acft.contrib.hf.nlp.constants.constants import DataSliceConstants
+from azureml.acft.contrib.hf.nlp.utils.preprocess_utils import restructure_columns
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class NLPMulticlassPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of SingleLabelPreprocessArgs +
-    # inhertied attributes from PreprocessArgsTemplate here.
+    # inherited attributes from PreprocessArgsTemplate here.
     # Otherwise, there will be issues related to ordering of default and
     # non-default attributes
 
     # extra args
     # Makesure the extra args don't overlap with names of PreprocessArgs Template
     sentence1_key: str = field(
         default=AutomlConstants.TEXT_CLASSIFICATION_COLUMN_NAME
@@ -123,97 +124,66 @@
         path_or_dict: Union[str, Path],
         dataset_args: Optional[Dict[str, Any]] = None,
         required_columns: Optional[List[str]] = None,
         required_column_dtypes: Optional[List[List[str]]] = None,
         label_column: Optional[str] = None,
         label_column_optional: bool = False,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
-        preprocess: bool = True,
+        preprocess: bool = False,
         pass_through_columns: List[str] = None,  # columns that are passed throgh to the next component.
         ignore_columns: List[str] = None,  # columns to be ignored while concat, to be ignored for next component.
-        dataset_columns:List[str] = None,  # full list of dataset columns to be considered while processing.
+        dataset_columns: List[str] = None,  # full list of dataset columns to be considered while processing.
+        slice: str = DataSliceConstants.NO_SPLIT
     ) -> None:
         # required_columns, required_column_dtypes are made optional to support loading the dataset
         # without the need for validation
 
         # initialize the dataset class
         super().__init__(
             path_or_dict,
             label_column=label_column,
             label_column_optional=label_column_optional,
+            slice=slice
         )
 
-        # initialze the validator mixin class
+        # initialize the validator mixin class
         super(AzuremlDataset, self).__init__(
             required_columns=required_columns,
             required_column_dtypes=required_column_dtypes
         )
         self._set_fields(dataset_args, required_columns, required_column_dtypes,
                          label_column, label_column_optional, tokenizer, preprocess,
                          pass_through_columns, ignore_columns, dataset_columns)
 
         if preprocess:
-            self.restructure_dataset()
+            restructure_columns(self)
     
+
     def _set_fields(self,
                     dataset_args: Optional[Dict[str, Any]] = None,
                     required_columns: Optional[List[str]] = None,
                     required_column_dtypes: Optional[List[List[str]]] = None,
                     label_column: Optional[str] = None,
                     label_column_optional: bool = False,
                     tokenizer: Optional[PreTrainedTokenizerBase] = None,
                     preprocess: bool = True,
                     pass_through_columns: List[str] = None,
                     ignore_columns: List[str] = None,
-                    dataset_columns:List[str] = None,):
+                    dataset_columns: List[str] = None,):
         self.dataset_args = dataset_args
         self.required_columns = required_columns
         self.required_column_dtypes = required_column_dtypes
         self.label_column_optional = label_column_optional
         self.preprocess = preprocess
         self.tokenizer = tokenizer
         self.pass_through_columns = pass_through_columns if pass_through_columns is not None else []
         self.ignore_columns = ignore_columns if ignore_columns is not None else []
         self.dataset_columns = dataset_columns if dataset_columns is not None else []
         self.label_column = label_column
 
-    def restructure_dataset(self):
-        # text column concatenation
-        # removal of contacted columns and all columns except the pass through/label/sentence.
-        # AutoML NLP Logic
-        # Generate warnings if passed in parameter columns are not present in the dataset
-        if self.label_column and self.label_column not in self.dataset.features:
-            logger.warning(f"Passed in Label column {self.label_column} not found in dataset")
-        if self.pass_through_columns:
-            for item in self.pass_through_columns:
-                if item not in self.dataset.features:
-                    logger.warning(f"Passed in pass through column {item} not found in dataset")
-        if self.dataset_columns:
-            for item in self.dataset_columns:
-                if item not in self.dataset.features:
-                    logger.warning(f"Passed in dataset column {item} not found in dataset")
-        if self.label_column and self.dataset_columns and self.label_column not in self.dataset_columns:
-            logger.warning(f"Passed in Label column {self.label_column} not found in dataset_columns passed")
-            
-        label_columns = [self.label_column] if self.label_column is not None else []
-        exclude_columns = label_columns + self.pass_through_columns
-        cols_to_remove = [col for col in self.dataset.column_names if col not in exclude_columns]
-        self.dataset = self.dataset.map(
-            partial(
-                concat_text_columns,
-                label_columns=label_columns,
-                pass_through_columns=self.pass_through_columns,
-                ignore_columns=self.ignore_columns,
-                dataset_columns=self.dataset_columns,
-            ),
-            batched=False,
-            remove_columns=cols_to_remove,
-        )
-
-
     def get_collation_function(self) -> Optional[Callable]:
         """Collation function for dynamic padding"""
         return DataCollatorWithPadding(self.tokenizer) if self.tokenizer is not None else None
 
     def update_dataset_columns_with_prefix(self):
         """Update the sentence1_key, sentece2_key and label_keys with prefix"""
         if self.dataset_args is not None:
@@ -249,15 +219,15 @@
                 *args,
                 padding=self.dataset_args["padding"],
                 max_length=self.dataset_args["max_length"],
                 truncation=self.dataset_args["truncation"]
             )
 
             if label_key is not None:
-                result["labels"] = [label_to_id[label] for label in examples[label_key]]
+                result["labels"] = [label_to_id[label.lower()] for label in examples[label_key]]
 
             return result
 
         # sentence and label keys
         sentence1_key, sentence2_key = self.dataset_args["sentence1_key"], self.dataset_args["sentence2_key"]
         label_key = self.dataset_args["label_key"]
 
@@ -288,10 +258,10 @@
         dataset_columns:List[str] = None,
     ) -> None:
         self._set_fields(dataset_args, required_columns, required_column_dtypes,
                          label_column, True, tokenizer, True,
                          pass_through_columns, ignore_columns, dataset_columns)
         
         self.dataset = Dataset.from_pandas(df)
-        self.restructure_dataset()
+        restructure_columns(self)
         self.update_dataset_columns_with_prefix()
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/preprocess_for_finetune.py

```diff
@@ -12,38 +12,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
-import os
-import json
 import copy
+import json
 
 from pathlib  import Path
 from argparse import Namespace
 from typing import Dict, Any
 from dataclasses import asdict
 
 from .base import NLPMulticlassPreprocessArgs, NLPMulticlassDataset
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....constants.constants import Tasks, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 from ....utils.preprocess_utils import get_max_seq_length
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NLPMulticlassPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: NLPMulticlassPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
@@ -88,15 +88,17 @@
             tokenizer=self.tokenizer,
             pass_through_columns=self.pass_through_columns,
             ignore_columns=self.ignore_columns,
             dataset_columns=self.dataset_columns
         )
         ds = NLPMulticlassDataset(
             self.component_args.train_data_path,
-           **copy.deepcopy(kwargs)
+           **copy.deepcopy(kwargs),
+           slice=self.component_args.train_slice,
+           preprocess=True,
         )
         max_seq_length = get_max_seq_length(
             ds.dataset, self.tokenizer, self.component_args.enable_long_range_text
         )
         encode_params["max_length"] = min(max_seq_length, self.tokenizer.model_max_length)
 
         return encode_params
@@ -120,25 +122,31 @@
             tokenizer=self.tokenizer,
             pass_through_columns=self.pass_through_columns,
             ignore_columns=self.ignore_columns,
             dataset_columns=self.dataset_columns
         )
         self.train_ds = NLPMulticlassDataset(
             self.component_args.train_data_path,
-           **copy.deepcopy(kwargs)
+            **copy.deepcopy(kwargs),
+            slice=self.component_args.train_slice,
+            preprocess=True,
         )
         self.valid_ds = NLPMulticlassDataset(
             self.component_args.validation_data_path,
-            **copy.deepcopy(kwargs)
+            **copy.deepcopy(kwargs),
+            slice=self.component_args.validation_slice,
+            preprocess=True,
         )
         if self.component_args.test_data_path is not None:
             self.test_ds = NLPMulticlassDataset(
                 self.component_args.test_data_path,
                 **copy.deepcopy(kwargs),
-                label_column_optional=True
+                slice=self.component_args.test_slice,
+                label_column_optional=True,
+                preprocess=True,
             )
         else:
             self.test_ds = None
 
         # add dataset prefix
         self.train_ds.update_dataset_columns_with_prefix()
         self.train_ds.update_required_columns_with_prefix()
@@ -163,22 +171,22 @@
             self.test_ds.validate()
 
         # Identify the class names - combination of train and validation datasets
         # class names are list of strings
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))  #type: ignore
         # few classes to do classification
         if len(self.class_names_train_plus_valid) < 2:
-            raise ValidationException._with_error(AzureMLError.create(InvalidDataset))
+            raise ACFTDataException._with_error(AzureMLError.create(InvalidDataset))
         logger.info(f"Identified class names: {self.class_names_train_plus_valid}")
         if self.test_ds is not None:
             self.class_names_test= self.test_ds.class_names
             # test ds has extra classes that are not in train and valid
             test_ds_extra_labels = set(self.class_names_test).difference(set(self.class_names_train_plus_valid))  #type: ignore
             if test_ds_extra_labels:
-                raise ValidationException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
+                raise ACFTDataException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset(label_to_id = self.label_to_id)
@@ -192,15 +200,15 @@
         """
         Preprocess the raw dataset
         """
 
         # load, validate and encode the datasets
         self._load_data_splits()
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))
-        self.label_to_id = {label:id for id, label in enumerate(self.class_names_train_plus_valid)}
+        self.label_to_id = {str(label).lower():id for id, label in enumerate(self.class_names_train_plus_valid)}
         # self._validate_data_splits()
         self._encode_data_splits()
 
         # Save
         # 1. encoded datasets
         # 2. Arguments
         # 3. class names
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/runner.py

```diff
@@ -17,17 +17,16 @@
 # ---------------------------------------------------------
 
 from argparse import Namespace
 from typing import List
 
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
-from .preprocess.base import NLPMultilabelPreprocessArgs
+from .preprocess.base import NLPMultilabelPreprocessArgs, NLPMultilabelDataset
 
-# from .preprocess.preprocess_for_inference import MultiLabelPreprocessForInfer
 from ...utils.hf_argparser import HfArgumentParser
 
 
 class NLPMultilabelRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
@@ -47,14 +46,14 @@
 
         from ...utils.model_selector_utils import model_selector
 
         model_selector(kwargs)
 
     def run_finetune(self, component_plus_preprocess_args: Namespace) -> None:
 
-        from .finetune.finetune import NLPMultilabelFinetune
+        from ..multi_label.finetune.finetune import MultiLabelFinetune
 
-        finetune_obj = NLPMultilabelFinetune(vars(component_plus_preprocess_args))
+        finetune_obj = MultiLabelFinetune(vars(component_plus_preprocess_args), NLPMultilabelDataset)
         finetune_obj.finetune()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         raise NotImplementedError
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/base.py

```diff
@@ -12,62 +12,56 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
+"""
+NLP Multilabel
+"""
+
 import ast
 from pathlib import Path
-from functools import partial
 
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 from sklearn.preprocessing import MultiLabelBinarizer
 
 from ....constants.constants import (
-    DatasetSplit,
-    SaveFileConstants,
     AzuremlConstants,
-    MLFlowHFFlavourConstants,
     PreprocessArgsTemplate,
     Tasks,
     MLFlowHFFlavourTasks,
-    HfModelTypes,
     STRING_DTYPES,
     AutomlConstants,
 )
-from ....base_runner import BaseRunner
 
 from ....utils.data_utils import AzuremlDataset
-from ....utils.preprocess_utils import concat_text_columns
 from ....utils.validation_utils import AzuremlValidatorMixin
 from ....constants.constants import TaskConstants
 
 from datasets.arrow_dataset import Dataset
-from datasets import Sequence
+from datasets import Sequence, Value
 
-import transformers
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorWithPadding
-from transformers.hf_argparser import HfArgumentParser
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
+from azureml.acft.contrib.hf.nlp.constants.constants import DataSliceConstants
+from azureml.acft.contrib.hf.nlp.utils.preprocess_utils import restructure_columns
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class NLPMultilabelPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of MultiLabelPreprocessArgs +
-    # inhertied attributes from _PreprocessArgsTemplate here.
+    # inherited attributes from _PreprocessArgsTemplate here.
     # Otherwise, there will be issues related to ordering of default and
     # non-default attributes
 
     # extra args
     # Makesure the extra args don't overlap with names of PreprocessArgs Template
     sentence1_key: str = field(
         default=AutomlConstants.TEXT_CLASSIFICATION_COLUMN_NAME
@@ -135,61 +129,80 @@
         path_or_dict: Union[str, Path],
         dataset_args: Optional[Dict[str, Any]] = None,
         required_columns: Optional[List[str]] = None,
         required_column_dtypes: Optional[List[List[str]]] = None,
         label_column: Optional[str] = None,
         label_column_optional: bool = False,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
-        preprocess: bool = True,
+        preprocess: bool = False,
+        pass_through_columns: List[str] = None,  # columns that are passed through to the next component.
+        ignore_columns: List[str] = None,  # columns to be ignored while concat, to be ignored for next component.
+        dataset_columns: List[str] = None,  # full list of dataset columns to be considered while processing.
+        slice: str = DataSliceConstants.NO_SPLIT
     ) -> None:
         # required_columns, required_column_dtypes are made optional to support loading the dataset
         # without the need for validation
 
         # special column is added for multi-label after the label_data is decoded and converted to list of string
         self.preprocess = preprocess
-        new_label_column = None
-        if label_column is not None and dataset_args is not None and required_columns is not None and required_column_dtypes is not None:
+        if label_column is not None and dataset_args is not None and required_columns is not None and \
+                required_column_dtypes is not None:
             new_label_column = label_column + TaskConstants.MULTI_LABEL_NEW_COLUMN_SUFFIX
             dataset_args["label_key"] = new_label_column
             self.label_list_column = new_label_column
             logger.info(f"Updated label column: {new_label_column}")
 
         # initialize the dataset class
         super().__init__(
             path_or_dict,
             label_column=label_column,
             label_column_optional=label_column_optional,
+            slice=slice
         )
 
-        # initialze the validator mixin class
+        # initialize the validator mixin class
         super(AzuremlDataset, self).__init__(
             required_columns=required_columns,
             required_column_dtypes=required_column_dtypes
         )
+        self._set_fields(dataset_args, required_columns, required_column_dtypes,
+                         label_column, label_column_optional, tokenizer, preprocess,
+                         pass_through_columns, ignore_columns, dataset_columns)
 
         self.dataset_args = dataset_args
         self.tokenizer = tokenizer
         self.old_label_column = label_column
 
         # decode the old label column and populate the new one
         self.dataset = self.dataset.map(self.decode_label_column, batched=True)
 
         if preprocess:
-            # text column concatenation
-            # AutoML NLP Logic
-            label_columns = [label_column, new_label_column]
-            cols_to_remove = [col for col in self.dataset.column_names if (col not in label_columns)]
-            self.dataset = self.dataset.map(
-                partial(
-                    concat_text_columns,
-                    label_columns=label_columns
-                ),
-                batched=False,
-                remove_columns=cols_to_remove,
-            )
+            restructure_columns(self)
+
+    def _set_fields(self,
+                    dataset_args: Optional[Dict[str, Any]] = None,
+                    required_columns: Optional[List[str]] = None,
+                    required_column_dtypes: Optional[List[List[str]]] = None,
+                    label_column: Optional[str] = None,
+                    label_column_optional: bool = False,
+                    tokenizer: Optional[PreTrainedTokenizerBase] = None,
+                    preprocess: bool = True,
+                    pass_through_columns: List[str] = None,
+                    ignore_columns: List[str] = None,
+                    dataset_columns: List[str] = None,):
+        self.dataset_args = dataset_args
+        self.required_columns = required_columns
+        self.required_column_dtypes = required_column_dtypes
+        self.label_column_optional = label_column_optional
+        self.preprocess = preprocess
+        self.tokenizer = tokenizer
+        self.pass_through_columns = pass_through_columns if pass_through_columns is not None else []
+        self.ignore_columns = ignore_columns if ignore_columns is not None else []
+        self.dataset_columns = dataset_columns if dataset_columns is not None else []
+        self.label_column = label_column
 
     def get_collation_function(self) -> Optional[Callable]:
         """Collation function for dynamic padding"""
         return DataCollatorWithPadding(self.tokenizer) if self.tokenizer is not None else None
 
     def encode_dataset(self, class_names_train_plus_valid: Optional[List[str]] = None):
         """
@@ -248,25 +261,22 @@
     def decode_label_column(self, examples: Dict[str, Any]) -> Dict[str, Any]:
         """
         The label column of multi-label is a list of class names encoded as string i.e. of type string of list of string
         This function encodes the old label column and populates the new label column
         :param examples
             Dictionary of dataset examples
         """
-        if self.old_label_column is None:
-            logger.info(f"label column is {self.old_label_column}. skipping label column decoding")
+        if self.old_label_column is None or not hasattr(self, 'label_list_column'):
+            logger.info(f"label column is None. skipping label column decoding")
             return examples
 
         item_decode_list = []
         for item in examples[self.old_label_column]:
             item_decode = ast.literal_eval(item)
-            if not (
-                isinstance(item_decode, List) and
-                (item_decode and isinstance(item_decode[0], str))
-            ):
+            if not isinstance(item_decode, List):
                 raise ValueError("data is incorrectly formatted")
             item_decode_list.append(item_decode)
 
         # label column is created ONLY when old_label_column is present
         examples[self.label_list_column] = item_decode_list  # type: ignore
 
         return examples
@@ -278,22 +288,52 @@
             if self.dataset_args["sentence2_key"] is not None:
                 self.dataset_args["sentence2_key"] = AzuremlConstants.DATASET_COLUMN_PREFIX + self.dataset_args["sentence2_key"]
             if self.dataset_args["label_key"] is not None:
                 self.dataset_args["label_key"] = AzuremlConstants.DATASET_COLUMN_PREFIX + self.dataset_args["label_key"]
 
         return super().update_dataset_columns_with_prefix()
 
-    def load(self) -> Dataset:
+    def load(self, slice: str = DataSliceConstants.NO_SPLIT) -> Dataset:
         """
         Load the dataset and add a dummy column for the new column
         new column will a list of strings which will be a decoded column of string input
         """
-        dataset = super().load()
+
+        dataset = super().load(slice=slice)
 
         # add a dummy column with list of strings dtype
-        if self.preprocess:
+        if self.preprocess and hasattr(self, 'label_list_column'):
             dataset = dataset.add_column(
                 name=self.label_list_column,
                 column=[[""]] * len(dataset) 
             )
         
         return dataset
+
+    @property
+    def class_names(self) -> Optional[List[str]]:
+
+        # Return the precomputed class names saved in a private variable
+        label_column = AzuremlConstants.DATASET_COLUMN_PREFIX + self.label_list_column
+        if hasattr(self, "_class_names"):
+            return self._class_names
+
+        if self.label_column is None:
+            logger.info(f"Label column is {label_column}. Couldn't compute class names")
+            return None
+
+        sequence_data_type = isinstance(self.dataset.features[label_column], Sequence)
+        value_data_type = isinstance(self.dataset.features[label_column], Value)
+        if sequence_data_type:
+            class_names = set()
+            label_column_uniq_data = self.dataset[label_column]
+            for item in label_column_uniq_data:
+                class_names.update(item)
+            # class_names needs to be sorted for reproducibility
+            self._class_names = sorted(class_names)
+            return self._class_names
+        elif value_data_type:
+            # class_names needs to be sorted for reproducibility
+            self._class_names = sorted(self.dataset.unique(label_column))
+            return self._class_names
+        else:
+            raise ValueError("Feature type is invalid. Only Value or Sequence types are supported")
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/preprocess_for_finetune.py

```diff
@@ -11,39 +11,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
-import os
 import copy
 import json
 
-
 from pathlib  import Path
 from argparse import Namespace
 from typing import Dict, Any
 from dataclasses import asdict
 
 from .base import NLPMultilabelPreprocessArgs, NLPMultilabelDataset
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....constants.constants import Tasks, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 from ....utils.preprocess_utils import get_max_seq_length
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NLPMultilabelPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: NLPMultilabelPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
@@ -51,14 +50,17 @@
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
         self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
         logger.info(self.preprocess_args)
 
         self.tokenizer = self._init_tokenizer()
+        self.pass_through_columns = None  # List[str]
+        self.ignore_columns = None  # List[str]
+        self.dataset_columns = None  # List[str]
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.MULTI_LABEL_CLASSIFICATION,
             "apply_adjust": True,
@@ -78,19 +80,24 @@
         # AutoML NLP logic
         dataset_args=asdict(self.preprocess_args)
         kwargs = dict(
             dataset_args=dataset_args,
             required_columns=self.preprocess_args.required_columns,
             required_column_dtypes=self.preprocess_args.required_column_dtypes,
             label_column=self.preprocess_args.label_column,
-            tokenizer=self.tokenizer
+            tokenizer=self.tokenizer,
+            pass_through_columns=self.pass_through_columns,
+            ignore_columns=self.ignore_columns,
+            dataset_columns=self.dataset_columns
         )
         ds = NLPMultilabelDataset(
             self.component_args.train_data_path,
             **copy.deepcopy(kwargs),
+            slice=self.component_args.train_slice,
+            preprocess=True
         )
         max_seq_length = get_max_seq_length(
             ds.dataset, self.tokenizer, self.component_args.enable_long_range_text
         )
         encode_params["max_length"] = min(max_seq_length, self.tokenizer.model_max_length)
 
         # returns all the scores of multi label model
@@ -103,48 +110,57 @@
         1. Load train, validation and test data splits
         2. Add column prefix for the data
         """
         # encode params used for encoding dataset
         self.encode_params = self._get_encode_dataset_params()
 
         # initialize dataset
-        dataset_args=asdict(self.preprocess_args)
+        dataset_args = asdict(self.preprocess_args)
         dataset_args.update(self.encode_params)
         kwargs = dict(
             dataset_args=dataset_args,
             required_columns=self.preprocess_args.required_columns,
             required_column_dtypes=self.preprocess_args.required_column_dtypes,
             label_column=self.preprocess_args.label_column,
-            tokenizer=self.tokenizer
+            tokenizer=self.tokenizer,
+            pass_through_columns=self.pass_through_columns,
+            ignore_columns=self.ignore_columns,
+            dataset_columns=self.dataset_columns
         )
         self.train_ds = NLPMultilabelDataset(
             self.component_args.train_data_path,
             **copy.deepcopy(kwargs),
+            slice=self.component_args.train_slice,
+            preprocess=True,
         )
         self.train_ds.dataset = self.train_ds.dataset.map(
             self.train_ds.decode_label_column,
             batched=True,
             batch_size=self.preprocess_args.batch_size,
             writer_batch_size=self.preprocess_args.batch_size
         )
         self.valid_ds = NLPMultilabelDataset(
             self.component_args.validation_data_path,
-            **copy.deepcopy(kwargs)
+            **copy.deepcopy(kwargs),
+            slice=self.component_args.validation_slice,
+            preprocess=True,
         )
         self.valid_ds.dataset = self.valid_ds.dataset.map(
             self.valid_ds.decode_label_column,
             batched=True,
             batch_size=self.preprocess_args.batch_size,
             writer_batch_size=self.preprocess_args.batch_size
         )
         if self.component_args.test_data_path is not None:
             self.test_ds = NLPMultilabelDataset(
                 self.component_args.test_data_path,
                 **copy.deepcopy(kwargs),
-                label_column_optional=True
+                label_column_optional=True,
+                slice=self.component_args.test_slice,
+                preprocess=True,
             )
             self.test_ds.dataset = self.test_ds.dataset.map(
                 self.test_ds.decode_label_column,
                 batched=True,
                 batch_size=self.preprocess_args.batch_size,
                 writer_batch_size=self.preprocess_args.batch_size
             )
@@ -175,22 +191,22 @@
             self.test_ds.validate()
 
         # Identify the class names - combination of train and validation datasets
         # class names are list of strings
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))  #type: ignore
         # few classes to do classification
         if len(self.class_names_train_plus_valid) < 2:
-            raise ValidationException._with_error(AzureMLError.create(InvalidDataset))
+            raise ACFTDataException._with_error(AzureMLError.create(InvalidDataset))
         logger.info(f"Identified class names: {self.class_names_train_plus_valid}")
         if self.test_ds is not None:
             self.class_names_test= self.test_ds.class_names
             # test ds has extra classes that are not in train and valid
             test_ds_extra_labels = set(self.class_names_test).difference(set(self.class_names_train_plus_valid))  #type: ignore
             if test_ds_extra_labels:
-                raise ValidationException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
+                raise ACFTDataException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset(class_names_train_plus_valid=self.class_names_train_plus_valid)
@@ -236,14 +252,17 @@
         # add the paths for encoded train, validation and test paths
         preprocess_args["encoded_train_data_fname"] = encoded_train_data_fname
         preprocess_args["encoded_validation_data_fname"] = encoded_validation_data_fname
         if self.test_ds is not None:
             preprocess_args["encoded_test_data_fname"] = encoded_test_data_fname
         preprocess_args_save_path = Path(self.component_args.output_dir, SaveFileConstants.PREPROCESS_ARGS_SAVE_PATH)
         preprocess_args["model_name_or_path"] = str(preprocess_args["model_name_or_path"])
+        preprocess_args["pass_through_columns"] = self.pass_through_columns
+        preprocess_args["ignore_columns"] = self.ignore_columns
+        preprocess_args["dataset_columns"] = self.dataset_columns
         logger.info(f"Saving the preprocess args to {preprocess_args_save_path}")
         with open(preprocess_args_save_path, 'w') as fp:
             json.dump(preprocess_args, fp, indent=2)
 
         # 3. class names
         class_names_save_path = Path(self.component_args.output_dir, SaveFileConstants.CLASSES_SAVE_PATH)
         logger.info(f"Saving the class names to {class_names_save_path}")
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_ner/runner.py

```diff
@@ -21,15 +21,15 @@
 """
 
 from argparse import Namespace
 from typing import List
 
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
-from .preprocess.base import NLPNerPreprocessArgs
+from .preprocess.base import NLPNerPreprocessArgs, NLPNerDataset
 
 from transformers.hf_argparser import HfArgumentParser
 
 
 class NLPNerRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
@@ -50,14 +50,14 @@
 
         from ...utils.model_selector_utils import model_selector
 
         model_selector(kwargs)
 
     def run_finetune(self, component_plus_preprocess_args: Namespace) -> None:
 
-        from .finetune.finetune import NLPNerFinetune
+        from ..ner.finetune.finetune import NerFinetune
 
-        finetune_obj = NLPNerFinetune(vars(component_plus_preprocess_args))
+        finetune_obj = NerFinetune(vars(component_plus_preprocess_args), NLPNerDataset)
         finetune_obj.finetune()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         raise NotImplementedError
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/base.py

```diff
@@ -17,56 +17,43 @@
 # ---------------------------------------------------------
 
 """
 NLP NER
 """
 
 import os
-import json
+import mltable
 from pathlib import Path
-from argparse import Namespace
 
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 
-import torch.nn as nn
-
-from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ....nlp_auto.config import AzuremlAutoConfig
 from ....constants.constants import (
-    DatasetSplit,
-    SaveFileConstants,
     AzuremlConstants,
-    MLFlowHFFlavourConstants,
     PreprocessArgsTemplate,
     Tasks,
     MLFlowHFFlavourTasks,
     STRING_DTYPES,
     TaskConstants,
     AutomlConstants,
 )
-from ....base_runner import BaseRunner
 
 from ....utils.data_utils import AzuremlDataset
 from ....utils.validation_utils import AzuremlValidatorMixin
 
 from datasets.arrow_dataset import Dataset
-from datasets import Sequence
 
-import transformers
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorForTokenClassification
-from transformers.hf_argparser import HfArgumentParser
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
+
+from ....utils.preprocess_utils import get_new_file_name, txt_to_jsonl
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class NLPNerPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of NerPreprocessArgs + inhertied attributes from
     # _PreprocessArgsTemplate here. Otherwise, there will be issues related to ordering of default and
     # non-default attributes
@@ -134,23 +121,25 @@
         path_or_dict: Union[str, Path, Dict],
         dataset_args: Optional[Dict[str, Any]] = None,
         required_columns: Optional[List[str]] = None,
         required_column_dtypes: Optional[List[List[str]]] = None,
         label_column: Optional[str] = None,
         label_column_optional: bool = False,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
+        slice: str = "train"
     ) -> None:
         # required_columns, required_column_dtypes are made optional to support loading the dataset
         # without the need for validation
 
         # initialize the dataset class
         super().__init__(
             path_or_dict,
             label_column=label_column,
             label_column_optional=label_column_optional,
+            slice=slice
         )
 
         # no need for 'id' column in nlp ner datasets
         if 'id' in self.dataset.features:
             self.dataset = self.dataset.remove_columns('id')
 
         # initialze the validator mixin class
@@ -158,14 +147,55 @@
             required_columns=required_columns,
             required_column_dtypes=required_column_dtypes
         )
 
         self.dataset_args = dataset_args
         self.tokenizer = tokenizer
 
+    def load(self, slice: str = "train") -> Dataset:
+        """
+        1. Loads the dataset
+        2. kwargs
+            data_format - json, csv, mltable, txt
+            dataset_type - could be dataset or torch
+            sample_size
+                0.1 - 1.0 percentage of data to load
+                1 - len(dataset) number of samples to load
+        3. Handle loading dataset from S3 URI, Azure blob store
+        """
+
+        if isinstance(self.path_or_dict, str):
+            # check if file exists
+            if Path(self.path_or_dict).is_file():
+                # check if the file format is supported
+                file_format = super()._get_file_format(self.path_or_dict)
+                if file_format == ".txt":
+                    new_file_name = get_new_file_name(self.path_or_dict, "txt", "jsonl")
+                    txt_to_jsonl(self.path_or_dict, new_file_name)
+                    self.path_or_dict = new_file_name
+
+            elif Path(self.path_or_dict).is_dir():
+                # check if valid MLTable and load it
+                directory_format = self._get_directory_format(self.path_or_dict)
+                logger.info(directory_format)
+                if directory_format:
+                    if directory_format == "mltable":
+
+                        data_tbl = mltable.load(self.path_or_dict)
+                        mltable_file = data_tbl.paths[0]['file'][2:]
+                        data_format = Path(mltable_file).suffix.lstrip(".")
+
+                        if data_format == "txt":
+                            self.path_or_dict = os.path.join(self.path_or_dict, mltable_file)
+                            new_file_name = get_new_file_name(self.path_or_dict, "txt", "jsonl")
+                            txt_to_jsonl(self.path_or_dict, new_file_name)
+                            self.path_or_dict = new_file_name
+
+        return super().load(slice=slice)
+
     def get_collation_function(self) -> Optional[Callable]:
         """Collation function for dynamic padding"""
         return DataCollatorForTokenClassification(self.tokenizer) if self.tokenizer is not None else None
 
     def encode_dataset(self, class_names_train_plus_valid: Optional[List[str]] = None):
         """
         datasets: HuggingFace datasets object
```

## azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/preprocess_for_finetune.py

```diff
@@ -28,24 +28,25 @@
 import json
 
 from .base import NLPNerPreprocessArgs, NLPNerDataset
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....constants.constants import Tasks, HfModelTypes, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import TokenizerNotSupported, InvalidLabel, InvalidDataset
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException, ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import TokenizerNotSupported, InvalidLabel, InvalidDataset
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.tokenization_utils_fast import PreTrainedTokenizerFast
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NLPNerPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: NLPNerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
@@ -73,15 +74,15 @@
                 }
             )
 
         tokenizer = AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
         # Only FastTokenizer is supported for TokenClassification
         # The python based tokenizer doesn't support `tokenizer.word_ids(<idx>)`
         if not isinstance(tokenizer, PreTrainedTokenizerFast):
-            raise ValidationException._with_error(
+            raise ACFTValidationException._with_error(
                 AzureMLError.create(
                     TokenizerNotSupported, Tokenizer=tokenizer, TaskName=Tasks.NAMED_ENTITY_RECOGNITION
                 )
             )
 
         return tokenizer
 
@@ -113,25 +114,28 @@
             required_columns=self.preprocess_args.required_columns,
             required_column_dtypes=self.preprocess_args.required_column_dtypes,
             label_column=self.preprocess_args.tag_key,
             tokenizer=self.tokenizer
         )
         self.train_ds = NLPNerDataset(
             self.component_args.train_data_path,
-           **copy.deepcopy(kwargs)
+            **copy.deepcopy(kwargs),
+            slice=self.component_args.train_slice,
         )
         self.valid_ds = NLPNerDataset(
             self.component_args.validation_data_path,
-            **copy.deepcopy(kwargs)
+            **copy.deepcopy(kwargs),
+            slice=self.component_args.validation_slice,
         )
         if self.component_args.test_data_path is not None:
             self.test_ds = NLPNerDataset(
                 self.component_args.test_data_path,
                 label_column_optional=True,
-                **copy.deepcopy(kwargs)
+                **copy.deepcopy(kwargs),
+                slice=self.component_args.test_slice,
             )
         else:
             self.test_ds = None
 
         # add dataset prefix
         self.train_ds.update_dataset_columns_with_prefix()
         self.train_ds.update_required_columns_with_prefix()
@@ -156,22 +160,22 @@
             self.test_ds.validate()
 
         # Identify the class names - combination of train and validation datasets
         # class names are list of strings
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))  # type: ignore
         # few classes to do classification
         if len(self.class_names_train_plus_valid) < 2:
-            raise ValidationException._with_error(AzureMLError.create(InvalidDataset))
+            raise ACFTDataException._with_error(AzureMLError.create(InvalidDataset))
         logger.info(f"Identified class names: {self.class_names_train_plus_valid}")
         if self.test_ds is not None:
             self.class_names_test= self.test_ds.class_names
             # test ds has extra classes that are not in train and valid
             test_ds_extra_labels = set(self.class_names_test).difference(set(self.class_names_train_plus_valid))
             if test_ds_extra_labels:
-                raise ValidationException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
+                raise ACFTDataException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset(class_names_train_plus_valid=self.class_names_train_plus_valid)
```

## azureml/acft/contrib/hf/nlp/tasks/qna/runner.py

```diff
@@ -22,27 +22,38 @@
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
 from .preprocess.base import QnAPreprocessArgs
 # from .preprocess.preprocess_for_inference import QnAPreprocessForInfer
 
 from transformers.hf_argparser import HfArgumentParser
 
+from azureml.acft.common_components import get_logger_app
+
+
+logger = get_logger_app(__name__)
+
 
 class QnARunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
         from .preprocess.preprocess_for_finetune import QnAPreprocessForFinetune
 
+        load_config_kwargs = getattr(component_args, "finetune_config", {}).get("load_config_kwargs", {})
         self.check_model_task_compatibility(
-            model_name_or_path=component_args.model_name_or_path, task_name=Tasks.QUESTION_ANSWERING
+            model_name_or_path=component_args.model_name_or_path,
+            task_name=Tasks.QUESTION_ANSWERING,
+            **load_config_kwargs,
         )
 
         preprocess_arg_parser = HfArgumentParser([QnAPreprocessArgs])
-        preprocess_args: QnAPreprocessArgs = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args)[0]
+        output_args = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args, return_remaining_strings=True)
+        preprocess_args: QnAPreprocessArgs = output_args[0]
+
+        logger.info(f"unused args - {output_args[1]}")
 
         preprocess_obj = QnAPreprocessForFinetune(component_args, preprocess_args)
         preprocess_obj.preprocess()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         pass
```

## azureml/acft/contrib/hf/nlp/tasks/qna/finetune/finetune.py

```diff
@@ -12,75 +12,70 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
-import json
 import numpy as np
 from pathlib import Path
 import collections
 from functools import partial
+import shutil
 
 from typing import Any, Dict, List, Tuple, Optional
 
+from ...base.finetune.finetune import FinetuneBase
 from ....constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, Tasks
 from ....nlp_auto.model import AzuremlAutoModelForQnA
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ..preprocess.base import QnADataset
-from ....utils.mlflow_utils import SaveMLflowModelCallback, replace_deepspeed_zero3_mlflow_pytorch_weights
+from ....utils.common_utils import write_dict_to_json_file
 
 import torch.nn as nn
 
 from datasets.arrow_dataset import Dataset
 from datasets.load import load_metric
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from azureml.acft.accelerator.finetune import AzuremlFinetuneArgs, AzuremlDatasetArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
 from azureml.acft.accelerator.constants import HfTrainerType
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_utils import EvalPrediction
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 
-from sklearn.metrics import (
-    f1_score,
-    accuracy_score,
-    matthews_corrcoef,
-    precision_score,
-    recall_score
-)
+from peft import TaskType
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
-class QnAFinetune:
+class QnAFinetune(FinetuneBase):
 
     def __init__(self, finetune_params: Dict[str, Any]) -> None:
         # finetune params is finetune component args + args saved as part of preprocess
         self.finetune_params = finetune_params
+        self.ft_config = finetune_params.get("finetune_config", {})
 
         logger.info(f"Task name: {Tasks.QUESTION_ANSWERING}")
 
         # set log_metrics_at_root=False to not to log to parent
         self.finetune_params["log_metrics_at_root"] = False
 
     def _get_finetune_args(self, model_type: str) -> AzuremlFinetuneArgs:
 
         self.finetune_params["model_type"] = model_type
+        self.finetune_params["peft_task_type"] = TaskType.QUESTION_ANS
         azml_trainer_finetune_args = AzuremlFinetuneArgs(
             self.finetune_params,
-            trainer_type=HfTrainerType.DEFAULT
+            trainer_type=HfTrainerType.DEFAULT,
         )
 
         return azml_trainer_finetune_args
 
     def _get_dataset_args(
         self,
         tokenizer: Optional[PreTrainedTokenizerBase] = None
@@ -101,96 +96,105 @@
 
         # load the raw validation ds
         raw_validation_ds = QnADataset(
             Path(self.finetune_params["preprocess_output"], self.finetune_params["raw_validation_data_fname"]),
         )
 
         return azml_trainer_dataset_args, raw_validation_ds
-    
+
     def _load_model(self) -> Tuple[nn.Module, str, List[str]]:
 
         model_params = {
             "ignore_mismatched_sizes": self.finetune_params["ignore_mismatched_sizes"],
             "resume_from_checkpoint": self.finetune_params["resume_from_checkpoint"],
+            "load_in_8bit": self.finetune_params["finetune_in_8bit"],
+            "load_in_4bit": self.finetune_params["finetune_in_4bit"],
         }
 
+        model_params.update(self.ft_config.get("load_model_kwargs", {}))
+        model_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading model with following args: {model_params}")
+
         model, model_type, new_initalized_layers = AzuremlAutoModelForQnA.from_pretrained(
             self.finetune_params["model_name_or_path"], **model_params)
 
         return model, model_type, new_initalized_layers
 
     def _get_tokenizer(self) -> PreTrainedTokenizerBase:
         """This method loads the tokenizer as is w/o any modifications to it"""
 
         tokenizer_params = {
             "apply_adjust": False,
             "task_name": self.finetune_params["task_name"],
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading tokenizer with following params: {tokenizer_params}")
+
         return AzuremlAutoTokenizer.from_pretrained(self.finetune_params["preprocess_output"], **tokenizer_params)
 
     def finetune(self) -> None:
 
-        # configure MLflow save callback
-        mlflow_infer_params_file_path = Path(
-            self.finetune_params["preprocess_output"], MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT
-        )
-        save_mlflow_callback = SaveMLflowModelCallback(
-            mlflow_infer_params_file_path=mlflow_infer_params_file_path,
-            mlflow_model_save_path=self.finetune_params["mlflow_model_folder"],
-            mlflow_task_type=self.finetune_params["mlflow_task_type"],
-            model_name=self.finetune_params["model_name"],
-            model_name_or_path=self.finetune_params["model_name_or_path"],
-        )
-
+        # Initializing the finetune args with dummy_model_type to enable the
+        # deepspeed stage3 which is used in :meth _load_model
+        finetune_args = self._get_finetune_args("dummy_model_type")
         model, model_type, new_initialized_params = self._load_model()
+        # Replacing the dummy_model_type -> original model_type information
+        setattr(finetune_args.optimization_args, "model_type", model_type)
+        self.finetune_params["model_type"] = model_type
         tokenizer = self._get_tokenizer()
         dataset_args, raw_validation_ds = self._get_dataset_args(tokenizer)
         trainer = AzuremlTrainer(
-            finetune_args=self._get_finetune_args(model_type),
+            finetune_args=finetune_args,
             dataset_args=dataset_args,
             model=model,
             tokenizer=tokenizer,
             metric_func=partial(
                 qna_metrics_func,
                 tokenizer=tokenizer,
                 raw_eval_dataset=raw_validation_ds.dataset,
                 enc_eval_dataset=dataset_args.validation_dataset,
                 n_best_size=self.finetune_params["n_best_size"],
                 max_answer_length_in_tokens=self.finetune_params["max_answer_length_in_tokens"],
                 answers_key=self.finetune_params["answers_key"],
                 context_key=self.finetune_params["context_key"]
             ),
             new_initalized_layers=new_initialized_params,
-            custom_trainer_callbacks=[save_mlflow_callback],
         )
 
+        self._save_mininum_finetune_args(finetune_args)
+
         # Torch barrier is used to complete the training on a distributed setup
         # Use callbacks for adding steps to be done at the end of training
         # NOTE Avoid adding any logic after trainer.train()
         # Test the distributed scenario in case you add any logic beyond trainer.train()
         trainer.train()
 
-        # replace pytorch weights for lora / deep speed zero3 optimization
-        if trainer.should_save and (self.finetune_params["apply_lora"] or is_deepspeed_zero3_enabled()):
-            logger.info("Replacing dummy MLflow weights ")
-            replace_deepspeed_zero3_mlflow_pytorch_weights(
-                self.finetune_params["pytorch_model_folder"],
-                self.finetune_params["mlflow_model_folder"]
-            )
-
         # save files only once by Rank-0 process
         if trainer.should_save:
-            # save finetune args
-            Path(self.finetune_params["pytorch_model_folder"]).mkdir(exist_ok=True, parents=True)
-            finetune_args_path = Path(self.finetune_params["pytorch_model_folder"], \
-                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
             self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
-            with open(finetune_args_path, 'w') as rptr:
-                json.dump(self.finetune_params, rptr, indent=2)
+            # save if model is trained via deepspeed stage 3
+            self.finetune_params["is_deepspeed_zero3_enabled"] = is_deepspeed_zero3_enabled()
+            # save finetune args
+            finetune_args_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH))
+            write_dict_to_json_file(self.finetune_params, finetune_args_path)
+
+            # save finetune_config file
+            ft_config_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.ACFT_CONFIG_SAVE_PATH))
+            write_dict_to_json_file(self.ft_config, ft_config_path)
+
+            # copy mlflow inference params file to pytorch output for model converter
+            mlflow_infer_params_file_path = Path(
+                self.finetune_params["preprocess_output"],
+                MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT,
+            )
+            shutil.copy(mlflow_infer_params_file_path, self.finetune_params["pytorch_model_folder"])
 
 
 def qna_metrics_func(
     eval_pred: EvalPrediction,
     tokenizer: PreTrainedTokenizerBase,
     raw_eval_dataset: Dataset,
     enc_eval_dataset: Dataset,
```

## azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/base.py

```diff
@@ -16,32 +16,38 @@
 # limitations under the License.
 # ---------------------------------------------------------
 
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 
-from ....constants.constants import AzuremlConstants, PreprocessArgsTemplate
-from ....constants.constants import Tasks, MLFlowHFFlavourTasks
-from ....constants.constants import STRING_DTYPES, INT_DTYPES
+from ....constants.constants import (
+    AzuremlConstants,
+    MLFlowHFFlavourTasks,
+    PreprocessArgsTemplate,
+    Tasks,
+    INT_DTYPES,
+    STRING_DTYPES
+)
 
-from ....utils.data_utils import AzuremlDataset
+from ....utils.data_utils import AzuremlDataset, clean_column_name
 from ....utils.validation_utils import AzuremlValidatorMixin
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 from datasets import Sequence
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class QnAPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of QnAPreprocessArgs +
     # inhertied attributes from PreprocessArgsTemplate here.
     # Otherwise, there will be issues related to ordering of default and
@@ -124,24 +130,27 @@
             STRING_DTYPES, STRING_DTYPES, "NOT_VALIDATED", INT_DTYPES, STRING_DTYPES
         ]
         #
         if self.placeholder_required_columns is not None:
             for idx, col_name in enumerate(self.placeholder_required_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
-                    self.required_columns.append(decoded_arg)
+                    cleaned_name = clean_column_name(decoded_arg)
+                    setattr(self, col_name, cleaned_name)  # reset with cleaned name for further use
+                    self.required_columns.append(cleaned_name)
                     self.required_column_dtypes.append(self.placeholder_required_column_dtypes[idx])
 
         if self.placeholder_nested_columns is not None:
             self.nested_columns = []
             for idx, col_name in enumerate(self.placeholder_nested_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
                     self.nested_columns.append(decoded_arg)
 
+        self.validate_required_columns()
         self.label_column = getattr(self, self.placeholder_label_column)
 
 
 class QnADataset(AzuremlDataset, AzuremlValidatorMixin):
 
     def __init__(
         self,
@@ -219,18 +228,18 @@
                 update_datset_columns,
                 batched=True,
                 remove_columns=self.dataset.column_names,
                 batch_size=self.dataset_args["batch_size"],
                 writer_batch_size=self.dataset_args["batch_size"]
             )
         except Exception as e:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Data is incorrectly formatted. Error while updating dataset columns: {e}"
+                    ACFTUserError,
+                    pii_safe_message=f"Data is incorrectly formatted. Error while updating dataset columns: {e}"
                 )
             )
 
         # update label column
         if self.label_column is not None:
             self.label_column = AzuremlConstants.DATASET_COLUMN_PREFIX + self.label_column
 
@@ -351,19 +360,25 @@
                         end_char = start_char + len(answers[answer_text_key][0])
 
                         # Start token index of the current span in the text.
                         # TODO check if we can optimize using np
                         token_start_index = 0
                         while sequence_ids[token_start_index] != (1 if pad_on_right else 0):
                             token_start_index += 1
+                            if token_start_index == len(sequence_ids):
+                                token_start_index -= 1
+                                break
 
                         # End token index of the current span in the text.
                         token_end_index = len(input_ids) - 1
                         while sequence_ids[token_end_index] != (1 if pad_on_right else 0):
                             token_end_index -= 1
+                            if token_end_index < 0:
+                                token_end_index += 1
+                                break
 
                         # Detect if the answer is out of the span (in which case this feature is labeled with the CLS index).
                         # offsets[token_start_index][0] <= start_char < end_char <= offsets[token_end_index][1]
                         if not (offsets[token_start_index][0] <= start_char and offsets[token_end_index][1] >= end_char):
                             tokenized_examples["start_positions"].append(cls_index)
                             tokenized_examples["end_positions"].append(cls_index)
                         else:
@@ -432,50 +447,50 @@
         """
 
         # first match outer columns as inner column might or might not always present
         outer_columns = [name for name in self.required_columns if name not in self.nested_columns]
         if sorted(outer_columns) != sorted(self.dataset.column_names):
             logger.warning(
                 "Exception occured while matching outer dataset columns with user passed columns, scrubbing exception")
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=(
+                    ACFTUserError,
+                    pii_safe_message=(
                         f"Path or dict: {self.path_or_dict}."
                         f"Dataset Columns: {self._remove_dataset_column_prefix(self.original_datset_columns)}."
                         f"User Passed Columns: {self._remove_dataset_column_prefix(self.required_columns)}."
                     )
                 )
             )
 
         # match nested columns
         answers_key = self.dataset_args["answers_key"]
         if self.label_column is not None:
             if not isinstance(self.dataset.features[answers_key], dict):
                 logger.warning(
                     "Invalid dataset format found during match columns, scrubbing exception")
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"Path or dict: {self.path_or_dict}."
                             f"Answers format: {type(self.dataset.features[answers_key])}."
                             "Expected format: dict."
                         )
                     )
                 )
 
             nested_answer_keys = list(self.dataset.features[answers_key].keys())
             if sorted(nested_answer_keys) != sorted(self.nested_columns):
                 logger.warning(
                     "Exception occured while matching nested dataset columns with user passed columns, scrubbing exception")
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"Path or dict: {self.path_or_dict}."
                             f"Dataset Columns: {self._remove_dataset_column_prefix(nested_answer_keys)}."
                             f"User Passed Columns: {self._remove_dataset_column_prefix(self.nested_columns)}."
                         )
                     )
                 )
 
@@ -496,18 +511,18 @@
             # special handling for nested columns
             if column_name in self.nested_columns:
                 answers_key = self.dataset_args["answers_key"]
                 sequence_column_type = isinstance(datset_features[answers_key][column_name], Sequence)
                 # Check if answers key is of sequence type
                 if not sequence_column_type:
                     logger.warning("Found invalid feature type for nested column")
-                    raise ValidationException._with_error(
+                    raise ACFTDataException._with_error(
                         AzureMLError.create(
-                            ValidationError,
-                            error=(
+                            ACFTUserError,
+                            pii_safe_message=(
                                 f"File path or data: {self.path_or_dict}\n"
                                 f"type mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                                 f"Found type: {type(datset_features[answers_key][column_name])}\n"
                                 f"Expected type: {Sequence}"
                             )
                         )
                     )
@@ -515,80 +530,78 @@
                 # check for the presence of column name in answers nested dict
                 column_dtype = datset_features[answers_key][column_name].feature.dtype
 
             else:
                 # outer column keys handling
                 if column_name not in datset_features:
                     logger.warning("Exception occured column name not present in dataset features, scrubbing exception")
-                    raise ValidationException._with_error(
+                    raise ACFTDataException._with_error(
                         AzureMLError.create(
-                            ValidationError,
-                            error=(
+                            ACFTUserError,
+                            pii_safe_message=(
                                 f"{column_name} not present in column to dataset features. "
                                 f"The following columns are present: {list(datset_features.keys())}"
                             )
                         )
                     )
                 else:
                     column_dtype = datset_features[column_name].dtype
 
             if column_dtype not in valid_dtypes:
                 logger.warning("Exception occured column dtype not valid, scrubbing exception")
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"File path or data: {self.path_or_dict}\n"
                             f"dtype mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                             f"Found dtype: {column_dtype}\n"
                             f"Expected dtypes: {valid_dtypes}"
                         )
                     )
                 )
 
     def qna_data_filter(self):
         """Remove the examples that contain null data. specific to ner task"""
 
         if self.dataset_args is None:
             logger.info(f"Dataset args is {self.dataset_args}. Skipping qna data filter")
             return
-
-        # filter examples with empty question or empty context
-        def question_context_non_empty(example):
-            if (
-                self.dataset_args["question_key"].strip() == "" or
-                self.dataset_args["context_key"].strip() == ""
-            ):
+        
+        answers_key = self.dataset_args["answers_key"]
+        answer_start_key = self.dataset_args["answer_start_key"]
+        answer_text_key = self.dataset_args["answer_text_key"]
+        
+        # filter examples with mismatched sizes for answer_text_key and answer_start_key
+        def mismatched_start_text_key(example):
+            if len(example[answers_key][answer_start_key]) != len(example[answers_key][answer_text_key]):
                 return False
             return True
 
         pre_filter_rows = self.dataset.num_rows
         self.dataset = self.dataset.filter(
-            question_context_non_empty,
+            mismatched_start_text_key,
             batch_size=self.dataset_args["batch_size"],
             writer_batch_size=self.dataset_args["batch_size"]
         )
         post_filter_rows = self.dataset.num_rows
-        logger.info(f"question_context_non_empty filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
+        logger.info(f"mismatched answer_start and answer_text sizes filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
+        
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
                 )
             )
 
-    def validate(self):
+    def validate(self, split: Optional[str] = None):
+        self.apply_common_validations(split, batch_size=self.dataset_args["batch_size"])
 
-        # Remove the extra columns and match the remaining columns
-        self.remove_extra_columns()
-        self.match_columns()
-
-        # filter data
-        # null filter
-        self.remove_null_examples(batch_size=self.dataset_args["batch_size"])
+        # check if feature columns are identical
+        self.check_column_contents(self.dataset_args["question_key"], self.dataset_args["context_key"])
         # check dtypes
         # NOTE doing dtype check before task specific data filter because :meth single_label_data_filter
         # assumes the dtypes for columns
         self.check_column_dtypes()
         # remove examples with empty sentence1 or sentence2
         self.qna_data_filter()
```

## azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_finetune.py

```diff
@@ -25,58 +25,66 @@
 import json
 
 from .base import QnAPreprocessArgs, QnADataset
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....constants.constants import Tasks, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import InvalidDataset, InvalidLabel, TokenizerNotSupported
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
+from azureml.acft.common_components.utils.error_handling.error_definitions import TokenizerNotSupported
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.tokenization_utils_fast import PreTrainedTokenizerFast
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class QnAPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: QnAPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
         #  - model_name arg from model selector
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
+        self.ft_config = getattr(component_args, "finetune_config", {})
 
         logger.info(f"Task name: {Tasks.QUESTION_ANSWERING}")
 
-        self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
+        self.model_type = AzuremlAutoConfig.get_model_type(
+            hf_model_name_or_path=component_args.model_name_or_path,
+            **self.ft_config.get("load_config_kwargs", {}),
+        )
         logger.info(self.preprocess_args)
 
         self.tokenizer = self._init_tokenizer()
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.QUESTION_ANSWERING,
             "apply_adjust": True,
-            "max_sequence_length": self.preprocess_args.max_seq_length
+            "max_sequence_length": self.preprocess_args.max_seq_length,
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+
         tokenizer = AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
 
         # Only FastTokenizer is supported for QA
         # The python based tokenizer doesn't support `return_offsets_mapping=True`
         if not isinstance(tokenizer, PreTrainedTokenizerFast):
-            raise ValidationException._with_error(
+            raise ACFTValidationException._with_error(
                 AzureMLError.create(
                     TokenizerNotSupported, Tokenizer=tokenizer, TaskName=Tasks.QUESTION_ANSWERING
                 )
             )
         return tokenizer
 
     def _get_encode_dataset_params(self) -> Dict[str, Any]:
@@ -200,20 +208,20 @@
 
         return (raw_train_data_fname, raw_validation_data_fname, raw_test_data_fname)
 
     def _validate_data_splits(self):
         """validate the datasets"""
         # validate the datasets
         logger.info("Validating the train dataset")
-        self.train_ds.validate()
+        self.train_ds.validate(DatasetSplit.TRAIN)
         logger.info("Validating the validation dataset")
-        self.valid_ds.validate()
+        self.valid_ds.validate(DatasetSplit.VALIDATION)
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             logger.info("Validating the test dataset")
-            self.test_ds.validate()
+            self.test_ds.validate(DatasetSplit.TEST)
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset()
```

## azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_inference.py

```diff
@@ -18,22 +18,20 @@
 
 from argparse import Namespace
 
 from .base import NerPreprocessArgs
 from ...constants.constants import Tasks
 from ...nlp_auto.tokenizer import AzuremlAutoTokenizer
 
-from azureml.train.finetune.core.utils.logging_utils import get_logger_app
-from azureml.train.finetune.core.utils.error_handling.exceptions import ValidationException
-from azureml.train.finetune.core.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForInfer():
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
```

## azureml/acft/contrib/hf/nlp/tasks/single_label/runner.py

```diff
@@ -17,46 +17,57 @@
 # ---------------------------------------------------------
 
 from argparse import Namespace
 from typing import List
 
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
-from .preprocess.base import SingleLabelPreprocessArgs
+from .preprocess.base import SingleLabelPreprocessArgs, SingleLabelDataset
 # from .preprocess.preprocess_for_inference import SingleLabelPreprocessForInfer
 
 from transformers.hf_argparser import HfArgumentParser
 
+from azureml.acft.common_components import get_logger_app
+
+
+logger = get_logger_app(__name__)
+
 
 class SingleLabelRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
         from .preprocess.preprocess_for_finetune import SingleLabelPreprocessForFinetune
 
+        load_config_kwargs = getattr(component_args, "finetune_config", {}).get("load_config_kwargs", {})
         self.check_model_task_compatibility(
-            model_name_or_path=component_args.model_name_or_path, task_name=Tasks.SINGLE_LABEL_CLASSIFICATION
+            model_name_or_path=component_args.model_name_or_path,
+            task_name=Tasks.SINGLE_LABEL_CLASSIFICATION,
+            **load_config_kwargs,
         )
 
         preprocess_arg_parser = HfArgumentParser([SingleLabelPreprocessArgs])
-        preprocess_args: SingleLabelPreprocessArgs = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args)[0]
+        output_args = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args, return_remaining_strings=True)
+        preprocess_args: SingleLabelPreprocessArgs = output_args[0]
+
+        logger.info(f"unused args - {output_args[1]}")
 
         preprocess_obj = SingleLabelPreprocessForFinetune(component_args, preprocess_args)
         preprocess_obj.preprocess()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         pass
 
     def run_finetune(self, component_plus_preprocess_args: Namespace) -> None:
 
         from .finetune.finetune import SingleLabelFinetune
 
         self.resolve_resume_from_checkpoint(component_plus_preprocess_args)
 
-        finetune_obj = SingleLabelFinetune(vars(component_plus_preprocess_args))
+        finetune_obj = SingleLabelFinetune(vars(component_plus_preprocess_args), SingleLabelDataset)
         finetune_obj.finetune()
 
     def run_modelselector(self, *args, **kwargs) -> None:
 
         from ...utils.model_selector_utils import model_selector
 
         model_selector(kwargs)
```

## azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/finetune.py

```diff
@@ -15,84 +15,87 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 import json
 import numpy as np
 from pathlib import Path
+import shutil
 
 from typing import Any, Dict, List, Tuple, Optional
 
+from ...base.finetune.finetune import FinetuneBase
 from ....constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, Tasks
 from ....nlp_auto.model import AzuremlAutoModelForSequenceClassification
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ..preprocess.base import SingleLabelDataset
-from ....utils.mlflow_utils import SaveMLflowModelCallback, replace_deepspeed_zero3_mlflow_pytorch_weights
+from ....utils.common_utils import write_dict_to_json_file
 
 import torch.nn as nn
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
 
 from azureml.acft.accelerator.finetune import AzuremlFinetuneArgs, AzuremlDatasetArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
 from azureml.acft.accelerator.constants import HfTrainerType
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_utils import EvalPrediction
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 
+from peft import TaskType
+
 from sklearn.metrics import (
     f1_score,
     accuracy_score,
     matthews_corrcoef,
     precision_score,
     recall_score
 )
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
-class SingleLabelFinetune:
+class SingleLabelFinetune(FinetuneBase):
 
-    def __init__(self, finetune_params: Dict[str, Any]) -> None:
+    def __init__(self, finetune_params: Dict[str, Any], dataset_class) -> None:
         # finetune params is finetune component args + args saved as part of preprocess
         self.finetune_params = finetune_params
+        self.dataset_class = dataset_class
+        self.ft_config = finetune_params.get("finetune_config", {})
 
         logger.info(f"Task name: {Tasks.SINGLE_LABEL_CLASSIFICATION}")
 
         # Load class names
         class_names_load_path = Path(self.finetune_params["preprocess_output"], SaveFileConstants.CLASSES_SAVE_PATH)
         with open(class_names_load_path, 'r') as rptr:
             self.finetune_params["class_names"] = json.load(rptr)[SaveFileConstants.CLASSES_SAVE_KEY]
             self.finetune_params["num_labels"] = len(self.finetune_params["class_names"])
 
         # set log_metrics_at_root=False to not to log to parent
-        self.finetune_params["log_metrics_at_root"] = False
+        self.finetune_params["log_metrics_at_root"] = True
 
     def _get_finetune_args(self, model_type: str) -> AzuremlFinetuneArgs:
 
         self.finetune_params["model_type"] = model_type
+        self.finetune_params["peft_task_type"] = TaskType.SEQ_CLS
         azml_trainer_finetune_args = AzuremlFinetuneArgs(
             self.finetune_params,
-            trainer_type=HfTrainerType.DEFAULT
+            trainer_type=HfTrainerType.DEFAULT,
         )
 
         return azml_trainer_finetune_args
 
-    def _get_dataset_args(self, tokenizer: Optional[PreTrainedTokenizerBase]=None) -> AzuremlDatasetArgs:
+    def _get_dataset_args(self, tokenizer: Optional[PreTrainedTokenizerBase] = None) -> AzuremlDatasetArgs:
 
-        encoded_train_ds = SingleLabelDataset(
+        encoded_train_ds = self.dataset_class(
             Path(self.finetune_params["preprocess_output"], self.finetune_params["encoded_train_data_fname"]),
             tokenizer=tokenizer
         )
-        encoded_validation_ds = SingleLabelDataset(
+        encoded_validation_ds = self.dataset_class(
             Path(self.finetune_params["preprocess_output"], self.finetune_params["encoded_validation_data_fname"]),
         )
         azml_trainer_dataset_args = AzuremlDatasetArgs(
             train_dataset=encoded_train_ds.dataset,
             validation_dataset=encoded_validation_ds.dataset,
             data_collator=encoded_train_ds.get_collation_function()
         )
@@ -107,89 +110,98 @@
         model_params = {
             "problem_type": "single_label_classification",
             "num_labels": self.finetune_params["num_labels"],
             "id2label": id2label,
             "label2id": label2id,
             "ignore_mismatched_sizes": self.finetune_params["ignore_mismatched_sizes"],
             "resume_from_checkpoint": self.finetune_params["resume_from_checkpoint"],
+            "load_in_8bit": self.finetune_params["finetune_in_8bit"],
+            "load_in_4bit": self.finetune_params["finetune_in_4bit"],
         }
 
+        model_params.update(self.ft_config.get("load_model_kwargs", {}))
+        model_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading model with following args: {model_params}")
+
         model, model_type, new_initalized_layers = AzuremlAutoModelForSequenceClassification.from_pretrained(
             self.finetune_params["model_name_or_path"], **model_params)
 
         return model, model_type, new_initalized_layers
 
     def _get_tokenizer(self) -> PreTrainedTokenizerBase:
         """This method loads the tokenizer as is w/o any modifications to it"""
 
         tokenizer_params = {
             "apply_adjust": False,
             "task_name": self.finetune_params["task_name"],
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading tokenizer with following params: {tokenizer_params}")
+
         return AzuremlAutoTokenizer.from_pretrained(self.finetune_params["preprocess_output"], **tokenizer_params)
 
     def finetune(self) -> None:
 
         self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
 
-        # configure MLflow save callback
-        mlflow_infer_params_file_path = Path(
-            self.finetune_params["preprocess_output"], MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT
-        )
-        save_mlflow_callback = SaveMLflowModelCallback(
-            mlflow_infer_params_file_path=mlflow_infer_params_file_path,
-            mlflow_model_save_path=self.finetune_params["mlflow_model_folder"],
-            mlflow_task_type=self.finetune_params["mlflow_task_type"],
-            class_names=self.finetune_params["class_names"],
-            model_name=self.finetune_params["model_name"],
-            model_name_or_path=self.finetune_params["model_name_or_path"],
-        )
-
+        # Initializing the finetune args with dummy_model_type to enable the
+        # deepspeed stage3 which is used in :meth _load_model
+        finetune_args = self._get_finetune_args("dummy_model_type")
         model, model_type, new_initialized_params = self._load_model()
+        # Replacing the dummy_model_type -> original model_type information
+        setattr(finetune_args.optimization_args, "model_type", model_type)
+        self.finetune_params["model_type"] = model_type
         tokenizer = self._get_tokenizer()
         trainer = AzuremlTrainer(
-            finetune_args=self._get_finetune_args(model_type),
+            finetune_args=finetune_args,
             dataset_args=self._get_dataset_args(tokenizer),
             model=model,
             tokenizer=tokenizer,
             metric_func=single_label_metrics_func,
             new_initalized_layers=new_initialized_params,
-            custom_trainer_callbacks=[save_mlflow_callback],
         )
 
+        self._save_mininum_finetune_args(finetune_args)
+
         # Torch barrier is used to complete the training on a distributed setup
         # Use callbacks for adding steps to be done at the end of training
         # NOTE Avoid adding any logic after trainer.train()
         # Test the distributed scenario in case you add any logic beyond trainer.train()
         trainer.train()
 
-        # replace pytorch weights for lora / deep speed zero3 optimization
-        if trainer.should_save and (self.finetune_params["apply_lora"] or is_deepspeed_zero3_enabled()):
-            logger.info("Replacing dummy MLflow weights ")
-            replace_deepspeed_zero3_mlflow_pytorch_weights(
-                self.finetune_params["pytorch_model_folder"],
-                self.finetune_params["mlflow_model_folder"]
-            )
-
         # save files only once by Rank-0 process
         if trainer.should_save:
+            self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
+            # save if model is trained via deepspeed stage 3
+            self.finetune_params["is_deepspeed_zero3_enabled"] = is_deepspeed_zero3_enabled()
             # save finetune args
-            Path(self.finetune_params["pytorch_model_folder"]).mkdir(exist_ok=True, parents=True)
-            finetune_args_path = Path(self.finetune_params["pytorch_model_folder"], \
-                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
-            with open(finetune_args_path, 'w') as rptr:
-                json.dump(self.finetune_params, rptr, indent=2)
-            # save the classes list for azuremlft inference compatability
-            classes_save_path = Path(self.finetune_params["pytorch_model_folder"], SaveFileConstants.CLASSES_SAVE_PATH)
+            finetune_args_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH))
+            write_dict_to_json_file(self.finetune_params, finetune_args_path)
+            # save the classes list for azmlft inference compatability
+            classes_save_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.CLASSES_SAVE_PATH))
             class_names_json = {SaveFileConstants.CLASSES_SAVE_KEY: self.finetune_params["class_names"]}
-            with open(classes_save_path, "w") as wptr:
-                json.dump(class_names_json, wptr)
+            write_dict_to_json_file(class_names_json, classes_save_path)
             logger.info(f"Classes file saved at {classes_save_path}")
 
+            # save finetune_config file
+            ft_config_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.ACFT_CONFIG_SAVE_PATH))
+            write_dict_to_json_file(self.ft_config, ft_config_path)
+
+            # copy mlflow inference params file to pytorch output for model converter
+            mlflow_infer_params_file_path = Path(
+                self.finetune_params["preprocess_output"],
+                MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT,
+            )
+            shutil.copy(mlflow_infer_params_file_path, self.finetune_params["pytorch_model_folder"])
+
 
 def single_label_metrics_func(eval_pred: EvalPrediction) -> Dict[str, Any]:
     """
     compute and return metrics for sequence classification
     """
 
     predictions, labels = eval_pred
```

## azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/base.py

```diff
@@ -16,31 +16,37 @@
 # limitations under the License.
 # ---------------------------------------------------------
 
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 
-from ....constants.constants import AzuremlConstants, PreprocessArgsTemplate
-from ....constants.constants import Tasks, MLFlowHFFlavourTasks
-from ....constants.constants  import STRING_DTYPES, INT_DTYPES
+from ....constants.constants import (
+    AzuremlConstants,
+    MLFlowHFFlavourTasks,
+    PreprocessArgsTemplate,
+    Tasks,
+    INT_DTYPES,
+    STRING_DTYPES
+)
 
-from ....utils.data_utils import AzuremlDataset
+from ....utils.data_utils import AzuremlDataset, clean_column_name
 from ....utils.validation_utils import AzuremlValidatorMixin
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorWithPadding
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class SingleLabelPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of SingleLabelPreprocessArgs +
     # inhertied attributes from PreprocessArgsTemplate here.
     # Otherwise, there will be issues related to ordering of default and
@@ -94,17 +100,19 @@
             STRING_DTYPES, STRING_DTYPES, STRING_DTYPES+INT_DTYPES
         ]
         #
         if self.placeholder_required_columns is not None:
             for idx, col_name in enumerate(self.placeholder_required_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
-                    self.required_columns.append(decoded_arg)
+                    cleaned_name = clean_column_name(decoded_arg)
+                    setattr(self, col_name, cleaned_name)  # reset with cleaned name for further use
+                    self.required_columns.append(cleaned_name)
                     self.required_column_dtypes.append(self.placeholder_required_column_dtypes[idx])
-
+        self.validate_required_columns()
         self.label_column = getattr(self, self.placeholder_label_column)
 
 
 class SingleLabelDataset(AzuremlDataset, AzuremlValidatorMixin):
 
     def __init__(
         self,
@@ -225,29 +233,25 @@
             filter_lambda,
             batch_size=self.dataset_args["batch_size"],
             writer_batch_size=self.dataset_args["batch_size"]
         )
         post_filter_rows = self.dataset.num_rows
         logger.info(f"Singlelabel data filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
                 )
             )
 
-    def validate(self):
+    def validate(self, split: Optional[str] = None):
+        self.apply_common_validations(split, batch_size=self.dataset_args["batch_size"])
 
-        # Remove the extra columns and match the remaining columns
-        self.remove_extra_columns()
-        self.match_columns()
-
-        # filter data
-        # null filter
-        self.remove_null_examples(batch_size=self.dataset_args["batch_size"])
+        # check if feature columns are identical
+        self.check_column_contents(self.dataset_args["sentence1_key"], self.dataset_args["sentence2_key"])
         # check dtypes
         # NOTE doing dtype check before task specific data filter because :meth single_label_data_filter
         # assumes the dtypes for columns
         self.check_column_dtypes()
         # remove examples with empty sentence1 or sentence2
         self.single_label_data_filter()
```

## azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_finetune.py

```diff
@@ -25,55 +25,62 @@
 import json
 
 from .base import SingleLabelPreprocessArgs, SingleLabelDataset
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....constants.constants import Tasks, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException, LLMException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import (
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import (
     InvalidDataset,
     InvalidLabel,
-    LLMInternalError,
+    ACFTUserError,
 )
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class SingleLabelPreprocessForFinetune:
 
     def __init__(self, component_args: Namespace, preprocess_args: SingleLabelPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
         #  - model_name arg from model selector
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
+        self.ft_config = getattr(component_args, "finetune_config", {})
 
         logger.info(f"Task name: {Tasks.SINGLE_LABEL_CLASSIFICATION}")
 
-        self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
+        self.model_type = AzuremlAutoConfig.get_model_type(
+            hf_model_name_or_path=component_args.model_name_or_path,
+            **self.ft_config.get("load_config_kwargs", {}),
+        )
         logger.info(self.preprocess_args)
 
         self.tokenizer = self._init_tokenizer()
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.SINGLE_LABEL_CLASSIFICATION,
             "apply_adjust": True,
-            "max_sequence_length": self.preprocess_args.max_seq_length
+            "max_sequence_length": self.preprocess_args.max_seq_length,
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+
         return AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
 
     def _get_encode_dataset_params(self) -> Dict[str, Any]:
 
         encode_params = {}
         # padding and truncation
         encode_params["padding"] = "max_length" if self.preprocess_args.pad_to_max_length else False
@@ -191,53 +198,54 @@
     def _validate_data_splits(self):
         """
         1. validate the datasets
         2. Identify the classnames and do some validations on them
         """
         # validate the datasets
         logger.info("Validating the train dataset")
-        self.train_ds.validate()
+        self.train_ds.validate(DatasetSplit.TRAIN)
         logger.info("Validating the validation dataset")
-        self.valid_ds.validate()
+        self.valid_ds.validate(DatasetSplit.VALIDATION)
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             logger.info("Validating the test dataset")
-            self.test_ds.validate()
+            self.test_ds.validate(DatasetSplit.TEST)
 
         # validate if train and validation dataset labels are of same data types
         train_class_names = self.train_ds.class_names  # type: ignore
         valid_class_names = self.valid_ds.class_names  # type: ignore
         same_class_type = True
         if train_class_names and len(train_class_names) > 0:
             same_class_type = all(isinstance(x, type(train_class_names[0])) for x in train_class_names)
             if same_class_type and valid_class_names and len(valid_class_names) > 0:
                 same_class_type = all(isinstance(x, type(train_class_names[0])) for x in valid_class_names)
             else:
                 same_class_type = False
         else:
             same_class_type = False
         if not same_class_type:
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=(
-                    "Train and Validation datasets have different data types as labels"
-                ))
+            raise ACFTDataException._with_error(
+                AzureMLError.create(
+                    ACFTUserError, 
+                    pii_safe_message=f"Train and Validation datasets have different data types as labels"
+                    )
             )
 
         # Identify the class names - combination of train and validation datasets
         # class names are list of strings
         self.class_names_train_plus_valid = sorted(set(self.train_ds.class_names + self.valid_ds.class_names))  #type: ignore
         # few classes to do classification
         if len(self.class_names_train_plus_valid) < 2:
-            raise ValidationException._with_error(AzureMLError.create(InvalidDataset))
+            raise ACFTDataException._with_error(AzureMLError.create(InvalidDataset))
         logger.info(f"Identified class names: {self.class_names_train_plus_valid}")
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             self.class_names_test= self.test_ds.class_names
             # test ds has extra classes that are not in train and valid
             test_ds_extra_labels = set(self.class_names_test).difference(set(self.class_names_train_plus_valid))  #type: ignore
             if test_ds_extra_labels:
-                raise ValidationException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
+                raise ACFTDataException._with_error(AzureMLError.create(InvalidLabel, label=test_ds_extra_labels))
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset(class_names_train_plus_valid=self.class_names_train_plus_valid)
```

## azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_inference.py

```diff
@@ -18,22 +18,20 @@
 
 from argparse import Namespace
 
 from .base import NerPreprocessArgs
 from ...constants.constants import Tasks
 from ...nlp_auto.tokenizer import AzuremlAutoTokenizer
 
-from azureml.train.finetune.core.utils.logging_utils import get_logger_app
-from azureml.train.finetune.core.utils.error_handling.exceptions import ValidationException
-from azureml.train.finetune.core.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForInfer():
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
```

## azureml/acft/contrib/hf/nlp/tasks/summarization/runner.py

```diff
@@ -26,26 +26,38 @@
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
 from .preprocess.base import SummarizationPreprocessArgs
 # from .preprocess.preprocess_for_inference import SummarizationPreprocessForInfer
 
 from transformers.hf_argparser import HfArgumentParser
 
+from azureml.acft.common_components import get_logger_app
+
+
+logger = get_logger_app(__name__)
+
 
 class SummarizationRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
         from .preprocess.preprocess_for_finetune import SummarizationPreprocessForFinetune
 
+        load_config_kwargs = getattr(component_args, "finetune_config", {}).get("load_config_kwargs", {})
         self.check_model_task_compatibility(
-            model_name_or_path=component_args.model_name_or_path, task_name=Tasks.SUMMARIZATION)
+            model_name_or_path=component_args.model_name_or_path,
+            task_name=Tasks.SUMMARIZATION,
+            **load_config_kwargs,
+        )
 
         preprocess_arg_parser = HfArgumentParser([SummarizationPreprocessArgs])
-        preprocess_args: SummarizationPreprocessArgs = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args)[0]
+        output_args = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args, return_remaining_strings=True)
+        preprocess_args: SummarizationPreprocessArgs = output_args[0]
+
+        logger.info(f"unused args - {output_args[1]}")
 
         preprocess_obj = SummarizationPreprocessForFinetune(component_args, preprocess_args)
         preprocess_obj.preprocess()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         data = kwargs["data"]
         return data
```

## azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/finetune.py

```diff
@@ -12,72 +12,75 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
-import json
 import numpy as np
 from pathlib import Path
 from functools import partial
+import shutil
 
 from typing import Any, Dict, List, Tuple, Optional
 
 from ..preprocess.base import SummarizationDataset
+from ...base.finetune.finetune import FinetuneBase
 from ....constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, TaskConstants, Tasks
 from ....nlp_auto.model import AzuremlAutoModelForSummarization
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ....utils.mlflow_utils import SaveMLflowModelCallback, replace_deepspeed_zero3_mlflow_pytorch_weights
+from ....utils.common_utils import write_dict_to_json_file
+from ....metrics.load_metric import load_acft_metric
 
 import torch.nn as nn
 import nltk
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-
 from azureml.acft.accelerator.finetune import AzuremlFinetuneArgs, AzuremlDatasetArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
 from azureml.acft.accelerator.constants import HfTrainerType
-
-from datasets.load import load_metric
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_utils import EvalPrediction
 from transformers.models.mbart.tokenization_mbart import MBartTokenizer
 from transformers.models.mbart.tokenization_mbart_fast import MBartTokenizerFast
 from transformers.models.mbart50.tokenization_mbart50 import MBart50Tokenizer
 from transformers.models.mbart50.tokenization_mbart50_fast import MBart50TokenizerFast
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 
+from peft import TaskType
+
 MULTILINGUAL_TOKENIZERS = [MBartTokenizer, MBartTokenizerFast, MBart50Tokenizer, MBart50TokenizerFast]
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
-class SummarizationFinetune:
+class SummarizationFinetune(FinetuneBase):
 
     def __init__(self, finetune_params: Dict[str, Any]) -> None:
         # finetune params is finetune component args + args saved as part of preprocess
         self.finetune_params = finetune_params
+        self.ft_config = finetune_params.get("finetune_config", {})
 
         logger.info(f"Task name: {Tasks.SUMMARIZATION}")
 
         # set predict_with_generate=True for Summarization
         self.finetune_params["predict_with_generate"] = True
 
         # set log_metrics_at_root=False to not to log to parent
         self.finetune_params["log_metrics_at_root"] = False
 
     def _get_finetune_args(self, model_type: str) -> AzuremlFinetuneArgs:
 
         self.finetune_params["model_type"] = model_type
+        self.finetune_params["peft_task_type"] = TaskType.SEQ_2_SEQ_LM
         azml_trainer_finetune_args = AzuremlFinetuneArgs(
             self.finetune_params,
-            trainer_type=HfTrainerType.SEQ2SEQ
+            trainer_type=HfTrainerType.SEQ2SEQ,
         )
 
         return azml_trainer_finetune_args
 
     def _get_dataset_args(self, tokenizer: Optional[PreTrainedTokenizerBase] = None) -> AzuremlDatasetArgs:
 
         encoded_train_ds = SummarizationDataset(
@@ -97,16 +100,22 @@
 
     def _load_model(self, tokenizer: PreTrainedTokenizerBase) -> Tuple[nn.Module, str, List[str]]:
 
         model_params = {
             "tok_prefix": self.finetune_params["tok_prefix"],
             "ignore_mismatched_sizes": self.finetune_params["ignore_mismatched_sizes"],
             "resume_from_checkpoint": self.finetune_params["resume_from_checkpoint"],
+            "load_in_8bit": self.finetune_params["finetune_in_8bit"],
+            "load_in_4bit": self.finetune_params["finetune_in_4bit"],
         }
 
+        model_params.update(self.ft_config.get("load_model_kwargs", {}))
+        model_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading model with following args: {model_params}")
+
         # load the model
         model, model_type, new_initalized_layers = AzuremlAutoModelForSummarization.from_pretrained(
             self.finetune_params["model_name_or_path"], **model_params)
 
         if isinstance(tokenizer, tuple(MULTILINGUAL_TOKENIZERS)):
             model.config.forced_bos_token_id = tokenizer.lang_code_to_id[tokenizer.tgt_lang]
             logger.info(f"`config.forced_bos_token_id` is set to {model.config.forced_bos_token_id}")
@@ -117,79 +126,82 @@
         """This method loads the tokenizer as is w/o any modifications to it"""
 
         tokenizer_params = {
             "apply_adjust": False,
             "task_name": self.finetune_params["task_name"],
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading tokenizer with following params: {tokenizer_params}")
+
         return AzuremlAutoTokenizer.from_pretrained(self.finetune_params["preprocess_output"], **tokenizer_params)
 
     def finetune(self) -> None:
 
-        # configure MLflow save callback
-        mlflow_infer_params_file_path = Path(
-            self.finetune_params["preprocess_output"], MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT
-        )
-        save_mlflow_callback = SaveMLflowModelCallback(
-            mlflow_infer_params_file_path=mlflow_infer_params_file_path,
-            mlflow_model_save_path=self.finetune_params["mlflow_model_folder"],
-            mlflow_task_type=self.finetune_params["mlflow_task_type"],
-            model_name=self.finetune_params["model_name"],
-            model_name_or_path=self.finetune_params["model_name_or_path"],
-        )
-
         # load the tokenizer
         tokenizer = self._get_tokenizer()
         # load the model
+        # Initializing the finetune args with dummy_model_type to enable the
+        # deepspeed stage3 which is used in :meth _load_model
+        finetune_args = self._get_finetune_args("dummy_model_type")
         model, model_type, new_initialized_params = self._load_model(tokenizer)
+        # Replacing the dummy_model_type -> original model_type information
+        setattr(finetune_args.optimization_args, "model_type", model_type)
+        self.finetune_params["model_type"] = model_type
 
         trainer = AzuremlTrainer(
-            finetune_args=self._get_finetune_args(model_type),
+            finetune_args=finetune_args,
             dataset_args=self._get_dataset_args(tokenizer),
             model=model,
             tokenizer=tokenizer,
             metric_func=partial(
                 summarization_metrics_func,
                 tokenizer=tokenizer
             ),
             new_initalized_layers=new_initialized_params,
-            custom_trainer_callbacks=[save_mlflow_callback],
         )
 
+        self._save_mininum_finetune_args(finetune_args)
+
         # Torch barrier is used to complete the training on a distributed setup
         # Use callbacks for adding steps to be done at the end of training
         # NOTE Avoid adding any logic after trainer.train()
         # Test the distributed scenario in case you add any logic beyond trainer.train()
         trainer.train()
 
-        # replace pytorch weights for lora / deep speed zero3 optimization
-        if trainer.should_save and (self.finetune_params["apply_lora"] or is_deepspeed_zero3_enabled()):
-            logger.info("Replacing dummy MLflow weights ")
-            replace_deepspeed_zero3_mlflow_pytorch_weights(
-                self.finetune_params["pytorch_model_folder"],
-                self.finetune_params["mlflow_model_folder"]
-            )
-
         # save files only once by Rank-0 process
         if trainer.should_save:
-            # save finetune args
-            Path(self.finetune_params["pytorch_model_folder"]).mkdir(exist_ok=True, parents=True)
-            finetune_args_path = Path(
-                self.finetune_params["pytorch_model_folder"], SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
             self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
-            with open(finetune_args_path, 'w') as rptr:
-                json.dump(self.finetune_params, rptr, indent=2)
+            # save if model is trained via deepspeed stage 3
+            self.finetune_params["is_deepspeed_zero3_enabled"] = is_deepspeed_zero3_enabled()
+            # save finetune args
+            finetune_args_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH))
+            write_dict_to_json_file(self.finetune_params, finetune_args_path)
+
+            # save finetune_config file
+            ft_config_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.ACFT_CONFIG_SAVE_PATH))
+            write_dict_to_json_file(self.ft_config, ft_config_path)
+
+            # copy mlflow inference params file to pytorch output for model converter
+            mlflow_infer_params_file_path = Path(
+                self.finetune_params["preprocess_output"],
+                MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT,
+            )
+            shutil.copy(mlflow_infer_params_file_path, self.finetune_params["pytorch_model_folder"])
 
 
 def summarization_metrics_func(eval_pred: EvalPrediction, tokenizer: PreTrainedTokenizerBase):
     """
     compute and return metrics for summarization
     """
 
-    metric = load_metric("rouge")
+    metric = load_acft_metric("rouge")
     predictions, labels = eval_pred
     decoded_preds = tokenizer.batch_decode(predictions, skip_special_tokens=True)
     # Replace -100 in the labels as we can't decode them.
     labels = np.where(labels != TaskConstants.SUMMARIZATION_IGNORE_INDEX, labels, tokenizer.pad_token_id)
     decoded_labels = tokenizer.batch_decode(labels, skip_special_tokens=True)
 
     # Rouge expects a newline after each sentence
```

## azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/base.py

```diff
@@ -12,46 +12,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
-import json
 from pathlib import Path
-from argparse import Namespace
 
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 
-import torch.nn as nn
+from ....constants.constants import (
+    AzuremlConstants,
+    MLFlowHFFlavourTasks,
+    PreprocessArgsTemplate,
+    TaskConstants,
+    Tasks,
+    STRING_DTYPES
+)
 
-from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ....nlp_auto.config import AzuremlAutoConfig
-from ....constants.constants import DatasetSplit, SaveFileConstants, AzuremlConstants, MLFlowHFFlavourConstants, PreprocessArgsTemplate
-from ....constants.constants import Tasks, MLFlowHFFlavourTasks, STRING_DTYPES, TaskConstants
-from ....base_runner import BaseRunner
-
-from ....utils.data_utils import AzuremlDataset
+from ....utils.data_utils import AzuremlDataset, clean_column_name
 from ....utils.validation_utils import AzuremlValidatorMixin
 
-from datasets.arrow_dataset import Dataset
-from datasets import Sequence
-
-import transformers
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorForSeq2Seq
-from transformers.hf_argparser import HfArgumentParser
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class SummarizationPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of SummarizationPreprocessArgs + inhertied attributes from
     # _PreprocessArgsTemplate here. Otherwise, there will be issues related to ordering of default and
     # non-default attributes
@@ -115,17 +110,19 @@
         self.placeholder_required_columns = ["document_key", "summary_key"]
         self.placeholder_required_column_dtypes = [STRING_DTYPES, STRING_DTYPES]
         #
         if self.placeholder_required_columns is not None:
             for idx, col_name in enumerate(self.placeholder_required_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
-                    self.required_columns.append(decoded_arg)
+                    cleaned_name = clean_column_name(decoded_arg)
+                    setattr(self, col_name, cleaned_name)  # reset with cleaned name for further use
+                    self.required_columns.append(cleaned_name)
                     self.required_column_dtypes.append(self.placeholder_required_column_dtypes[idx])
-
+        self.validate_required_columns()
         self.label_column = getattr(self, self.placeholder_label_column)
 
 
 class SummarizationDataset(AzuremlDataset, AzuremlValidatorMixin):
 
     def __init__(
         self,
@@ -251,29 +248,25 @@
             filter_lambda,
             batch_size=self.dataset_args["batch_size"],
             writer_batch_size=self.dataset_args["batch_size"]
         )
         post_filter_rows = self.dataset.num_rows
         logger.info(f"Summarization data filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
                 )
             )
 
-    def validate(self):
+    def validate(self, split: Optional[str] = None):
+        self.apply_common_validations(split, batch_size=self.dataset_args["batch_size"])
 
-        # Remove the extra columns and match the remaining columns
-        self.remove_extra_columns()
-        self.match_columns()
-
-        # filter data
-        # null filter
-        self.remove_null_examples(batch_size=self.dataset_args["batch_size"])
+        # check if feature columns are identical
+        self.check_column_contents(self.dataset_args['document_key'], self.dataset_args['summary_key'])
         # check dtypes
         # NOTE doing dtype check before task specific data filter because :meth summarization_data_filter
         # assumes the dtypes for columns
         self.check_column_dtypes()
         # using ner specific filter
         self.summarization_data_filter()
```

## azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_finetune.py

```diff
@@ -27,29 +27,20 @@
 import json
 
 from .base import SummarizationPreprocessArgs, SummarizationDataset
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....constants.constants import Tasks, HfModelTypes, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import (
-    TokenizerNotSupported,
-    InvalidLabel, 
-    InvalidDataset,
-    BadArgument,
-)
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
-from transformers.tokenization_utils_fast import PreTrainedTokenizerFast
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 BART_LANGUAGE_CODES = ["en"]
 T5_SOURCE_LANGUAGE_CODES = ["en"]
 T5_TARGET_LANGUAGE_CODES = ["fr", "de", "ro"]
 MBART_LANGUAGE_CODES = ["ar_AR", "cs_CZ", "de_DE", "en_XX", "es_XX", "et_EE", "fi_FI", "fr_XX", "gu_IN", "hi_IN", "it_IT", "ja_XX", "kk_KZ", "ko_KR", "lt_LT", "lv_LV", "my_MM", "ne_NP", "nl_XX", "ro_RO", "ru_RU", "si_LK", "tr_TR", "vi_VN", "zh_CN"]
 
@@ -59,18 +50,22 @@
     def __init__(self, component_args: Namespace, preprocess_args: SummarizationPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
         #  - model_name arg from model selector
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
+        self.ft_config = getattr(component_args, "finetune_config", {})
 
         logger.info(f"Task name: {Tasks.SUMMARIZATION}")
 
-        self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
+        self.model_type = AzuremlAutoConfig.get_model_type(
+            hf_model_name_or_path=component_args.model_name_or_path,
+            **self.ft_config.get("load_config_kwargs", {}),
+        )
         if self.model_type == HfModelTypes.T5:
             self.preprocess_args.tok_prefix = "summarize: "
             logger.info(f'Setting tokenizer prefix to "{self.preprocess_args.tok_prefix}"')
         logger.info(self.preprocess_args)
         # validate summarization language
         self._validate_summarization_lang_setting()
 
@@ -114,24 +109,27 @@
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.SUMMARIZATION,
             "apply_adjust": True,
-            "max_sequence_length": self.preprocess_args.max_seq_length
+            "max_sequence_length": self.preprocess_args.max_seq_length,
         }
         if self.model_type == HfModelTypes.MBART:
             tokenizer_params.update(
                 {
                     "src_lang": self.preprocess_args.summarization_lang,
-                    "tgt_lang": self.preprocess_args.summarization_lang
+                    "tgt_lang": self.preprocess_args.summarization_lang,
                 }
             )
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+
         return AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
 
     def _get_encode_dataset_params(self) -> Dict[str, Any]:
 
         encode_params = {}
         # padding and truncation
         encode_params["padding"] = "max_length" if self.preprocess_args.pad_to_max_length else False
@@ -255,20 +253,20 @@
         if save_raw_data:
             return (raw_train_data_fname, raw_validation_data_fname, raw_test_data_fname)
 
     def _validate_data_splits(self):
         """validate the datasets"""
         # validate the datasets
         logger.info("Validating the train dataset")
-        self.train_ds.validate()
+        self.train_ds.validate(DatasetSplit.TRAIN)
         logger.info("Validating the validation dataset")
-        self.valid_ds.validate()
+        self.valid_ds.validate(DatasetSplit.VALIDATION)
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             logger.info("Validating the test dataset")
-            self.test_ds.validate()
+            self.test_ds.validate(DatasetSplit.TEST)
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset()
```

## azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_inference.py

```diff
@@ -22,19 +22,19 @@
 
 from argparse import Namespace
 
 from .base import NerPreprocessArgs
 from ....constants.constants import Tasks
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForInfer():
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
```

## azureml/acft/contrib/hf/nlp/tasks/translation/runner.py

```diff
@@ -22,26 +22,38 @@
 from ...constants.constants import Tasks
 from ...base_runner import BaseRunner
 from .preprocess.base import TranslationPreprocessArgs
 # from .preprocess.preprocess_for_inference import TranslationPreprocessForInfer
 
 from transformers.hf_argparser import HfArgumentParser
 
+from azureml.acft.common_components import get_logger_app
+
+
+logger = get_logger_app(__name__)
+
 
 class TranslationRunner(BaseRunner):
 
     def run_preprocess_for_finetune(self, component_args: Namespace, unknown_args: List[str]) -> None:
 
         from .preprocess.preprocess_for_finetune import TranslationPreprocessForFinetune
 
+        load_config_kwargs = getattr(component_args, "finetune_config", {}).get("load_config_kwargs", {})
         self.check_model_task_compatibility(
-            model_name_or_path=component_args.model_name_or_path, task_name=Tasks.TRANSLATION)
+            model_name_or_path=component_args.model_name_or_path,
+            task_name=Tasks.TRANSLATION,
+            **load_config_kwargs,
+        )
 
         preprocess_arg_parser = HfArgumentParser([TranslationPreprocessArgs])
-        preprocess_args: TranslationPreprocessArgs = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args)[0]
+        output_args = preprocess_arg_parser.parse_args_into_dataclasses(unknown_args, return_remaining_strings=True)
+        preprocess_args: TranslationPreprocessArgs = output_args[0]
+
+        logger.info(f"unused args - {output_args[1]}")
 
         preprocess_obj = TranslationPreprocessForFinetune(component_args, preprocess_args)
         preprocess_obj.preprocess()
 
     def run_preprocess_for_infer(self, *args, **kwargs) -> None:
         data = kwargs["data"]
         return data
```

## azureml/acft/contrib/hf/nlp/tasks/translation/finetune/finetune.py

```diff
@@ -12,72 +12,76 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
-import json
 import numpy as np
 from pathlib import Path
 from functools import partial
+import shutil
 
 from typing import Any, Dict, List, Tuple, Optional
 
 from ..preprocess.base import TranslationDataset
+from ...base.finetune.finetune import FinetuneBase
 from ....constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, TaskConstants, Tasks
 from ....nlp_auto.model import AzuremlAutoModelForTranslation
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ....utils.mlflow_utils import SaveMLflowModelCallback, replace_deepspeed_zero3_mlflow_pytorch_weights
+from ....utils.common_utils import write_dict_to_json_file
+from ....metrics.load_metric import load_acft_metric
 
 import torch.nn as nn
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
 from azureml.acft.accelerator.finetune import AzuremlFinetuneArgs, AzuremlDatasetArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
 from azureml.acft.accelerator.constants import HfTrainerType
-
-from datasets.load import load_metric
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_utils import EvalPrediction
 from transformers.models.mbart.tokenization_mbart import MBartTokenizer
 from transformers.models.mbart.tokenization_mbart_fast import MBartTokenizerFast
 from transformers.models.mbart50.tokenization_mbart50 import MBart50Tokenizer
 from transformers.models.mbart50.tokenization_mbart50_fast import MBart50TokenizerFast
 from transformers.models.m2m_100.tokenization_m2m_100 import M2M100Tokenizer
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 
+from peft import TaskType
+
 
 MULTILINGUAL_TOKENIZERS = [MBartTokenizer, MBartTokenizerFast, MBart50Tokenizer, MBart50TokenizerFast]
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
-class TranslationFinetune:
+class TranslationFinetune(FinetuneBase):
 
     def __init__(self, finetune_params: Dict[str, Any]) -> None:
         # finetune params is finetune component args + args saved as part of preprocess
         self.finetune_params = finetune_params
+        self.ft_config = finetune_params.get("finetune_config", {})
 
         logger.info(f"Task name: {Tasks.TRANSLATION}")
 
         # set predict_with_generate=True for Translation
         self.finetune_params["predict_with_generate"] = True
 
         # set log_metrics_at_root=False to not to log to parent
         self.finetune_params["log_metrics_at_root"] = False
 
     def _get_finetune_args(self, model_type: str) -> AzuremlFinetuneArgs:
 
         self.finetune_params["model_type"] = model_type
+        self.finetune_params["peft_task_type"] = TaskType.SEQ_2_SEQ_LM
         azml_trainer_finetune_args = AzuremlFinetuneArgs(
             self.finetune_params,
-            trainer_type=HfTrainerType.SEQ2SEQ
+            trainer_type=HfTrainerType.SEQ2SEQ,
         )
 
         return azml_trainer_finetune_args
 
     def _get_dataset_args(self, tokenizer: Optional[PreTrainedTokenizerBase] = None) -> AzuremlDatasetArgs:
 
         encoded_train_ds = TranslationDataset(
@@ -90,23 +94,25 @@
         azml_trainer_dataset_args = AzuremlDatasetArgs(
             train_dataset=encoded_train_ds.dataset,
             validation_dataset=encoded_validation_ds.dataset,
             data_collator=encoded_train_ds.get_collation_function()
         )
 
         return azml_trainer_dataset_args
-    
+
     def _load_model(self, tokenizer: PreTrainedTokenizerBase) -> Tuple[nn.Module, str, List[str]]:
 
         model_params = {
             "tok_prefix": self.finetune_params["tok_prefix"],
             "source_lang": self.finetune_params["source_lang"],
             "target_lang": self.finetune_params["target_lang"],
             "ignore_mismatched_sizes": self.finetune_params["ignore_mismatched_sizes"],
             "resume_from_checkpoint": self.finetune_params["resume_from_checkpoint"],
+            "load_in_8bit": self.finetune_params["finetune_in_8bit"],
+            "load_in_4bit": self.finetune_params["finetune_in_4bit"],
         }
 
         if isinstance(tokenizer, MBartTokenizer):
             model_params.update(
                 {
                     "decoder_start_token_id": tokenizer.lang_code_to_id[tokenizer.tgt_lang]
                 }
@@ -116,14 +122,18 @@
             model_params.update(
                 {
                     "decoder_start_token_id": tokenizer.convert_tokens_to_ids(tokenizer.tgt_lang)
                 }
             )
             logger.info(f'decoder_start_token_id is set to {model_params["decoder_start_token_id"]}')
 
+        model_params.update(self.ft_config.get("load_model_kwargs", {}))
+        model_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading model with following args: {model_params}")
+
         # load the model
         model, model_type, new_initalized_layers = AzuremlAutoModelForTranslation.from_pretrained(
             self.finetune_params["model_name_or_path"], **model_params,
         )
 
         if isinstance(tokenizer, tuple(MULTILINGUAL_TOKENIZERS)) and model.config.decoder_start_token_id is None:
             raise ValueError("Make sure that `config.decoder_start_token_id` is correctly defined")
@@ -141,81 +151,86 @@
         """This method loads the tokenizer as is w/o any modifications to it"""
 
         tokenizer_params = {
             "apply_adjust": False,
             "task_name": self.finetune_params["task_name"],
         }
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+        logger.info(f"Loading tokenizer with following params: {tokenizer_params}")
+
         return AzuremlAutoTokenizer.from_pretrained(self.finetune_params["preprocess_output"], **tokenizer_params)
 
     def finetune(self) -> None:
 
-        # configure MLflow save callback
-        mlflow_infer_params_file_path = Path(
-            self.finetune_params["preprocess_output"], MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT
-        )
-        save_mlflow_callback = SaveMLflowModelCallback(
-            mlflow_infer_params_file_path=mlflow_infer_params_file_path,
-            mlflow_model_save_path=self.finetune_params["mlflow_model_folder"],
-            mlflow_task_type=self.finetune_params["mlflow_task_type"],
-            model_name=self.finetune_params["model_name"],
-            model_name_or_path=self.finetune_params["model_name_or_path"],
-        )
-
+        # load the tokenizer
         tokenizer = self._get_tokenizer()
+        # load the model
+        # Initializing the finetune args with dummy_model_type to enable the
+        # deepspeed stage3 which is used in :meth _load_model
+        finetune_args = self._get_finetune_args("dummy_model_type")
         model, model_type, new_initialized_params = self._load_model(tokenizer)
+        # Replacing the dummy_model_type -> original model_type information
+        setattr(finetune_args.optimization_args, "model_type", model_type)
+        self.finetune_params["model_type"] = model_type
         trainer = AzuremlTrainer(
-            finetune_args=self._get_finetune_args(model_type),
+            finetune_args=finetune_args,
             dataset_args=self._get_dataset_args(tokenizer),
             model=model,
             tokenizer=tokenizer,
             metric_func=partial(
                 translation_metrics_func,
                 tokenizer=tokenizer
             ),
             new_initalized_layers=new_initialized_params,
-            custom_trainer_callbacks=[save_mlflow_callback],
         )
 
+        self._save_mininum_finetune_args(finetune_args)
+
         # Torch barrier is used to complete the training on a distributed setup
         # Use callbacks for adding steps to be done at the end of training
         # NOTE Avoid adding any logic after trainer.train()
         # Test the distributed scenario in case you add any logic beyond trainer.train()
         trainer.train()
 
-        # replace pytorch weights for lora / deep speed zero3 optimization
-        if trainer.should_save and (self.finetune_params["apply_lora"] or is_deepspeed_zero3_enabled()):
-            logger.info("Replacing dummy MLflow weights ")
-            replace_deepspeed_zero3_mlflow_pytorch_weights(
-                self.finetune_params["pytorch_model_folder"],
-                self.finetune_params["mlflow_model_folder"]
-            )
-
         # save files only once by Rank-0 process
         if trainer.should_save:
-            # save finetune args
-            Path(self.finetune_params["pytorch_model_folder"]).mkdir(exist_ok=True, parents=True)
-            finetune_args_path = Path(
-                self.finetune_params["pytorch_model_folder"], SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
             self.finetune_params["model_name_or_path"] = str(self.finetune_params["model_name_or_path"])
-            with open(finetune_args_path, 'w') as rptr:
-                json.dump(self.finetune_params, rptr, indent=2)
+            # save if model is trained via deepspeed stage 3
+            self.finetune_params["is_deepspeed_zero3_enabled"] = is_deepspeed_zero3_enabled()
+            # save finetune args
+            finetune_args_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.FINETUNE_ARGS_SAVE_PATH))
+            write_dict_to_json_file(self.finetune_params, finetune_args_path)
+
+            # save finetune_config file
+            ft_config_path = str(Path(self.finetune_params["pytorch_model_folder"], \
+                SaveFileConstants.ACFT_CONFIG_SAVE_PATH))
+            write_dict_to_json_file(self.ft_config, ft_config_path)
+
+            # copy mlflow inference params file to pytorch output for model converter
+            mlflow_infer_params_file_path = Path(
+                self.finetune_params["preprocess_output"],
+                MLFlowHFFlavourConstants.INFERENCE_PARAMS_SAVE_NAME_WITH_EXT,
+            )
+            shutil.copy(mlflow_infer_params_file_path, self.finetune_params["pytorch_model_folder"])
 
 
 def translation_metrics_func(eval_pred: EvalPrediction, tokenizer: PreTrainedTokenizerBase):
     """
     compute and return metrics for translation
     """
     def postprocess_text(preds, labels):
         preds = [pred.strip() for pred in preds]
         labels = [[label.strip()] for label in labels]
 
         return preds, labels
 
-    metric = load_metric("sacrebleu")
+    metric = load_acft_metric("sacrebleu")
     preds, labels = eval_pred
     if isinstance(preds, tuple):
         preds = preds[0]
     decoded_preds = tokenizer.batch_decode(preds, skip_special_tokens=True)
 
     # Replace -100 in the labels as we can't decode them.
     labels = np.where(labels != TaskConstants.TRANSLATION_IGNORE_INDEX, labels, tokenizer.pad_token_id)
```

## azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/base.py

```diff
@@ -12,46 +12,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
-import json
 from pathlib import Path
-from argparse import Namespace
 
 from typing import Any, Callable, Dict, List, Optional, Union
 from dataclasses import dataclass, field
 
-import torch.nn as nn
+from ....constants.constants import (
+    AzuremlConstants,
+    MLFlowHFFlavourTasks,
+    PreprocessArgsTemplate,
+    TaskConstants,
+    Tasks,
+    STRING_DTYPES
+)
 
-from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
-from ....nlp_auto.config import AzuremlAutoConfig
-from ....constants.constants import DatasetSplit, SaveFileConstants, AzuremlConstants, MLFlowHFFlavourConstants, PreprocessArgsTemplate
-from ....constants.constants import Tasks, MLFlowHFFlavourTasks, STRING_DTYPES, TaskConstants
-from ....base_runner import BaseRunner
-
-from ....utils.data_utils import AzuremlDataset
+from ....utils.data_utils import AzuremlDataset, clean_column_name
 from ....utils.validation_utils import AzuremlValidatorMixin
 
-from datasets.arrow_dataset import Dataset
-from datasets import Sequence
-
-import transformers
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.data.data_collator import DataCollatorForSeq2Seq
-from transformers.hf_argparser import HfArgumentParser
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 @dataclass
 class TranslationPreprocessArgs(PreprocessArgsTemplate):
     # Specify the defaults for all new attributes of TranslationPreprocessArgs + inhertied attributes from
     # _PreprocessArgsTemplate here. Otherwise, there will be issues related to ordering of default and
     # non-default attributes
@@ -112,17 +107,19 @@
         self.placeholder_required_columns = ["source_lang", "target_lang"]
         self.placeholder_required_column_dtypes = [STRING_DTYPES, STRING_DTYPES]
         #
         if self.placeholder_required_columns is not None:
             for idx, col_name in enumerate(self.placeholder_required_columns):
                 decoded_arg = getattr(self, col_name, None)
                 if decoded_arg is not None:
-                    self.required_columns.append(decoded_arg)
+                    cleaned_name = clean_column_name(decoded_arg)
+                    setattr(self, col_name, cleaned_name)  # reset with cleaned name for further use
+                    self.required_columns.append(cleaned_name)
                     self.required_column_dtypes.append(self.placeholder_required_column_dtypes[idx])
-
+        self.validate_required_columns()
         self.label_column = getattr(self, self.placeholder_label_column)
 
 
 class TranslationDataset(AzuremlDataset, AzuremlValidatorMixin):
 
     def __init__(
         self,
@@ -258,29 +255,25 @@
             filter_lambda,
             batch_size=self.dataset_args["batch_size"],
             writer_batch_size=self.dataset_args["batch_size"]
         )
         post_filter_rows = self.dataset.num_rows
         logger.info(f"Translation data filter | before example count: {pre_filter_rows} | after example count: {post_filter_rows}")
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
                 )
             )
 
-    def validate(self):
+    def validate(self, split: Optional[str] = None):
+        self.apply_common_validations(split, batch_size=self.dataset_args["batch_size"])
 
-        # Remove the extra columns and match the remaining columns
-        self.remove_extra_columns()
-        self.match_columns()
-
-        # filter data
-        # null filter
-        self.remove_null_examples(batch_size=self.dataset_args["batch_size"])
+        # check if feature columns are identical
+        self.check_column_contents(self.dataset_args['source_lang'], self.dataset_args['target_lang'])
         # check dtypes
         # NOTE doing dtype check before task specific data filter because :meth translation_data_filter
         # assumes the dtypes for columns
         self.check_column_dtypes()
         # using ner specific filter
         self.translation_data_filter()
```

## azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_finetune.py

```diff
@@ -24,28 +24,20 @@
 import json
 
 from .base import TranslationPreprocessArgs, TranslationDataset
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 from ....nlp_auto.config import AzuremlAutoConfig
 from ....constants.constants import Tasks, HfModelTypes, DatasetSplit, SaveFileConstants, MLFlowHFFlavourConstants
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import (
-    TokenizerNotSupported,
-    InvalidLabel,
-    InvalidDataset,
-    BadArgument,
-)
-from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 T5_SOURCE_LANGUAGE_CODES = ["en"]
 T5_TARGET_LANGUAGE_CODES = ["fr", "de", "ro"]
 MBART_LANGUAGE_CODES = ["ar_AR", "cs_CZ", "de_DE", "en_XX", "es_XX", "et_EE", "fi_FI", "fr_XX", "gu_IN", "hi_IN", "it_IT", "ja_XX", "kk_KZ", "ko_KR", "lt_LT", "lv_LV", "my_MM", "ne_NP", "nl_XX", "ro_RO", "ru_RU", "si_LK", "tr_TR", "vi_VN", "zh_CN"]
 
 T5_CODE2LANG_MAP = {
@@ -61,18 +53,22 @@
     def __init__(self, component_args: Namespace, preprocess_args: TranslationPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
         #  - model_name arg from model selector
         #  - newly constructed model_name_or_path
         self.component_args = component_args
         self.preprocess_args = preprocess_args
+        self.ft_config = getattr(component_args, "finetune_config", {})
 
         logger.info(f"Task name: {Tasks.TRANSLATION}")
 
-        self.model_type = AzuremlAutoConfig.get_model_type(hf_model_name_or_path=component_args.model_name_or_path)
+        self.model_type = AzuremlAutoConfig.get_model_type(
+            hf_model_name_or_path=component_args.model_name_or_path,
+            **self.ft_config.get("load_config_kwargs", {}),
+        )
         if self.model_type == HfModelTypes.T5:
             if (
                 self.preprocess_args.source_lang not in T5_CODE2LANG_MAP or
                 self.preprocess_args.target_lang not in T5_CODE2LANG_MAP
             ):
                 raise ValueError(
                     "Either source or target language is not supported for T5. Supported languages are "
@@ -139,24 +135,27 @@
 
     def _init_tokenizer(self) -> PreTrainedTokenizerBase:
         """Initialize the tokenizer and set the model max length for the tokenizer if not already set"""
 
         tokenizer_params = {
             "task_name": Tasks.TRANSLATION,
             "apply_adjust": True,
-            "max_sequence_length": self.preprocess_args.max_seq_length
+            "max_sequence_length": self.preprocess_args.max_seq_length,
         }
         if self.model_type == HfModelTypes.MBART:
             tokenizer_params.update(
                 {
                     "src_lang": self.preprocess_args.source_lang,
-                    "tgt_lang": self.preprocess_args.target_lang
+                    "tgt_lang": self.preprocess_args.target_lang,
                 }
             )
 
+        tokenizer_params.update(self.ft_config.get("load_tokenizer_kwargs", {}))
+        tokenizer_params.update({"load_config_kwargs": self.ft_config.get("load_config_kwargs", {})})
+
         return AzuremlAutoTokenizer.from_pretrained(self.component_args.model_name_or_path, **tokenizer_params)
 
     def _get_encode_dataset_params(self) -> Dict[str, Any]:
 
         encode_params = {}
         # padding and truncation
         encode_params["padding"] = "max_length" if self.preprocess_args.pad_to_max_length else False
@@ -277,20 +276,20 @@
         if save_raw_data:
             return (raw_train_data_fname, raw_validation_data_fname, raw_test_data_fname)
 
     def _validate_data_splits(self):
         """validate the datasets"""
         # validate the datasets
         logger.info("Validating the train dataset")
-        self.train_ds.validate()
+        self.train_ds.validate(DatasetSplit.TRAIN)
         logger.info("Validating the validation dataset")
-        self.valid_ds.validate()
+        self.valid_ds.validate(DatasetSplit.VALIDATION)
         if not self.component_args.skip_test_data_processing and self.test_ds is not None:
             logger.info("Validating the test dataset")
-            self.test_ds.validate()
+            self.test_ds.validate(DatasetSplit.TEST)
 
     def _encode_data_splits(self):
         """
         Encode the dataset
         """
         logger.info("Encoding the train dataset")
         self.train_ds.encode_dataset()
```

## azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_inference.py

```diff
@@ -22,19 +22,19 @@
 
 from argparse import Namespace
 
 from .base import NerPreprocessArgs
 from ....constants.constants import Tasks
 from ....nlp_auto.tokenizer import AzuremlAutoTokenizer
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from azureml.acft.common_components import get_logger_app
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class NerPreprocessForInfer():
 
     def __init__(self, component_args: Namespace, preprocess_args: NerPreprocessArgs) -> None:
         # component args is combined args of
         #  - preprocess component args
```

## azureml/acft/contrib/hf/nlp/utils/data_utils.py

```diff
@@ -15,36 +15,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """
 data utils
 """
-
 from pathlib import Path
 from typing import Optional, List, Union, Dict, Tuple, Any
 import shutil
 import mltable
 
 from abc import ABC, abstractmethod
-
 from datasets.load import load_dataset
 from datasets import Sequence, Value, ClassLabel
 from datasets.arrow_dataset import Dataset
+from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import PathNotFound, ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException, ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import PathNotFound, ACFTUserError
+from azureml._common._error_definition.user_error import BadData
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
-from ..constants.constants import AzuremlConstants
-from .preprocess_utils import get_new_file_name, txt_to_jsonl
+from ..constants.constants import AzuremlConstants, DataSliceConstants
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class AzuremlDataset(ABC):
     """
     All the logic related to data can be a part of this class or the subclass inheriting this
     1. loading and saving the dataset
     2. data wrangling
@@ -58,15 +57,15 @@
     VALID_DATA_FORMATS_ERROR_STRING = f"Data format not supported. Supported formats are {VALID_DATA_FORMATS}"
 
     def __init__(
         self,
         path_or_dict: Union[str, Path, Dict],
         label_column: Optional[str] = None,
         label_column_optional: bool = False,
-        slice: str = "train",
+        slice: str = DataSliceConstants.NO_SPLIT,
     ) -> None:
         """
         :param label_column
             The column in self.dataset to be used as label_column. Setting this value to None makes some of
             the attributes / methods invalid
                 :attr `class_names` calculates the class_names of the label_column
                 :method `convert_label_column_using_classlabel` converts the label column to `dataset.ClassLabel`
@@ -90,87 +89,160 @@
         self.label_column_optional = label_column_optional
 
         self.slice = slice
 
         # load the dataset
         self.dataset = self.load(self.slice)
 
-    def load(self, slice: str = "train") -> Dataset:
+    def load(self, slice: str = DataSliceConstants.NO_SPLIT) -> Dataset:
         """
         1. Loads the dataset
         2. kwargs
             data_format - json, csv, mltable
             dataset_type - could be dataset or torch
             sample_size
                 0.1 - 1.0 percentage of data to load
                 1 - len(dataset) number of samples to load
         3. Handle loading dataset from S3 URI, Azure blob store
         """
 
+        def _load_mltable(path_or_dict: str) -> Dataset:
+            """
+            Load mltable from any of the permissible input port.
+            """
+            try:
+                data_tbl = mltable.load(path_or_dict)
+                df = data_tbl.to_pandas_dataframe()
+                ds = Dataset.from_pandas(df)
+                logger.info(f"Dataset loaded with examples = {ds.num_rows}")
+                return ds
+            except Exception as e:
+                raise ACFTDataException._with_error(
+                            AzureMLError.create(
+                                ACFTUserError,
+                                pii_safe_message=f"Error while loading the dataset: {e}"
+                            )
+                        )
+
         logger.info(f"Loading dataset with slice : {slice}")
         if isinstance(self.path_or_dict, str):
             # check if file exists
             if Path(self.path_or_dict).is_file():
                 # check if the file format is supported
                 file_format = self._get_file_format(self.path_or_dict)
                 if file_format:
                     data_file_extension, dataset_kwargs = self._get_dataset_format(file_format)
                     try:
                         ds = load_dataset(data_file_extension, data_files=self.path_or_dict, split=slice, **dataset_kwargs)
                         logger.info(f"Dataset loaded with examples = {ds.num_rows}")
                     except Exception as e:
-                        raise ValidationException._with_error(
+                        raise ACFTDataException._with_error(
                             AzureMLError.create(
-                                ValidationError,
-                                error=f"Error while loading the dataset: {e}"
+                                ACFTUserError,
+                                pii_safe_message=(
+                                    f"Error while loading the dataset: {e} \n "
+                                    "Please validate your data by launching run through notebooks at "
+                                    "https://github.com/Azure/azureml-examples/tree/main/sdk/python/"
+                                    "foundation-models/system/finetune \n"
+                                    "or alternately try loading each of your data file using the following"
+                                    " code snippet \n"
+                                    "```\nfrom datasets.load import load_dataset\n"
+                                    f"ds = load_dataset('{data_file_extension}', data_files='path_to_file',"
+                                    f"split='train', **{dataset_kwargs})\n```"
+                                )
                             )
                         )
-
+                    # clean datset column names
+                    ds = self._clean_dataset_columns(ds)
                     return ds
                 else:
-                    raise ValueError(AzuremlDataset.VALID_DATA_FORMATS_ERROR_STRING)
+                    raise ACFTValidationException._with_error(
+                        AzureMLError.create(
+                            BadData,
+                            data_argument_name=AzuremlDataset.VALID_DATA_FORMATS_ERROR_STRING
+                        )
+                    )
+
+            elif self.path_or_dict.lower().startswith(AzuremlConstants.AZUREML_URL_PREFIX):
+                # check if input is MLTable with input port as Direct and load it
+                try:
+                    logger.info("Azureml url detected in input. Trying to load it as mltable.")
+                    ds = _load_mltable(self.path_or_dict)
+                except Exception as e:
+                    raise ACFTDataException._with_error(
+                        AzureMLError.create(
+                            ACFTUserError,
+                            pii_safe_message=f"Currently input port=Direct is supported for mltable input only: {e}"
+                        )
+                    )
 
+                ds = self._get_dataset_slice(ds, slice)
+                # clean datset column names
+                ds = self._clean_dataset_columns(ds)
+                return ds
             elif Path(self.path_or_dict).is_dir():
-                # check if valid MLTable and load it
+                # check if input is MLTable with input port as RO_Mount and load it
                 directory_format = self._get_directory_format(self.path_or_dict)
                 logger.info(directory_format)
                 if directory_format:
                     if directory_format == "mltable":
-                        data_tbl = mltable.load(self.path_or_dict)
-                        df = data_tbl.to_pandas_dataframe()
-                        ds = Dataset.from_pandas(df)
-                        logger.info(f"Dataset loaded with examples = {ds.num_rows}")
+                        ds = _load_mltable(self.path_or_dict)
                         ds = self._get_dataset_slice(ds, slice)
+                        # clean datset column names
+                        ds = self._clean_dataset_columns(ds)
                         return ds
                     else:
-                        raise ValueError(AzuremlDataset.VALID_DATA_FORMATS_ERROR_STRING)
+                        raise ACFTValidationException._with_error(
+                            AzureMLError.create(
+                                BadData,
+                                data_argument_name=AzuremlDataset.VALID_DATA_FORMATS_ERROR_STRING
+                            )
+                        )
                 else:
-                    raise ValueError(AzuremlDataset.VALID_DATA_FORMATS_ERROR_STRING)
+                    raise ACFTValidationException._with_error(
+                        AzureMLError.create(
+                            BadData,
+                            data_argument_name=AzuremlDataset.VALID_DATA_FORMATS_ERROR_STRING
+                        )
+                    )
             else:
-                raise ValidationException._with_error(AzureMLError.create(PathNotFound, path=self.path_or_dict))
+                raise ACFTValidationException._with_error(AzureMLError.create(PathNotFound, path=self.path_or_dict))
 
         elif isinstance(self.path_or_dict, Dict):
             # TODO add logic to load data from dictionary
             ds = Dataset.from_dict(self.path_or_dict)
             logger.info(f"Dataset loaded with examples = {ds.num_rows}")
             ds = self._get_dataset_slice(ds, slice)
+            # clean datset column names
+            ds = self._clean_dataset_columns(ds)
             return ds
 
-        raise ValidationException._with_error(AzureMLError.create(PathNotFound, path=self.path_or_dict))
-    
-    def _get_dataset_slice(self, ds: Dataset, slice: str = "train") -> Dataset:
+        raise ACFTValidationException._with_error(AzureMLError.create(PathNotFound, path=self.path_or_dict))
+
+    def _clean_dataset_columns(self, ds: Dataset) -> Dataset:
+        column_mapping = {}
+        for column in ds.column_names:
+            cleaned_column = clean_column_name(column)
+            if cleaned_column != column:
+                column_mapping[column] = cleaned_column
+        if column_mapping:
+            logger.info(f"Cleaning column names: {column_mapping}")
+            ds = ds.rename_columns(column_mapping)
+        return ds
+
+    def _get_dataset_slice(self, ds: Dataset, slice: str = DataSliceConstants.NO_SPLIT) -> Dataset:
         """
         returns slice of dataset
         `slice`: The below format is followed as load_dataset() supports it.
         e.g.: slice="train[:50%]"
               slice="train[50%:75%]"
               slice="train[-25%:]"
         If slice == "train" the original dataset is returned
         """
-        if not slice or slice == "train":
+        if not slice or slice == DataSliceConstants.NO_SPLIT:
             return ds
         
         num_rows = ds.num_rows
         try:
             slice_ratio = slice[len("train["): -1]
             x, y = slice_ratio.split(":")
             if len(x) > 0 and x[-1] == "%":
@@ -185,24 +257,27 @@
             y = int((y/100) * num_rows)
             logger.info(f"Splicing data indexes from {x} to {y}")
             ds_new = Dataset.from_dict(ds[x:y])
             logger.info(f"Dataset after slice is with examples = {ds_new.num_rows}")
             return ds_new
         except:
             logger.warning("Unable to slice dataset")
-        
+
         return ds
 
     def _get_file_format(self, path: str) -> Union[str, None]:
         """identify valid file format"""
         file_extension = Path(path).suffix
         file_format = file_extension.lstrip(".")
         self.data_format = file_format
         if file_format not in AzuremlDataset.VALID_FILE_FORMATS:
             file_extension = None
+
+        logger.info(f'Identified file format: "{file_extension}"')
+
         return file_extension
 
     def _get_dataset_format(self, file_format: str) -> Tuple[str, Dict[str, Any]]:
         """find data file extension and respective dataset loading kwargs"""
         dataset_kwargs = {}
         if file_format == ".jsonl":
             data_file_extension = "json"
@@ -211,36 +286,32 @@
         elif file_format == ".csv":
             data_file_extension = "csv"
         elif file_format == ".tsv":
             data_file_extension = "csv"
             dataset_kwargs["sep"] = "\t"
         elif file_format == ".parquet":
             data_file_extension = "parquet"
-        elif file_format == ".txt":
-            data_file_extension = "json"
-            new_file_name = get_new_file_name(self.path_or_dict, "txt", "jsonl")
-            txt_to_jsonl(self.path_or_dict, new_file_name)
-            self.path_or_dict = new_file_name
         else:
             data_file_extension = None
 
         return data_file_extension, dataset_kwargs  # type: ignore
 
     def _get_directory_format(self, path: str) -> Union[str, None]:
         """identify valid directory format"""
         data_format = None
         directory_path = Path(path)
         mltable_file_path = Path.joinpath(directory_path, "MLTable")
-        logger.info(f"{mltable_file_path.is_file()}, {str(mltable_file_path)}")
         if mltable_file_path.is_file():
             # currently only supported format is MLTable
             data_format = "mltable"
         if data_format not in AzuremlDataset.VALID_DIRECTORY_FORMATS:
             data_format = None
         self.data_format = data_format
+        logger.info(f'Identified directory format: "{data_format}"')
+
         return data_format
 
     @property
     def class_names(self) -> Optional[List[str]]:
 
         # Return the precomputed class names saved in a private variable
         if hasattr(self, "_class_names"):
@@ -340,14 +411,15 @@
     def get_collation_function(self) -> None:
         """
         used for data collation during training. The default behaviour is implemented here
         None => no dynamic padding happens during training
         """
         return None
 
+
     @abstractmethod
     def encode_dataset(self) -> None:
         """
         tokenize the dataset which is task dependent and needs to be implemented by the subclass
         """
         pass
 
@@ -355,7 +427,11 @@
 def copy_and_overwrite(from_path: str, to_path: str):
     """
     copy and overwrites the directory
     """
     if Path(to_path).is_dir():
         shutil.rmtree(to_path)
     shutil.copytree(from_path, to_path)
+
+
+def clean_column_name(column_name: str) -> str:
+    return column_name.strip()
```

## azureml/acft/contrib/hf/nlp/utils/hf_argparser.py

```diff
@@ -25,15 +25,17 @@
 import sys
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, ArgumentTypeError
 from copy import copy
 from enum import Enum
 from inspect import isclass
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, NewType, Optional, Tuple, Union, get_type_hints
-
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError, ACFTSystemError
+from azureml._common._error_definition.azureml_error import AzureMLError
 import yaml
 
 
 try:
     # For Python versions <3.8, Literal is not in typing: https://peps.python.org/pep-0586/
     from typing import Literal
 except ImportError:
@@ -50,16 +52,21 @@
     if isinstance(v, bool):
         return v
     if v.lower() in ("yes", "true", "t", "y", "1"):
         return True
     elif v.lower() in ("no", "false", "f", "n", "0"):
         return False
     else:
-        raise ArgumentTypeError(
-            f"Truthy value expected: got {v} but expected one of yes/no, true/false, t/f, y/n, 1/0 (case insensitive)."
+        raise ACFTValidationException._with_error(
+            AzureMLError.create(
+                ACFTUserError,
+                pii_safe_message=(
+                    "Truthy value expected: got {v} but expected one of yes/no, true/false, t/f, y/n, 1/0 (case insensitive)."
+                )
+            )
         )
 
 
 def make_choice_type_function(choices: list) -> Callable[[str], Any]:
     """
     Creates a mapping function from each choices string representation to the actual value. Used to support multiple
     value types for a single argument.
@@ -153,33 +160,44 @@
     @staticmethod
     def _parse_dataclass_field(parser: ArgumentParser, field: dataclasses.Field):
         field_name = f"--{field.name}"
         kwargs = field.metadata.copy()
         # field.metadata is not used at all by Data Classes,
         # it is provided as a third-party extension mechanism.
         if isinstance(field.type, str):
-            raise RuntimeError(
-                "Unresolved type detected, which should have been done with the help of "
-                "`typing.get_type_hints` method by default"
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(
+                    ACFTSystemError,
+                    pii_safe_message=(
+                        "Unresolved type detected, which should have been done with the help of "
+                        "`typing.get_type_hints` method by default"
+                    )
+                )
             )
 
         aliases = kwargs.pop("aliases", [])
         if isinstance(aliases, str):
             aliases = [aliases]
 
         origin_type = getattr(field.type, "__origin__", field.type)
         if origin_type is Union:
             if str not in field.type.__args__ and (
                 len(field.type.__args__) != 2 or type(None) not in field.type.__args__
             ):
-                raise ValueError(
-                    "Only `Union[X, NoneType]` (i.e., `Optional[X]`) is allowed for `Union` because"
-                    " the argument parser only supports one type per argument."
-                    f" Problem encountered in field '{field.name}'."
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(
+                        ACFTSystemError,
+                        pii_safe_message=(
+                            "Only `Union[X, NoneType]` (i.e., `Optional[X]`) is allowed for `Union` because"
+                            " the argument parser only supports one type per argument."
+                            f" Problem encountered in field '{field.name}'."
+                        )
+                    )
                 )
+                
             if type(None) not in field.type.__args__:
                 # filter `str` in Union
                 field.type = field.type.__args__[0] if field.type.__args__[1] == str else field.type.__args__[1]
                 origin_type = getattr(field.type, "__origin__", field.type)
             elif bool not in field.type.__args__:
                 # filter `NoneType` in Union (except for `Union[bool, NoneType]`)
                 field.type = (
@@ -248,18 +266,23 @@
             parser = self.add_argument_group(dtype._argument_group_name)
         else:
             parser = self
 
         try:
             type_hints: Dict[str, type] = get_type_hints(dtype)
         except NameError:
-            raise RuntimeError(
-                f"Type resolution failed for f{dtype}. Try declaring the class in global scope or "
-                "removing line of `from __future__ import annotations` which opts in Postponed "
-                "Evaluation of Annotations (PEP 563)"
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(
+                    ACFTSystemError,
+                    pii_safe_message=(
+                        f"Type resolution failed for f{dtype}. Try declaring the class in global scope or "
+                        "removing line of `from __future__ import annotations` which opts in Postponed "
+                        "Evaluation of Annotations (PEP 563)"
+                    )
+                )
             )
 
         for field in dataclasses.fields(dtype):
             if not field.init:
                 continue
             field.type = type_hints[field.name]
             self._parse_dataclass_field(parser, field)
@@ -342,15 +365,22 @@
         if len(namespace.__dict__) > 0:
             # additional namespace.
             outputs.append(namespace)
         if return_remaining_strings:
             return (*outputs, remaining_args)
         else:
             if remaining_args:
-                raise ValueError(f"Some specified arguments are not used by the HfArgumentParser: {remaining_args}")
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(
+                        ACFTUserError,
+                        pii_safe_message=(
+                            f"Some specified arguments are not used by the HfArgumentParser: {remaining_args}"
+                        )
+                    )
+                )
 
             return (*outputs,)
 
     def parse_dict(self, args: Dict[str, Any], allow_extra_keys: bool = False) -> Tuple[DataClass, ...]:
         """
         Alternative helper method that does not use `argparse` at all, instead uses a dict and populating the dataclass
         types.
@@ -368,18 +398,35 @@
         """
         unused_keys = set(args.keys())
         outputs = []
         for dtype in self.dataclass_types:
             keys = {f.name for f in dataclasses.fields(dtype) if f.init}
             inputs = {k: v for k, v in args.items() if k in keys}
             unused_keys.difference_update(inputs.keys())
-            obj = dtype(**inputs)
+            try: 
+                obj = dtype(**inputs)
+            except TypeError as e:
+                raise ACFTValidationException._with_error(
+                    AzureMLError.create(
+                        ACFTUserError,
+                        pii_safe_message=(
+                            "Invalid config file. Error when creating {dtype} while parsing argument:\n{e}"
+                        )
+                    )
+                )
             outputs.append(obj)
         if not allow_extra_keys and unused_keys:
-            raise ValueError(f"Some keys are not used by the HfArgumentParser: {sorted(unused_keys)}")
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(
+                    ACFTUserError,
+                    pii_safe_message=(
+                        f"Some keys are not used by the HfArgumentParser: {sorted(unused_keys)}"
+                    )
+                )
+            )
         return tuple(outputs)
 
     def parse_json_file(self, json_file: str, allow_extra_keys: bool = False) -> Tuple[DataClass, ...]:
         """
         Alternative helper method that does not use `argparse` at all, instead loading a json file and populating the
         dataclass types.
```

## azureml/acft/contrib/hf/nlp/utils/mlflow_utils.py

```diff
@@ -14,143 +14,220 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 """
 mlflow utilities
 """
-from pathlib import Path
 import json
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Tuple
 import shutil
-
+import yaml
 from pathlib import Path
+from mlflow.models import Model
+
+from ..constants.constants import MLFlowHFFlavourConstants, MLFLOW_FLAVORS
+from .common_utils import deep_update
+from .io_utils import find_files_with_inc_excl_pattern
 
-from ..constants.constants import MLFlowHFFlavourConstants
+from peft import PeftModel
 
 from transformers import TrainerCallback, TrainingArguments, TrainerState, TrainerControl
-from transformers import PreTrainedModel
+from transformers import PreTrainedModel, PreTrainedTokenizerBase
+from transformers import pipeline
 from transformers.utils import (
     WEIGHTS_INDEX_NAME,
     SAFE_WEIGHTS_INDEX_NAME,
     WEIGHTS_NAME,
     SAFE_WEIGHTS_NAME
 )
+from transformers.deepspeed import is_deepspeed_zero3_enabled
+
+import torch
 
 from torch_ort import ORTModule
 
 from azureml._common._error_definition.azureml_error import AzureMLError
-from azureml.acft.accelerator.utils.error_handling.exceptions import LLMException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import LLMInternalError
+
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTSystemException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTSystemError
+from azureml.acft.common_components import get_logger_app
+
 from azureml.acft.accelerator.utils.license_utils import download_license_file
+from azureml.acft.accelerator.utils.code_utils import get_model_custom_code_files, copy_code_files
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-import azureml.evaluate.mlflow as mlflow
+import azureml.evaluate.mlflow as hf_mlflow
+import mlflow
 
-from .mlflow_preprocess import prepare_mlflow_preprocess, restructure_mlflow_acft_code
 
+logger = get_logger_app(__name__)
 
-logger = get_logger_app()
 
+def replace_mlflow_weights_with_pytorch_weights_zero3(pytorch_model_save_path: str, mlflow_model_save_path: str):
+    """The mlflow.save saves the dummy model weights when deepspeed stage3 optimization is enabled. This is because
+    in evaluation model is saved using ModelClass.save_pretrained to save the model. The save_pretrained method
+    fetches the state dictionary using model.state_dict which is dummy when stage3 is enabled.To circumvent this
+    behavior, we are copying the PyTorch model weights to MlFlow folder.
 
-def replace_deepspeed_zero3_mlflow_pytorch_weights(pytorch_model_save_path: str, mlflow_model_save_path: str):
-    """
-    Case1
-        finetune [nlp contrib] -> AzuremlTrainer.train() [callbacks] -> merge lora weights -> final PyTorch model
-        During the mlflow callback, the merged model is not accessible to the model.
-        LoRA weights needs to be updated after merging
-    Case2
-        When deep speed stage3 optimizer is enabled, the model is a dummy object. Hence, the mlflow weights are replaced
-        with the PyTorch weights which has decoded weights
+    :param pytorch_model_save_path: Folder where the PyTorch weights are saved. The weights saved in this
+        folder are final weights and the model should be able to load using AutoModelFor<TaskName>.from_pretrained(...)
+    :type: str
+    :param mlflow_model_save_path: Output folder where the MlFlow weights are saved. The weights in this folder gets
+    updated
+    :type: str
     """
-    # copy the checkpoint files when deepspeed zero3 is enabled as the model object is a dummy model
     dst_folder = Path(mlflow_model_save_path, "data", "model")
 
+    # Copy the PyTorch artifacts -> mlflow
     index_file = Path(pytorch_model_save_path, WEIGHTS_INDEX_NAME)
     safe_index_file = Path(pytorch_model_save_path, SAFE_WEIGHTS_INDEX_NAME)
     weights_file = Path(pytorch_model_save_path, WEIGHTS_NAME)
     safe_weights_file = Path(pytorch_model_save_path, SAFE_WEIGHTS_NAME)
 
-    # remove the existing dummy file if any
-    if index_file.exists() or safe_index_file.exists():
-        if weights_file.exists():
-            weights_file.unlink()
-        elif safe_weights_file.exists():
-            safe_weights_file.unlink()
+    # Clean the directory for already created dummy files
+    # Identify all the model artifacts files
+    dummy_model_artifacts_file_paths = find_files_with_inc_excl_pattern(
+        str(dst_folder),
+        include_pat=".bin$|.safetensors$|" + f"{str(safe_index_file)}|{str(index_file)}"
+    )
+    logger.info("Removing the dummy files created with mlflow.save")
+    for file_name in dummy_model_artifacts_file_paths:
+        logger.info(f"Removing {file_name}")
+        Path(file_name).unlink()
 
+    if index_file.exists() or safe_index_file.exists():
+        logger.info("Copying the index file + shards to MlFlow model folder")
         # copy the sharded files to mlflow model artifacts
         load_index_file = index_file if index_file.exists() else safe_index_file
         with open(load_index_file, "r", encoding="utf-8") as f:
             index = json.load(f)
-        shard_files = list(set(index["weight_map"].values()))
-        shard_files += str(load_index_file)
+        shard_files = [str(Path(pytorch_model_save_path, x)) for x in list(set(index["weight_map"].values()))]
+        shard_files.append(str(load_index_file))    # already has pytorch_model_save_path as prefix
         for shard_file in shard_files:
+            logger.info(f"Copy started for {shard_file}")
             shutil.copy(shard_file, str(dst_folder))
+    elif weights_file.exists() or safe_weights_file.exists():
+        # copy the file to mlflow model artifacts
+        existing_weights_file = weights_file if weights_file.exists() else safe_weights_file
+        logger.info(f"Copy started for {existing_weights_file}")
+        shutil.copy(str(existing_weights_file), str(dst_folder))
     else:
-        if weights_file.exists() or safe_weights_file.exists():
-            # copy the file to mlflow model artifacts
-            existing_weights_file = weights_file if weights_file.exists() else safe_weights_file
-            shutil.copy(str(existing_weights_file), str(dst_folder))
-        else:
-            raise LLMException._with_error(
-                AzureMLError.create(
-                    LLMInternalError,
-                    error=("PyTorch -> MLFlow model conversion failed with DS Stage3 optimizer")
-                )
+        raise ACFTSystemException._with_error(
+            AzureMLError.create(
+                ACFTSystemError,
+                pii_safe_message=("Unable to replace dummy MlFlow weights with PyTorch weights with DS-Zero3 optimizer")
             )
+        )
 
 
 class SaveMLflowModelCallback(TrainerCallback):
     """
     A [`TrainerCallback`] that sends the logs to [AzureML](https://pypi.org/project/azureml-sdk/).
     """
 
     def __init__(
         self,
         mlflow_model_save_path: Union[str, Path],
+        pytorch_model_save_path: Optional[Union[str, Path]],
         mlflow_infer_params_file_path: Union[str, Path],
         mlflow_task_type: str,
         model_name: str,
         model_name_or_path: Optional[str] = None,
         class_names: Optional[List[str]] = None,
+        metadata: str = None,
         **kwargs
     ) -> None:
         """
         init azureml_run which is azureml Run object
         """
         self.mlflow_model_save_path = mlflow_model_save_path
+
+        # Use pytorch save folder to load the model. This is set in case of LoRA where the base model is wrapped to add
+        # lora weights
+        self.pytorch_model_save_path = pytorch_model_save_path
+        if self.pytorch_model_save_path is not None:
+            logger.info(
+                f"Will use pytorch folder - {pytorch_model_save_path} while saving the mlflow model")
+
         self.mlflow_infer_params_file_path = mlflow_infer_params_file_path
         self.mlflow_task_type = mlflow_task_type
         self.class_names = class_names
         self.model_name = model_name
         self.model_name_or_path = model_name_or_path
+        self.mlflow_hf_args = kwargs.get("mlflow_hf_args", {})
+        self.mlflow_ft_conf = kwargs.get("mlflow_ft_conf", {})
+        self.mlflow_hftransformers_misc_conf = self.mlflow_ft_conf.get("mlflow_hftransformers_misc_conf", {})
+        self.mlflow_model_signature = self.mlflow_ft_conf.get("mlflow_model_signature", None)
+        self.mlflow_save_model_kwargs = self.mlflow_ft_conf.get("mlflow_save_model_kwargs", {})
+        self.metadata = metadata
+        self.mlflow_flavor = self.mlflow_ft_conf.get("mlflow_flavor", None)
+
+    def load_model_tokenizer(self, **kwargs) -> Tuple[PreTrainedModel, PreTrainedTokenizerBase]:
+
+        model, tokenizer = kwargs["model"], kwargs["tokenizer"]
+
+        reload_model = True
+        if self.pytorch_model_save_path is None:
+            reload_model = False
+        elif is_deepspeed_zero3_enabled() and isinstance(model, PeftModel):
+            # do not try to load peft model again if it is deepspeed stage-3
+            reload_model = False
+
+        if reload_model:
+
+            base_model_cls = model.__class__
+            if isinstance(model, PeftModel):
+                base_model_cls = model.base_model.model.__class__
+            logger.info(f"Base model class to load the model before mlflow model save: {base_model_cls}")
+
+            model = base_model_cls.from_pretrained(
+                self.pytorch_model_save_path,
+                low_cpu_mem_usage=True,
+                torch_dtype="auto"
+            )
+            tokenizer = tokenizer.__class__.from_pretrained(self.pytorch_model_save_path)
+
+        return model, tokenizer
 
     def on_train_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
         """
         Event called at the end of training.
         Save MLflow model at the end of training
 
         Model and Tokenizer information is part of kwargs
         """
 
-        model, tokenizer = kwargs["model"], kwargs["tokenizer"]
-
         # saving the mlflow on world process 0
         if state.is_world_process_zero:
+
+            model, tokenizer = self.load_model_tokenizer(**kwargs)
+
             # tokenization parameters for inference
             # task related parameters
             with open(self.mlflow_infer_params_file_path, 'r') as fp:
                 mlflow_inference_params = json.load(fp)
 
             misc_conf = {
                 MLFlowHFFlavourConstants.TASK_TYPE: self.mlflow_task_type,
                 MLFlowHFFlavourConstants.TRAIN_LABEL_LIST: self.class_names,
-                MLFlowHFFlavourConstants.HUGGINGFACE_ID: self.model_name,
                 **mlflow_inference_params,
             }
+
+            # if a huggingface_id was passed, save it to MLModel file, otherwise not
+            if self.model_name != MLFlowHFFlavourConstants.DEFAULT_MODEL_NAME:
+                misc_conf.update({MLFlowHFFlavourConstants.HUGGINGFACE_ID: self.model_name})
+
+            # auto classes need to be passed in misc_conf if custom code files are present in the model folder
+            if hasattr(model.config, "auto_map"):
+                misc_conf.update(self.mlflow_hf_args)
+                logger.info(f"Updated misc conf with Auto classes - {misc_conf}")
+
+            logger.info(f"Adding additional misc to MLModel - {self.mlflow_hftransformers_misc_conf}")
+            misc_conf = deep_update(misc_conf, self.mlflow_hftransformers_misc_conf)
+
             # files_list = prepare_mlflow_preprocess()
             # model_artifact_path = "llm_multiclass_model"
             # conda_env = {
             #     'channels': ['conda-forge'],
             #     'dependencies': [
             #         'python=3.8.8',
             #         'pip',
@@ -162,28 +239,108 @@
             #     ],
             #     'name': 'mlflow-env'
             # }
             if isinstance(model, PreTrainedModel):
                 acft_model = model
             elif isinstance(model, ORTModule) and hasattr(model, "module"):
                 acft_model = model.module
+            elif is_deepspeed_zero3_enabled() and isinstance(model, PeftModel) and hasattr(model, "base_model"):
+                # save dummy model in-case of peft deepspeed stage-3 model
+                acft_model = model.base_model
             else:
-                raise LLMException._with_error(
-                    AzureMLError.create(LLMInternalError, error=(
+                raise ACFTSystemException._with_error(
+                    AzureMLError.create(ACFTSystemError, pii_safe_message=(
                         f"Got unexpected model - {model}"
                     ))
                 )
-            mlflow.hftransformers.save_model(
-                acft_model, self.mlflow_model_save_path, tokenizer, model.config, misc_conf,)
-            # code_paths=files_list, artifact_path=model_artifact_path, conda_env=conda_env,)
-            # restructure_mlflow_acft_code(self.mlflow_model_save_path)
+
+            # Check if any code files are present in the model folder
+            py_code_files = get_model_custom_code_files(self.model_name_or_path, model)
+
+            # Save Model depending on flavor
+            if self.mlflow_flavor == MLFLOW_FLAVORS.TRANSFORMERS:
+                self.save_oss_flavor_mlflow_model(model=acft_model, tokenizer=tokenizer, py_code_files=py_code_files)
+            else:
+                # save hftransformers or hftransformers model
+                self.save_hftransformers_mlflow_model(model=acft_model, tokenizer=tokenizer, misc_conf=misc_conf, py_code_files=py_code_files)
 
             # save LICENSE file to MlFlow model
             if self.model_name_or_path:
                 license_file_path = Path(self.model_name_or_path, MLFlowHFFlavourConstants.LICENSE_FILE)
                 if license_file_path.is_file():
                     shutil.copy(str(license_file_path), self.mlflow_model_save_path)
                     logger.info("LICENSE file is copied to mlflow model folder")
                 else:
                     download_license_file(self.model_name, str(self.mlflow_model_save_path))
 
+            # setting mlflow model signature for inference
+            if self.mlflow_model_signature is not None:
+                logger.info(f"Adding mlflow model signature - {self.mlflow_model_signature}")
+                mlflow_model_file = Path(self.mlflow_model_save_path, MLFlowHFFlavourConstants.MISC_CONFIG_FILE)
+                if mlflow_model_file.is_file():
+                    mlflow_model_data = {}
+                    with open(str(mlflow_model_file), "r") as fp:
+                        yaml_data = yaml.safe_load(fp)
+                        mlflow_model_data.update(yaml_data)
+                        mlflow_model_data["signature"] = self.mlflow_model_signature
+
+                    with open(str(mlflow_model_file), "w") as fp:
+                        yaml.dump(mlflow_model_data, fp)
+                        logger.info(f"Updated mlflow model file with 'signature': {self.mlflow_model_signature}")
+                else:
+                    logger.info("No MLmodel file to update signature")
+            else:
+                logger.info("No signature will be added to mlflow model")
+
             logger.info("Saved as mlflow model at {}".format(self.mlflow_model_save_path))
+
+
+    def save_oss_flavor_mlflow_model(self, model, tokenizer, py_code_files):
+        """
+        Saves the finetuned model with transformers mlflow flavor
+        """
+        logger.info(f"Trying Saving Finetuned Model with FLAVOR : {self.mlflow_flavor}")
+        model_pipeline = pipeline(task=self.mlflow_task_type, model=model, tokenizer=tokenizer, config=model.config)
+        mlflow.transformers.save_model(
+            transformers_model=model_pipeline,
+            path=self.mlflow_model_save_path,
+            code_paths=py_code_files,
+            conda_env=str(Path(str(self.model_name_or_path), MLFlowHFFlavourConstants.CONDA_YAML_FILE)),
+            metadata=self.metadata,
+            **self.mlflow_save_model_kwargs,
+        )
+        logger.info(f"Saved Finetuned Model with FLAVOR : {self.mlflow_flavor}")
+        copy_code_files(
+            py_code_files,
+            [str(Path(self.mlflow_model_save_path, dir)) for dir in ['model', Path("components", "tokenizer")]]
+        )
+
+
+    def save_hftransformers_mlflow_model(self, model, tokenizer, misc_conf, py_code_files):
+        """
+        Saves the finetuned model with hftransformers/hftransfomersv2 mlflow flavor
+        """
+        logger.info(f"Trying Saving Finetuned Model with FLAVOR : {self.mlflow_flavor}")
+        # passing metadata through mlflow.models.Model api will dump the metadata
+        # inline with the pyfunc at the parent level of the MLmodel yaml
+        mlflow_model = Model(metadata=self.metadata)
+        hf_mlflow.hftransformers.save_model(
+            model,
+            self.mlflow_model_save_path,
+            tokenizer,
+            model.config,
+            misc_conf,
+            code_paths=py_code_files,
+            mlflow_model=mlflow_model,
+            **self.mlflow_save_model_kwargs,
+        )
+        logger.info(f"Saved Finetuned Model with FLAVOR : {self.mlflow_flavor}")
+
+        # code_paths=files_list, artifact_path=model_artifact_path, conda_env=conda_env,)
+        # restructure_mlflow_acft_code(self.mlflow_model_save_path)
+
+        # copying the py files to mlflow destination
+        # copy dynamic python files to config, model and tokenizer
+        copy_code_files(
+            py_code_files,
+            [str(Path(self.mlflow_model_save_path, 'data', dir)) for dir in ['config', 'model', 'tokenizer']]
+        )
```

## azureml/acft/contrib/hf/nlp/utils/model_selector_utils.py

```diff
@@ -15,141 +15,207 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 """
 model selector utils
 """
 
-import os
 from pathlib import Path
 from typing import Dict, Any, Union
 import shutil
 import yaml
 import json
 
-from ..constants.constants import SaveFileConstants, MLFlowHFFlavourConstants
+from ..constants.constants import SaveFileConstants, MLFlowHFFlavourConstants, MLFLOW_FLAVORS
+from .io_utils import read_json_file
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import LLMException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import LLMInternalError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTSystemException, ACFTValidationException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTSystemError, ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 MODEL_REGISTRY_NAME = "azureml-preview"
 
+# flavor map to fallback to hftransformers
+FLAVOR_MAP_FOR_FALLBACK = {
+    MLFLOW_FLAVORS.HFTRANSFORMERSV2: {
+        "tokenizer": "data/tokenizer",
+        "model": "data/model",
+        "config": "data/config"
+    },
+    MLFLOW_FLAVORS.HFTRANSFORMERS: {
+        "tokenizer": "data/tokenizer",
+        "model": "data/model",
+        "config": "data/config"
+    }
+}
 
-def get_model_name_from_pytorch_model(model_path: str) -> str:
-    """
-    Fetch model_name information from pytorch model metadata file
-    """
-    finetune_args_file = Path(model_path, SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
 
-    # load the metadata file
+def _load_mlflow_model(model_path: str) -> str:
+    mlflow_config_file = Path(model_path, MLFlowHFFlavourConstants.MISC_CONFIG_FILE)
+
+    # load mlflow config file
     try:
-        with open(finetune_args_file, "r") as rptr:
-            finetune_args = json.load(rptr)
+        with open(mlflow_config_file, "r") as rptr:
+            mlmodel_data = yaml.safe_load(rptr)
     except Exception as e:
-        raise LLMException._with_error(
-            AzureMLError.create(LLMInternalError, error=(
-                f"Failed to load {finetune_args_file}\n"
+        raise ACFTSystemException._with_error(
+            AzureMLError.create(ACFTSystemError, pii_safe_message=(
+                f"Failed to load {mlflow_config_file}\n"
                 f"{e}"
                 )
             )
         )
+    return mlmodel_data
 
-    # check for `model_name` in metadata file
-    if finetune_args and "model_name" in finetune_args:
-        return finetune_args["model_name"]
-    else:
-        raise LLMException._with_error(
-            AzureMLError.create(LLMInternalError, error=(
-                f"model_name is missing in "
-                f"{SaveFileConstants.FINETUNE_ARGS_SAVE_PATH} file"
-                )
+
+def _get_model_flavor(flavor_map: dict, mlmodel_data: dict) -> str:
+    supported_flavours = list(flavor_map.keys())
+    for each_flavor in supported_flavours:
+        if each_flavor in mlmodel_data["flavors"]:
+            return each_flavor
+
+    raise ACFTValidationException._with_error(
+        AzureMLError.create(
+            ACFTUserError,
+            pii_safe_message=(
+                f"MLFlow model is only supported for flavours: {supported_flavours}"
             )
         )
+    )
 
 
-def get_model_name_from_mlflow_model(model_path: str) -> str:
-    """
-    Fetch model_name information from mlflow metadata file
+def get_model_name_from_pytorch_model(model_path: str) -> str:
+    """Fetch model_name information from pytorch model metadata file.
+
+    Search order for model_name: finetune_args.json > finetune_config.json > default model name
     """
-    mlflow_config_file = Path(model_path, MLFlowHFFlavourConstants.MISC_CONFIG_FILE)
+    finetune_args_file = Path(model_path, SaveFileConstants.FINETUNE_ARGS_SAVE_PATH)
+    finetune_config_file = Path(model_path, SaveFileConstants.ACFT_CONFIG_SAVE_PATH)
+    default_model_name = MLFlowHFFlavourConstants.DEFAULT_MODEL_NAME
 
-    # load mlflow config file
-    try:
-        with open(mlflow_config_file, "r") as rptr:
-            mlflow_data = yaml.safe_load(rptr)
-    except Exception as e:
-        raise LLMException._with_error(
-            AzureMLError.create(LLMInternalError, error=(
-                f"Failed to load {mlflow_config_file}\n"
-                f"{e}"
-                )
-            )
+    # check if the metadata files exist
+    if not any([finetune_args_file.exists(), finetune_config_file.exists()]):
+        logger.warning(
+            f"Both {finetune_args_file} and {finetune_args_file} doesn't exist. "
+            f"Setting the model name to default value: {MLFlowHFFlavourConstants.DEFAULT_MODEL_NAME}"
         )
+        return MLFlowHFFlavourConstants.DEFAULT_MODEL_NAME
+
+    # load the finetune_args metadata file
+    if finetune_args_file.exists():
+        finetune_args_data = read_json_file(finetune_args_file)
+        if finetune_args_data is not None and "model_name" in finetune_args_data:
+            logger.info(f'model name: {finetune_args_data["model_name"]}')
+            return finetune_args_data["model_name"]
+    logger.debug(f"Model name not found in {finetune_args_file}")
+
+    # load the finetune_config metadata file
+    if finetune_config_file.exists():
+        finetune_config_data = read_json_file(finetune_config_file)
+        if finetune_config_data is not None and "model_name" in finetune_config_data:
+            logger.info(f'model name: {finetune_config_data["model_name"]}')
+            return finetune_config_data["model_name"]
+    logger.debug(f"Model name not found in {finetune_config_file}")
+
+    return default_model_name
+
+
+def get_model_name_from_mlflow_model(mlmodel_data: dict, flavor_map: dict, mlflow_flavor: str) -> str:
+    """
+    Fetch model_name information from mlflow metadata file
+    """
 
     # fetch the model name
     # TODO try to remove the hard limitation on the flavor name
-    try:
-        logger.info("Attempt #1 Searching with hftransformers flavor")
-        return mlflow_data["flavors"]["hftransformers"][MLFlowHFFlavourConstants.HUGGINGFACE_ID]
-    except Exception as _:
-        try:
-            logger.info("Attempt #2 Searching with hftransformersv2 flavor")
-            return mlflow_data["flavors"]["hftransformersv2"][MLFlowHFFlavourConstants.HUGGINGFACE_ID]
-        except Exception as e:
-            raise LLMException._with_error(
-                AzureMLError.create(LLMInternalError, error=(
-                    "{Invalid mlflow config file}\n"
-                    f"{e}"
-                    )
+
+    flavors = " ,".join(str(flvr) for flvr in flavor_map.keys())
+    if not mlflow_flavor:
+        raise ACFTValidationException._with_error(
+            AzureMLError.create(ACFTUserError, pii_safe_message=(
+                f"Failed to find any of mlflow flavors {flavors} in MLmodel\n"
                 )
             )
+        )
+
+    model_name = MLFlowHFFlavourConstants.DEFAULT_MODEL_NAME
+    logger.info(f"Model Flavor : {mlflow_flavor}")
+    if MLFlowHFFlavourConstants.HUGGINGFACE_ID in mlmodel_data["flavors"][mlflow_flavor].keys():
+        model_name = mlmodel_data["flavors"][mlflow_flavor][MLFlowHFFlavourConstants.HUGGINGFACE_ID]
+    else:
+        logger.info("Huggingface_id not found in mlflow config, setting default_model_name")
 
+    logger.info(f"model name: {model_name}")
+    return model_name
 
-def convert_mlflow_model_to_pytorch_model(mlflow_model_path: Union[str, Path], download_dir: Path):
+def convert_mlflow_model_to_pytorch_model(mlflow_model_path: Union[str, Path], download_dir: Path, flavor_map: dict, mlflow_flavor: str):
     """
     converts mlflow model to pytorch model
     """
     download_dir.mkdir(exist_ok=True, parents=True)
     try:
         # copy the model files
-        shutil.copytree(
-            Path(mlflow_model_path, 'data/model'),
-            download_dir,
-            dirs_exist_ok=True
-        )
+        mlflow_model_dir = Path(mlflow_model_path, flavor_map[mlflow_flavor]["model"])
+        if mlflow_model_dir.is_dir():
+            shutil.copytree(
+                mlflow_model_dir,
+                download_dir,
+                dirs_exist_ok=True
+            )
+        else:
+            logger.warning("Model folder is not present in `mlflow_model_folder`. Skipping the copy.")
+
         # copy config files
-        shutil.copytree(
-            Path(mlflow_model_path, 'data/config'),
-            download_dir,
-            dirs_exist_ok=True
-        )
+        mlflow_config_dir = Path(mlflow_model_path, flavor_map[mlflow_flavor]["config"])
+        if mlflow_config_dir.is_dir():
+            shutil.copytree(
+                mlflow_config_dir,
+                download_dir,
+                dirs_exist_ok=True
+            )
+        else:
+            logger.warning("Config folder is not present in `mlflow_model_folder`. Skipping the copy.")
+
         # copy tokenizer files
-        shutil.copytree(
-            Path(mlflow_model_path, 'data/tokenizer'),
-            download_dir,
-            dirs_exist_ok=True
-        )
+        mlflow_tokenizer_dir = Path(mlflow_model_path, flavor_map[mlflow_flavor]["tokenizer"])
+        if mlflow_tokenizer_dir.is_dir():
+            shutil.copytree(
+                mlflow_tokenizer_dir,
+                download_dir,
+                dirs_exist_ok=True
+            )
+        else:
+            logger.warning("Tokenizer folder is not present in `mlflow_model_folder`. Skipping the copy.")
+
+        # copy code files
+        # TODO: update code path on basis of flavor, will be done after phi model onboarding
+        mlflow_code_dir = Path(mlflow_model_path, 'code')
+        if mlflow_code_dir.is_dir():
+            shutil.copytree(
+                mlflow_code_dir,
+                download_dir,
+                dirs_exist_ok=True
+            )
+
         # copy LICENSE file
         license_file_path = Path(mlflow_model_path, MLFlowHFFlavourConstants.LICENSE_FILE)
         if license_file_path.is_file():
             shutil.copy(str(license_file_path), download_dir)
+
     except Exception as e:
         shutil.rmtree(download_dir, ignore_errors=True)
-        raise LLMException._with_error(
-            AzureMLError.create(
-                LLMInternalError,
-                error=(
-                    "Failed to convert mlflow model to pytorch model.\n"
-                    f"{e}"
+        raise ACFTValidationException._with_error(
+            AzureMLError.create(ACFTUserError, pii_safe_message=(
+                "Failed to convert mlflow model to pytorch model.\n"
+                f"{e}"
                 )
             )
         )
 
 
 def model_selector(model_selector_args: Dict[str, Any]):
     """
@@ -172,41 +238,46 @@
         model_selector_args["model_name"] = model_name
         download_dir = Path(model_selector_args["output_dir"], model_name)
         download_dir.mkdir(exist_ok=True, parents=True)
         try:
             shutil.copytree(pytorch_model_path, download_dir, dirs_exist_ok=True)
         except Exception as e:
             shutil.rmtree(download_dir, ignore_errors=True)
-            raise LLMException._with_error(
+            raise ACFTSystemException._with_error(
                 AzureMLError.create(
-                    LLMInternalError,
-                    error=(
+                    ACFTSystemError,
+                    pii_safe_message=(
                         "shutil copy failed.\n"
                         f"{e}"
                     )
                 )
             )
     elif mlflow_model_path is not None:
         logger.info("Working with Mlflow model")
         model_selector_args["huggingface_id"] = None
-        model_name = get_model_name_from_mlflow_model(mlflow_model_path)
+        # load MLModel File
+        mlmodel_data = _load_mlflow_model( mlflow_model_path)
+        flavor_map = model_selector_args.get("flavor_map", FLAVOR_MAP_FOR_FALLBACK)
+        mlflow_flavor = _get_model_flavor(flavor_map, mlmodel_data)
+        model_name = get_model_name_from_mlflow_model(mlmodel_data, flavor_map, mlflow_flavor)
         model_selector_args["model_name"] = model_name
         # convert mlflow model to pytorch model and save it to model_save_path
         download_dir = Path(model_selector_args["output_dir"], model_name)
-        convert_mlflow_model_to_pytorch_model(mlflow_model_path, download_dir)
+        convert_mlflow_model_to_pytorch_model(mlflow_model_path, download_dir, flavor_map, mlflow_flavor)
     elif model_selector_args["model_name"]:
         logger.info(f'Will fetch {model_selector_args["model_name"]} model while fine-tuning')
     else:
-        raise LLMException._with_error(
+        raise ACFTValidationException._with_error(
                 AzureMLError.create(
-                    LLMInternalError,
-                    error=(
+                    ACFTUserError,
+                    pii_safe_message=(
                         "Please provide `huggingface_id` or pass valid model to `pytorch_model_path` or `mlflow_model_path`"
                     )
                 )
             )
 
     # Saving model selector args
-    model_selector_args_save_path = str(Path(model_selector_args["output_dir"], SaveFileConstants.MODEL_SELECTOR_ARGS_SAVE_PATH))
+    model_selector_args_save_path = str(
+        Path(model_selector_args["output_dir"], SaveFileConstants.MODEL_SELECTOR_ARGS_SAVE_PATH))
     logger.info(f"Saving the model selector args to {model_selector_args_save_path}")
     with open(model_selector_args_save_path, "w") as wptr:
         json.dump(model_selector_args, wptr, indent=2)
```

## azureml/acft/contrib/hf/nlp/utils/preprocess_utils.py

```diff
@@ -15,30 +15,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 """
 preprocess utils
 """
 
+from functools import partial
 import os
 import json
 import numpy as np
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
+from azureml.acft.common_components import get_logger_app
+from azureml.acft.contrib.hf.nlp.utils.data_utils import AzuremlDataset
+from azureml.acft.contrib.hf.nlp.utils.validation_utils import get_set_difference
 from ..constants.constants import AutomlConstants, DataConstants
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 # AutoML NLP tasks
 
 def get_new_file_name(path, old_format, new_format):
     prefix = os.path.splitext(path)[0]
     old_name = prefix.split('/')[-1]
-    return f'./{old_format}_{old_name}.{new_format}'
+    return f'{old_format}_{old_name}.{new_format}'
 
 
 def txt_to_jsonl(txt_file, name):
     with open(txt_file, encoding=DataConstants.ENCODING, errors=DataConstants.ERRORS) as f:
         data = f.read()
 
     with open(name, 'w') as output_file:
@@ -85,14 +88,56 @@
     new_input = ". ".join(input_col_entries)
     new_example = {AutomlConstants.TEXT_CLASSIFICATION_COLUMN_NAME: new_input}
     for label_col in pass_through_columns.intersection(dataset_columns):
         new_example[label_col] = example[label_col]
     return new_example
 
 
+def restructure_columns(nlp_obj: AzuremlDataset) -> None:
+    """
+    1) Concatenate all Text-columns
+    2) Remove columns from dataset which got concatenated, except for columns
+    specified in pass_through_columns/ label/ sentence
+    3) Generate warnings if passed in parameter columns are not present in the dataset
+
+    :param nlp_obj: Object of class AzuremlDataset or its subclass from azureml.acft.contrib.hf.nlp package.
+    :type nlp_obj: str
+    """
+    if nlp_obj.label_column and nlp_obj.label_column not in nlp_obj.dataset.features:
+        logger.warning(f"Passed in Label column {nlp_obj.label_column} not found in dataset")
+
+    absent_cols = get_set_difference(nlp_obj.pass_through_columns, list(nlp_obj.dataset.features.keys()))
+    if len(absent_cols) > 0:
+        logger.warning(f"Passed in pass through column {absent_cols} not found in dataset")
+
+    absent_cols = get_set_difference(nlp_obj.dataset_columns, list(nlp_obj.dataset.features.keys()))
+    if len(absent_cols) > 0:
+        logger.warning(f"Passed in dataset column {absent_cols} not found in dataset")
+
+    if nlp_obj.label_column and nlp_obj.dataset_columns and nlp_obj.label_column not in nlp_obj.dataset_columns:
+        logger.warning(f"Passed in Label column {nlp_obj.label_column} not found in dataset_columns passed")
+
+    label_columns = [nlp_obj.label_column] if nlp_obj.label_column is not None else []
+    label_columns = label_columns + \
+                    ([nlp_obj.dataset_args["label_key"]] if nlp_obj.dataset_args["label_key"] is not None else [])
+    exclude_columns = label_columns + nlp_obj.pass_through_columns
+    cols_to_remove = [col for col in nlp_obj.dataset.column_names if col not in exclude_columns]
+    nlp_obj.dataset = nlp_obj.dataset.map(
+        partial(
+            concat_text_columns,
+            label_columns=label_columns,
+            pass_through_columns=nlp_obj.pass_through_columns,
+            ignore_columns=nlp_obj.ignore_columns,
+            dataset_columns=nlp_obj.dataset_columns,
+        ),
+        batched=False,
+        remove_columns=cols_to_remove,
+    )
+
+
 def get_max_seq_length(train_data,
                        tokenizer,
                        enable_long_range_text) -> int:
     """
     Default value for max_seq_length is 128.
 
     If the user opts in for long range text, we use this heuristic to determine optimal max_seq_length value.
```

## azureml/acft/contrib/hf/nlp/utils/validation_utils.py

```diff
@@ -14,30 +14,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 """
 validation utils
 """
-
+import typing
 from abc import ABC
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Set
 import copy
 
 from datasets import Value, Sequence
 
-from azureml.acft.accelerator.utils.logging_utils import get_logger_app
-from azureml.acft.accelerator.utils.error_handling.exceptions import ValidationException
-from azureml.acft.accelerator.utils.error_handling.error_definitions import ValidationError
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTDataException
+from azureml.acft.common_components.utils.error_handling.error_definitions import ACFTUserError
+
+from azureml.acft.common_components import get_logger_app
 from azureml._common._error_definition.azureml_error import AzureMLError
 
-from ..constants.constants import AzuremlConstants
+from ..constants.constants import AzuremlConstants, DatasetSplit, ValidationConstants, Tasks
 
 
-logger = get_logger_app()
+logger = get_logger_app(__name__)
 
 
 class AzuremlValidatorMixin(ABC):
     """
     This is a mixin to be used with 'AzuremlDataset' class to provide common utility functions for data validation
     """
 
@@ -65,32 +66,50 @@
             _ = self.required_columns.pop(label_column_index)
             _ = self.required_column_dtypes.pop(label_column_index)
             self.label_column = None
 
         # backup input dataset columns to log error in case the columns don't match during :meth match_columns
         self.original_datset_columns = copy.copy(self.dataset.column_names)
 
+    def apply_common_validations(self, split, batch_size: int = 1000, task_name: Optional[str] = None) -> None:
+        """
+        Applies Data Validations common to all tasks
+        """
+        # Remove the extra columns and match the remaining columns
+        self.remove_extra_columns()
+        self.match_columns()
+        # Check for duplicate column names
+        self.check_duplicate_column_names()
+
+        # filter data
+        # null filter
+        self.remove_null_examples(batch_size=batch_size)
+
+        # check for minimum num of training samples
+        if split == DatasetSplit.TRAIN:
+            self.check_min_train_samples(task_name)
+
     def remove_extra_columns(self) -> None:
         """
         Removes columns other than required columns and updates the self.dataset
         """
         columns_to_remove = [name for name in self.dataset.column_names if name not in self.required_columns]
         self.dataset = self.dataset.remove_columns(columns_to_remove)
         logger.info(f"Removed columns: {columns_to_remove} from dataset")
 
     def match_columns(self) -> None:
         """
         Match the dataset columns with the keep columns and raise error otherwise
         """
         if sorted(self.required_columns) != sorted(self.dataset.column_names):
             logger.warning("Exception occured while matching dataset columns with user passed columns, scrubbing exception")
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=(
+                    ACFTUserError,
+                    pii_safe_message=(
                         f"Path or dict: {self.path_or_dict}."
                         f"Dataset Columns: {self._remove_dataset_column_prefix(self.original_datset_columns)}."
                         f"User Passed Columns: {self._remove_dataset_column_prefix(self.required_columns)}."
                     )
                 )
             )
 
@@ -104,21 +123,35 @@
             if column_name not in datset_features:
                 logger.warning("Exception occured column name not present in dataset, scrubbing exception")
                 raise ValueError(
                     f"{column_name} not present in column to dtypes map file."
                     f"The following columns are present: {list(datset_features.keys())}"
                 )
 
+            if not isinstance(datset_features[column_name], Value):
+                logger.warning("Unable to validate dataset dtypes")
+                raise ACFTDataException._with_error(
+                    AzureMLError.create(
+                        ACFTUserError,
+                        pii_safe_message=(
+                            f"File path or data: {self.path_or_dict}\n"
+                            f"Unable to validate dtype for feature {self._remove_dataset_column_prefix(column_name)}\n"
+                            f"Found column type: {type(datset_features[column_name])}\n"
+                            f"Expected dtypes: {valid_dtypes}"
+                        )
+                    )
+                )
+
             column_dtype = datset_features[column_name].dtype
             if column_dtype not in valid_dtypes:
                 logger.warning("Exception occured column dtype not valid, scrubbing exception")
-                raise ValidationException._with_error(
+                raise ACFTDataException._with_error(
                     AzureMLError.create(
-                        ValidationError,
-                        error=(
+                        ACFTUserError,
+                        pii_safe_message=(
                             f"File path or data: {self.path_or_dict}\n"
                             f"dtype mismatch for feature {self._remove_dataset_column_prefix(column_name)}\n"
                             f"Found dtype: {column_dtype}\n"
                             f"Expected dtypes: {valid_dtypes}"
                         )
                     )
                 )
@@ -151,18 +184,76 @@
             null_filter,
             batch_size=batch_size,
             writer_batch_size=batch_size
         )
         post_filter_rows = self.dataset.num_rows
         logger.info(f"Null filter - examples before filter: {pre_filter_rows} | examples after filter: {post_filter_rows}")
         if post_filter_rows == 0:
-            raise ValidationException._with_error(
+            raise ACFTDataException._with_error(
+                AzureMLError.create(
+                    ACFTUserError,
+                    pii_safe_message=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                )
+            )
+
+    def check_min_train_samples(self, task_name: Optional[str] = None) -> None:
+        """
+        Raises error if the number of examples in training set (after earlier checks) is lower than threshold
+        """
+        training_rows = self.dataset.num_rows
+        logger.info(f"Number of training samples post filtration: {training_rows}")
+        min_train_samples = ValidationConstants.MIN_TRAINING_SAMPLE
+        # Overriding min number of samples to consider for generative tasks like Text Generation and Chat completion
+        # This would allow customers to finetune on smaller datasets as we have seen 
+        # customers having less than 50 rows of training data trying to do finetuning
+        if task_name == Tasks.TEXT_GENERATION:
+            logger.info(
+                "Overriding min number of training samples to be considered for generative tasks to: {}".format(ValidationConstants.MIN_TRAINING_SAMPLE_GENERATIVE_TASKS)
+            )
+            min_train_samples = ValidationConstants.MIN_TRAINING_SAMPLE_GENERATIVE_TASKS
+        if training_rows < min_train_samples:
+            raise ACFTDataException._with_error(
                 AzureMLError.create(
-                    ValidationError,
-                    error=f"Found no examples after data preprocessing for {self.path_or_dict}"
+                    ACFTUserError,
+                    pii_safe_message=f"Training dataset has {training_rows} non-null samples, which is fewer than "\
+                        f"{min_train_samples} samples, which is the min required to finetune. "\
+                        f"Please check your training dataset or provide a validation dataset"\
+                        f"(training dataset will be split if no validation dataset)."
+                )
+            )
+
+    def check_duplicate_column_names(self) -> None:
+        """
+        Raises error if any duplicate column names are found
+        """
+        if len(self.dataset.column_names) != len(set(self.dataset.column_names)):
+            logger.warning("Exception occured: duplicate column names detected, scrubbing exception")
+            raise ACFTDataException._with_error(
+                AzureMLError.create(
+                    ACFTUserError,
+                    pii_safe_message=(
+                        f"File path or data: {self.path_or_dict}\n"
+                        f"Dataset has one or more duplicate column names\n"
+                    )
+                )
+            )
+
+    def check_column_contents(self, column1_name: Optional[str], column2_name: Optional[str]) -> None:
+        """
+        Raises error if the feature columns are identical
+        """
+        if column1_name is not None and column2_name is not None and self.dataset[column1_name] == self.dataset[column2_name]:
+            logger.warning("Exception occured: identical feature columns detected, scrubbing exception")
+            raise ACFTDataException._with_error(
+                AzureMLError.create(
+                    ACFTUserError,
+                    pii_safe_message=(
+                        f"File path or data: {self.path_or_dict}\n"
+                        f"Dataset columns are identical\n"
+                    )
                 )
             )
 
     def update_required_columns_with_prefix(self) -> None:
         """
         This function  will update the :param `required_columns` with a constant prefix
         """
@@ -199,7 +290,32 @@
         prefix_to_remove = AzuremlConstants.DATASET_COLUMN_PREFIX
         if data.startswith(prefix_to_remove):
             return prefix_to_remove.join(data.split(prefix_to_remove)[1:])
         else:
             logger.warning("Prefix not found! Skipping removal")
             return data
     return data
+
+
+def get_set_difference(minuend: Union[List, Set, str, dict], subtrahend: Union[List, Set, str, dict]) -> List:
+    """
+    Return set difference as minuend - subtrahend
+    e.g. [1,2,3] - [2, 3, 9], will return [1]
+
+    :param minuend:
+    :type minuend: Union[List, Set, str, dict]
+    :param subtrahend:
+    :type subtrahend: Union[List, Set, str, dict]
+
+    :return: True if all elements in <subset> are present in <superset>
+    :rtype: List
+    """
+    if minuend and subtrahend and len(minuend) > 0:
+        if not isinstance(minuend[0], typing.Hashable):
+            raise ValueError("minuend parameter in get_set_difference() should be list, set or dict of hashable type.")
+        if len(subtrahend) > 0 and not isinstance(subtrahend[0], typing.Hashable):
+            raise ValueError("subtrahend parameter in get_set_difference() should be list, set or dict of "
+                             "hashable type.")
+
+        return list(set(minuend).difference(set(subtrahend)))
+
+    return []
```

## Comparing `azureml_acft_contrib_hf_nlp-0.0.9.data/data/azureml-acft-contrib-hf-nlp/NOTICE` & `azureml_acft_contrib_hf_nlp-47.0.0.data/data/azureml-acft-contrib-hf-nlp/NOTICE`

 * *Files identical despite different names*

## Comparing `azureml_acft_contrib_hf_nlp-0.0.9.dist-info/LICENSE.txt` & `azureml_acft_contrib_hf_nlp-47.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_acft_contrib_hf_nlp-0.0.9.dist-info/RECORD` & `azureml_acft_contrib_hf_nlp-47.0.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,126 @@
 azureml/__init__.py,sha256=9yEu-iBWQHMmb7eapxBKtSs5hHWMDIZeGhXEntYSp4w,267
 azureml/acft/__init__.py,sha256=9yEu-iBWQHMmb7eapxBKtSs5hHWMDIZeGhXEntYSp4w,267
 azureml/acft/contrib/__init__.py,sha256=9yEu-iBWQHMmb7eapxBKtSs5hHWMDIZeGhXEntYSp4w,267
-azureml/acft/contrib/hf/__init__.py,sha256=9yEu-iBWQHMmb7eapxBKtSs5hHWMDIZeGhXEntYSp4w,267
+azureml/acft/contrib/hf/__init__.py,sha256=qC5hRHbTbRwhm4xSfuFpDl0ungDu3rxgX7bfPsaTQVA,792
+azureml/acft/contrib/hf/_version.py,sha256=6tbwTfcvkL7u8i_rkvzyeWb_6rwSOsoLFvfhWf89WZM,36
 azureml/acft/contrib/hf/nlp/NOTICE,sha256=EuZDT4SJ0Anyd3VCItECyYWbihi8KkmHDk1Oupz_NG8,869245
 azureml/acft/contrib/hf/nlp/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/base_runner.py,sha256=c1mjJJByWwP4coOfen6FYvYpb07ci5CCYeEaXNbXwKM,4929
-azureml/acft/contrib/hf/nlp/task_factory.py,sha256=u_gQt8kFROE131wdm7dgrR1dK_c1WrQOxnA3ohJ1fHY,2555
+azureml/acft/contrib/hf/nlp/base_runner.py,sha256=yorQpKXW7KvJOCU8ClglJvmurJoTait1DmNrtWEFm5I,7317
+azureml/acft/contrib/hf/nlp/task_factory.py,sha256=giLx0e6ToD17KAr_8o0-qMelpMCU8TdGS3c4XnWuqFY,2710
 azureml/acft/contrib/hf/nlp/constants/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/constants/constants.py,sha256=Vwx1oLmWQhOEjZPoiKtSU4vjNZ5kcvifxC6JfgAD1VQ,8213
+azureml/acft/contrib/hf/nlp/constants/constants.py,sha256=1OOeHXeQpSAvWOfDYYXw9it42t8j-wLWd_rvn13tuAE,11035
+azureml/acft/contrib/hf/nlp/entry_point/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/entry_point/data_import/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/entry_point/data_import/data_import.py,sha256=QK4kwaQvBsrg1svS-c8AcoiiO5tpKTXRU3CTO50idnU,4513
+azureml/acft/contrib/hf/nlp/entry_point/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/entry_point/finetune/finetune.py,sha256=Z2BCkF0gCvcnSJQ6iO4qugOerwLgykzMW0njRZi-_6Q,50782
+azureml/acft/contrib/hf/nlp/entry_point/finetune/finetune_config.py,sha256=L3kcgakPzsZQF4oLSuP39CYr-7W_4opJayteOuJ-1nI,11993
+azureml/acft/contrib/hf/nlp/entry_point/finetune/model_selector.py,sha256=wVmJtEeOt6ljOJ7za7SS4AVQpCYke3g-EB0Bk6I54Q0,15159
+azureml/acft/contrib/hf/nlp/entry_point/finetune/preprocess.py,sha256=BxnU5UqYCI0xxRnjk9e6E7VTqIf7LDRC3aXCukpLIMc,14043
+azureml/acft/contrib/hf/nlp/entry_point/finetune/register_model.py,sha256=kPoFeRoApcyp1D5OQPgEXDNijxKMwLGiNdG3xnNvzuo,11694
+azureml/acft/contrib/hf/nlp/entry_point/finetune/register_presets_model.py,sha256=vyR6m3rioaIM2hTum7xQAv8zjI_pwRxNfZ2VymmnW7s,18143
+azureml/acft/contrib/hf/nlp/entry_point/finetune/validate_lora_weights.py,sha256=OuT8Snis5_CcQRt6PDpaznXDRn5pI21GZhdvPoCxWSQ,4526
+azureml/acft/contrib/hf/nlp/entry_point/finetune/zero2.json,sha256=pSfQIRR3UKdPsv7e_rZYxIAh-FVxiIkpapoBkLCORN8,1166
+azureml/acft/contrib/hf/nlp/entry_point/finetune/zero3.json,sha256=-rBF2-DwJaBKDE0fhrAoWjGLn0fACJundFLS0Y1SAQw,1726
+azureml/acft/contrib/hf/nlp/metrics/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/metrics/load_metric.py,sha256=EuqEFEWhy-XAOpY0K_JN9vf2SfxWPrPUPESLGQ7PeO8,1303
+azureml/acft/contrib/hf/nlp/metrics/rouge.py,sha256=0YFVxdRRMKdcd7jyPMOQQiCAADjCOljM4iYczXTUHhE,5968
+azureml/acft/contrib/hf/nlp/metrics/sacrebleu.py,sha256=9RdmxtcgAFF5bot7wWGQGRlvJG0shtKt_42SQuesknw,8001
 azureml/acft/contrib/hf/nlp/nlp_auto/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/nlp_auto/config.py,sha256=bVpimbMtkElV1XBcTyZq2tAtR6Qg8_w1GK5X6RHS28o,3265
-azureml/acft/contrib/hf/nlp/nlp_auto/model.py,sha256=g0Th5aZJ4MwYmAp94OqKDpy6Yd19pPfl5fDkxLIzcus,14065
-azureml/acft/contrib/hf/nlp/nlp_auto/tokenizer.py,sha256=RbehFTgqLaLE3T2-Yfm7k4FwcEqlannMYlekV4D0Ums,4358
+azureml/acft/contrib/hf/nlp/nlp_auto/config.py,sha256=GAVv5A3g0RgZOA8LBSMXVQQOj0PGQnV1vnLW4zx9U8w,3289
+azureml/acft/contrib/hf/nlp/nlp_auto/model.py,sha256=i3vKEE8Mx-f23mBnYeOkAZGm7cKUkkTBdxtlOLTxfvA,20805
+azureml/acft/contrib/hf/nlp/nlp_auto/tokenizer.py,sha256=uEULefSuhP7TxDloT5iepyLXtdB_T8q3a3UQI-iZem0,4514
 azureml/acft/contrib/hf/nlp/tasks/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/tasks/base/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/tasks/base/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/tasks/base/finetune/finetune.py,sha256=ZjEF058NJ7QlJXhY-_WVCRB3_bbXa049ia0Yq7ZzXE8,4385
 azureml/acft/contrib/hf/nlp/tasks/multi_label/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/multi_label/runner.py,sha256=oyEFP_iq9C9sx9EAXvLW20nt1mXMidyI4mOaJMw2RMM,2520
+azureml/acft/contrib/hf/nlp/tasks/multi_label/runner.py,sha256=H_dUkcxWwmJTxa6ApCkrHaPa0d4gfD_gNs-AmKxvAAM,2857
 azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/finetune.py,sha256=UQIRkXsR67fO3pQ78JfNzMaebVg6HoEno6xQBIkF_fQ,10105
+azureml/acft/contrib/hf/nlp/tasks/multi_label/finetune/finetune.py,sha256=PUVAUPjouCmFdvxYX5QB6HgOymPGgsDyj4ffhMH5S1E,10875
 azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/base.py,sha256=V0BiBHXvQ_0FU_D3s4zXI8HGvaHAcITnaBw1ObYU09A,16173
-azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_finetune.py,sha256=-0ea579MvwvqWMvqFWw7qoU4m_xVfFCXC4H_ie7x9So,15582
-azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_inference.py,sha256=Z28E8dr0b61oDalR_A6R-9Q7h_S-4G8FPJUaTG80gPM,2552
+azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/base.py,sha256=Qeb4vISKoa8fZDr3ItPDI4kGQAa5Y7AkeEDopntBbTU,16318
+azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_finetune.py,sha256=gqhjcJnQb_fNYzIYF0_Tcqp_aFjhHEJuxcTZPL67uhM,15987
+azureml/acft/contrib/hf/nlp/tasks/multi_label/preprocess/preprocess_for_inference.py,sha256=IpQTVrxdK49awMtLpCEgB9MdFSevUGn6K-_2ed3nE2c,2349
 azureml/acft/contrib/hf/nlp/tasks/ner/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/ner/runner.py,sha256=FFGJEVpLuJ5EuY4E558--hUWz8GRLdc04McBhXYcYUc,3126
+azureml/acft/contrib/hf/nlp/tasks/ner/runner.py,sha256=wms5jRk_o1t-vrKue-9Mtw1nkXRFbZ813fYmlUm2YIU,3540
 azureml/acft/contrib/hf/nlp/tasks/ner/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/ner/finetune/finetune.py,sha256=n8zhWVlvc5duV_HjbklWYzjlPMp5f6OyVZV-85TLZww,9751
+azureml/acft/contrib/hf/nlp/tasks/ner/finetune/finetune.py,sha256=SuZwqRPKZ2FfyLpt34CO58_mHq7Rt_U0CiEr_nhHGWQ,10482
 azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/base.py,sha256=jMDvYM5-rD79XolBNrG_20MitbrxQ5JBPNTd6A8mbfs,13206
-azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_finetune.py,sha256=7vqrQ3xm7XNEMSYWNOc-_maEc7_SphGCGgFfKKkRte8,14826
-azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_inference.py,sha256=vEiUl2fyj7-BqeTSEhhYdFG2-jiTHq7hm9_VyDu78j8,4000
+azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/base.py,sha256=lnBcjhi9E6TLJX_8ZDOK9z2K0r-pupXCZkM4fqhKg30,13300
+azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_finetune.py,sha256=vSFv-ESrr_EN0Ct2c259UHVm1l7GIeuE3F4vH9UaSSo,15263
+azureml/acft/contrib/hf/nlp/tasks/ner/preprocess/preprocess_for_inference.py,sha256=VGOmAI0RjucOU2A50hTBUD_WkQxP2-WNkIUAaQkn3dM,3994
 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/runner.py,sha256=GmtKUOZeNVL-H-y1R-Yc5OIcLUf-vwHve0ZCdnenfZE,2487
-azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/finetune/finetune.py,sha256=EyOtaoFHPKZmh0zpVdwbWxejBFtvkZlgbgziKOY43Lg,9596
+azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/runner.py,sha256=QM7M-VQRaxIwI7-GVy3NagkudrWJQHtrewQzXnHiR2g,2541
 azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/base.py,sha256=PQ8KsXC8SSTpGwrN3XbbxcthYIOpUW0Oldy8fs2dejw,12965
-azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/preprocess_for_finetune.py,sha256=Gx3Fs_69b11zG_7lFswNN7gOcoj-SfN7CGc70ZYq5eE,12150
+azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/base.py,sha256=jzvsxIXT1uPLWn69lzq-Hovtohk9YwiaI3O8Fu0zFfg,11026
+azureml/acft/contrib/hf/nlp/tasks/nlp_multiclass/preprocess/preprocess_for_finetune.py,sha256=QO60dQ2-2pDb6LIhzYMCayAu09ZCPpEfrTO1TZxpi0k,12497
 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/runner.py,sha256=lnbCYWm3n5gvd_pBq7eghk5EsQqTBbgjFbin1M06o_A,2494
-azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/finetune/finetune.py,sha256=WAOJwp_KREH4PU2zAv8ersi0JC-3oJ9-so0S1Pk-CrM,10143
+azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/runner.py,sha256=GT5kfWV4-YaK-FtT_JI_bOQ6nlNX41hrYQCRAEL_STY,2464
 azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/base.py,sha256=17hrnWdSSCkSL1bcAQk4r4IaHQ8ro0c-nsXjpJXXJy4,12067
-azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/preprocess_for_finetune.py,sha256=lq1tbzrs9EWMuAYxdb5LXonZuDfXPw0nrE3y2N0x68s,12464
+azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/base.py,sha256=0iSjUasj848chFYhgGxe2l8smJGKBHrmjlSYvolx7ls,14453
+azureml/acft/contrib/hf/nlp/tasks/nlp_multilabel/preprocess/preprocess_for_finetune.py,sha256=uWCTS4ta9EV3Ir4XCK8LGYPKCBTbF-QEK5JEa7lsvnQ,13481
 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_ner/runner.py,sha256=uM8CKwUmFCsvVbB-Kjb0NpYFWtDImE7gry7I2V8kSQI,2380
-azureml/acft/contrib/hf/nlp/tasks/nlp_ner/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_ner/finetune/finetune.py,sha256=RFL-PZMUJIbtuRYuzlpxzQZ6qc94KxvtQHVZ06LyHAI,9649
+azureml/acft/contrib/hf/nlp/tasks/nlp_ner/runner.py,sha256=yYt6el0tpVgBC1yGWTckrI4Movr7W266iKEfXWGoagI,2409
 azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/base.py,sha256=VEyVWKF4X1Oirby7a0qj0nqUWsWJeV_AqZc5J6XxmbI,9985
-azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/preprocess_for_finetune.py,sha256=7Dlep4lsyCUIc28TwiIupObIzosDjqWTDsi_T1AfNzg,11434
+azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/base.py,sha256=OPhsUhnuM6Jp5ZcUIy41W9X0ZJLq1OtfjOgJx39_ErM,11377
+azureml/acft/contrib/hf/nlp/tasks/nlp_ner/preprocess/preprocess_for_finetune.py,sha256=AQoU-3xXZJZ81bpq-7Um1daWdYLTEI14_KxIkYKQlh8,11633
 azureml/acft/contrib/hf/nlp/tasks/qna/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/qna/runner.py,sha256=UFeBgjyuz9K1ECZToooYfDVB7j_mS0H8TQJLj_WIKI4,2453
+azureml/acft/contrib/hf/nlp/tasks/qna/runner.py,sha256=3q5SBKzG7ON-7deTKzucUQHbib2oIfrKAgtFnqSouIs,2833
 azureml/acft/contrib/hf/nlp/tasks/qna/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/qna/finetune/finetune.py,sha256=_rJrA-7qoLbwVnvp2HCJbbwvON2w7p4KPdE7rlrXLNs,14466
+azureml/acft/contrib/hf/nlp/tasks/qna/finetune/finetune.py,sha256=oqm-p9gFU13alof_RvLWzxIw4mOz2zE1XKQaPQR__Uo,14953
 azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/base.py,sha256=IsGIMls8BqD3BVl8wLCiQzx1JMKqg8yChb9vKr9QrKc,28677
-azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_finetune.py,sha256=IMPiEyyqOaFKaHgzLNGiXAguH-Nm4aJVFCiE5aItLIY,13059
-azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_inference.py,sha256=mxJqtZ4irl5w3zYc5QWTItT5_4bnnUCv1gwkwPGFMuo,2561
+azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/base.py,sha256=DDXXlRWrJwiSPjYkacvs0oNI2K0hSuVGLGRGafefn9A,29454
+azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_finetune.py,sha256=myRHPrcceWJ2v9JOVlfm5JRhjLIfXdSNnLc54X31y9Q,13450
+azureml/acft/contrib/hf/nlp/tasks/qna/preprocess/preprocess_for_inference.py,sha256=IpQTVrxdK49awMtLpCEgB9MdFSevUGn6K-_2ed3nE2c,2349
 azureml/acft/contrib/hf/nlp/tasks/single_label/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/single_label/runner.py,sha256=yGmF41_YNwXgHz2l7p2rAHXNAkFd6XqZAAzpHPrjHoU,2534
+azureml/acft/contrib/hf/nlp/tasks/single_label/runner.py,sha256=jHqZ78XwKX8SDAKWY7xHyljkKdFT9E-BdZBwoiqXrlg,2954
 azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/finetune.py,sha256=RnufNTmY3hln1iBbk_p7FUfR9wydzvxsb7Mr0mzclYE,9843
+azureml/acft/contrib/hf/nlp/tasks/single_label/finetune/finetune.py,sha256=ED-7z2a0vpkbccxxYQf2pORpbzaiq06rUK-O9WldNZ8,10430
 azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/base.py,sha256=AIwiDzvnzB8eEA4RdtVuuoDsYc8M_xk2rJ-nNY6D1Qw,10429
-azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_finetune.py,sha256=KF_wwIu-KImY5bD5xiSg3c8J6UXF6pRW2GVD1_YTxYQ,15153
-azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_inference.py,sha256=mxJqtZ4irl5w3zYc5QWTItT5_4bnnUCv1gwkwPGFMuo,2561
+azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/base.py,sha256=i0ODBhoN8DfxGASzqDnt6qjmiuYclh6iyIT7n4q7x_k,10646
+azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_finetune.py,sha256=97v2K0hYvDldNHoIcLzMV84Gj6N6_Uid_6O_HBdE6PM,15579
+azureml/acft/contrib/hf/nlp/tasks/single_label/preprocess/preprocess_for_inference.py,sha256=IpQTVrxdK49awMtLpCEgB9MdFSevUGn6K-_2ed3nE2c,2349
 azureml/acft/contrib/hf/nlp/tasks/summarization/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/summarization/runner.py,sha256=9havTTcqxz9CIh6H_1rBw2e_d14DZQ8dTg5BBETxoFc,2583
+azureml/acft/contrib/hf/nlp/tasks/summarization/runner.py,sha256=-aihzJKBLlczxVO1hepprMs2d511BsMTIujbpSH4d4U,2973
 azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/finetune.py,sha256=UoVIzIi31_cAQ5McW9UNSj3yLanPqQ8Qn1At5dAUMX4,9515
+azureml/acft/contrib/hf/nlp/tasks/summarization/finetune/finetune.py,sha256=lmTRSfBlLAmFCypHYk1b65Bgqmh-oJYoGN15ZzZRjAI,10356
 azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/base.py,sha256=OBUetoVMiai1k8mlBaNDh1nPLmdkvjqKgapLIVmD4Jw,11203
-azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_finetune.py,sha256=ee8c8MGMO4dnH7gef_-Fg2zD-MaGwtg8aJxOzikLSg0,16583
-azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_inference.py,sha256=xlGr2FrcWMQCS0Fx1bpMy6zR6d-szc4tEYPQ7XJ8kpw,2284
+azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/base.py,sha256=Ol_9wzKxAd9rqFjeEJIIB6ODp-JBWxxh9b58uFomTA4,11009
+azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_finetune.py,sha256=p6jAtcDJJRAoShtHsNCE8bQIENPOa-3fzcM-iiAoUxs,16560
+azureml/acft/contrib/hf/nlp/tasks/summarization/preprocess/preprocess_for_inference.py,sha256=uEq31XgiYWXtjg5AEFjadJRlJybatWjRB4V1Mt9jSXk,2278
+azureml/acft/contrib/hf/nlp/tasks/text_generation/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/tasks/text_generation/runner.py,sha256=ORT9y8dqEVK1tqqDoWAnGUaksg5_IqW4rMxibc2bJrA,2919
+azureml/acft/contrib/hf/nlp/tasks/text_generation/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/tasks/text_generation/finetune/finetune.py,sha256=zDr6dUIXZ1-DPHx9WkLvt-cTuckbWmJQ_43l2Evy8xI,8611
+azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
+azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/base.py,sha256=tIPcUyV2GMkQTOx9xqVGpXZH21vRiNs1e5yQoLwgG-o,15549
+azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/preprocess_for_finetune.py,sha256=fi7AFg3cyqM6iGjJZ4XB8bPsBJNoibQ8u4ljKmhDuiY,15448
+azureml/acft/contrib/hf/nlp/tasks/text_generation/preprocess/preprocess_for_inference.py,sha256=dkMhDcEq0C6eBsSJlmjL8182iSOetXEgl0g0-_-bogo,2391
 azureml/acft/contrib/hf/nlp/tasks/translation/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/translation/runner.py,sha256=t0urQYLorzVhyh4h634Yunw2JY6yD9VXhSctJPVDYIE,2546
+azureml/acft/contrib/hf/nlp/tasks/translation/runner.py,sha256=sk_MZTMQux284O8GUkHCObNPYulvvkc-qHGsGZmfQxM,2936
 azureml/acft/contrib/hf/nlp/tasks/translation/finetune/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/translation/finetune/finetune.py,sha256=n5sjlhhQ_P3GThMFO7KEX7lxGqEXR4KykEtXFxWIRxc,10788
+azureml/acft/contrib/hf/nlp/tasks/translation/finetune/finetune.py,sha256=aU-PkmptcQjnoevvG0vPwpy9-rCNuwe8OQxXvekIT_k,11683
 azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/base.py,sha256=sgSKZ-NJwn1zSwkrZG8ren9_aIHqfoEaLG1YK_yAbvU,11537
-azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_finetune.py,sha256=TEub2Xzdax0rDiPczGaOHfJW0Y1h3NpHFBE9-3GT61A,17727
-azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_inference.py,sha256=xlGr2FrcWMQCS0Fx1bpMy6zR6d-szc4tEYPQ7XJ8kpw,2284
+azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/base.py,sha256=X_CQp4fXH-bU3Rsl-cRrVey-SmPxMLKGptOvJOBky5A,11342
+azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_finetune.py,sha256=1mIW4bT84FUpZJhTUv2CeGxGPEZXPYO5fAkajftAFas,17779
+azureml/acft/contrib/hf/nlp/tasks/translation/preprocess/preprocess_for_inference.py,sha256=uEq31XgiYWXtjg5AEFjadJRlJybatWjRB4V1Mt9jSXk,2278
 azureml/acft/contrib/hf/nlp/utils/__init__.py,sha256=ouf2rAWSHFJAg_qtQ9B9JwI7xakZ69hDiMGqpDuzL-c,298
-azureml/acft/contrib/hf/nlp/utils/data_utils.py,sha256=mwFaZvhZZoORCDxklZjn7jWMsa_lnthZGm4f3Q_8cBg,16029
-azureml/acft/contrib/hf/nlp/utils/hf_argparser.py,sha256=n0eDuBW-rPZ5FF_1JomIGf8A4nAC4hNTarPstKEvSWU,19641
+azureml/acft/contrib/hf/nlp/utils/common_utils.py,sha256=BYAPEZiz8OF_370S0GBkBT9k4AvqI0KyNHWTubkXEcw,5477
+azureml/acft/contrib/hf/nlp/utils/data_utils.py,sha256=CN9foplrzG6m6hnDDjRmg1-uUpN9hcDn9pzUBnCsyGM,19817
+azureml/acft/contrib/hf/nlp/utils/hf_argparser.py,sha256=gwGgUC7VsmLtaBapNeOx1_4-UqWAvmH6hkJnK0GGVnc,21628
+azureml/acft/contrib/hf/nlp/utils/io_utils.py,sha256=PPDKKnJJKJgbmkXTKsZEAG94qCZbFMDujkxGElqRTmY,3516
 azureml/acft/contrib/hf/nlp/utils/mlflow_preprocess.py,sha256=NV4QQWPD9Gi5hQpXUkYpimNs5IXOLPBtcStIbKtSTcQ,1167
-azureml/acft/contrib/hf/nlp/utils/mlflow_utils.py,sha256=22MJXYPhKTmmQJFKsCfDPpMXRDaOJeqm-WLT0qQDkHY,8105
-azureml/acft/contrib/hf/nlp/utils/model_selector_utils.py,sha256=E7fntIeseAafDEHt4WK-MgEuUuBB1WyQn685tgFH9Uw,8208
+azureml/acft/contrib/hf/nlp/utils/mlflow_utils.py,sha256=Qq1yo5g9-hyPtqbtn5N4wk29pe9ucl1Ca1KFUuMvG8M,16226
+azureml/acft/contrib/hf/nlp/utils/model_selector_utils.py,sha256=L3Yx1Qsg0FTl3X8gPSEnXHvKTFZ_QjFVNOLHfjUlbrM,11706
 azureml/acft/contrib/hf/nlp/utils/preprocess.py,sha256=CmJaFRnAMnC9ksika4KLLB7WgfV4NXOU9XX0nm7JAAQ,801
-azureml/acft/contrib/hf/nlp/utils/preprocess_utils.py,sha256=aDFXqIhMX4IVzy7Lc2zVCH-SsAvMYtLHhWJ4N4E0vc4,5409
-azureml/acft/contrib/hf/nlp/utils/validation_utils.py,sha256=qR1ffqjnj76Z7pkVPHC_dweMZHUQ6WxwSluWGjBLI0M,9380
-azureml_acft_contrib_hf_nlp-0.0.9.data/data/azureml-acft-contrib-hf-nlp/NOTICE,sha256=EuZDT4SJ0Anyd3VCItECyYWbihi8KkmHDk1Oupz_NG8,869245
-azureml_acft_contrib_hf_nlp-0.0.9.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_acft_contrib_hf_nlp-0.0.9.dist-info/METADATA,sha256=ns37_mvVU7w1Qf9xOi4LfMyEBZ0RIFje1HiMwFVxMRU,1502
-azureml_acft_contrib_hf_nlp-0.0.9.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-azureml_acft_contrib_hf_nlp-0.0.9.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
-azureml_acft_contrib_hf_nlp-0.0.9.dist-info/RECORD,,
+azureml/acft/contrib/hf/nlp/utils/preprocess_utils.py,sha256=x6LpmS3gjL9RfY5INZNmSIZqfBpYQqj0cc4Lbndjtmc,7729
+azureml/acft/contrib/hf/nlp/utils/validation_utils.py,sha256=kr49t9XkqRSQELbHJzNy3iheVGDNLG-vtuxWDHALjAg,15039
+azureml_acft_contrib_hf_nlp-47.0.0.data/data/azureml-acft-contrib-hf-nlp/NOTICE,sha256=EuZDT4SJ0Anyd3VCItECyYWbihi8KkmHDk1Oupz_NG8,869245
+azureml_acft_contrib_hf_nlp-47.0.0.data/data/deepspeed/zero2.json,sha256=pSfQIRR3UKdPsv7e_rZYxIAh-FVxiIkpapoBkLCORN8,1166
+azureml_acft_contrib_hf_nlp-47.0.0.data/data/deepspeed/zero3.json,sha256=-rBF2-DwJaBKDE0fhrAoWjGLn0fACJundFLS0Y1SAQw,1726
+azureml_acft_contrib_hf_nlp-47.0.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_acft_contrib_hf_nlp-47.0.0.dist-info/METADATA,sha256=tlAw_s-2E6zrK4N0E1FMLg2wLe7xigu_kpXeVU-Stfw,1631
+azureml_acft_contrib_hf_nlp-47.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+azureml_acft_contrib_hf_nlp-47.0.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml_acft_contrib_hf_nlp-47.0.0.dist-info/RECORD,,
```

