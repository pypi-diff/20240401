# Comparing `tmp/dcicutils-8.8.1.1b7.tar.gz` & `tmp/dcicutils-8.8.1.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.1.1b7.tar", max compression
+gzip compressed data, was "dcicutils-8.8.1.1b9.tar", max compression
```

## Comparing `dcicutils-8.8.1.1b7.tar` & `dcicutils-8.8.1.1b9.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1102 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/README.rst
--rw-r--r--   0        0        0        0 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     2522 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    68891 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-03-30 02:55:03.077302 dcicutils-8.8.1.1b7/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/log_utils.py
--rw-r--r--   0        0        0   102210 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15408 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30260 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    31250 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-03-30 02:55:03.081302 dcicutils-8.8.1.1b7/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    59323 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/structured_data.py
--rw-r--r--   0        0        0     8082 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-03-30 02:55:03.085302 dcicutils-8.8.1.1b7/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.1.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/README.rst
+-rw-r--r--   0        0        0        0 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     2522 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-03-30 14:40:46.754067 dcicutils-8.8.1.1b9/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    68891 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   102210 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15408 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30260 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0     1475 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/progress_constants.py
+-rw-r--r--   0        0        0    31250 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-03-30 14:40:46.758067 dcicutils-8.8.1.1b9/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58559 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     8082 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-03-30 14:40:46.762067 dcicutils-8.8.1.1b9/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.1.1b9/PKG-INFO
```

### Comparing `dcicutils-8.8.1.1b7/LICENSE.txt` & `dcicutils-8.8.1.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/README.rst` & `dcicutils-8.8.1.1b9/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/base.py` & `dcicutils-8.8.1.1b9/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/bundle_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/captured_output.py` & `dcicutils-8.8.1.1b9/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/codebuild_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/command_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/common.py` & `dcicutils-8.8.1.1b9/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/contribution_scripts.py` & `dcicutils-8.8.1.1b9/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/contribution_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/creds_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/data_readers.py` & `dcicutils-8.8.1.1b9/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/data_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/datetime_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/deployment_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/diff_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/docker_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/ecr_scripts.py` & `dcicutils-8.8.1.1b9/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/ecr_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/ecs_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/env_base.py` & `dcicutils-8.8.1.1b9/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/env_manager.py` & `dcicutils-8.8.1.1b9/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/env_scripts.py` & `dcicutils-8.8.1.1b9/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/env_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.1.1b9/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/es_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/exceptions.py` & `dcicutils-8.8.1.1b9/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/ff_mocks.py` & `dcicutils-8.8.1.1b9/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/ff_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/file_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.1.1b9/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/glacier_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/jh_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.1.1b9/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/kibana/readme.md` & `dcicutils-8.8.1.1b9/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/lang_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.1.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/license_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/log_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/misc_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/opensearch_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/portal_object_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/portal_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/project_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/qa_checkers.py` & `dcicutils-8.8.1.1b9/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/qa_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/redis_tools.py` & `dcicutils-8.8.1.1b9/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/redis_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/s3_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/schema_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.1.1b9/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.1.1b9/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.1.1b9/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/secrets_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/sheet_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/snapshot_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/structured_data.py` & `dcicutils-8.8.1.1b9/dcicutils/structured_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from dcicutils.datetime_utils import normalize_date_string, normalize_datetime_string
 from dcicutils.file_utils import search_for_file
 from dcicutils.misc_utils import (create_dict, create_readonly_object, is_uuid, load_json_if,
                                   merge_objects, remove_empty_properties, right_trim, split_string,
                                   to_boolean, to_enum, to_float, to_integer, VirtualApp)
 from dcicutils.portal_object_utils import PortalObject
 from dcicutils.portal_utils import Portal as PortalBase
+from dcicutils.progress_constants import PROGRESS_PARSE as PROGRESS
 from dcicutils.schema_utils import Schema as SchemaBase
 from dcicutils.zip_utils import unpack_gz_file_to_temporary_file, unpack_files
 
 
 # Classes/functions to parse a CSV or Excel Spreadsheet into structured data, using a specialized
 # syntax to allow structured object properties to be referenced by column specifiers. This syntax
 # uses an (intuitive) dot notation to reference nested objects, and a (less intuitive) notation
