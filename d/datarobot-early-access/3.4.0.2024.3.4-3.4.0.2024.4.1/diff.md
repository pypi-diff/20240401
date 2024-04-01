# Comparing `tmp/datarobot_early_access-3.4.0.2024.3.4.tar.gz` & `tmp/datarobot_early_access-3.4.0.2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.4.0.2024.3.4.tar", last modified: Mon Mar  4 16:46:50 2024, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.4.0.2024.4.1.tar", last modified: Mon Apr  1 16:47:17 2024, max compression
```

## Comparing `datarobot_early_access-3.4.0.2024.3.4.tar` & `datarobot_early_access-3.4.0.2024.4.1.tar`

### file list

```diff
@@ -1,208 +1,215 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   207796 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2443 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20584 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/chunking_service.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/custom_jobs/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      344 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/custom_jobs/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12958 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/custom_jobs/custom_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9983 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/custom_jobs/custom_job_run.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/data_matching.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10144 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/enums.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16560 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/chat_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9371 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/comparison_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2017 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/custom_model_llm_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7979 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/custom_model_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9846 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/llm.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21283 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/llm_blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6886 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/playground.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/user_limits.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25744 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/vector_database.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/incremental_learning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5778 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/key_values.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    29350 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/recipe_operations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/recipes.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/config.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    31376 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      164 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9107 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/base.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1409 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1622 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/shap_preview.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4284 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86009 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19540 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33397 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59840 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      417 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/challenger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   114986 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/sharing.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   305945 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/common.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/registered_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/registered_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   223790 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    56833 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24583 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-03-04 16:46:15.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7248 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-03-04 16:46:50.000000 datarobot_early_access-3.4.0.2024.3.4/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-03-04 16:46:16.000000 datarobot_early_access-3.4.0.2024.3.4/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   221774 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2535 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25506 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/chunking_service.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11572 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/enums.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5661 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23220 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5939 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13717 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1818 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15666 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22662 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6886 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26323 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/incremental_learning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    29350 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-04-01 16:46:25.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/config.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32947 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9262 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/base.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2698 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1409 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1622 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_preview.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4351 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32414 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    61948 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/challenger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/champion_model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57730 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/custom_metrics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_exports.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/sharing.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11232 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/key_values.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   305975 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/common.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/recommended_model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job_run.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/runtime_parameters.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:46:28.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7487 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-04-01 16:47:16.000000 datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-04-01 16:47:17.000000 datarobot_early_access-3.4.0.2024.4.1/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-04-01 16:46:26.000000 datarobot_early_access-3.4.0.2024.4.1/setup_weekly.py
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/CHANGES.rst` & `datarobot_early_access-3.4.0.2024.4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,23 @@
         - :meth:`DatasetChunkDefinition.get <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to get a specific dataset chunk definition.
         - :meth:`DatasetChunkDefinition.list <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get>` to list all dataset chunk definitions.
         - :meth:`DatasetChunkDefinition.get_datasource_definition <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_datasource_definition>` to retrieve the data source definition.
         - :meth:`DatasetChunkDefinition.get_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.get_chunk>` to get specific chunk metadata belonging to a dataset chunk definition.
         - :meth:`DatasetChunkDefinition.list_chunks <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.list_chunks>` to list all chunk metadata belonging to a dataset chunk definition.
         - :meth:`DatasetChunkDefinition.create_chunk <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk>` to submit a job to retrieve the data from the origin data source.
         - :meth:`DatasetChunkDefinition.create_chunk_by_index <datarobot._experimental.models.chunking_service.DatasetChunkDefinition.create_chunk_by_index>` to submit a job to retrieve data from the origin data source by index.
-    - :class:`ChunkingServiceStorageKind <datarobot._experimental.models.chunking_service.StorageKind>`
+    - :class:`OriginStorageType <datarobot._experimental.models.chunking_service.OriginStorageType>`
     - :class:`Chunk <datarobot._experimental.models.chunking_service.Chunk>`
-    - :class:`ExternalStorageType <datarobot._experimental.models.chunking_service.ExternalStorageType>`
-    - :class:`ExternalStorage <datarobot._experimental.models.chunking_service.ExternalStorage>`
+    - :class:`ChunkStorageType <datarobot._experimental.models.chunking_service.ChunkStorageType>`
+    - :class:`ChunkStorage <datarobot._experimental.models.chunking_service.ChunkStorage>`
     - :class:`DatasourceDefinition <datarobot._experimental.models.chunking_service.DatasourceDefinition>`
+    - :class:`DatasourceAICatalogInfo <datarobot._experimental.models.chunking_service.DatasourceAICatalogInfo>` to define the datasource AI catalog information to create a new dataset chunk definition.
+    - :class:`DatasourceDataWarehouseInfo <datarobot._experimental.models.chunking_service.DatasourceDataWarehouseInfo>` to define the datasource data warehouse (snowflake, big query, etc) information to create a new dataset chunk definition.
+    - :class:`RuntimeParameter <datarobot.models.custom_model_version.RuntimeParameter>` for retrieving runtime parameters assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+    - :class:`RuntimeParameterValue <datarobot.models.custom_model_version.RuntimeParameterValue>` to define runtime parameter override value, to be assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
 
 - Added Snowflake Key Pair authentication for uploading datasets from Snowflake or creating a project from Snowflake data
 - Added :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>` to retrieve models.
   Method :meth:`Project.get_models <datarobot.models.Project.get_models>` is deprecated and will be removed soon in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
 - Extended the advanced options available when setting a target to include new
   parameter: 'chunkDefinitionId'(part of the AdvancedOptions object). This parameter allows you to specify the chunking definition needed for incremental learning automation.
 - Extended the advanced options available when setting a target to include new Autopilot
@@ -54,30 +58,79 @@
   :meth:`Challenger.get <datarobot.models.deployment.challenger.Challenger.get>` to retrieve challenger objects by ID.
   :meth:`Challenger.list <datarobot.models.deployment.challenger.Challenger.list>` to list all challengers.
   :meth:`Challenger.create <datarobot.models.deployment.challenger.Challenger.create>` to create a new challenger.
   :meth:`Challenger.update <datarobot.models.deployment.challenger.Challenger.update>` to update a challenger.
   :meth:`Challenger.delete <datarobot.models.deployment.challenger.Challenger.delete>` to delete a challenger.
 - Added a new method :meth:`Deployment.get_challenger_replay_settings <datarobot.models.Deployment.get_challenger_replay_settings>` to retrieve the challenger replay settings of a deployment.
 - Added a new method :meth:`Deployment.list_challengers <datarobot.models.Deployment.list_challengers>` to retrieve the challengers of a deployment.
+- Added a new method :meth:`Deployment.get_champion_model_package <datarobot.models.Deployment.get_champion_model_package>` to retrieve the champion model package from a deployment.
+- Added a new method :meth:`Deployment.list_prediction_data_exports <datarobot.models.Deployment.list_prediction_data_exports>` to retrieve deployment prediction data exports.
+- Added a new method :meth:`Deployment.list_actuals_data_exports <datarobot.models.Deployment.list_actuals_data_exports>` to retrieve deployment actuals data exports.
+- Added a new method :meth:`Deployment.list_training_data_exports <datarobot.models.Deployment.list_training_data_exports>` to retrieve deployment training data exports.
+- Manage deployment health settings with the following methods:
+    - Get health settings :meth:`Deployment.get_health_settings <datarobot.models.Deployment.get_health_settings>`
+    - Update health settings :meth:`Deployment.update_health_settings <datarobot.models.Deployment.update_health_settings>`
+    - Get default health settings :meth:`Deployment.get_default_health_settings <datarobot.models.Deployment.get_default_health_settings>`
 - Added new enum value to ``datarobot.enums._SHARED_TARGET_TYPE`` to support Text Generation use case.
 - Added new enum value ``datarobotServerless`` to ``datarobot.enums.PredictionEnvironmentPlatform`` to support DataRobot Serverless prediction environments.
+- Added new enum value ``notApplicable`` to ``datarobot.enums.PredictionEnvironmentHealthType`` to support new health status from DataRobot API.
+- Added a new enum value to ``datarobot.enums.TARGET_TYPE`` and ``datarobot.enums.CUSTOM_MODEL_TARGET_TYPE`` to support text generation custom inference models.
+- Updated ``datarobot.CustomModel`` to support the creation of text generation custom models.
+- Added a new class :class:`CustomMetric <datarobot.models.deployment.custom_metrics.CustomMetric>` for interacting with DataRobot custom metrics to support the following methods:
+  :meth:`CustomMetric.get <datarobot.models.deployment.custom_metrics.CustomMetric.get>` to retrieve a custom metric object by ID from a given deployment.
+  :meth:`CustomMetric.list <datarobot.models.deployment.custom_metrics.CustomMetric.list>` to list all custom metrics from a given deployment.
+  :meth:`CustomMetric.create <datarobot.models.deployment.custom_metrics.CustomMetric.create>` to create a new custom metric for a given deployment.
+  :meth:`CustomMetric.update <datarobot.models.deployment.custom_metrics.CustomMetric.update>` to update a custom metric for a given deployment.
+  :meth:`CustomMetric.delete <datarobot.models.deployment.custom_metrics.CustomMetric.delete>` to delete a custom metric for a given deployment.
+  :meth:`CustomMetric.unset_baseline <datarobot.models.deployment.custom_metrics.CustomMetric.unset_baseline>` to remove baseline for a given custom metric.
+  :meth:`CustomMetric.submit_values <datarobot.models.deployment.custom_metrics.CustomMetric.submit_values>` to submit aggregated custom metrics values from code. The provided data should be in the form of a dict or a Pandas DataFrame.
+  :meth:`CustomMetric.report_single_value <datarobot.models.deployment.custom_metrics.CustomMetric.report_single_value>` to submit a single custom metric value.
+  :meth:`CustomMetric.submit_values_from_catalog <datarobot.models.deployment.custom_metrics.CustomMetric.submit_values_from_catalog>` to submit aggregated custom metrics values from a dataset via the AI Catalog.
+  :meth:`CustomMetric.get_values_over_time <datarobot.models.deployment.custom_metrics.CustomMetric.get_values_over_time>` to retrieve values of a custom metric over a time period.
+  :meth:`CustomMetric.get_summary <datarobot.models.deployment.custom_metrics.CustomMetric.get_summary>` to retrieve the summary of a custom metric over a time period.
+  :meth:`CustomMetric.get_values_over_batch <datarobot.models.deployment.custom_metrics.CustomMetric.get_values_over_batch>` to retrieve values of a custom metric over batches.
+  :meth:`CustomMetric.get_batch_summary <datarobot.models.deployment.custom_metrics.CustomMetric.get_batch_summary>` to retrieve the summary of a custom metric over batches.
+- Added :class:`CustomMetricValuesOverTime <datarobot.models.deployment.custom_metrics.CustomMetricValuesOverTime>` to retrieve custom metric over time information.
+- Added :class:`CustomMetricSummary <datarobot.models.deployment.custom_metrics.CustomMetricSummary>` to retrieve custom metric over time summary.
+- Added :class:`CustomMetricValuesOverBatch <datarobot.models.deployment.custom_metrics.CustomMetricValuesOverBatch>` to retrieve custom metric over batch information.
+- Added :class:`CustomMetricBatchSummary <datarobot.models.deployment.custom_metrics.CustomMetricBatchSummary>` to retrieve custom metric batch summary.
+- Added :class:`Job <datarobot.models.registry.job.Job>` and  :class:`JobRun <datarobot.models.registry.job_run.JobRun>`  to create, read, update, run, and delete jobs in the Registry.
+- Added :class:`KeyValue <datarobot.models.key_values.KeyValue>` to create, read, update, and delete key values.
+- Added a new class :class:`PredictionDataExport <datarobot.models.deployment.data_exports.PredictionDataExport>` for interacting with DataRobot deployment data export to support the following methods:
+  :meth:`PredictionDataExport.get <datarobot.models.deployment.data_exports.PredictionDataExport.get>` to retrieve a prediction data export object by ID from a given deployment.
+  :meth:`PredictionDataExport.list <datarobot.models.deployment.data_exports.PredictionDataExport.list>` to list all prediction data exports from a given deployment.
+  :meth:`PredictionDataExport.create <datarobot.models.deployment.data_exports.PredictionDataExport.create>` to create a new prediction data export for a given deployment.
+  :meth:`PredictionDataExport.fetch_data <datarobot.models.deployment.data_exports.PredictionDataExport.fetch_data>` to retrieve a prediction export data as a DataRobot dataset.
+- Added a new class :class:`ActualsDataExport <datarobot.models.deployment.data_exports.ActualsDataExport>` for interacting with DataRobot deployment data export to support the following methods:
+  :meth:`ActualsDataExport.get <datarobot.models.deployment.data_exports.ActualsDataExport.get>` to retrieve an actuals data export object by ID from a given deployment.
+  :meth:`ActualsDataExport.list <datarobot.models.deployment.data_exports.ActualsDataExport.list>` to list all actuals data exports from a given deployment.
+  :meth:`ActualsDataExport.create <datarobot.models.deployment.data_exports.ActualsDataExport.create>` to create a new actuals data export for a given deployment.
+  :meth:`ActualsDataExport.fetch_data <datarobot.models.deployment.data_exports.ActualsDataExport.fetch_data>` to retrieve an actuals export data  as a DataRobot dataset.
+- Added a new class :class:`TrainingDataExport <datarobot.models.deployment.data_exports.TrainingDataExport>` for interacting with DataRobot deployment data export to support the following methods:
+  :meth:`TrainingDataExport.get <datarobot.models.deployment.data_exports.TrainingDataExport.get>` to retrieve a training data export object by ID from a given deployment.
+  :meth:`TrainingDataExport.list <datarobot.models.deployment.data_exports.TrainingDataExport.list>` to list all training data exports from a given deployment.
+  :meth:`TrainingDataExport.create <datarobot.models.deployment.data_exports.TrainingDataExport.create>` to create a new training data export for a given deployment.
+  :meth:`TrainingDataExport.fetch_data <datarobot.models.deployment.data_exports.TrainingDataExport.fetch_data>` to retrieve a training export data as a DataRobot dataset.
+
+Key Changes
+  1.	Parameter Overrides: Users can now override most of the previously set configuration values directly through parameters when initializing the Client.
+  2.	Exceptions: The endpoint and token values must be initiated from one source(client params, environment, or config file) and cannot be overridden individually for security and consistency reasons.
 
-  Key Changes
-	1.	Parameter Overrides: Users can now override most of the previously set configuration values directly through parameters when initializing the Client.
-	2.	Exceptions: The endpoint and token values must be initiated from one source(client params, environments, or config file) and cannot be overridden individually for security and consistency reasons.
-
-  Configuration Priority:
+Configuration Priority:
   1.	Client Params
-  2.  Client config_path param
-  2.	Environment Variables
-  3.	Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
+  2.    Client config_path param
+  3.	Environment Variables
+  4.	Default to reading YAML config file from `~/.config/datarobot/drconfig.yaml`
 
 - `DATAROBOT_API_CONSUMER_TRACKING_ENABLED` now always defaults to `True` in all cases.
-- Added Databricks service principal and personal access token authentication for uploading datasets from Databricks or creating a project from Databricks data.
+- Added Databricks personal access token and service principal (also shared credentials via secure config) authentication for uploading datasets from Databricks or creating a project from Databricks data.
+- Added secure config support for AWS long term credentials.
 - Implemented support for `dr-database-v1` to `DataStore <datarobot.models.DataStore>`, `DataSource <datarobot.models.DataStore>`, and  `DataDriver <datarobot.models.DataDriver>.` Added enum classes to support the changes.
+- You can retrieve the canonical URI for a Use Case using :meth:`UseCase.get_uri <datarobot.UseCase.get_uri>`.
+- You can open a Use Case in a browser using :meth:`UseCase.open_in_browser <datarobot.UseCase.open_in_browser>`.
 
 Enhancements
 ************
 - Added a new parameter to :meth:`Dataset.create_from_url <datarobot.models.Dataset.create_from_url>` to support fast dataset registration:
     - `sample_size`
 - Added a new parameter to :meth:`Dataset.create_from_data_source <datarobot.models.Dataset.create_from_data_source>` to support fast dataset registration:
     - `sample_size`
@@ -102,17 +155,66 @@
 - Removed `Model.get_leaderboard_ui_permalink` and `Model.open_model_browser`
 - Deprecated :meth:`Project.get_models <datarobot.models.Project.get_models>` in favour of :meth:`Project.get_model_records <datarobot.models.Project.get_model_records>`.
 - :meth:`BatchPredictionJobDefinition.list <datarobot.models.BatchPredictionJobDefinition.list>` will no longer return all job definitions after version 3.6 is released.
   To preserve current behavior please pass limit=0.
 - `new_model_id` parameter in :meth:`Deployment.validate_replacement_model<datarobot.models.Deployment.validate_replacement_model>` will be removed after version 3.6 is released.
 - :meth:`Deployment.replace_model<datarobot.models.Deployment.replace_model>` will be removed after version 3.6 is released.
   Method :meth:`Deployment.perform_model_replace<datarobot.models.Deployment.perform_model_replace>` should be used instead.
+- Removed `CustomInferenceModel.assign_training_data`.
+  Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
+
+Documentation changes
+*********************
+- Updated `genai_example.rst` to utilize latest genAI features and methods introduced most recently in the API client.
 
 Experimental changes
 *********************
+- Added optional parameters, `use_case`, `name`, and `model` to :meth:`CustomModelValidation.create <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.create>`.
+- Added a method :meth:`CustomModelValidation.list <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.list>`, to list custom model validations available to a user with several optional parameters to filter the results.
+- Added a method :meth:`CustomModelValidation.update <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.update>`, to update a custom model validation.
+
+- Added an optional parameter, `use_case`, to :meth:`LLMDefinition.list <datarobot._experimental.models.genai.llm.LLMDefinition.list>`,
+  to include in the returned LLMs the external LLMs available for the specified `use_case` as well.
+
+- Added optional parameter, `playground` to :meth:`VectorDatabase.list <datarobot._experimental.models.genai.vector_database.VectorDatabase.list>`
+  to list vector databases by playground.
+
+- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.list <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.list>`, to list comparison prompts by comparison chat.
+- Added optional parameter, `comparison_chat`, to :meth:`ComparisonPrompt.create <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.create>`, to specify the comparison chat to create the comparison prompt in.
+- Added optional parameter, `feedback_result`, to :meth:`ComparisonPrompt.update <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.update>`, to update a comparison prompt with feedback.
+
+- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.update <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.update>`
+  to update the LLM Blueprint's starred status.
+- Added optional parameters, `is_starred` to :meth:`LLMBlueprint.list <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.list>`
+  to filter the returned LLM blueprints to those matching `is_starred`.
+
+- Added a new enum PromptType, :class:`PromptType <datarobot._experimental.models.enums.PromptType>` to identify the LLMBlueprint's prompting type.
+- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.create <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.create>`,
+  to specify the LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot._experimental.models.enums.PromptType>`.
+- Added optional parameters, `prompt_type` to :meth:`LLMBlueprint.update <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.update>`,
+  to specify the updated LLM Blueprint's prompting type. This can be set with :class:`PromptType <datarobot._experimental.models.enums.PromptType>`.
+
+- Added a new class, :class:`ComparisonChat <datarobot._experimental.models.genai.comparison_chat.ComparisonChat>`, for interacting with DataRobot generative AI comparison chats.
+  :meth:`ComparisonChat.get <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.get>` retrieves a comparison chat object by ID.
+  :meth:`ComparisonChat.list <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.list>` lists all comparison chats available to the user.
+  :meth:`ComparisonChat.create <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.create>` creates a new comparison chat.
+  :meth:`ComparisonChat.update <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.update>` updates the name of a comparison chat.
+  :meth:`ComparisonChat.delete <datarobot._experimental.models.genai.comparison_chat.ComparisonChat.delete>` deletes a single comparison chat.
+
+- Added optional parameters, `playground` and `chat` to :meth:`ChatPrompt.list <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.list>`, to list chat prompts by playground and chat.
+- Added optional parameter, `chat` to :meth:`ChatPrompt.create <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.create>`, to specify the chat to create the chat prompt in.
+- Added a new method, :meth:`ChatPrompt.update <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.update>`, to update a chat prompt with custom metrics and feedback.
+
+- Added a new class, :class:`Chat <datarobot._experimental.models.genai.chat.Chat>`, for interacting with DataRobot generative AI chats.
+  :meth:`Chat.get <datarobot._experimental.models.genai.chat.Chat.get>` retrieves a chat object by ID.
+  :meth:`Chat.list <datarobot._experimental.models.genai.chat.Chat.list>` lists all chats available to the user.
+  :meth:`Chat.create <datarobot._experimental.models.genai.chat.Chat.create>` creates a new chat.
+  :meth:`Chat.update <datarobot._experimental.models.genai.chat.Chat.update>` updates the name of a chat.
+  :meth:`Chat.delete <datarobot._experimental.models.genai.chat.Chat.delete>` deletes a single chat.
+
 - Removed the `model_package` module. Use :class:`RegisteredModelVersion <datarobot.models.RegisteredModelVersion>` instead.
 - Added new class :class:`UserLimits <datarobot._experimental.models.genai.user_limits.UserLimits>`
     - Added support to get the count of users' LLM API requests. :meth:`UserLimits.get_llm_requests_count <datarobot._experimental.models.genai.user_limits.UserLimits.get_llm_requests_count>`
     - Added support to get the count of users' vector databases. :meth:`UserLimits.get_vector_database_count <datarobot._experimental.models.genai.user_limits.UserLimits.get_vector_database_count>`
 - Added new methods to the class :class:`Notebook <datarobot._experimental.models.notebooks.Notebook>` which includes :meth:`Notebook.run <datarobot._experimental.models.notebooks.Notebook.run>` and :meth:`Notebook.download_revision <datarobot._experimental.models.notebooks.Notebook.download_revision>`. See the documentation for example usage.
 - Added new class :class:`NotebookScheduledJob <datarobot._experimental.models.notebooks.NotebookScheduledJob>`.
 - Added new class :class:`NotebookScheduledRun <datarobot._experimental.models.notebooks.NotebookScheduledRun>`.
@@ -245,15 +347,15 @@
   :meth:`ComparisonPrompt.update <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.update>` updates a comparison prompt.
   :meth:`ComparisonPrompt.delete <datarobot._experimental.models.genai.comparison_prompt.ComparisonPrompt.delete>` deletes a single comparison prompt.
 
 - Extended :class:`UseCase <datarobot.UseCase>`, adding two new fields to represent the count of vector databases and playgrounds.
 
 - Added a new method, :meth:`ChatPrompt.create_llm_blueprint <datarobot._experimental.models.genai.chat_prompt.ChatPrompt.create_llm_blueprint>`, to create an LLM blueprint from a chat prompt.
 
-- Added a new method, :meth:`CustomModelLLMValidation.delete <datarobot._experimental.models.genai.custom_model_llm_validation.CustomModelLLMValidation.delete>`, to delete a custom model LLM validation record.
+- Added a new method, :meth:`CustomModelLLMValidation.delete <datarobot._experimental.models.genai.custom_model_validation.CustomModelValidation.delete>`, to delete a custom model LLM validation record.
 
 - Added a new method, :meth:`LLMBlueprint.register_custom_model <datarobot._experimental.models.genai.llm_blueprint.LLMBlueprint.register_custom_model>`, for registering a custom model from a generative AI LLM blueprint.
 
 3.2.0
 =====
 
 New Features
