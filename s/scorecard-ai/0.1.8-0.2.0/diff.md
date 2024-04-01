# Comparing `tmp/scorecard_ai-0.1.8.tar.gz` & `tmp/scorecard_ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_ai-0.1.8.tar", max compression
+gzip compressed data, was "scorecard_ai-0.2.0.tar", max compression
```

## Comparing `scorecard_ai-0.1.8.tar` & `scorecard_ai-0.2.0.tar`

### file list

```diff
@@ -1,74 +1,82 @@
--rw-r--r--   0        0        0     3605 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/README.md
--rw-r--r--   0        0        0      407 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2919 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/__init__.py
--rw-r--r--   0        0        0     2627 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/client.py
--rw-r--r--   0        0        0      519 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/core/__init__.py
--rw-r--r--   0        0        0      426 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/core/api_error.py
--rw-r--r--   0        0        0     1081 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      162 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/environment.py
--rw-r--r--   0        0        0      363 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/errors/__init__.py
--rw-r--r--   0        0        0      309 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/errors/forbidden_error.py
--rw-r--r--   0        0        0      297 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/errors/not_found_error.py
--rw-r--r--   0        0        0      308 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/py.typed
--rw-r--r--   0        0        0      684 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/resources/run/__init__.py
--rw-r--r--   0        0        0    12865 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/resources/run/client.py
--rw-r--r--   0        0        0      255 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/resources/testcase/__init__.py
--rw-r--r--   0        0        0    13043 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/resources/testcase/client.py
--rw-r--r--   0        0        0      347 2024-01-10 13:12:58.945589 scorecard_ai-0.1.8/src/scorecard/resources/testcase/types/__init__.py
--rw-r--r--   0        0        0      187 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testcase/types/testcase_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      187 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testcase/types/testcase_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      381 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testrecord/__init__.py
--rw-r--r--   0        0        0    11658 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testrecord/client.py
--rw-r--r--   0        0        0      518 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testrecord/types/__init__.py
--rw-r--r--   0        0        0      189 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      189 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      190 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_outputs_value.py
--rw-r--r--   0        0        0       65 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testset/__init__.py
--rw-r--r--   0        0        0    19335 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/resources/testset/client.py
--rw-r--r--   0        0        0     3179 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/__init__.py
--rw-r--r--   0        0        0      112 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/app_create_run_params.py
--rw-r--r--   0        0        0      113 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/app_test_record_create.py
--rw-r--r--   0        0        0      110 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/app_test_set_create.py
--rw-r--r--   0        0        0      140 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/body_start_github_workflow_start_github_workflow_post.py
--rw-r--r--   0        0        0     1002 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/create_run_params.py
--rw-r--r--   0        0        0     1126 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/custom_schema_input.py
--rw-r--r--   0        0        0     1127 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/custom_schema_output.py
--rw-r--r--   0        0        0     1116 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/custom_variable.py
--rw-r--r--   0        0        0      695 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/data_type_enum.py
--rw-r--r--   0        0        0      109 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/execution_params.py
--rw-r--r--   0        0        0      945 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/file_url.py
--rw-r--r--   0        0        0      966 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/http_validation_error.py
--rw-r--r--   0        0        0      120 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/lib_dto_types_create_run_params.py
--rw-r--r--   0        0        0      121 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/lib_dto_types_test_record_create.py
--rw-r--r--   0        0        0      118 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/lib_dto_types_test_set_create.py
--rw-r--r--   0        0        0      105 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/model_params.py
--rw-r--r--   0        0        0      974 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/not_found_error_body.py
--rw-r--r--   0        0        0     1016 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/paginated_testcase_response.py
--rw-r--r--   0        0        0      787 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/role_enum.py
--rw-r--r--   0        0        0     1512 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/run_external.py
--rw-r--r--   0        0        0     1248 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/run_status.py
--rw-r--r--   0        0        0      114 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/score_execution_params.py
--rw-r--r--   0        0        0      107 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/scoring_params.py
--rw-r--r--   0        0        0     1363 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_case.py
--rw-r--r--   0        0        0      998 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_case_create.py
--rw-r--r--   0        0        0      113 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_case_create_input.py
--rw-r--r--   0        0        0      178 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_case_custom_inputs_value.py
--rw-r--r--   0        0        0      178 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_case_custom_labels_value.py
--rw-r--r--   0        0        0     1229 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_record_create.py
--rw-r--r--   0        0        0      934 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/test_set_create.py
--rw-r--r--   0        0        0     1645 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/testrecord.py
--rw-r--r--   0        0        0      180 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/testrecord_custom_inputs_value.py
--rw-r--r--   0        0        0      180 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/testrecord_custom_labels_value.py
--rw-r--r--   0        0        0      181 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/testrecord_custom_outputs_value.py
--rw-r--r--   0        0        0     1385 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/testset.py
--rw-r--r--   0        0        0      977 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/unauthenticated_error.py
--rw-r--r--   0        0        0      978 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/unauthorized_error_body.py
--rw-r--r--   0        0        0      992 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-01-10 13:12:58.949589 scorecard_ai-0.1.8/src/scorecard/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 scorecard_ai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3605 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/README.md
+-rw-r--r--   0        0        0      408 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3159 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/__init__.py
+-rw-r--r--   0        0        0     8199 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/client.py
+-rw-r--r--   0        0        0      519 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/core/api_error.py
+-rw-r--r--   0        0        0     1082 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      162 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/environment.py
+-rw-r--r--   0        0        0      363 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/errors/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/errors/forbidden_error.py
+-rw-r--r--   0        0        0      297 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/errors/not_found_error.py
+-rw-r--r--   0        0        0      308 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/py.typed
+-rw-r--r--   0        0        0      890 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/resources/run/__init__.py
+-rw-r--r--   0        0        0    14688 2024-04-01 17:59:20.969019 scorecard_ai-0.2.0/src/scorecard/resources/run/client.py
+-rw-r--r--   0        0        0       65 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/score/__init__.py
+-rw-r--r--   0        0        0    11534 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/score/client.py
+-rw-r--r--   0        0        0      255 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testcase/__init__.py
+-rw-r--r--   0        0        0    14479 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testcase/client.py
+-rw-r--r--   0        0        0      347 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testcase/types/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testcase/types/testcase_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      244 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testcase/types/testcase_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      567 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/__init__.py
+-rw-r--r--   0        0        0    14995 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/client.py
+-rw-r--r--   0        0        0      812 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      246 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      247 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_outputs_value.py
+-rw-r--r--   0        0        0      154 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/testrecord_create_params_model_debug_info_value.py
+-rw-r--r--   0        0        0      151 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/testrecord_create_params_model_params_value.py
+-rw-r--r--   0        0        0       65 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testset/__init__.py
+-rw-r--r--   0        0        0    20257 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/resources/testset/client.py
+-rw-r--r--   0        0        0     3222 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/app_create_run_params.py
+-rw-r--r--   0        0        0      113 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/app_test_record_create.py
+-rw-r--r--   0        0        0      110 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/app_test_set_create.py
+-rw-r--r--   0        0        0      120 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/create_github_workflow_params.py
+-rw-r--r--   0        0        0      109 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/create_run_params.py
+-rw-r--r--   0        0        0     1121 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/custom_schema.py
+-rw-r--r--   0        0        0     1116 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/custom_variable.py
+-rw-r--r--   0        0        0      695 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/data_type_enum.py
+-rw-r--r--   0        0        0      109 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/execution_params.py
+-rw-r--r--   0        0        0      945 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/file_url.py
+-rw-r--r--   0        0        0     1327 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/grade.py
+-rw-r--r--   0        0        0      966 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/http_validation_error.py
+-rw-r--r--   0        0        0     1200 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/json_object.py
+-rw-r--r--   0        0        0      231 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/json_object_input_value.py
+-rw-r--r--   0        0        0      232 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/json_object_output_value.py
+-rw-r--r--   0        0        0      105 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/model_params.py
+-rw-r--r--   0        0        0      974 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/not_found_error_body.py
+-rw-r--r--   0        0        0     1016 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/paginated_testcase_response.py
+-rw-r--r--   0        0        0      787 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/role_enum.py
+-rw-r--r--   0        0        0     1504 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/run.py
+-rw-r--r--   0        0        0     1462 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/run_status.py
+-rw-r--r--   0        0        0      114 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/score_execution_params.py
+-rw-r--r--   0        0        0      639 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/score_status.py
+-rw-r--r--   0        0        0      107 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/scoring_params.py
+-rw-r--r--   0        0        0     1363 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_case.py
+-rw-r--r--   0        0        0      998 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_case_create.py
+-rw-r--r--   0        0        0      113 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_case_create_input.py
+-rw-r--r--   0        0        0      214 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_case_custom_inputs_value.py
+-rw-r--r--   0        0        0      214 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_case_custom_labels_value.py
+-rw-r--r--   0        0        0      110 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_record_create.py
+-rw-r--r--   0        0        0      107 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/test_set_create.py
+-rw-r--r--   0        0        0     2148 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testrecord.py
+-rw-r--r--   0        0        0      216 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testrecord_custom_inputs_value.py
+-rw-r--r--   0        0        0      216 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testrecord_custom_labels_value.py
+-rw-r--r--   0        0        0      217 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testrecord_custom_outputs_value.py
+-rw-r--r--   0        0        0      142 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testrecord_model_debug_info_value.py
+-rw-r--r--   0        0        0      139 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testrecord_model_params_value.py
+-rw-r--r--   0        0        0     1366 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/testset.py
+-rw-r--r--   0        0        0      977 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/unauthenticated_error.py
+-rw-r--r--   0        0        0      978 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0      992 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-01 17:59:20.973019 scorecard_ai-0.2.0/src/scorecard/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 scorecard_ai-0.2.0/PKG-INFO
```

### Comparing `scorecard_ai-0.1.8/README.md` & `scorecard_ai-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/__init__.py` & `scorecard_ai-0.2.0/src/scorecard/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,96 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     AppCreateRunParams,
     AppTestRecordCreate,
     AppTestSetCreate,