@@ -33,39 +34,18 @@
 ACCEPTABLE_FILE_SUFFIXES = [".csv", ".tsv", ".json", ".xls", ".xlsx", ".gz", ".tar", ".tar.gz", ".tgz", ".zip"]
 ARRAY_VALUE_DELIMITER_CHAR = "|"
 ARRAY_VALUE_DELIMITER_ESCAPE_CHAR = "\\"
 ARRAY_NAME_SUFFIX_CHAR = "#"
 ARRAY_NAME_SUFFIX_REGEX = re.compile(rf"{ARRAY_NAME_SUFFIX_CHAR}\d+")
 DOTTED_NAME_DELIMITER_CHAR = "."
 
+
 # TODO: Should probably pass this knowledge in from callers.
 FILE_TYPE_NAME = "File"
 FILE_TYPE_PROPERTY_NAME = "filename"
-# This ExtraFile is a pseudo-type to handle extra_files in smaht-submitr.
-EXTRA_FILE_TYPE_NAME = "ExtraFile"
-EXTRA_FILE_TYPE_PROPERTY_NAME = "extra_files"
-
-ENABLE_ARRAY_SHEET_REFS = False
-
-# The ExtraFile pseudo-type schema.
-EXTRA_FILE_SCHEMA = {
-    "title": "ExtraFile",
-    "type": "object",
-    "required": [
-        "filename"
-    ],
-    "identifyingProperties": [
-        "filename"
-    ],
-    "properties": {
-        "filename": {
-            "type": "string"
-        }
-    }
-}
 
 # Forward type references for type hints.
 Portal = Type["Portal"]
 Schema = Type["Schema"]
 StructuredDataSet = Type["StructuredDataSet"]
 
 
@@ -208,15 +188,16 @@
                 ntypes = len(self.data)
                 for type_name in self.data:
                     nobjects += len(self.data[type_name])
             return ntypes, nobjects
         diffs = {}
         if callable(progress):
             ntypes, nobjects = get_counts()
-            progress({"start": True, "types": ntypes, "objects": nobjects})
+            progress({PROGRESS.ANALYZE_START: True,
+                      PROGRESS.ANALYZE_COUNT_TYPES: ntypes, PROGRESS.ANALYZE_COUNT_ITEMS: nobjects})
         if self.data or self.portal:  # TODO: what is this OR biz?
             refs = self.resolved_refs_with_uuids
             # TODO: Need feedback/progress tracking mechanism here.
             # TODO: Check validity of reference; actually check that earlier on even maybe.
             for type_name in self.data:
                 if not diffs.get(type_name):
                     diffs[type_name] = []
@@ -227,26 +208,27 @@
                     if existing_object:
                         object_diffs, nlookups_compare = portal_object.compare(
                             existing_object, consider_refs=True, resolved_refs=refs)
                         diffs[type_name].append(create_readonly_object(path=identifying_path,
                                                                        uuid=existing_object.uuid,
                                                                        diffs=object_diffs or None))
                         if callable(progress):
-                            progress({"update": True, "lookups": nlookups + nlookups_compare})
+                            progress({PROGRESS.ANALYZE_UPDATE: True,
+                                      PROGRESS.ANALYZE_COUNT_LOOKUP: nlookups + nlookups_compare})
                     elif identifying_path:
                         # If there is no existing object we still create a record for this object
                         # but with no uuid which will be the indication that it does not exist.
                         diffs[type_name].append(create_readonly_object(path=identifying_path, uuid=None, diffs=None))
                         if callable(progress):
-                            progress({"create": True, "lookups": nlookups})
+                            progress({PROGRESS.ANALYZE_CREATE: True, PROGRESS.ANALYZE_COUNT_LOOKUP: nlookups})
                     else:
                         if callable(progress):
-                            progress({"lookups": nlookups})
+                            progress({PROGRESS.ANALYZE_COUNT_LOOKUP: nlookups})
         if callable(progress):
-            progress({"finish": True})
+            progress({PROGRESS.ANALYZE_DONE: True})
         return diffs
 
     def load_file(self, file: str) -> None:
         # Returns a dictionary where each property is the name (i.e. the type) of the data,
         # and the value is array of dictionaries for the data itself. Handle these kinds of files:
         # 1.  Single CSV, TSV, or JSON file, where the (base) name of the file is the data type name.
         # 2.  Single Excel file containing one or more sheets, where each sheet
