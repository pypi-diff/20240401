# Comparing `tmp/tecton-0.9.0rc1.tar.gz` & `tmp/tecton-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.9.0rc1.tar", last modified: Thu Mar 28 22:00:25 2024, max compression
+gzip compressed data, was "tecton-0.9.0rc2.tar", last modified: Mon Apr  1 19:41:49 2024, max compression
```

## Comparing `tecton-0.9.0rc1.tar` & `tecton-0.9.0rc2.tar`

### file list

```diff
@@ -1,670 +1,670 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.587744 tecton-0.9.0rc1/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3918 2024-03-28 22:00:25.587744 tecton-0.9.0rc1/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.519744 tecton-0.9.0rc1/protoc_gen_openapiv2/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.519744 tecton-0.9.0rc1/protoc_gen_openapiv2/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-03-28 22:00:25.587744 tecton-0.9.0rc1/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2391 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.523744 tecton-0.9.0rc1/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5977 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_gen_version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.527744 tecton-0.9.0rc1/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27051 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/ingestion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.527744 tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/service_modules.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/offline_store_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/pandas_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/query_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21072 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/querytree_api.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.527744 tecton-0.9.0rc1/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15912 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/secret_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7034 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/tecton_pydantic.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.527744 tecton-0.9.0rc1/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25510 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/auth.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/completion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34260 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7938 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/environment_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/pex_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/repo.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9757 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/repo_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4711 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.531744 tecton-0.9.0rc1/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   119708 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28984 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38070 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13799 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    42563 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   222874 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.531744 tecton-0.9.0rc1/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.531744 tecton-0.9.0rc1/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.531744 tecton-0.9.0rc1/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.531744 tecton-0.9.0rc1/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.531744 tecton-0.9.0rc1/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.535744 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.539744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.539744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.539744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.539744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.539744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.543744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.543744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.543744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.543744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.543744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.543744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.547744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.547744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.547744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.547744 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.523744 tecton-0.9.0rc1/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3918 2024-03-28 22:00:23.000000 tecton-0.9.0rc1/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22872 2024-03-28 22:00:24.000000 tecton-0.9.0rc1/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-03-28 22:00:23.000000 tecton-0.9.0rc1/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-03-28 22:00:24.000000 tecton-0.9.0rc1/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      949 2024-03-28 22:00:24.000000 tecton-0.9.0rc1/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-03-28 22:00:24.000000 tecton-0.9.0rc1/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.547744 tecton-0.9.0rc1/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5764 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/odfv_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.547744 tecton-0.9.0rc1/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.551744 tecton-0.9.0rc1/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.555744 tecton-0.9.0rc1/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/_gen_version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/arrow.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/aws_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    24781 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3171 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/duckdb_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.555744 tecton-0.9.0rc1/tecton_core/embeddings/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/embeddings/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/embeddings/config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25988 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/http.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/iterators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/materialization_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.555744 tecton-0.9.0rc1/tecton_core/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/providers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19967 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7383 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/pipeline_common.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.555744 tecton-0.9.0rc1/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55834 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/compaction_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/dialect.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.559744 tecton-0.9.0rc1/tecton_core/query/duckdb/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/duckdb/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9192 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/duckdb/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7770 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/duckdb/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/duckdb/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/executor_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1767 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/executor_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/node_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   125906 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.559744 tecton-0.9.0rc1/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22035 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pandas/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/pipeline_sql_builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/prefixed_uri_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/query_tree_compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21798 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/query_tree_executor.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/rewrite.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.559744 tecton-0.9.0rc1/tecton_core/query/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/snowflake/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11857 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/schema_validation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/snowflake_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.559744 tecton-0.9.0rc1/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44000 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/time_window_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.559744 tecton-0.9.0rc1/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/queue.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.559744 tecton-0.9.0rc1/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/batch_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_materialization/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/common/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/common/job_metadata_aws.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/common/job_metadata_gcp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/common/task_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/consumption.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/delta_maintenance.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/entity_deletion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/materialization_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_materialization/ray/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/batch_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23363 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/delta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6164 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6720 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/job_status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9748 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/materialization_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/ray/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_materialization/remote_host/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/remote_host/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/remote_host/pyspark_remote_host.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_materialization/stream_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.563744 tecton-0.9.0rc1/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.567744 tecton-0.9.0rc1/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21470 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    41703 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.567744 tecton-0.9.0rc1/tecton_proto/auditlog/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auditlog/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auditlog/metadata_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.567744 tecton-0.9.0rc1/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.567744 tecton-0.9.0rc1/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.567744 tecton-0.9.0rc1/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.571744 tecton-0.9.0rc1/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/aws_credentials_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/compute_mode_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/spark_schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/common/time_window_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.571744 tecton-0.9.0rc1/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20168 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/materialization_roles_allowlists_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/offlinestore/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/offlinestore/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.575744 tecton-0.9.0rc1/tecton_proto/offlinestore/delta/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/offlinestore/delta/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/offlinestore/delta/metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/online_store_writer/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/online_store_writer/copier_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/secrets/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/secrets/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/secrets/secrets_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/snowflake/location_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/snowflake/snowflake_credentials_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/testhelperservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/testhelperservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/testhelperservice/test_helper_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.579744 tecton-0.9.0rc1/tecton_snowflake/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/dataframe_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13559 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/queries.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33728 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.583744 tecton-0.9.0rc1/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.583744 tecton-0.9.0rc1/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35476 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.587744 tecton-0.9.0rc1/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/jars/class_loader.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7202 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14834 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33278 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:25.587744 tecton-0.9.0rc1/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7449 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17887 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-03-28 22:00:21.000000 tecton-0.9.0rc1/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.514936 tecton-0.9.0rc2/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-01 19:41:49.514936 tecton-0.9.0rc2/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.446929 tecton-0.9.0rc2/protoc_gen_openapiv2/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.446929 tecton-0.9.0rc2/protoc_gen_openapiv2/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-04-01 19:41:49.514936 tecton-0.9.0rc2/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2503 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.446929 tecton-0.9.0rc2/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5977 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_gen_version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.450929 tecton-0.9.0rc2/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27420 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/ingestion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.450929 tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/service_modules.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/offline_store_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/pandas_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/query_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21072 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/querytree_api.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.450929 tecton-0.9.0rc2/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15912 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/secret_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7034 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/tecton_pydantic.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.454930 tecton-0.9.0rc2/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25510 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/auth.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/completion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34260 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7938 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/environment_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/pex_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/repo.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9757 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/repo_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4711 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   119708 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28984 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    38553 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13799 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    42563 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   225468 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.458930 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.462931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.462931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.466931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.466931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.466931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.470931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.470931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.470931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.470931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.470931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.470931 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.446929 tecton-0.9.0rc2/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-01 19:41:47.000000 tecton-0.9.0rc2/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22872 2024-04-01 19:41:48.000000 tecton-0.9.0rc2/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-04-01 19:41:47.000000 tecton-0.9.0rc2/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-04-01 19:41:48.000000 tecton-0.9.0rc2/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1044 2024-04-01 19:41:48.000000 tecton-0.9.0rc2/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-04-01 19:41:48.000000 tecton-0.9.0rc2/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5764 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/odfv_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.474932 tecton-0.9.0rc2/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.478932 tecton-0.9.0rc2/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/_gen_version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/arrow.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/aws_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    24781 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/duckdb_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.478932 tecton-0.9.0rc2/tecton_core/embeddings/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/embeddings/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/embeddings/config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27252 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/http.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/iterators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/materialization_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.482932 tecton-0.9.0rc2/tecton_core/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/providers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20281 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7383 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/pipeline_common.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.482932 tecton-0.9.0rc2/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    56201 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/compaction_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/dialect.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.482932 tecton-0.9.0rc2/tecton_core/query/duckdb/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/duckdb/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9618 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/duckdb/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/duckdb/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/duckdb/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/executor_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/executor_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/node_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126328 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.482932 tecton-0.9.0rc2/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22035 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pandas/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/pipeline_sql_builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/prefixed_uri_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/query_tree_compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21774 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/query_tree_executor.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/rewrite.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.482932 tecton-0.9.0rc2/tecton_core/query/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/snowflake/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11857 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/schema_validation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/snowflake_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.486933 tecton-0.9.0rc2/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    43502 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/time_window_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.486933 tecton-0.9.0rc2/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/queue.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.486933 tecton-0.9.0rc2/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.486933 tecton-0.9.0rc2/tecton_materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23171 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/batch_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.486933 tecton-0.9.0rc2/tecton_materialization/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/common/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/common/job_metadata_aws.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/common/job_metadata_gcp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/common/task_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/consumption.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/delta_maintenance.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/entity_deletion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/materialization_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_materialization/ray/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/batch_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/delta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5938 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/job_status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9672 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/materialization_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/ray/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_materialization/remote_host/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/remote_host/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/remote_host/pyspark_remote_host.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_materialization/stream_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.490933 tecton-0.9.0rc2/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21470 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    41821 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.494934 tecton-0.9.0rc2/tecton_proto/auditlog/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auditlog/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auditlog/metadata_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.494934 tecton-0.9.0rc2/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.494934 tecton-0.9.0rc2/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.494934 tecton-0.9.0rc2/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.494934 tecton-0.9.0rc2/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/aws_credentials_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/compute_mode_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/spark_schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/common/time_window_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.494934 tecton-0.9.0rc2/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.498934 tecton-0.9.0rc2/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20254 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/materialization_roles_allowlists_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.498934 tecton-0.9.0rc2/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/offlinestore/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/offlinestore/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/offlinestore/delta/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/offlinestore/delta/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/offlinestore/delta/metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/online_store_writer/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/online_store_writer/copier_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/secrets/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/secrets/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/secrets/secrets_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.502935 tecton-0.9.0rc2/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/snowflake/location_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/snowflake/snowflake_credentials_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.506935 tecton-0.9.0rc2/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.506935 tecton-0.9.0rc2/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.506935 tecton-0.9.0rc2/tecton_proto/testhelperservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/testhelperservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/testhelperservice/test_helper_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.506935 tecton-0.9.0rc2/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.506935 tecton-0.9.0rc2/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.506935 tecton-0.9.0rc2/tecton_snowflake/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/dataframe_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13559 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/queries.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33728 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.510935 tecton-0.9.0rc2/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.510935 tecton-0.9.0rc2/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    35476 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.510935 tecton-0.9.0rc2/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/jars/class_loader.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7188 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15383 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33278 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:49.514936 tecton-0.9.0rc2/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7533 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17887 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-04-01 19:41:45.000000 tecton-0.9.0rc2/tecton_spark/udfs.py
```

### Comparing `tecton-0.9.0rc1/PKG-INFO` & `tecton-0.9.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Provides-Extra: databricks-connect11
 Provides-Extra: pyspark
 Provides-Extra: pyspark3
 Provides-Extra: pyspark3.1
 Provides-Extra: pyspark3.2
 Provides-Extra: pyspark3.3
 Provides-Extra: rift
+Provides-Extra: rift-materialization
 Provides-Extra: snowflake
 Provides-Extra: athena
 Provides-Extra: materialization
 
 ![logo](https://s3.us-west-2.amazonaws.com/tecton.ai.public/documentation/pypi/tecton-logo.svg)
 
 Tecton is the fastest way to build operational machine learning applications. It helps automate real-time decision making like fraud detection, product recommendations, and search result ranking in production applications.
```

### Comparing `tecton-0.9.0rc1/README.md` & `tecton-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/protoc_gen_openapiv2/options/annotations_pb2.py` & `tecton-0.9.0rc2/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `tecton-0.9.0rc2/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/setup.py` & `tecton-0.9.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.9.0rc1',
+    version='0.9.0rc2',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas>=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version', 'pyarrow<15,>=8', 'pydantic<3,>=1.10.13', 'pyyaml', 'setuptools', 'pip', 'pex~=2.1'],
-    extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'rift': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0'], 'snowflake': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=3.0'], 'materialization': ['statsd==3.3.0', 'urllib3<2.0.0']},
+    extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'rift': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0'], 'rift-materialization': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0', 'pydantic<2', 'urllib3<1.27'], 'snowflake': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=3.0'], 'materialization': ['statsd==3.3.0', 'urllib3<2.0.0']},
     packages=packages,
 )
```

### Comparing `tecton-0.9.0rc1/tecton/__init__.py` & `tecton-0.9.0rc2/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/analytics.py` & `tecton-0.9.0rc2/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/athena_api.py` & `tecton-0.9.0rc2/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/data_frame_helper.py` & `tecton-0.9.0rc2/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/delete_keys_api.py` & `tecton-0.9.0rc2/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/display.py` & `tecton-0.9.0rc2/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/env_utils.py` & `tecton-0.9.0rc2/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/errors.py` & `tecton-0.9.0rc2/tecton/_internals/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,14 +557,24 @@
     )
 
 
 def INGESTAPI_USER_ERROR(status_code: int, reason: str, error_message: str):
     return TectonValidationError(f"Received {status_code} {reason} from Stream IngestAPI. Details: \n {error_message}")
 
 
+def AGGREGATION_INTERVAL_SET_COMPACTION():
+    return TectonValidationError("Feature views with stream compaction enabled cannot have `aggregation_interval` set.")
+
+
+def COMPACTION_TIME_WINDOW_SERIES_UNSUPPORTED():
+    return TectonValidationError(
+        "Aggregations using a TimeWindowSeries window are not supported when `stream_compaction_enabled=True`."
+    )
+
+
 # New Read API
 GET_FEATURES_FOR_EVENTS_UNSUPPORTED = TectonValidationError(
     "get_features_for_events() is only supported for SPARK or RIFT Compute Modes."
 )
 
 GET_FEATURES_IN_RANGE_UNSUPPORTED = TectonValidationError(
     "get_features_in_range() is only supported for SPARK or RIFT Compute Modes."
```

### Comparing `tecton-0.9.0rc1/tecton/_internals/find_spark.py` & `tecton-0.9.0rc2/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/ingest_utils.py` & `tecton-0.9.0rc2/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/ingestion.py` & `tecton-0.9.0rc2/tecton/_internals/ingestion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/materialization_api.py` & `tecton-0.9.0rc2/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/metadata_service.py` & `tecton-0.9.0rc2/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/metadata_service_impl/service_modules.py` & `tecton-0.9.0rc2/tecton/_internals/metadata_service_impl/service_modules.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/mock_source_utils.py` & `tecton-0.9.0rc2/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/offline_store_credentials.py` & `tecton-0.9.0rc2/tecton/_internals/offline_store_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/pandas_compat.py` & `tecton-0.9.0rc2/tecton/_internals/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/query_helper.py` & `tecton-0.9.0rc2/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/querytree_api.py` & `tecton-0.9.0rc2/tecton/_internals/querytree_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/repo/function_serialization.py` & `tecton-0.9.0rc2/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/rewrite.py` & `tecton-0.9.0rc2/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/run_api.py` & `tecton-0.9.0rc2/tecton/_internals/run_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/sdk_decorators.py` & `tecton-0.9.0rc2/tecton/_internals/sdk_decorators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/secret_resolver.py` & `tecton-0.9.0rc2/tecton/_internals/secret_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/snowflake_api.py` & `tecton-0.9.0rc2/tecton/_internals/snowflake_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/spark_api.py` & `tecton-0.9.0rc2/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/spark_utils.py` & `tecton-0.9.0rc2/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/tecton_pydantic.py` & `tecton-0.9.0rc2/tecton/_internals/tecton_pydantic.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/time_utils.py` & `tecton-0.9.0rc2/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/type_utils.py` & `tecton-0.9.0rc2/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/utils.py` & `tecton-0.9.0rc2/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/_internals/validations_api.py` & `tecton-0.9.0rc2/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/aggregation_functions.py` & `tecton-0.9.0rc2/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/access_control.py` & `tecton-0.9.0rc2/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/api_key.py` & `tecton-0.9.0rc2/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/auth.py` & `tecton-0.9.0rc2/tecton/cli/auth.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/cli.py` & `tecton-0.9.0rc2/tecton/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/cli_utils.py` & `tecton-0.9.0rc2/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/command.py` & `tecton-0.9.0rc2/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/completion.py` & `tecton-0.9.0rc2/tecton/cli/completion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/engine.py` & `tecton-0.9.0rc2/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/engine_renderer.py` & `tecton-0.9.0rc2/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/environment.py` & `tecton-0.9.0rc2/tecton/cli/environment.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/environment_utils.py` & `tecton-0.9.0rc2/tecton/cli/environment_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/error_utils.py` & `tecton-0.9.0rc2/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/materialization.py` & `tecton-0.9.0rc2/tecton/cli/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/pex_wrapper.py` & `tecton-0.9.0rc2/tecton/cli/pex_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/printer.py` & `tecton-0.9.0rc2/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/repo.py` & `tecton-0.9.0rc2/tecton/cli/repo.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/repo_config.py` & `tecton-0.9.0rc2/tecton/cli/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/repo_utils.py` & `tecton-0.9.0rc2/tecton/cli/repo_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/secrets.py` & `tecton-0.9.0rc2/tecton/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/service_account.py` & `tecton-0.9.0rc2/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/test.py` & `tecton-0.9.0rc2/tecton/cli/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/user.py` & `tecton-0.9.0rc2/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/workspace.py` & `tecton-0.9.0rc2/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/cli/workspace_utils.py` & `tecton-0.9.0rc2/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/fco_listers.py` & `tecton-0.9.0rc2/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/base_tecton_object.py` & `tecton-0.9.0rc2/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/configs.py` & `tecton-0.9.0rc2/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/data_frame.py` & `tecton-0.9.0rc2/tecton/framework/data_frame.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/data_source.py` & `tecton-0.9.0rc2/tecton/framework/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Union
 
 import attrs
+import pandas
 from pyspark.sql import dataframe as pyspark_dataframe
 from pyspark.sql import streaming as pyspark_streaming
 from typeguard import typechecked
 
 from tecton import types
 from tecton._internals import display
 from tecton._internals import errors
@@ -40,14 +41,15 @@
 from tecton_proto.args import fco_args_pb2
 from tecton_proto.args import virtual_data_source_pb2 as virtual_data_source__args_pb2
 from tecton_proto.common import data_source_type_pb2
 from tecton_proto.common import fco_locator_pb2
 from tecton_proto.common import framework_version_pb2
 from tecton_proto.common import schema_container_pb2
 from tecton_proto.common import spark_schema_pb2
+from tecton_proto.common.spark_schema_pb2 import SparkSchema
 from tecton_proto.metadataservice import metadata_service_pb2
 from tecton_proto.validation import validator_pb2
 from tecton_spark import spark_schema_wrapper
 
 
 BatchConfigType = Union[
     configs.FileConfig,
@@ -124,17 +126,26 @@
             validator_pb2.ValidationRequest(validation_args=[self._build_fco_validation_args()]),
             indentation_level,
         )
 
         self._spec = specs.DataSourceSpec.from_args_proto(self._args, self._args_supplement)
 
     @sdk_decorators.assert_local_object
-    def _create_unvalidated_spec(self, mock_data: pyspark_dataframe.DataFrame) -> specs.DataSourceSpec:
+    def _create_unvalidated_spec(
+        self, mock_data: Union[pandas.DataFrame, pyspark_dataframe.DataFrame]
+    ) -> specs.DataSourceSpec:
         """Create an unvalidated spec. Used for user unit testing, where backend validation is unavailable."""
-        schema = spark_schema_wrapper.SparkSchemaWrapper.from_spark_schema(mock_data.schema)
+        if isinstance(mock_data, pyspark_dataframe.DataFrame):
+            schema = spark_schema_wrapper.SparkSchemaWrapper.from_spark_schema(mock_data.schema)
+        elif isinstance(mock_data, pandas.DataFrame):
+            # Using a empty schema for Rift, since Rift does not use the schema for batch sources.
+            schema = SparkSchema()
+        else:
+            msg = f"Unexpected mock source type {type(mock_data)}"
+            raise TypeError(msg)
         # Use the mock schema as both the batch and stream schema because StreamSource specs expect a non-nil stream
         # schema.
         supplement = attrs.evolve(self._args_supplement, batch_schema=schema, stream_schema=schema)
         return specs.DataSourceSpec.from_args_proto(self._args, supplement)
 
     def _derive_schemas(self, indentation_level: int) -> None:
         raise NotImplementedError
```

### Comparing `tecton-0.9.0rc1/tecton/framework/dataset.py` & `tecton-0.9.0rc2/tecton/framework/dataset.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/entity.py` & `tecton-0.9.0rc2/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/feature_service.py` & `tecton-0.9.0rc2/tecton/framework/feature_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/feature_view.py` & `tecton-0.9.0rc2/tecton/framework/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import enum
 import inspect
 import logging
+from datetime import timedelta
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
@@ -16,14 +17,15 @@
 from typing import Union
 from typing import overload
 
 import attrs
 import numpy as np
 import pandas
 import pendulum
+from google.protobuf import duration_pb2
 from pyspark.sql import dataframe as pyspark_dataframe
 from pyspark.sql import streaming
 from typeguard import typechecked
 
 from tecton import tecton_context
 from tecton import types
 from tecton._internals import athena_api
@@ -1129,15 +1131,15 @@
                 raise errors.FV_WITH_INC_BACKFILLS_GET_MATERIALIZED_FEATURES_MOCK_DATA(
                     self.name, self.get_partial_aggregates.__name__
                 )
 
         if not self._feature_definition.is_temporal_aggregate:
             raise errors.GET_PARTIAL_AGGREGATES_UNSUPPORTED_NON_AGGREGATE()
 
-        if self._feature_definition.compaction_enabled_for_materialization:
+        if self._feature_definition.batch_compaction_enabled:
             raise errors.GET_PARTIAL_AGGREGATES_UNSUPPORTED_COMPACTED()
 
         if any(ds._data_source_type == DataSourceType.PUSH_NO_BATCH for ds in self.sources):
             msg = "The `get_partial_aggregates()` method is currently unsupported for Feature Views that are backed by a PushSource without a batch_config."
             raise TectonValidationError(msg)
 
         if entities is not None:
@@ -1504,24 +1506,29 @@
             )
 
     @sdk_decorators.assert_local_object
     def _create_unvalidated_feature_definition(
         self,
         mock_inputs: Optional[Dict[str, Union[pandas.DataFrame, pyspark_dataframe.DataFrame]]] = None,
     ) -> feature_definition_wrapper.FeatureDefinitionWrapper:
-        if mock_inputs:
+        compute_mode = offline_retrieval_compute_mode(conf.get_or_none("TECTON_OFFLINE_RETRIEVAL_COMPUTE_MODE"))
+        # Only convert to PySpark DataFrames if we're in Spark mode.
+        # For all other compute modes (RIFT, SNOWFLAKE) leave the mock_inputs as-is.
+        if mock_inputs and compute_mode == ComputeMode.SPARK:
             mock_inputs = _to_pyspark_mocks(mock_inputs)
-        else:
+        elif not mock_inputs:
             mock_inputs = {}
 
         """Create an unvalidated feature definition. Used for user unit testing, where backend validation is unavailable."""
         input_name_to_ds_ids = pipeline_common.get_input_name_to_ds_id_map(self._args.pipeline)
 
-        if set(input_name_to_ds_ids.keys()) != set(mock_inputs.keys()):
-            raise errors.FV_INVALID_MOCK_SOURCES(list(mock_inputs.keys()), list(input_name_to_ds_ids.keys()))
+        columns = mock_inputs.columns if isinstance(mock_inputs, pandas.DataFrame) else mock_inputs.keys()
+
+        if set(input_name_to_ds_ids.keys()) != set(columns):
+            raise errors.FV_INVALID_MOCK_SOURCES(list(columns), list(input_name_to_ds_ids.keys()))
 
         # It's possible to have the same data source included twice in mock_inputs under two different input names, but
         # we only need to generate an unvalidated spec once for data source. (Putting two conflicting specs with the
         # same id in the fco container will lead to erros.)
         ds_id_to_mock_df = {}
         for input_name, ds_id in input_name_to_ds_ids.items():
             mock_df = mock_inputs[input_name]
@@ -2270,14 +2277,23 @@
             stream_compute = repo_config.get_stream_feature_view_defaults().stream_compute
 
         _validate_fv_input_count([source], feature_view_function)
 
         if has_push_source:
             # Stream Feature Views with Push Sources are mandatorily continuous-mode only.
             stream_processing_mode_ = StreamProcessingMode.CONTINUOUS
+        elif batch_compaction_enabled:
+            # This is a Compacted stream feature view. We set defaults here for compacted feature views. The actual validations
+            # will be in the validation server.
+            if not stream_compaction_enabled:
+                stream_processing_mode_ = (
+                    stream_processing_mode or StreamProcessingMode.CONTINUOUS
+                )  # Default to continuous
+            else:
+                stream_processing_mode_ = stream_processing_mode or None
         else:
             if aggregations:
                 stream_processing_mode_ = stream_processing_mode or StreamProcessingMode.TIME_INTERVAL
             else:
                 stream_processing_mode_ = stream_processing_mode
 
         if feature_view_function:
@@ -4340,17 +4356,19 @@
     monitoring = configs.MonitoringConfig(
         monitor_freshness=monitor_freshness, expected_freshness=expected_feature_freshness, alert_email=alert_email
     )
 
     aggregation_protos = None
     if aggregations:
         is_continuous = stream_processing_mode == StreamProcessingMode.CONTINUOUS
-        if aggregation_interval is None:
-            aggregation_interval = datetime.timedelta(seconds=0)
-
+        if batch_compaction_enabled and stream_compaction_enabled and aggregation_interval:
+            raise errors.AGGREGATION_INTERVAL_SET_COMPACTION()
+        else:
+            if aggregation_interval is None:
+                aggregation_interval = datetime.timedelta(seconds=0)
         aggregation_protos = [
             agg._to_proto(aggregation_interval, is_continuous, batch_compaction_enabled) for agg in aggregations
         ]
 
     secondary_key_output_columns = (
         _create_secondary_key_output_columns(aggregations, aggregation_secondary_key)
         if aggregation_secondary_key
@@ -4402,14 +4420,17 @@
             aggregations=aggregation_protos,
             aggregation_interval=time_utils.timedelta_to_proto(aggregation_interval),
             schema=schema_proto,
             run_transformation_validation=run_transformation_validation,
             tecton_materialization_runtime=tecton_materialization_runtime,
             offline_store=offline_store._to_proto(),
             stream_compaction_enabled=stream_compaction_enabled,
+            stream_compaction_tile_size=_compute_stream_compaction_tile_size(aggregations)
+            if stream_compaction_enabled
+            else None,
             batch_compaction_enabled=batch_compaction_enabled,
             environment=environment,
         ),
         options=options,
         cache_config=cache_config._to_proto() if cache_config else None,
     )
 
@@ -4443,7 +4464,34 @@
                 name=name,
             )
         else:
             msg = f"Unexpected time window type in agg args proto: {type(window)}"
             raise ValueError(msg)
         secondary_key_output_columns.append(output_col)
     return secondary_key_output_columns
+
+
+def _compute_stream_compaction_tile_size(
+    aggregations: Optional[Sequence[configs.Aggregation]],
+) -> Optional[duration_pb2.Duration]:
+    """Calculate stream compaction tile size.
+
+    Only applicable for fvs with stream_comapction_enabled=True. This calculates the tile sized used for the online stream table. Currently, this cannot be set by the user."""
+    if aggregations is None or len(aggregations) == 0:
+        msg = "Only feature views with aggregations can set a stream compaction tile size."
+        raise ValueError(msg)
+
+    relative_time_windows = []
+    for agg in aggregations:
+        if isinstance(agg.time_window, configs.TimeWindow):
+            relative_time_windows.append(agg.time_window)
+        elif isinstance(agg.time_window, configs.TimeWindowSeries):
+            raise errors.COMPACTION_TIME_WINDOW_SERIES_UNSUPPORTED()
+
+    if relative_time_windows:
+        min_time_window = min([window.window_size for window in relative_time_windows])
+        if min_time_window < timedelta(hours=1):
+            return time_utils.timedelta_to_proto(timedelta(minutes=1))
+        elif min_time_window < timedelta(hours=10):
+            return time_utils.timedelta_to_proto(timedelta(minutes=5))
+
+    return time_utils.timedelta_to_proto(timedelta(hours=1))
```

### Comparing `tecton-0.9.0rc1/tecton/framework/filtered_source.py` & `tecton-0.9.0rc2/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/repo_config.py` & `tecton-0.9.0rc2/tecton/framework/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/transformation.py` & `tecton-0.9.0rc2/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/utils.py` & `tecton-0.9.0rc2/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/validation_mode.py` & `tecton-0.9.0rc2/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/framework/workspace.py` & `tecton-0.9.0rc2/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/identities/api_keys.py` & `tecton-0.9.0rc2/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/identities/credentials.py` & `tecton-0.9.0rc2/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/identities/okta.py` & `tecton-0.9.0rc2/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/pytest_tecton.py` & `tecton-0.9.0rc2/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/snowflake_context.py` & `tecton-0.9.0rc2/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/tecton_context.py` & `tecton-0.9.0rc2/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/types.py` & `tecton-0.9.0rc2/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/__diff.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/_dill.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/_objects.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/detect.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/info.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/pointers.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/settings.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/source.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/dill/dill/temp.py` & `tecton-0.9.0rc2/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.9.0rc2/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/vendor_dill.py` & `tecton-0.9.0rc2/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/vendor/vendor_pyspark.py` & `tecton-0.9.0rc2/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton/version.py` & `tecton-0.9.0rc2/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton.egg-info/PKG-INFO` & `tecton-0.9.0rc2/tecton.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.0rc1
+Version: 0.9.0rc2
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Provides-Extra: databricks-connect11
 Provides-Extra: pyspark
 Provides-Extra: pyspark3
 Provides-Extra: pyspark3.1
 Provides-Extra: pyspark3.2
 Provides-Extra: pyspark3.3
 Provides-Extra: rift
+Provides-Extra: rift-materialization
 Provides-Extra: snowflake
 Provides-Extra: athena
 Provides-Extra: materialization
 
 ![logo](https://s3.us-west-2.amazonaws.com/tecton.ai.public/documentation/pypi/tecton-logo.svg)
 
 Tecton is the fastest way to build operational machine learning applications. It helps automate real-time decision making like fraud detection, product recommendations, and search result ranking in production applications.
```

### Comparing `tecton-0.9.0rc1/tecton.egg-info/SOURCES.txt` & `tecton-0.9.0rc2/tecton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton.egg-info/requires.txt` & `tecton-0.9.0rc2/tecton.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -63,9 +63,16 @@
 pyspark[sql]~=3.3.2
 
 [rift]
 duckdb==0.10.0
 deltalake~=0.15
 pyarrow>=11.0.0
 
+[rift-materialization]
+duckdb==0.10.0
+deltalake~=0.15
+pyarrow>=11.0.0
+pydantic<2
+urllib3<1.27
+
 [snowflake]
 snowflake-snowpark-python[pandas]~=1.0
```

### Comparing `tecton-0.9.0rc1/tecton_athena/athena_session.py` & `tecton-0.9.0rc2/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/data_catalog_helper.py` & `tecton-0.9.0rc2/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/odfv_helper.py` & `tecton-0.9.0rc2/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/query/translate.py` & `tecton-0.9.0rc2/tecton_athena/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/sql_helper.py` & `tecton-0.9.0rc2/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/templates/create_table.sql` & `tecton-0.9.0rc2/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/templates/historical_features.sql` & `tecton-0.9.0rc2/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/templates/materialization_tile.sql` & `tecton-0.9.0rc2/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.9.0rc2/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/templates/time_limit.sql` & `tecton-0.9.0rc2/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_athena/templates_utils.py` & `tecton-0.9.0rc2/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/aggregation_utils.py` & `tecton-0.9.0rc2/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/arrow.py` & `tecton-0.9.0rc2/tecton_core/arrow.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/aws_credentials.py` & `tecton-0.9.0rc2/tecton_core/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/compute_mode.py` & `tecton-0.9.0rc2/tecton_core/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/conf.py` & `tecton-0.9.0rc2/tecton_core/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/data_types.py` & `tecton-0.9.0rc2/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/duckdb_context.py` & `tecton-0.9.0rc2/tecton_core/duckdb_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,24 +54,33 @@
                 connection.sql("INSTALL tecton")
             else:
                 # Otherwise, always download the latest version of the duckdb extension
                 # from the repo.
                 connection.sql("FORCE INSTALL tecton")
             connection.sql("LOAD tecton")
 
+        connection.sql("SET TimeZone='UTC'")
+
     def get_connection(self):
         return self._connection
 
     @classmethod
     def get_instance(cls, home_dir_override: Optional[str] = None) -> "DuckDBContext":
         """
         Get the singleton instance of DuckDBContext.
         """
         if cls._current_context_instance is None:
-            import duckdb
+            try:
+                import duckdb
+            except ImportError:
+                msg = (
+                    "Couldn't initialize Rift compute. "
+                    "To use Rift install all Rift dependencies first by executing `pip install tecton[rift]`."
+                )
+                raise RuntimeError(msg)
 
             conn_config = {}
             if conf.get_or_none("DUCKDB_EXTENSION_REPO"):
                 conn_config["allow_unsigned_extensions"] = "true"
 
             if conf.get_bool("DUCKDB_PERSIST_DB"):
                 conn = duckdb.connect("duckdb.db", config=conn_config)
```

### Comparing `tecton-0.9.0rc1/tecton_core/errors.py` & `tecton-0.9.0rc2/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/fco_container.py` & `tecton-0.9.0rc2/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/feature_definition_wrapper.py` & `tecton-0.9.0rc2/tecton_core/feature_definition_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -416,14 +416,30 @@
                 self.fv_spec.batch_schedule, self.get_feature_store_format_version
             )
 
         msg = "Invalid invocation on unsupported FeatureView type"
         raise TypeError(msg)
 
     @property
+    def get_tile_interval_duration_for_offline_store(self) -> pendulum.Duration:
+        """The tile interval to be used for offline retrieval.
+
+        For most cases this will be the aggregation interval. For fvs with stream_compaction_enabled=True, the online store is tiled, but offline retrieval should not be using tiles (like continuous mode).
+        """
+        if self.is_temporal_aggregate and self.fv_spec.stream_compaction_enabled:
+            return pendulum.Duration(seconds=0)
+        return self.get_tile_interval
+
+    @property
+    def get_tile_interval_seconds_for_offline_store(self) -> int:
+        return time_utils.convert_timedelta_for_version(
+            self.get_tile_interval_duration_for_offline_store, self.get_feature_store_format_version
+        )
+
+    @property
     def get_aggregate_slide_interval_string(self) -> str:
         if not self.is_temporal_aggregate:
             msg = "Invalid invocation on unsupported FeatureView type"
             raise TypeError(msg)
 
         return self.fv_spec.slide_interval_string
 
@@ -514,15 +530,15 @@
         if not self.is_temporal_aggregate:
             return None
 
         # TODO(sanika) - trailing_time_window_aggregation fills time_window based on data proto, which is used in to_query methods.
         # This should be cleaned up when we work on ranges using offset
         return feature_view_pb2.TrailingTimeWindowAggregation(
             time_key=self.timestamp_key,
-            is_continuous=self.fv_spec.is_continuous,
+            is_continuous=self.is_continuous,
             aggregation_slide_period=self.aggregate_slide_interval,
             features=self.fv_spec.aggregate_features,
         )
 
     @property
     def serving_ttl(self) -> Optional[pendulum.Duration]:
         if isinstance(self.fv_spec, (specs.MaterializedFeatureViewSpec, specs.FeatureTableSpec)):
@@ -597,19 +613,29 @@
     def time_range_for_relative_time_window(self, time_window: RelativeTimeWindowSpec) -> Tuple[int, int]:
         start = self.earliest_anchor_time_from_window_start(time_window.window_start)
         end = convert_timedelta_for_version(time_window.window_end, self.get_feature_store_format_version)
         assert start <= end
         return start, end
 
     @property
-    def compaction_enabled_for_materialization(self):
+    def batch_compaction_enabled(self):
+        """Whether a feature view has batch_compaction_enabled set to True."""
         if not isinstance(self.fv_spec, specs.MaterializedFeatureViewSpec):
             return False
         return self.fv_spec.batch_compaction_enabled
 
+    @property
+    def stream_compaction_enabled(self):
+        """Whether a stream feature view has stream_compaction_enabled set to True.
+
+        stream_compaction_enabled is only applicable to stream feature views with batch_compaction_enabled=True."""
+        if not isinstance(self.fv_spec, specs.MaterializedFeatureViewSpec):
+            return False
+        return self.fv_spec.stream_compaction_enabled
+
 
 def pipeline_to_ds_inputs(pipeline: Pipeline) -> Dict[str, DataSourceNode]:
     ds_nodes: Dict[str, DataSourceNode] = {}
 
     def _recurse_pipeline_to_ds_nodes(pipeline_node: PipelineNode, ds_nodes_: Dict[str, DataSourceNode]) -> None:
         if pipeline_node.HasField("data_source_node"):
             ds_nodes_[pipeline_node.data_source_node.input_name] = pipeline_node.data_source_node
```

### Comparing `tecton-0.9.0rc1/tecton_core/feature_set_config.py` & `tecton-0.9.0rc2/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/feature_view_utils.py` & `tecton-0.9.0rc2/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/function_deserialization.py` & `tecton-0.9.0rc2/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/http.py` & `tecton-0.9.0rc2/tecton_core/http.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/id_helper.py` & `tecton-0.9.0rc2/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/iterators.py` & `tecton-0.9.0rc2/tecton_core/iterators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/materialization_context.py` & `tecton-0.9.0rc2/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/metadata_service_impl/error_lib.py` & `tecton-0.9.0rc2/tecton_core/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/metadata_service_impl/http_client.py` & `tecton-0.9.0rc2/tecton_core/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/metadata_service_impl/providers.py` & `tecton-0.9.0rc2/tecton_core/metadata_service_impl/providers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/metadata_service_impl/response.py` & `tecton-0.9.0rc2/tecton_core/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/metadata_service_impl/service_calls.py` & `tecton-0.9.0rc2/tecton_core/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/offline_store.py` & `tecton-0.9.0rc2/tecton_core/offline_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,15 @@
     if options is None:
         msg = f"Unable to retrieve S3 store credentials for feature view {fd.name}."
         raise ValueError(msg)
 
     return options
 
 
-def _patch_arrow_schema(schema: pyarrow.Schema) -> pyarrow.Schema:
+def patch_timestamps_in_arrow_schema(schema: pyarrow.Schema) -> pyarrow.Schema:
     """Patches schema to replace tz-naive columns with UTC timestamps"""
     for idx, field in enumerate(schema):
         if isinstance(field.type, pyarrow.TimestampType) and field.type.tz is None:
             schema = schema.set(idx, pyarrow.field(field.name, pyarrow.timestamp(field.type.unit, "UTC")))
     return schema
 
 
@@ -373,15 +373,22 @@
         if self._params.delta_table_uri.startswith("s3"):
             return get_s3_options_for_fd(self._fd, self._options_providers)
 
         return None
 
     def read(self, partition_time_limits: Optional[pendulum.Period] = None) -> "pyarrow.RecordBatchReader":
         # TODO(TEC-16757): Move import to top of file.
-        from deltalake import DeltaTable
+        try:
+            from deltalake import DeltaTable
+        except ImportError:
+            msg = (
+                "Couldn't initialize Rift compute. "
+                "To use Rift install all Rift dependencies first by executing `pip install tecton[rift]`."
+            )
+            raise RuntimeError(msg)
 
         filters = None
         if partition_time_limits is not None and self._partition_size:
             filters = []
             aligned_start_time = time_utils.align_time_downwards(partition_time_limits.start, self._partition_size)
             start_partition = datetime_to_partition_str(aligned_start_time, self._partition_size)
             filters.append((TIME_PARTITION, ">=", start_partition))
@@ -419,15 +426,15 @@
 
         # "partitions" parameters is applied earlier by DeltaTable itself (and not passed to pyarrow like filters)
         ds = table.to_pyarrow_dataset(partitions=filters)
         batches = ds.to_batches(
             batch_readahead=int(conf.get_or_raise("ARROW_BATCH_READ_AHEAD")),
             fragment_readahead=int(conf.get_or_raise("ARROW_FRAGMENT_READ_AHEAD")),
         )
-        schema = _patch_arrow_schema(ds.schema)
+        schema = patch_timestamps_in_arrow_schema(ds.schema)
         return pyarrow.RecordBatchReader.from_batches(schema, batches)
 
 
 class ParquetReader(OfflineStoreReader):
     def __init__(
         self,
         fd: FeatureDefinitionWrapper,
@@ -493,9 +500,9 @@
         )
         ds = pyarrow.dataset.FileSystemDatasetFactory(fs, selector, file_format, options).finish()
         batches = ds.to_batches(
             filter=self._filter(partition_time_limits),
             batch_readahead=int(conf.get_or_raise("ARROW_BATCH_READ_AHEAD")),
             fragment_readahead=int(conf.get_or_raise("ARROW_FRAGMENT_READ_AHEAD")),
         )
-        schema = _patch_arrow_schema(ds.schema)
+        schema = patch_timestamps_in_arrow_schema(ds.schema)
         return pyarrow.RecordBatchReader.from_batches(schema, batches)
```

### Comparing `tecton-0.9.0rc1/tecton_core/online_serving_index.py` & `tecton-0.9.0rc2/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/pipeline_common.py` & `tecton-0.9.0rc2/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/aggregation_plans.py` & `tecton-0.9.0rc2/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/builder.py` & `tecton-0.9.0rc2/tecton_core/query/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     if for_stream:
         watermark = _get_stream_watermark(fdw)
         if watermark:
             tree = StreamWatermarkNode(dialect, compute_mode, tree, fdw.time_key, watermark).as_ref()
     if enable_feature_metrics:
         tree = MetricsCollectorNode(dialect, compute_mode, tree).as_ref()
 
-    if fdw.compaction_enabled_for_materialization and not for_stream:
+    if fdw.batch_compaction_enabled and not for_stream:
         return _build_compaction_materialization_querytree(
             dialect=dialect,
             compute_mode=compute_mode,
             fdw=fdw,
             pipeline_tree=tree,
         )
 
@@ -456,24 +456,25 @@
             fdw,
             for_stream=False,
             feature_data_time_limits=feature_data_time_limits,
             aggregation_anchor_time=aggregation_anchor_time,
             include_window_end_time=include_window_end_time,
         )
 
-    if fdw.compaction_enabled_for_materialization and fdw.is_temporal_aggregate:
+    if fdw.batch_compaction_enabled and fdw.is_temporal_aggregate:
         end_column_name = window_end_column_name() if include_window_end_time else None
         tree = PartialAggNode(
             dialect=dialect,
             compute_mode=compute_mode,
             input_node=tree,
             fdw=fdw,
             window_start_column_name=anchor_time(),
             window_end_column_name=end_column_name,
             aggregation_anchor_time=aggregation_anchor_time,
+            create_tiles=fdw.get_tile_interval_seconds_for_offline_store > 0,
         ).as_ref()
 
     return tree
 
 
 def build_temporal_time_range_query(
     dialect: Dialect,
@@ -611,15 +612,19 @@
             compute_mode=compute_mode,
             full_aggregation_node=full_aggregation_node,
             fdw=fdw,
             group_by_columns=[*list(fdw.join_keys), anchor_time()],
         ).as_ref()
 
     qt = _filter_and_update_timestamp_columns(
-        full_aggregation_node, dialect, compute_mode, fdw, show_effective_time=True
+        full_aggregation_node,
+        dialect,
+        compute_mode,
+        fdw,
+        show_effective_time=True,
     )
 
     qt = TakeLastRowNode(
         dialect,
         compute_mode,
         input_node=qt,
         partition_by_columns=(*fdw.join_keys, effective_timestamp()),
@@ -677,15 +682,20 @@
             compute_mode=compute_mode,
             full_aggregation_node=full_aggregation_node,
             fdw=fdw,
             group_by_columns=[*list(fdw.join_keys), anchor_time()],
         ).as_ref()
 
     qt = _filter_and_update_timestamp_columns(
-        full_aggregation_node, dialect, compute_mode, fdw, respect_feature_start_time=True, show_effective_time=True
+        full_aggregation_node,
+        dialect,
+        compute_mode,
+        fdw,
+        respect_feature_start_time=True,
+        show_effective_time=True,
     )
 
     if entities is not None:
         qt = _filter_entity_dataframe(dialect, compute_mode, qt, entities)
 
     qt = _filter_by_time_range(dialect, compute_mode, qt, query_time_range, fdw.timestamp_key, fdw.timestamp_key)
 