-    BodyStartGithubWorkflowStartGithubWorkflowPost,
+    CreateGithubWorkflowParams,
     CreateRunParams,
-    CustomSchemaInput,
-    CustomSchemaOutput,
+    CustomSchema,
     CustomVariable,
     DataTypeEnum,
     ExecutionParams,
     FileUrl,
+    Grade,
     HttpValidationError,
-    LibDtoTypesCreateRunParams,
-    LibDtoTypesTestRecordCreate,
-    LibDtoTypesTestSetCreate,
+    JsonObject,
+    JsonObjectInputValue,
+    JsonObjectOutputValue,
     ModelParams,
     NotFoundErrorBody,
     PaginatedTestcaseResponse,
     RoleEnum,
-    RunExternal,
+    Run,
     RunStatus,
     ScoreExecutionParams,
+    ScoreStatus,
     ScoringParams,
     TestCase,
     TestCaseCreate,
     TestCaseCreateInput,
     TestCaseCustomInputsValue,
     TestCaseCustomLabelsValue,
     TestRecordCreate,
     TestSetCreate,
     Testrecord,
     TestrecordCustomInputsValue,
     TestrecordCustomLabelsValue,
     TestrecordCustomOutputsValue,
+    TestrecordModelDebugInfoValue,
+    TestrecordModelParamsValue,
     Testset,
     UnauthenticatedError,
     UnauthorizedErrorBody,
     ValidationError,
     ValidationErrorLocItem,
 )
 from .errors import ForbiddenError, NotFoundError, UnauthorizedError, UnprocessableEntityError
 from .resources import (
     TestcaseCreateParamsCustomInputsValue,
     TestcaseCreateParamsCustomLabelsValue,
     TestrecordCreateParamsCustomInputsValue,
     TestrecordCreateParamsCustomLabelsValue,
     TestrecordCreateParamsCustomOutputsValue,
+    TestrecordCreateParamsModelDebugInfoValue,
+    TestrecordCreateParamsModelParamsValue,
     run,
+    score,
     testcase,
     testrecord,
     testset,
 )
 from .environment import ScorecardEnvironment
 
 __all__ = [
     "AppCreateRunParams",
     "AppTestRecordCreate",
     "AppTestSetCreate",
-    "BodyStartGithubWorkflowStartGithubWorkflowPost",
+    "CreateGithubWorkflowParams",
     "CreateRunParams",
-    "CustomSchemaInput",
-    "CustomSchemaOutput",
+    "CustomSchema",
     "CustomVariable",
     "DataTypeEnum",
     "ExecutionParams",
     "FileUrl",
     "ForbiddenError",
+    "Grade",
     "HttpValidationError",
-    "LibDtoTypesCreateRunParams",
-    "LibDtoTypesTestRecordCreate",
-    "LibDtoTypesTestSetCreate",
+    "JsonObject",
+    "JsonObjectInputValue",
+    "JsonObjectOutputValue",
     "ModelParams",
     "NotFoundError",
     "NotFoundErrorBody",
     "PaginatedTestcaseResponse",
     "RoleEnum",
-    "RunExternal",
+    "Run",
     "RunStatus",
     "ScoreExecutionParams",
+    "ScoreStatus",
     "ScorecardEnvironment",
     "ScoringParams",
     "TestCase",
     "TestCaseCreate",
     "TestCaseCreateInput",
     "TestCaseCustomInputsValue",
     "TestCaseCustomLabelsValue",
@@ -91,22 +98,27 @@
     "TestSetCreate",
     "TestcaseCreateParamsCustomInputsValue",
     "TestcaseCreateParamsCustomLabelsValue",
     "Testrecord",
     "TestrecordCreateParamsCustomInputsValue",
     "TestrecordCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomOutputsValue",
+    "TestrecordCreateParamsModelDebugInfoValue",
+    "TestrecordCreateParamsModelParamsValue",
     "TestrecordCustomInputsValue",
     "TestrecordCustomLabelsValue",
     "TestrecordCustomOutputsValue",
+    "TestrecordModelDebugInfoValue",
+    "TestrecordModelParamsValue",
     "Testset",
     "UnauthenticatedError",
     "UnauthorizedError",
     "UnauthorizedErrorBody",
     "UnprocessableEntityError",
     "ValidationError",
     "ValidationErrorLocItem",
     "run",
+    "score",
     "testcase",
     "testrecord",
     "testset",
 ]
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/core/__init__.py` & `scorecard_ai-0.2.0/src/scorecard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/core/client_wrapper.py` & `scorecard_ai-0.2.0/src/scorecard/core/client_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "scorecard-ai",
-            "X-Fern-SDK-Version": "0.1.8",
+            "X-Fern-SDK-Version": "v0.2.0",
         }
         headers["X-API-Key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/core/datetime_utils.py` & `scorecard_ai-0.2.0/src/scorecard/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/core/jsonable_encoder.py` & `scorecard_ai-0.2.0/src/scorecard/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/resources/__init__.py` & `scorecard_ai-0.2.0/src/scorecard/resources/testrecord/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import run, testcase, testrecord, testset
-from .testcase import TestcaseCreateParamsCustomInputsValue, TestcaseCreateParamsCustomLabelsValue
-from .testrecord import (
+from .types import (
     TestrecordCreateParamsCustomInputsValue,
     TestrecordCreateParamsCustomLabelsValue,
     TestrecordCreateParamsCustomOutputsValue,
+    TestrecordCreateParamsModelDebugInfoValue,
+    TestrecordCreateParamsModelParamsValue,
 )
 
 __all__ = [
-    "TestcaseCreateParamsCustomInputsValue",
-    "TestcaseCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomInputsValue",
     "TestrecordCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomOutputsValue",
-    "run",
-    "testcase",
-    "testrecord",
-    "testset",
+    "TestrecordCreateParamsModelDebugInfoValue",
+    "TestrecordCreateParamsModelParamsValue",
 ]
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/resources/run/client.py` & `scorecard_ai-0.2.0/src/scorecard/resources/testcase/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,149 +9,173 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.run_external import RunExternal
-from ...types.run_status import RunStatus
+from ...types.test_case import TestCase
 from ...types.unauthenticated_error import UnauthenticatedError
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
+from .types.testcase_create_params_custom_inputs_value import TestcaseCreateParamsCustomInputsValue
+from .types.testcase_create_params_custom_labels_value import TestcaseCreateParamsCustomLabelsValue
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class RunClient:
+class TestcaseClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self,
-        *,
         testset_id: int,
-        scoring_config_id: typing.Optional[int] = OMIT,
-        status: typing.Optional[str] = OMIT,
-        model_params: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-    ) -> RunExternal:
+        *,
+        user_query: str,
+        context: typing.Optional[str] = OMIT,
+        ideal: typing.Optional[str] = OMIT,
+        custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]] = OMIT,
+        custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]] = OMIT,
+    ) -> TestCase:
         """
-        Create a new Run
+        Create a new Testcase
 
         Parameters:
             - testset_id: int.
 
-            - scoring_config_id: typing.Optional[int].
+            - user_query: str.
+
+            - context: typing.Optional[str].
+
+            - ideal: typing.Optional[str].
 
-            - status: typing.Optional[str].
+            - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]].
+
+            - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]].
+        ---
+        from scorecard.client import Scorecard
 
-            - model_params: typing.Optional[typing.Dict[str, typing.Any]].
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.testcase.create(
+            testset_id=1,
+            user_query="user_query",
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"testset_id": testset_id}
-        if scoring_config_id is not OMIT:
-            _request["scoring_config_id"] = scoring_config_id
-        if status is not OMIT:
-            _request["status"] = status
-        if model_params is not OMIT:
-            _request["model_params"] = model_params
+        _request: typing.Dict[str, typing.Any] = {"user_query": user_query}
+        if context is not OMIT:
+            _request["context"] = context
+        if ideal is not OMIT:
+            _request["ideal"] = ideal
+        if custom_inputs is not OMIT:
+            _request["custom_inputs"] = custom_inputs
+        if custom_labels is not OMIT:
+            _request["custom_labels"] = custom_labels
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/run"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RunExternal, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, run_id: int) -> RunExternal:
+    def get(self, testcase_id: int, testset_id: int) -> TestCase:
         """