@@ -283,17 +265,18 @@
             nonlocal file
             excel = Excel(file)
             nrows = 0
             for sheet_name in excel.sheet_names:
                 for row in excel.sheet_reader(sheet_name):
                     nrows += 1
             return nrows, len(excel.sheet_names)
-        if self._progress:
+        if self._progress:  # TODO: Move to _load_reader
             nrows, nsheets = get_counts()
-            self._progress({"start": True, "sheets": nsheets, "rows": nrows})
+            self._progress({PROGRESS.LOAD_START: True,
+                            PROGRESS.LOAD_COUNT_SHEETS: nsheets, PROGRESS.LOAD_COUNT_ROWS: nrows})
         excel = Excel(file)  # Order the sheet names by any specified ordering (e.g. ala snovault.loadxl).
         order = {Schema.type_name(key): index for index, key in enumerate(self._order)} if self._order else {}
         for sheet_name in sorted(excel.sheet_names, key=lambda key: order.get(Schema.type_name(key), sys.maxsize)):
             self._load_reader(excel.sheet_reader(sheet_name), type_name=Schema.type_name(sheet_name))
         # TODO: Do we really need progress reporting for the below?
         # Check for unresolved reference errors which really are not because of ordering.
         # Yes such internal references will be handled correctly on actual database update via snovault.loadxl.
@@ -309,24 +292,23 @@
                     self.portal._ref_total_notfound_count -= 1
                     self._resolved_refs.add((ref, resolved.get("uuid")))
             if ref_errors_actual:
                 self._errors["ref"] = ref_errors_actual
             else:
                 del self._errors["ref"]
         if self._progress:
-            # TODO: Refactor with same thing below in _load_reader.
-            self._progress({
-                "finish": True,
-                "refs": self.ref_total_count,
-                "refs_found": self.ref_total_found_count,
-                "refs_not_found": self.ref_total_notfound_count,
-                "refs_lookup": self.ref_lookup_count,
-                "refs_lookup_cache_hit": self.ref_lookup_cache_hit_count,
-                "refs_exists_cache_hit": self.ref_exists_cache_hit_count,
-                "refs_invalid": self.ref_invalid_identifying_property_count
+            self._progress({   # TODO: Refactor with same thing below in _load_reader.
+                PROGRESS.LOAD_DONE: True,
+                PROGRESS.LOAD_COUNT_REFS: self.ref_total_count,
+                PROGRESS.LOAD_COUNT_REFS_FOUND: self.ref_total_found_count,
+                PROGRESS.LOAD_COUNT_REFS_NOT_FOUND: self.ref_total_notfound_count,
+                PROGRESS.LOAD_COUNT_REFS_LOOKUP: self.ref_lookup_count,
+                PROGRESS.LOAD_COUNT_REFS_LOOKUP_CACHE_HIT: self.ref_lookup_cache_hit_count,
+                PROGRESS.LOAD_COUNT_REFS_EXISTS_CACHE_HIT: self.ref_exists_cache_hit_count,
+                PROGRESS.LOAD_COUNT_REFS_INVALID: self.ref_invalid_identifying_property_count
             })
 
     def _load_json_file(self, file: str) -> None:
         with open(file) as f:
             self._add(Schema.type_name(file), json.load(f))
 
     def _load_reader(self, reader: RowReader, type_name: str) -> None:
@@ -348,22 +330,22 @@
             for column_name, value in row.items():
                 structured_row_template.set_value(structured_row, column_name, value, reader.file, reader.row_number)
                 if self._autoadd_properties:
                     self._add_properties(structured_row, self._autoadd_properties, schema)
             self._add(type_name, structured_row)
             if self._progress:
                 self._progress({
-                    "parse": True,
-                    "refs": self.ref_total_count,
-                    "refs_found": self.ref_total_found_count,
-                    "refs_not_found": self.ref_total_notfound_count,
-                    "refs_lookup": self.ref_lookup_count,
-                    "refs_lookup_cache_hit": self.ref_lookup_cache_hit_count,
-                    "refs_exists_cache_hit": self.ref_exists_cache_hit_count,
-                    "refs_invalid": self.ref_invalid_identifying_property_count
+                    PROGRESS.LOAD_ITEM: True,
+                    PROGRESS.LOAD_COUNT_REFS: self.ref_total_count,
+                    PROGRESS.LOAD_COUNT_REFS_FOUND: self.ref_total_found_count,
+                    PROGRESS.LOAD_COUNT_REFS_NOT_FOUND: self.ref_total_notfound_count,
+                    PROGRESS.LOAD_COUNT_REFS_LOOKUP: self.ref_lookup_count,
+                    PROGRESS.LOAD_COUNT_REFS_LOOKUP_CACHE_HIT: self.ref_lookup_cache_hit_count,
+                    PROGRESS.LOAD_COUNT_REFS_EXISTS_CACHE_HIT: self.ref_exists_cache_hit_count,
+                    PROGRESS.LOAD_COUNT_REFS_INVALID: self.ref_invalid_identifying_property_count
                 })
         self._note_warning(reader.warnings, "reader")
         if schema:
             self._note_error(schema._unresolved_refs, "ref")
             self._resolved_refs.update(schema._resolved_refs)
 
     def _add(self, type_name: str, data: Union[dict, List[dict]]) -> None:
@@ -461,20 +443,18 @@
             if not issues.get(group):
                 issues[group] = []
             issues[group].extend(item)
 
 
 class _StructuredRowTemplate:
 
-    def __init__(self, column_names: List[str], schema: Optional[Schema] = None,
-                 obtain_array_values: Optional[Callable] = None) -> None:
+    def __init__(self, column_names: List[str], schema: Optional[Schema] = None) -> None:
         self._schema = schema
         self._set_value_functions = {}
         self._template = self._create_row_template(column_names)
-        self._obtain_array_values = obtain_array_values if callable(obtain_array_values) else None
 
     def create_row(self) -> dict:
         return copy.deepcopy(self._template)
 
     def set_value(self, data: dict, column_name: str, value: str, file: Optional[str], row_number: int = -1) -> None:
         if (set_value_function := self._set_value_functions.get(column_name)):
             src = create_dict(type=self._schema.type if self._schema else None,
@@ -526,24 +506,14 @@
             if isinstance(path[-1], int) and (json_value := load_json_if(value, is_array=True)):
                 path = right_trim(path, remove=lambda value: isinstance(value, int))
             for i, p in enumerate(path[:-1]):
                 if isinstance(p, str) and (not isinstance(data, dict) or p not in data):
                     set_value_backtrack_object(i, p)
                 data = data[p]
             if (p := path[-1]) == -1 and isinstance(value, str):
-                if ENABLE_ARRAY_SHEET_REFS and False:
-                    # TODO: IN PROGRESS. DISABLED FOR NOW.
-                    if isinstance(value, str) and value.lower().startswith("[ref:") and value.endswith("]"):
-                        if self._obtain_array_values:
-                            values = self._obtain_array_values(value)
-                        if sheet_name_containing_array := value[5:].strip():
-                            if dot := sheet_name_containing_array.find(".") > 0:
-                                if sheet_name_containing_array := sheet_name_containing_array[0:dot].strip():
-                                    pass
-                                    # sheet_column_containing_array = sheet_name_containing_array[dot + 1:].strip()
                 values = _split_array_string(value, unique=typeinfo.get("unique") if typeinfo else False)
                 if mapv:
                     values = [mapv(value, src) for value in values]
                 merge_objects(data, values)
             else:
                 if json_value or (json_value := load_json_if(value, is_array=True, is_object=True)):
                     data[p] = json_value
```

### Comparing `dcicutils-8.8.1.1b7/dcicutils/task_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/trace_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/validation_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/variant_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/dcicutils/zip_utils.py` & `dcicutils-8.8.1.1b9/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.1.1b7/pyproject.toml` & `dcicutils-8.8.1.1b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.1.1b7"  # TODO: To become 8.8.2
+version = "8.8.1.1b9"  # TODO: To become 8.8.2
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.1.1b7/PKG-INFO` & `dcicutils-8.8.1.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.1.1b7
+Version: 8.8.1.1b9
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

