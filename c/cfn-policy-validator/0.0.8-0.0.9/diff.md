# Comparing `tmp/cfn-policy-validator-0.0.8.tar.gz` & `tmp/cfn-policy-validator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-policy-validator-0.0.8.tar", last modified: Thu Dec 16 20:43:37 2021, max compression
+gzip compressed data, was "cfn-policy-validator-0.0.9.tar", last modified: Wed Jan 19 20:28:16 2022, max compression
```

## Comparing `cfn-policy-validator-0.0.8.tar` & `cfn-policy-validator-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.086277 cfn-policy-validator-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16906 2021-12-16 20:43:37.086277 cfn-policy-validator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16043 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.082277 cfn-policy-validator-0.0.8/cfn_policy_validator/
--rw-r--r--   0 runner    (1001) docker     (121)     7945 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/application_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/argument_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.082277 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/cfn_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/cfn_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/common_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/schema_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     7899 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.082277 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/account_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/identity_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     6004 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.082277 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (121)     7489 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/lambda_aws.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.082277 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7499 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/arn_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/arn_generator_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)   133470 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/cfn_to_arn_map.json
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/cycle_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.086277 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/aws_no_value_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/aws_url_suffix_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/dynamic_ref_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_find_in_map_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4122 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_get_att_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_import_value_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_join_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_select_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_split_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_sub_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6049 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/ref_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6298 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/node_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7016 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/services_where_ref_returns_arn.json
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/topological_sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.086277 cfn-policy-validator-0.0.8/cfn_policy_validator/validation/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/validation/findings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5244 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/validation/reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)    13457 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/validation/validator.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/cfn_policy_validator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 20:43:37.082277 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16906 2021-12-16 20:43:37.000000 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2021-12-16 20:43:37.000000 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-16 20:43:37.000000 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-12-16 20:43:37.000000 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-16 20:43:37.000000 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-16 20:43:37.000000 cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-16 20:43:37.086277 cfn-policy-validator-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2021-12-16 20:43:26.000000 cfn-policy-validator-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.088938 cfn-policy-validator-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    17122 2022-01-19 20:28:16.088938 cfn-policy-validator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.084938 cfn-policy-validator-0.0.9/cfn_policy_validator/
+-rw-r--r--   0 runner    (1001) docker     (121)     7945 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/application_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/argument_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.084938 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/cfn_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/cfn_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/common_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/schema_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7899 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.084938 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/account_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/identity_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6004 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/output.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.084938 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7489 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/lambda_aws.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.088938 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7499 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/arn_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/arn_generator_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)   139409 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/cfn_to_arn_map.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/cycle_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.088938 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/aws_no_value_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/aws_url_suffix_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/dynamic_ref_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_find_in_map_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4122 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_get_att_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_import_value_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_join_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_select_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_split_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_sub_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6049 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/ref_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6304 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/node_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7016 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/services_where_ref_returns_arn.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/topological_sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.088938 cfn-policy-validator-0.0.9/cfn_policy_validator/validation/
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/validation/findings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/validation/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18998 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/validation/validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/cfn_policy_validator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 20:28:16.084938 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17122 2022-01-19 20:28:16.000000 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-01-19 20:28:16.000000 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-19 20:28:16.000000 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-01-19 20:28:16.000000 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-19 20:28:16.000000 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-19 20:28:16.000000 cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-19 20:28:16.088938 cfn-policy-validator-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-01-19 20:28:03.000000 cfn-policy-validator-0.0.9/setup.py
```

### Comparing `cfn-policy-validator-0.0.8/LICENSE` & `cfn-policy-validator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/PKG-INFO` & `cfn-policy-validator-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-policy-validator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parses IAM identity-based and resource-based policies from a CloudFormation template and runs them through IAM Access Analyzer checks.
 Home-page: https://github.com/awslabs/aws-cloudformation-iam-policy-validator
 Author: matluttr
 Author-email: matluttr@amazon.com
 License: MIT-0
 Keywords: cfn-policy-validator aws iam access-analyzer cloudformation
 Platform: UNKNOWN