-        Retrieve a Run metadata
+        Retrieve Testcase data
 
         Parameters:
-            - run_id: int. The id of the run to retrieve.
+            - testcase_id: int.
+
+            - testset_id: int.
         ---
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.run.get(
-            run_id=1,
+        client.testcase.get(
+            testcase_id=1,
+            testset_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RunExternal, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_status(self, run_id: int, *, status: RunStatus) -> RunExternal:
+    def delete(self, testcase_id: int, testset_id: int) -> typing.Any:
         """
-        Update the status of a run.
+        Delete a Testcase
 
         Parameters:
-            - run_id: int. The id of the run to update.
+            - testcase_id: int.
 
-            - status: RunStatus.
+            - testset_id: int.
         ---
-        from scorecard import RunStatus
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.run.update_status(
-            run_id=1,
-            status=RunStatus.PENDING,
+        client.testcase.delete(
+            testcase_id=1,
+            testset_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/status"),
-            json=jsonable_encoder({"status": status}),
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RunExternal, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
@@ -159,135 +183,158 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncRunClient:
+class AsyncTestcaseClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
         self,
-        *,
         testset_id: int,
-        scoring_config_id: typing.Optional[int] = OMIT,
-        status: typing.Optional[str] = OMIT,
-        model_params: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-    ) -> RunExternal:
+        *,
+        user_query: str,
+        context: typing.Optional[str] = OMIT,
+        ideal: typing.Optional[str] = OMIT,
+        custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]] = OMIT,
+        custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]] = OMIT,
+    ) -> TestCase:
         """
-        Create a new Run
+        Create a new Testcase
 
         Parameters:
             - testset_id: int.
 
-            - scoring_config_id: typing.Optional[int].
+            - user_query: str.
+
+            - context: typing.Optional[str].
+
+            - ideal: typing.Optional[str].
 
-            - status: typing.Optional[str].
+            - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]].
+
+            - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]].
+        ---
+        from scorecard.client import AsyncScorecard
 
-            - model_params: typing.Optional[typing.Dict[str, typing.Any]].
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.testcase.create(
+            testset_id=1,
+            user_query="user_query",
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"testset_id": testset_id}
-        if scoring_config_id is not OMIT:
-            _request["scoring_config_id"] = scoring_config_id
-        if status is not OMIT:
-            _request["status"] = status
-        if model_params is not OMIT:
-            _request["model_params"] = model_params
+        _request: typing.Dict[str, typing.Any] = {"user_query": user_query}
+        if context is not OMIT:
+            _request["context"] = context
+        if ideal is not OMIT:
+            _request["ideal"] = ideal
+        if custom_inputs is not OMIT:
+            _request["custom_inputs"] = custom_inputs
+        if custom_labels is not OMIT:
+            _request["custom_labels"] = custom_labels
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/run"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RunExternal, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, run_id: int) -> RunExternal:
+    async def get(self, testcase_id: int, testset_id: int) -> TestCase:
         """
-        Retrieve a Run metadata
+        Retrieve Testcase data
 
         Parameters:
-            - run_id: int. The id of the run to retrieve.
+            - testcase_id: int.
+
+            - testset_id: int.
         ---
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.run.get(
-            run_id=1,
+        await client.testcase.get(
+            testcase_id=1,
+            testset_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}"),
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RunExternal, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_status(self, run_id: int, *, status: RunStatus) -> RunExternal:
+    async def delete(self, testcase_id: int, testset_id: int) -> typing.Any:
         """