@@ -432,15 +534,15 @@
   Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
 - ``DatetimeModel.get_or_request_feature_fit`` has been removed.
   Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
 - Deprecated the use of :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` in favor of :class:`SharingRole <datarobot.models.sharing.SharingRole>` for sharing in the following classes:
   - :meth:`DataStore.share <datarobot.DataStore.share>`
 - Deprecated the following methods for retrieving :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` information.
   - :meth:`DataStore.get_access_list <datarobot.DataStore.get_access_list>`. Please use :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>` instead.
-- :meth:`CustomInferenceModel.assign_training_data <datarobot.CustomInferenceModel.assign_training_data>` was marked as deprecated and will be removed in v3.4.
+- `CustomInferenceModel.assign_training_data` was marked as deprecated and will be removed in v3.4.
   Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
 
 Configuration Changes
 *********************
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
 Deprecation Summary
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/LICENSE.txt` & `datarobot_early_access-3.4.0.2024.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/PKG-INFO` & `datarobot_early_access-3.4.0.2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.4.0.2024.3.4
+Version: 3.4.0.2024.4.1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/README.md` & `datarobot_early_access-3.4.0.2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/common_setup.py` & `datarobot_early_access-3.4.0.2024.4.1/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/__init__.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # flake8: noqa
 from ._version import __version__
 from .client import Client
 from .context import Context
 from .enums import (
     AUTOPILOT_MODE,
+    KeyValueCategory,
+    KeyValueEntityType,
+    KeyValueType,
     NETWORK_EGRESS_POLICY,
     PredictionEnvironmentPlatform,
     QUEUE_STATUS,
     SCORING_TYPE,
     SNAPSHOT_POLICY,
     TARGET_TYPE,
     VERBOSITY_LEVEL,
@@ -69,14 +72,15 @@
     FeatureImpactJob,
     FeatureLineage,
     Featurelist,
     FrozenModel,
     ImportedModel,
     InteractionFeature,
     Job,
+    KeyValue,
     Model,
     ModelBlueprintChart,
     ModelingFeature,
     ModelingFeaturelist,
     ModelJob,
     ModelRecommendation,
     PayoffMatrix,
@@ -90,14 +94,15 @@
     PrimeFile,
     PrimeModel,
     Project,
     RatingTable,
     RatingTableModel,
     RegisteredModel,
     RegisteredModelVersion,
+    registry,
     RelationshipsConfiguration,
     Ruleset,
     SecondaryDatasetConfigurations,
     SegmentationTask,
     SegmentInfo,
     ShapImpact,
     ShapMatrix,
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_compat.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/chunking_service.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/chunking_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,55 +7,57 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
+import inspect
 from typing import Any, Dict, List, Optional, Union
 
 import trafaret as t
 
-from datarobot._experimental.models.enums import ExternalStorageType, StorageKind
+from datarobot._experimental.models.enums import ChunkStorageType, OriginStorageType
 from datarobot.enums import DEFAULT_MAX_WAIT
 from datarobot.models.api_object import APIObject
+from datarobot.utils import camelize
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
-class ExternalStorage(APIObject):
+class ChunkStorage(APIObject):
     """
-    The external storage location for the data chunks.
+    The chunk storage location for the data chunks.
 
     Attributes
     ----------
-     external_reference_id : str
+     storage_reference_id : str
         The ID of the storage entity.
-     external_storage_type : str
-        The type of external storage.
+     chunk_storage_type : str
+        The type of the chunk storage.
      version_id : str
         The catalog version ID. This will only be used if the storage type is "AI Catalog".
 
     """
 
     _converter = t.Dict(
         {
-            t.Key("external_reference_id"): t.String,
-            t.Key("external_storage_type"): t.String,
+            t.Key("storage_reference_id"): t.String,
+            t.Key("chunk_storage_type"): t.String,
             t.Key("version_id", optional=True): t.Or(t.String, t.Null),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
-        external_reference_id: str,
-        external_storage_type: str,
+        storage_reference_id: str,
+        chunk_storage_type: str,
         version_id: Optional[str] = None,
     ):
-        self.external_reference_id = external_reference_id
-        self.external_storage_type = external_storage_type
+        self.storage_reference_id = storage_reference_id
+        self.chunk_storage_type = chunk_storage_type
         self.version_id = version_id
 
 
 class Chunk(APIObject):
     """
     Data chunk object that holds metadata about a chunk.
 
@@ -69,108 +71,107 @@
         The number of rows in the chunk.
     offset : int
         The offset in the dataset to create the chunk.
     chunk_index : str
         The index of the chunk if chunks are divided uniformly. Otherwise, it is None.
     data_source_id : str
         The ID of the data request used to create the chunk.
-    external_storage : ExternalStorage
+    chunk_storage : ChunkStorage
         A list of storage locations where the chunk is stored.
 
     """
 
     _converter = t.Dict(
         {
             t.Key("id"): t.String,
             t.Key("chunk_definition_id"): t.String,
             t.Key("limit"): t.Int,
             t.Key("offset"): t.Int,
             t.Key("chunk_index", optional=True): t.Or(t.Int, t.Null),
             t.Key("data_source_id", optional=True): t.Or(t.String, t.Null),
-            t.Key("external_storage", optional=True): t.Or(
-                t.List(ExternalStorage._converter), t.Null
-            ),
+            t.Key("chunk_storage", optional=True): t.Or(t.List(ChunkStorage._converter), t.Null),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id: str,
         chunk_definition_id: str,
         limit: int,
         offset: int,
         chunk_index: Optional[int] = None,
         data_source_id: Optional[str] = None,
-        external_storage: Optional[List[ExternalStorage]] = None,
+        chunk_storage: Optional[List[ChunkStorage]] = None,
     ):
         self.id = id
         self.chunk_definition_id = chunk_definition_id
         self.chunk_index = chunk_index
         self.offset = offset
         self.limit = limit
         self.data_source_id = data_source_id
-        self.external_storage = external_storage
+        self.chunk_storage = chunk_storage
 
-    def get_external_storage_id(self, storage_type: ExternalStorageType) -> Optional[str]:
+    def get_chunk_storage_id(self, storage_type: ChunkStorageType) -> Optional[str]:
         """
-        Get external storage id for the chunk.
+        Get storage location ID for the chunk.
 
         Parameters
         ----------
-        storage_type: ExternalStorageType
-            The external storage type where the chunk is store.
+        storage_type: ChunkStorageType
+            The storage type where the chunk is stored.
 
         Returns
         -------
-        external_reference_id: str
-            An ID that references the external storage for the chunk.
+        storage_reference_id: str
+            An ID that references the storage location for the chunk.
 
         """
-        if self.external_storage is None:
+        if self.chunk_storage is None:
             return None
 
-        for external_storage in self.external_storage:
-            if isinstance(external_storage, Dict):
-                external_storage = ExternalStorage(**external_storage)
+        for chunk_storage in self.chunk_storage:
+            if isinstance(chunk_storage, Dict):
+                chunk_storage = ChunkStorage(**chunk_storage)
 
-            if external_storage.external_storage_type == storage_type:
-                return external_storage.external_reference_id
+            if chunk_storage.chunk_storage_type == storage_type:
+                return chunk_storage.storage_reference_id
         return None
 
-    def get_external_storage_version_id(self, storage_type: ExternalStorageType) -> Optional[str]:
+    def get_chunk_storage_version_id(self, storage_type: ChunkStorageType) -> Optional[str]:
         """
-        Get external storage version id for the chunk.
+        Get storage version ID for the chunk.
 
         Parameters
         ----------
-        storage_type: ExternalStorageType
-            The external storage type where the chunk is store.
+        storage_type: ChunkStorageType
+            The storage type where the chunk is stored.
 
         Returns
         -------
-        external_reference_id: str
-            A catalog version ID associated with AI Catalog dataset ID.
+        storage_reference_id: str
+            A catalog version ID associated with the AI Catalog dataset ID.
 
         """
-        if self.external_storage is None:
+        if self.chunk_storage is None:
             return None
 
-        for external_storage in self.external_storage:
-            if isinstance(external_storage, Dict):
-                external_storage = ExternalStorage(**external_storage)
+        for chunk_storage in self.chunk_storage:
+            if isinstance(chunk_storage, Dict):
+                chunk_storage = ChunkStorage(**chunk_storage)
 
-            if external_storage.external_storage_type == storage_type:
-                return external_storage.version_id
+            if chunk_storage.chunk_storage_type == storage_type:
+                return chunk_storage.version_id
         return None
 
 
 class DatasourceDefinition(APIObject):
     """
-    Data source definition that holds information data source.
-
+    Data source definition that holds information of data source for API responses.
+    Do not use this to 'create' DatasourceDefinition objects directly, use
+    DatasourceAICatalogInfo and DatasourceDataWarehouseInfo.
 
      Attributes
      ----------
      id : str
          The ID of the data source definition.
      data_store_id : str
          The ID of the data store.
@@ -178,76 +179,238 @@
         The ID of the credentials.
      table : str
          The data source table name.
      schema : str
          The offset into the dataset to create the chunk.
      catalog : str
          The database or catalog name.
-     storage_kind : str
+     storage_origin : str
          The origin data source or data warehouse (e.g., Snowflake, BigQuery).
      data_source_id : str
          The ID of the data request used to generate sampling and metadata.
      total_rows : str
          The total number of rows in the dataset.
      source_size : str
          The size of the dataset.
      estimated_size_per_row : str
          The estimated size per row.
      columns : str
          The list of column names in the dataset.
+     order_by_columns : List[str]
+         A list of columns used to sort the dataset.
+     select_columns : List[str]
+         A list of columns to select from the dataset.
 
     """
 
     _converter = t.Dict(
         {
             t.Key("id"): t.String,
-            t.Key("data_store_id"): t.String,
-            t.Key("credentials_id"): t.String,
-            t.Key("table"): t.String,
-            t.Key("schema"): t.String,
-            t.Key("catalog"): t.String,
-            t.Key("storage_kind"): t.String,
+            t.Key("data_store_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("credentials_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("table", optional=True): t.Or(t.String, t.Null),
+            t.Key("schema", optional=True): t.Or(t.String, t.Null),
+            t.Key("catalog", optional=True): t.Or(t.String, t.Null),
+            t.Key("storage_origin"): t.String,
             t.Key("name", optional=True): t.Or(t.String, t.Null),
             t.Key("data_source_id", optional=True): t.Or(t.String, t.Null),
             t.Key("total_rows", optional=True): t.Or(t.Int, t.Null),
             t.Key("source_size", optional=True): t.Or(t.Int, t.Null),
             t.Key("estimated_size_per_row", optional=True): t.Or(t.Int, t.Null),
             t.Key("columns", optional=True): t.Or(t.List(t.String), t.Null),
+            t.Key("catalog_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("catalog_version_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("order_by_columns"): t.List(t.String, min_length=0),
+            t.Key("select_columns", optional=True): t.Or(t.List(t.String), t.Null),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id: str,
-        data_store_id: str,
-        credentials_id: str,
-        table: str,
-        schema: str,
-        catalog: str,
-        storage_kind: StorageKind,
+        storage_origin: OriginStorageType,
+        order_by_columns: Optional[List[str]] = None,
+        table: Optional[str] = None,
+        data_store_id: Optional[str] = None,
+        credentials_id: Optional[str] = None,
+        schema: Optional[str] = None,
+        catalog: Optional[str] = None,
         name: Optional[str] = None,
         data_source_id: Optional[str] = None,
         total_rows: Optional[int] = None,
         source_size: Optional[int] = None,
         estimated_size_per_row: Optional[int] = None,
         columns: Optional[List[str]] = None,
+        catalog_id: Optional[str] = None,
+        catalog_version_id: Optional[str] = None,
+        select_columns: Optional[List[str]] = None,
     ):
         self.id = id
         self.name = name
         self.data_store_id = data_store_id
         self.credentials_id = credentials_id
         self.table = table
         self.schema = schema
         self.catalog = catalog
-        self.storage_kind = storage_kind
+        self.storage_origin = storage_origin
         self.data_source_id = data_source_id
         self.total_rows = total_rows
         self.source_size = source_size
         self.estimated_size_per_row = estimated_size_per_row
         self.columns = columns
+        self.catalog_id = catalog_id
+        self.catalog_version_id = catalog_version_id
+        self.order_by_columns = [] if order_by_columns is None else order_by_columns
+        self.select_columns = select_columns
+
+
+class DatasourceDataWarehouseInfo(APIObject):
+    """
+    Data source information used at creation time with dataset chunk definition.
+    Data warehouses supported: Snowflake, BigQuery, Databricks
+
+
+    Attributes
+    ----------
+    name: str
+        The optional custom name of the data source.
+    table : str
+        The data source table name or AI Catalog dataset name.
+    storage_origin : str
+        The origin data source or data warehouse (e.g., Snowflake, BigQuery).
+    data_store_id : str
+        The ID of the data store.
+    credentials_id : str
+        The ID of the credentials.
+    schema : str
+        The offset into the dataset to create the chunk.
+    catalog : str
+        The database or catalog name.
+    data_source_id : str
+        The ID of the data request used to generate sampling and metadata.
+    order_by_columns : List[str]
+        A list of columns used to sort the dataset.
+    select_columns: List[str]
+        A list of columns to select from the dataset.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("data_store_id"): t.String,
+            t.Key("credentials_id"): t.String,
+            t.Key("table"): t.String,
+            t.Key("order_by_columns"): t.List(t.String),
+            t.Key("storage_origin"): t.Enum(
+                OriginStorageType.SNOWFLAKE,
+                OriginStorageType.BIGQUERY,
+                OriginStorageType.AI_CATALOG,
+                OriginStorageType.DATABRICKS,
+            ),
+            t.Key("schema", optional=True): t.Or(t.String, t.Null),
+            t.Key("catalog", optional=True): t.Or(t.String, t.Null),
+            t.Key("name", optional=True): t.Or(t.String, t.Null),
+            t.Key("data_source_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("select_columns", optional=True): t.Or(t.List(t.String), t.Null),
+        }
+    )
+
+    def __init__(
+        self,
+        data_store_id: str,
+        credentials_id: str,
+        table: str,
+        storage_origin: OriginStorageType,
+        order_by_columns: List[str],
+        schema: Optional[str] = None,
+        catalog: Optional[str] = None,
+        name: Optional[str] = None,
+        data_source_id: Optional[str] = None,
+        select_columns: Optional[List[str]] = None,
+    ):
+        self.name = name
+        self.data_store_id = data_store_id
+        self.credentials_id = credentials_id
+        self.table = table
+        self.schema = schema
+        self.catalog = catalog
+        self.storage_origin = storage_origin
+        self.data_source_id = data_source_id
+        self.order_by_columns = order_by_columns
+        self.select_columns = select_columns
+        self._converter.check(self.to_dict())
+
+    def to_dict(self) -> Dict[str, Any]:
+        self_dict = {
+            attr[0]: attr[1]
+            for attr in inspect.getmembers(self)
+            if (not attr[0].startswith("_") and not inspect.ismethod(attr[1]))
+        }
+        return self_dict
+
+
+class DatasourceAICatalogInfo(APIObject):
+    """
+    AI Catalog data source information used at creation time with dataset chunk definition.
+
+
+    Attributes
+    ----------
+    name: str
+        The optional custom name of the data source.
+    table : str
+        The data source table name or AI Catalog dataset name.
+    storage_origin : str
+        The origin data source, always AI Catalog type.
+    catalog_id : str
+        The ID of the AI Catalog dataset.
+    catalog_version_id : str
+        The ID of the AI Catalog dataset version.
+    order_by_columns : List[str]
+        A list of columns used to sort the dataset.
+    select_columns: List[str]
+        A list of columns to select from the dataset.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("catalog_version_id"): t.String,
+            t.Key("catalog_id", optional=True): t.Or(t.String, t.Null),
+            t.Key("storage_origin"): t.Atom(OriginStorageType.AI_CATALOG),
+            t.Key("table", optional=True): t.Or(t.String, t.Null),
+            t.Key("name", optional=True): t.Or(t.String, t.Null),
+            t.Key("order_by_columns", optional=True): t.List(t.String, min_length=0),
+            t.Key("select_columns", optional=True): t.Or(t.List(t.String), t.Null),
+        }
+    )
+
+    def __init__(
+        self,
+        catalog_version_id: str,
+        catalog_id: Optional[str] = None,
+        table: Optional[str] = None,
+        name: Optional[str] = None,
+        order_by_columns: Optional[List[str]] = None,
+        select_columns: Optional[List[str]] = None,
+    ):
+        self.name = name
+        self.catalog_version_id = catalog_version_id
+        self.catalog_id = catalog_id
+        self.table = table
+        self.storage_origin = OriginStorageType.AI_CATALOG
+        self.order_by_columns = [] if order_by_columns is None else order_by_columns
+        self.select_columns = select_columns
+        self._converter.check(self.to_dict())
+
+    def to_dict(self) -> Dict[str, Any]:
+        self_dict = {
+            attr[0]: attr[1]
+            for attr in inspect.getmembers(self)
+            if (not attr[0].startswith("_") and not inspect.ismethod(attr[1]))
+        }
+        return self_dict
 
 
 class DatasetChunkDefinition(APIObject):
     """
     Dataset chunking definition that holds information about how to chunk the dataset.
 
      Attributes
@@ -256,26 +419,18 @@
         The ID of the dataset chunk definition.
     user_id : str
         The ID of the user who created the definition.
     name : str
         The name of the dataset chunk definition.
     project_starter_chunk_size : int
         The size, in bytes, of the project starter chunk.
-    order_by_columns : List[str]
-        A list of columns used to sort the dataset.
+    user_chunk_size : int
+        Chunk size in bytes.
     datasource_definition_id : str
-        The datasource definition ID associated with the dataset chunk definition.
-    storage_kind : str
-        The origin data source or data warehouse e.g. Snowflake, BigQuery.
-    data_source_id : str
-        The ID of the data request used to generate sampling and metadata.
-    filter_id : str
-       The ID of the filter.
-    columns_to_select : List[str]
-        A list of columns to select from the dataset.
+        The data source definition ID associated with the dataset chunk definition.
 
     """
 
     _path = "datasetChunkDefinitions/"
     _path_with_id = _path + "{}/"
     _path_datasource = _path + "{}/datasourceDefinition/"
     _path_chunks = _path + "{}/chunks/"
@@ -284,42 +439,33 @@
     _converter = t.Dict(
         {
             t.Key("id"): t.String,
             t.Key("user_id"): t.String,
             t.Key("name"): t.String,
             t.Key("project_starter_chunk_size"): t.Int,
             t.Key("user_chunk_size"): t.Int,
-            t.Key("order_by_columns"): t.List(t.String),
             t.Key("datasource_definition_id", optional=True): t.Or(t.String, t.Null),
-            t.Key("filter_id", optional=True): t.Or(t.String, t.Null),
-            t.Key("select_columns", optional=True): t.Or(t.List(t.String), t.Null),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         id: str,
         user_id: str,
         name: str,
         project_starter_chunk_size: int,
         user_chunk_size: int,
-        order_by_columns: List[str],
         datasource_definition_id: Optional[str] = None,
-        filter_id: Optional[str] = None,
-        select_columns: Optional[List[str]] = None,
     ):
         self.id = id
         self.user_id = user_id
         self.name = name
         self.project_starter_chunk_size = project_starter_chunk_size
         self.user_chunk_size = user_chunk_size
-        self.order_by_columns = order_by_columns
         self.datasource_definition_id = datasource_definition_id
-        self.filter_id = filter_id
-        self.select_columns = select_columns
 
     @classmethod
     def get(cls, dataset_chunk_definition_id: str) -> DatasetChunkDefinition:
         """
         Retrieve a specific dataset chunk definition metadata.
 
         Parameters
@@ -360,90 +506,67 @@
 
     @classmethod
     def create(
         cls,
         name: str,
         project_starter_chunk_size: int,
         user_chunk_size: int,
-        data_store_id: str,
-        credentials_id: str,
-        table: str,
-        schema: str,
-        catalog: str,
-        storage_kind: StorageKind,
-        order_by_columns: List[str],
-        filter_id: Optional[str] = None,
-        select_columns: Optional[List[str]] = None,
+        datasource_info: Union[DatasourceDataWarehouseInfo, DatasourceAICatalogInfo],
     ) -> DatasetChunkDefinition:
         """
         Create a dataset chunk definition. Required for both index-based and custom chunks.
 
         In order to create a dataset chunk definition, you must first:
+
             - Create a data connection to the target data source via ``dr.DataStore.create()``
             - Create credentials that must be attached to the data connection via ``dr.Credential.create()``
 
         If you have an existing data connections and credentials:
-            - Retrieve the data store id by the canonical name via
-              ``[ds for ds in dr.DataStore.list() if ds.canonical_name == <name>][0].id``
-            - Retrieve the credential id by the name via
-              ``[cr for cr in dr.Credential.list() if ds.name == <name>][0].id``
+
+            - Retrieve the data store ID by the canonical name via:
+
+                - ``[ds for ds in dr.DataStore.list() if ds.canonical_name == <name>][0].id``
+            - Retrieve the credential ID by the name via:
+
+                - ``[cr for cr in dr.Credential.list() if ds.name == <name>][0].id``
+
+        You must create the required 'datasource_info' object with the datasource information
+        that corresponds to your use case:
+
+            - DatasourceAICatalogInfo for AI catalog datasets.
+            - DatasourceDataWarehouseInfo for Snowflake, BigQuery, or other data warehouse.
 
         Parameters
         ----------
         name : str
             The name of the dataset chunk definition.
         project_starter_chunk_size : int
-            The size in bytes of the first chunk. Used to start a datarobot project.
-        data_store_id : str
-            The ID of the target data source.
-        credentials_id : str
-            The ID of the credentials attached or associated with the data_store_id.
-        table : str
-            The name of the table.
-        schema : str
-            The name of the schema.
-        catalog : str
-            The name of the database.
-        catalog : str
-            The name of the database.
-        storage_kind : str
-            The type of data source or data warehouse e.g Snowflake, BigQuery.
-        order_by_columns : List[str]
-            A list of columns used to sort the dataset.
-        filter_id: str
-            The ID of the filter object used to filter the data.
-        select_columns: List[str]
-            A list of columns to select from the dataset.
+            The size, in bytes, of the first chunk. Used to start a DataRobot project.
+        datasource_info : Union[DatasourceDataWarehouseInfo, DatasourceAICatalogInfo]
+            The object that contains the information of the data source.
 
 
         Returns
         -------
         dataset_chunk_definition: DatasetChunkDefinition
             An instance of a created dataset chunk definition.
 
         """
-
+        if not isinstance(datasource_info, (DatasourceAICatalogInfo, DatasourceDataWarehouseInfo)):
+            raise TypeError(
+                "'datasource_info' expects object of ('DatasourceAICatalogInfo', 'DatasourceDataWarehouseInfo')"
+            )
+        datasource_info_dict = datasource_info.to_dict()
         payload = {
             "name": name,
             "starterChunkSize": project_starter_chunk_size,
             "chunkSize": user_chunk_size,
-            "columnsOrder": order_by_columns,
-            "dataStoreId": data_store_id,
-            "credentialsId": credentials_id,
-            "table": table,
-            "schema": schema,
-            "catalog": catalog,
-            "storageKind": storage_kind,
+            "datasourceInfo": {camelize(key): val for key, val in datasource_info_dict.items()},
         }
 
-        if select_columns is not None:
-            payload["select_columns"] = select_columns
-        if filter_id is not None:
-            payload["filter_id"] = filter_id
-
         response = cls._client.post(cls._path, data=payload)
         data = response.json()
         return cls.from_server_data(data)
 
     @classmethod
     def get_datasource_definition(cls, dataset_chunk_definition_id: str) -> DatasourceDefinition:
         """
@@ -525,31 +648,31 @@
         )
         return DatasourceDefinition.from_location(datasource_location)
 
     def create_chunk(
         self,
         limit: int,
         offset: int = 0,
-        storage_type: ExternalStorageType = ExternalStorageType.DATASTAGE,
+        storage_type: ChunkStorageType = ChunkStorageType.DATASTAGE,
         max_wait_time: int = DEFAULT_MAX_WAIT,
     ) -> Chunk:
         """
         Creates a data chunk using the limit and offset. By default, the data chunk is stored in data stages.
 
         Depending on the size of the data set, adding ``order_by_columns`` to the dataset chunking definition
         will increase the execution time to retrieve or create the data chunk.
         Set the ``max_wait_time`` for the appropriate wait time.
 
         Parameters
         ----------
         limit: int
             The maximum number of rows.
         offset: int
-            The offset into the dataset to begin reading.
-        storage_type: ExternalStorageType
+            The offset into the dataset (where reading begins).
+        storage_type: ChunkStorageType
             The storage location of the chunk.
 
         Returns
         -------
         chunk: Chunk
             An instance of a created or updated chunk.
         """
@@ -562,31 +685,31 @@
         url = self._path_with_id + "createChunk"
         path = url.format(self.id)
         return self._create_chunk(path, payload, max_wait_time=max_wait_time)
 
     def create_chunk_by_index(
         self,
         index: int,
-        storage_type: ExternalStorageType = ExternalStorageType.DATASTAGE,
+        storage_type: ChunkStorageType = ChunkStorageType.DATASTAGE,
         max_wait_time: int = DEFAULT_MAX_WAIT,
     ) -> Chunk:
         """
         Creates a data chunk using the limit and offset. By default, the data chunk is stored in data stages.
 
         Depending on the size of the data set, adding ``order_by_columns`` to the dataset chunking definition
         will increase the execution time to retrieve or create the data chunk.
         Set the ``max_wait_time`` for the appropriate wait time.
 
         Parameters
         ----------
         limit: int
             The maximum number of rows.
         offset: int
-            The offset into the dataset to begin reading.
-        storage_type: ExternalStorageType
+            The offset into the dataset (where reading begins).
+        storage_type: ChunkStorageType
             The storage location of the chunk.
 
         Returns
         -------
         chunk: Chunk
             An instance of a created or updated chunk.
         """
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/custom_jobs/custom_job_run.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/registry/job_run.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,316 +13,331 @@
 
 from enum import Enum
 from typing import cast, List, Optional, Set
 
 import trafaret as t
 
 from datarobot._compat import String
-from datarobot._experimental.models.custom_jobs.custom_job import (
-    CustomJob,
-    CustomJobFileItem,
-    CustomJobFileItemType,
-)
 from datarobot.enums import DEFAULT_MAX_WAIT
 from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
+from datarobot.models.registry.job import Job, JobFileItem, JobFileItemType
+from datarobot.models.runtime_parameters import RuntimeParameter, RuntimeParameterValue
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
-class CustomJobRunStatus(Enum):
-    """Enum of the custom job run statuses"""
+class JobRunStatus(Enum):
+    """Enum of the job run statuses"""
 
     SUCCEEDED = "succeeded"
     FAILED = "failed"
     RUNNING = "running"
     INTERRUPTED = "interrupted"
     CANCELING = "canceling"
     CANCELED = "canceled"
 
 
-class CustomJobRun(APIObject):
-    """A DataRobot custom job run.
+class JobRun(APIObject):
+    """A DataRobot job run.
 
-    .. versionadded:: v2.33
+    .. versionadded:: v3.4
 
     Attributes
     ----------
     id: str
-        id of the custom job run
+        The ID of the job run.
     custom_job_id: str
-        id of the parent custom job
+        The ID of the parent job.
     description: str
-        description of the custom job run
+        A description of the job run.
     created_at: str
         ISO-8601 formatted timestamp of when the version was created
-    items: List[CustomJobFileItem]
-        a list of file items attached to the custom job
-    status: CustomJobRunStatus
-        status of the custom job run
+    items: List[JobFileItem]
+        A list of file items attached to the job.
+    status: JobRunStatus
+        The status of the job run.
     duration: float
-        duration of the custom job run
+        The duration of the job run.
     """
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("custom_job_id"): String(),
             t.Key("description", optional=True): t.Or(
                 String(max_length=10000, allow_blank=True), t.Null()
             ),
             t.Key("created") >> "created_at": String(),
-            t.Key("items"): t.List(CustomJobFileItem.schema),
-            t.Key("status"): t.Enum(*[e.value for e in CustomJobRunStatus]),
+            t.Key("items"): t.List(JobFileItem.schema),
+            t.Key("status"): t.Enum(*[e.value for e in JobRunStatus]),
             t.Key("duration"): t.Float(),
+            t.Key("runtime_parameters", optional=True): t.List(RuntimeParameter.schema),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
     def __init__(
         self,
         id: str,
         custom_job_id: str,
         created_at: str,
-        items: List[CustomJobFileItemType],
+        items: List[JobFileItemType],
         status: str,
         duration: float,
         description: Optional[str] = None,
+        runtime_parameters: Optional[List[RuntimeParameter]] = None,
     ) -> None:
         self.id = id
         self.custom_job_id = custom_job_id
         self.description = description
         self.created_at = created_at
 
-        # NOTE: CustomJobFileItem's __init__ instead of from_server_data is used, because at this point
+        # NOTE: JobFileItem's __init__ instead of from_server_data is used, because at this point
         #   the data is already converted from API representation to "object" representation.
-        #   In case of CustomJobFileItem it converted {"created": ..., ...} to {"created_at": ..., ...}.
-        #   For type hinting, TypedDict CustomJobFileItemType is used, which reflects expected property names and types.
-        self.items = [CustomJobFileItem(**data) for data in items]
+        #   In case of JobFileItem it converted {"created": ..., ...} to {"created_at": ..., ...}.
+        #   For type hinting, TypedDict JobFileItemType is used, which reflects expected property names and types.
+        self.items = [JobFileItem(**data) for data in items]
 
-        self.status = CustomJobRunStatus(status)
+        self.status = JobRunStatus(status)
         self.duration = duration
 
+        self.runtime_parameters = (
+            [RuntimeParameter(**param) for param in runtime_parameters]  # type: ignore[arg-type]
+            if runtime_parameters
+            else None
+        )
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.id!r})"
 
-    def _update_values(self, new_response: CustomJobRun) -> None:
+    def _update_values(self, new_response: JobRun) -> None:
         fields: Set[str] = self._fields()  # type: ignore[no-untyped-call]
         for attr in fields:
             new_value = getattr(new_response, attr)
             setattr(self, attr, new_value)
 
     @classmethod
-    def _custom_job_run_base_path(cls, custom_job_id: str) -> str:
-        return f"customJobs/{custom_job_id}/runs/"
+    def _job_run_base_path(cls, job_id: str) -> str:
+        return f"customJobs/{job_id}/runs/"
 
     @classmethod
-    def _custom_job_run_path(cls, custom_job_id: str, custom_job_run_id: str) -> str:
-        return f"customJobs/{custom_job_id}/runs/{custom_job_run_id}/"
+    def _job_run_path(cls, job_id: str, job_run_id: str) -> str:
+        return f"customJobs/{job_id}/runs/{job_run_id}/"
 
     @classmethod
-    def _custom_job_run_logs_path(cls, custom_job_id: str, custom_job_run_id: str) -> str:
-        return f"customJobs/{custom_job_id}/runs/{custom_job_run_id}/logs/"
+    def _job_run_logs_path(cls, job_id: str, job_run_id: str) -> str:
+        return f"customJobs/{job_id}/runs/{job_run_id}/logs/"
 
     @classmethod
     def create(
         cls,
-        custom_job_id: str,
+        job_id: str,
         max_wait: Optional[int] = DEFAULT_MAX_WAIT,
-    ) -> CustomJobRun:
-        """Create a custom job run.
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
+    ) -> JobRun:
+        """Create a job run.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        custom_job_id: str
-            the id of the custom job
+        job_id: str
+            The ID of the job.
         max_wait: int, optional
             max time to wait for a terminal status ("succeeded", "failed", "interrupted", "canceled").
             If set to None - method will return without waiting.
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]]
+            Additional parameters to be injected into a model at runtime. The fieldName
+            must match a fieldName that is listed in the runtimeParameterDefinitions section
+            of the model-metadata.yaml file.
 
         Returns
         -------
-        CustomJob
-            created custom job
+        Job
+            created job
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
         ValueError
-            if execution environment or entry point is not specified for the custom job
+            if execution environment or entry point is not specified for the job
         """
 
-        custom_job = CustomJob.get(custom_job_id)
-        if not custom_job.environment_id:
-            raise ValueError("Environment ID must be set for the custom job in order to be run")
-        if not custom_job.entry_point:
-            raise ValueError("Entry point must be set for the custom job in order to be run")
+        job = Job.get(job_id)
+        if not job.environment_id:
+            raise ValueError("Environment ID must be set for the job in order to be run")
+        if not job.entry_point:
+            raise ValueError("Entry point must be set for the job in order to be run")
 
-        path = cls._custom_job_run_base_path(custom_job_id)
+        path = cls._job_run_base_path(job_id)
 
-        response = cls._client.post(path)
+        payload = {}
+
+        if runtime_parameter_values:
+            payload["runtimeParameterValues"] = [
+                param.to_dict() for param in runtime_parameter_values
+            ]
+
+        response = cls._client.post(path, data=payload)
 
         data = response.json()
 
         if max_wait is None:
             return cls.from_server_data(data)
 
-        custom_job_run_loc = wait_for_async_resolution(
-            cls._client, response.headers["Location"], max_wait
-        )
-        return cls.from_location(custom_job_run_loc)
+        job_run_loc = wait_for_async_resolution(cls._client, response.headers["Location"], max_wait)
+        return cls.from_location(job_run_loc)
 
     @classmethod
-    def list(cls, custom_job_id: str) -> List[CustomJobRun]:
-        """List custom job runs.
+    def list(cls, job_id: str) -> List[JobRun]:
+        """List job runs.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        custom_job_id: str
-            the id of the custom job
+        job_id: str
+            The ID of the job.
 
         Returns
         -------
-        List[CustomJob]
-            a list of custom job runs
+        List[Job]
+            A list of job runs.
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
         """
-        data = unpaginate(cls._custom_job_run_base_path(custom_job_id), None, cls._client)
+        data = unpaginate(cls._job_run_base_path(job_id), None, cls._client)
         return [cls.from_server_data(item) for item in data]
 
     @classmethod
-    def get(cls, custom_job_id: str, custom_job_run_id: str) -> CustomJobRun:
-        """Get custom job run by id.
+    def get(cls, job_id: str, job_run_id: str) -> JobRun:
+        """Get job run by id.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Parameters
         ----------
-        custom_job_id: str
-            the id of the custom job
-        custom_job_run_id: str
-            the id of the custom job run
+        job_id: str
+            The ID of the job.
+        job_run_id: str
+            The ID of the job run.
 
         Returns
         -------
-        CustomJob
-            retrieved custom job run
+        Job
+            The retrieved job run.
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status.
         datarobot.errors.ServerError
             if the server responded with 5xx status.
         """
-        path = cls._custom_job_run_path(custom_job_id, custom_job_run_id)
+        path = cls._job_run_path(job_id, job_run_id)
         return cls.from_location(path)
 
     def update(self, description: Optional[str] = None) -> None:
-        """Update custom job run properties.
+        """Update job run properties.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Parameters
         ----------
         description: str
-            new custom job run description
+            new job run description
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status.
         datarobot.errors.ServerError
             if the server responded with 5xx status.
         """
         payload = {}
         if description:
             payload.update({"description": description})
 
-        path = self._custom_job_run_path(self.custom_job_id, self.id)
+        path = self._job_run_path(self.custom_job_id, self.id)
 
         response = self._client.patch(path, data=payload)
 
         data = response.json()
-        new_version = CustomJobRun.from_server_data(data)
+        new_version = JobRun.from_server_data(data)
         self._update_values(new_version)
 
     def cancel(self) -> None:
-        """Cancel custom job run.
+        """Cancel job run.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Raises
         ------
         datarobot.errors.ClientError
             If the server responded with 4xx status.
         datarobot.errors.ServerError
             If the server responded with 5xx status.
         """
-        url = self._custom_job_run_path(self.custom_job_id, self.id)
+        url = self._job_run_path(self.custom_job_id, self.id)
         self._client.delete(url)
 
     def refresh(self) -> None:
-        """Update custom job run with the latest data from server.
+        """Update job run with the latest data from server.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
         """
 
         new_object = self.get(self.custom_job_id, self.id)
         self._update_values(new_object)
 
     def get_logs(self) -> Optional[str]:
-        """Get log of the custom job run.
+        """Get log of the job run.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
         """
-        path = self._custom_job_run_logs_path(self.custom_job_id, self.id)
+        path = self._job_run_logs_path(self.custom_job_id, self.id)
         try:
             response = self._client.get(path)
             return cast(str, response.text)
         except ClientError as exc:
             if exc.status_code == 404 and exc.json == {"message": "No log found"}:
                 return None
             raise
 
     def delete_logs(self) -> None:
-        """Get log of the custom job run.
+        """Get log of the job run.
 
-        .. versionadded:: v2.33
+        .. versionadded:: v3.4
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
         """
-        path = self._custom_job_run_logs_path(self.custom_job_id, self.id)
+        path = self._job_run_logs_path(self.custom_job_id, self.id)
         self._client.delete(path)
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/dataset.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/enums.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-from enum import Enum
 from typing import List
 
 from strenum import StrEnum
 
 
 class AllEnumMixin:
     @classmethod
@@ -55,105 +54,105 @@
             cls.ABORTED,
             cls.COMPLETED,
             cls.ERROR,
             cls.COMPLETED_WITH_ERRORS,
         ]
 
 
-class NotebookPermissions(str, Enum):
+class NotebookPermissions(StrEnum):
     CAN_READ = "CAN_READ"
     CAN_UPDATE = "CAN_UPDATE"
     CAN_DELETE = "CAN_DELETE"
     CAN_SHARE = "CAN_SHARE"
     CAN_COPY = "CAN_COPY"
     CAN_EXECUTE = "CAN_EXECUTE"
 
 
-class NotebookStatus(str, Enum):
+class NotebookStatus(StrEnum):
     STOPPING = "stopping"
     STOPPED = "stopped"
     STARTING = "starting"
     RUNNING = "running"
     RESTARTING = "restarting"
     DEAD = "dead"
     DELETED = "deleted"
 
 
-class CategoricalStatsMethods(str, Enum):
+class CategoricalStatsMethods(StrEnum):
     MOST_FREQUENT = "most-frequent"
 
 
-class NumericStatsMethods(str, Enum):
+class NumericStatsMethods(StrEnum):
     MAX = "max"
     MIN = "min"
     AVG = "avg"
     STDDEV = "stddev"
     MEDIAN = "median"
 
 
-class DataWranglingDialect(str, Enum):
+class DataWranglingDialect(StrEnum):
     SNOWFLAKE = "snowflake"
 
 
-class RecipeInputType(str, Enum):
+class RecipeInputType(StrEnum):
     DATASOURCE = "datasource"
 
 
-class DatetimeSamplingStrategy(str, Enum):
+class DatetimeSamplingStrategy(StrEnum):
     EARLIEST = "earliest"
     LATEST = "latest"
 
 
-class WranglingOperations(str, Enum):
+class WranglingOperations(StrEnum):
     """Supported data wrangling operations."""
 
     COMPUTE_NEW = "compute-new"
     DROP_COLUMNS = "drop-columns"
     RENAME_COLUMNS = "rename-columns"
     FILTER = "filter"
 
     LAGS = "lags"
     WINDOW_NUMERIC_STATS = "window-numeric-stats"
     TIME_SERIES = "time-series"
 
 
-class SamplingOperations(str, Enum):
+class SamplingOperations(StrEnum):
     """Supported data wrangling sampling operations."""
 
     RANDOM_SAMPLE = "random-sample"
     DATETIME_SAMPLE = "datetime-sample"
 
 
-class DownsamplingOperations(str, Enum):
+class DownsamplingOperations(StrEnum):
     """Supported data wrangling sampling operations."""
 
     RANDOM_SAMPLE = "random-sample"
     SMART_DOWNSAMPLING = "smart-downsampling"
 
 
-class DataWranglingDataSourceTypes(str, Enum):
+class DataWranglingDataSourceTypes(StrEnum):
     JDBC = "jdbc"
 
 
-class FilterOperationFunctions(str, Enum):
+class FilterOperationFunctions(StrEnum):
     """Operations, supported in FilterOperation."""
 
     EQUALS = "eq"
     NOT_EQUALS = "neq"
     LESS_THAN = "lt"
     LESS_THAN_OR_EQUALS = "lte"
     GREATER_THAN = "gt"
     GREATER_THAN_OR_EQUALS = "gte"
     IS_NULL = "null"
     IS_NOT_NULL = "notnull"
     BETWEEN = "between"
     CONTAINS = "contains"
 
 
-class ListVectorDatabasesSortQueryParams(str, Enum):
+class ListVectorDatabasesSortQueryParams(StrEnum):
     """supported Sort query params for the Vectordatabase.list method."""
 
     NAME_ASCENDING = "name"
     NAME_DESCENDING = "-name"
     CREATION_USER_DATE_ASCENDING = "creationUserId"
     CREATION_USER_DATE_DESCENDING = "-creationUserId"
     CREATION_DATE_ASCENDING = "creationDate"
@@ -174,31 +173,31 @@
     DATASET_NAME_DESCENDING = "-datasetName"
     PLAYGROUNDS_COUNT_ASCENDING = "playgroundsCount"
     PLAYGROUNDS_COUNT_DESCENDING = "-playgroundsCount"
     SOURCE_ASCENDING = "source"
     SOURCE_DESCENDING = "-source"
 
 
-class VectorDatabaseEmbeddingModel(str, Enum):
+class VectorDatabaseEmbeddingModel(StrEnum):
     """Text embedding model names for VectorDatabases."""
 
     E5_LARGE_V2 = "intfloat/e5-large-v2"
     E5_BASE_V2 = "intfloat/e5-base-v2"
     MULTILINGUAL_E5_BASE = "intfloat/multilingual-e5-base"
     ALL_MINILM_L6_V2 = "sentence-transformers/all-MiniLM-L6-v2"
     JINA_EMBEDDING_T_EN_V1 = "jinaai/jina-embedding-t-en-v1"
 
 
-class VectorDatabaseChunkingMethod(str, Enum):
+class VectorDatabaseChunkingMethod(StrEnum):
     """Text chunking method names for VectorDatabases."""
 
     RECURSIVE = "recursive"
 
 
-class VectorDatabaseDatasetLanguages(str, Enum):
+class VectorDatabaseDatasetLanguages(StrEnum):
     """Dataset languages supported by VectorDatabases."""
 
     AFRIKAANS = "Afrikaans"
     AMHARIC = "Amharic"
     ARABIC = "Arabic"
     ASSAMESE = "Assamese"
     AZERBAIJANI = "Azerbaijani"
@@ -292,38 +291,38 @@
     CHINESE = "Chinese"
 
     @classmethod
     def list_all_languages(cls):
         return list(map(lambda c: c.value, cls))  # type: ignore [attr-defined]
 
 
-class VectorDatabaseChunkingParameterType(str, Enum):
+class VectorDatabaseChunkingParameterType(StrEnum):
     """Chunking parameter types supported by VectorDatabases."""
 
     INT = "int"
     LIST_STR = "list[str]"
 
 
-class VectorDatabaseSource(str, Enum):
+class VectorDatabaseSource(StrEnum):
     """Supported source for VectorDatabases."""
 
     DATAROBOT = "DataRobot"
     EXTERNAL = "External"
 
 
-class VectorDatabaseExecutionStatus(str, Enum):
+class VectorDatabaseExecutionStatus(StrEnum):
     """Execution Statuses VectorDatabases can be in."""
 
     NEW = "NEW"
     RUNNING = "RUNNING"
     COMPLETED = "COMPLETED"
     ERROR = "ERROR"
 
 
-class ListPlaygroundsSortQueryParams(str, Enum):
+class ListPlaygroundsSortQueryParams(StrEnum):
     """supported Sort query params for the Playground.list method."""
 
     NAME_ASCENDING = "name"
     NAME_DESCENDING = "-name"
     DESCRIPTION_ASCENDING = "description"
     DESCRIPTION_DESCENDING = "-description"
     CREATION_USER_DATE_ASCENDING = "creationUserId"
@@ -332,15 +331,33 @@
     CREATION_DATE_DESCENDING = "-creationDate"
     LAST_UPDATE_USER_DATE_ASCENDING = "lastUpdateUserId"
     LAST_UPDATE_USER_DATE_DESCENDING = "-lastUpdateUserId"
     SAVED_LLM_BLUEPRINTS_COUNT_ASCENDING = "savedLLMBlueprintsCount"
     SAVED_LLM_BLUEPRINTS_COUNT_DESCENDING = "-savedLLMBlueprintsCount"
 
 
-class ListLLMBlueprintsSortQueryParams(str, Enum):
+class ListChatsSortQueryParams(StrEnum):
+    """supported Sort query params for the Chat.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class ListComparisonChatsSortQueryParams(StrEnum):
+    """supported Sort query params for the ComparisonChat.list method."""
+
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class ListLLMBlueprintsSortQueryParams(StrEnum):
     """supported Sort query params for the LLMBlueprint.list method."""
 
     NAME_ASCENDING = "name"
     NAME_DESCENDING = "-name"
     DESCRIPTION_ASCENDING = "description"
     DESCRIPTION_DESCENDING = "-description"
     CREATION_USER_DATE_ASCENDING = "creationUserId"
@@ -353,14 +370,30 @@
     LAST_UPDATE_DATE_DESCENDING = "-lastUpdateDate"
     LLM_ID_ASCENDING = "llmId"
     LLM_ID_DESCENDING = "-llmId"
     VECTOR_DATABASE_ID_ASCENDING = "vectorDatabaseId"
     VECTOR_DATABASE_ID_DESCENDING = "-vectorDatabaseId"
 
 
+class ListCustomModelValidationsSortQueryParams(StrEnum):
+    NAME_ASCENDING = "name"
+    NAME_DESCENDING = "-name"
+    DEPLOYMENT_NAME_ASCENDING = "deploymentName"
+    DEPLOYMENT_NAME_DESCENDING = "-deploymentName"
+    USER_NAME_ASCENDING = "userName"
+    USER_NAME_DESCENDING = "-userName"
+    CREATION_DATE_ASCENDING = "creationDate"
+    CREATION_DATE_DESCENDING = "-creationDate"
+
+
+class FeedbackSentiment(StrEnum):
+    POSITIVE = "1"
+    NEGATIVE = "0"
+
+
 class IncrementalLearningStatus(object):
     STARTED = "started"
     IN_PROGRESS = "in_progress"
     COMPLETED = "completed"
     STOPPED = "stopped"
     ERROR = "error"
 
@@ -371,19 +404,38 @@
     IN_PROGRESS = "in_progress"
     COMPLETED = "completed"
     ERROR = "error"
 
     ALL = [IN_PROGRESS, COMPLETED, ERROR]
 
 
-class StorageKind(StrEnum):
-    """Supported Data Sources."""
+class StorageType(StrEnum):
+    """Supported data storages."""
 
     SNOWFLAKE = "snowflake"
     BIGQUERY = "bigquery"
+    DATABRICKS = "databricks"
+    AI_CATALOG = "aicatalog"
+    DATASTAGE = "datastage"
 
 
-class ExternalStorageType(StrEnum):
-    """Supported External Storage"""
+class OriginStorageType(StrEnum):
+    """Supported data sources."""
 
-    DATASTAGE = "datastage"
-    AI_CATALOG = "aiCatalog"
+    SNOWFLAKE = StorageType.SNOWFLAKE
+    BIGQUERY = StorageType.BIGQUERY
+    DATABRICKS = StorageType.DATABRICKS
+    AI_CATALOG = StorageType.AI_CATALOG
+
+
+class ChunkStorageType(StrEnum):
+    """Supported chunk storage."""
+
+    DATASTAGE = StorageType.DATASTAGE
+    AI_CATALOG = StorageType.AI_CATALOG
+
+
+class PromptType(StrEnum):
+    """Supported LLM Blueprint prompting types."""
+
+    ONE_TIME_PROMPT = "ONE_TIME_PROMPT"
+    CHAT_HISTORY_AWARE = "CHAT_HISTORY_AWARE"
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/chat_prompt.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/chat_prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,30 +9,35 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
+from mypy_extensions import TypedDict
 import trafaret as t
 
+from datarobot._experimental.models.enums import FeedbackSentiment
+from datarobot._experimental.models.genai.chat import Chat
 from datarobot._experimental.models.genai.llm import LLMDefinition
 from datarobot._experimental.models.genai.llm_blueprint import (
     LLMBlueprint,
     vector_database_settings_trafaret,
     VectorDatabaseSettings,
 )
+from datarobot._experimental.models.genai.playground import Playground
 from datarobot._experimental.models.genai.vector_database import VectorDatabase
+from datarobot.enums import enum_to_list
 from datarobot.models.api_object import APIObject
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
 def get_entity_id(
-    entity: Union[ChatPrompt, LLMBlueprint, LLMDefinition, VectorDatabase, str]
+    entity: Union[Playground, Chat, ChatPrompt, LLMBlueprint, LLMDefinition, VectorDatabase, str]
 ) -> str:
     """
     Get the entity ID from the entity parameter.
 
     Parameters
     ----------
     entity : ApiObject or str
@@ -45,14 +50,46 @@
     """
     if isinstance(entity, str):
         return entity
 
     return entity.id
 
 
+class FeedbackMetadataDict(TypedDict):
+    feedback: FeedbackSentiment
+
+
+class MetricMetadataDict(TypedDict):
+    name: str
+    value: Any
+    formatted_value: Optional[str]
+    sidecar_model_metric_validation_id: Optional[str]
+    custom_model_id: Optional[str]
+    evaluation_dataset_configuration_id: Optional[str]
+    cost_configuration_id: Optional[str]
+
+
+feedback_metadata_trafaret = t.Dict(
+    {t.Key("feedback"): t.Enum(*enum_to_list(FeedbackSentiment))}
+).ignore_extra("*")
+
+
+metric_metadata_trafaret = t.Dict(
+    {
+        t.Key("name"): t.String,
+        t.Key("value"): t.Any,
+        t.Key("formatted_value", optional=True): t.Or(t.String, t.Null),
+        t.Key("sidecar_model_metric_validation_id", optional=True): t.Or(t.String, t.Null),
+        t.Key("custom_model_id", optional=True): t.Or(t.String, t.Null),
+        t.Key("evaluation_dataset_configuration_id", optional=True): t.Or(t.String, t.Null),
+        t.Key("cost_configuration_id", optional=True): t.Or(t.String, t.Null),
+    }
+).ignore_extra("*")
+
+
 result_metadata_trafaret = t.Dict(
     {
         t.Key("cost", optional=True): t.Or(t.Float, t.Null),
         t.Key("output_token_count"): t.Int,
         t.Key("input_token_count"): t.Int,
         t.Key("total_token_count"): t.Int,
         t.Key("estimated_docs_token_count"): t.Int,
@@ -93,18 +130,104 @@
             vector_database_settings_trafaret, t.Null
         ),
         t.Key("result_metadata", optional=True): t.Or(result_metadata_trafaret, t.Null),
         t.Key("result_text", optional=True): t.Or(t.String, t.Null),
         t.Key("confidence_scores", optional=True): t.Or(confidence_scores_trafaret, t.Null),
         t.Key("citations"): t.List(citation_trafaret),
         t.Key("execution_status"): t.String,
+        t.Key("chat_id", optional=True): t.Or(t.String, t.Null),
+        t.Key("chat_context_id", optional=True): t.Or(t.String, t.Null),
+        t.Key("chat_prompt_ids_included_in_history", optional=True): t.Or(t.List(t.String), t.Null),
     }
 ).ignore_extra("*")
 
 
+class FeedbackMetadata(APIObject):
+    """
+    Metadata for feedback associated with a chat prompt.
+
+    Attributes
+    ----------
+    feedback : FeedbackSentiment
+        The sentiment of the feedback.
+    """
+
+    _converter = feedback_metadata_trafaret
+
+    def __init__(self, feedback: FeedbackSentiment):
+        self.feedback = feedback
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(feedback={self.feedback})"
+
+    def to_dict(self) -> FeedbackMetadataDict:
+        return {"feedback": self.feedback}
+
+
+class MetricMetadata(APIObject):
+    """
+    Metadata for the custom metrics associated with a chat prompt.
+
+    Attributes
+    ----------
+    name : str
+        The name of the metric.
+    value : Any
+        The value of the metric.
+    formatted_value : Optional[str], optional
+        The formatted value of the metric, if any.
+    sidecar_model_metric_validation_id : Optional[str], optional
+        The ID of the sidecar model implementing the metric, if any.
+    custom_model_id : Optional[str], optional
+        The ID of the custom model implementing the metric, if any.
+    evaluation_dataset_configuration_id : Optional[str], optional
+        The ID of the evaluation dataset configuration associated with the metric, if any.
+    cost_configuration_id : Optional[str], optional
+        The ID of the cost configuration associated with the metric, if any.
+    """
+
+    _converter = metric_metadata_trafaret
+
+    def __init__(
+        self,
+        name: str,
+        value: Any,
+        formatted_value: Optional[str] = None,
+        sidecar_model_metric_validation_id: Optional[str] = None,
+        custom_model_id: Optional[str] = None,
+        evaluation_dataset_configuration_id: Optional[str] = None,
+        cost_configuration_id: Optional[str] = None,
+    ):
+        self.name = name
+        self.value = value
+        self.formatted_value = formatted_value
+        self.sidecar_model_metric_validation_id = sidecar_model_metric_validation_id
+        self.custom_model_id = custom_model_id
+        self.evaluation_dataset_configuration_id = evaluation_dataset_configuration_id
+        self.cost_configuration_id = cost_configuration_id
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(name={self.name}, "
+            f"value={self.value}, "
+            f"formatted_value={self.formatted_value})"
+        )
+
+    def to_dict(self) -> MetricMetadataDict:
+        return {
+            "name": self.name,
+            "value": self.value,
+            "formatted_value": self.formatted_value,
+            "sidecar_model_metric_validation_id": self.sidecar_model_metric_validation_id,
+            "custom_model_id": self.custom_model_id,
+            "evaluation_dataset_configuration_id": self.evaluation_dataset_configuration_id,
+            "cost_configuration_id": self.cost_configuration_id,
+        }
+
+
 class ResultMetadata(APIObject):
     """
     Metadata for the result of a chat prompt submission.
 
     Attributes
     ----------
     output_token_count : int
@@ -222,30 +345,30 @@
     id : str
         Chat prompt ID.
     text : str
         The prompt text.
     llm_blueprint_id : str
         ID of the LLM blueprint associated with the chat prompt.
     llm_id : str
-        ID of the LLM type. This must be one of the IDs returned by LLMDefinition.list
+        ID of the LLM type. This must be one of the IDs returned by `LLMDefinition.list`
         for this user.
     llm_settings : dict or None
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from LLMDefinition.list
+        constraints on the values are defined in the response from `LLMDefinition.list`
         but this typically has dict fields:
         - system_prompt - The system prompt that tells the LLM how to behave.
         - max_completion_length - The maximum number of token in the completion.
         - temperature - controls the variability in the LLM response.
         - top_p - the model considers next tokens with top_p probability mass
         or
         - system_prompt - The system prompt that tells the LLM how to behave.
         - validation_id - The ID of the custom model LLM validation
         for custom model LLM blueprints.
     creation_date : str
-        Date when the playground was created.
+        The date the chat prompt was created.
     creation_user_id : str
         ID of the creating user.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
         The settings for the vector database associated with the LLM blueprint, if any.
     result_metadata : ResultMetadata or None
@@ -254,14 +377,20 @@
         The result text from the chat prompt submission.
     confidence_scores: ConfidenceScores or None
         The confidence scores if there is a vector database associated with the chat prompt.
     citations: list[Citation]
         List of citations from text retrieved from the vector database, if any.
     execution_status: str
         The execution status of the chat prompt.
+    chat_id: Optional[str]
+        ID of the chat associated with the chat prompt.
+    chat_context_id: Optional[str]
+        The ID of the chat context for the chat prompt.
+    chat_prompt_ids_included_in_history: Optional[list[str]]
+        The IDs of the chat prompts included in the chat history for this chat prompt.
     """
 
     _path = "api-gw/genai/chatPrompts"
 
     _converter = chat_prompt_trafaret
 
     def __init__(
@@ -276,14 +405,17 @@
         execution_status: str,
         llm_settings: Optional[Dict[str, Any]] = None,
         vector_database_id: Optional[str] = None,
         vector_database_settings: Optional[Dict[str, Any]] = None,
         result_metadata: Optional[Dict[str, Any]] = None,
         result_text: Optional[str] = None,
         confidence_scores: Optional[Dict[str, float]] = None,
+        chat_id: Optional[str] = None,
+        chat_context_id: Optional[str] = None,
+        chat_prompt_ids_included_in_history: Optional[list[str]] = None,
     ):
         self.id = id
         self.text = text
         self.llm_blueprint_id = llm_blueprint_id
         self.llm_id = llm_id
         self.llm_settings = llm_settings
         self.creation_date = creation_date
@@ -299,81 +431,81 @@
         self.result_metadata = (
             ResultMetadata.from_server_data(result_metadata) if result_metadata else None
         )
         self.result_text = result_text
         self.confidence_scores = (
             ConfidenceScores.from_server_data(confidence_scores) if confidence_scores else None
         )
+        self.chat_id = chat_id
+        self.chat_context_id = chat_context_id
+        self.chat_prompt_ids_included_in_history = chat_prompt_ids_included_in_history
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(id={self.id}, "
             f"execution_status={self.execution_status}, text={self.text[:1000]})"
         )
 
     @classmethod
     def create(
         cls,
-        llm_blueprint: Union[LLMBlueprint, str],
         text: str,
+        llm_blueprint: Optional[Union[LLMBlueprint, str]] = None,
+        chat: Optional[Union[Chat, str]] = None,
         llm: Optional[Union[LLMDefinition, str]] = None,
         llm_settings: Optional[Dict[str, Optional[Union[bool, int, float, str]]]] = None,
         vector_database: Optional[Union[VectorDatabase, str]] = None,
         vector_database_settings: Optional[VectorDatabaseSettings] = None,
         wait_for_completion: bool = False,
     ) -> ChatPrompt:
         """
-        Create a new ChatPrompt. This submits the prompt text to the LLM.
+        Create a new ChatPrompt. This submits the prompt text to the LLM. Either `llm_blueprint`
+        or `chat` is required.
 
         Parameters
         ----------
-        llm_blueprint : LLMBlueprint or str
-            The LLM blueprint associated with the created chat prompt.
-            Accepts LLM blueprint or ID.
         text : str
             The prompt text.
+        llm_blueprint : LLMBlueprint or str or None, optional
+            The LLM blueprint associated with the created chat prompt, either `LLMBlueprint` or
+            LLM blueprint ID.
+        chat : Chat or str or None, optional
+            The chat associated with the created chat prompt, either `Chat` or chat ID.
         llm : LLMDefinition, str, or None, optional
-            LLM to use for the chat prompt. Accepts LLMDefinition or LLM ID. This can only be
-            submitted if the LLM blueprint is not saved and the underlying LLM blueprint
-            will be updated with the new LLM ID.
+            LLM to use for the chat prompt. Accepts `LLMDefinition` or LLM ID.
         llm_settings: dict or None
-            LLM settings to use for the chat prompt. This can only be
-            submitted if the LLM blueprint is not saved and the underlying LLM blueprint
-            will be updated with the new LLM settings. The specific keys allowed and the
-            constraints on the values are defined in the response from LLMDefinition.list
+            LLM settings to use for the chat prompt. The specific keys allowed and the
+            constraints on the values are defined in the response from `LLMDefinition.list`
             but this typically has dict fields:
             - system_prompt - The system prompt that tells the LLM how to behave.
             - max_completion_length - The maximum number of token in the completion.
             - temperature - controls the variability in the LLM response.
             - top_p - the model considers next tokens with top_p probability mass
             or
             - system_prompt - The system prompt that tells the LLM how to behave.
             - validation_id - The ID of the custom model LLM validation
             for custom model LLM blueprints.
         vector_database: VectorDatabase, str, or None, optional
             The vector database to use with this chat prompt submission.
-            Accepts VectorDatabase or vector database ID. This can only be
-            submitted if the LLM blueprint is not saved and the underlying LLM blueprint
-            will be updated with the new vector database ID.
+            Accepts `VectorDatabase` or vector database ID.
         vector_database_settings: VectorDatabaseSettings or None, optional
-            Settings for the vector database, if any. This can only be
-            submitted if the LLM blueprint is not saved and the underlying LLM blueprint
-            will be updated with the new vector database settings.
+            Settings for the vector database, if any.
         wait_for_completion : bool
             If set to True code will wait for the chat prompt job to complete before
             returning the result (up to 10 minutes, raising timeout error after that).
-            Otherwise, you can check current status by using ChatPrompt.get with returned ID.
+            Otherwise, you can check current status by using `ChatPrompt.get` with returned ID.
 
         Returns
         -------
         chat_prompt : ChatPrompt
             The created chat prompt.
         """
         payload = {
-            "llm_blueprint_id": get_entity_id(llm_blueprint),
+            "llm_blueprint_id": get_entity_id(llm_blueprint) if llm_blueprint else None,
+            "chat_id": get_entity_id(chat) if chat else None,
             "text": text,
             "llm_id": get_entity_id(llm) if llm else None,
             "llm_settings": llm_settings,
             "vector_database_id": get_entity_id(vector_database) if vector_database else None,
             "vector_database_settings": vector_database_settings.to_dict()
             if vector_database_settings
             else None,
@@ -389,48 +521,89 @@
     @classmethod
     def get(cls, chat_prompt: Union[ChatPrompt, str]) -> ChatPrompt:
         """
         Retrieve a single chat prompt.
 
         Parameters
         ----------
-        chat_prompt : str
-            The chat prompt you want to retrieve. Accepts entity or ID.
+        chat_prompt : ChatPrompt or str
+            The chat prompt you want to retrieve, either `ChatPrompt` or chat prompt ID.
 
         Returns
         -------
         chat_prompt : ChatPrompt
             The requested chat prompt.
         """
         url = f"{cls._client.domain}/{cls._path}/{get_entity_id(chat_prompt)}/"
         r_data = cls._client.get(url)
         return cls.from_server_data(r_data.json())
 
+    def update(
+        self,
+        custom_metrics: Optional[list[MetricMetadata]] = None,
+        feedback_metadata: Optional[FeedbackMetadata] = None,
+    ) -> ChatPrompt:
+        """
+        Update the chat prompt.
+
+        Parameters
+        ----------
+        custom_metrics : Optional[list[MetricMetadata]], optional
+            The new custom metrics to add to the chat prompt.
+        feedback_metadata: Optional[FeedbackMetadata], optional
+            The new feedback to add to the chat prompt.
+
+        Returns
+        -------
+        chat_prompt : ChatPrompt
+            The updated chat prompt.
+        """
+        payload = {
+            "custom_metrics": [metadata.to_dict() for metadata in custom_metrics]
+            if custom_metrics
+            else None,
+            "feedback_metadata": feedback_metadata.to_dict() if feedback_metadata else None,
+        }
+        url = f"{self._client.domain}/{self._path}/{self.id}/"
+        r_data = self._client.patch(url, data=payload)
+        return self.from_server_data(r_data.json())
+
     @classmethod
     def list(
         cls,
         llm_blueprint: Optional[Union[LLMBlueprint, str]] = None,
+        playground: Optional[Union[Playground, str]] = None,
+        chat: Optional[Union[Chat, str]] = None,
     ) -> List[ChatPrompt]:
         """
-        List all chat prompts available to the user. If the LLM blueprint is specified then the
-        results are restricted to the chat prompts associated with the LLM blueprint.
+        List all chat prompts available to the user. If the `llm_blueprint`, `playground`, or `chat`
+        is specified then the results are restricted to the chat prompts associated with that
+        entity.
 
         Parameters
         ----------
         llm_blueprint : Optional[Union[LLMBlueprint, str]], optional
             The returned chat prompts are filtered to those associated with a specific LLM blueprint
-            if it is specified. Accepts either the entity or the ID.
+            if it is specified. Accepts either `LLMBlueprint` or LLM blueprint ID.
+        playground : Optional[Union[Playground, str]], optional
+            The returned chat prompts are filtered to those associated with a specific playground
+            if it is specified. Accepts either `Playground` or playground ID.
+        chat : Optional[Union[Chat, str]], optional
+            The returned chat prompts are filtered to those associated with a specific chat
+            if it is specified. Accepts either `Chat` or chat ID.
 
         Returns
         -------
         chat_prompts : list[ChatPrompt]
             A list of chat prompts available to the user.
         """
         params = {
             "llm_blueprint_id": get_entity_id(llm_blueprint) if llm_blueprint else None,
+            "playground_id": get_entity_id(playground) if playground else None,
+            "chat_id": get_entity_id(chat) if chat else None,
         }
         url = f"{cls._client.domain}/{cls._path}/"
         r_data = unpaginate(url, params, cls._client)
         return [cls.from_server_data(data) for data in r_data]
 
     def delete(self) -> None:
         """
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/comparison_prompt.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/comparison_prompt.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,31 +9,36 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
+from mypy_extensions import TypedDict
 import trafaret as t
 
 from datarobot._experimental.models.genai.chat_prompt import (
     Citation,
     citation_trafaret,
     confidence_scores_trafaret,
     ConfidenceScores,
+    feedback_metadata_trafaret,
+    FeedbackMetadata,
+    FeedbackMetadataDict,
     result_metadata_trafaret,
     ResultMetadata,
 )
+from datarobot._experimental.models.genai.comparison_chat import ComparisonChat
 from datarobot._experimental.models.genai.llm_blueprint import LLMBlueprint
 from datarobot.models.api_object import APIObject
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
-def _get_genai_entity_id(entity: Union[ComparisonPrompt, LLMBlueprint, str]) -> str:
+def _get_genai_entity_id(entity: Union[ComparisonChat, ComparisonPrompt, LLMBlueprint, str]) -> str:
     """
     Get the entity ID from the entity parameter.
 
     Parameters
     ----------
     entity : ApiObject or str
         May be entity ID or the entity.
@@ -45,78 +50,144 @@
     """
     if isinstance(entity, str):
         return entity
 
     return entity.id
 
 
+class FeedbackResultDict(TypedDict):
+    comparison_prompt_result_id: str
+    feedback_metadata: FeedbackMetadataDict
+
+
+feedback_result_trafaret = t.Dict(
+    {
+        t.Key("comparison_prompt_result_id"): t.String,
+        t.Key("feedback_metadata"): feedback_metadata_trafaret,
+    }
+).ignore_extra("*")
+
+
 comparison_prompt_result_trafaret = t.Dict(
     {
+        t.Key("id"): t.String,
         t.Key("llm_blueprint_id"): t.String,
         t.Key("result_metadata", optional=True): t.Or(result_metadata_trafaret, t.Null),
         t.Key("result_text", optional=True): t.Or(t.String, t.Null),
         t.Key("confidence_scores", optional=True): t.Or(confidence_scores_trafaret, t.Null),
         t.Key("citations"): t.List(citation_trafaret),
         t.Key("execution_status"): t.String,
+        t.Key("chat_context_id", optional=True): t.Or(t.String, t.Null),
+        t.Key("comparison_prompt_result_ids_included_in_history", optional=True): t.Or(
+            t.List(t.String), t.Null
+        ),
     }
 ).ignore_extra("*")
 
 
 comparison_prompt_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("text"): t.String,
         t.Key("results"): t.List(comparison_prompt_result_trafaret),
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
+        t.Key("comparison_chat_id", optional=True): t.Or(t.String, t.Null),
     }
 ).ignore_extra("*")
 
 
+class FeedbackResult(APIObject):
+    """
+    Feedback associated with a comparison prompt result.
+
+    Attributes
+    ----------
+    comparison_prompt_result_id : str
+        The ID of the comparison prompt result associated with the feedback.
+    feedback_metadata : FeedbackMetadata
+        The metadata for the feedback.
+    """
+
+    _converter = feedback_result_trafaret
+
+    def __init__(self, comparison_prompt_result_id: str, feedback_metadata: FeedbackMetadata):
+        self.comparison_prompt_result_id = comparison_prompt_result_id
+        self.feedback_metadata = feedback_metadata
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}"
+            f"(comparison_prompt_result_id={self.comparison_prompt_result_id},"
+            f"feedback_metadata={self.feedback_metadata})"
+        )
+
+    def to_dict(self) -> FeedbackResultDict:
+        return {
+            "comparison_prompt_result_id": self.comparison_prompt_result_id,
+            "feedback_metadata": self.feedback_metadata.to_dict(),
+        }
+
+
 class ComparisonPromptResult(APIObject):
     """
     Metadata for a DataRobot GenAI comparison prompt result.
 
     Attributes
     ----------
+    id: str
+        The ID of the comparison prompt result.
     llm_blueprint_id : str
-        ID of the LLM blueprint associated with the chat prompt.
+        The ID of the LLM blueprint associated with the chat prompt.
     result_metadata : ResultMetadata or None
         Metadata for the result of the chat prompt submission.
     result_text: str or None
         The result text from the chat prompt submission.
     confidence_scores: ConfidenceScores or None
         The confidence scores if there is a vector database associated with the chat prompt.
     citations: list[Citation]
         List of citations from text retrieved from the vector database, if any.
     execution_status: str
         The execution status of the chat prompt.
+    chat_context_id: Optional[str], optional
+        The ID of the chat context for this comparison prompt result.
+    comparison_prompt_result_ids_included_in_history: Optional[List[str]], optional
+        The IDs of the comparison prompt results included in the chat history for this
+        comparison prompt result.
     """
 
     _converter = comparison_prompt_result_trafaret
 
     def __init__(
         self,
+        id: str,
         llm_blueprint_id: str,
         citations: List[Dict[str, Any]],
         execution_status: str,
         result_metadata: Optional[Dict[str, Any]] = None,
         result_text: Optional[str] = None,
         confidence_scores: Optional[Dict[str, float]] = None,
+        chat_context_id: Optional[str] = None,
+        comparison_prompt_result_ids_included_in_history: Optional[List[str]] = None,
     ):
+        self.id = id
         self.llm_blueprint_id = llm_blueprint_id
         self.citations = [Citation.from_server_data(citation) for citation in citations]
         self.execution_status = execution_status
         self.result_metadata = (
             ResultMetadata.from_server_data(result_metadata) if result_metadata else None
         )
         self.result_text = result_text
         self.confidence_scores = (
             ConfidenceScores.from_server_data(confidence_scores) if confidence_scores else None
         )
+        self.chat_context_id = chat_context_id
+        self.comparison_prompt_result_ids_included_in_history = (
+            comparison_prompt_result_ids_included_in_history
+        )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(llm_blueprint_id={self.llm_blueprint_id}, "
             f"execution_status={self.execution_status})"
         )
 
@@ -133,69 +204,80 @@
         The prompt text.
     results : list[ComparisonPromptResult]
         The list of results for individual LLM blueprints that are part of the comparison prompt.
     creation_date : str
         Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
+    comparison_chat_id : str
+        The ID of the comparison chat this comparison prompt is associated with.
     """
 
     _path = "api-gw/genai/comparisonPrompts"
 
     _converter = comparison_prompt_trafaret
 
     def __init__(
         self,
         id: str,
         text: str,
         results: List[Dict[str, Any]],
         creation_date: str,
         creation_user_id: str,
+        comparison_chat_id: Optional[str] = None,
     ):
         self.id = id
         self.text = text
         self.results = [ComparisonPromptResult.from_server_data(result) for result in results]
         self.creation_date = creation_date
         self.creation_user_id = creation_user_id
+        self.comparison_chat_id = comparison_chat_id
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id}, text={self.text[:1000]})"
 
     @classmethod
     def create(
         cls,
         llm_blueprints: List[Union[LLMBlueprint, str]],
         text: str,
+        comparison_chat: Optional[Union[ComparisonChat, str]] = None,
         wait_for_completion: bool = False,
     ) -> ComparisonPrompt:
         """
         Create a new ComparisonPrompt. This submits the prompt text to the LLM blueprints that
         are specified.
 
         Parameters
         ----------
         llm_blueprints : list[LLMBlueprint or str]
             The LLM blueprints associated with the created comparison prompt.
             Accepts LLM blueprints or IDs.
         text : str
             The prompt text.
+        comparison_chat: Optional[ComparisonChat or str], optional
+            The comparison chat to add the comparison prompt to. Accepts `ComparisonChat` or
+            comparison chat ID.
         wait_for_completion : bool
             If set to True code will wait for the chat prompt job to complete before
             returning the result (up to 10 minutes, raising timeout error after that).
             Otherwise, you can check current status by using ChatPrompt.get with returned ID.
 
         Returns
         -------
         comparison_prompt : ComparisonPrompt
             The created comparison prompt.
         """
         payload = {
             "llm_blueprint_ids": [
                 _get_genai_entity_id(llm_blueprint) for llm_blueprint in llm_blueprints
             ],
+            "comparison_chat_id": _get_genai_entity_id(comparison_chat)
+            if comparison_chat
+            else None,
             "text": text,
         }
 
         url = f"{cls._client.domain}/{cls._path}/"
         r_data = cls._client.post(url, data=payload)
         if wait_for_completion:
             location = wait_for_async_resolution(cls._client, r_data.headers["Location"])
@@ -220,43 +302,54 @@
         url = f"{cls._client.domain}/{cls._path}/{_get_genai_entity_id(comparison_prompt)}/"
         r_data = cls._client.get(url)
         return cls.from_server_data(r_data.json())
 
     @classmethod
     def list(
         cls,
-        llm_blueprints: List[Union[LLMBlueprint, str]],
+        llm_blueprints: Optional[List[Union[LLMBlueprint, str]]] = None,
+        comparison_chat: Optional[Union[ComparisonChat, str]] = None,
     ) -> List[ComparisonPrompt]:
         """
-        List all comparison prompts available to the user that include the specified LLM blueprints.
+        List all comparison prompts available to the user that include the specified LLM blueprints
+        or from the specified comparison chat.
 
         Parameters
         ----------
-        llm_blueprints : [List[Union[LLMBlueprint, str]]]
+        llm_blueprints : Optional[List[Union[LLMBlueprint, str]]], optional
             The returned comparison prompts are only those associated with the specified LLM
-            blueprints. Accepts either the entity or the ID.
+            blueprints. Accepts either `LLMBlueprint` or LLM blueprint ID.
+        comparison_chat : Optional[Union[ComparisonChat, str]], optional
+            The returned comparison prompts are only those associated with the specified comparison
+            chat. Accepts either `ComparisonChat` or comparison chat ID.
 
         Returns
         -------
         comparison_prompts : list[ComparisonPrompt]
             A list of comparison prompts available to the user that use the specified LLM
             blueprints.
         """
+        llm_blueprint_ids = (
+            [_get_genai_entity_id(llm_blueprint) for llm_blueprint in llm_blueprints]
+            if llm_blueprints
+            else None
+        )
+        comparison_chat_id = _get_genai_entity_id(comparison_chat) if comparison_chat else None
         params = {
-            "llm_blueprint_ids": [
-                _get_genai_entity_id(llm_blueprint) for llm_blueprint in llm_blueprints
-            ],
+            "llm_blueprint_ids": llm_blueprint_ids,
+            "comparison_chat_id": comparison_chat_id,
         }
         url = f"{cls._client.domain}/{cls._path}/"
         r_data = unpaginate(url, params, cls._client)
         return [cls.from_server_data(data) for data in r_data]
 
     def update(
         self,
-        additional_llm_blueprints: List[Union[LLMBlueprint, str]],
+        additional_llm_blueprints: Optional[List[Union[LLMBlueprint, str]]] = None,
+        feedback_result: Optional[FeedbackResult] = None,
         wait_for_completion: bool = False,
     ) -> ComparisonPrompt:
         """
         Update the comparison prompt.
 
         Parameters
         ----------
@@ -267,22 +360,29 @@
         -------
         comparison_prompt : ComparisonPrompt
             The updated comparison prompt.
         """
         payload = {
             "additionalLLMBlueprintIds": [
                 _get_genai_entity_id(bp) for bp in additional_llm_blueprints
-            ],
+            ]
+            if additional_llm_blueprints
+            else None,
+            "feedbackResult": feedback_result.to_dict() if feedback_result else None,
         }
         url = f"{self._client.domain}/{self._path}/{_get_genai_entity_id(self.id)}/"
         r_data = self._client.patch(url, data=payload)
-        if wait_for_completion:
+        if wait_for_completion and additional_llm_blueprints:
+            # If no additional_llm_blueprints then we get no location header
             location = wait_for_async_resolution(self._client, r_data.headers["Location"])
             return self.from_location(location)
-        return self.from_server_data(r_data.json())
+        else:
+            # Update route returns empty string so we need to GET here
+            r_data = self._client.get(url)
+            return self.from_server_data(r_data.json())
 
     def delete(self) -> None:
         """
         Delete the single comparison prompt.
         """
         url = f"{self._client.domain}/{self._path}/{_get_genai_entity_id(self.id)}/"
         self._client.delete(url)
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/custom_model_llm_validation.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/custom_model_llm_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,7 @@
     tenant_id : str
         Creating user's tenant ID.
     error_message : Optional[str]
         Additional information for errored validation.
     """
 
     _path = "api-gw/genai/customModelLLMValidations"
-
-    def delete(self) -> None:
-        """
-        Delete the custom model LLM validation.
-        """
-        url = f"{self._client.domain}/{self._path}/{self.id}/"
-        self._client.delete(url)
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/llm.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 from typing import Any, Dict, List, Optional, Union
 
 from mypy_extensions import TypedDict
 import trafaret as t
 
 from datarobot.models.api_object import APIObject
+from datarobot.models.use_cases.use_case import UseCase
+from datarobot.models.use_cases.utils import get_use_case_id
 from datarobot.utils import underscorize
 from datarobot.utils.pagination import unpaginate
 
 
 class BooleanConstraintsDict(TypedDict):
     type: str
 
@@ -296,25 +298,35 @@
         self.settings = [LLMSettingDefinition.from_server_data(setting) for setting in settings]
         self.context_size = context_size
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id}, name={self.name})"
 
     @classmethod
-    def list(cls, as_dict: bool = True) -> Union[List[LLMDefinition], List[LLMDefinitionDict]]:
+    def list(
+        cls, use_case: Optional[Union[UseCase, str]] = None, as_dict: bool = True
+    ) -> Union[List[LLMDefinition], List[LLMDefinitionDict]]:
         """
-        List all playgrounds associated with a specific use case available to the user.
+        List all large language models (LLMs) available to the user.
+
+        Parameters
+        ----------
+        use_case : Optional[UseCase or str], optional
+            The returned LLMs, including external LLMs, available
+            for the specified Use Case.
+            Accepts either the entity or the Use CaseID.
 
         Returns
         -------
         llms : list[LLMDefinition] or list[LLMDefinitionDict]
-            A list of large language models available to the user.
+            A list of large language models (LLMs) available to the user.
         """
         url = f"{cls._client.domain}/{cls._path}/"
-        r_data = unpaginate(url, None, cls._client)
+        params = {"use_case_id": get_use_case_id(use_case, is_required=False)}
+        r_data = unpaginate(url, params, cls._client)
         llms = [cls.from_server_data(data) for data in r_data]
 
         if as_dict:
             return [llm.to_dict() for llm in llms]
         return llms
 
     def to_dict(self) -> LLMDefinitionDict:
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/llm_blueprint.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/llm_blueprint.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 from __future__ import annotations
 
 from typing import Any, cast, Dict, List, Optional, Union
 
 from mypy_extensions import TypedDict
 import trafaret as t
 
+from datarobot._experimental.models.enums import PromptType
 from datarobot._experimental.models.genai.llm import LLMDefinition
 from datarobot._experimental.models.genai.playground import Playground
 from datarobot._experimental.models.genai.vector_database import VectorDatabase
+from datarobot.enums import enum_to_list
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model import CustomModelVersion
 from datarobot.utils import to_api
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 
@@ -62,22 +64,24 @@
 
 llm_blueprint_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("name"): t.String,
         t.Key("description"): t.String(allow_blank=True),
         t.Key("is_saved"): t.Bool,
+        t.Key("is_starred"): t.Bool,
         t.Key("playground_id"): t.String,
         t.Key("llm_id", optional=True): t.Or(t.String, t.Null),
         t.Key("llm_settings", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null),
         t.Key("llm_name", optional=True): t.Or(t.String, t.Null),
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
         t.Key("last_update_date"): t.String,
         t.Key("last_update_user_id"): t.String,
+        t.Key("prompt_type"): t.Enum(*enum_to_list(PromptType)),
         t.Key("vector_database_id", optional=True): t.Or(t.String, t.Null),
         t.Key("vector_database_settings", optional=True): t.Or(
             vector_database_settings_trafaret, t.Null
         ),
         t.Key("vector_database_name", optional=True): t.Or(t.String, t.Null),
         t.Key("vector_database_status", optional=True): t.Or(t.String, t.Null),
         t.Key("vector_database_error_message", optional=True): t.Or(t.String, t.Null),
@@ -128,15 +132,17 @@
         LLM blueprint ID.
     name : str
         LLM blueprint name.
     description : str
         Description of the LLM blueprint.
     is_saved : bool
         Whether the LLM blueprint is saved (settings are locked and blueprint is eligible for
-        use with ComparisonPrompts.)
+        use with ComparisonPrompts).
+    is_starred : bool
+        Whether the LLM blueprint is starred.
     playground_id : str
         ID of the Gen AI playground associated with the LLM blueprint.
     llm_id : str or None
         ID of the LLM type. If not None this must be one of the IDs returned by LLMDefinition.list
         for this user.
     llm_name : str or None
         Name of the LLM.
@@ -156,14 +162,17 @@
         Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     last_update_date : str
         Date when the playground was most recently updated.
     last_update_user_id : str
         ID of the user who most recently updated the playground.
+    prompt_type : PromptType
+        The prompting strategy for the LLM Blueprint.
+        Currently supported options are listed in PromptType.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
         The settings for the vector database associated with the LLM blueprint, if any.
     vector_database_name : str or None
         The name of the vector database associated with the LLM blueprint, if any.
     vector_database_status : str or None
@@ -186,19 +195,21 @@
 
     def __init__(
         self,
         id: str,
         name: str,
         description: str,
         is_saved: bool,
+        is_starred: bool,
         playground_id: str,
         creation_date: str,
         creation_user_id: str,
         last_update_date: str,
         last_update_user_id: str,
+        prompt_type: PromptType,
         llm_id: Optional[str] = None,
         llm_name: Optional[str] = None,
         llm_settings: Optional[Dict[str, Any]] = None,
         vector_database_id: Optional[str] = None,
         vector_database_settings: Optional[Dict[str, Any]] = None,
         vector_database_name: Optional[str] = None,
         vector_database_status: Optional[str] = None,
@@ -208,22 +219,24 @@
         custom_model_llm_error_message: Optional[str] = None,
         custom_model_llm_error_resolution: Optional[str] = None,
     ):
         self.id = id
         self.name = name
         self.description = description
         self.is_saved = is_saved
+        self.is_starred = is_starred
         self.playground_id = playground_id
         self.llm_id = llm_id
         self.llm_name = llm_name
         self.llm_settings = llm_settings
         self.creation_date = creation_date
         self.creation_user_id = creation_user_id
         self.last_update_date = last_update_date
         self.last_update_user_id = last_update_user_id
+        self.prompt_type = prompt_type
         self.vector_database_id = vector_database_id
         self.vector_database_settings = (
             VectorDatabaseSettings.from_server_data(vector_database_settings)
             if vector_database_settings
             else None
         )
         self.vector_database_name = vector_database_name
@@ -240,14 +253,15 @@
         )
 
     @classmethod
     def create(
         cls,
         playground: Union[Playground, str],
         name: str,
+        prompt_type: PromptType = PromptType.CHAT_HISTORY_AWARE,
         description: str = "",
         llm: Optional[Union[LLMDefinition, str]] = None,
         llm_settings: Optional[Dict[str, Optional[Union[bool, int, float, str]]]] = None,
         vector_database: Optional[Union[VectorDatabase, str]] = None,
         vector_database_settings: Optional[VectorDatabaseSettings] = None,
     ) -> LLMBlueprint:
         """
@@ -256,14 +270,16 @@
         Parameters
         ----------
         playground : Playground or str
             The playground associated with the created LLM blueprint.
             Accepts playground or playground ID.
         name : str
             LLM blueprint name.
+        prompt_type : PromptType, optional
+            Prompting type of the LLM Blueprint, by default PromptType.CHAT_HISTORY_AWARE.
         description : str, optional
             Description of the LLM blueprint, by default "".
         llm : LLMDefinition, str, or None, optional
             LLM to use for the blueprint. Accepts LLMDefinition or LLM ID.
         llm_settings : dict or None
             The LLM settings for the LLM blueprint. The specific keys allowed and the
             constraints on the values are defined in the response from LLMDefinition.list
@@ -286,14 +302,15 @@
         -------
         llm_blueprint : LLMBlueprint
             The created LLM blueprint.
         """
         payload = {
             "playground_id": get_entity_id(playground),
             "name": name,
+            "prompt_type": prompt_type,
             "description": description,
             "llm_id": get_entity_id(llm) if llm else None,
             "llm_settings": llm_settings,
             "vector_database_id": get_entity_id(vector_database) if vector_database else None,
             "vector_database_settings": vector_database_settings.to_dict()
             if vector_database_settings
             else None,
@@ -360,14 +377,15 @@
     @classmethod
     def list(
         cls,
         playground: Optional[Union[Playground, str]] = None,
         llms: Optional[List[Union[LLMDefinition, str]]] = None,
         vector_databases: Optional[List[Union[VectorDatabase, str]]] = None,
         is_saved: Optional[bool] = None,
+        is_starred: Optional[bool] = None,
         sort: Optional[str] = None,
     ) -> List[LLMBlueprint]:
         """
         Lists all LLM blueprints available to the user. If the playground is specified, then the
         results are restricted to the LLM blueprints associated with the playground. If the
         LLMs are specified, then the results are restricted to the LLM blueprints using those
         LLM types. If `vector_databases` are specified, then the results are restricted to the
@@ -382,14 +400,16 @@
             The returned LLM blueprints are filtered to those associated with the LLM types
             specified. Accepts either the entity or the ID.
         vector_databases : Optional[list[Union[VectorDatabase, str]]], optional
             The returned LLM blueprints are filtered to those associated with the vector databases
             specified. Accepts either the entity or the ID.
         is_saved: Optional[bool], optional
             The returned LLM blueprints are filtered to those matching is_saved.
+        is_starred: Optional[bool], optional
+            The returned LLM blueprints are filtered to those matching is_starred.
         sort : str, optional
             Property to sort LLM blueprints by.
             Prefix the attribute name with a dash to sort in descending order,
             e.g. sort='-creationDate'.
             Currently supported options are listed in ListLLMBlueprintsSortQueryParams
             but the values can differ with different platform versions.
             By default, the sort parameter is None which will result in
@@ -403,14 +423,15 @@
         params = {
             "playground_id": get_entity_id(playground) if playground else None,
             "llm_ids": [get_entity_id(llm) for llm in llms] if llms else None,
             "vector_databases": [get_entity_id(vdb) for vdb in vector_databases]
             if vector_databases
             else None,
             "is_saved": is_saved,
+            "is_starred": is_starred,
             "sort": sort,
         }
         url = f"{cls._client.domain}/{cls._path}/"
         r_data = unpaginate(url, params, cls._client)
         return [cls.from_server_data(data) for data in r_data]
 
     def update(
@@ -418,14 +439,16 @@
         name: Optional[str] = None,
         description: Optional[str] = None,
         llm: Optional[Union[LLMDefinition, str]] = None,
         llm_settings: Optional[Dict[str, Optional[Union[bool, int, float, str]]]] = None,
         vector_database: Optional[Union[VectorDatabase, str]] = None,
         vector_database_settings: Optional[VectorDatabaseSettings] = None,
         is_saved: Optional[bool] = None,
+        is_starred: Optional[bool] = None,
+        prompt_type: Optional[PromptType] = None,
         remove_vector_database: Optional[bool] = False,
     ) -> LLMBlueprint:
         """
         Update the LLM blueprint.
 
         Parameters
         ----------
@@ -449,14 +472,18 @@
             for custom model LLM blueprints.
         vector_database: Optional[Union[VectorDatabase, str]], optional
             The new vector database for the LLM blueprint.
         vector_database_settings: Optional[VectorDatabaseSettings], optional
             The new vector database settings for the LLM blueprint.
         is_saved: Optional[bool], optional
             The new is_saved attribute for the LLM blueprint.
+        is_starred: Optional[bool], optional
+            The new is_starred attribute for the LLM blueprint.
+        prompt_type : PromptType, optional
+            The new prompting type of the LLM Blueprint.
         remove_vector_database: Optional[bool], optional
             Whether to remove the vector database from the LLM blueprint.
 
         Returns
         -------
         llm_blueprint : LLMBlueprint
             The updated LLM blueprint.
@@ -467,14 +494,16 @@
             "llm_id": get_entity_id(llm) if llm else None,
             "llm_settings": llm_settings,
             "vector_database_id": get_entity_id(vector_database) if vector_database else None,
             "vector_database_settings": vector_database_settings.to_dict()
             if vector_database_settings
             else None,
             "is_saved": is_saved,
+            "is_starred": is_starred,
+            "prompt_type": prompt_type,
         }
         url = f"{self._client.domain}/{self._path}/{self.id}/"
         json_payload = cast(Dict[str, Any], to_api(payload))
         if remove_vector_database:  # This forces the removal of the vector database.
             json_payload["vectorDatabaseId"] = None
             json_payload["vectorDatabaseSettings"] = None
         r_data = self._client.patch(url, json=json_payload)
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/playground.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/playground.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/user_limits.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/user_limits.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/genai/vector_database.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/genai/vector_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,41 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
 import trafaret as t
 
 from datarobot._experimental.models.genai.custom_model_validation import CustomModelValidation
-from datarobot.errors import InvalidUsageError
+from datarobot._experimental.models.genai.playground import Playground
 from datarobot.models.api_object import APIObject
 from datarobot.models.use_cases.use_case import UseCase
 from datarobot.models.use_cases.utils import get_use_case_id, resolve_use_cases, UseCaseLike
 from datarobot.utils.pagination import unpaginate
 
+
+def get_entity_id(entity: Union[Playground, str]) -> str:
+    """
+    Get the entity ID from the entity parameter.
+
+    Parameters
+    ----------
+    entity : ApiObject or str
+        May be entity ID or the entity.
+
+    Returns
+    -------
+    id : str
+        Entity ID
+    """
+    if isinstance(entity, str):
+        return entity
+
+    return entity.id
+
+
 chunking_parameters_trafaret = t.Dict(
     {
         t.Key("embedding_model"): str,
         t.Key("chunking_method"): str,
         t.Key("chunk_size"): t.Int,
         t.Key("chunk_overlap_percentage"): t.Int,
         t.Key("separators"): t.List(t.String),
@@ -575,27 +596,31 @@
         r_data = cls._client.get(url)
         return cls.from_server_data(r_data.json())
 
     @classmethod
     def list(
         cls,
         use_case: Optional[UseCaseLike] = None,
+        playground: Optional[Union[Playground, str]] = None,
         search: Optional[str] = None,
         sort: Optional[str] = None,
         completed_only: Optional[bool] = None,
     ) -> List[VectorDatabase]:
         """
         List all vector databases associated with a specific use case available to the user.
 
         Parameters
         ----------
         use_case : Optional[UseCaseLike], optional
             The returned vector databases are filtered to those associated with a specific Use Case
             or Cases if specified or can be inferred from the Context.
             Accepts either the entity or the ID.
+        playground : Optional[Union[Playground, str]], optional
+            The returned vector databases are filtered to those associated with a specific playground
+            if it is specified. Accepts either the entity or the ID.
         search : str, optional
             String for filtering vector databases.
             Vector databases that contain the string in name will be returned.
             If not specified, all vector databases will be returned.
         sort : str, optional
             Property to sort vector databases by.
             Prefix the attribute name with a dash to sort in descending order,
@@ -613,23 +638,19 @@
         vectorbases : list[VectorDatabase]
             A list of vector databases available to the user.
         """
         params = {
             "search": search,
             "sort": sort,
             "completed_only": completed_only,
+            "playground_id": get_entity_id(playground) if playground else None,
         }
 
         params = resolve_use_cases(use_cases=use_case, params=params, use_case_key="use_case_id")
 
-        if "use_case_id" not in params:
-            raise InvalidUsageError(
-                "Use case was not specified and could not be inferred from the Context"
-            )
-
         url = f"{cls._client.domain}/{cls._path}/"
         r_data = unpaginate(url, params, cls._client)
         return [cls.from_server_data(data) for data in r_data]
 
     def update(self, name: str) -> VectorDatabase:
         """
         Update the vector database.
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/incremental_learning.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/incremental_learning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/key_values.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/lift_chart.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,203 +1,199 @@
 #
-# Copyright 2021-2024 DataRobot, Inc. and its affiliates.
+# Copyright 2021 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from __future__ import annotations
-
-from enum import Enum
+from typing import Any, Dict, Iterable, List, Mapping, Optional
 
+from mypy_extensions import TypedDict
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.models.api_object import APIObject
 
+LiftChartBinsTrafaret = t.Dict(
+    {
+        t.Key("bins"): t.List(
+            t.Dict(
+                {
+                    t.Key("actual"): t.Float,
+                    t.Key("predicted"): t.Float,
+                    t.Key("bin_weight"): t.Float,
+                }
+            ).ignore_extra("*")
+        )
+    }
+)
+
+
+class LiftChartBin(TypedDict):
+    actual: float
+    predicted: float
+    bin_weight: float
 
-class KeyValueEntityType(Enum):
-    """Key-Value entity type"""
-
-    DEPLOYMENT = "deployment"
-    MODEL_PACKAGE = "modelPackage"
-    REGISTERED_MODEL = "registeredModel"
-    CUSTOM_JOB = "customJob"
-    CUSTOM_JOB_RUN = "customJobRun"
-
-
-class KeyValueType(Enum):
-    """Key-Value type"""
-
-    BINARY = "binary"
-    BOOLEAN = "boolean"
-    CREDENTIAL = "credential"
-    DEPLOYMENT_ID = "deploymentId"
-    DATASET = "dataset"
-    IMAGE = "image"
-    JSON = "json"
-    MODEL_VERSION = "modelVersion"
-    NUMERIC = "numeric"
-    PICKLE = "pickle"
-    STRING = "string"
-    URL = "url"
-    YAML = "yaml"
-
-
-class KeyValueCategory(Enum):
-    """Key-Value category"""
-
-    TRAINING_PARAMETER = "trainingParameter"
-    METRIC = "metric"
-    TAG = "tag"
-    ARTIFACT = "artifact"
-    RUNTIME_PARAMETER = "runtimeParameter"
 
+class LiftChartData(TypedDict):
+    bins: List[LiftChartBin]
 
-class KeyValue(APIObject):
-    """A DataRobot Key-Value.
 
-    .. versionadded:: v2.33
+class LiftChartServerData(TypedDict):
+    id: str
+    entity_id: str
+    project_id: str
+    source: str
+    data_slice_id: Optional[str]
+    data: LiftChartData
+
+
+class LiftChart(APIObject):
+    """ Lift chart data for model.
+
+    Notes
+    -----
+    ``LiftChartBin`` is a dict containing the following:
+
+        * ``actual`` (float) Sum of actual target values in bin
+        * ``predicted`` (float) Sum of predicted target values in bin
+        * ``bin_weight`` (float) The weight of the bin. For weighted projects, it is the sum of \
+          the weights of the rows in the bin. For unweighted projects, it is the number of rows in \
+          the bin.
 
     Attributes
     ----------
-    id: str
-        ID of the Key-Value
-    created_at: str
-        creation time of the Key-Value
-    entity_id: str
-        ID of the related Entity
-    entity_type: KeyValueEntityType
-        type of the related Entity
-    name: str
-        Key-Value name
-    value: str
-        Key-Value value
-    numeric_value: float
-        Key-Value numeric value
-    boolean_value: bool
-        Key-Value boolean value
-    value_type: KeyValueType
-        Key-Value type
-    description: str
-        Key-Value description
-    creator_id: str
-        ID of the user who created the Key-Value
-    creator_name: str
-        ID of the user who created the Key-Value
-    category: KeyValueCategory
-        Key-Value category
-    artifact_size: int
-        size in bytes of associated image, if applicable
-    original_file_name: str
-        name of uploaded original image or dataset file
-    is_editable: bool
-        true if a user with permissions can edit or delete
-    is_dataset_missing: bool
-        true if the key-value type is "dataset" and its dataset is not visible to the user
-    error_message: str
-        additional information if "isDataSetMissing" is true. Blank if there are no errors
+    source : str
+        Lift chart data source. Can be 'validation', 'crossValidation' or 'holdout'.
+    bins : list of dict
+        List of dicts with schema described as ``LiftChartBin`` above.
+    source_model_id : str
+        ID of the model this lift chart represents; in some cases,
+        insights from the parent of a frozen model may be used
+    target_class : str, optional
+        For multiclass lift - target class for this lift chart data.
+    data_slice_id: string or None
+        The slice to retrieve Lift Chart for; if None, retrieve unsliced data.
     """
 
-    _path = "keyValues/"
+    _converter = (
+        t.Dict(
+            {
+                t.Key("source"): String,
+                t.Key("source_model_id"): String,
+                t.Key("target_class", optional=True, default=None): t.Or(String, t.Null),
+                t.Key("data_slice_id", optional=True): t.Or(String, t.Null),
+            }
+        )
+        .merge(LiftChartBinsTrafaret)
+        .ignore_extra("*")
+    )
+
+    def __init__(self, source, bins, source_model_id, target_class, data_slice_id=None):
+        self.source = source
+        self.bins = bins
+        self.source_model_id = source_model_id
+        self.target_class = target_class
+        self.data_slice_id = data_slice_id
+
+    def __repr__(self):
+        additional_params = ""
+        if self.target_class:
+            additional_params += f"{self.target_class}:"
+        if self.data_slice_id:
+            additional_params += f"{self.data_slice_id}:"
+        return f"LiftChart({additional_params}{self.source})"
+
+    @staticmethod
+    def _repack_insights_response(server_data: LiftChartServerData):
+        """Repack the JSON sent by the GET /insights/ endpoint to match the format expected by the
+        insight APIObject class.
+
+        Parameters
+        ----------
+        server_data : dict
+        {
+            "id": "6474726c7ca961a4ebce068d",
+            "entityId": "64747242956c7390bb15b206",
+            "projectId": "647471b6b5d9cbd454f2cf63",
+            "source": "validation",
+            "dataSliceId": "647471b6b5d9cbd454f2ab99",
+            "data": {"bins": [{"actual":0.0, "predicted":0.0, "binWeight":27.0}, ...]}
+        }
 
-    _converter = t.Dict(
+        Returns
+        -------
+        dict
         {
-            t.Key("id"): String(),
-            t.Key("created_at"): String(),
-            t.Key("entity_id"): String(),
-            t.Key("entity_type"): t.Enum(*[e.value for e in KeyValueEntityType]),
-            t.Key("name"): String(),
-            t.Key("value"): String(),
-            t.Key("numeric_value"): t.Float(),
-            t.Key("boolean_value", optional=True, default=False): t.Bool(),
-            t.Key("value_type"): t.Enum(*[e.value for e in KeyValueType]),
-            t.Key("description"): String(allow_blank=True),
-            t.Key("creator_id"): String(),
-            t.Key("creator_name"): String(),
-            t.Key("category"): t.Enum(*[e.value for e in KeyValueCategory]),
-            t.Key("artifact_size"): t.Int(),
-            t.Key("original_file_name"): String(allow_blank=True),
-            t.Key("is_editable"): t.Bool(),
-            t.Key("is_dataset_missing"): t.Bool(),
-            t.Key("error_message"): String(allow_blank=True),
+            "source": "validation",
+            "bins": [{"actual":0.0, "predicted":0.0, "binWeight":27.0}, ...],
+            "sourceModelId": "64747242956c7390bb15b206",
+            "dataSliceId": "647471b6b5d9cbd454f2ab99",
+        }
+        """
+        return {
+            "source": server_data["source"],
+            "bins": server_data["data"]["bins"],
+            "sourceModelId": server_data["entityId"],
+            "dataSliceId": server_data["dataSliceId"],
         }
-    ).ignore_extra("*")
 
-    schema = _converter
+    @classmethod
+    def from_server_data(cls, data, keep_attrs=None, use_insights_format=False, **kwargs):
+        """
+        Overwrite APIObject.from_server_data to handle lift chart data retrieved
+        from either legacy URL or /insights/ new URL.
 
-    def __init__(
-        self,
-        id: str,
-        created_at: str,
-        entity_id: str,
-        entity_type: KeyValueEntityType,
-        name: str,
-        value: str,
-        numeric_value: float,
-        boolean_value: bool,
-        value_type: KeyValueType,
-        description: str,
-        creator_id: str,
-        creator_name: str,
-        category: KeyValueCategory,
-        artifact_size: int,
-        original_file_name: str,
-        is_editable: bool,
-        is_dataset_missing: bool,
-        error_message: str,
-    ) -> None:
-        self.id = id
-        self.created_at = created_at
-        self.entity_id = entity_id
-        self.entity_type = KeyValueEntityType(entity_type)
-        self.name = name
-        self.value = value
-        self.numeric_value = numeric_value
-        self.boolean_value = boolean_value
-        self.value_type = KeyValueType(value_type)
-        self.description = description
-        self.creator_id = creator_id
-        self.creator_name = creator_name
-        self.category = KeyValueCategory(category)
-        self.artifact_size = artifact_size
-        self.original_file_name = original_file_name
-        self.is_editable = is_editable
-        self.is_dataset_missing = is_dataset_missing
-        self.error_message = error_message
+        Parameters
+        ----------
+        data : dict
+            The directly translated dict of JSON from the server. No casing fixes have
+            taken place
+        use_insights_format : bool, optional
+            Whether to repack the data from the format used in the GET /insights/liftChart/ URL
+            to the format used in the legacy URL.
+        """
+        if use_insights_format:
+            data = cls._repack_insights_response(data)
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.name or self.id!r})"
+        return super().from_server_data(data=data, keep_attrs=keep_attrs)
 
-    @classmethod
-    def _key_value_path(cls, key_value_id: str) -> str:
-        return f"{cls._path}{key_value_id}/"
 
-    @classmethod
-    def get(cls, key_value_id: str) -> KeyValue:
-        """Get Key-Value by id.
+class SlicedLiftChart(LiftChart):
+    """Wrapper around LiftChart to override `from_server_data` method"""
 
-        .. versionadded:: v2.33
+    @classmethod
+    # type: ignore[override]
+    def from_server_data(
+        cls,
+        data: Dict[str, Any],
+        keep_attrs: Optional[Iterable[str]] = None,
+        use_insights_format: bool = True,
+        **kwargs: Mapping[str, Any],
+    ) -> "LiftChart":
+        """
+        Overwrite LiftChart.from_server_data to set `use_insights_format=True` by default
+        This is necessary for the correct transformation of data received from /insights endpoints
 
         Parameters
         ----------
-        key_value_id: str
-            ID of the Key-Value
-
-        Returns
-        -------
-        KeyValue
-            retrieved Key-Value
-
-        Raises
-        ------
-        datarobot.errors.ClientError
-            if the server responded with 4xx status.
-        datarobot.errors.ServerError
-            if the server responded with 5xx status.
+        data : dict
+            The directly translated dict of JSON from the server. No casing fixes have
+            taken place.
+        keep_attrs : iterable
+            List, set or tuple of the dotted namespace notations for attributes to keep within the
+            object structure even if their values are None
+        use_insights_format : bool, optional
+            Whether to repack the data from the format used in the GET /insights/liftChart/ URL
+            to the format used in the legacy URL.
         """
-        path = cls._key_value_path(key_value_id)
-        return cls.from_location(path)
+        if data.get("count"):
+            # it's a list
+            data = data["data"][0]
+
+        return super().from_server_data(
+            data=data, keep_attrs=keep_attrs, use_insights_format=use_insights_format, **kwargs
+        )
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/notebooks.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/recipe_operations.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipe_operations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/recipes.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/recipes.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/analytics.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/client.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/config.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/config.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/context.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/enums.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
 class TARGET_TYPE:
     BINARY = "Binary"
     MULTICLASS = "Multiclass"
     MULTILABEL = "Multilabel"
     REGRESSION = "Regression"
     UNSTRUCTURED = "Unstructured"
     ANOMALY = "Anomaly"
-    ALL = [BINARY, MULTICLASS, MULTILABEL, REGRESSION, UNSTRUCTURED, ANOMALY]
+    TEXT_GENERATION = "TextGeneration"
+    ALL = [BINARY, MULTICLASS, MULTILABEL, REGRESSION, UNSTRUCTURED, ANOMALY, TEXT_GENERATION]
 
 
 JOB_TYPE = enum(
     BATCH_MONITORING="batchMonitoring",
     BATCH_PREDICTIONS="batchPredictions",
     BATCH_PREDICTION_JOB_DEFINITIONS="batchPredictionJobDefinitions",
     FEATURE_IMPACT="featureImpact",
@@ -552,15 +553,15 @@
     ALL = [BINARY, ANOMALY, REGRESSION, MULTICLASS, TEXT_GENERATION]
 
 
 class CUSTOM_MODEL_TARGET_TYPE(_SHARED_TARGET_TYPE):
     """Enum of valid custom model target types"""
 
     UNSTRUCTURED = "Unstructured"
-    REQUIRES_TARGET_NAME = ("Binary", "Multiclass", "Regression")
+    REQUIRES_TARGET_NAME = ("Binary", "Multiclass", "Regression", "TextGeneration")
 
     ALL = _SHARED_TARGET_TYPE.ALL + [UNSTRUCTURED]
 
 
 class CUSTOM_TASK_TARGET_TYPE(_SHARED_TARGET_TYPE):
     """Enum of valid custom task target types"""
 
@@ -1112,16 +1113,17 @@
     """
 
     PASSING = "passing"
     WARNING = "warning"
     FAILING = "failing"
     UNKNOWN = "unknown"
     UNAVAILABLE = "unavailable"
+    NOT_APPLICABLE = "notApplicable"
 
-    ALL = [PASSING, WARNING, FAILING, UNKNOWN, UNAVAILABLE]
+    ALL = [PASSING, WARNING, FAILING, UNKNOWN, UNAVAILABLE, NOT_APPLICABLE]
 
 
 class DocumentTextExtractionMethod:
     OCR = "TESSERACT_OCR"
     EMBEDDED = "DOCUMENT_TEXT_EXTRACTOR"
 
     ALL = [OCR, EMBEDDED]
@@ -1164,7 +1166,75 @@
     ) -> Optional["CustomTaskOutgoingNetworkPolicy"]:
         if input_string is None:
             return None
         for el in cls:
             if el.name == input_string:
                 return el
         raise ValueError(f"{input_string!r} does not match any of {[el.name for el in cls]}")
+
+
+class CustomMetricDirectionality:
+    HIGHER_IS_BETTER = "higherIsBetter"
+    LOWER_IS_BETTER = "lowerIsBetter"
+    ALL = [HIGHER_IS_BETTER, LOWER_IS_BETTER]
+
+
+class CustomMetricAggregationType:
+    SUM = "sum"
+    AVERAGE = "average"
+    GAUGE = "gauge"
+    ALL = [SUM, AVERAGE, GAUGE]
+
+
+class CustomMetricBucketTimeStep:
+    HOUR = "hour"
+    ALL = [HOUR]
+
+
+class KeyValueEntityType(Enum):
+    """Key-Value entity type"""
+
+    DEPLOYMENT = "deployment"
+    MODEL_PACKAGE = "modelPackage"
+    REGISTERED_MODEL = "registeredModel"
+    CUSTOM_JOB = "customJob"
+    CUSTOM_JOB_RUN = "customJobRun"
+
+
+class KeyValueType(Enum):
+    """Key-Value type"""
+
+    BINARY = "binary"
+    BOOLEAN = "boolean"
+    CREDENTIAL = "credential"
+    DEPLOYMENT_ID = "deploymentId"
+    DATASET = "dataset"
+    IMAGE = "image"
+    JSON = "json"
+    MODEL_VERSION = "modelVersion"
+    NUMERIC = "numeric"
+    PICKLE = "pickle"
+    STRING = "string"
+    URL = "url"
+    YAML = "yaml"
+
+
+class KeyValueCategory(Enum):
+    """Key-Value category"""
+
+    TRAINING_PARAMETER = "trainingParameter"
+    METRIC = "metric"
+    TAG = "tag"
+    ARTIFACT = "artifact"
+    RUNTIME_PARAMETER = "runtimeParameter"
+
+
+class ExportStatus:
+    """A prediction data export processing state."""
+
+    CREATED = "CREATED"
+    SCHEDULED = "SCHEDULED"
+    CANCELLED = "CANCELLED"
+    FAILED = "FAILED"
+    SUCCEEDED = "SUCCEEDED"
+
+    ALL = [CREATED, SCHEDULED, CANCELLED, FAILED, SUCCEEDED]
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/errors.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/__init__.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/base.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from typing import Any, cast, Dict, Iterable, List, Optional
+from typing import Any, cast, Dict, Iterable, List, Optional, Union
 
 import trafaret as t
 from typing_extensions import Self
 
 from datarobot.enums import DEFAULT_MAX_WAIT, INSIGHTS_SOURCES
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models import StatusCheckJob
@@ -146,45 +146,47 @@
         if all(attrib in data for attrib in ["count", "next", "previous"]):
             # If true, the data response is a paginated response from a compute command and the data
             # entity should be unwrapped. There should only be one response.
             data = data["data"][0]
 
         return super().from_server_data(data=data, keep_attrs=keep_attrs)
 
-    @staticmethod
+    @classmethod
     def _get_payload(
+        cls,
         entity_id: str,
         source: str = INSIGHTS_SOURCES.VALIDATION,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
         **kwargs: Any,
-    ) -> Dict[str, str]:
+    ) -> Dict[str, Union[str, int]]:
         """Construct a payload for a compute request
 
         May be override by insight subclasses to accept additional parameters
         """
         _ = kwargs
         payload = {
             "entityId": entity_id,
             "source": source,
         }
         if data_slice_id is not None:
             payload["dataSliceId"] = data_slice_id
         if external_dataset_id is not None:
             payload["externalDatasetId"] = external_dataset_id
 
-        return payload
+        return cast(Dict[str, Union[str, int]], payload)
 
     @classmethod
     def compute(
         cls,
         entity_id: str,
         source: str = INSIGHTS_SOURCES.VALIDATION,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
+        **kwargs: Any,
     ) -> StatusCheckJob:
         """Submit an insight compute request. You can use `create` if you want to
         wait synchronously for the completion of the job.
 
         May be override by insight subclasses to accept additional parameters
 
         Parameters
@@ -204,27 +206,29 @@
             Status check job entity for the asynchronous insight calculation
         """
         payload = cls._get_payload(
             entity_id=entity_id,
             source=source,
             data_slice_id=data_slice_id,
             external_dataset_id=external_dataset_id,
+            **kwargs,
         )
         response = cls._client.post(cls._compute_url(), data=payload)
 
         return StatusCheckJob.from_response(response, cls)
 
     @classmethod
     def create(
         cls,
         entity_id: str,
         source: str = INSIGHTS_SOURCES.VALIDATION,
         data_slice_id: Optional[str] = None,
         external_dataset_id: Optional[str] = None,
         max_wait: Optional[int] = DEFAULT_MAX_WAIT,
+        **kwargs: Any,
     ) -> Self:
         """Create an insight and wait for completion
 
         May be override by insight subclasses to accept additional parameters
 
         Parameters
         ----------
@@ -245,14 +249,15 @@
             Entity of the newly or already computed insights
         """
         status_check_job = cls.compute(
             entity_id=entity_id,
             source=source,
             data_slice_id=data_slice_id,
             external_dataset_id=external_dataset_id,
+            **kwargs,
         )
         return cast(Self, status_check_job.get_result_when_complete(max_wait=cast(int, max_wait)))
 
     @classmethod
     def list(cls, entity_id: str) -> List[Self]:
         """List all generated insights
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/shap_matrix.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/insights/shap_preview.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/insights/shap_preview.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/__init__.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
+import datarobot.models.registry
+
 from .application import Application
 from .automated_documentation import AutomatedDocument
 from .batch_monitoring_job import BatchMonitoringJob, BatchMonitoringJobDefinition
 from .batch_prediction_job import BatchPredictionJob, BatchPredictionJobDefinition
 from .blueprint import Blueprint, BlueprintChart, BlueprintTaskDocument, ModelBlueprintChart
 from .calendar_file import CalendarFile
 from .change_request import ChangeRequest, ChangeRequestReview
@@ -61,14 +63,15 @@
     FeatureEffectMetadataDatetimePerBacktest,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
 from .featurelist import DatasetFeaturelist, Featurelist, ModelingFeaturelist
 from .imported_model import ImportedModel
 from .job import FeatureImpactJob, Job, TrainingPredictionsJob
+from .key_values import KeyValue
 from .model import (
     BlenderModel,
     ClusteringModel,
     CombinedModel,
     DatetimeModel,
     FrozenModel,
     GenericModel,
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/api_object.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/application.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/batch_job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/batch_prediction_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
             t.Key("explanation_num_top_classes", optional=True): t.Int(),
             t.Key("deployment_id", optional=True): String(),
             t.Key("model_id", optional=True): String(),
             t.Key("passthrough_columns", optional=True): t.List(String(allow_blank=True)),
             t.Key("passthrough_columns_set", optional=True): String(),
             t.Key("max_explanations", optional=True): Int(),
             t.Key("max_ngram_explanations", optional=True): t.Int(gte=0) | t.Atom("all"),
+            t.Key("explanation_algorithm", optional=True): String(),
             t.Key("prediction_threshold", optional=True): t.Float(gte=0.0, lte=1.0) | t.Null(),
             t.Key("prediction_warning_enabled", optional=True): t.Bool(),
             t.Key("intake_settings", optional=True): t.Dict().allow_extra("*"),
             t.Key("output_settings", optional=True): t.Dict().allow_extra("*"),
             t.Key("timeseries_settings", optional=True): t.Dict().allow_extra("*"),
         }
     ).allow_extra("*")
@@ -203,14 +204,15 @@
         timeseries_settings: Optional[TimeSeriesSettings] = None,
         num_concurrent: Optional[int] = None,
         chunk_size: Optional[Union[int, str]] = None,
         passthrough_columns: Optional[List[str]] = None,
         passthrough_columns_set: Optional[str] = None,
         max_explanations: Optional[int] = None,
         max_ngram_explanations: Optional[Union[int, str]] = None,
+        explanation_algorithm: Optional[str] = None,
         threshold_high: Optional[float] = None,
         threshold_low: Optional[float] = None,
         prediction_threshold: Optional[float] = None,
         prediction_warning_enabled: Optional[bool] = None,
         include_prediction_status: bool = False,
         skip_drift_tracking: bool = False,
         prediction_instance: Optional[PredictionInstance] = None,
@@ -238,14 +240,17 @@
 
         if max_explanations is not None:
             job_data["maxExplanations"] = int(max_explanations)
 
         if max_ngram_explanations is not None:
             job_data["maxNgramExplanations"] = max_ngram_explanations
 
+        if explanation_algorithm is not None:
+            job_data["explanationAlgorithm"] = explanation_algorithm
+
         if threshold_high is not None:
             job_data["thresholdHigh"] = float(threshold_high)
 
         if threshold_low is not None:
             job_data["thresholdLow"] = float(threshold_low)
 
         if prediction_threshold is not None:
@@ -388,14 +393,15 @@
         timeseries_settings: Optional[TimeSeriesSettings] = None,
         num_concurrent: Optional[int] = None,
         chunk_size: Optional[Union[int, str]] = None,
         passthrough_columns: Optional[List[str]] = None,
         passthrough_columns_set: Optional[str] = None,
         max_explanations: Optional[int] = None,
         max_ngram_explanations: Optional[Union[int, str]] = None,
+        explanation_algorithm: Optional[str] = None,
         threshold_high: Optional[float] = None,
         threshold_low: Optional[float] = None,
         prediction_threshold: Optional[float] = None,
         prediction_warning_enabled: Optional[bool] = None,
         include_prediction_status: bool = False,
         skip_drift_tracking: bool = False,
         prediction_instance: Optional[PredictionInstance] = None,
@@ -687,14 +693,15 @@
             timeseries_settings=timeseries_settings,
             num_concurrent=num_concurrent,
             chunk_size=chunk_size,
             passthrough_columns=passthrough_columns,
             passthrough_columns_set=passthrough_columns_set,
             max_explanations=max_explanations,
             max_ngram_explanations=max_ngram_explanations,
+            explanation_algorithm=explanation_algorithm,
             threshold_high=threshold_high,
             threshold_low=threshold_low,
             prediction_threshold=prediction_threshold,
             prediction_warning_enabled=prediction_warning_enabled,
             include_prediction_status=include_prediction_status,
             skip_drift_tracking=skip_drift_tracking,
             prediction_instance=prediction_instance,
@@ -1296,14 +1303,15 @@
         output_settings: Optional[OutputSettings] = None,
         csv_settings: Optional[CsvSettings] = None,
         timeseries_settings: Optional[TimeSeriesSettings] = None,
         passthrough_columns: Optional[List[str]] = None,
         passthrough_columns_set: Optional[str] = None,
         max_explanations: Optional[int] = None,
         max_ngram_explanations: Optional[Union[int, str]] = None,
+        explanation_algorithm: Optional[str] = None,
         threshold_high: Optional[float] = None,
         threshold_low: Optional[float] = None,
         prediction_threshold: Optional[float] = None,
         prediction_warning_enabled: Optional[bool] = None,
         include_prediction_status: bool = False,
         abort_on_error: bool = True,
         column_names_remapping: Optional[Dict[str, str]] = None,
@@ -1526,14 +1534,15 @@
             output_settings=output_settings,
             csv_settings=csv_settings,
             timeseries_settings=timeseries_settings,
             passthrough_columns=passthrough_columns,
             passthrough_columns_set=passthrough_columns_set,
             max_explanations=max_explanations,
             max_ngram_explanations=max_ngram_explanations,
+            explanation_algorithm=explanation_algorithm,
             threshold_high=threshold_high,
             threshold_low=threshold_low,
             prediction_threshold=prediction_threshold,
             prediction_warning_enabled=prediction_warning_enabled,
             include_prediction_status=include_prediction_status,
             abort_on_error=abort_on_error,
             column_names_remapping=column_names_remapping,
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/blueprint.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/calendar_file.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/change_request.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/cluster.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/connector.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/credential.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/credential.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,14 +228,15 @@
     @classmethod
     def create_s3(
         cls,
         name: str,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
+        config_id: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Credential:
         """
         Creates the S3 credentials.
 
         Parameters
         ----------
@@ -243,14 +244,17 @@
             the name to use for this set of credentials.
         aws_access_key_id : str, optional
             the AWS access key id.
         aws_secret_access_key : str, optional
             the AWS secret access key.
         aws_session_token : str, optional
             the AWS session token.
+        config_id: str, optional
+            The ID of the saved shared secure configuration. If specified, cannot include awsAccessKeyId,
+            awsSecretAccessKey or awsSessionToken.
         description : str, optional
             the description to use for this set of credentials.
 
         Returns
         -------
         credential : Credential
             the created credential.
@@ -271,16 +275,18 @@
         """
         payload = {
             "name": name,
             "credentialType": CredentialTypes.S3.value,
             "awsAccessKeyId": aws_access_key_id,
             "awsSecretAccessKey": aws_secret_access_key,
             "awsSessionToken": aws_session_token,
+            "configId": config_id,
             "description": description,
         }
+        payload = {key: value for key, value in payload.items() if value is not None}
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
     @classmethod
     def create_azure(
         cls,
         name: str,
         azure_connection_string: str,
@@ -344,15 +350,15 @@
             the Snowflake login name
         private_key: str, optional
             the private key copied exactly from user private key file. Since it contains multiple
             lines, when assign to a variable, put the key string inside triple-quotes
         passphrase: str, optional
             the string used to encrypt the private key
         config_id: str, optional
-            The ID of the saved shared credentials. If specified, cannot include user,
+            The ID of the saved shared secure configuration. If specified, cannot include user,
             privateKeyStr or passphrase.
         description : str, optional
             the description to use for this set of credentials.
 
         Returns
         -------
         credential : Credential
@@ -429,29 +435,33 @@
         payload = {key: value for key, value in payload.items() if value is not None}
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
     @classmethod
     def create_databricks_service_principal(
         cls,
         name: str,
-        client_id: str,
-        client_secret: str,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        config_id: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Credential:
         """
         Creates the Databricks access token credentials.
 
         Parameters
         ----------
         name : str
             the name to use for this set of credentials.
         client_id: str, optional
             the client ID for Databricks Service Principal
         client_secret: str, optional
             the client secret for Databricks Service Principal
+        config_id: str, optional
+            The ID of the saved shared secure configuration. If specified, cannot include clientId
+            and clientSecret.
         description : str, optional
             the description to use for this set of credentials.
 
         Returns
         -------
         credential : Credential
             the created credential.
@@ -470,14 +480,15 @@
             Credential('5e429d6ecf8a5f36c5693e03', 'svc_principal_cred', 'databricks_service_principal_account'),
         """
         payload = {
             "name": name,
             "credentialType": CredentialTypes.DATABRICKS_SERVICE_PRINCIPAL.value,
             "clientId": client_id,
             "clientSecret": client_secret,
+            "configId": config_id,
             "description": description,
         }
         payload = {key: value for key, value in payload.items() if value is not None}
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
     def __repr__(self) -> str:
         return "{}('{}', '{}', '{}')".format(
@@ -577,14 +588,15 @@
 
 S3CredentialsSchema = t.Dict(
     {
         t.Key("credentialType"): t.Atom("s3"),
         t.Key("awsAccessKeyId", optional=True): String(),
         t.Key("awsSecretAccessKey", optional=True): String(),
         t.Key("awsSessionToken", optional=True): String(),
+        t.Key("configId", optional=True): String(),
     }
 ).allow_extra("*")
 
 OauthCredentialsSchema = t.Dict(
     {
         t.Key("credentialType"): t.Atom("oauth"),
         t.Key("oauthRefreshToken"): String(),
@@ -610,16 +622,17 @@
         t.Key("databricksAccessToken"): String(),
     }
 ).allow_extra("*")
 
 DatabricksServicePrincipalCredentialsSchema = t.Dict(
     {
         t.Key("credentialType"): t.Atom("databricks_service_principal_account"),
-        t.Key("clientId"): String(),
-        t.Key("clientSecret"): String(),
+        t.Key("clientId", optional=True): String(),
+        t.Key("clientSecret", optional=True): String(),
+        t.Key("configId", optional=True): String(),
     }
 ).allow_extra("*")
 
 AnyCredentialsSchema = t.Dict({t.Key("credentialType"): String()}).allow_extra("*")
 
 CredentialDataSchema = t.Or(
     BasicCredentialsSchema,
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_model.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,34 @@
 from __future__ import annotations
 
 from typing import Any, cast, Dict, List, Optional, Type, TypeVar
 
 import trafaret as t
 
 from datarobot._compat import Int, String
-from datarobot.enums import (
-    CUSTOM_MODEL_TARGET_TYPE,
-    DEFAULT_MAX_WAIT,
-    NETWORK_EGRESS_POLICY,
-    TARGET_TYPE,
-)
+from datarobot.enums import CUSTOM_MODEL_TARGET_TYPE, NETWORK_EGRESS_POLICY, TARGET_TYPE
 from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import CustomModelVersion
-from datarobot.utils import deprecated
 from datarobot.utils.pagination import unpaginate
-from datarobot.utils.waiters import wait_for_async_resolution
 
 T_CustomModelBase = TypeVar("T_CustomModelBase", bound="_CustomModelBase")
 
 
 class _CustomModelBase(APIObject):  # pylint: disable=missing-class-docstring
     _path = "customModels/"
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("name"): String(),
             t.Key("description"): String(allow_blank=True),
             t.Key("supports_binary_classification", optional=True, default=False): t.Bool(),
             t.Key("supports_regression", optional=True, default=False): t.Bool(),
+            t.Key("supports_textgeneration", optional=True, default=False): t.Bool(),
             t.Key("latest_version", optional=True, default=None): t.Or(
                 CustomModelVersion.schema, t.Null()
             ),
             t.Key("deployments_count", optional=True, default=None): Int(),
             t.Key("created_by"): String(),
             t.Key("updated") >> "updated_at": String(),
             t.Key("created") >> "created_at": String(),
@@ -62,47 +56,57 @@
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
         id: str,
         name: str,
         description: str,
         supports_binary_classification: bool,
         supports_regression: bool,
+        supports_textgeneration: bool,
         latest_version: CustomModelVersion,
         deployments_count: int,
         created_by: str,
         updated_at: str,
         created_at: str,
         target_type: str,
     ) -> None:
         self.id = id
         self.name = name
         self.description = description
 
         self.target_type = target_type
-        if supports_binary_classification and supports_regression:
+        if supports_binary_classification + supports_regression + supports_textgeneration > 1:
             raise ValueError("Model should support only 1 target type")
 
         if not target_type:
             if supports_binary_classification:
                 self.target_type = CUSTOM_MODEL_TARGET_TYPE.BINARY
             elif supports_regression:
                 self.target_type = CUSTOM_MODEL_TARGET_TYPE.REGRESSION
+            elif supports_textgeneration:
+                self.target_type = CUSTOM_MODEL_TARGET_TYPE.TEXT_GENERATION
             else:
                 raise ValueError("Target type must be provided")
         else:
             if target_type != CUSTOM_MODEL_TARGET_TYPE.BINARY and supports_binary_classification:
                 raise ValueError(
                     "Cannot specify both target_type {} and "
                     "supports_binary_classification.".format(target_type)
                 )
             elif target_type != CUSTOM_MODEL_TARGET_TYPE.REGRESSION and supports_regression:
                 raise ValueError(
                     "Cannot specify both target_type {} and "
                     "supports_regression.".format(target_type)
                 )
+            elif (
+                target_type != CUSTOM_MODEL_TARGET_TYPE.TEXT_GENERATION and supports_textgeneration
+            ):
+                raise ValueError(
+                    "Cannot specify both target_type {} and "
+                    "supports_text_generation.".format(target_type)
+                )
 
         self.latest_version = CustomModelVersion(**latest_version) if latest_version else None  # type: ignore[arg-type]
         self.deployments_count = deployments_count
         self.created_by = created_by
         self.updated_at = updated_at
         self.created_at = created_at
 
@@ -384,15 +388,15 @@
         Can be "python", "r", "java" or "other".
     description: str
         The description of the custom inference model.
     target_type: datarobot.TARGET_TYPE
         Target type of the custom inference model.
         Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
         `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`,
-        `datarobot.TARGET_TYPE.ANOMALY`]
+        `datarobot.TARGET_TYPE.ANOMALY`, `datarobot.TARGET_TYPE.TEXT_GENERATION`]
     target_name: str, optional
         Target feature name.
         It is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED`
         or `datarobot.TARGET_TYPE.ANOMALY` target type.
     latest_version: datarobot.CustomModelVersion or None
         The latest version of the custom model if the model has a latest version.
     deployments_count: int