@@ -124,14 +124,16 @@
 
 | CloudFormation Resource Type | Policy best practice checks | Access previews (check for external access) |
 | ---------------------------- | :----------------: | :-----------------------------------------: |
 | AWS::KMS::Key                | x                  | x |
 | AWS::Lambda::Permission      | x                  | |
 | AWS::Lambda::LayerVersionPermission | x           | |
 | AWS::S3::BucketPolicy        | x                  | x |
+| AWS::S3::AccessPoint         | x                  | x |
+| AWS::S3::MultiRegionAccessPoint | x | x |
 | AWS::SQS::QueuePolicy        | x                  | x |
 | AWS::SNS::TopicPolicy        | x                  | |
 | AWS::SecretsManager::ResourcePolicy | x           | |
 | AWS::IAM::Role (trust policy) | x | x |
 
 ### Intrinsic function and Pseudo parameter support
 
@@ -160,15 +162,15 @@
 
 Notes:
 - Fn::Transform (includes macros and AWS::Serverless/SAM transforms) not yet supported
 - References (Ref/GetAtt) to CloudFormation modules are not yet supported
 
 ### Credentials
 
-The cfn-policy-validator uses boto3 to interact with your AWS environment. You can use one of the following methods to specify credentials:
+The cfn-policy-validator should be run using credentials from the AWS account that you plan to deploy the CloudFormation template to. The tool uses boto3 to interact with your AWS account. You can use one of the following methods to specify credentials:
 
 - Environment variables
 - Shared credential file (~/.aws/credentials)
 - AWS config file (~/.aws/config)
 - Assume Role provider
 - Instance metadata service on an Amazon EC2 instance that has an IAM role configured.
```

### Comparing `cfn-policy-validator-0.0.8/README.md` & `cfn-policy-validator-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 
 | CloudFormation Resource Type | Policy best practice checks | Access previews (check for external access) |
 | ---------------------------- | :----------------: | :-----------------------------------------: |
 | AWS::KMS::Key                | x                  | x |
 | AWS::Lambda::Permission      | x                  | |
 | AWS::Lambda::LayerVersionPermission | x           | |
 | AWS::S3::BucketPolicy        | x                  | x |
+| AWS::S3::AccessPoint         | x                  | x |
+| AWS::S3::MultiRegionAccessPoint | x | x |
 | AWS::SQS::QueuePolicy        | x                  | x |
 | AWS::SNS::TopicPolicy        | x                  | |
 | AWS::SecretsManager::ResourcePolicy | x           | |
 | AWS::IAM::Role (trust policy) | x | x |
 
 ### Intrinsic function and Pseudo parameter support
 
@@ -139,15 +141,15 @@
 
 Notes:
 - Fn::Transform (includes macros and AWS::Serverless/SAM transforms) not yet supported
 - References (Ref/GetAtt) to CloudFormation modules are not yet supported
 
 ### Credentials
 