-        Update the status of a run.
+        Delete a Testcase
 
         Parameters:
-            - run_id: int. The id of the run to update.
+            - testcase_id: int.
 
-            - status: RunStatus.
+            - testset_id: int.
         ---
-        from scorecard import RunStatus
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.run.update_status(
-            run_id=1,
-            status=RunStatus.PENDING,
+        await client.testcase.delete(
+            testcase_id=1,
+            testset_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/status"),
-            json=jsonable_encoder({"status": status}),
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RunExternal, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/resources/testcase/client.py` & `scorecard_ai-0.2.0/src/scorecard/resources/run/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,143 +9,178 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.test_case import TestCase
+from ...types.run import Run
+from ...types.run_status import RunStatus
 from ...types.unauthenticated_error import UnauthenticatedError
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
-from .types.testcase_create_params_custom_inputs_value import TestcaseCreateParamsCustomInputsValue
-from .types.testcase_create_params_custom_labels_value import TestcaseCreateParamsCustomLabelsValue
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class TestcaseClient:
+class RunClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self,
-        testset_id: int,
         *,
-        user_query: str,
-        context: typing.Optional[str] = OMIT,
-        ideal: typing.Optional[str] = OMIT,
-        custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]] = OMIT,
-        custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]] = OMIT,
-    ) -> TestCase:
+        testset_id: typing.Optional[int] = OMIT,
+        scoring_config_id: typing.Optional[int] = OMIT,
+        status: typing.Optional[str] = OMIT,
+        model_params: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        source: typing.Optional[str] = OMIT,
+        notes: typing.Optional[str] = OMIT,
+        prompt_template: typing.Optional[str] = OMIT,
+    ) -> Run:
         """
-        Create a new Testcase
+        Create a new Run
 
         Parameters:
-            - testset_id: int.
+            - testset_id: typing.Optional[int].
 
-            - user_query: str.
+            - scoring_config_id: typing.Optional[int].
 
-            - context: typing.Optional[str].
+            - status: typing.Optional[str].
 
-            - ideal: typing.Optional[str].
+            - model_params: typing.Optional[typing.Dict[str, typing.Any]].
 
-            - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]].
+            - source: typing.Optional[str].
 
-            - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]].
+            - notes: typing.Optional[str].
+
+            - prompt_template: typing.Optional[str].
+        ---
+        from scorecard.client import Scorecard
+
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.run.create(
+            testset_id=1,
+            scoring_config_id=2,
+            status="RUNNING_EXECUTION",
+            model_params={"param1": "value1", "param2": "value2"},
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"user_query": user_query}
-        if context is not OMIT:
-            _request["context"] = context
-        if ideal is not OMIT:
-            _request["ideal"] = ideal
-        if custom_inputs is not OMIT:
-            _request["custom_inputs"] = custom_inputs
-        if custom_labels is not OMIT:
-            _request["custom_labels"] = custom_labels
+        _request: typing.Dict[str, typing.Any] = {}
+        if testset_id is not OMIT:
+            _request["testset_id"] = testset_id
+        if scoring_config_id is not OMIT:
+            _request["scoring_config_id"] = scoring_config_id
+        if status is not OMIT:
+            _request["status"] = status
+        if model_params is not OMIT:
+            _request["model_params"] = model_params
+        if source is not OMIT:
+            _request["source"] = source
+        if notes is not OMIT:
+            _request["notes"] = notes
+        if prompt_template is not OMIT:
+            _request["prompt_template"] = prompt_template
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/run"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Run, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, testcase_id: int, testset_id: int) -> TestCase:
+    def get(self, run_id: int) -> Run:
         """
-        Retrieve Testcase data
+        Retrieve a Run metadata
 
         Parameters:
-            - testcase_id: int.
+            - run_id: int. The id of the run to retrieve.
+        ---
+        from scorecard.client import Scorecard
 
-            - testset_id: int.
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.run.get(
+            run_id=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Run, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, testcase_id: int, testset_id: int) -> typing.Any:
+    def update_status(self, run_id: int, *, status: RunStatus) -> Run:
         """
-        Delete a Testcase
+        Update the status of a run.
 
         Parameters:
-            - testcase_id: int.
+            - run_id: int. The id of the run to update.
+
+            - status: RunStatus.
+        ---
+        from scorecard import RunStatus
+        from scorecard.client import Scorecard
 
-            - testset_id: int.
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.run.update_status(
+            run_id=1,
+            status=RunStatus.PENDING,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
-            ),
+            "PATCH",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/status"),
+            json=jsonable_encoder({"status": status}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Run, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
@@ -153,128 +188,164 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTestcaseClient:
+class AsyncRunClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
         self,
-        testset_id: int,
         *,
-        user_query: str,
-        context: typing.Optional[str] = OMIT,
-        ideal: typing.Optional[str] = OMIT,
-        custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]] = OMIT,
-        custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]] = OMIT,
-    ) -> TestCase:
+        testset_id: typing.Optional[int] = OMIT,
+        scoring_config_id: typing.Optional[int] = OMIT,
+        status: typing.Optional[str] = OMIT,
+        model_params: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        source: typing.Optional[str] = OMIT,
+        notes: typing.Optional[str] = OMIT,
+        prompt_template: typing.Optional[str] = OMIT,
+    ) -> Run:
         """
-        Create a new Testcase
+        Create a new Run
 
         Parameters:
-            - testset_id: int.
+            - testset_id: typing.Optional[int].
 
-            - user_query: str.
+            - scoring_config_id: typing.Optional[int].
 
-            - context: typing.Optional[str].
+            - status: typing.Optional[str].
 
-            - ideal: typing.Optional[str].
+            - model_params: typing.Optional[typing.Dict[str, typing.Any]].
 
-            - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]].
+            - source: typing.Optional[str].
 