@@ -727,17 +737,21 @@
         full_aggregation_node = AggregationSecondaryKeyRollupNode(
             dialect=dialect,
             compute_mode=compute_mode,
             full_aggregation_node=full_aggregation_node,
             fdw=fdw,
             group_by_columns=[*list(fdw.join_keys), anchor_time()],
         ).as_ref()
-
     qt = _filter_and_update_timestamp_columns(
-        full_aggregation_node, dialect, compute_mode, fdw, respect_feature_start_time=False, show_effective_time=False
+        full_aggregation_node,
+        dialect,
+        compute_mode,
+        fdw,
+        respect_feature_start_time=False,
+        show_effective_time=False,
     )
 
     return qt
 
 
 def _filter_by_time_range(
     dialect: Dialect,
@@ -787,30 +801,34 @@
     2. Converts the anchor time to a timestamp from epoch ns.
     3. Adjusts the anchor time to reflect the end of the materialization window
     4. Optionally adds the _effective_time column
     """
 
     if respect_feature_start_time and fdw.feature_start_timestamp:
         full_aggregation_node = RespectFeatureStartTimeNode.for_anchor_time_column(
-            dialect, compute_mode, full_aggregation_node, anchor_time(), fdw
+            dialect,
+            compute_mode,
+            full_aggregation_node,
+            anchor_time(),
+            fdw,
         ).as_ref()
 
     # The `AsofJoinFullAggNode` returned by `build_get_full_agg_features` converts timestamps to epochs. We convert back
     # from epochs to timestamps so that we can add an effective timestamp column.
     qt = ConvertEpochToTimestampNode(
         dialect, compute_mode, full_aggregation_node, {anchor_time(): fdw.get_feature_store_format_version}
     ).as_ref()
 
     # We want the time to be on the end of the window not the start.
     qt = AddDurationNode(
         dialect,
         compute_mode,
         qt,
         timestamp_field=anchor_time(),
-        duration=fdw.get_tile_interval,
+        duration=fdw.get_tile_interval_duration_for_offline_store,
         new_column_name=fdw.trailing_time_window_aggregation.time_key,
     ).as_ref()
     qt = RenameColsNode(dialect, compute_mode, qt, drop=[anchor_time()]).as_ref()
 
     if show_effective_time:
         batch_schedule_seconds = 0 if fdw.is_feature_table else fdw.batch_materialization_schedule.in_seconds()
         qt = AddEffectiveTimestampNode(
@@ -885,15 +903,14 @@
         spine_node = RenameColsNode(
             dialect, compute_mode, spine_node, mapping={spine_time_field: fdw.timestamp_key}
         ).as_ref()
     if any(jk[0] != jk[1] for jk in dac.join_keys):
         spine_node = RenameColsNode(
             dialect, compute_mode, spine_node, mapping={jk[0]: jk[1] for jk in dac.join_keys if jk[0] != jk[1]}
         ).as_ref()
-
     if fdw.is_temporal or fdw.is_feature_table:
         ret = _build_spine_query_tree_temporal_or_feature_table(
             dialect=dialect,
             compute_mode=compute_mode,
             spine_node=spine_node,
             dac=dac,
             data_delay_seconds=fdw.online_store_data_delay_seconds,
@@ -909,15 +926,19 @@
             # NOTE: feature_data_time_limits is set to None since time pushdown
             # should happen as part of a optimization rewrite.
             feature_data_time_limits=None,
             aggregation_anchor_time=None,
         )
 
         augmented_spine = _augment_spine_for_window_aggregation(
-            dialect, compute_mode, fdw, spine_node, partial_agg_node
+            dialect,
+            compute_mode,
+            fdw,
+            spine_node,
+            partial_agg_node,
         )
 
         full_agg_node = AsofJoinFullAggNode(
             dialect=dialect,
             compute_mode=compute_mode,
             spine=augmented_spine,
             partial_agg_node=partial_agg_node,
@@ -938,15 +959,19 @@
                 #   2. Grouping by TECTON_UNIQUE_ID_COL can distinguish duplicated rows in the spine.
                 group_by_columns=[*list(fdw.join_keys), anchor_time(), fdw.timestamp_key, tecton_unique_id_col()],
             ).as_ref()
             full_agg_node = RenameColsNode(dialect, compute_mode, full_agg_node, drop=[tecton_unique_id_col()]).as_ref()
 
         if fdw.feature_start_timestamp:
             full_agg_node = RespectFeatureStartTimeNode.for_anchor_time_column(
-                dialect, compute_mode, full_agg_node, anchor_time(), fdw
+                dialect,
+                compute_mode,
+                full_agg_node,
+                anchor_time(),
+                fdw,
             ).as_ref()
         ret = _rename_feature_columns_and_drop_non_feature_columns(
             dialect, compute_mode, dac, full_agg_node, use_namespace_feature_prefix
         )
     elif fdw.is_on_demand:
         inputs = find_dependent_feature_set_items(
             fdw.fco_container,
@@ -1270,15 +1295,15 @@
     augmented_spine = AddRetrievalAnchorTimeNode(
         dialect,
         compute_mode,
         spine_node,
         name=fdw.name,
         feature_store_format_version=fdw.get_feature_store_format_version,
         batch_schedule=fdw.get_batch_schedule_for_version,
-        tile_interval=fdw.get_tile_interval_for_version,
+        tile_interval=fdw.get_tile_interval_seconds_for_offline_store,
         timestamp_field=fdw.timestamp_key,
         is_stream=fdw.is_stream,
         data_delay_seconds=fdw.online_store_data_delay_seconds,
     ).as_ref()
 
     # We need to explode the spine for the secondary key if:
     #     1. A Feature View with an aggregation_secondary_key: an aggregation_secondary_key is never in the spine,
```

### Comparing `tecton-0.9.0rc1/tecton_core/query/compaction_utils.py` & `tecton-0.9.0rc2/tecton_core/query/compaction_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/duckdb/compute.py` & `tecton-0.9.0rc2/tecton_core/query/duckdb/compute.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 import logging
 import re
 import typing
 from typing import Optional
 from typing import Union
 
 import attrs
-import duckdb
+
+
+try:
+    import duckdb
+except ImportError:
+    msg = (
+        "Couldn't initialize Rift compute. "
+        "To use Rift install all Rift dependencies first by executing `pip install tecton[rift]`."
+    )
+    raise RuntimeError(msg)
 import pandas as pd
 import pyarrow
 import pyarrow.dataset
 import pyarrow.fs
 import pyarrow.json
 import sqlparse
 from duckdb import DuckDBPyConnection
@@ -93,14 +102,16 @@
         if monitor:
             monitor.set_query(sql_string)
 
         # Need to use DuckDB cursor (which creates a new connection based on the original connection)
         # to be thread-safe. It avoids a mysterious "unsuccessful or closed pending query result" error too.
         try:
             cursor = self.session.cursor()
+            # Although we set timezone globally, DuckDB still needs this cursor-level config to produce
+            # correct arrow result. Otherwise, timestamps in arrow table will have a local timezone.
             cursor.sql("SET TimeZone='UTC'")
             duckdb_relation = cursor.sql(sql_string)
             if return_dataframe:
                 res = duckdb_relation.fetch_arrow_reader()
             else:
                 res = None
```

### Comparing `tecton-0.9.0rc1/tecton_core/query/duckdb/nodes.py` & `tecton-0.9.0rc2/tecton_core/query/duckdb/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             dialect=query_node.dialect,
             compute_mode=query_node.compute_mode,
             input_node=query_node.input_node,
             fdw=query_node.fdw,
             window_start_column_name=query_node.window_start_column_name,
             window_end_column_name=query_node.window_end_column_name,
             aggregation_anchor_time=query_node.aggregation_anchor_time,
+            create_tiles=query_node.create_tiles,
         )
 
     def _get_partial_agg_columns_and_names(self) -> List[Tuple[Term, str]]:
         """
         Primarily overwritten to do additional type casts to make DuckDB's post-aggregation types consistent with Spark
 
         The two main cases:
```

### Comparing `tecton-0.9.0rc1/tecton_core/query/duckdb/rewrite.py` & `tecton-0.9.0rc2/tecton_core/query/duckdb/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/errors.py` & `tecton-0.9.0rc2/tecton_core/query/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/executor_params.py` & `tecton-0.9.0rc2/tecton_core/query/executor_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/executor_utils.py` & `tecton-0.9.0rc2/tecton_core/query/executor_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def set_query(self, stage_id: int, sql: str) -> None:
         pass
 
     def update_progress(self, stage_id: int, progress: float) -> None:
         pass
 
-    def set_failed(self, stage_id: int, exc: Exception, user_error: bool) -> None:
+    def set_failed(self, stage_id: int, user_error: bool) -> None:
         pass
 
     def set_completed(self, stage_id: int) -> None:
         pass
 
 
 class DebugOutput(QueryTreeMonitor):
@@ -40,15 +40,15 @@
         return 0
 
     def set_completed(self, stage_id: int) -> None:
         stage_done_time = datetime.now()
         if self.is_debug:
             logger.warning(f"{self.step} took time (sec): {(stage_done_time - self.start_time).total_seconds()}")
 
-    def set_failed(self, stage_id: int, exc: Exception, user_error: bool) -> None:
+    def set_failed(self, stage_id: int, user_error: bool) -> None:
         return self.set_completed(stage_id)
 
 
 def get_stage_type_for_dialect(dialect: Dialect) -> TectonManagedStage.StageType:
     if dialect == Dialect.SNOWFLAKE:
         return TectonManagedStage.StageType.SNOWFLAKE
```

### Comparing `tecton-0.9.0rc1/tecton_core/query/node_interface.py` & `tecton-0.9.0rc2/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/node_utils.py` & `tecton-0.9.0rc2/tecton_core/query/node_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/nodes.py` & `tecton-0.9.0rc2/tecton_core/query/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     """
 
     feature_definition_wrapper: FeatureDefinitionWrapper
     partition_time_filter: Optional[pendulum.Period] = None
 
     @property
     def columns(self) -> Sequence[str]:
-        if self.feature_definition_wrapper.compaction_enabled_for_materialization:
+        if self.feature_definition_wrapper.batch_compaction_enabled:
             return self.feature_definition_wrapper.view_schema.column_names()
 
         store_type = get_offline_store_type(self.feature_definition_wrapper)
         cols = self.feature_definition_wrapper.materialization_schema.column_names()
         if store_type == OfflineStoreType.SNOWFLAKE:
             if self.feature_definition_wrapper.is_temporal_aggregate:
                 # Snowflake stores the timestamp_key instead of _anchor_time in offline store, but it's not used in QT for aggregates
@@ -1316,21 +1316,24 @@
     Attributes:
         input_node: The input node to be transformed.
         fdw: The feature view to be partially aggregated.
         window_start_column_name: The name of the anchor time column.
         window_end_column_name: If set, a column will be added to represent the end times of the tiles, and it will
             have name `window_end_column_name`. This is ignored for continuous mode.
         aggregation_anchor_time: If set, it will be used to determine the offset for the tiles.
+        create_tiles: If set to True, the resulting dataframe will be tiled by the aggregation interval. If set to False, the resulting dataframe will have an anchor time column
+            that is just a copy of the input timestamp column. If set to None, the default behavior for the fv type will be used (ie continuous vs non-continuous).
     """
 
     input_node: NodeRef
     fdw: FeatureDefinitionWrapper = attrs.field()
     window_start_column_name: str
     window_end_column_name: Optional[str] = None
     aggregation_anchor_time: Optional[datetime] = None
+    create_tiles: Optional[bool] = None
 
     @property
     def columns(self) -> Sequence[str]:
         cols = list(self.fdw.materialization_schema.column_names())
         # TODO(danny): Move this logic into just the Snowflake version of this node
         # Snowflake stores timestamp key in offline store, so it has timestamp key in materialized schema.
         # But we are returning _ANCHOR_TIME here for partial agg node.
@@ -2182,24 +2185,26 @@
         scenarios where we want to apply this logic to 'anchor
         time' columns.
         """
         start_time_anchor_units = time_utils.convert_timestamp_for_version(
             fdw.feature_start_timestamp, fdw.get_feature_store_format_version
         )
 
+        tile_interval = fdw.get_tile_interval_seconds_for_offline_store
+
         # TODO: ideally we could join using 'window end' timestamps rather
         # than 'window start' anchor times and avoid this complexity.
-        if fdw.is_continuous:
+        if tile_interval == 0:
             # No correction needed since the earliest 'anchor time' is the
             # feature start time for continuous.
             ts = start_time_anchor_units
         else:
             # We have to subtract the tile interval from the start time to get
             # the appropriate earliest anchor time.
-            ts = start_time_anchor_units - fdw.get_tile_interval_for_version
+            ts = start_time_anchor_units - tile_interval
 
         # NOTE: this filter is extremely important for correctness.
         #   The offline store contains partial aggregates from _before_ the
         #   feature start time (with the goal of having the feature start
         #   time be the first complete aggregate). This filter ensures that
         #   spine timestamps from before the feature start time, but after
         #   we have partial aggregates in the offline store, receive null
```

### Comparing `tecton-0.9.0rc1/tecton_core/query/pandas/compute.py` & `tecton-0.9.0rc2/tecton_core/query/pandas/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/pandas/node.py` & `tecton-0.9.0rc2/tecton_core/query/pandas/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/pandas/nodes.py` & `tecton-0.9.0rc2/tecton_core/query/pandas/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/pandas/pipeline_helper.py` & `tecton-0.9.0rc2/tecton_core/query/pandas/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/pandas/rewrite.py` & `tecton-0.9.0rc2/tecton_core/query/pandas/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/pandas/translate.py` & `tecton-0.9.0rc2/tecton_core/query/pandas/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/pipeline_sql_builder.py` & `tecton-0.9.0rc2/tecton_core/query/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/prefixed_uri_resolver.py` & `tecton-0.9.0rc2/tecton_core/query/prefixed_uri_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/query_tree_compute.py` & `tecton-0.9.0rc2/tecton_core/query/query_tree_compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/query_tree_executor.py` & `tecton-0.9.0rc2/tecton_core/query/query_tree_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,19 +149,19 @@
 
         try:
             self.monitor.update_progress(monitor_stage_id, 0)
             yield ComputeMonitor(
                 log_progress=lambda p: self.monitor.update_progress(monitor_stage_id, p),
                 set_query=lambda q: self.monitor.set_query(monitor_stage_id, q),
             )
-        except UserErrors as exc:
-            self.monitor.set_failed(monitor_stage_id, exc, user_error=True)
+        except UserErrors:
+            self.monitor.set_failed(monitor_stage_id, user_error=True)
             raise
-        except Exception as exc:
-            self.monitor.set_failed(monitor_stage_id, exc, user_error=False)
+        except Exception:
+            self.monitor.set_failed(monitor_stage_id, user_error=False)
             raise
         else:
             self.monitor.update_progress(monitor_stage_id, 1)
             self.monitor.set_completed(monitor_stage_id)
 
     def exec_qt(self, qt_root: NodeRef) -> QueryTreeOutput:
         # Make copy so the execution doesn't mutate the original QT visible to users
```

### Comparing `tecton-0.9.0rc1/tecton_core/query/snowflake/compute.py` & `tecton-0.9.0rc2/tecton_core/query/snowflake/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query/sql_compat.py` & `tecton-0.9.0rc2/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/query_consts.py` & `tecton-0.9.0rc2/tecton_core/query_consts.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/repo_file_handler.py` & `tecton-0.9.0rc2/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/request_context.py` & `tecton-0.9.0rc2/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/schema.py` & `tecton-0.9.0rc2/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/schema_derivation_utils.py` & `tecton-0.9.0rc2/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/schema_validation.py` & `tecton-0.9.0rc2/tecton_core/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/secrets.py` & `tecton-0.9.0rc2/tecton_core/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/snowflake_context.py` & `tecton-0.9.0rc2/tecton_core/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/__init__.py` & `tecton-0.9.0rc2/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/data_source_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/data_source_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/entity_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/feature_service_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/feature_view_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/feature_view_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import enum
-from datetime import timedelta
 from types import MappingProxyType
 from typing import Any
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Tuple
 from typing import Union
@@ -212,14 +211,15 @@
     # TODO(TEC-12321): Audit and fix feature view spec fields that should be required.
     # See failure: https://tectonworkspace.slack.com/archives/C04L8M14XGX/p1675279851469019
     batch_trigger: Optional[feature_view__args_pb2.BatchTriggerType.ValueType]
     manual_trigger_backfill_end_time: Optional[pendulum.DateTime]
 
     online_batch_table_format: Optional[OnlineBatchTableFormat]
     batch_compaction_enabled: bool
+    stream_compaction_enabled: bool
 
     has_explicit_view_schema: bool
 
     @classmethod
     @typechecked
     def from_data_proto(cls, proto: feature_view__data_pb2.FeatureView) -> "MaterializedFeatureViewSpec":
         if proto.HasField("temporal_aggregate"):
@@ -315,14 +315,15 @@
             ),
             url=utils.get_field_or_none(proto, "web_url"),
             online_batch_table_format=_get_online_batch_table_format(proto.schemas),
             batch_compute_mode=BatchComputeMode(proto.batch_compute_mode)
             if proto.HasField("batch_compute_mode")
             else None,
             batch_compaction_enabled=proto.materialization_params.batch_compaction_enabled,
+            stream_compaction_enabled=proto.materialization_params.stream_compaction_enabled,
             options=MappingProxyType(proto.options),
         )
 
     @classmethod
     @typechecked
     def from_args_proto(
         cls, proto: feature_view__args_pb2.FeatureViewArgs, supplement: FeatureViewSpecArgsSupplement
@@ -337,15 +338,15 @@
         aggregate_features = get_aggregate_features_from_feature_view_args(proto)
 
         is_aggregate = len(proto.materialized_feature_view_args.aggregations) > 0
         if is_aggregate:
             fv_type = MaterializedFeatureViewType.TEMPORAL_AGGREGATE
 
             slide_interval_proto = _get_aggregation_interval_from_feature_view_args(
-                proto, is_continuous, data_source_type, aggregate_features
+                proto, is_continuous, data_source_type
             )
             if slide_interval_proto:
                 slide_interval = time_utils.proto_to_duration(slide_interval_proto)
                 slide_interval_string = feature_view_utils.construct_aggregation_interval_name(
                     slide_interval_proto, is_continuous
                 )
             else:
@@ -438,14 +439,15 @@
             online_batch_table_format=OnlineBatchTableFormat.from_proto(supplement.online_batch_table_format)
             if supplement.online_batch_table_format
             else None,
             batch_compute_mode=BatchComputeMode(proto.batch_compute_mode)
             if proto.HasField("batch_compute_mode")
             else None,
             batch_compaction_enabled=batch_compaction_enabled,
+            stream_compaction_enabled=proto.materialized_feature_view_args.stream_compaction_enabled,
             options=MappingProxyType(proto.options),
         )
 
     @property
     def features(self) -> List[str]:
         if len(self.aggregate_features) > 0:
             # Temporal aggregate feature view.
@@ -784,40 +786,27 @@
 
 
 @typechecked
 def _get_aggregation_interval_from_feature_view_args(
     proto: feature_view__args_pb2.FeatureViewArgs,
     is_continuous: bool,
     data_source_type: Optional[data_source_type_pb2.DataSourceType.ValueType],
-    aggregate_features: Tuple[feature_view__data_pb2.AggregateFeature, ...],
 ) -> Optional[duration_pb2.Duration]:
-    if not proto.materialized_feature_view_args.batch_compaction_enabled or is_continuous:
-        return utils.get_field_or_none(proto.materialized_feature_view_args, "aggregation_interval")
-
-    batch_schedule = utils.get_field_or_none(proto.materialized_feature_view_args, "batch_schedule")
-    is_stream = data_source_type == data_source_type_pb2.DataSourceType.STREAM_WITH_BATCH if data_source_type else False
-    if not is_stream:
+    if proto.materialized_feature_view_args.batch_compaction_enabled:
+        is_stream = (
+            data_source_type == data_source_type_pb2.DataSourceType.STREAM_WITH_BATCH if data_source_type else False
+        )
         # Default set in Kotlin for batch fvs with compaction is the batch schedule. Batch schedule is required for fvs with batch_compaction_enabled=True
-        return batch_schedule
-
-    # Stream FV with batch_compaction_enabled=True and stream_compaction_enabled=True.
-    # Calculate stream compaction tile size. This is not user configurable, and calculated in Kotlin during plan/apply.
-    relative_time_windows = [
-        RelativeTimeWindowSpec.from_args_proto(agg.time_window)
-        for agg in aggregate_features
-        if agg.time_window.HasField("relative_time_window")
-    ]
-    if relative_time_windows:
-        min_time_window = min([window.window_duration() for window in relative_time_windows])
-        if min_time_window < timedelta(hours=1):
-            return time_utils.timedelta_to_proto(timedelta(minutes=1))
-        elif min_time_window < timedelta(hours=10):
-            return time_utils.timedelta_to_proto(timedelta(minutes=5))
+        # Default set in Kotlin for non-continuous stream fvs with compaction is the stream compaction tile size.
+        if not is_stream:
+            return utils.get_field_or_none(proto.materialized_feature_view_args, "batch_schedule")
+        elif not is_continuous:
+            return utils.get_field_or_none(proto.materialized_feature_view_args, "stream_compaction_tile_size")
 
-    return time_utils.timedelta_to_proto(timedelta(hours=1))
+    return utils.get_field_or_none(proto.materialized_feature_view_args, "aggregation_interval")
 
 
 @typechecked
 def get_is_continuous_from_feature_view_args(
     proto: feature_view__args_pb2.FeatureViewArgs,
 ) -> bool:
     data_source_type = utils.get_field_or_none(proto.materialized_feature_view_args, "data_source_type")
```

### Comparing `tecton-0.9.0rc1/tecton_core/specs/tecton_object_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/time_window_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/time_window_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/transformation_spec.py` & `tecton-0.9.0rc2/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/specs/utils.py` & `tecton-0.9.0rc2/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/time_utils.py` & `tecton-0.9.0rc2/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/queue.py` & `tecton-0.9.0rc2/tecton_core/vendor/queue.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/treelib/__init__.py` & `tecton-0.9.0rc2/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.9.0rc2/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/treelib/misc.py` & `tecton-0.9.0rc2/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/treelib/node.py` & `tecton-0.9.0rc2/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/treelib/plugins.py` & `tecton-0.9.0rc2/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/treelib/tree.py` & `tecton-0.9.0rc2/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_core/vendor/vendor_treelib.py` & `tecton-0.9.0rc2/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/__init__.py` & `tecton-0.9.0rc2/tecton_materialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/batch_materialization.py` & `tecton-0.9.0rc2/tecton_materialization/batch_materialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,18 +120,18 @@
 ) -> DataFrame:
     df = df_to_online_store_msg(
         df,
         fd.id,
         is_batch=True,
         is_status=False,
         canary_id=None,
-        is_compaction_job=fd.compaction_enabled_for_materialization,
+        is_compaction_job=fd.batch_compaction_enabled,
     )
     udf_name = f"to_dynamodb_json_{fd.id}"
-    if fd.compaction_enabled_for_materialization:
+    if fd.batch_compaction_enabled:
         # UDF used for compaction jobs. Compatible with TableFormatVersionV3
         spark._jvm.com.tecton.onlinestorewriter.RegisterFeatureToDynamoDbJsonUDFV2().register(
             udf_name, materialization_task_params.SerializeToString()
         )
         udf_column_name = "dynamodb_json"
         df = df.select(expr(f"{udf_name}(value) as {udf_column_name}"))
         return df.select(explode(udf_column_name))
@@ -478,15 +478,15 @@
                 write_checkpoint(spark, materialization_task_params, query_feature_start_time, run_id)
 
         logger.info(f"Wrote {total_rows} total rows")
 
     if write_to_online_from_offline_store and step in (None, 2):
         assert not materialization_task_params.HasField("canary_id")
         # we don't do metrics collection here, because they already got collected in the jobs writing to the offline store
-        if fd.compaction_enabled_for_materialization:
+        if fd.batch_compaction_enabled:
             plan = materialization_plan.get_batch_compaction_online_materialization_plan(
                 spark=spark, feature_definition=fd, compaction_job_end_time=task_feature_end_time
             )
         else:
             # used for bootstrap bulk backfill jobs
             plan = MaterializationPlan.from_offline_store(fd, task_feature_start_time, task_feature_end_time, spark)
         if plan is not None:
```

### Comparing `tecton-0.9.0rc1/tecton_materialization/common/job_metadata.py` & `tecton-0.9.0rc2/tecton_materialization/common/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/common/job_metadata_aws.py` & `tecton-0.9.0rc2/tecton_materialization/common/job_metadata_aws.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/common/job_metadata_gcp.py` & `tecton-0.9.0rc2/tecton_materialization/common/job_metadata_gcp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/common/task_params.py` & `tecton-0.9.0rc2/tecton_materialization/common/task_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/consumption.py` & `tecton-0.9.0rc2/tecton_materialization/consumption.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/delta_maintenance.py` & `tecton-0.9.0rc2/tecton_materialization/delta_maintenance.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/entity_deletion.py` & `tecton-0.9.0rc2/tecton_materialization/entity_deletion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/feature_export.py` & `tecton-0.9.0rc2/tecton_materialization/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/ingest_materialization.py` & `tecton-0.9.0rc2/tecton_materialization/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/job_metadata.py` & `tecton-0.9.0rc2/tecton_materialization/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/materialization.py` & `tecton-0.9.0rc2/tecton_materialization/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/materialization_utils.py` & `tecton-0.9.0rc2/tecton_materialization/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/batch_materialization.py` & `tecton-0.9.0rc2/tecton_materialization/ray/batch_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/delta.py` & `tecton-0.9.0rc2/tecton_materialization/ray/delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 
 from tecton_core import offline_store
 from tecton_core.arrow import PARQUET_WRITE_OPTIONS
 from tecton_core.compute_mode import ComputeMode
 from tecton_core.duckdb_context import DuckDBContext
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
 from tecton_core.offline_store import BotoOfflineStoreOptionsProvider
+from tecton_core.offline_store import patch_timestamps_in_arrow_schema
 from tecton_core.query.dialect import Dialect
 from tecton_core.query.nodes import AddAnchorTimeNode
+from tecton_core.query.nodes import ConvertTimestampToUTCNode
 from tecton_core.query.nodes import StagedTableScanNode
 from tecton_materialization.common.task_params import TimeInterval
 from tecton_materialization.ray.nodes import AddTimePartitionNode
 from tecton_materialization.ray.nodes import TimeSpec
 from tecton_proto.common import data_type_pb2
 from tecton_proto.common import schema_pb2
 from tecton_proto.common.aws_credentials_pb2 import AwsIamRole
@@ -128,15 +130,15 @@
     if column.offline_data_type.type == data_type_pb2.DataTypeEnum.DATA_TYPE_INT64:
         assert_type(pyarrow.int64())
         lit = transaction_writer_pb2.Expression.Literal(int64=pa_value.as_py())
     elif column.offline_data_type.type == data_type_pb2.DataTypeEnum.DATA_TYPE_STRING:
         assert_type(pyarrow.string())
         lit = transaction_writer_pb2.Expression.Literal(str=pa_value.as_py())
     elif column.offline_data_type.type == data_type_pb2.DataTypeEnum.DATA_TYPE_TIMESTAMP:
-        assert_type(pyarrow.timestamp("us"))
+        assert_type(pyarrow.timestamp("us", "UTC"))
         lit = transaction_writer_pb2.Expression.Literal()
         lit.timestamp.FromDatetime(pa_value.as_py())
     else:
         msg = f"Unsupported type {column.offline_data_type.type} in column {column.name}"
         raise Exception(msg)
     return transaction_writer_pb2.Expression(literal=lit)
 
@@ -243,19 +245,24 @@
 
         tree = AddTimePartitionNode(
             dialect=Dialect.DUCKDB,
             compute_mode=ComputeMode.RIFT,
             input_node=AddAnchorTimeNode(
                 dialect=Dialect.DUCKDB,
                 compute_mode=ComputeMode.RIFT,
-                input_node=StagedTableScanNode(
+                input_node=ConvertTimestampToUTCNode(
                     dialect=Dialect.DUCKDB,
                     compute_mode=ComputeMode.RIFT,
-                    staged_columns=(timestamp_key,),
-                    staging_table_name="timestamp_table",
+                    input_node=StagedTableScanNode(
+                        dialect=Dialect.DUCKDB,
+                        compute_mode=ComputeMode.RIFT,
+                        staged_columns=(timestamp_key,),
+                        staging_table_name="timestamp_table",
+                    ).as_ref(),
+                    timestamp_key=timestamp_key,
                 ).as_ref(),
                 feature_store_format_version=self._feature_params.feature_store_format_version,
                 batch_schedule=self._feature_params.batch_schedule,
                 timestamp_field=timestamp_key,
             ).as_ref(),
             time_spec=self._feature_params.time_spec,
         ).as_ref()
@@ -304,25 +311,27 @@
         :param interval: The feature data time interval to delete
         """
         time_spec = self._feature_params.time_spec
         conn = DuckDBContext.get_instance().get_connection()
 
         def table_filter(input_table: pyarrow.dataset.Dataset) -> pyarrow.Table:
             time_limit_table = self._time_limits(interval)
+            # Add timezone to timestamps
+            input_table = input_table.cast(patch_timestamps_in_arrow_schema(input_table.schema))
             # Not using pypika because it lacks support for ANTI JOIN
             return conn.sql(
                 f"""
                 WITH flattened_limits AS(
                     SELECT MIN("{time_spec.time_column}") AS start, MAX("{time_spec.time_column}") AS end
                     FROM time_limit_table
                 )
                 SELECT * FROM input_table
                 LEFT JOIN flattened_limits
-                ON CAST(input_table."{time_spec.time_column}" as TIMESTAMP) >= flattened_limits.start
-                AND CAST(input_table."{time_spec.time_column}" as TIMESTAMP) < flattened_limits.end
+                ON input_table."{time_spec.time_column}" >= flattened_limits.start
+                AND input_table."{time_spec.time_column}" < flattened_limits.end
                 WHERE flattened_limits.start IS NULL
             """
             ).arrow()
 
         predicate = self._time_limit_predicate(interval)
         self._filter_files(predicate, table_filter)
```

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/feature_export.py` & `tecton-0.9.0rc2/tecton_materialization/ray/feature_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from datetime import timedelta
 from typing import Tuple
 
 import pendulum
-from google.protobuf import timestamp_pb2
 
 from tecton_core import query_consts
 from tecton_core.compute_mode import ComputeMode
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
 from tecton_core.query.builder import build_aggregated_time_range_validity_query
 from tecton_core.query.builder import build_temporal_time_range_validity_query
 from tecton_core.query.dialect import Dialect
@@ -96,19 +95,15 @@
         dialect=Dialect.DUCKDB,
         compute_mode=ComputeMode.RIFT,
         input_node=qt,
         time_spec=feature_export_time_spec(),
     ).as_ref()
 
     # return the interval we queried
-    start_interval = timestamp_pb2.Timestamp()
-    start_interval.FromDatetime(effective_start_time)
-    end_interval = timestamp_pb2.Timestamp()
-    end_interval.FromDatetime(effective_end_time)
-    interval = TimeInterval(start_interval, end_interval)
+    interval = TimeInterval(effective_start_time, effective_end_time)
 
     return qt, interval
 
 
 def get_feature_export_store_params(fd: FeatureDefinitionWrapper) -> OfflineStoreParams:
     schema = compute_features_schema_from_feature_definition(fd)
     to_remove = [col for col in schema.columns if col.name in (fd.timestamp_key, query_consts.anchor_time())]
```

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/ingest_materialization.py` & `tecton-0.9.0rc2/tecton_materialization/ray/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/job_status.py` & `tecton-0.9.0rc2/tecton_materialization/ray/job_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import logging
+import traceback
 import typing
 from datetime import datetime
 from typing import Optional
 
 from tecton_core.query.executor_utils import QueryTreeMonitor
 from tecton_materialization.common.job_metadata import JobMetadataClient
 from tecton_proto.materialization.job_metadata_pb2 import JobMetadata
@@ -37,30 +38,33 @@
     def create_stage(self, stage_type: TectonManagedStage.StageType, description: str) -> int:
         """
         Returns created stage index
         """
         self._started = True
 
         def _update(job_metadata: JobMetadata) -> Optional[JobMetadata]:
-            if any(s.stage_type == stage_type for s in job_metadata.tecton_managed_info.stages):
+            if any(
+                s.stage_type == stage_type and s.description == description
+                for s in job_metadata.tecton_managed_info.stages
+            ):
                 return None
             new_proto = JobMetadata()
             new_proto.CopyFrom(job_metadata)
 
             new_stage = TectonManagedStage(
                 description=description,
                 stage_type=stage_type,
                 state=TectonManagedStage.State.PENDING,
             )
             new_proto.tecton_managed_info.stages.append(new_stage)
             return new_proto
 
         metadata = self._metadata_client.update(_update)
         for i, stage in enumerate(metadata.tecton_managed_info.stages):
-            if stage.stage_type == stage_type:
+            if stage.stage_type == stage_type and stage.description == description:
                 return i
         msg = f"Stage {stage_type} does not exist"
         raise ValueError(msg)
 
     def set_query(self, stage_idx, sql: str):
         def _update(job_metadata: JobMetadata) -> JobMetadata:
             new_proto = JobMetadata()
@@ -107,40 +111,40 @@
             stage = new_proto.tecton_managed_info.stages[stage_idx]
             stage.state = TectonManagedStage.State.SUCCESS
 
             return new_proto
 
         self._metadata_client.update(_update)
 
-    def set_failed(self, stage_idx: int, exc: Exception, user_error: bool):
+    def set_failed(self, stage_idx: int, user_error: bool):
         def _update(job_metadata: JobMetadata) -> JobMetadata:
             new_proto = JobMetadata()
             new_proto.CopyFrom(job_metadata)
 
             stage = new_proto.tecton_managed_info.stages[stage_idx]
             stage.error_type = (
                 TectonManagedStage.ErrorType.USER_ERROR if user_error else TectonManagedStage.ErrorType.UNEXPECTED_ERROR
             )
-            stage.error_detail = str(exc)
+            stage.error_detail = traceback.format_exc()
             stage.state = TectonManagedStage.State.ERROR
 
             return new_proto
 
         self._metadata_client.update(_update)
 
-    def set_current_stage_failed(self, error_type: TectonManagedStage.ErrorType, error_detail: str):
+    def set_current_stage_failed(self, error_type: TectonManagedStage.ErrorType):
         def _update(job_metadata: JobMetadata) -> JobMetadata:
             new_proto = JobMetadata()
             new_proto.CopyFrom(job_metadata)
 
+            if any(s.state == TectonManagedStage.State.ERROR for s in new_proto.tecton_managed_info.stages):
+                return new_proto
+
             current_stage = None
             for stage in new_proto.tecton_managed_info.stages:
-                if stage.state == TectonManagedStage.State.ERROR:
-                    return new_proto
-
                 # Select first RUNNING or PENDING stage
                 # Or if all stages are complete - just the last one
                 current_stage = stage
                 if stage.state in (TectonManagedStage.State.RUNNING, TectonManagedStage.State.PENDING):
                     break
 
             if not current_stage:
@@ -148,15 +152,15 @@
                 current_stage = TectonManagedStage(
                     description="Setting up materialization job",
                     state=TectonManagedStage.State.ERROR,
                 )
                 new_proto.tecton_managed_info.stages.append(current_stage)
 
             current_stage.error_type = error_type
-            current_stage.error_detail = error_detail
+            current_stage.error_detail = traceback.format_exc()
             current_stage.state = TectonManagedStage.State.ERROR
 
             return new_proto
 
         self._metadata_client.update(_update)
 
     def create_stage_monitor(
@@ -171,15 +175,15 @@
             if sql:
                 self.set_query(stage_idx, sql)
 
             self.update_progress(stage_idx, 0)
 
             try:
                 yield lambda p: self.update_progress(stage_idx, p)
-            except Exception as err:
-                self.set_failed(stage_idx, err, user_error=False)
+            except Exception:
+                self.set_failed(stage_idx, user_error=False)
                 raise
             else:
                 self.update_progress(stage_idx, 1)
                 self.set_completed(stage_idx)
 
         return monitor
```

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/materialization.py` & `tecton-0.9.0rc2/tecton_materialization/ray/materialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import contextlib
 import os
-import traceback
 from typing import Optional
 
 import pyarrow.fs
 import ray
 
 from tecton_core import conf
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
@@ -147,18 +146,15 @@
     conf.set("TECTON_RUNTIME_MODE", "MATERIALIZATION")
     assert materialization_task_params.feature_view.schemas.HasField("materialization_schema"), "missing schema"
     job_status_client = JobStatusClient(JobMetadataClient.for_params(materialization_task_params))
     try:
         with _ray():
             run_ray_job(materialization_task_params, job_status_client)
     except Exception:
-        job_status_client.set_current_stage_failed(
-            TectonManagedStage.ErrorType.UNEXPECTED_ERROR,
-            traceback.format_exc(),
-        )
+        job_status_client.set_current_stage_failed(TectonManagedStage.ErrorType.UNEXPECTED_ERROR)
         raise
 
 
 def run_ray_job(materialization_task_params: MaterializationTaskParams, job_status_client: JobStatusClient) -> None:
     fd = feature_definition_from_task_params(materialization_task_params)
     secret_resolver = _get_secret_resolver(materialization_task_params)
     task_type = _get_task_type(materialization_task_params)
```

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/materialization_utils.py` & `tecton-0.9.0rc2/tecton_materialization/ray/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/ray/nodes.py` & `tecton-0.9.0rc2/tecton_materialization/ray/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/remote_host/pyspark_remote_host.py` & `tecton-0.9.0rc2/tecton_materialization/remote_host/pyspark_remote_host.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/secrets.py` & `tecton-0.9.0rc2/tecton_materialization/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_materialization/stream_materialization.py` & `tecton-0.9.0rc2/tecton_materialization/stream_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.9.0rc2/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.9.0rc2/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.9.0rc2/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/basic_info_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/data_source_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/diff_options_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/diff_test_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/entity_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/fco_args_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/feature_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/feature_view_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/feature_view_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from tecton_proto.common import framework_version_pb2 as tecton__proto_dot_common_dot_framework__version__pb2
 from tecton_proto.common import id_pb2 as tecton__proto_dot_common_dot_id__pb2
 from tecton_proto.common import schema_pb2 as tecton__proto_dot_common_dot_schema__pb2
 from tecton_proto.common import spark_schema_pb2 as tecton__proto_dot_common_dot_spark__schema__pb2
 from tecton_proto.common import time_window_pb2 as tecton__proto_dot_common_dot_time__window__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/feature_view.proto\x12\x11tecton_proto.args\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"tecton_proto/args/basic_info.proto\x1a#tecton_proto/args/data_source.proto\x1a$tecton_proto/args/diff_options.proto\x1a tecton_proto/args/pipeline.proto\x1a+tecton_proto/args/version_constraints.proto\x1a+tecton_proto/common/analytics_options.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a&tecton_proto/common/spark_schema.proto\x1a%tecton_proto/common/time_window.proto\"\xfd\r\n\x0f\x46\x65\x61tureViewArgs\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12N\n\x11\x66\x65\x61ture_view_type\x18\x02 \x01(\x0e\x32\".tecton_proto.args.FeatureViewTypeR\x0f\x66\x65\x61tureViewType\x12\x37\n\x04info\x18\x03 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x1d \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18  \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12P\n\x07options\x18\" \x03(\x0b\x32/.tecton_proto.args.FeatureViewArgs.OptionsEntryB\x05\x92M\x02\x08\x01R\x07options\x12H\n\x0c\x63\x61\x63he_config\x18$ \x01(\x0b\x32\x1e.tecton_proto.args.CacheConfigB\x05\x92M\x02\x08\x01R\x0b\x63\x61\x63heConfig\x12G\n\x08\x65ntities\x18\x04 \x03(\x0b\x32$.tecton_proto.args.EntityKeyOverrideB\x05\x92M\x02\x08\x06R\x08\x65ntities\x12M\n\rtemporal_args\x18\x17 \x01(\x0b\x32\x1f.tecton_proto.args.TemporalArgsB\x05\x92M\x02\x10\x01H\x00R\x0ctemporalArgs\x12i\n\x17temporal_aggregate_args\x18\x18 \x01(\x0b\x32(.tecton_proto.args.TemporalAggregateArgsB\x05\x92M\x02\x10\x01H\x00R\x15temporalAggregateArgs\x12|\n\x1ematerialized_feature_view_args\x18\x1c \x01(\x0b\x32..tecton_proto.args.MaterializedFeatureViewArgsB\x05\x92M\x02\x10\x01H\x00R\x1bmaterializedFeatureViewArgs\x12N\n\x0eon_demand_args\x18\x19 \x01(\x0b\x32\x1f.tecton_proto.args.OnDemandArgsB\x05\x92M\x02\x10\x01H\x00R\x0conDemandArgs\x12Z\n\x12\x66\x65\x61ture_table_args\x18\x1a \x01(\x0b\x32#.tecton_proto.args.FeatureTableArgsB\x05\x92M\x02\x10\x01H\x00R\x10\x66\x65\x61tureTableArgs\x12\x30\n\x14online_serving_index\x18\x05 \x03(\tR\x12onlineServingIndex\x12,\n\x0eonline_enabled\x18\x0e \x01(\x08\x42\x05\x92M\x02 \x0bR\ronlineEnabled\x12.\n\x0foffline_enabled\x18\x0f \x01(\x08\x42\x05\x92M\x02 \x0bR\x0eofflineEnabled\x12Z\n\x12\x62\x61tch_compute_mode\x18# \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeB\x05\x92M\x02\x08\tR\x10\x62\x61tchComputeMode\x12>\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineB\x05\x92M\x02\x08\x06R\x08pipeline\x12`\n\x13\x64\x61ta_quality_config\x18! \x01(\x0b\x32$.tecton_proto.args.DataQualityConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\x11\x64\x61taQualityConfig\x12N\n\x12\x66orced_view_schema\x18\x1e \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x10\x66orcedViewSchema\x12^\n\x1a\x66orced_materialized_schema\x18\x1f \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x18\x66orcedMaterializedSchema\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0b\n\ttype_argsJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08\x16\x10\x17J\x04\x08\x1b\x10\x1c\"f\n\x11\x45ntityKeyOverride\x12\x34\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08\x65ntityId\x12\x1b\n\tjoin_keys\x18\x02 \x03(\tR\x08joinKeys\"K\n\x0e\x42\x61\x63kfillConfig\x12\x39\n\x04mode\x18\x01 \x01(\x0e\x32%.tecton_proto.args.BackfillConfigModeR\x04mode\"\xce\x01\n\x0cOutputStream\x12)\n\x10include_features\x18\x01 \x01(\x08R\x0fincludeFeatures\x12\x44\n\x07kinesis\x18\x02 \x01(\x0b\x32(.tecton_proto.args.KinesisDataSourceArgsH\x00R\x07kinesis\x12>\n\x05kafka\x18\x03 \x01(\x0b\x32&.tecton_proto.args.KafkaDataSourceArgsH\x00R\x05kafkaB\r\n\x0bstream_sink\"\xb9\x08\n\x0cTemporalArgs\x12#\n\rtimestamp_key\x18\x01 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12S\n\x0eoffline_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12Q\n\x0f\x62\x61\x63kfill_config\x18\x0b \x01(\x0b\x32!.tecton_proto.args.BackfillConfigB\x05\x92M\x02\x08\x03R\x0e\x62\x61\x63kfillConfig\x12T\n\x13online_store_config\x18\x0c \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x33\n\x15incremental_backfills\x18\r \x01(\x08R\x14incrementalBackfills\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xe9\x08\n\x15TemporalAggregateArgs\x12k\n!aggregation_slide_period_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x05R\x1e\x61ggregationSlidePeriodDuration\x12\x38\n\x18\x61ggregation_slide_period\x18\x02 \x01(\tR\x16\x61ggregationSlidePeriod\x12I\n\x0c\x61ggregations\x18\x03 \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12#\n\rtimestamp_key\x18\x04 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x07 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12S\n\x0eoffline_config\x18\x08 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\n \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\x0b \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\x0c \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12T\n\x13online_store_config\x18\r \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xa5\x11\n\x1bMaterializedFeatureViewArgs\x12\'\n\x0ftimestamp_field\x18\x01 \x01(\tR\x0etimestampField\x12G\n\x0e\x62\x61tch_schedule\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02 \x08R\rbatchSchedule\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12i\n manual_trigger_backfill_end_time\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x1cmanualTriggerBackfillEndTime\x12\x85\x01\n\x15max_backfill_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB6\x92M\"* \n\x1emax_batch_aggregation_interval\x92M\t*\x07\x12\x05\x30.7.0\x92M\x02\x08\x01R\x13maxBackfillInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12\x85\x01\n\x14offline_store_legacy\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB%\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x19 \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12\x45\n\rbatch_compute\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x0c\x62\x61tchCompute\x12G\n\x0estream_compute\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\rstreamCompute\x12O\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12G\n\x0conline_store\x18\x0b \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x0bonlineStore\x12\x33\n\x15incremental_backfills\x18\x0c \x01(\x08R\x14incrementalBackfills\x12L\n\x14\x61ggregation_interval\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x13\x61ggregationInterval\x12\x64\n\x16stream_processing_mode\x18\x0f \x01(\x0e\x32\'.tecton_proto.args.StreamProcessingModeB\x05\x92M\x02 \x06R\x14streamProcessingMode\x12I\n\x0c\x61ggregations\x18\x0e \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12\x44\n\routput_stream\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12O\n\rbatch_trigger\x18\x11 \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeB\x05\x92M\x02\x08\x01R\x0c\x62\x61tchTrigger\x12:\n\x06schema\x18\x12 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaB\x05\x92M\x02\x08\x06R\x06schema\x12:\n\x19\x61ggregation_secondary_key\x18\x14 \x01(\tR\x17\x61ggregationSecondaryKey\x12s\n\x1csecondary_key_output_columns\x18\x15 \x03(\x0b\x32+.tecton_proto.args.SecondaryKeyOutputColumnB\x05\x92M\x02\x18\x05R\x19secondaryKeyOutputColumns\x12I\n\x1drun_transformation_validation\x18\x16 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x1brunTransformationValidation\x12K\n\x1etecton_materialization_runtime\x18\x17 \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\x12J\n\x13lifetime_start_time\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11lifetimeStartTime\x12\x38\n\x18\x62\x61tch_compaction_enabled\x18\x1a \x01(\x08R\x16\x62\x61tchCompactionEnabled\x12:\n\x19stream_compaction_enabled\x18\x1c \x01(\x08R\x17streamCompactionEnabled\x12\'\n\x0b\x65nvironment\x18\x1b \x01(\tB\x05\x92M\x02\x08\x01R\x0b\x65nvironment\"\xd3\x01\n\x0cOnDemandArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x02 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12.\n\x0c\x65nvironments\x18\x04 \x03(\tB\n\x92M\x02\x08\x01\x82}\x02\x08\x05R\x0c\x65nvironmentsJ\x04\x08\x03\x10\x04\"\x97\x08\n\x10\x46\x65\x61tureTableArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12\x41\n\x0bserving_ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Z\n\x0eoffline_config\x18\x03 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x10\x03R\rofflineConfig\x12\x8a\x01\n\x14offline_store_legacy\x18\x07 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB*\x82}\x02\x08\x05\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x0c \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12[\n\x13online_store_config\x18\x04 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x10\x03R\x11onlineStoreConfig\x12N\n\x0conline_store\x18\x08 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x08\x05R\x0bonlineStore\x12\\\n\x15\x62\x61tch_materialization\x18\x05 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x10\x03R\x14\x62\x61tchMaterialization\x12L\n\rbatch_compute\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x08\x05R\x0c\x62\x61tchCompute\x12O\n\nmonitoring\x18\n \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12K\n\x1etecton_materialization_runtime\x18\x0b \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\"\x94\x06\n\x12\x46\x65\x61tureAggregation\x12\x16\n\x06\x63olumn\x18\x01 \x01(\tR\x06\x63olumn\x12\x1a\n\x08\x66unction\x18\x02 \x01(\tR\x08\x66unction\x12\x62\n\x0f\x66unction_params\x18\x05 \x03(\x0b\x32\x39.tecton_proto.args.FeatureAggregation.FunctionParamsEntryR\x0e\x66unctionParams\x12\x43\n\x0ctime_windows\x18\x03 \x03(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x0btimeWindows\x12\x34\n\x10time_window_strs\x18\x04 \x03(\tB\n\x82}\x02\x10\x03\x92M\x02\x08\x05R\x0etimeWindowStrs\x12q\n\x12time_window_legacy\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB(\x92M\x0f*\r\n\x0btime_window\x92M\t*\x07\x12\x05\x30.8.0\x82}\x02\x08\x05\x92M\x02 \tR\x10timeWindowLegacy\x12\x1e\n\x04name\x18\x07 \x01(\tB\n\x82}\x02\x08\x05\x92M\x02 \x01R\x04name\x12G\n\x0btime_window\x18\x08 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowB\x05\x92M\x02 \nH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\t \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\n \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x1a`\n\x13\x46unctionParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.args.ParamValueR\x05value:\x02\x38\x01\x42\x08\n\x06window\"]\n\nParamValue\x12!\n\x0bint64_value\x18\x01 \x01(\x03H\x00R\nint64Value\x12#\n\x0c\x64ouble_value\x18\x02 \x01(\x01H\x00R\x0b\x64oubleValueB\x07\n\x05value\"\x8f\x01\n\x11\x44\x61taQualityConfig\x12\x37\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08\x42\x05\x92M\x02 \x03R\x12\x64\x61taQualityEnabled\x12\x41\n\x19skip_default_expectations\x18\x02 \x01(\x08\x42\x05\x92M\x02 \x03R\x17skipDefaultExpectations\"\xac\x05\n\rClusterConfig\x12\\\n\x10\x65xisting_cluster\x18\x01 \x01(\x0b\x32(.tecton_proto.args.ExistingClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0f\x65xistingCluster\x12S\n\x0enew_databricks\x18\x02 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\rnewDatabricks\x12\x45\n\x07new_emr\x18\x03 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x06newEmr\x12^\n\x0fimplicit_config\x18\x04 \x01(\x0b\x32\'.tecton_proto.args.DefaultClusterConfigB\n\x92M\x02\x08\x01\x92M\x02\x18\x05H\x00R\x0eimplicitConfig\x12V\n\x0fjson_databricks\x18\x05 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0ejsonDatabricks\x12H\n\x08json_emr\x18\x06 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x07jsonEmr\x12R\n\rjson_dataproc\x18\x07 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0cjsonDataproc\x12\x41\n\x04rift\x18\x08 \x01(\x0b\x32$.tecton_proto.args.RiftClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x04riftB\x08\n\x06\x63onfig\"@\n\x11JsonClusterConfig\x12+\n\x04json\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x04json\"G\n\x15\x45xistingClusterConfig\x12.\n\x13\x65xisting_cluster_id\x18\x01 \x01(\tR\x11\x65xistingClusterId\"\x9f\x03\n\x10NewClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\x12\x33\n\x15instance_availability\x18\x06 \x01(\tR\x14instanceAvailability\x12*\n\x11number_of_workers\x18\x02 \x01(\x05R\x0fnumberOfWorkers\x12\x32\n\x16root_volume_size_in_gb\x18\x03 \x01(\x05R\x12rootVolumeSizeInGb\x12\x34\n\x16\x65xtra_pip_dependencies\x18\x04 \x03(\tR\x14\x65xtraPipDependencies\x12\x41\n\x0cspark_config\x18\x05 \x01(\x0b\x32\x1e.tecton_proto.args.SparkConfigR\x0bsparkConfig\x12&\n\x0f\x66irst_on_demand\x18\x07 \x01(\x05R\rfirstOnDemand\x12\x30\n\x14pinned_spark_version\x18\x08 \x01(\tR\x12pinnedSparkVersion\"8\n\x11RiftClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\"\xbd\x01\n\x14\x44\x65\x66\x61ultClusterConfig\x12\x38\n\x18\x64\x61tabricks_spark_version\x18\x01 \x01(\tR\x16\x64\x61tabricksSparkVersion\x12*\n\x11\x65mr_spark_version\x18\x02 \x01(\tR\x0f\x65mrSparkVersion\x12?\n\x1ctecton_compute_instance_type\x18\x03 \x01(\tR\x19tectonComputeInstanceType\"\x83\x03\n\x0bSparkConfig\x12.\n\x13spark_driver_memory\x18\x01 \x01(\tR\x11sparkDriverMemory\x12\x32\n\x15spark_executor_memory\x18\x02 \x01(\tR\x13sparkExecutorMemory\x12?\n\x1cspark_driver_memory_overhead\x18\x03 \x01(\tR\x19sparkDriverMemoryOverhead\x12\x43\n\x1espark_executor_memory_overhead\x18\x04 \x01(\tR\x1bsparkExecutorMemoryOverhead\x12L\n\nspark_conf\x18\x05 \x03(\x0b\x32-.tecton_proto.args.SparkConfig.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xe6\x01\n\x11OnlineStoreConfig\x12@\n\x06\x64ynamo\x18\x01 \x01(\x0b\x32&.tecton_proto.args.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x02 \x01(\x0b\x32#.tecton_proto.args.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x03 \x01(\x0b\x32&.tecton_proto.args.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"G\n\x13\x44ynamoDbOnlineStore\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\xc8\x01\n\x10RedisOnlineStore\x12\x30\n\x10primary_endpoint\x18\x02 \x01(\tB\x05\x92M\x02\x08\x06R\x0fprimaryEndpoint\x12=\n\x14\x61uthentication_token\x18\x04 \x01(\tB\n\x92M\x02\x08\x01\x92M\x02\x18\x06R\x13\x61uthenticationToken\x12\x1f\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x05\x92M\x02\x18\x05R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\xdb\x01\n\x19OfflineFeatureStoreConfig\x12<\n\x07parquet\x18\x01 \x01(\x0b\x32 .tecton_proto.args.ParquetConfigH\x00R\x07parquet\x12\x36\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.args.DeltaConfigH\x00R\x05\x64\x65lta\x12:\n\x15subdirectory_override\x18\x03 \x01(\tB\x05\x92M\x02\x08\x01R\x14subdirectoryOverrideB\x0c\n\nstore_type\"\x0f\n\rParquetConfig\"X\n\x0b\x44\x65ltaConfig\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\"\x80\x02\n\x12OfflineStoreConfig\x12^\n\x14staging_table_format\x18\x01 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12stagingTableFormat\x12\x39\n\x15publish_full_features\x18\x02 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x13publishFullFeatures\x12O\n\x12publish_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10publishStartTime\"\x99\x02\n\x10MonitoringConfig\x12+\n\x11monitor_freshness\x18\x01 \x01(\x08R\x10monitorFreshness\x12^\n\x1a\x65xpected_feature_freshness\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x18\x65xpectedFeatureFreshness\x12O\n\x12\x65xpected_freshness\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\x11\x65xpectedFreshness\x12\'\n\x0b\x61lert_email\x18\x03 \x01(\tB\x06\xf2\xe2\x02\x02\x08\x01R\nalertEmail\"\x9f\x02\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\x03 \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\x04 \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x12\x12\n\x04name\x18\x02 \x01(\tR\x04nameB\x08\n\x06window\"\x83\x01\n\nTimeWindow\x12\x42\n\x0fwindow_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\x12\x31\n\x06offset\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06offset\"\x86\x02\n\x10TimeWindowSeries\x12<\n\x0cseries_start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bseriesStart\x12\x38\n\nseries_end\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\tseriesEnd\x12\x36\n\tstep_size\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08stepSize\x12\x42\n\x0fwindow_duration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\"5\n\x0b\x43\x61\x63heConfig\x12&\n\x0fmax_age_seconds\x18\x01 \x01(\x03R\rmaxAgeSeconds*\xed\x01\n\x0f\x46\x65\x61tureViewType\x12!\n\x1d\x46\x45\x41TURE_VIEW_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_VIEW_TYPE_TEMPORAL\x10\x01\x12(\n$FEATURE_VIEW_TYPE_TEMPORAL_AGGREGATE\x10\x02\x12\x1f\n\x1b\x46\x45\x41TURE_VIEW_TYPE_ON_DEMAND\x10\x03\x12#\n\x1f\x46\x45\x41TURE_VIEW_TYPE_FEATURE_TABLE\x10\x04\x12\'\n#FEATURE_VIEW_TYPE_FWV5_FEATURE_VIEW\x10\x05*\xbf\x01\n\x12\x42\x61\x63kfillConfigMode\x12$\n BACKFILL_CONFIG_MODE_UNSPECIFIED\x10\x00\x12?\n;BACKFILL_CONFIG_MODE_SINGLE_BATCH_SCHEDULE_INTERVAL_PER_JOB\x10\x01\x12\x42\n>BACKFILL_CONFIG_MODE_MULTIPLE_BATCH_SCHEDULE_INTERVALS_PER_JOB\x10\x02*\x8f\x01\n\x14StreamProcessingMode\x12&\n\"STREAM_PROCESSING_MODE_UNSPECIFIED\x10\x00\x12(\n$STREAM_PROCESSING_MODE_TIME_INTERVAL\x10\x01\x12%\n!STREAM_PROCESSING_MODE_CONTINUOUS\x10\x02*\xa8\x01\n\x10\x42\x61tchTriggerType\x12\"\n\x1e\x42\x41TCH_TRIGGER_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1c\x42\x41TCH_TRIGGER_TYPE_SCHEDULED\x10\x01\x12\x1d\n\x19\x42\x41TCH_TRIGGER_TYPE_MANUAL\x10\x02\x12/\n+BATCH_TRIGGER_TYPE_NO_BATCH_MATERIALIZATION\x10\x03\x42\x13\n\x0f\x63om.tecton.argsP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/feature_view.proto\x12\x11tecton_proto.args\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"tecton_proto/args/basic_info.proto\x1a#tecton_proto/args/data_source.proto\x1a$tecton_proto/args/diff_options.proto\x1a tecton_proto/args/pipeline.proto\x1a+tecton_proto/args/version_constraints.proto\x1a+tecton_proto/common/analytics_options.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a&tecton_proto/common/spark_schema.proto\x1a%tecton_proto/common/time_window.proto\"\xfd\r\n\x0f\x46\x65\x61tureViewArgs\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12N\n\x11\x66\x65\x61ture_view_type\x18\x02 \x01(\x0e\x32\".tecton_proto.args.FeatureViewTypeR\x0f\x66\x65\x61tureViewType\x12\x37\n\x04info\x18\x03 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x1d \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18  \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12P\n\x07options\x18\" \x03(\x0b\x32/.tecton_proto.args.FeatureViewArgs.OptionsEntryB\x05\x92M\x02\x08\x01R\x07options\x12H\n\x0c\x63\x61\x63he_config\x18$ \x01(\x0b\x32\x1e.tecton_proto.args.CacheConfigB\x05\x92M\x02\x08\x01R\x0b\x63\x61\x63heConfig\x12G\n\x08\x65ntities\x18\x04 \x03(\x0b\x32$.tecton_proto.args.EntityKeyOverrideB\x05\x92M\x02\x08\x06R\x08\x65ntities\x12M\n\rtemporal_args\x18\x17 \x01(\x0b\x32\x1f.tecton_proto.args.TemporalArgsB\x05\x92M\x02\x10\x01H\x00R\x0ctemporalArgs\x12i\n\x17temporal_aggregate_args\x18\x18 \x01(\x0b\x32(.tecton_proto.args.TemporalAggregateArgsB\x05\x92M\x02\x10\x01H\x00R\x15temporalAggregateArgs\x12|\n\x1ematerialized_feature_view_args\x18\x1c \x01(\x0b\x32..tecton_proto.args.MaterializedFeatureViewArgsB\x05\x92M\x02\x10\x01H\x00R\x1bmaterializedFeatureViewArgs\x12N\n\x0eon_demand_args\x18\x19 \x01(\x0b\x32\x1f.tecton_proto.args.OnDemandArgsB\x05\x92M\x02\x10\x01H\x00R\x0conDemandArgs\x12Z\n\x12\x66\x65\x61ture_table_args\x18\x1a \x01(\x0b\x32#.tecton_proto.args.FeatureTableArgsB\x05\x92M\x02\x10\x01H\x00R\x10\x66\x65\x61tureTableArgs\x12\x30\n\x14online_serving_index\x18\x05 \x03(\tR\x12onlineServingIndex\x12,\n\x0eonline_enabled\x18\x0e \x01(\x08\x42\x05\x92M\x02 \x0bR\ronlineEnabled\x12.\n\x0foffline_enabled\x18\x0f \x01(\x08\x42\x05\x92M\x02 \x0bR\x0eofflineEnabled\x12Z\n\x12\x62\x61tch_compute_mode\x18# \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeB\x05\x92M\x02\x08\tR\x10\x62\x61tchComputeMode\x12>\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineB\x05\x92M\x02\x08\x06R\x08pipeline\x12`\n\x13\x64\x61ta_quality_config\x18! \x01(\x0b\x32$.tecton_proto.args.DataQualityConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\x11\x64\x61taQualityConfig\x12N\n\x12\x66orced_view_schema\x18\x1e \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x10\x66orcedViewSchema\x12^\n\x1a\x66orced_materialized_schema\x18\x1f \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x18\x66orcedMaterializedSchema\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0b\n\ttype_argsJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08\x16\x10\x17J\x04\x08\x1b\x10\x1c\"f\n\x11\x45ntityKeyOverride\x12\x34\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08\x65ntityId\x12\x1b\n\tjoin_keys\x18\x02 \x03(\tR\x08joinKeys\"K\n\x0e\x42\x61\x63kfillConfig\x12\x39\n\x04mode\x18\x01 \x01(\x0e\x32%.tecton_proto.args.BackfillConfigModeR\x04mode\"\xce\x01\n\x0cOutputStream\x12)\n\x10include_features\x18\x01 \x01(\x08R\x0fincludeFeatures\x12\x44\n\x07kinesis\x18\x02 \x01(\x0b\x32(.tecton_proto.args.KinesisDataSourceArgsH\x00R\x07kinesis\x12>\n\x05kafka\x18\x03 \x01(\x0b\x32&.tecton_proto.args.KafkaDataSourceArgsH\x00R\x05kafkaB\r\n\x0bstream_sink\"\xb9\x08\n\x0cTemporalArgs\x12#\n\rtimestamp_key\x18\x01 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12S\n\x0eoffline_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12Q\n\x0f\x62\x61\x63kfill_config\x18\x0b \x01(\x0b\x32!.tecton_proto.args.BackfillConfigB\x05\x92M\x02\x08\x03R\x0e\x62\x61\x63kfillConfig\x12T\n\x13online_store_config\x18\x0c \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x33\n\x15incremental_backfills\x18\r \x01(\x08R\x14incrementalBackfills\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xe9\x08\n\x15TemporalAggregateArgs\x12k\n!aggregation_slide_period_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x05R\x1e\x61ggregationSlidePeriodDuration\x12\x38\n\x18\x61ggregation_slide_period\x18\x02 \x01(\tR\x16\x61ggregationSlidePeriod\x12I\n\x0c\x61ggregations\x18\x03 \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12#\n\rtimestamp_key\x18\x04 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x07 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12S\n\x0eoffline_config\x18\x08 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\n \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\x0b \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\x0c \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12T\n\x13online_store_config\x18\r \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xff\x11\n\x1bMaterializedFeatureViewArgs\x12\'\n\x0ftimestamp_field\x18\x01 \x01(\tR\x0etimestampField\x12G\n\x0e\x62\x61tch_schedule\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02 \x08R\rbatchSchedule\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12i\n manual_trigger_backfill_end_time\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x1cmanualTriggerBackfillEndTime\x12\x85\x01\n\x15max_backfill_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB6\x92M\"* \n\x1emax_batch_aggregation_interval\x92M\t*\x07\x12\x05\x30.7.0\x92M\x02\x08\x01R\x13maxBackfillInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12\x85\x01\n\x14offline_store_legacy\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB%\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x19 \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12\x45\n\rbatch_compute\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x0c\x62\x61tchCompute\x12G\n\x0estream_compute\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\rstreamCompute\x12O\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12G\n\x0conline_store\x18\x0b \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x0bonlineStore\x12\x33\n\x15incremental_backfills\x18\x0c \x01(\x08R\x14incrementalBackfills\x12L\n\x14\x61ggregation_interval\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x13\x61ggregationInterval\x12\x64\n\x16stream_processing_mode\x18\x0f \x01(\x0e\x32\'.tecton_proto.args.StreamProcessingModeB\x05\x92M\x02 \x06R\x14streamProcessingMode\x12I\n\x0c\x61ggregations\x18\x0e \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12\x44\n\routput_stream\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12O\n\rbatch_trigger\x18\x11 \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeB\x05\x92M\x02\x08\x01R\x0c\x62\x61tchTrigger\x12:\n\x06schema\x18\x12 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaB\x05\x92M\x02\x08\x06R\x06schema\x12:\n\x19\x61ggregation_secondary_key\x18\x14 \x01(\tR\x17\x61ggregationSecondaryKey\x12s\n\x1csecondary_key_output_columns\x18\x15 \x03(\x0b\x32+.tecton_proto.args.SecondaryKeyOutputColumnB\x05\x92M\x02\x18\x05R\x19secondaryKeyOutputColumns\x12I\n\x1drun_transformation_validation\x18\x16 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x1brunTransformationValidation\x12K\n\x1etecton_materialization_runtime\x18\x17 \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\x12J\n\x13lifetime_start_time\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11lifetimeStartTime\x12\x38\n\x18\x62\x61tch_compaction_enabled\x18\x1a \x01(\x08R\x16\x62\x61tchCompactionEnabled\x12:\n\x19stream_compaction_enabled\x18\x1c \x01(\x08R\x17streamCompactionEnabled\x12X\n\x1bstream_compaction_tile_size\x18\x1d \x01(\x0b\x32\x19.google.protobuf.DurationR\x18streamCompactionTileSize\x12\'\n\x0b\x65nvironment\x18\x1b \x01(\tB\x05\x92M\x02\x08\x01R\x0b\x65nvironment\"\xd3\x01\n\x0cOnDemandArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x02 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12.\n\x0c\x65nvironments\x18\x04 \x03(\tB\n\x92M\x02\x08\x01\x82}\x02\x08\x05R\x0c\x65nvironmentsJ\x04\x08\x03\x10\x04\"\x97\x08\n\x10\x46\x65\x61tureTableArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12\x41\n\x0bserving_ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Z\n\x0eoffline_config\x18\x03 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x10\x03R\rofflineConfig\x12\x8a\x01\n\x14offline_store_legacy\x18\x07 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB*\x82}\x02\x08\x05\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x0c \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12[\n\x13online_store_config\x18\x04 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x10\x03R\x11onlineStoreConfig\x12N\n\x0conline_store\x18\x08 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x08\x05R\x0bonlineStore\x12\\\n\x15\x62\x61tch_materialization\x18\x05 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x10\x03R\x14\x62\x61tchMaterialization\x12L\n\rbatch_compute\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x08\x05R\x0c\x62\x61tchCompute\x12O\n\nmonitoring\x18\n \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12K\n\x1etecton_materialization_runtime\x18\x0b \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\"\x94\x06\n\x12\x46\x65\x61tureAggregation\x12\x16\n\x06\x63olumn\x18\x01 \x01(\tR\x06\x63olumn\x12\x1a\n\x08\x66unction\x18\x02 \x01(\tR\x08\x66unction\x12\x62\n\x0f\x66unction_params\x18\x05 \x03(\x0b\x32\x39.tecton_proto.args.FeatureAggregation.FunctionParamsEntryR\x0e\x66unctionParams\x12\x43\n\x0ctime_windows\x18\x03 \x03(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x0btimeWindows\x12\x34\n\x10time_window_strs\x18\x04 \x03(\tB\n\x82}\x02\x10\x03\x92M\x02\x08\x05R\x0etimeWindowStrs\x12q\n\x12time_window_legacy\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB(\x92M\x0f*\r\n\x0btime_window\x92M\t*\x07\x12\x05\x30.8.0\x82}\x02\x08\x05\x92M\x02 \tR\x10timeWindowLegacy\x12\x1e\n\x04name\x18\x07 \x01(\tB\n\x82}\x02\x08\x05\x92M\x02 \x01R\x04name\x12G\n\x0btime_window\x18\x08 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowB\x05\x92M\x02 \nH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\t \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\n \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x1a`\n\x13\x46unctionParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.args.ParamValueR\x05value:\x02\x38\x01\x42\x08\n\x06window\"]\n\nParamValue\x12!\n\x0bint64_value\x18\x01 \x01(\x03H\x00R\nint64Value\x12#\n\x0c\x64ouble_value\x18\x02 \x01(\x01H\x00R\x0b\x64oubleValueB\x07\n\x05value\"\x8f\x01\n\x11\x44\x61taQualityConfig\x12\x37\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08\x42\x05\x92M\x02 \x03R\x12\x64\x61taQualityEnabled\x12\x41\n\x19skip_default_expectations\x18\x02 \x01(\x08\x42\x05\x92M\x02 \x03R\x17skipDefaultExpectations\"\xac\x05\n\rClusterConfig\x12\\\n\x10\x65xisting_cluster\x18\x01 \x01(\x0b\x32(.tecton_proto.args.ExistingClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0f\x65xistingCluster\x12S\n\x0enew_databricks\x18\x02 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\rnewDatabricks\x12\x45\n\x07new_emr\x18\x03 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x06newEmr\x12^\n\x0fimplicit_config\x18\x04 \x01(\x0b\x32\'.tecton_proto.args.DefaultClusterConfigB\n\x92M\x02\x08\x01\x92M\x02\x18\x05H\x00R\x0eimplicitConfig\x12V\n\x0fjson_databricks\x18\x05 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0ejsonDatabricks\x12H\n\x08json_emr\x18\x06 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x07jsonEmr\x12R\n\rjson_dataproc\x18\x07 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0cjsonDataproc\x12\x41\n\x04rift\x18\x08 \x01(\x0b\x32$.tecton_proto.args.RiftClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x04riftB\x08\n\x06\x63onfig\"@\n\x11JsonClusterConfig\x12+\n\x04json\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x04json\"G\n\x15\x45xistingClusterConfig\x12.\n\x13\x65xisting_cluster_id\x18\x01 \x01(\tR\x11\x65xistingClusterId\"\x9f\x03\n\x10NewClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\x12\x33\n\x15instance_availability\x18\x06 \x01(\tR\x14instanceAvailability\x12*\n\x11number_of_workers\x18\x02 \x01(\x05R\x0fnumberOfWorkers\x12\x32\n\x16root_volume_size_in_gb\x18\x03 \x01(\x05R\x12rootVolumeSizeInGb\x12\x34\n\x16\x65xtra_pip_dependencies\x18\x04 \x03(\tR\x14\x65xtraPipDependencies\x12\x41\n\x0cspark_config\x18\x05 \x01(\x0b\x32\x1e.tecton_proto.args.SparkConfigR\x0bsparkConfig\x12&\n\x0f\x66irst_on_demand\x18\x07 \x01(\x05R\rfirstOnDemand\x12\x30\n\x14pinned_spark_version\x18\x08 \x01(\tR\x12pinnedSparkVersion\"8\n\x11RiftClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\"\xbd\x01\n\x14\x44\x65\x66\x61ultClusterConfig\x12\x38\n\x18\x64\x61tabricks_spark_version\x18\x01 \x01(\tR\x16\x64\x61tabricksSparkVersion\x12*\n\x11\x65mr_spark_version\x18\x02 \x01(\tR\x0f\x65mrSparkVersion\x12?\n\x1ctecton_compute_instance_type\x18\x03 \x01(\tR\x19tectonComputeInstanceType\"\x83\x03\n\x0bSparkConfig\x12.\n\x13spark_driver_memory\x18\x01 \x01(\tR\x11sparkDriverMemory\x12\x32\n\x15spark_executor_memory\x18\x02 \x01(\tR\x13sparkExecutorMemory\x12?\n\x1cspark_driver_memory_overhead\x18\x03 \x01(\tR\x19sparkDriverMemoryOverhead\x12\x43\n\x1espark_executor_memory_overhead\x18\x04 \x01(\tR\x1bsparkExecutorMemoryOverhead\x12L\n\nspark_conf\x18\x05 \x03(\x0b\x32-.tecton_proto.args.SparkConfig.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xe6\x01\n\x11OnlineStoreConfig\x12@\n\x06\x64ynamo\x18\x01 \x01(\x0b\x32&.tecton_proto.args.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x02 \x01(\x0b\x32#.tecton_proto.args.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x03 \x01(\x0b\x32&.tecton_proto.args.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"G\n\x13\x44ynamoDbOnlineStore\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\xc8\x01\n\x10RedisOnlineStore\x12\x30\n\x10primary_endpoint\x18\x02 \x01(\tB\x05\x92M\x02\x08\x06R\x0fprimaryEndpoint\x12=\n\x14\x61uthentication_token\x18\x04 \x01(\tB\n\x92M\x02\x08\x01\x92M\x02\x18\x06R\x13\x61uthenticationToken\x12\x1f\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x05\x92M\x02\x18\x05R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\xdb\x01\n\x19OfflineFeatureStoreConfig\x12<\n\x07parquet\x18\x01 \x01(\x0b\x32 .tecton_proto.args.ParquetConfigH\x00R\x07parquet\x12\x36\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.args.DeltaConfigH\x00R\x05\x64\x65lta\x12:\n\x15subdirectory_override\x18\x03 \x01(\tB\x05\x92M\x02\x08\x01R\x14subdirectoryOverrideB\x0c\n\nstore_type\"\x0f\n\rParquetConfig\"X\n\x0b\x44\x65ltaConfig\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\"\x80\x02\n\x12OfflineStoreConfig\x12^\n\x14staging_table_format\x18\x01 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12stagingTableFormat\x12\x39\n\x15publish_full_features\x18\x02 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x13publishFullFeatures\x12O\n\x12publish_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10publishStartTime\"\x99\x02\n\x10MonitoringConfig\x12+\n\x11monitor_freshness\x18\x01 \x01(\x08R\x10monitorFreshness\x12^\n\x1a\x65xpected_feature_freshness\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x18\x65xpectedFeatureFreshness\x12O\n\x12\x65xpected_freshness\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\x11\x65xpectedFreshness\x12\'\n\x0b\x61lert_email\x18\x03 \x01(\tB\x06\xf2\xe2\x02\x02\x08\x01R\nalertEmail\"\x9f\x02\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\x03 \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\x04 \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x12\x12\n\x04name\x18\x02 \x01(\tR\x04nameB\x08\n\x06window\"\x83\x01\n\nTimeWindow\x12\x42\n\x0fwindow_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\x12\x31\n\x06offset\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06offset\"\x86\x02\n\x10TimeWindowSeries\x12<\n\x0cseries_start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bseriesStart\x12\x38\n\nseries_end\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\tseriesEnd\x12\x36\n\tstep_size\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08stepSize\x12\x42\n\x0fwindow_duration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\"5\n\x0b\x43\x61\x63heConfig\x12&\n\x0fmax_age_seconds\x18\x01 \x01(\x03R\rmaxAgeSeconds*\xed\x01\n\x0f\x46\x65\x61tureViewType\x12!\n\x1d\x46\x45\x41TURE_VIEW_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_VIEW_TYPE_TEMPORAL\x10\x01\x12(\n$FEATURE_VIEW_TYPE_TEMPORAL_AGGREGATE\x10\x02\x12\x1f\n\x1b\x46\x45\x41TURE_VIEW_TYPE_ON_DEMAND\x10\x03\x12#\n\x1f\x46\x45\x41TURE_VIEW_TYPE_FEATURE_TABLE\x10\x04\x12\'\n#FEATURE_VIEW_TYPE_FWV5_FEATURE_VIEW\x10\x05*\xbf\x01\n\x12\x42\x61\x63kfillConfigMode\x12$\n BACKFILL_CONFIG_MODE_UNSPECIFIED\x10\x00\x12?\n;BACKFILL_CONFIG_MODE_SINGLE_BATCH_SCHEDULE_INTERVAL_PER_JOB\x10\x01\x12\x42\n>BACKFILL_CONFIG_MODE_MULTIPLE_BATCH_SCHEDULE_INTERVALS_PER_JOB\x10\x02*\x8f\x01\n\x14StreamProcessingMode\x12&\n\"STREAM_PROCESSING_MODE_UNSPECIFIED\x10\x00\x12(\n$STREAM_PROCESSING_MODE_TIME_INTERVAL\x10\x01\x12%\n!STREAM_PROCESSING_MODE_CONTINUOUS\x10\x02*\xa8\x01\n\x10\x42\x61tchTriggerType\x12\"\n\x1e\x42\x41TCH_TRIGGER_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1c\x42\x41TCH_TRIGGER_TYPE_SCHEDULED\x10\x01\x12\x1d\n\x19\x42\x41TCH_TRIGGER_TYPE_MANUAL\x10\x02\x12/\n+BATCH_TRIGGER_TYPE_NO_BATCH_MATERIALIZATION\x10\x03\x42\x13\n\x0f\x63om.tecton.argsP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.args.feature_view_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.argsP\001'
@@ -193,22 +193,22 @@
   _OFFLINESTORECONFIG.fields_by_name['publish_start_time']._serialized_options = b'\222M\002\010\001'
   _MONITORINGCONFIG.fields_by_name['expected_feature_freshness']._options = None
   _MONITORINGCONFIG.fields_by_name['expected_feature_freshness']._serialized_options = b'\202}\002\020\003'
   _MONITORINGCONFIG.fields_by_name['expected_freshness']._options = None
   _MONITORINGCONFIG.fields_by_name['expected_freshness']._serialized_options = b'\202}\002\010\005'
   _MONITORINGCONFIG.fields_by_name['alert_email']._options = None
   _MONITORINGCONFIG.fields_by_name['alert_email']._serialized_options = b'\362\342\002\002\010\001'
-  _FEATUREVIEWTYPE._serialized_start=13694
-  _FEATUREVIEWTYPE._serialized_end=13931
-  _BACKFILLCONFIGMODE._serialized_start=13934
-  _BACKFILLCONFIGMODE._serialized_end=14125
-  _STREAMPROCESSINGMODE._serialized_start=14128
-  _STREAMPROCESSINGMODE._serialized_end=14271
-  _BATCHTRIGGERTYPE._serialized_start=14274
-  _BATCHTRIGGERTYPE._serialized_end=14442
+  _FEATUREVIEWTYPE._serialized_start=13784
+  _FEATUREVIEWTYPE._serialized_end=14021
+  _BACKFILLCONFIGMODE._serialized_start=14024
+  _BACKFILLCONFIGMODE._serialized_end=14215
+  _STREAMPROCESSINGMODE._serialized_start=14218
+  _STREAMPROCESSINGMODE._serialized_end=14361
+  _BATCHTRIGGERTYPE._serialized_start=14364
+  _BATCHTRIGGERTYPE._serialized_end=14532
   _FEATUREVIEWARGS._serialized_start=662
   _FEATUREVIEWARGS._serialized_end=2451
   _FEATUREVIEWARGS_OPTIONSENTRY._serialized_start=2290
   _FEATUREVIEWARGS_OPTIONSENTRY._serialized_end=2348
   _ENTITYKEYOVERRIDE._serialized_start=2453
   _ENTITYKEYOVERRIDE._serialized_end=2555
   _BACKFILLCONFIG._serialized_start=2557
@@ -216,63 +216,63 @@
   _OUTPUTSTREAM._serialized_start=2635
   _OUTPUTSTREAM._serialized_end=2841
   _TEMPORALARGS._serialized_start=2844
   _TEMPORALARGS._serialized_end=3925
   _TEMPORALAGGREGATEARGS._serialized_start=3928
   _TEMPORALAGGREGATEARGS._serialized_end=5057
   _MATERIALIZEDFEATUREVIEWARGS._serialized_start=5060
-  _MATERIALIZEDFEATUREVIEWARGS._serialized_end=7273
-  _ONDEMANDARGS._serialized_start=7276
-  _ONDEMANDARGS._serialized_end=7487
-  _FEATURETABLEARGS._serialized_start=7490
-  _FEATURETABLEARGS._serialized_end=8537
-  _FEATUREAGGREGATION._serialized_start=8540
-  _FEATUREAGGREGATION._serialized_end=9328
-  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_start=9222
-  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_end=9318
-  _PARAMVALUE._serialized_start=9330
-  _PARAMVALUE._serialized_end=9423
-  _DATAQUALITYCONFIG._serialized_start=9426
-  _DATAQUALITYCONFIG._serialized_end=9569
-  _CLUSTERCONFIG._serialized_start=9572
-  _CLUSTERCONFIG._serialized_end=10256
-  _JSONCLUSTERCONFIG._serialized_start=10258
-  _JSONCLUSTERCONFIG._serialized_end=10322
-  _EXISTINGCLUSTERCONFIG._serialized_start=10324
-  _EXISTINGCLUSTERCONFIG._serialized_end=10395
-  _NEWCLUSTERCONFIG._serialized_start=10398
-  _NEWCLUSTERCONFIG._serialized_end=10813
-  _RIFTCLUSTERCONFIG._serialized_start=10815
-  _RIFTCLUSTERCONFIG._serialized_end=10871
-  _DEFAULTCLUSTERCONFIG._serialized_start=10874
-  _DEFAULTCLUSTERCONFIG._serialized_end=11063
-  _SPARKCONFIG._serialized_start=11066
-  _SPARKCONFIG._serialized_end=11453
-  _SPARKCONFIG_SPARKCONFENTRY._serialized_start=11393
-  _SPARKCONFIG_SPARKCONFENTRY._serialized_end=11453
-  _ONLINESTORECONFIG._serialized_start=11456
-  _ONLINESTORECONFIG._serialized_end=11686
-  _DYNAMODBONLINESTORE._serialized_start=11688
-  _DYNAMODBONLINESTORE._serialized_end=11759
-  _REDISONLINESTORE._serialized_start=11762
-  _REDISONLINESTORE._serialized_end=11962
-  _BIGTABLEONLINESTORE._serialized_start=11964
-  _BIGTABLEONLINESTORE._serialized_end=12075
-  _OFFLINEFEATURESTORECONFIG._serialized_start=12078
-  _OFFLINEFEATURESTORECONFIG._serialized_end=12297
-  _PARQUETCONFIG._serialized_start=12299
-  _PARQUETCONFIG._serialized_end=12314
-  _DELTACONFIG._serialized_start=12316
-  _DELTACONFIG._serialized_end=12404
-  _OFFLINESTORECONFIG._serialized_start=12407
-  _OFFLINESTORECONFIG._serialized_end=12663
-  _MONITORINGCONFIG._serialized_start=12666
-  _MONITORINGCONFIG._serialized_end=12947
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=12950
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=13237
-  _TIMEWINDOW._serialized_start=13240
-  _TIMEWINDOW._serialized_end=13371
-  _TIMEWINDOWSERIES._serialized_start=13374
-  _TIMEWINDOWSERIES._serialized_end=13636
-  _CACHECONFIG._serialized_start=13638
-  _CACHECONFIG._serialized_end=13691
+  _MATERIALIZEDFEATUREVIEWARGS._serialized_end=7363
+  _ONDEMANDARGS._serialized_start=7366
+  _ONDEMANDARGS._serialized_end=7577
+  _FEATURETABLEARGS._serialized_start=7580
+  _FEATURETABLEARGS._serialized_end=8627
+  _FEATUREAGGREGATION._serialized_start=8630
+  _FEATUREAGGREGATION._serialized_end=9418
+  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_start=9312
+  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_end=9408
+  _PARAMVALUE._serialized_start=9420
+  _PARAMVALUE._serialized_end=9513
+  _DATAQUALITYCONFIG._serialized_start=9516
+  _DATAQUALITYCONFIG._serialized_end=9659
+  _CLUSTERCONFIG._serialized_start=9662
+  _CLUSTERCONFIG._serialized_end=10346
+  _JSONCLUSTERCONFIG._serialized_start=10348
+  _JSONCLUSTERCONFIG._serialized_end=10412
+  _EXISTINGCLUSTERCONFIG._serialized_start=10414
+  _EXISTINGCLUSTERCONFIG._serialized_end=10485
+  _NEWCLUSTERCONFIG._serialized_start=10488
+  _NEWCLUSTERCONFIG._serialized_end=10903
+  _RIFTCLUSTERCONFIG._serialized_start=10905
+  _RIFTCLUSTERCONFIG._serialized_end=10961
+  _DEFAULTCLUSTERCONFIG._serialized_start=10964
+  _DEFAULTCLUSTERCONFIG._serialized_end=11153
+  _SPARKCONFIG._serialized_start=11156
+  _SPARKCONFIG._serialized_end=11543
+  _SPARKCONFIG_SPARKCONFENTRY._serialized_start=11483
+  _SPARKCONFIG_SPARKCONFENTRY._serialized_end=11543
+  _ONLINESTORECONFIG._serialized_start=11546
+  _ONLINESTORECONFIG._serialized_end=11776
+  _DYNAMODBONLINESTORE._serialized_start=11778
+  _DYNAMODBONLINESTORE._serialized_end=11849
+  _REDISONLINESTORE._serialized_start=11852
+  _REDISONLINESTORE._serialized_end=12052
+  _BIGTABLEONLINESTORE._serialized_start=12054
+  _BIGTABLEONLINESTORE._serialized_end=12165
+  _OFFLINEFEATURESTORECONFIG._serialized_start=12168
+  _OFFLINEFEATURESTORECONFIG._serialized_end=12387
+  _PARQUETCONFIG._serialized_start=12389
+  _PARQUETCONFIG._serialized_end=12404
+  _DELTACONFIG._serialized_start=12406
+  _DELTACONFIG._serialized_end=12494
+  _OFFLINESTORECONFIG._serialized_start=12497
+  _OFFLINESTORECONFIG._serialized_end=12753
+  _MONITORINGCONFIG._serialized_start=12756
+  _MONITORINGCONFIG._serialized_end=13037
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=13040
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=13327
+  _TIMEWINDOW._serialized_start=13330
+  _TIMEWINDOW._serialized_end=13461
+  _TIMEWINDOWSERIES._serialized_start=13464
+  _TIMEWINDOWSERIES._serialized_end=13726
+  _CACHECONFIG._serialized_start=13728
+  _CACHECONFIG._serialized_end=13781
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.9.0rc1/tecton_proto/args/pipeline_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/transformation_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.9.0rc2/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auditlog/metadata_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auditlog/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auth/acl_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auth/principal_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auth/resource_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/auth/service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/canary/type_pb2.py` & `tecton-0.9.0rc2/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/canary/update_pb2.py` & `tecton-0.9.0rc2/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.9.0rc2/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/aws_credentials_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/aws_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/column_type_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/compute_mode_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/compute_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/container_image_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/data_type_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/framework_version_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/id_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/pair_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/schema_container_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/schema_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/secret_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/common/time_window_pb2.py` & `tecton-0.9.0rc2/tecton_proto/common/time_window_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.9.0rc2/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/entity_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/fco_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/feature_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/feature_store_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/feature_view_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/feature_view_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from tecton_proto.common import time_window_pb2 as tecton__proto_dot_common_dot_time__window__pb2
 from tecton_proto.data import fco_metadata_pb2 as tecton__proto_dot_data_dot_fco__metadata__pb2
 from tecton_proto.data import fv_materialization_pb2 as tecton__proto_dot_data_dot_fv__materialization__pb2
 from tecton_proto.data import odfv_compute_pb2 as tecton__proto_dot_data_dot_odfv__compute__pb2
 from tecton_proto.validation import validator_pb2 as tecton__proto_dot_validation_dot_validator__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/data/feature_view.proto\x12\x11tecton_proto.data\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$tecton_proto/args/feature_view.proto\x1a tecton_proto/args/pipeline.proto\x1a.tecton_proto/common/aggregation_function.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a%tecton_proto/common/time_window.proto\x1a$tecton_proto/data/fco_metadata.proto\x1a*tecton_proto/data/fv_materialization.proto\x1a$tecton_proto/data/odfv_compute.proto\x1a\'tecton_proto/validation/validator.proto\"\xad\x10\n\x0b\x46\x65\x61tureView\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12\x41\n\x0c\x66\x63o_metadata\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.data.FcoMetadataR\x0b\x66\x63oMetadata\x12\x36\n\nentity_ids\x18\x03 \x03(\x0b\x32\x17.tecton_proto.common.IdR\tentityIds\x12\x1b\n\tjoin_keys\x18\x04 \x03(\tR\x08joinKeys\x12?\n\x07schemas\x18\x0b \x01(\x0b\x32%.tecton_proto.data.FeatureViewSchemasR\x07schemas\x12P\n\x0b\x65nrichments\x18\xe8\x07 \x01(\x0b\x32).tecton_proto.data.FeatureViewEnrichmentsB\x02\x18\x01R\x0b\x65nrichments\x12U\n\x12temporal_aggregate\x18\x07 \x01(\x0b\x32$.tecton_proto.data.TemporalAggregateH\x00R\x11temporalAggregate\x12\x39\n\x08temporal\x18\x08 \x01(\x0b\x32\x1b.tecton_proto.data.TemporalH\x00R\x08temporal\x12]\n\x16on_demand_feature_view\x18\x11 \x01(\x0b\x32&.tecton_proto.data.OnDemandFeatureViewH\x00R\x13onDemandFeatureView\x12\x46\n\rfeature_table\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.data.FeatureTableH\x00R\x0c\x66\x65\x61tureTable\x12#\n\rtimestamp_key\x18\n \x01(\tR\x0ctimestampKey\x12W\n\x14online_serving_index\x18\x05 \x01(\x0b\x32%.tecton_proto.data.OnlineServingIndexR\x12onlineServingIndex\x12\x37\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineR\x08pipeline\x12\x62\n\x16materialization_params\x18\t \x01(\x0b\x32+.tecton_proto.data.NewMaterializationParamsR\x15materializationParams\x12\x37\n\x17materialization_enabled\x18\x0c \x01(\x08R\x16materializationEnabled\x12}\n!materialization_state_transitions\x18\r \x03(\x0b\x32\x31.tecton_proto.data.MaterializationStateTransitionR\x1fmaterializationStateTransitions\x12P\n\x11monitoring_params\x18\x0e \x01(\x0b\x32#.tecton_proto.data.MonitoringParamsR\x10monitoringParams\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x17 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12G\n\x0esnowflake_data\x18\x18 \x01(\x0b\x32 .tecton_proto.data.SnowflakeDataR\rsnowflakeData\x12/\n\x11\x66ramework_version\x18\x13 \x01(\x05\x42\x02\x18\x01R\x10\x66rameworkVersion\x12H\n\nfw_version\x18\x1a \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x02\x18\x01R\tfwVersion\x12\x17\n\x07web_url\x18\x19 \x01(\tR\x06webUrl\x12H\n\rbatch_trigger\x18\x1b \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeR\x0c\x62\x61tchTrigger\x12[\n\x0fvalidation_args\x18\x1c \x01(\x0b\x32\x32.tecton_proto.validation.FeatureViewValidationArgsR\x0evalidationArgs\x12T\n\x13\x64\x61ta_quality_config\x18\x1d \x01(\x0b\x32$.tecton_proto.data.DataQualityConfigR\x11\x64\x61taQualityConfig\x12\x45\n\x07options\x18\x1e \x03(\x0b\x32+.tecton_proto.data.FeatureView.OptionsEntryR\x07options\x12S\n\x12\x62\x61tch_compute_mode\x18\x1f \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeR\x10\x62\x61tchComputeMode\x12L\n\x0c\x63\x61\x63he_config\x18  \x01(\x0b\x32).tecton_proto.data.FeatureViewCacheConfigR\x0b\x63\x61\x63heConfig\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x13\n\x11\x66\x65\x61ture_view_type\"\xe8\x03\n\x11TemporalAggregate\x12@\n\x0eslide_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\rslideInterval\x12\x32\n\x15slide_interval_string\x18\x05 \x01(\tR\x13slideIntervalString\x12?\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x03 \x01(\x08R\x0cisContinuous\x12M\n\x10\x64\x61ta_source_type\x18\x04 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12:\n\x19\x61ggregation_secondary_key\x18\x06 \x01(\tR\x17\x61ggregationSecondaryKey\x12l\n\x1csecondary_key_output_columns\x18\x07 \x03(\x0b\x32+.tecton_proto.data.SecondaryKeyOutputColumnR\x19secondaryKeyOutputColumns\"\x84\x03\n\x10\x41ggregateFeature\x12,\n\x12input_feature_name\x18\x01 \x01(\tR\x10inputFeatureName\x12.\n\x13output_feature_name\x18\x02 \x01(\tR\x11outputFeatureName\x12\x44\n\x08\x66unction\x18\x03 \x01(\x0e\x32(.tecton_proto.common.AggregationFunctionR\x08\x66unction\x12W\n\x0f\x66unction_params\x18\x05 \x01(\x0b\x32..tecton_proto.common.AggregationFunctionParamsR\x0e\x66unctionParams\x12\x31\n\x06window\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06window\x12@\n\x0btime_window\x18\x06 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\"\xf5\x01\n\x1dTrailingTimeWindowAggregation\x12\x19\n\x08time_key\x18\x01 \x01(\tR\x07timeKey\x12S\n\x18\x61ggregation_slide_period\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x16\x61ggregationSlidePeriod\x12?\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x04 \x01(\x08R\x0cisContinuous\"\xbb\x02\n\x08Temporal\x12:\n\x0bserving_ttl\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\x12M\n\x10\x64\x61ta_source_type\x18\x11 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12J\n\x0f\x62\x61\x63kfill_config\x18\x12 \x01(\x0b\x32!.tecton_proto.args.BackfillConfigR\x0e\x62\x61\x63kfillConfig\x12\x33\n\x15incremental_backfills\x18\x13 \x01(\x08R\x14incrementalBackfills\x12#\n\ris_continuous\x18\x14 \x01(\x08R\x0cisContinuous\"\x9a\x01\n\x0c\x46\x65\x61tureTable\x12%\n\x0eonline_enabled\x18\x01 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x02 \x01(\x08R\x0eofflineEnabled\x12:\n\x0bserving_ttl\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\"\x8f\x01\n\x13OnDemandFeatureView\x12\x13\n\x05no_op\x18\x01 \x01(\x08R\x04noOp\x12]\n\x16supported_environments\x18\x03 \x03(\x0b\x32&.tecton_proto.data.RemoteComputeConfigR\x15supportedEnvironmentsJ\x04\x08\x02\x10\x03\"\xc5\x02\n\x12\x46\x65\x61tureViewSchemas\x12<\n\x0bview_schema\x18\x01 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\nviewSchema\x12\x35\n\x17is_explicit_view_schema\x18\x04 \x01(\x08R\x14isExplicitViewSchema\x12R\n\x16materialization_schema\x18\x02 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\x15materializationSchema\x12\x66\n\x19online_batch_table_format\x18\x03 \x01(\x0b\x32+.tecton_proto.common.OnlineBatchTableFormatR\x16onlineBatchTableFormat\"1\n\x12OnlineServingIndex\x12\x1b\n\tjoin_keys\x18\x01 \x03(\tR\x08joinKeys\"\xb3\x03\n\x1eMaterializationStateTransition\x12\x38\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\x12%\n\x0eonline_enabled\x18\x02 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x03 \x01(\x08R\x0eofflineEnabled\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12\x44\n\x1ematerialization_serial_version\x18\x05 \x01(\x05R\x1cmaterializationSerialVersion\x12\x37\n\x18\x66orce_stream_job_restart\x18\x06 \x01(\x08R\x15\x66orceStreamJobRestart\x12\x34\n\x16tecton_runtime_version\x18\x07 \x01(\tR\x14tectonRuntimeVersion\"\xaf\x01\n\x19ParquetOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12G\n\x07version\x18\x02 \x01(\x0e\x32-.tecton_proto.data.ParquetOfflineStoreVersionR\x07version\"\xab\x01\n\x17\x44\x65ltaOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12\x45\n\x07version\x18\x02 \x01(\x0e\x32+.tecton_proto.data.DeltaOfflineStoreVersionR\x07version\"\xac\x01\n\x12OfflineStoreParams\x12H\n\x07parquet\x18\x01 \x01(\x0b\x32,.tecton_proto.data.ParquetOfflineStoreParamsH\x00R\x07parquet\x12\x42\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32*.tecton_proto.data.DeltaOfflineStoreParamsH\x00R\x05\x64\x65ltaB\x08\n\x06params\"\xa0\x01\n FeaturePublishOfflineStoreConfig\x12\x32\n\x15publish_full_features\x18\x01 \x01(\x08R\x13publishFullFeatures\x12H\n\x12publish_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10publishStartTime\"\xe3\r\n\x18NewMaterializationParams\x12\x46\n\x11schedule_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12\x62\n\x1fmaterialization_start_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x1dmaterializationStartTimestamp\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12l\n%manual_trigger_backfill_end_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.TimestampR!manualTriggerBackfillEndTimestamp\x12M\n\x15max_backfill_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x13maxBackfillInterval\x12\x33\n\x16writes_to_online_store\x18\x04 \x01(\x08R\x13writesToOnlineStore\x12\x35\n\x17writes_to_offline_store\x18\x05 \x01(\x08R\x14writesToOfflineStore\x12^\n\x14offline_store_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12offlineStoreConfig\x12W\n\x14offline_store_params\x18\x0e \x01(\x0b\x32%.tecton_proto.data.OfflineStoreParamsR\x12offlineStoreParams\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12W\n\x16stream_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x15streamMaterialization\x12L\n\x15max_source_data_delay\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationR\x12maxSourceDataDelay\x12T\n\x13online_store_params\x18\n \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParams\x12\x44\n\routput_stream\x18\x0b \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12]\n\x11time_range_policy\x18\x0c \x01(\x0e\x32\x31.tecton_proto.data.MaterializationTimeRangePolicyR\x0ftimeRangePolicy\x12\x64\n\x19online_backfill_load_type\x18\x10 \x01(\x0e\x32).tecton_proto.data.OnlineBackfillLoadTypeR\x16onlineBackfillLoadType\x12\x44\n\x1etecton_materialization_runtime\x18\x11 \x01(\tR\x1ctectonMaterializationRuntime\x12\x83\x01\n$feature_publish_offline_store_config\x18\x13 \x01(\x0b\x32\x33.tecton_proto.data.FeaturePublishOfflineStoreConfigR featurePublishOfflineStoreConfig\x12\x38\n\x18\x62\x61tch_compaction_enabled\x18\x14 \x01(\x08R\x16\x62\x61tchCompactionEnabled\x12 \n\x0b\x65nvironment\x18\x15 \x01(\tR\x0b\x65nvironment\x12X\n\x1bstream_compaction_tile_size\x18\x16 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18streamCompactionTileSizeJ\x04\x08\x12\x10\x13\"\x8d\x02\n\x11OnlineStoreParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12@\n\x06\x64ynamo\x18\x02 \x01(\x0b\x32&.tecton_proto.data.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x03 \x01(\x0b\x32#.tecton_proto.data.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x04 \x01(\x0b\x32&.tecton_proto.data.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"\xa1\x02\n\x13\x44ynamoDbOnlineStore\x12\x33\n\x16\x63ross_account_role_arn\x18\x01 \x01(\tR\x13\x63rossAccountRoleArn\x12\x39\n\x19\x63ross_account_external_id\x18\x02 \x01(\tR\x16\x63rossAccountExternalId\x12L\n#cross_account_intermediate_role_arn\x18\x05 \x01(\tR\x1f\x63rossAccountIntermediateRoleArn\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabled\x12\x32\n\x15\x64\x62\x66s_credentials_path\x18\x04 \x01(\tR\x13\x64\x62\x66sCredentialsPath\"\xeb\x01\n\x10RedisOnlineStore\x12)\n\x10primary_endpoint\x18\x02 \x01(\tR\x0fprimaryEndpoint\x12\x31\n\x14\x61uthentication_token\x18\x04 \x01(\tR\x13\x61uthenticationToken\x12\x1f\n\x0btls_enabled\x18\x06 \x01(\x08R\ntlsEnabled\x12\x18\n\x07\x65nabled\x18\x05 \x01(\x08R\x07\x65nabled\x12&\n\x0finject_host_sni\x18\t \x01(\x08R\rinjectHostSniJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\x92\x02\n\x10MonitoringParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12+\n\x11monitor_freshness\x18\x02 \x01(\x08R\x10monitorFreshness\x12W\n\x1a\x65xpected_feature_freshness\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18\x65xpectedFeatureFreshness\x12\x1f\n\x0b\x61lert_email\x18\x04 \x01(\tR\nalertEmail\x12\x30\n\x14grace_period_seconds\x18\x05 \x01(\x05R\x12gracePeriodSeconds\"\x85\x01\n\x16\x46\x65\x61tureViewEnrichments\x12S\n\x12\x66p_materialization\x18\x04 \x01(\x0b\x32$.tecton_proto.data.FvMaterializationR\x11\x66pMaterializationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x05\x10\x06\"?\n\rSnowflakeData\x12.\n\x13snowflake_view_name\x18\x01 \x01(\tR\x11snowflakeViewName\"\x81\x01\n\x11\x44\x61taQualityConfig\x12\x30\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08R\x12\x64\x61taQualityEnabled\x12:\n\x19skip_default_expectations\x18\x02 \x01(\x08R\x17skipDefaultExpectations\"p\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\x92\x02\n\x16\x46\x65\x61tureViewCacheConfig\x12\x1c\n\tnamespace\x18\x01 \x01(\tR\tnamespace\x12(\n\x10\x63\x61\x63he_group_name\x18\x02 \x01(\tR\x0e\x63\x61\x63heGroupName\x12\x41\n\x0fmax_age_seconds\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\rmaxAgeSeconds\x12?\n\x0emax_age_jitter\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0cmaxAgeJitter\x12,\n\x12remapped_join_keys\x18\x05 \x03(\tR\x10remappedJoinKeys*\x95\x01\n\x1aParquetOfflineStoreVersion\x12-\n)PARQUET_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_1\x10\x01\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_2\x10\x02*\x8d\x01\n\x18\x44\x65ltaOfflineStoreVersion\x12+\n\'DELTA_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_1\x10\x01\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_2\x10\x02*\xc6\x01\n\x1eMaterializationTimeRangePolicy\x12\x31\n-MATERIALIZATION_TIME_RANGE_POLICY_UNSPECIFIED\x10\x00\x12:\n6MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE\x10\x01\x12\x35\n1MATERIALIZATION_TIME_RANGE_POLICY_FILTER_TO_RANGE\x10\x02\x42\x13\n\x0f\x63om.tecton.dataP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/data/feature_view.proto\x12\x11tecton_proto.data\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$tecton_proto/args/feature_view.proto\x1a tecton_proto/args/pipeline.proto\x1a.tecton_proto/common/aggregation_function.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a%tecton_proto/common/time_window.proto\x1a$tecton_proto/data/fco_metadata.proto\x1a*tecton_proto/data/fv_materialization.proto\x1a$tecton_proto/data/odfv_compute.proto\x1a\'tecton_proto/validation/validator.proto\"\xad\x10\n\x0b\x46\x65\x61tureView\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12\x41\n\x0c\x66\x63o_metadata\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.data.FcoMetadataR\x0b\x66\x63oMetadata\x12\x36\n\nentity_ids\x18\x03 \x03(\x0b\x32\x17.tecton_proto.common.IdR\tentityIds\x12\x1b\n\tjoin_keys\x18\x04 \x03(\tR\x08joinKeys\x12?\n\x07schemas\x18\x0b \x01(\x0b\x32%.tecton_proto.data.FeatureViewSchemasR\x07schemas\x12P\n\x0b\x65nrichments\x18\xe8\x07 \x01(\x0b\x32).tecton_proto.data.FeatureViewEnrichmentsB\x02\x18\x01R\x0b\x65nrichments\x12U\n\x12temporal_aggregate\x18\x07 \x01(\x0b\x32$.tecton_proto.data.TemporalAggregateH\x00R\x11temporalAggregate\x12\x39\n\x08temporal\x18\x08 \x01(\x0b\x32\x1b.tecton_proto.data.TemporalH\x00R\x08temporal\x12]\n\x16on_demand_feature_view\x18\x11 \x01(\x0b\x32&.tecton_proto.data.OnDemandFeatureViewH\x00R\x13onDemandFeatureView\x12\x46\n\rfeature_table\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.data.FeatureTableH\x00R\x0c\x66\x65\x61tureTable\x12#\n\rtimestamp_key\x18\n \x01(\tR\x0ctimestampKey\x12W\n\x14online_serving_index\x18\x05 \x01(\x0b\x32%.tecton_proto.data.OnlineServingIndexR\x12onlineServingIndex\x12\x37\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineR\x08pipeline\x12\x62\n\x16materialization_params\x18\t \x01(\x0b\x32+.tecton_proto.data.NewMaterializationParamsR\x15materializationParams\x12\x37\n\x17materialization_enabled\x18\x0c \x01(\x08R\x16materializationEnabled\x12}\n!materialization_state_transitions\x18\r \x03(\x0b\x32\x31.tecton_proto.data.MaterializationStateTransitionR\x1fmaterializationStateTransitions\x12P\n\x11monitoring_params\x18\x0e \x01(\x0b\x32#.tecton_proto.data.MonitoringParamsR\x10monitoringParams\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x17 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12G\n\x0esnowflake_data\x18\x18 \x01(\x0b\x32 .tecton_proto.data.SnowflakeDataR\rsnowflakeData\x12/\n\x11\x66ramework_version\x18\x13 \x01(\x05\x42\x02\x18\x01R\x10\x66rameworkVersion\x12H\n\nfw_version\x18\x1a \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x02\x18\x01R\tfwVersion\x12\x17\n\x07web_url\x18\x19 \x01(\tR\x06webUrl\x12H\n\rbatch_trigger\x18\x1b \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeR\x0c\x62\x61tchTrigger\x12[\n\x0fvalidation_args\x18\x1c \x01(\x0b\x32\x32.tecton_proto.validation.FeatureViewValidationArgsR\x0evalidationArgs\x12T\n\x13\x64\x61ta_quality_config\x18\x1d \x01(\x0b\x32$.tecton_proto.data.DataQualityConfigR\x11\x64\x61taQualityConfig\x12\x45\n\x07options\x18\x1e \x03(\x0b\x32+.tecton_proto.data.FeatureView.OptionsEntryR\x07options\x12S\n\x12\x62\x61tch_compute_mode\x18\x1f \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeR\x10\x62\x61tchComputeMode\x12L\n\x0c\x63\x61\x63he_config\x18  \x01(\x0b\x32).tecton_proto.data.FeatureViewCacheConfigR\x0b\x63\x61\x63heConfig\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x13\n\x11\x66\x65\x61ture_view_type\"\xe8\x03\n\x11TemporalAggregate\x12@\n\x0eslide_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\rslideInterval\x12\x32\n\x15slide_interval_string\x18\x05 \x01(\tR\x13slideIntervalString\x12?\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x03 \x01(\x08R\x0cisContinuous\x12M\n\x10\x64\x61ta_source_type\x18\x04 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12:\n\x19\x61ggregation_secondary_key\x18\x06 \x01(\tR\x17\x61ggregationSecondaryKey\x12l\n\x1csecondary_key_output_columns\x18\x07 \x03(\x0b\x32+.tecton_proto.data.SecondaryKeyOutputColumnR\x19secondaryKeyOutputColumns\"\x84\x03\n\x10\x41ggregateFeature\x12,\n\x12input_feature_name\x18\x01 \x01(\tR\x10inputFeatureName\x12.\n\x13output_feature_name\x18\x02 \x01(\tR\x11outputFeatureName\x12\x44\n\x08\x66unction\x18\x03 \x01(\x0e\x32(.tecton_proto.common.AggregationFunctionR\x08\x66unction\x12W\n\x0f\x66unction_params\x18\x05 \x01(\x0b\x32..tecton_proto.common.AggregationFunctionParamsR\x0e\x66unctionParams\x12\x31\n\x06window\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06window\x12@\n\x0btime_window\x18\x06 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\"\xf5\x01\n\x1dTrailingTimeWindowAggregation\x12\x19\n\x08time_key\x18\x01 \x01(\tR\x07timeKey\x12S\n\x18\x61ggregation_slide_period\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x16\x61ggregationSlidePeriod\x12?\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x04 \x01(\x08R\x0cisContinuous\"\xbb\x02\n\x08Temporal\x12:\n\x0bserving_ttl\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\x12M\n\x10\x64\x61ta_source_type\x18\x11 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12J\n\x0f\x62\x61\x63kfill_config\x18\x12 \x01(\x0b\x32!.tecton_proto.args.BackfillConfigR\x0e\x62\x61\x63kfillConfig\x12\x33\n\x15incremental_backfills\x18\x13 \x01(\x08R\x14incrementalBackfills\x12#\n\ris_continuous\x18\x14 \x01(\x08R\x0cisContinuous\"\x9a\x01\n\x0c\x46\x65\x61tureTable\x12%\n\x0eonline_enabled\x18\x01 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x02 \x01(\x08R\x0eofflineEnabled\x12:\n\x0bserving_ttl\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\"\x8f\x01\n\x13OnDemandFeatureView\x12\x13\n\x05no_op\x18\x01 \x01(\x08R\x04noOp\x12]\n\x16supported_environments\x18\x03 \x03(\x0b\x32&.tecton_proto.data.RemoteComputeConfigR\x15supportedEnvironmentsJ\x04\x08\x02\x10\x03\"\xc5\x02\n\x12\x46\x65\x61tureViewSchemas\x12<\n\x0bview_schema\x18\x01 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\nviewSchema\x12\x35\n\x17is_explicit_view_schema\x18\x04 \x01(\x08R\x14isExplicitViewSchema\x12R\n\x16materialization_schema\x18\x02 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\x15materializationSchema\x12\x66\n\x19online_batch_table_format\x18\x03 \x01(\x0b\x32+.tecton_proto.common.OnlineBatchTableFormatR\x16onlineBatchTableFormat\"1\n\x12OnlineServingIndex\x12\x1b\n\tjoin_keys\x18\x01 \x03(\tR\x08joinKeys\"\xb3\x03\n\x1eMaterializationStateTransition\x12\x38\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\x12%\n\x0eonline_enabled\x18\x02 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x03 \x01(\x08R\x0eofflineEnabled\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12\x44\n\x1ematerialization_serial_version\x18\x05 \x01(\x05R\x1cmaterializationSerialVersion\x12\x37\n\x18\x66orce_stream_job_restart\x18\x06 \x01(\x08R\x15\x66orceStreamJobRestart\x12\x34\n\x16tecton_runtime_version\x18\x07 \x01(\tR\x14tectonRuntimeVersion\"\xaf\x01\n\x19ParquetOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12G\n\x07version\x18\x02 \x01(\x0e\x32-.tecton_proto.data.ParquetOfflineStoreVersionR\x07version\"\xab\x01\n\x17\x44\x65ltaOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12\x45\n\x07version\x18\x02 \x01(\x0e\x32+.tecton_proto.data.DeltaOfflineStoreVersionR\x07version\"\xac\x01\n\x12OfflineStoreParams\x12H\n\x07parquet\x18\x01 \x01(\x0b\x32,.tecton_proto.data.ParquetOfflineStoreParamsH\x00R\x07parquet\x12\x42\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32*.tecton_proto.data.DeltaOfflineStoreParamsH\x00R\x05\x64\x65ltaB\x08\n\x06params\"\xa0\x01\n FeaturePublishOfflineStoreConfig\x12\x32\n\x15publish_full_features\x18\x01 \x01(\x08R\x13publishFullFeatures\x12H\n\x12publish_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10publishStartTime\"\x9f\x0e\n\x18NewMaterializationParams\x12\x46\n\x11schedule_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12\x62\n\x1fmaterialization_start_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x1dmaterializationStartTimestamp\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12l\n%manual_trigger_backfill_end_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.TimestampR!manualTriggerBackfillEndTimestamp\x12M\n\x15max_backfill_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x13maxBackfillInterval\x12\x33\n\x16writes_to_online_store\x18\x04 \x01(\x08R\x13writesToOnlineStore\x12\x35\n\x17writes_to_offline_store\x18\x05 \x01(\x08R\x14writesToOfflineStore\x12^\n\x14offline_store_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12offlineStoreConfig\x12W\n\x14offline_store_params\x18\x0e \x01(\x0b\x32%.tecton_proto.data.OfflineStoreParamsR\x12offlineStoreParams\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12W\n\x16stream_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x15streamMaterialization\x12L\n\x15max_source_data_delay\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationR\x12maxSourceDataDelay\x12T\n\x13online_store_params\x18\n \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParams\x12\x44\n\routput_stream\x18\x0b \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12]\n\x11time_range_policy\x18\x0c \x01(\x0e\x32\x31.tecton_proto.data.MaterializationTimeRangePolicyR\x0ftimeRangePolicy\x12\x64\n\x19online_backfill_load_type\x18\x10 \x01(\x0e\x32).tecton_proto.data.OnlineBackfillLoadTypeR\x16onlineBackfillLoadType\x12\x44\n\x1etecton_materialization_runtime\x18\x11 \x01(\tR\x1ctectonMaterializationRuntime\x12\x83\x01\n$feature_publish_offline_store_config\x18\x13 \x01(\x0b\x32\x33.tecton_proto.data.FeaturePublishOfflineStoreConfigR featurePublishOfflineStoreConfig\x12\x38\n\x18\x62\x61tch_compaction_enabled\x18\x14 \x01(\x08R\x16\x62\x61tchCompactionEnabled\x12:\n\x19stream_compaction_enabled\x18\x17 \x01(\x08R\x17streamCompactionEnabled\x12 \n\x0b\x65nvironment\x18\x15 \x01(\tR\x0b\x65nvironment\x12X\n\x1bstream_compaction_tile_size\x18\x16 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18streamCompactionTileSizeJ\x04\x08\x12\x10\x13\"\x8d\x02\n\x11OnlineStoreParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12@\n\x06\x64ynamo\x18\x02 \x01(\x0b\x32&.tecton_proto.data.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x03 \x01(\x0b\x32#.tecton_proto.data.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x04 \x01(\x0b\x32&.tecton_proto.data.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"\xa1\x02\n\x13\x44ynamoDbOnlineStore\x12\x33\n\x16\x63ross_account_role_arn\x18\x01 \x01(\tR\x13\x63rossAccountRoleArn\x12\x39\n\x19\x63ross_account_external_id\x18\x02 \x01(\tR\x16\x63rossAccountExternalId\x12L\n#cross_account_intermediate_role_arn\x18\x05 \x01(\tR\x1f\x63rossAccountIntermediateRoleArn\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabled\x12\x32\n\x15\x64\x62\x66s_credentials_path\x18\x04 \x01(\tR\x13\x64\x62\x66sCredentialsPath\"\xeb\x01\n\x10RedisOnlineStore\x12)\n\x10primary_endpoint\x18\x02 \x01(\tR\x0fprimaryEndpoint\x12\x31\n\x14\x61uthentication_token\x18\x04 \x01(\tR\x13\x61uthenticationToken\x12\x1f\n\x0btls_enabled\x18\x06 \x01(\x08R\ntlsEnabled\x12\x18\n\x07\x65nabled\x18\x05 \x01(\x08R\x07\x65nabled\x12&\n\x0finject_host_sni\x18\t \x01(\x08R\rinjectHostSniJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\x92\x02\n\x10MonitoringParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12+\n\x11monitor_freshness\x18\x02 \x01(\x08R\x10monitorFreshness\x12W\n\x1a\x65xpected_feature_freshness\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18\x65xpectedFeatureFreshness\x12\x1f\n\x0b\x61lert_email\x18\x04 \x01(\tR\nalertEmail\x12\x30\n\x14grace_period_seconds\x18\x05 \x01(\x05R\x12gracePeriodSeconds\"\x85\x01\n\x16\x46\x65\x61tureViewEnrichments\x12S\n\x12\x66p_materialization\x18\x04 \x01(\x0b\x32$.tecton_proto.data.FvMaterializationR\x11\x66pMaterializationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x05\x10\x06\"?\n\rSnowflakeData\x12.\n\x13snowflake_view_name\x18\x01 \x01(\tR\x11snowflakeViewName\"\x81\x01\n\x11\x44\x61taQualityConfig\x12\x30\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08R\x12\x64\x61taQualityEnabled\x12:\n\x19skip_default_expectations\x18\x02 \x01(\x08R\x17skipDefaultExpectations\"p\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\x92\x02\n\x16\x46\x65\x61tureViewCacheConfig\x12\x1c\n\tnamespace\x18\x01 \x01(\tR\tnamespace\x12(\n\x10\x63\x61\x63he_group_name\x18\x02 \x01(\tR\x0e\x63\x61\x63heGroupName\x12\x41\n\x0fmax_age_seconds\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\rmaxAgeSeconds\x12?\n\x0emax_age_jitter\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0cmaxAgeJitter\x12,\n\x12remapped_join_keys\x18\x05 \x03(\tR\x10remappedJoinKeys*\x95\x01\n\x1aParquetOfflineStoreVersion\x12-\n)PARQUET_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_1\x10\x01\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_2\x10\x02*\x8d\x01\n\x18\x44\x65ltaOfflineStoreVersion\x12+\n\'DELTA_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_1\x10\x01\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_2\x10\x02*\xc6\x01\n\x1eMaterializationTimeRangePolicy\x12\x31\n-MATERIALIZATION_TIME_RANGE_POLICY_UNSPECIFIED\x10\x00\x12:\n6MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE\x10\x01\x12\x35\n1MATERIALIZATION_TIME_RANGE_POLICY_FILTER_TO_RANGE\x10\x02\x42\x13\n\x0f\x63om.tecton.dataP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.data.feature_view_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.dataP\001'
@@ -40,20 +40,20 @@
   _FEATUREVIEW_OPTIONSENTRY._serialized_options = b'8\001'
   _FEATUREVIEW.fields_by_name['enrichments']._options = None
   _FEATUREVIEW.fields_by_name['enrichments']._serialized_options = b'\030\001'
   _FEATUREVIEW.fields_by_name['framework_version']._options = None
   _FEATUREVIEW.fields_by_name['framework_version']._serialized_options = b'\030\001'
   _FEATUREVIEW.fields_by_name['fw_version']._options = None
   _FEATUREVIEW.fields_by_name['fw_version']._serialized_options = b'\030\001'
-  _PARQUETOFFLINESTOREVERSION._serialized_start=9674
-  _PARQUETOFFLINESTOREVERSION._serialized_end=9823
-  _DELTAOFFLINESTOREVERSION._serialized_start=9826
-  _DELTAOFFLINESTOREVERSION._serialized_end=9967
-  _MATERIALIZATIONTIMERANGEPOLICY._serialized_start=9970
-  _MATERIALIZATIONTIMERANGEPOLICY._serialized_end=10168
+  _PARQUETOFFLINESTOREVERSION._serialized_start=9734
+  _PARQUETOFFLINESTOREVERSION._serialized_end=9883
+  _DELTAOFFLINESTOREVERSION._serialized_start=9886
+  _DELTAOFFLINESTOREVERSION._serialized_end=10027
+  _MATERIALIZATIONTIMERANGEPOLICY._serialized_start=10030
+  _MATERIALIZATIONTIMERANGEPOLICY._serialized_end=10228
   _FEATUREVIEW._serialized_start=638
   _FEATUREVIEW._serialized_end=2731
   _FEATUREVIEW_OPTIONSENTRY._serialized_start=2652
   _FEATUREVIEW_OPTIONSENTRY._serialized_end=2710
   _TEMPORALAGGREGATE._serialized_start=2734
   _TEMPORALAGGREGATE._serialized_end=3222
   _AGGREGATEFEATURE._serialized_start=3225
@@ -77,29 +77,29 @@
   _DELTAOFFLINESTOREPARAMS._serialized_start=5480
   _DELTAOFFLINESTOREPARAMS._serialized_end=5651
   _OFFLINESTOREPARAMS._serialized_start=5654
   _OFFLINESTOREPARAMS._serialized_end=5826
   _FEATUREPUBLISHOFFLINESTORECONFIG._serialized_start=5829
   _FEATUREPUBLISHOFFLINESTORECONFIG._serialized_end=5989
   _NEWMATERIALIZATIONPARAMS._serialized_start=5992
-  _NEWMATERIALIZATIONPARAMS._serialized_end=7755
-  _ONLINESTOREPARAMS._serialized_start=7758
-  _ONLINESTOREPARAMS._serialized_end=8027
-  _DYNAMODBONLINESTORE._serialized_start=8030
-  _DYNAMODBONLINESTORE._serialized_end=8319
-  _REDISONLINESTORE._serialized_start=8322
-  _REDISONLINESTORE._serialized_end=8557
-  _BIGTABLEONLINESTORE._serialized_start=8559
-  _BIGTABLEONLINESTORE._serialized_end=8670
-  _MONITORINGPARAMS._serialized_start=8673
-  _MONITORINGPARAMS._serialized_end=8947
-  _FEATUREVIEWENRICHMENTS._serialized_start=8950
-  _FEATUREVIEWENRICHMENTS._serialized_end=9083
-  _SNOWFLAKEDATA._serialized_start=9085
-  _SNOWFLAKEDATA._serialized_end=9148
-  _DATAQUALITYCONFIG._serialized_start=9151
-  _DATAQUALITYCONFIG._serialized_end=9280
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=9282
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=9394
-  _FEATUREVIEWCACHECONFIG._serialized_start=9397
-  _FEATUREVIEWCACHECONFIG._serialized_end=9671
+  _NEWMATERIALIZATIONPARAMS._serialized_end=7815
+  _ONLINESTOREPARAMS._serialized_start=7818
+  _ONLINESTOREPARAMS._serialized_end=8087
+  _DYNAMODBONLINESTORE._serialized_start=8090
+  _DYNAMODBONLINESTORE._serialized_end=8379
+  _REDISONLINESTORE._serialized_start=8382
+  _REDISONLINESTORE._serialized_end=8617
+  _BIGTABLEONLINESTORE._serialized_start=8619
+  _BIGTABLEONLINESTORE._serialized_end=8730
+  _MONITORINGPARAMS._serialized_start=8733
+  _MONITORINGPARAMS._serialized_end=9007
+  _FEATUREVIEWENRICHMENTS._serialized_start=9010
+  _FEATUREVIEWENRICHMENTS._serialized_end=9143
+  _SNOWFLAKEDATA._serialized_start=9145
+  _SNOWFLAKEDATA._serialized_end=9208
+  _DATAQUALITYCONFIG._serialized_start=9211
+  _DATAQUALITYCONFIG._serialized_end=9340
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=9342
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=9454
+  _FEATUREVIEWCACHECONFIG._serialized_start=9457
+  _FEATUREVIEWCACHECONFIG._serialized_end=9731
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.9.0rc1/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/materialization_roles_allowlists_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/materialization_roles_allowlists_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/onboarding_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/principal_group_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/serving_status_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/state_update_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/summary_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/transformation_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/user_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/data/workspace_pb2.py` & `tecton-0.9.0rc2/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.9.0rc2/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/dataobs/config_pb2.py` & `tecton-0.9.0rc2/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.9.0rc2/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.9.0rc2/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.9.0rc2/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.9.0rc2/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.9.0rc2/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.9.0rc2/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.9.0rc2/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.9.0rc2/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.9.0rc2/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/materialization/params_pb2.py` & `tecton-0.9.0rc2/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.9.0rc2/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.9.0rc2/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/offlinestore/delta/metadata_pb2.py` & `tecton-0.9.0rc2/tecton_proto/offlinestore/delta/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/offlinestore/delta/transaction_writer_pb2.py` & `tecton-0.9.0rc2/tecton_proto/offlinestore/delta/transaction_writer_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.9.0rc2/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.9.0rc2/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.9.0rc2/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/online_store_writer/copier_pb2.py` & `tecton-0.9.0rc2/tecton_proto/online_store_writer/copier_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/secrets/secrets_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/secrets/secrets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/snowflake/location_pb2.py` & `tecton-0.9.0rc2/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/snowflake/snowflake_credentials_pb2.py` & `tecton-0.9.0rc2/tecton_proto/snowflake/snowflake_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/spark_api/error_pb2.py` & `tecton-0.9.0rc2/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.9.0rc2/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.9.0rc2/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.9.0rc2/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/testhelperservice/test_helper_service_pb2.py` & `tecton-0.9.0rc2/tecton_proto/testhelperservice/test_helper_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_proto/validation/validator_pb2.py` & `tecton-0.9.0rc2/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/pipeline_helper.py` & `tecton-0.9.0rc2/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/query/aggregation_plans.py` & `tecton-0.9.0rc2/tecton_snowflake/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/query/dataframe_helper.py` & `tecton-0.9.0rc2/tecton_snowflake/query/dataframe_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/query/nodes.py` & `tecton-0.9.0rc2/tecton_snowflake/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/query/queries.py` & `tecton-0.9.0rc2/tecton_snowflake/query/queries.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/query/rewrite.py` & `tecton-0.9.0rc2/tecton_snowflake/query/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/query/translate.py` & `tecton-0.9.0rc2/tecton_snowflake/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.9.0rc2/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.9.0rc2/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/sql_helper.py` & `tecton-0.9.0rc2/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/historical_features.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates/time_limit.sql` & `tecton-0.9.0rc2/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_snowflake/templates_utils.py` & `tecton-0.9.0rc2/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/__init__.py` & `tecton-0.9.0rc2/tecton_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/aggregation_plans.py` & `tecton-0.9.0rc2/tecton_spark/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/data_observability.py` & `tecton-0.9.0rc2/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/data_source_credentials.py` & `tecton-0.9.0rc2/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/data_source_helper.py` & `tecton-0.9.0rc2/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/feature_view_spark_utils.py` & `tecton-0.9.0rc2/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/jars/class_loader.py` & `tecton-0.9.0rc2/tecton_spark/jars/class_loader.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.9.0rc2/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/materialization_plan.py` & `tecton-0.9.0rc2/tecton_spark/materialization_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         return self.base_data_frame
 
     @property
     def online_store_data_frame(self) -> DataFrame:
         online_df = self.base_data_frame
 
         # batch online and offline df are slightly different
-        if not self._fd.compaction_enabled_for_materialization and self._fd.is_temporal and not online_df.isStreaming:
+        if not self._fd.batch_compaction_enabled and self._fd.is_temporal and not online_df.isStreaming:
             version = self._fd.get_feature_store_format_version
             batch_mat_schedule = convert_timedelta_for_version(self._fd.batch_materialization_schedule, version)
             online_df = self.base_data_frame.withColumn(
                 MATERIALIZED_RAW_DATA_END_TIME, functions.col(anchor_time()) + batch_mat_schedule
             ).drop(anchor_time())
         return online_df
```

### Comparing `tecton-0.9.0rc1/tecton_spark/offline_store.py` & `tecton-0.9.0rc2/tecton_spark/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/partial_aggregations.py` & `tecton-0.9.0rc2/tecton_spark/partial_aggregations.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     time_aggregation: TrailingTimeWindowAggregation,
     version: int,
     view_schema: Schema,
     window_start_column_name: Optional[str] = None,
     window_end_column_name: Optional[str] = None,
     convert_to_epoch: bool = True,
     aggregation_anchor_time: Optional[datetime] = None,
+    create_tiles: Optional[bool] = None,
 ) -> pyspark.sql.DataFrame:
     """Constructs a dataframe that performs partial aggregations on the input dataframe.
 
     Also removes the default window column that is generated, and replaces it with a start time column, and optionally
     an end time column.
 
     If the time aggregation is continuous, no aggregations will be performed. Instead, a start time column will be added
@@ -103,14 +104,16 @@
         time_aggregation: The set of partial aggregations to be performed.
         version: The feature store version.
         window_start_column_name: If specified, the name of the start time column; otherwise it will use the default value "_anchor_time".
         window_end_column_name: If specified, the end time column will be included with this name.
         convert_to_epoch: If True, the window start and end times will be converted to epoch.
         aggregation_anchor_time: If specified, the offset for the aggregation windows.
         view_schema: The schema of the dataframe the partial aggregations are being performed for.
+        create_tiles: If set to True, the resulting dataframe will be tiled by the aggregation interval. If set to False, the resulting dataframe will have an anchor time column
+            that is just a copy of the input timestamp column. If set to None, the default behavior for the fv type will be used (ie continuous vs non-continuous).
 
     Returns:
         A dataframe with the partial aggregations. For example, if `user_id` is the only join key, there are two
         aggregations (min and max), `window_start_column_name` is `tile_start_time`, `window_end_column_name` is
         `tile_end_time`, and `convert_to_epoch` is `False`, then the resulting dataframe might look something like:
 
         +-------+------------+------------+-------------------+-------------------+
@@ -118,15 +121,17 @@
         +-------+------------+------------+-------------------+-------------------+
         |      1|           7|           9|2022-05-15 00:00:00|2022-05-16 00:00:00|
         |      2|          10|          12|2022-05-16 00:00:00|2022-05-17 00:00:00|
         |      1|          13|          13|2022-05-16 00:00:00|2022-05-17 00:00:00|
         +-------+------------+------------+-------------------+-------------------+
     """
     output_columns = set()
-    if not time_aggregation.is_continuous:
+    # If create_tiles is None, default to creating tiles whenever the fv is not using continuous mode
+    create_tiles = create_tiles if create_tiles is not None else not time_aggregation.is_continuous
+    if create_tiles:
         group_by_cols = [F.col(col) for col in group_by_columns]
         slide_str = f"{time_aggregation.aggregation_slide_period.seconds} seconds"
 
         anchor_time_offset_string = None
         if aggregation_anchor_time:
             # Compute the offset from the epoch such that anchor_time aligns to an interval boundary of size
             # aggregation_slide_period. i.e. `epoch + offset + (X * slide_period) = anchor_time`, where X is
@@ -210,15 +215,15 @@
         # Drop the original feature columns.
         for column in columns_to_drop:
             df = df.drop(column)
         output_df = df
 
     output_df = _convert_window_to_anchor_time(
         output_df,
-        time_aggregation.is_continuous,
+        not create_tiles,
         time_aggregation.time_key,
         version,
         window_start_column_name,
         window_end_column_name,
         convert_to_epoch,
     )
     # TOOD: TEC-12299 drop the `timestamp` column in m13n schema for continuous WAFV
```

### Comparing `tecton-0.9.0rc1/tecton_spark/pipeline_helper.py` & `tecton-0.9.0rc2/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/query/data_source.py` & `tecton-0.9.0rc2/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/query/filter.py` & `tecton-0.9.0rc2/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/query/join.py` & `tecton-0.9.0rc2/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/query/node.py` & `tecton-0.9.0rc2/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/query/pipeline.py` & `tecton-0.9.0rc2/tecton_spark/query/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,25 +96,27 @@
 @attrs.frozen
 class PartialAggSparkNode(SparkExecNode):
     input_node: SparkExecNode
     fdw: FeatureDefinitionWrapper = attrs.field()
     window_start_column_name: str
     window_end_column_name: Optional[str] = None
     aggregation_anchor_time: Optional[datetime] = None
+    create_tiles: Optional[bool] = None
 
     def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
         df = partial_aggregations.construct_partial_time_aggregation_df(
             self.input_node.to_dataframe(spark),
             self.fdw.partial_aggregate_group_by_columns,
             self.fdw.trailing_time_window_aggregation,
             self.fdw.get_feature_store_format_version,
             self.fdw.view_schema,
             window_start_column_name=self.window_start_column_name,
             window_end_column_name=self.window_end_column_name,
             aggregation_anchor_time=self.aggregation_anchor_time,
+            create_tiles=self.create_tiles,
         )
         return df
 
 
 @attrs.frozen
 class OnlinePartialAggSparkNodeV2(SparkExecNode):
     input_node: SparkExecNode
```

### Comparing `tecton-0.9.0rc1/tecton_spark/query/projection.py` & `tecton-0.9.0rc2/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/query/translate.py` & `tecton-0.9.0rc2/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/schema_derivation_utils.py` & `tecton-0.9.0rc2/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/schema_spark_utils.py` & `tecton-0.9.0rc2/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/spark_helper.py` & `tecton-0.9.0rc2/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/spark_schema_wrapper.py` & `tecton-0.9.0rc2/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/time_utils.py` & `tecton-0.9.0rc2/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc1/tecton_spark/udfs.py` & `tecton-0.9.0rc2/tecton_spark/udfs.py`

 * *Files identical despite different names*