-The cfn-policy-validator uses boto3 to interact with your AWS environment. You can use one of the following methods to specify credentials:
+The cfn-policy-validator should be run using credentials from the AWS account that you plan to deploy the CloudFormation template to. The tool uses boto3 to interact with your AWS account. You can use one of the following methods to specify credentials:
 
 - Environment variables
 - Shared credential file (~/.aws/credentials)
 - AWS config file (~/.aws/config)
 - Assume Role provider
 - Instance metadata service on an Amazon EC2 instance that has an IAM role configured.
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/__init__.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/argument_actions.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/argument_actions.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/cfn_loader.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/cfn_loader.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/cfn_object.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/cfn_object.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/regex_patterns.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/schema_validator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/schema_validator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/cfn_tools/yaml_loader.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/cfn_tools/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/client.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/client.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/logger.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/logger.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/main.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/main.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parameters.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parameters.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/identity.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/identity.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/identity_schemas.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/identity_schemas.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/output.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/output.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/kms.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/kms.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/lambda_aws.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/lambda_aws.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/parser.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 SPDX-License-Identifier: MIT-0
 """
 import logging
 
 from cfn_policy_validator.parsers.resource.kms import KmsKeyPolicyParser
-from cfn_policy_validator.parsers.resource.s3 import S3BucketPolicyParser
+from cfn_policy_validator.parsers.resource.s3 import S3BucketPolicyParser, S3AccessPointPolicyParser, \
+    S3MultiRegionAccessPointPolicyParser
 from cfn_policy_validator.parsers.resource.sns import SnsTopicPolicyParser
 from cfn_policy_validator.parsers.resource.sqs import SqsQueuePolicyParser
 from cfn_policy_validator.parsers.resource.lambda_aws import LambdaPermissionPolicyParser, LambdaLayerVersionPermissionParser
 from cfn_policy_validator.parsers.resource.secrets_manager import SecretsManagerPolicyParser
 
 from cfn_policy_validator.parsers.utils.topological_sorter import TopologicalSorter
 
@@ -26,14 +27,16 @@
     @classmethod
     def parse(cls, template, account_config):
         # topologically sort which allows us to process dependent resources first
         sorter = TopologicalSorter(template)
         sorted_resources = sorter.sort_resources()
 
         parsers = {
+            'AWS::S3::AccessPoint': S3AccessPointPolicyParser(),
+            'AWS::S3::MultiRegionAccessPointPolicy': S3MultiRegionAccessPointPolicyParser(),
             'AWS::S3::BucketPolicy': S3BucketPolicyParser(),
             'AWS::SQS::QueuePolicy': SqsQueuePolicyParser(),
             'AWS::SNS::TopicPolicy': SnsTopicPolicyParser(),
             'AWS::KMS::Key': KmsKeyPolicyParser(),
             'AWS::Lambda::Permission': LambdaPermissionPolicyParser(account_config),
             'AWS::Lambda::LayerVersionPermission': LambdaLayerVersionPermissionParser(account_config.partition),
             'AWS::SecretsManager::ResourcePolicy': SecretsManagerPolicyParser()
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/s3.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/s3.py`

 * *Files 25% similar despite different names*

```diff
@@ -41,8 +41,94 @@
                     'type': 'object'
                 }
             },
             'required': ['Bucket', 'PolicyDocument']
         }
     },
     'required': ['Properties']
-}
+}
+
+
+class S3AccessPointPolicyParser:
+    """ AWS::S3::AccessPoint
+    """
+
+    def __init__(self):
+        self.access_point_policies = []
+
+    def parse(self, resource_name, resource):
+        evaluated_resource = resource.eval(access_point_policy_schema)
+        properties = evaluated_resource['Properties']
+
+        access_point_name = properties.get('Name', resource_name)
+        policy_document = properties['Policy']
+
+        policy = Policy('AccessPointPolicy', policy_document)
+        resource = Resource(access_point_name, 'AWS::S3::AccessPoint', policy)
+
+        self.access_point_policies.append(resource)
+
+    def get_policies(self):
+        return self.access_point_policies
+
+
+access_point_policy_schema = {
+    'type': 'object',
+    'properties': {
+        'Properties': {
+            'type': 'object',
+            'properties': {
+                'Name': {
+                    'type': 'string'
+                },
+                'Policy': {
+                    'type': 'object'
+                }
+            },
+            'required': ['Policy']
+        }
+    },
+    'required': ['Properties']
+}
+
+
+class S3MultiRegionAccessPointPolicyParser:
+    """ AWS::S3::MultiRegionAccessPointPolicy
+    """
+
+    def __init__(self):
+        self.multi_region_access_point_policies = []
+
+    def parse(self, _, resource):
+        evaluated_resource = resource.eval(multi_region_access_point_policy_schema)
+        properties = evaluated_resource['Properties']
+
+        mrap_name = properties['MrapName']
+        policy = properties['Policy']
+
+        policy_document = Policy('MultiRegionAccessPointPolicy', policy)
+        resource = Resource(mrap_name, 'AWS::S3::MultiRegionAccessPoint', policy_document)
+
+        self.multi_region_access_point_policies.append(resource)
+
+    def get_policies(self):
+        return self.multi_region_access_point_policies
+
+
+multi_region_access_point_policy_schema = {
+    'type': 'object',
+    'properties': {
+        'Properties': {
+            'type': 'object',
+            'properties': {
+                'MrapName': {
+                    'type': 'string'
+                },
+                'Policy': {
+                    'type': 'object'
+                }
+            },
+            'required': ['MrapName', 'Policy']
+        }
+    },
+    'required': ['Properties']
+}
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/secrets_manager.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/secrets_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         policy_document = properties['ResourcePolicy']
         secret_arn = properties['SecretId']
 
         try:
             secret_name = secret_arn.split("secret:", 1)[1]
         except IndexError:
-            raise ApplicationError(f'Invalid value for {properties.ancestors_as_string()}.SecretId. Must be a valid Secret ARN. SecretId value: {secret_arn}')
+            raise ApplicationError(f'Invalid value for {resource.ancestors_as_string()}.Properties.SecretId. Must be a valid Secret ARN. SecretId value: {secret_arn}')
 
         policy = Policy('ResourcePolicy', policy_document)
         resource = Resource(secret_name, 'AWS::SecretsManager::Secret', policy)
 
         self.policies.append(resource)
 
     def get_policies(self):
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/sns.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/sns.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/resource/sqs.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/arn_generator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/arn_generator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/arn_generator_schemas.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/arn_generator_schemas.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/cfn_to_arn_map.json` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/cfn_to_arn_map.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971902557319224%*

 * *Differences: {"'EC2'": "{'IPAM': {'Arn': {replace: OrderedDict([('Value', "*

 * *          "'arn:${Partition}:ec2::${Account}:ipam/${IpamId}'), ('ServicePrefix', 'ec2'), "*

 * *          "('ResourceType', 'ipam')])}}, 'IPAMPool': {'Arn': {replace: OrderedDict([('Value', "*

 * *          "'arn:${Partition}:ec2::${Account}:ipam-pool/${IpamPoolId}'), ('ServicePrefix', 'ec2'), "*

 * *          "('ResourceType', 'ipam-pool')])}, 'IpamScopeArn': {replace: OrderedDict([('Value', "*

 * *          "'arn:${Partition}:ec2::${Account}:ipam-scope/${IpamScop […]*

```diff
@@ -895,24 +895,62 @@
                 "ServicePrefix": "dynamodb",
                 "Value": "arn:${Partition}:dynamodb:${Region}:${Account}:table/${TableName}/stream/${StreamLabel}"
             }
         }
     },
     "EC2": {
         "IPAM": {
-            "Arn": null
+            "Arn": {
+                "ResourceType": "ipam",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2::${Account}:ipam/${IpamId}"
+            }
         },
         "IPAMPool": {
-            "Arn": null,
-            "IpamArn": null,
-            "IpamScopeArn": null
+            "Arn": {
+                "ResourceType": "ipam-pool",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2::${Account}:ipam-pool/${IpamPoolId}"
+            },
+            "IpamArn": {
+                "ResourceType": "ipam",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2::${Account}:ipam/${IpamId}"
+            },
+            "IpamScopeArn": {
+                "ResourceType": "ipam-scope",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2::${Account}:ipam-scope/${IpamScopeId}"
+            }
         },
         "IPAMScope": {
-            "Arn": null,
-            "IpamArn": null
+            "Arn": {
+                "ResourceType": "ipam-scope",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2::${Account}:ipam-scope/${IpamScopeId}"
+            },
+            "IpamArn": {
+                "ResourceType": "ipam",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2::${Account}:ipam/${IpamId}"
+            }
+        },
+        "NetworkInsightsAccessScope": {
+            "NetworkInsightsAccessScopeArn": {
+                "ResourceType": "network-insights-access-scope",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2:${Region}:${Account}:network-insights-access-scope/${NetworkInsightsAccessScopeId}"
+            }
+        },
+        "NetworkInsightsAccessScopeAnalysis": {
+            "NetworkInsightsAccessScopeAnalysisArn": {
+                "ResourceType": "network-insights-access-scope-analysis",
+                "ServicePrefix": "ec2",
+                "Value": "arn:${Partition}:ec2:${Region}:${Account}:network-insights-access-scope-analysis/${NetworkInsightsAccessScopeAnalysisId}"
+            }
         },
         "NetworkInsightsAnalysis": {
             "NetworkInsightsAnalysisArn": {
                 "ResourceType": "network-insights-analysis",
                 "ServicePrefix": "ec2",
                 "Value": "arn:${Partition}:ec2:${Region}:${Account}:network-insights-analysis/${NetworkInsightsAnalysisId}"
             }
@@ -1285,14 +1323,30 @@
             "EnvironmentArn": {
                 "ResourceType": "environment",
                 "ServicePrefix": "finspace",
                 "Value": "arn:${Partition}:finspace:${Region}:${Account}:environment/${environmentId}"
             }
         }
     },
+    "Forecast": {
+        "Dataset": {
+            "Arn": {
+                "ResourceType": "dataset",
+                "ServicePrefix": "forecast",
+                "Value": "arn:${Partition}:forecast:${Region}:${Account}:dataset/${ResourceId}"
+            }
+        },
+        "DatasetGroup": {
+            "DatasetGroupArn": {
+                "ResourceType": "dataset-group",
+                "ServicePrefix": "forecast",
+                "Value": "arn:${Partition}:forecast:${Region}:${Account}:dataset-group/${ResourceId}"
+            }
+        }
+    },
     "FraudDetector": {
         "Detector": {
             "Arn": {
                 "ResourceType": "detector",
                 "ServicePrefix": "frauddetector",
                 "Value": "arn:${Partition}:frauddetector:${Region}:${Account}:detector/${ResourcePath}"
             },
@@ -1848,14 +1902,28 @@
             "Ref": null
         },
         "ResourceGroup": {
             "Arn": null,
             "Ref": null
         }
     },
+    "InspectorV2": {
+        "Filter": {
+            "Arn": {
+                "ResourceType": "filter",
+                "ServicePrefix": "inspector2",
+                "Value": "arn:${Partition}:inspector2:${Region}:${Account}:owner/${OwnerId}/filter/${FilterId}"
+            },
+            "Ref": {
+                "ResourceType": "filter",
+                "ServicePrefix": "inspector2",
+                "Value": "arn:${Partition}:inspector2:${Region}:${Account}:owner/${OwnerId}/filter/${FilterId}"
+            }
+        }
+    },
     "IoT": {
         "Authorizer": {
             "Arn": {
                 "ResourceType": "authorizer",
                 "ServicePrefix": "iot",
                 "Value": "arn:${Partition}:iot:${Region}:${Account}:authorizer/${AuthorizerName}"
             }
@@ -2035,14 +2103,30 @@
             "Arn": {
                 "ResourceType": "deliverystream",
                 "ServicePrefix": "firehose",
                 "Value": "arn:${Partition}:firehose:${Region}:${Account}:deliverystream/${DeliveryStreamName}"
             }
         }
     },
+    "KinesisVideo": {
+        "SignalingChannel": {
+            "Arn": {
+                "ResourceType": "channel",
+                "ServicePrefix": "kinesisvideo",
+                "Value": "arn:${Partition}:kinesisvideo:${Region}:${Account}:channel/${ChannelName}/${CreationTime}"
+            }
+        },
+        "Stream": {
+            "Arn": {
+                "ResourceType": "stream",
+                "ServicePrefix": "kinesisvideo",
+                "Value": "arn:${Partition}:kinesisvideo:${Region}:${Account}:stream/${StreamName}/${CreationTime}"
+            }
+        }
+    },
     "Lambda": {
         "Alias": {
             "Ref": {
                 "ResourceType": "functionalias",
                 "ServicePrefix": "lambda",
                 "Value": "arn:${Partition}:lambda:${Region}:${Account}:function:${FunctionName}:${Alias}"
             }
@@ -2092,14 +2176,28 @@
                 "ResourceType": "license",
                 "ServicePrefix": "license-manager",
                 "Value": "arn:${Partition}:license-manager::${Account}:license:${LicenseId}"
             }
         }
     },
     "Lightsail": {
+        "Alarm": {
+            "AlarmArn": {
+                "ResourceType": "alarm",
+                "ServicePrefix": "lightsail",
+                "Value": "arn:${Partition}:lightsail:${Region}:${Account}:Alarm/${Id}"
+            }
+        },
+        "Bucket": {
+            "BucketArn": {
+                "ResourceType": "bucket",
+                "ServicePrefix": "lightsail",
+                "Value": "arn:${Partition}:lightsail:${Region}:${Account}:Bucket/${Id}"
+            }
+        },
         "Database": {
             "DatabaseArn": {
                 "ResourceType": "relational-database",
                 "ServicePrefix": "lightsail",
                 "Value": "arn:${Partition}:lightsail:${Region}:${Account}:RelationalDatabase/${Id}"
             }
         },
@@ -2113,14 +2211,28 @@
         "Instance": {
             "InstanceArn": {
                 "ResourceType": "instance",
                 "ServicePrefix": "lightsail",
                 "Value": "arn:${Partition}:lightsail:${Region}:${Account}:Instance/${Id}"
             }
         },
+        "LoadBalancer": {
+            "LoadBalancerArn": {
+                "ResourceType": "load-balancer",
+                "ServicePrefix": "lightsail",
+                "Value": "arn:${Partition}:lightsail:${Region}:${Account}:LoadBalancer/${Id}"
+            }
+        },
+        "LoadBalancerTlsCertificate": {
+            "LoadBalancerTlsCertificateArn": {
+                "ResourceType": "load-balancer-tls-certificate",
+                "ServicePrefix": "lightsail",
+                "Value": "arn:${Partition}:lightsail:${Region}:${Account}:LoadBalancerTlsCertificate/${Id}"
+            }
+        },
         "StaticIp": {
             "StaticIpArn": {
                 "ResourceType": "static-ip",
                 "ServicePrefix": "lightsail",
                 "Value": "arn:${Partition}:lightsail:${Region}:${Account}:StaticIp/${Id}"
             }
         }
@@ -2132,63 +2244,95 @@
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:geofence-collection/${GeofenceCollectionName}"
             },
             "CollectionArn": {
                 "ResourceType": "geofence-collection",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:geofence-collection/${GeofenceCollectionName}"
+            },
+            "Ref": {
+                "ResourceType": "geofence-collection",
+                "ServicePrefix": "geo",
+                "Value": "arn:${Partition}:geo:${Region}:${Account}:geofence-collection/${GeofenceCollectionName}"
             }
         },
         "Map": {
             "Arn": {
                 "ResourceType": "map",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:map/${MapName}"
             },
             "MapArn": {
                 "ResourceType": "map",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:map/${MapName}"
+            },
+            "Ref": {
+                "ResourceType": "map",
+                "ServicePrefix": "geo",
+                "Value": "arn:${Partition}:geo:${Region}:${Account}:map/${MapName}"
             }
         },
         "PlaceIndex": {
             "Arn": {
                 "ResourceType": "place-index",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:place-index/${IndexName}"
             },
             "IndexArn": {
                 "ResourceType": "place-index",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:place-index/${IndexName}"
+            },
+            "Ref": {
+                "ResourceType": "place-index",
+                "ServicePrefix": "geo",
+                "Value": "arn:${Partition}:geo:${Region}:${Account}:place-index/${IndexName}"
             }
         },
         "RouteCalculator": {
             "Arn": {
                 "ResourceType": "route-calculator",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:route-calculator/${CalculatorName}"
             },
             "CalculatorArn": {
                 "ResourceType": "route-calculator",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:route-calculator/${CalculatorName}"
+            },
+            "Ref": {
+                "ResourceType": "route-calculator",
+                "ServicePrefix": "geo",
+                "Value": "arn:${Partition}:geo:${Region}:${Account}:route-calculator/${CalculatorName}"
             }
         },
         "Tracker": {
             "Arn": {
                 "ResourceType": "tracker",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:tracker/${TrackerName}"
             },
+            "Ref": {
+                "ResourceType": "tracker",
+                "ServicePrefix": "geo",
+                "Value": "arn:${Partition}:geo:${Region}:${Account}:tracker/${TrackerName}"
+            },
             "TrackerArn": {
                 "ResourceType": "tracker",
                 "ServicePrefix": "geo",
                 "Value": "arn:${Partition}:geo:${Region}:${Account}:tracker/${TrackerName}"
             }
+        },
+        "TrackerConsumer": {
+            "Ref": {
+                "ResourceType": "geofence-collection",
+                "ServicePrefix": "geo",
+                "Value": "arn:${Partition}:geo:${Region}:${Account}:geofence-collection/${GeofenceCollectionName}"
+            }
         }
     },
     "Logs": {
         "Destination": {
             "Arn": {
                 "ResourceType": "destination",
                 "ServicePrefix": "logs",
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/cycle_detection.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/cycle_detection.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/aws_no_value_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/aws_no_value_evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class AwsNoValueEvaluator:
 	"""
 	Removes any references to NoValue from the evaluated output.  If a dictionary key has a NoValue reference, the key
 	is also removed.
 	"""
 	def evaluate(self, value):
-		if isinstance(value, CfnObject):
+		if isinstance(value, dict):
 			for key in list(value.keys()):
 				child_value = value[key]
 				if isinstance(child_value, NoValue):
 					del value[key]
 				else:
 					self.evaluate(child_value)
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/dynamic_ref_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/dynamic_ref_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_find_in_map_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_find_in_map_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_get_att_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_get_att_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_import_value_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_import_value_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_join_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_join_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_select_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_select_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_split_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_split_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_sub_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/fn_sub_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/intrinsic_functions/ref_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/intrinsic_functions/ref_evaluator.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/node_evaluator.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/node_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,11 +115,11 @@
                         continue
 
                 # when passing the list of visited values to child evals, create a separate copy for each so
                 # that they don't share the same visited references
                 copy_of_visited_values = copy.deepcopy(visited_values)
                 value[key] = self.eval(value[key], resource_properties_to_eval, copy_of_visited_values)
 
-            return value
+            return dict(value)
 
         else:
             return value
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/services_where_ref_returns_arn.json` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/services_where_ref_returns_arn.json`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/parsers/utils/topological_sorter.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/parsers/utils/topological_sorter.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/validation/findings.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/validation/findings.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator/validation/reporter.py` & `cfn-policy-validator-0.0.9/cfn_policy_validator/validation/reporter.py`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/PKG-INFO` & `cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-policy-validator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parses IAM identity-based and resource-based policies from a CloudFormation template and runs them through IAM Access Analyzer checks.
 Home-page: https://github.com/awslabs/aws-cloudformation-iam-policy-validator
 Author: matluttr
 Author-email: matluttr@amazon.com
 License: MIT-0
 Keywords: cfn-policy-validator aws iam access-analyzer cloudformation
 Platform: UNKNOWN
@@ -124,14 +124,16 @@
 
 | CloudFormation Resource Type | Policy best practice checks | Access previews (check for external access) |
 | ---------------------------- | :----------------: | :-----------------------------------------: |
 | AWS::KMS::Key                | x                  | x |
 | AWS::Lambda::Permission      | x                  | |
 | AWS::Lambda::LayerVersionPermission | x           | |
 | AWS::S3::BucketPolicy        | x                  | x |
+| AWS::S3::AccessPoint         | x                  | x |
+| AWS::S3::MultiRegionAccessPoint | x | x |
 | AWS::SQS::QueuePolicy        | x                  | x |
 | AWS::SNS::TopicPolicy        | x                  | |
 | AWS::SecretsManager::ResourcePolicy | x           | |
 | AWS::IAM::Role (trust policy) | x | x |
 
 ### Intrinsic function and Pseudo parameter support
 
@@ -160,15 +162,15 @@
 
 Notes:
 - Fn::Transform (includes macros and AWS::Serverless/SAM transforms) not yet supported
 - References (Ref/GetAtt) to CloudFormation modules are not yet supported
 
 ### Credentials
 
-The cfn-policy-validator uses boto3 to interact with your AWS environment. You can use one of the following methods to specify credentials:
+The cfn-policy-validator should be run using credentials from the AWS account that you plan to deploy the CloudFormation template to. The tool uses boto3 to interact with your AWS account. You can use one of the following methods to specify credentials:
 
 - Environment variables
 - Shared credential file (~/.aws/credentials)
 - AWS config file (~/.aws/config)
 - Assume Role provider
 - Instance metadata service on an Amazon EC2 instance that has an IAM role configured.
```

### Comparing `cfn-policy-validator-0.0.8/cfn_policy_validator.egg-info/SOURCES.txt` & `cfn-policy-validator-0.0.9/cfn_policy_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfn-policy-validator-0.0.8/setup.py` & `cfn-policy-validator-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     ],
     entry_points={"console_scripts": "cfn-policy-validator=cfn_policy_validator.main:main"},
     python_requires='>=3.6',
     package_data={
         '': ['*.json']
     },
     install_requires=[
-        'boto3>=1.17',
+        'boto3>=1.20',
         'pyYAML>=5.3',
         'urllib3>=1.25',
         'jsonschema~=3.2'
     ]
 )
```