-            - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]].
+            - notes: typing.Optional[str].
+
+            - prompt_template: typing.Optional[str].
+        ---
+        from scorecard.client import AsyncScorecard
+
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.run.create(
+            testset_id=1,
+            scoring_config_id=2,
+            status="RUNNING_EXECUTION",
+            model_params={"param1": "value1", "param2": "value2"},
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"user_query": user_query}
-        if context is not OMIT:
-            _request["context"] = context
-        if ideal is not OMIT:
-            _request["ideal"] = ideal
-        if custom_inputs is not OMIT:
-            _request["custom_inputs"] = custom_inputs
-        if custom_labels is not OMIT:
-            _request["custom_labels"] = custom_labels
+        _request: typing.Dict[str, typing.Any] = {}
+        if testset_id is not OMIT:
+            _request["testset_id"] = testset_id
+        if scoring_config_id is not OMIT:
+            _request["scoring_config_id"] = scoring_config_id
+        if status is not OMIT:
+            _request["status"] = status
+        if model_params is not OMIT:
+            _request["model_params"] = model_params
+        if source is not OMIT:
+            _request["source"] = source
+        if notes is not OMIT:
+            _request["notes"] = notes
+        if prompt_template is not OMIT:
+            _request["prompt_template"] = prompt_template
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/run"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Run, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, testcase_id: int, testset_id: int) -> TestCase:
+    async def get(self, run_id: int) -> Run:
         """
-        Retrieve Testcase data
+        Retrieve a Run metadata
 
         Parameters:
-            - testcase_id: int.
+            - run_id: int. The id of the run to retrieve.
+        ---
+        from scorecard.client import AsyncScorecard
 
-            - testset_id: int.
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.run.get(
+            run_id=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TestCase, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Run, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, testcase_id: int, testset_id: int) -> typing.Any:
+    async def update_status(self, run_id: int, *, status: RunStatus) -> Run:
         """
-        Delete a Testcase
+        Update the status of a run.
 
         Parameters:
-            - testcase_id: int.
+            - run_id: int. The id of the run to update.
+
+            - status: RunStatus.
+        ---
+        from scorecard import RunStatus
+        from scorecard.client import AsyncScorecard
 
-            - testset_id: int.
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.run.update_status(
+            run_id=1,
+            status=RunStatus.PENDING,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase/{testcase_id}"
-            ),
+            "PATCH",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/status"),
+            json=jsonable_encoder({"status": status}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Run, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/resources/testrecord/client.py` & `scorecard_ai-0.2.0/src/scorecard/resources/testrecord/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.testrecord import Testrecord
 from ...types.unauthenticated_error import UnauthenticatedError
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 from .types.testrecord_create_params_custom_inputs_value import TestrecordCreateParamsCustomInputsValue
 from .types.testrecord_create_params_custom_labels_value import TestrecordCreateParamsCustomLabelsValue
 from .types.testrecord_create_params_custom_outputs_value import TestrecordCreateParamsCustomOutputsValue
+from .types.testrecord_create_params_model_debug_info_value import TestrecordCreateParamsModelDebugInfoValue
+from .types.testrecord_create_params_model_params_value import TestrecordCreateParamsModelParamsValue
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
@@ -37,14 +39,24 @@
         """
         Retrieve Testrecord metadata
 
         Parameters:
             - testrecord_id: int.
 
             - run_id: int.
+        ---
+        from scorecard.client import Scorecard
+
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.testrecord.get(
+            testrecord_id=1,
+            run_id=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord/{testrecord_id}"
             ),
             headers=self._client_wrapper.get_headers(),
@@ -66,71 +78,99 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         run_id: int,
         *,
-        testset_id: int,
-        testcase_id: int,
-        user_query: str,
+        testset_id: typing.Optional[int] = OMIT,
+        testcase_id: typing.Optional[int] = OMIT,
+        user_query: typing.Optional[str] = OMIT,
         context: typing.Optional[str] = OMIT,
         response: typing.Optional[str] = OMIT,
         ideal: typing.Optional[str] = OMIT,
         custom_inputs: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]
         ] = OMIT,
         custom_outputs: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]
         ] = OMIT,
         custom_labels: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]
         ] = OMIT,
+        prompt: typing.Optional[str] = OMIT,
+        model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]] = OMIT,
+        model_debug_info: typing.Optional[
+            typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]
+        ] = OMIT,
     ) -> Testrecord:
         """
         Create a new Testrecord
 
         Parameters:
             - run_id: int.
 
-            - testset_id: int.
+            - testset_id: typing.Optional[int].
 
-            - testcase_id: int.
+            - testcase_id: typing.Optional[int].
 
-            - user_query: str.
+            - user_query: typing.Optional[str].
 
             - context: typing.Optional[str].
 
             - response: typing.Optional[str].
 
             - ideal: typing.Optional[str].
 
             - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]].
 
             - custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]].
 
             - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]].
+
+            - prompt: typing.Optional[str].
+
+            - model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]].
+
+            - model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]].
+        ---
+        from scorecard.client import Scorecard
+
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.testrecord.create(
+            run_id=1,
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "testset_id": testset_id,
-            "testcase_id": testcase_id,
-            "user_query": user_query,
-        }
+        _request: typing.Dict[str, typing.Any] = {}
+        if testset_id is not OMIT:
+            _request["testset_id"] = testset_id
+        if testcase_id is not OMIT:
+            _request["testcase_id"] = testcase_id
+        if user_query is not OMIT:
+            _request["user_query"] = user_query
         if context is not OMIT:
             _request["context"] = context
         if response is not OMIT:
             _request["response"] = response
         if ideal is not OMIT:
             _request["ideal"] = ideal
         if custom_inputs is not OMIT:
             _request["custom_inputs"] = custom_inputs
         if custom_outputs is not OMIT:
             _request["custom_outputs"] = custom_outputs
         if custom_labels is not OMIT:
             _request["custom_labels"] = custom_labels
+        if prompt is not OMIT:
+            _request["prompt"] = prompt
+        if model_params is not OMIT:
+            _request["model_params"] = model_params
+        if model_debug_info is not OMIT:
+            _request["model_debug_info"] = model_debug_info
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -159,14 +199,24 @@
         """
         Retrieve Testrecord metadata
 
         Parameters:
             - testrecord_id: int.
 
             - run_id: int.
+        ---
+        from scorecard.client import AsyncScorecard
+
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.testrecord.get(
+            testrecord_id=1,
+            run_id=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord/{testrecord_id}"
             ),
             headers=self._client_wrapper.get_headers(),
@@ -188,71 +238,99 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         run_id: int,
         *,
-        testset_id: int,
-        testcase_id: int,
-        user_query: str,
+        testset_id: typing.Optional[int] = OMIT,
+        testcase_id: typing.Optional[int] = OMIT,
+        user_query: typing.Optional[str] = OMIT,
         context: typing.Optional[str] = OMIT,
         response: typing.Optional[str] = OMIT,
         ideal: typing.Optional[str] = OMIT,
         custom_inputs: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]
         ] = OMIT,
         custom_outputs: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]
         ] = OMIT,
         custom_labels: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]
         ] = OMIT,
+        prompt: typing.Optional[str] = OMIT,
+        model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]] = OMIT,
+        model_debug_info: typing.Optional[
+            typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]
+        ] = OMIT,
     ) -> Testrecord:
         """
         Create a new Testrecord
 
         Parameters:
             - run_id: int.
 
-            - testset_id: int.
+            - testset_id: typing.Optional[int].
 
-            - testcase_id: int.
+            - testcase_id: typing.Optional[int].
 