@@ -614,15 +618,16 @@
         Parameters
         ----------
         name: str
             Name of the custom inference model.
         target_type: datarobot.TARGET_TYPE
             Target type of the custom inference model.
             Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
-            `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`]
+            `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`,
+            `datarobot.TARGET_TYPE.TEXT_GENERATION`]
         target_name: str, optional
             Target feature name.
             It is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED` target type.
         language: str, optional
             Programming language of the custom learning model.
         description: str, optional
             Description of the custom learning model.
@@ -814,52 +819,7 @@
         ------
         datarobot.errors.ClientError
             If the server responded with 4xx status.
         datarobot.errors.ServerError
             If the server responded with 5xx status.
         """
         super().delete()
-
-    @deprecated(
-        deprecated_since_version="v3.2",
-        will_remove_version="v3.4",
-        message="Please use training data assignment on the model version level: "
-        "CustomModelVersion.create_from_previous or CustomModelVersion.create_clean",
-    )
-    def assign_training_data(
-        self,
-        dataset_id: str,
-        partition_column: Optional[str] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
-    ) -> None:
-        """Assign training data to the custom inference model.
-
-        .. versionadded:: v2.21
-
-        Parameters
-        ----------
-        dataset_id: str
-            The id of the training dataset to be assigned.
-        partition_column: str, optional
-            Name of a partition column in the training dataset.
-        max_wait: int, optional
-            Max time to wait for a training data assignment.
-            If set to None - method will return without waiting.
-            Defaults to 10 min.
-
-        Raises
-        ------
-        datarobot.errors.ClientError
-            If the server responded with 4xx status
-        datarobot.errors.ServerError
-            If the server responded with 5xx status
-        """
-        payload = {"dataset_id": dataset_id, "partition_column": partition_column}
-
-        path = f"{self._path}{self.id}/trainingData/"
-
-        response = self._client.patch(path, data=payload)
-
-        if max_wait is not None:
-            wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
-
-        self.refresh()
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_model_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
 from datarobot.errors import InvalidUsageError, TrainingDataAssignmentError
 from datarobot.models.api_object import APIObject, ServerDataType
 from datarobot.models.job import filter_feature_impact_result
+from datarobot.models.runtime_parameters import RuntimeParameter, RuntimeParameterValue
 from datarobot.models.validators import custom_model_feature_impact_trafaret
 from datarobot.utils import camelize
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution, wait_for_custom_resolution
 
 
 class RequiredMetadataValue(APIObject):
@@ -566,14 +567,15 @@
             t.Key("dependencies", optional=True): t.List(CustomDependency.schema),
             t.Key("network_egress_policy", optional=True): t.Enum(*NETWORK_EGRESS_POLICY.ALL),
             t.Key("maximum_memory", optional=True): Int(),
             t.Key("replicas", optional=True): Int(),
             t.Key("required_metadata_values", optional=True): t.List(RequiredMetadataValue.schema),
             t.Key("training_data", optional=True): t.Or(TrainingData.schema, t.Null()),
             t.Key("holdout_data", optional=True): t.Or(HoldoutData.schema, t.Null()),
+            t.Key("runtime_parameters", optional=True): t.List(RuntimeParameter.schema),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
     def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
@@ -597,14 +599,15 @@
         dependencies: Optional[List[CustomDependency]] = None,
         network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
         maximum_memory: Optional[int] = None,
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_data: Optional[Mapping[str, Any]] = None,
         holdout_data: Optional[Mapping[str, Any]] = None,
+        runtime_parameters: Optional[List[RuntimeParameter]] = None,
     ) -> None:
         self.id = id
         self.custom_model_id = custom_model_id
         self.version_minor = version_minor
         self.version_major = version_major
         self.is_frozen = is_frozen
         self.items = [CustomModelFileItem(**item) for item in items]  # type: ignore[arg-type]
@@ -620,14 +623,19 @@
         self.required_metadata_values = (
             [RequiredMetadataValue.from_server_data(val) for val in required_metadata_values]  # type: ignore[arg-type]
             if required_metadata_values
             else None
         )
         self.training_data = TrainingData(**training_data) if training_data else None
         self.holdout_data = HoldoutData(**holdout_data) if holdout_data else None
+        self.runtime_parameters = (
+            [RuntimeParameter(**param) for param in runtime_parameters]  # type: ignore[arg-type]
+            if runtime_parameters
+            else None
+        )
 
     @classmethod
     def from_server_data(
         cls, data: ServerDataType, keep_attrs: Optional[Iterable[str]] = None
     ) -> CustomModelVersion:
         initial = super().from_server_data(data, keep_attrs)
         # from_server_data will make the keys in requiredMetadata lowercase,
@@ -648,14 +656,15 @@
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_dataset_id: Optional[str] = None,
         partition_column: Optional[str] = None,
         holdout_dataset_id: Optional[str] = None,
         keep_training_holdout_data: Optional[bool] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
     ) -> CustomModelVersion:
         """Create a custom model version without files from previous versions.
 
            Create a version with training or holdout data:
            If training/holdout data related parameters are provided,
            the training data is assigned asynchronously.
            In this case:
@@ -717,14 +726,18 @@
             Defaults to True.
             This field is only applicable if the model has training data for versions enabled,
             otherwise the field value will be ignored.
         max_wait: int, optional
             Max time to wait for training data assignment.
             If set to None - method will return without waiting.
             Defaults to 10 minutes.
+        runtime_parameter_values: List[RuntimeParameterValue]
+            Additional parameters to be injected into a model at runtime. The fieldName
+            must match a fieldName that is listed in the runtimeParameterDefinitions section
+            of the model-metadata.yaml file.
 
         Returns
         -------
         CustomModelVersion
             Created custom model version.
 
         Raises
@@ -794,14 +807,15 @@
             replicas=replicas,
             required_metadata_values=required_metadata_values,
             training_dataset_id=training_dataset_id,
             partition_column=partition_column,
             holdout_dataset_id=holdout_dataset_id,
             keep_training_holdout_data=keep_training_holdout_data,
             max_wait=max_wait,
+            runtime_parameter_values=runtime_parameter_values,
         )
 
     @classmethod
     def create_from_previous(
         cls,
         custom_model_id: str,
         base_environment_id: str,
@@ -814,14 +828,15 @@
         replicas: Optional[int] = None,
         required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
         training_dataset_id: Optional[str] = None,
         partition_column: Optional[str] = None,
         holdout_dataset_id: Optional[str] = None,
         keep_training_holdout_data: Optional[bool] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
     ) -> CustomModelVersion:
         """Create a custom model version containing files from a previous version.
 
            Create a version with training/holdout data:
            If training/holdout data related parameters are provided,
            the training data is assigned asynchronously.
            In this case:
@@ -887,14 +902,20 @@
             Defaults to True.
             This field is only applicable if the model has training data for versions enabled,
             otherwise the field value will be ignored.
         max_wait: int, optional
             Max time to wait for training data assignment.
             If set to None - method will return without waiting.
             Defaults to 10 minutes.
+        runtime_parameter_values: List[RuntimeParameterValue]
+            Additional parameters to be injected into the model at runtime. The fieldName
+            must match a fieldName that is listed in the runtimeParameterDefinitions section
+            of the model-metadata.yaml file. This list will be merged with any existing
+            runtime values set from the prior version, so it is possible to specify a `null` value
+            to unset specific parameters and fall back to the defaultValue from the definition.
 
         Returns
         -------
         CustomModelVersion
             created custom model version
 
         Raises
@@ -969,14 +990,15 @@
             replicas,
             required_metadata_values=required_metadata_values,
             training_dataset_id=training_dataset_id,
             partition_column=partition_column,
             holdout_dataset_id=holdout_dataset_id,
             keep_training_holdout_data=keep_training_holdout_data,
             max_wait=max_wait,
+            runtime_parameter_values=runtime_parameter_values,
         )
 
     @classmethod
     def _create(
         cls,
         method: str,
         custom_model_id: str,
@@ -990,14 +1012,15 @@
         replicas: Optional[int],
         required_metadata_values: Optional[List[RequiredMetadataValue]],
         training_dataset_id: Optional[str],
         partition_column: Optional[str],
         holdout_dataset_id: Optional[str],
         keep_training_holdout_data: Optional[bool],
         max_wait: Optional[int],
+        runtime_parameter_values: Optional[List[RuntimeParameterValue]] = None,
     ) -> CustomModelVersion:
         # TODO: pass model object
         """Create a custom model version"""
 
         def _wait_for_training_data_assignment(version: CustomModelVersion) -> None:
             # This check is needed to make sure user explicitly passes new training data.
             # Checking only for `version.training_data.assignment_in_progress` is not enough as it is not known
@@ -1106,14 +1129,27 @@
                     hd_payload["partitionColumn"] = partition_column
 
                 if len(hd_payload):
                     upload_data.append(("holdoutData", json.dumps(hd_payload)))
             if keep_training_holdout_data is not None:
                 upload_data.append(("keepTrainingHoldoutData", str(keep_training_holdout_data)))
 
+            if runtime_parameter_values is not None:
+                upload_data.append(
+                    (
+                        "runtimeParameterValues",
+                        json.dumps(
+                            [
+                                {camelize(k): v for k, v in param.to_dict().items()}
+                                for param in runtime_parameter_values
+                            ]
+                        ),
+                    )
+                )
+
             encoder = MultipartEncoder(fields=upload_data)
             headers = {"Content-Type": encoder.content_type}
             response = cls._client.request(method, url, data=encoder, headers=headers)
             new_version = cls.from_server_data(response.json())
 
             _wait_for_training_data_assignment(new_version)
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_task.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_slice.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_source.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/data_store.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/dataset.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/challenger.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/challenger.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.enums import (
     ACCURACY_METRIC,
     BUCKET_SIZE,
     DEFAULT_MAX_WAIT,
+    ExportStatus,
     FileLocationType,
     LocalSourceType,
 )
 from datarobot.errors import ClientError, InvalidUsageError
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
@@ -39,15 +40,21 @@
 from datarobot.models.deployment.accuracy import (
     Accuracy,
     AccuracyOverTime,
     PredictionsVsActualsOverTime,
 )
 from datarobot.models.deployment.bias_and_fairness import FairnessScoresOverTime
 from datarobot.models.deployment.challenger import Challenger
+from datarobot.models.deployment.champion_model_package import ChampionModelPackage
 from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
+from datarobot.models.deployment.data_exports import (
+    ActualsDataExport,
+    PredictionDataExport,
+    TrainingDataExport,
+)
 from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
@@ -2012,14 +2019,90 @@
                 Actuals timeliness health settings.
         """
 
         url = f"{self._path}{self.id}/healthSettings/"
         response_json = cast(ServerDataDictType, from_api(self._client.get(url).json()))
         return cast("HealthSettings", response_json)
 
+    def update_health_settings(
+        self,
+        service: Optional[Dict[str, Any]] = None,
+        data_drift: Optional[Dict[str, Any]] = None,
+        accuracy: Optional[Dict[str, Any]] = None,
+        fairness: Optional[Dict[str, Any]] = None,
+        custom_metrics: Optional[Dict[str, Any]] = None,
+        predictions_timeliness: Optional[Dict[str, Any]] = None,
+        actuals_timeliness: Optional[Dict[str, Any]] = None,
+    ) -> HealthSettings:
+        """Update health settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Parameters
+        ----------
+        service : dict
+            Service health settings.
+        data_drift : dict
+            Data drift health settings.
+        accuracy : dict
+            Accuracy health settings.
+        fairness : dict
+            Fairness health settings.
+        custom_metrics : dict
+            Custom metrics health settings.
+        predictions_timeliness : dict
+            Predictions timeliness health settings.
+        actuals_timeliness : dict
+            Actuals timeliness health settings.
+        """
+
+        url = f"{self._path}{self.id}/healthSettings/"
+        payload = {
+            "service": service,
+            "data_drift": data_drift,
+            "accuracy": accuracy,
+            "fairness": fairness,
+            "custom_metrics": custom_metrics,
+            "predictions_timeliness": predictions_timeliness,
+            "actuals_timeliness": actuals_timeliness,
+        }
+        payload = {key: value for key, value in payload.items() if value is not None}
+        if not payload:
+            raise ValueError("Must provide at least one health settings object.")
+        response = self._client.patch(url, data=to_api(payload))
+        return cast("HealthSettings", from_api(response.json()))
+
+    def get_default_health_settings(self) -> HealthSettings:
+        """Retrieve default health settings of this deployment.
+
+        .. versionadded:: v3.4
+
+        Returns
+        -------
+        settings : dict in the following format:
+            service : dict
+                Service health settings.
+            data_drift : dict
+                Data drift health settings.
+            accuracy : dict
+                Accuracy health settings.
+            fairness : dict
+                Fairness health settings.
+            custom_metrics : dict
+                Custom metrics health settings.
+            predictions_timeliness : dict
+                Predictions timeliness health settings.
+            actuals_timeliness : dict
+                Actuals timeliness health settings.
+        """
+
+        url = f"{self._path}{self.id}/healthSettings/defaults/"
+        response_json = cast(ServerDataDictType, from_api(self._client.get(url).json()))
+        return cast("HealthSettings", response_json)
+
     def get_service_stats(
         self,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         execution_time_quantile: Optional[float] = None,
         response_time_quantile: Optional[float] = None,
@@ -2836,14 +2919,118 @@
 
         Returns
         -------
         list(Challenger)
         """
         return Challenger.list(self.id)
 
+    def get_champion_model_package(self) -> ChampionModelPackage:
+        """
+        Get a champion model package for this deployment.
+
+        Returns
+        -------
+        champion_model_package : ChampionModelPackage
+            A champion model package object.
+
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from datarobot import Deployment
+            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
+            champion_model_package = deployment.get_champion_model_package()
+        """
+        path = f"{self._path}{self.id}/championModelPackage/"
+        response = self._client.get(path)
+        champion_model_package = ChampionModelPackage.from_data(data=from_api(response.json()))
+        return champion_model_package
+
+    def list_prediction_data_exports(
+        self,
+        model_id: Optional[str] = None,
+        status: Optional[ExportStatus] = None,
+        batch: Optional[bool] = None,
+        offset: Optional[int] = 0,
+        limit: Optional[int] = 100,
+    ) -> List[PredictionDataExport]:
+        """
+        Retrieve a list of asynchronous prediction data exports.
+
+        Parameters
+        ----------
+        model_id: Optional[str]
+            The ID of the model used for prediction data export.
+        status: Optional[str]
+            A prediction data export processing state.
+        batch: Optional[bool]
+            If true, only return batch exports.
+            If false, only return real-time exports.
+            If not provided, return both real-time and batch exports.
+        limit: Optional[int]
+            The maximum number of objects to return. The default is 100 (0 means no limit).
+        offset: Optional[int]
+            The starting offset of the results. The default is 0.
+
+        Returns
+        -------
+        prediction_data_exports: List[PredictionDataExport]
+            A list of prediction data exports.
+        """
+        return PredictionDataExport.list(
+            deployment_id=self.id,
+            model_id=model_id,
+            status=status,
+            batch=batch,
+            offset=offset,
+            limit=limit,
+        )
+
+    def list_actuals_data_exports(
+        self,
+        status: Optional[ExportStatus] = None,
+        offset: Optional[int] = 0,
+        limit: Optional[int] = 100,
+    ) -> List[ActualsDataExport]:
+        """
+        Retrieve a list of asynchronous actuals data exports.
+
+        Parameters
+        ----------
+        status: Optional[str]
+            Actuals data export processing state.
+        limit: Optional[int]
+            The maximum number of objects to return. The default is 100 (0 means no limit).
+        offset: Optional[int]
+            The starting offset of the results. The default is 0.
+
+        Returns
+        -------
+        actuals_data_exports: List[ActualsDataExport]
+            A list of actuals data exports.
+        """
+        return ActualsDataExport.list(
+            deployment_id=self.id,
+            status=status,
+            offset=offset,
+            limit=limit,
+        )
+
+    def list_training_data_exports(self) -> List[TrainingDataExport]:
+        """
+        Retrieve a list of successful training data exports.
+
+        Returns
+        -------
+        training_data_export: List[TrainingDataExport]
+            A list of training data exports.
+        """
+        return TrainingDataExport.list(deployment_id=self.id)
+
 
 class DeploymentListFilters:  # pylint: disable=missing-class-docstring
     def __init__(
         self,
         role: Optional[str] = None,
         service_health: Optional[List[str]] = None,
         model_health: Optional[List[str]] = None,
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/documentai/document.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/driver.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/execution_environment.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_effect.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/feature_impact.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/featurelist.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/imported_model.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/lift_chart.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/residuals.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,185 +1,172 @@
 #
-# Copyright 2021 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from typing import Any, Dict, Iterable, List, Mapping, Optional
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Union
 
-from mypy_extensions import TypedDict
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.models.api_object import APIObject
+from datarobot.utils import from_api
 
-LiftChartBinsTrafaret = t.Dict(
-    {
-        t.Key("bins"): t.List(
-            t.Dict(
-                {
-                    t.Key("actual"): t.Float,
-                    t.Key("predicted"): t.Float,
-                    t.Key("bin_weight"): t.Float,
-                }
-            ).ignore_extra("*")
-        )
-    }
-)
-
-
-class LiftChartBin(TypedDict):
-    actual: float
-    predicted: float
-    bin_weight: float
-
+ResidualsTrafaret = {
+    t.Key("residual_mean"): t.Float,
+    t.Key("coefficient_of_determination"): t.Float,
+    t.Key("standard_deviation", optional=True): t.Float,
+}
 
-class LiftChartData(TypedDict):
-    bins: List[LiftChartBin]
 
+class ResidualsChart(APIObject):
+    """Residual analysis chart data for model.
 
-class LiftChartServerData(TypedDict):
-    id: str
-    entity_id: str
-    project_id: str
-    source: str
-    data_slice_id: Optional[str]
-    data: LiftChartData
+    .. versionadded:: v2.18
 
-
-class LiftChart(APIObject):
-    """ Lift chart data for model.
+    This data is calculated over a randomly downsampled subset of the source data
+    (capped at 1000 rows).
 
     Notes
     -----
-    ``LiftChartBin`` is a dict containing the following:
 
-        * ``actual`` (float) Sum of actual target values in bin
-        * ``predicted`` (float) Sum of predicted target values in bin
-        * ``bin_weight`` (float) The weight of the bin. For weighted projects, it is the sum of \
-          the weights of the rows in the bin. For unweighted projects, it is the number of rows in \
-          the bin.
+    ``ResidualsChartRow`` is a list of floats and ints containing the following:
+        * Element 0 (float) is the actual target value for the source data row.
+        * Element 1 (float) is the predicted target value for that row.
+        * Element 2 (float) is the error rate of predicted - actual and is optional.
+        * Element 3 (int) is the row number in the source dataset from which the values
+          were selected and is optional.
 
     Attributes
     ----------
     source : str
         Lift chart data source. Can be 'validation', 'crossValidation' or 'holdout'.
-    bins : list of dict
-        List of dicts with schema described as ``LiftChartBin`` above.
+    data : list
+        List of lists with schema described as ``ResidualsChartRow`` above.
+    coefficient_of_determination : float
+        The r-squared value for the downsampled dataset
+    residual_mean : float
+        The arithmetic mean of the residual (predicted value minus actual value)
     source_model_id : str
-        ID of the model this lift chart represents; in some cases,
+        ID of the model this chart represents; in some cases,
         insights from the parent of a frozen model may be used
-    target_class : str, optional
-        For multiclass lift - target class for this lift chart data.
+    standard_deviation : float
+        standard_deviation of residual values
     data_slice_id: string or None
-        The slice to retrieve Lift Chart for; if None, retrieve unsliced data.
+        The slice to retrieve Feature Effects for; if None, retrieve unsliced data.
     """
 
     _converter = (
         t.Dict(
             {
                 t.Key("source"): String,
+                t.Key("data"): t.List(t.List(t.Float)),
                 t.Key("source_model_id"): String,
-                t.Key("target_class", optional=True, default=None): t.Or(String, t.Null),
                 t.Key("data_slice_id", optional=True): t.Or(String, t.Null),
             }
         )
-        .merge(LiftChartBinsTrafaret)
+        .merge(ResidualsTrafaret)
         .ignore_extra("*")
     )
 
-    def __init__(self, source, bins, source_model_id, target_class, data_slice_id=None):
+    def __init__(
+        self,
+        source: str,
+        data: List[Union[float, int]],
+        residual_mean: float,
+        coefficient_of_determination: float,
+        source_model_id: str,
+        standard_deviation: Optional[float] = None,
+        data_slice_id: Optional[str] = None,
+    ) -> None:
         self.source = source
-        self.bins = bins
+        self.data = data
         self.source_model_id = source_model_id
-        self.target_class = target_class
+        self.coefficient_of_determination = coefficient_of_determination
+        self.residual_mean = residual_mean
+        self.standard_deviation = standard_deviation
         self.data_slice_id = data_slice_id
 
-    def __repr__(self):
-        additional_params = ""
-        if self.target_class:
-            additional_params += f"{self.target_class}:"
-        if self.data_slice_id:
-            additional_params += f"{self.data_slice_id}:"
-        return f"LiftChart({additional_params}{self.source})"
+    def __repr__(self) -> str:
+        return f"ResidualChart({self.source})"
 
     @staticmethod
-    def _repack_insights_response(server_data: LiftChartServerData):
+    def _repack_insights_response(raw_server_record: Dict[str, Any]) -> Dict[str, Any]:
         """Repack the JSON sent by the GET /insights/ endpoint to match the format expected by the
         insight APIObject class.
 
         Parameters
         ----------
-        server_data : dict
-        {
-            "id": "6474726c7ca961a4ebce068d",
-            "entityId": "64747242956c7390bb15b206",
-            "projectId": "647471b6b5d9cbd454f2cf63",
-            "source": "validation",
-            "dataSliceId": "647471b6b5d9cbd454f2ab99",
-            "data": {"bins": [{"actual":0.0, "predicted":0.0, "binWeight":27.0}, ...]}
-        }
+        raw_server_record : dict
 
         Returns
         -------
-        dict
-        {
-            "source": "validation",
-            "bins": [{"actual":0.0, "predicted":0.0, "binWeight":27.0}, ...],
-            "sourceModelId": "64747242956c7390bb15b206",
-            "dataSliceId": "647471b6b5d9cbd454f2ab99",
-        }
+        server_record : dict
         """
         return {
-            "source": server_data["source"],
-            "bins": server_data["data"]["bins"],
-            "sourceModelId": server_data["entityId"],
-            "dataSliceId": server_data["dataSliceId"],
+            "source": raw_server_record["source"],
+            "data": raw_server_record["data"]["data"],
+            "residual_mean": raw_server_record["data"]["residualMean"],
+            "coefficient_of_determination": raw_server_record["data"]["coefficientOfDetermination"],
+            "source_model_id": raw_server_record["entityId"],
+            "standard_deviation": raw_server_record["data"]["standardDeviation"],
+            "data_slice_id": raw_server_record["dataSliceId"],
         }
 
     @classmethod
-    def from_server_data(cls, data, keep_attrs=None, use_insights_format=False, **kwargs):
+    # type: ignore[override]
+    def from_server_data(
+        cls,
+        data: Dict[str, Any],
+        keep_attrs: Optional[Iterable[str]] = None,
+        use_insights_format: bool = False,
+        **kwargs: Mapping[str, Any],
+    ) -> "ResidualsChart":
         """
-        Overwrite APIObject.from_server_data to handle lift chart data retrieved
+        Overwrite APIObject.from_server_data to handle residuals chart data retrieved
         from either legacy URL or /insights/ new URL.
-
         Parameters
         ----------
         data : dict
             The directly translated dict of JSON from the server. No casing fixes have
-            taken place
+            taken place.
+        keep_attrs : iterable
+            List, set or tuple of the dotted namespace notations for attributes to keep within the
+            object structure even if their values are None
         use_insights_format : bool, optional
-            Whether to repack the data from the format used in the GET /insights/liftChart/ URL
+            Whether to repack the data from the format used in the GET /insights/residuals/ URL
             to the format used in the legacy URL.
         """
         if use_insights_format:
             data = cls._repack_insights_response(data)
 
-        return super().from_server_data(data=data, keep_attrs=keep_attrs)
+        case_converted = from_api(data)
+        return cls.from_data(case_converted)
 
 
-class SlicedLiftChart(LiftChart):
-    """Wrapper around LiftChart to override `from_server_data` method"""
+class SlicedResidualsChart(ResidualsChart):
+    """Wrapper around ResidualsChart to override `from_server_data` method"""
 
     @classmethod
     # type: ignore[override]
     def from_server_data(
         cls,
         data: Dict[str, Any],
         keep_attrs: Optional[Iterable[str]] = None,
         use_insights_format: bool = True,
         **kwargs: Mapping[str, Any],
-    ) -> "LiftChart":
+    ) -> "ResidualsChart":
         """
-        Overwrite LiftChart.from_server_data to set `use_insights_format=True` by default
+        Overwrite ResidualsChart.from_server_data to set `use_insights_format=True` by default
         This is necessary for the correct transformation of data received from /insights endpoints
 
         Parameters
         ----------
         data : dict
             The directly translated dict of JSON from the server. No casing fixes have
             taken place.
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/missing_report.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
 
     _base_model_path_template = "projects/{}/models/"
 
     _converter = t.Dict(
         {
             t.Key("id"): String,
-            t.Key("processes"): t.List(String),
+            t.Key("processes", optional=True): t.List(String),
             t.Key("featurelist_name", optional=True): String,
             t.Key("featurelist_id", optional=True): String,
             t.Key("project_id"): String,
             t.Key("sample_pct", optional=True): t.Float,
             t.Key("model_type"): String,
             t.Key("model_category"): String,
             t.Key("model_number"): Int,
@@ -3552,15 +3552,15 @@
         Whether this model is supported Composable ML.
 
     """
 
     _converter = t.Dict(
         {
             t.Key("id"): String,
-            t.Key("processes"): t.List(String),
+            t.Key("processes", optional=True): t.List(String),
             t.Key("featurelist_name", optional=True): String,
             t.Key("featurelist_id", optional=True): String,
             t.Key("project_id"): String,
             t.Key("sample_pct", optional=True): t.Float,
             t.Key("model_type"): String,
             t.Key("model_category"): String,
             t.Key("is_frozen"): t.Bool,
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/deployment.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/registered_model.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/model_registry/registered_model_version.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/model_registry/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/modeljob.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/pareto_front.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/predict_job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_environment.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prediction_server.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/predictions.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/prime_file.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/project.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,17 +129,18 @@
         credentialType: CredentialTypes
 
     class BasicCredentialsDataDict(BaseCredentialsDataDict):
         user: str
         password: str
 
     class S3CredentialsDataDict(BaseCredentialsDataDict):
-        awsAccessKeyId: str
-        awsSecretAccessKey: str
-        awsSessionToken: str
+        awsAccessKeyId: Optional[str]
+        awsSecretAccessKey: Optional[str]
+        awsSessionToken: Optional[str]
+        configId: Optional[str]
 
     class OAuthCredentialsDataDict(BaseCredentialsDataDict):
         oauthRefreshToken: str
         oauthClientId: str
         oauthClientSecret: str
         oauthAccessToken: str
 
@@ -149,16 +150,17 @@
         passphrase: Optional[str]
         configId: Optional[str]
 
     class DatabricksAccessTokenCredentialsDataDict(BaseCredentialsDataDict):
         databricksAccessToken: str
 
     class DatabricksServicePrincipalCredentialsDataDict(BaseCredentialsDataDict):
-        clientId: str
-        clientSecret: str
+        clientId: Optional[str]
+        clientSecret: Optional[str]
+        configId: Optional[str]
 
     class BasicCredentialsDict(TypedDict):
         user: str
         password: str
 
     class CredentialIdCredentialsDict(TypedDict):
         credentialId: str
@@ -2537,20 +2539,23 @@
                 password : str
                     The password for database authentication.
                     The password is encrypted at rest and never saved or stored.
 
             S3 Credentials
                 credentialType : str
                     The credential type. For S3 credentials, this value must be CredentialTypes.S3.
-                awsAccessKeyId : str
+                awsAccessKeyId : str, optional
                     The S3 AWS access key ID.
-                awsSecretAccessKey : str
+                awsSecretAccessKey : str, optional
                     The S3 AWS secret access key.
-                awsSessionToken : str
+                awsSessionToken : str, optional
                     The S3 AWS session token.
+                config_id: str, optional
+                    The ID of the saved shared secure configuration. If specified, cannot include awsAccessKeyId,
+                    awsSecretAccessKey or awsSessionToken.
 
             OAuth Credentials
                 credentialType : str
                     The credential type. For OAuth credentials, this value must be CredentialTypes.OAUTH.
                 oauthRefreshToken : str
                     The oauth refresh token.
                 oauthClientId : str
@@ -2569,32 +2574,35 @@
                 privateKeyStr : str, optional
                     The private key copied exactly from user private key file. Since it contains
                     multiple lines, when assign to a variable,
                     put the key string inside triple-quotes
                 passphrase : str, optional
                     The string used to encrypt the private key.
                 configId : str, optional
-                    The ID of the saved shared credentials. If specified, cannot include user,
+                    The ID of the saved shared secure configuration. If specified, cannot include user,
                     privateKeyStr or passphrase.
 
             Databricks Access Token Credentials
                 credentialType : str
                     The credential type. For a Databricks access token, this value must be
                     CredentialTypes.DATABRICKS_ACCESS_TOKEN.
                 databricksAccessToken : str
                     The Databricks personal access token.
 
             Databricks Service Principal Credentials
                 credentialType : str
                     The credential type. For Databricks service principal, this value must be
                     CredentialTypes.DATABRICKS_SERVICE_PRINCIPAL.
-                clientId : str
+                clientId : str, optional
                     The client ID for Databricks service principal.
-                clientSecret : str
+                clientSecret : str, optional
                     The client secret for Databricks service principal.
+                configId : str, optional
+                    The ID of the saved shared secure configuration. If specified, cannot include clientId
+                    and clientSecret.
 
         dataset_version_id : str, optional
             The version id of the dataset to use.
         max_wait : int, optional
             Optional, the maximum number of seconds to wait before giving up.
         forecast_point : datetime.datetime or None, optional
             For time series projects only. This is the default point relative
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/project_options.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/project_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1115,14 +1115,18 @@
             "treat_as_exponential": self.treat_as_exponential,
             "use_gpu": self.use_gpu,
             "unsupervised_mode": self.unsupervised_mode,
             "use_supervised_feature_reduction": self.use_supervised_feature_reduction,
             "use_time_series": self.use_time_series,
             "validation_duration": self.validation_duration,
             "windows_basis_unit": self.windows_basis_unit,
+            "incremental_learning_only_mode": self.incremental_learning_only_mode,
+            "incremental_learning_on_best_model": self.incremental_learning_on_best_model,
+            "incremental_learning_early_stopping_rounds": self.incremental_learning_early_stopping_rounds,
+            "chunk_definition_id": self.chunk_definition_id,
         }
 
     def collect_autopilot_payload(self) -> Dict[str, Any]:
         if not self.is_empty:
             return super().collect_payload()
         return {
             default_field: getattr(self, default_field)
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/rating_table.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/recommended_model.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/roc_curve.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/ruleset.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/segmentation.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/shap_impact.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/sharing.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/status_check_job.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/trafarets.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/training_predictions.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/types.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/use_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SHARING_RECIPIENT_TYPE,
     SHARING_ROLE,
     UseCaseAPIPathEntityType,
     UseCaseEntityType,
     UseCaseReferenceEntityMap,
 )
 from datarobot.errors import InvalidUsageError
+from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject
 from datarobot.models.sharing import SharingRole
 from datarobot.utils.pagination import unpaginate
 
 T = TypeVar("T")
 
 use_case_user_trafaret = t.Dict(
@@ -164,15 +165,15 @@
         error_message = (
             error_message + " PredictionDataset is not a subclass of Dataset and "
             "cannot be added to a UseCase at this time."
         )
     raise TypeError(error_message)
 
 
-class UseCase(APIObject):
+class UseCase(APIObject, BrowserMixin):
     """Representation of a Use Case.
 
     Attributes
     ----------
     id : str
         The ID of the Use Case.
     name : str
@@ -285,14 +286,23 @@
             f"models={self.models_count}, "
             f"projects={self.projects_count}, "
             f"datasets={self.datasets_count}, "
             f"notebooks={self.notebooks_count}, "
             f"applications={self.applications_count})"
         )
 
+    def get_uri(self) -> str:
+        """
+        Returns
+        -------
+        url : str
+            Permanent static hyperlink to this Use Case.
+        """
+        return f"{self._client.domain}/usecases/{self.id}/overview/recent"
+
     @classmethod
     def get(cls, use_case_id: str) -> UseCase:
         """
         Gets information about a Use Case.
 
         Parameters
         ----------
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/validators.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/images.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/models/word_cloud.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/rest.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/__init__.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/deprecation.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/pagination.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/retry.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/source.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot/utils/waiters.py` & `datarobot_early_access-3.4.0.2024.4.1/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.4.0.2024.3.4
+Version: 3.4.0.2024.4.1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,27 +22,25 @@
 datarobot/_experimental/models/__init__.py
 datarobot/_experimental/models/chunking_service.py
 datarobot/_experimental/models/data_matching.py
 datarobot/_experimental/models/dataset.py
 datarobot/_experimental/models/enums.py
 datarobot/_experimental/models/idiomatic_project.py
 datarobot/_experimental/models/incremental_learning.py
-datarobot/_experimental/models/key_values.py
 datarobot/_experimental/models/model.py
 datarobot/_experimental/models/model_lineage.py
 datarobot/_experimental/models/notebooks.py
 datarobot/_experimental/models/project_options.py
 datarobot/_experimental/models/recipe_operations.py
 datarobot/_experimental/models/recipes.py
 datarobot/_experimental/models/retraining.py
-datarobot/_experimental/models/custom_jobs/__init__.py
-datarobot/_experimental/models/custom_jobs/custom_job.py
-datarobot/_experimental/models/custom_jobs/custom_job_run.py
 datarobot/_experimental/models/genai/__init__.py
+datarobot/_experimental/models/genai/chat.py
 datarobot/_experimental/models/genai/chat_prompt.py
+datarobot/_experimental/models/genai/comparison_chat.py
 datarobot/_experimental/models/genai/comparison_prompt.py
 datarobot/_experimental/models/genai/custom_model_llm_validation.py
 datarobot/_experimental/models/genai/custom_model_validation.py
 datarobot/_experimental/models/genai/llm.py
 datarobot/_experimental/models/genai/llm_blueprint.py
 datarobot/_experimental/models/genai/playground.py
 datarobot/_experimental/models/genai/user_limits.py
@@ -51,14 +49,15 @@
 datarobot/helpers/binary_data_utils.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
 datarobot/helpers/image_utils.py
 datarobot/helpers/partitioning_methods.py
 datarobot/insights/__init__.py
 datarobot/insights/base.py
+datarobot/insights/shap_impact.py
 datarobot/insights/shap_matrix.py
 datarobot/insights/shap_preview.py
 datarobot/mixins/__init__.py
 datarobot/mixins/browser_mixin.py
 datarobot/mixins/update_attributes_mixin.py
 datarobot/models/__init__.py
 datarobot/models/advanced_tuning.py
@@ -96,14 +95,15 @@
 datarobot/models/external_baseline_validation.py
 datarobot/models/feature.py
 datarobot/models/feature_effect.py
 datarobot/models/feature_impact.py
 datarobot/models/featurelist.py
 datarobot/models/imported_model.py
 datarobot/models/job.py
+datarobot/models/key_values.py
 datarobot/models/lift_chart.py
 datarobot/models/missing_report.py
 datarobot/models/model.py
 datarobot/models/modeljob.py
 datarobot/models/pairwise_statistics.py
 datarobot/models/pareto_front.py
 datarobot/models/payoff_matrix.py
@@ -119,14 +119,15 @@
 datarobot/models/rating_table.py
 datarobot/models/recommended_model.py
 datarobot/models/relationships_configuration.py
 datarobot/models/residuals.py
 datarobot/models/restore_discarded_features.py
 datarobot/models/roc_curve.py
 datarobot/models/ruleset.py
+datarobot/models/runtime_parameters.py
 datarobot/models/secondary_dataset.py
 datarobot/models/segmentation.py
 datarobot/models/shap_impact.py
 datarobot/models/shap_matrix.py
 datarobot/models/shap_matrix_job.py
 datarobot/models/sharing.py
 datarobot/models/status_check_job.py
@@ -135,15 +136,18 @@
 datarobot/models/types.py
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
 datarobot/models/deployment/bias_and_fairness.py
 datarobot/models/deployment/challenger.py
+datarobot/models/deployment/champion_model_package.py
+datarobot/models/deployment/custom_metrics.py
 datarobot/models/deployment/data_drift.py
+datarobot/models/deployment/data_exports.py
 datarobot/models/deployment/deployment.py
 datarobot/models/deployment/mixins.py
 datarobot/models/deployment/service_stats.py
 datarobot/models/deployment/sharing.py
 datarobot/models/documentai/__init__.py
 datarobot/models/documentai/document.py
 datarobot/models/external_dataset_scores_insights/__init__.py
@@ -158,14 +162,17 @@
 datarobot/models/feature_association_matrix/feature_association_matrix.py
 datarobot/models/feature_association_matrix/feature_association_matrix_details.py
 datarobot/models/model_registry/__init__.py
 datarobot/models/model_registry/common.py
 datarobot/models/model_registry/deployment.py
 datarobot/models/model_registry/registered_model.py
 datarobot/models/model_registry/registered_model_version.py
+datarobot/models/registry/__init__.py
+datarobot/models/registry/job.py
+datarobot/models/registry/job_run.py
 datarobot/models/use_cases/__init__.py
 datarobot/models/use_cases/use_case.py
 datarobot/models/use_cases/utils.py
 datarobot/models/user_blueprints/__init__.py
 datarobot/models/user_blueprints/models.py
 datarobot/models/user_blueprints/trafarets.py
 datarobot/models/visualai/__init__.py
```

### Comparing `datarobot_early_access-3.4.0.2024.3.4/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.4.0.2024.4.1/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/pyproject.toml` & `datarobot_early_access-3.4.0.2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/setup.py` & `datarobot_early_access-3.4.0.2024.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.4.0.2024.3.4/setup_weekly.py` & `datarobot_early_access-3.4.0.2024.4.1/setup_weekly.py`

 * *Files identical despite different names*