-            - user_query: str.
+            - user_query: typing.Optional[str].
 
             - context: typing.Optional[str].
 
             - response: typing.Optional[str].
 
             - ideal: typing.Optional[str].
 
             - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]].
 
             - custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]].
 
             - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]].
+
+            - prompt: typing.Optional[str].
+
+            - model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]].
+
+            - model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]].
+        ---
+        from scorecard.client import AsyncScorecard
+
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.testrecord.create(
+            run_id=1,
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "testset_id": testset_id,
-            "testcase_id": testcase_id,
-            "user_query": user_query,
-        }
+        _request: typing.Dict[str, typing.Any] = {}
+        if testset_id is not OMIT:
+            _request["testset_id"] = testset_id
+        if testcase_id is not OMIT:
+            _request["testcase_id"] = testcase_id
+        if user_query is not OMIT:
+            _request["user_query"] = user_query
         if context is not OMIT:
             _request["context"] = context
         if response is not OMIT:
             _request["response"] = response
         if ideal is not OMIT:
             _request["ideal"] = ideal
         if custom_inputs is not OMIT:
             _request["custom_inputs"] = custom_inputs
         if custom_outputs is not OMIT:
             _request["custom_outputs"] = custom_outputs
         if custom_labels is not OMIT:
             _request["custom_labels"] = custom_labels
+        if prompt is not OMIT:
+            _request["prompt"] = prompt
+        if model_params is not OMIT:
+            _request["model_params"] = model_params
+        if model_debug_info is not OMIT:
+            _request["model_debug_info"] = model_debug_info
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/resources/testrecord/types/__init__.py` & `scorecard_ai-0.2.0/src/scorecard/resources/testrecord/types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .testrecord_create_params_custom_inputs_value import TestrecordCreateParamsCustomInputsValue
 from .testrecord_create_params_custom_labels_value import TestrecordCreateParamsCustomLabelsValue
 from .testrecord_create_params_custom_outputs_value import TestrecordCreateParamsCustomOutputsValue
+from .testrecord_create_params_model_debug_info_value import TestrecordCreateParamsModelDebugInfoValue
+from .testrecord_create_params_model_params_value import TestrecordCreateParamsModelParamsValue
 
 __all__ = [
     "TestrecordCreateParamsCustomInputsValue",
     "TestrecordCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomOutputsValue",
+    "TestrecordCreateParamsModelDebugInfoValue",
+    "TestrecordCreateParamsModelParamsValue",
 ]
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/resources/testset/client.py` & `scorecard_ai-0.2.0/src/scorecard/resources/testset/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...errors.forbidden_error import ForbiddenError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.custom_schema_input import CustomSchemaInput
-from ...types.custom_schema_output import CustomSchemaOutput
+from ...types.custom_schema import CustomSchema
 from ...types.http_validation_error import HttpValidationError
 from ...types.not_found_error_body import NotFoundErrorBody
 from ...types.paginated_testcase_response import PaginatedTestcaseResponse
 from ...types.testset import Testset
 from ...types.unauthenticated_error import UnauthenticatedError
 from ...types.unauthorized_error_body import UnauthorizedErrorBody
 
@@ -32,15 +31,15 @@
 
 class TestsetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(self, testset_id: int) -> Testset:
         """
-        Retrieve Testset metadata without Testcase data.
+        Retrieve Testset metadata without Testcase data
 
         Parameters:
             - testset_id: int.
         ---
         from scorecard.client import Scorecard
 
         client = Scorecard(
@@ -111,32 +110,43 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         name: str,
         description: typing.Optional[str] = OMIT,
-        using_retrieval: bool,
-        custom_schema: typing.Optional[CustomSchemaInput] = OMIT,
+        using_retrieval: typing.Optional[bool] = OMIT,
+        custom_schema: typing.Optional[CustomSchema] = OMIT,
     ) -> Testset:
         """
         Create a new Testset
 
         Parameters:
             - name: str.
 
             - description: typing.Optional[str].
 
-            - using_retrieval: bool.
+            - using_retrieval: typing.Optional[bool].
 
-            - custom_schema: typing.Optional[CustomSchemaInput].
+            - custom_schema: typing.Optional[CustomSchema].
+        ---
+        from scorecard.client import Scorecard
+
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.testset.create(
+            name="name",
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "using_retrieval": using_retrieval}
+        _request: typing.Dict[str, typing.Any] = {"name": name}
         if description is not OMIT:
             _request["description"] = description
+        if using_retrieval is not OMIT:
+            _request["using_retrieval"] = using_retrieval
         if custom_schema is not OMIT:
             _request["custom_schema"] = custom_schema
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/testset"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -154,38 +164,38 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_schema(self, testset_id: int) -> CustomSchemaOutput:
+    def read_schema(self, testset_id: int) -> CustomSchema:
         """
-        Read the schema of a Testset.
+        Read the schema of a Testset
 
         Parameters:
             - testset_id: int.
         ---
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.testset.get_schema(
+        client.testset.read_schema(
             testset_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/schema"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CustomSchemaOutput, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CustomSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
@@ -193,30 +203,39 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_testcases(
-        self, testset_id: int, *, page: typing.Optional[int] = None, page_size: typing.Optional[int] = None
+        self, testset_id: int, *, offset: typing.Optional[int] = None, limit: typing.Optional[int] = None
     ) -> PaginatedTestcaseResponse:
         """
         Retrieve all Testcases from a Testset
 
         Parameters:
             - testset_id: int.
 
-            - page: typing.Optional[int].
+            - offset: typing.Optional[int].
 
-            - page_size: typing.Optional[int].
+            - limit: typing.Optional[int].
+        ---
+        from scorecard.client import Scorecard
+
+        client = Scorecard(
+            api_key="YOUR_API_KEY",
+        )
+        client.testset.get_testcases(
+            testset_id=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase"),
-            params=remove_none_from_dict({"page": page, "page_size": page_size}),
+            params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTestcaseResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
@@ -235,15 +254,15 @@
 
 class AsyncTestsetClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get(self, testset_id: int) -> Testset:
         """
-        Retrieve Testset metadata without Testcase data.
+        Retrieve Testset metadata without Testcase data
 
         Parameters:
             - testset_id: int.
         ---
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
@@ -314,32 +333,43 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         name: str,
         description: typing.Optional[str] = OMIT,
-        using_retrieval: bool,
-        custom_schema: typing.Optional[CustomSchemaInput] = OMIT,
+        using_retrieval: typing.Optional[bool] = OMIT,
+        custom_schema: typing.Optional[CustomSchema] = OMIT,
     ) -> Testset:
         """
         Create a new Testset
 
         Parameters:
             - name: str.
 
             - description: typing.Optional[str].
 
-            - using_retrieval: bool.
+            - using_retrieval: typing.Optional[bool].
 
-            - custom_schema: typing.Optional[CustomSchemaInput].
+            - custom_schema: typing.Optional[CustomSchema].
+        ---
+        from scorecard.client import AsyncScorecard
+
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.testset.create(
+            name="name",
+        )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "using_retrieval": using_retrieval}
+        _request: typing.Dict[str, typing.Any] = {"name": name}
         if description is not OMIT:
             _request["description"] = description
+        if using_retrieval is not OMIT:
+            _request["using_retrieval"] = using_retrieval
         if custom_schema is not OMIT:
             _request["custom_schema"] = custom_schema
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/testset"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -357,38 +387,38 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_schema(self, testset_id: int) -> CustomSchemaOutput:
+    async def read_schema(self, testset_id: int) -> CustomSchema:
         """
-        Read the schema of a Testset.
+        Read the schema of a Testset
 
         Parameters:
             - testset_id: int.
         ---
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.testset.get_schema(
+        await client.testset.read_schema(
             testset_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/schema"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CustomSchemaOutput, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CustomSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
         if _response.status_code == 403:
             raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 422:
@@ -396,30 +426,39 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_testcases(
-        self, testset_id: int, *, page: typing.Optional[int] = None, page_size: typing.Optional[int] = None
+        self, testset_id: int, *, offset: typing.Optional[int] = None, limit: typing.Optional[int] = None
     ) -> PaginatedTestcaseResponse:
         """
         Retrieve all Testcases from a Testset
 
         Parameters:
             - testset_id: int.
 
-            - page: typing.Optional[int].
+            - offset: typing.Optional[int].
 
-            - page_size: typing.Optional[int].
+            - limit: typing.Optional[int].
+        ---
+        from scorecard.client import AsyncScorecard
+
+        client = AsyncScorecard(
+            api_key="YOUR_API_KEY",
+        )
+        await client.testset.get_testcases(
+            testset_id=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{testset_id}/testcase"),
-            params=remove_none_from_dict({"page": page, "page_size": page_size}),
+            params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTestcaseResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/__init__.py` & `scorecard_ai-0.2.0/src/scorecard/types/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .app_create_run_params import AppCreateRunParams
 from .app_test_record_create import AppTestRecordCreate
 from .app_test_set_create import AppTestSetCreate
-from .body_start_github_workflow_start_github_workflow_post import BodyStartGithubWorkflowStartGithubWorkflowPost
+from .create_github_workflow_params import CreateGithubWorkflowParams
 from .create_run_params import CreateRunParams
-from .custom_schema_input import CustomSchemaInput
-from .custom_schema_output import CustomSchemaOutput
+from .custom_schema import CustomSchema
 from .custom_variable import CustomVariable
 from .data_type_enum import DataTypeEnum
 from .execution_params import ExecutionParams
 from .file_url import FileUrl
+from .grade import Grade
 from .http_validation_error import HttpValidationError
-from .lib_dto_types_create_run_params import LibDtoTypesCreateRunParams
-from .lib_dto_types_test_record_create import LibDtoTypesTestRecordCreate
-from .lib_dto_types_test_set_create import LibDtoTypesTestSetCreate
+from .json_object import JsonObject
+from .json_object_input_value import JsonObjectInputValue
+from .json_object_output_value import JsonObjectOutputValue
 from .model_params import ModelParams
 from .not_found_error_body import NotFoundErrorBody
 from .paginated_testcase_response import PaginatedTestcaseResponse
 from .role_enum import RoleEnum
-from .run_external import RunExternal
+from .run import Run
 from .run_status import RunStatus
 from .score_execution_params import ScoreExecutionParams
+from .score_status import ScoreStatus
 from .scoring_params import ScoringParams
 from .test_case import TestCase
 from .test_case_create import TestCaseCreate
 from .test_case_create_input import TestCaseCreateInput
 from .test_case_custom_inputs_value import TestCaseCustomInputsValue
 from .test_case_custom_labels_value import TestCaseCustomLabelsValue
 from .test_record_create import TestRecordCreate
 from .test_set_create import TestSetCreate
 from .testrecord import Testrecord
 from .testrecord_custom_inputs_value import TestrecordCustomInputsValue
 from .testrecord_custom_labels_value import TestrecordCustomLabelsValue
 from .testrecord_custom_outputs_value import TestrecordCustomOutputsValue
+from .testrecord_model_debug_info_value import TestrecordModelDebugInfoValue
+from .testrecord_model_params_value import TestrecordModelParamsValue
 from .testset import Testset
 from .unauthenticated_error import UnauthenticatedError
 from .unauthorized_error_body import UnauthorizedErrorBody
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "AppCreateRunParams",
     "AppTestRecordCreate",
     "AppTestSetCreate",
-    "BodyStartGithubWorkflowStartGithubWorkflowPost",
+    "CreateGithubWorkflowParams",
     "CreateRunParams",
-    "CustomSchemaInput",
-    "CustomSchemaOutput",
+    "CustomSchema",
     "CustomVariable",
     "DataTypeEnum",
     "ExecutionParams",
     "FileUrl",
+    "Grade",
     "HttpValidationError",
-    "LibDtoTypesCreateRunParams",
-    "LibDtoTypesTestRecordCreate",
-    "LibDtoTypesTestSetCreate",
+    "JsonObject",
+    "JsonObjectInputValue",
+    "JsonObjectOutputValue",
     "ModelParams",
     "NotFoundErrorBody",
     "PaginatedTestcaseResponse",
     "RoleEnum",
-    "RunExternal",
+    "Run",
     "RunStatus",
     "ScoreExecutionParams",
+    "ScoreStatus",
     "ScoringParams",
     "TestCase",
     "TestCaseCreate",
     "TestCaseCreateInput",
     "TestCaseCustomInputsValue",
     "TestCaseCustomLabelsValue",
     "TestRecordCreate",
     "TestSetCreate",
     "Testrecord",
     "TestrecordCustomInputsValue",
     "TestrecordCustomLabelsValue",
     "TestrecordCustomOutputsValue",
+    "TestrecordModelDebugInfoValue",
+    "TestrecordModelParamsValue",
     "Testset",
     "UnauthenticatedError",
     "UnauthorizedErrorBody",
     "ValidationError",
     "ValidationErrorLocItem",
 ]
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/create_run_params.py` & `scorecard_ai-0.2.0/src/scorecard/types/unauthenticated_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CreateRunParams(pydantic.BaseModel):
-    testset_id: int
-    scoring_config_id: int
-    status: typing.Optional[str]
-    model_params: typing.Optional[typing.Dict[str, typing.Any]]
+class UnauthenticatedError(pydantic.BaseModel):
+    error: typing.Optional[str]
+    error_description: typing.Optional[str]
+    status_code: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/custom_schema_input.py` & `scorecard_ai-0.2.0/src/scorecard/types/custom_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CustomSchemaInput(pydantic.BaseModel):
+class CustomSchema(pydantic.BaseModel):
     """
     Custom schema model with an ordered list of custom variables.
     """
 
     variables: typing.Optional[typing.List[CustomVariable]] = pydantic.Field(
         description="Ordered list of custom variables"
     )
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/custom_schema_output.py` & `scorecard_ai-0.2.0/src/scorecard/types/custom_variable.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .custom_variable import CustomVariable
+from .data_type_enum import DataTypeEnum
+from .role_enum import RoleEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CustomSchemaOutput(pydantic.BaseModel):
+class CustomVariable(pydantic.BaseModel):
     """
-    Custom schema model with an ordered list of custom variables.
+    Custom variable model with name, description, role and data type.
     """
 
-    variables: typing.Optional[typing.List[CustomVariable]] = pydantic.Field(
-        description="Ordered list of custom variables"
-    )
+    name: str
+    description: typing.Optional[str]
+    role: RoleEnum
+    data_type: DataTypeEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/custom_variable.py` & `scorecard_ai-0.2.0/src/scorecard/types/unauthorized_error_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .data_type_enum import DataTypeEnum
-from .role_enum import RoleEnum
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CustomVariable(pydantic.BaseModel):
-    """
-    Custom variable model with name, description, role and data type.
-    """
-
-    name: str
-    description: typing.Optional[str]
-    role: RoleEnum
-    data_type: DataTypeEnum
+class UnauthorizedErrorBody(pydantic.BaseModel):
+    error: typing.Optional[str]
+    error_description: typing.Optional[str]
+    status_code: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/data_type_enum.py` & `scorecard_ai-0.2.0/src/scorecard/types/data_type_enum.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/file_url.py` & `scorecard_ai-0.2.0/src/scorecard/types/file_url.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/http_validation_error.py` & `scorecard_ai-0.2.0/src/scorecard/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/not_found_error_body.py` & `scorecard_ai-0.2.0/src/scorecard/types/not_found_error_body.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/paginated_testcase_response.py` & `scorecard_ai-0.2.0/src/scorecard/types/paginated_testcase_response.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/role_enum.py` & `scorecard_ai-0.2.0/src/scorecard/types/role_enum.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/run_external.py` & `scorecard_ai-0.2.0/src/scorecard/types/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class RunExternal(pydantic.BaseModel):
+class Run(pydantic.BaseModel):
     id: typing.Optional[int]
     created_at: typing.Optional[dt.datetime]
     updated_at: typing.Optional[dt.datetime]
     execution_start_time: typing.Optional[dt.datetime]
     execution_end_time: typing.Optional[dt.datetime]
     testset_id: typing.Optional[int]
     status: typing.Optional[str]
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/run_status.py` & `scorecard_ai-0.2.0/src/scorecard/types/run_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 
 class RunStatus(str, enum.Enum):
     PENDING = "pending"
     AWAITING_EXECUTION = "awaiting_execution"
     RUNNING_EXECUTION = "running_execution"
     AWAITING_SCORING = "awaiting_scoring"
     RUNNING_SCORING = "running_scoring"
+    AWAITING_HUMAN_SCORING = "awaiting_human_scoring"
     COMPLETED = "completed"
 
     def visit(
         self,
         pending: typing.Callable[[], T_Result],
         awaiting_execution: typing.Callable[[], T_Result],
         running_execution: typing.Callable[[], T_Result],
         awaiting_scoring: typing.Callable[[], T_Result],
         running_scoring: typing.Callable[[], T_Result],
+        awaiting_human_scoring: typing.Callable[[], T_Result],
         completed: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is RunStatus.PENDING:
             return pending()
         if self is RunStatus.AWAITING_EXECUTION:
             return awaiting_execution()
         if self is RunStatus.RUNNING_EXECUTION:
             return running_execution()
         if self is RunStatus.AWAITING_SCORING:
             return awaiting_scoring()
         if self is RunStatus.RUNNING_SCORING:
             return running_scoring()
+        if self is RunStatus.AWAITING_HUMAN_SCORING:
+            return awaiting_human_scoring()
         if self is RunStatus.COMPLETED:
             return completed()
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/test_case.py` & `scorecard_ai-0.2.0/src/scorecard/types/test_case.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/test_case_create.py` & `scorecard_ai-0.2.0/src/scorecard/types/test_case_create.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/test_record_create.py` & `scorecard_ai-0.2.0/src/scorecard/types/json_object.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TestRecordCreate(pydantic.BaseModel):
-    run_id: int
-    testcase_id: int
-    model_response: str
-    user_query: typing.Optional[str]
-    context: typing.Optional[str]
-    prompt: typing.Optional[str]
-    ideal: typing.Optional[str]
-    debug_output: typing.Optional[str]
-    model_params: typing.Optional[typing.Dict[str, typing.Any]]
-    testset_id: typing.Optional[int]
-    status: typing.Optional[str]
+class JsonObject(pydantic.BaseModel):
+    value: typing.Optional[JsonObjectOutputValue] = pydantic.Field(
+        description="The value of the JSON object, which can be a dictionary, list, string, integer, float, boolean, or None."
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .json_object_output_value import JsonObjectOutputValue  # noqa: E402
+
+JsonObject.update_forward_refs()
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/testrecord.py` & `scorecard_ai-0.2.0/src/scorecard/types/testrecord.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,34 +3,41 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .testrecord_custom_inputs_value import TestrecordCustomInputsValue
 from .testrecord_custom_labels_value import TestrecordCustomLabelsValue
 from .testrecord_custom_outputs_value import TestrecordCustomOutputsValue
+from .testrecord_model_debug_info_value import TestrecordModelDebugInfoValue
+from .testrecord_model_params_value import TestrecordModelParamsValue
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class Testrecord(pydantic.BaseModel):
     id: typing.Optional[int]
     created_at: typing.Optional[dt.datetime]
-    run_id: int
-    testset_id: int
-    user_query: str
+    run_id: typing.Optional[int]
+    testset_id: typing.Optional[int]
+    testcase_id: typing.Optional[int]
+    user_query: typing.Optional[str]
     context: typing.Optional[str]
     model_response: typing.Optional[str]
     ideal: typing.Optional[str]
     full_prompt: typing.Optional[str]
     custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomInputsValue]]]
     custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomLabelsValue]]]
     custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomOutputsValue]]]
+    status: typing.Optional[str]
+    prompt: typing.Optional[str]
+    model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelParamsValue]]]
+    model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelDebugInfoValue]]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/testset.py` & `scorecard_ai-0.2.0/src/scorecard/types/testset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .custom_schema_output import CustomSchemaOutput
+from .custom_schema import CustomSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
@@ -20,15 +20,15 @@
     using_retrieval: typing.Optional[bool]
     ingestion_method: typing.Optional[str]
     num_testcases: typing.Optional[int]
     published: typing.Optional[bool]
     updated_at: typing.Optional[dt.datetime]
     is_archived: typing.Optional[bool]
     project_id: typing.Optional[int]
-    custom_schema: typing.Optional[CustomSchemaOutput]
+    custom_schema: typing.Optional[CustomSchema]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `scorecard_ai-0.1.8/src/scorecard/types/unauthenticated_error.py` & `scorecard_ai-0.2.0/src/scorecard/types/validation_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .validation_error_loc_item import ValidationErrorLocItem
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UnauthenticatedError(pydantic.BaseModel):
-    error: typing.Optional[str]
-    error_description: typing.Optional[str]
-    status_code: typing.Optional[int]
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `scorecard_ai-0.1.8/PKG-INFO` & `scorecard_ai-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard-ai
-Version: 0.1.8
+Version: 0.2.0
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

