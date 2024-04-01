# Comparing `tmp/google-cloud-bigquery-3.8.0.tar.gz` & `tmp/google-cloud-bigquery-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-3.8.0.tar", last modified: Mon Mar 27 14:08:40 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-3.9.0.tar", last modified: Tue Mar 28 16:33:35 2023, max compression
```

## Comparing `google-cloud-bigquery-3.8.0.tar` & `google-cloud-bigquery-3.9.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.537762 google-cloud-bigquery-3.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5828 2023-03-27 14:08:40.537762 google-cloud-bigquery-3.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4718 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.509763 google-cloud-bigquery-3.8.0/google/
--rw-rw-r--   0 root         (0)     1003      790 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.509763 google-cloud-bigquery-3.8.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      790 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.513763 google-cloud-bigquery-3.8.0/google/cloud/bigquery/
--rw-rw-r--   0 root         (0)     1003     7865 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003    31709 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/_helpers.py
--rw-rw-r--   0 root         (0)     1003     2039 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/_http.py
--rw-rw-r--   0 root         (0)     1003     9457 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/_job_helpers.py
--rw-rw-r--   0 root         (0)     1003    35944 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/_pandas_helpers.py
--rw-rw-r--   0 root         (0)     1003     4542 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/_tqdm_helpers.py
--rw-rw-r--   0 root         (0)     1003   160137 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/client.py
--rw-rw-r--   0 root         (0)     1003    31331 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dataset.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.513763 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/
--rw-rw-r--   0 root         (0)     1003     2980 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/__init__.py
--rw-rw-r--   0 root         (0)     1003    17000 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/_helpers.py
--rw-rw-r--   0 root         (0)     1003     4476 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/connection.py
--rw-rw-r--   0 root         (0)     1003    19796 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/cursor.py
--rw-rw-r--   0 root         (0)     1003     1685 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/exceptions.py
--rw-rw-r--   0 root         (0)     1003     2769 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/types.py
--rw-rw-r--   0 root         (0)     1003     2635 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/encryption_configuration.py
--rw-rw-r--   0 root         (0)     1003     9750 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/enums.py
--rw-rw-r--   0 root         (0)     1003      954 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/exceptions.py
--rw-rw-r--   0 root         (0)     1003    33949 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/external_config.py
--rw-rw-r--   0 root         (0)     1003     4402 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/format_options.py
--rw-rw-r--   0 root         (0)     1003     1554 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/iam.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.513763 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/
--rw-rw-r--   0 root         (0)     1003     3270 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/__init__.py
--rw-rw-r--   0 root         (0)     1003    35713 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/base.py
--rw-rw-r--   0 root         (0)     1003    10125 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/copy_.py
--rw-rw-r--   0 root         (0)     1003     9573 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/extract.py
--rw-rw-r--   0 root         (0)     1003    32445 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/load.py
--rw-rw-r--   0 root         (0)     1003    80201 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/query.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.513763 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/
--rw-rw-r--   0 root         (0)     1003      775 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.517762 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/
--rw-rw-r--   0 root         (0)     1003     1252 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/__init__.py
--rw-rw-r--   0 root         (0)     1003      779 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/exceptions.py
--rw-rw-r--   0 root         (0)     1003     7948 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/lexer.py
--rw-rw-r--   0 root         (0)     1003    15999 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/parser.py
--rw-rw-r--   0 root         (0)     1003     5151 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/visitors.py
--rw-rw-r--   0 root         (0)     1003    28101 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/magics.py
--rw-rw-r--   0 root         (0)     1003    14826 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/model.py
--rw-rw-r--   0 root         (0)     1003     4848 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/py.typed
--rw-rw-r--   0 root         (0)     1003    34707 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/query.py
--rw-rw-r--   0 root         (0)     1003     2621 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/retry.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.517762 google-cloud-bigquery-3.8.0/google/cloud/bigquery/routine/
--rw-rw-r--   0 root         (0)     1003     1037 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/routine/__init__.py
--rw-rw-r--   0 root         (0)     1003    18466 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/routine/routine.py
--rw-rw-r--   0 root         (0)     1003    18603 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/schema.py
--rw-rw-r--   0 root         (0)     1003    12081 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/standard_sql.py
--rw-rw-r--   0 root         (0)     1003   104940 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/table.py
--rw-rw-r--   0 root         (0)     1003      597 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.517762 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/
--rw-rw-r--   0 root         (0)     1003     1782 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.517762 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/
--rw-rw-r--   0 root         (0)     1003     1385 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1399 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/encryption_config.py
--rw-rw-r--   0 root         (0)     1003    75103 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/model.py
--rw-rw-r--   0 root         (0)     1003     1539 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/model_reference.py
--rw-rw-r--   0 root         (0)     1003     4428 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/standard_sql.py
--rw-rw-r--   0 root         (0)     1003     2509 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/table_reference.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.517762 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/
--rw-r--r--   0 root         (0)     1003     5828 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4953 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003     1351 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:08:40.000000 google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003      238 2023-03-27 14:08:40.537762 google-cloud-bigquery-3.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     5239 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.517762 google-cloud-bigquery-3.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.521762 google-cloud-bigquery-3.8.0/tests/data/
--rw-rw-r--   0 root         (0)     1003     4306 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/characters.json
--rw-rw-r--   0 root         (0)     1003     3546 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/characters.jsonl
--rw-rw-r--   0 root         (0)     1003      308 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/colors.avro
--rw-rw-r--   0 root         (0)     1003      307 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/numeric_38_12.parquet
--rw-rw-r--   0 root         (0)     1003       55 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/people.csv
--rw-rw-r--   0 root         (0)     1003      745 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/scalars.jsonl
--rw-rw-r--   0 root         (0)     1003     2206 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/scalars_extreme.jsonl
--rw-rw-r--   0 root         (0)     1003     1141 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/scalars_schema.json
--rw-rw-r--   0 root         (0)     1003     2027 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/data/schema.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/scrub_datasets.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.521762 google-cloud-bigquery-3.8.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      575 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     5086 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003     3411 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/helpers.py
--rw-rw-r--   0 root         (0)     1003     6362 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_arrow.py
--rw-rw-r--   0 root         (0)     1003    97205 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_client.py
--rw-rw-r--   0 root         (0)     1003     2465 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_job_retry.py
--rw-rw-r--   0 root         (0)     1003     4455 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_list_rows.py
--rw-rw-r--   0 root         (0)     1003     2924 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_magics.py
--rw-rw-r--   0 root         (0)     1003    47476 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_pandas.py
--rw-rw-r--   0 root         (0)     1003    16388 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_query.py
--rw-rw-r--   0 root         (0)     1003      998 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/system/test_structs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.529762 google-cloud-bigquery-3.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.533762 google-cloud-bigquery-3.8.0/tests/unit/_helpers/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/_helpers/__init__.py
--rw-rw-r--   0 root         (0)     1003     5960 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/_helpers/test_from_json.py
--rw-rw-r--   0 root         (0)     1003     1486 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/conftest.py
--rw-rw-r--   0 root         (0)     1003     2391 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.533762 google-cloud-bigquery-3.8.0/tests/unit/job/
--rw-rw-r--   0 root         (0)     1003      574 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/__init__.py
--rw-rw-r--   0 root         (0)     1003     6046 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/helpers.py
--rw-rw-r--   0 root         (0)     1003    43583 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_base.py
--rw-rw-r--   0 root         (0)     1003    20461 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_copy.py
--rw-rw-r--   0 root         (0)     1003    17397 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_extract.py
--rw-rw-r--   0 root         (0)     1003    35138 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_load.py
--rw-rw-r--   0 root         (0)     1003    32315 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_load_config.py
--rw-rw-r--   0 root         (0)     1003    81646 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_query.py
--rw-rw-r--   0 root         (0)     1003    12758 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_query_config.py
--rw-rw-r--   0 root         (0)     1003    37499 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_query_pandas.py
--rw-rw-r--   0 root         (0)     1003    15882 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/job/test_query_stats.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.533762 google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/
--rw-rw-r--   0 root         (0)     1003      574 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/__init__.py
--rw-rw-r--   0 root         (0)     1003     1073 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/test_lexer.py
--rw-rw-r--   0 root         (0)     1003     7546 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/test_parser.py
--rw-rw-r--   0 root         (0)     1003     1075 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/test_visitors.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.537762 google-cloud-bigquery-3.8.0/tests/unit/model/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/model/__init__.py
--rw-rw-r--   0 root         (0)     1003    14162 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/model/test_model.py
--rw-rw-r--   0 root         (0)     1003     4413 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/model/test_model_reference.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:08:40.537762 google-cloud-bigquery-3.8.0/tests/unit/routine/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/routine/__init__.py
--rw-rw-r--   0 root         (0)     1003    18313 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/routine/test_routine.py
--rw-rw-r--   0 root         (0)     1003     3088 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/routine/test_routine_argument.py
--rw-rw-r--   0 root         (0)     1003     4509 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/routine/test_routine_reference.py
--rw-rw-r--   0 root         (0)     1003    48444 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test__helpers.py
--rw-rw-r--   0 root         (0)     1003     5927 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test__http.py
--rw-rw-r--   0 root         (0)     1003    11322 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test__job_helpers.py
--rw-rw-r--   0 root         (0)     1003    68599 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test__pandas_helpers.py
--rw-rw-r--   0 root         (0)     1003   347092 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003    12326 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_create_dataset.py
--rw-rw-r--   0 root         (0)     1003    40670 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_dataset.py
--rw-rw-r--   0 root         (0)     1003    26678 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_dbapi__helpers.py
--rw-rw-r--   0 root         (0)     1003     8884 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_dbapi_connection.py
--rw-rw-r--   0 root         (0)     1003    31145 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_dbapi_cursor.py
--rw-rw-r--   0 root         (0)     1003     2039 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_dbapi_types.py
--rw-rw-r--   0 root         (0)     1003     2798 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_delete_dataset.py
--rw-rw-r--   0 root         (0)     1003     4433 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_encryption_configuration.py
--rw-rw-r--   0 root         (0)     1003    33532 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_external_config.py
--rw-rw-r--   0 root         (0)     1003     2124 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_format_options.py
--rw-rw-r--   0 root         (0)     1003     8550 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_job_retry.py
--rw-rw-r--   0 root         (0)     1003      985 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_legacy_types.py
--rw-rw-r--   0 root         (0)     1003     4104 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_list_datasets.py
--rw-rw-r--   0 root         (0)     1003     9475 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_list_jobs.py
--rw-rw-r--   0 root         (0)     1003     2970 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_list_models.py
--rw-rw-r--   0 root         (0)     1003     3822 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_list_projects.py
--rw-rw-r--   0 root         (0)     1003     3074 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_list_routines.py
--rw-rw-r--   0 root         (0)     1003     5826 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_list_tables.py
--rw-rw-r--   0 root         (0)     1003    74919 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_magics.py
--rw-rw-r--   0 root         (0)     1003     9718 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003    58111 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_query.py
--rw-rw-r--   0 root         (0)     1003     4306 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_retry.py
--rw-rw-r--   0 root         (0)     1003    36266 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_schema.py
--rw-rw-r--   0 root         (0)     1003     2054 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_signature_compatibility.py
--rw-rw-r--   0 root         (0)     1003    20124 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_standard_sql_types.py
--rw-rw-r--   0 root         (0)     1003   195640 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_table.py
--rw-rw-r--   0 root         (0)     1003     7665 2023-03-27 14:06:29.000000 google-cloud-bigquery-3.8.0/tests/unit/test_table_pandas.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.169806 google-cloud-bigquery-3.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5828 2023-03-28 16:33:35.169806 google-cloud-bigquery-3.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4718 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.141804 google-cloud-bigquery-3.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      790 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.141804 google-cloud-bigquery-3.9.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      790 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.145804 google-cloud-bigquery-3.9.0/google/cloud/bigquery/
+-rw-rw-r--   0 root         (0)     1003     7865 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003    31709 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     2039 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/_http.py
+-rw-rw-r--   0 root         (0)     1003     9457 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/_job_helpers.py
+-rw-rw-r--   0 root         (0)     1003    35972 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/_pandas_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4542 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/_tqdm_helpers.py
+-rw-rw-r--   0 root         (0)     1003   160137 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/client.py
+-rw-rw-r--   0 root         (0)     1003    31331 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dataset.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.149804 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/
+-rw-rw-r--   0 root         (0)     1003     2980 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17000 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4476 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/connection.py
+-rw-rw-r--   0 root         (0)     1003    20135 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/cursor.py
+-rw-rw-r--   0 root         (0)     1003     1685 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     2769 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/types.py
+-rw-rw-r--   0 root         (0)     1003     2635 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/encryption_configuration.py
+-rw-rw-r--   0 root         (0)     1003     9750 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/enums.py
+-rw-rw-r--   0 root         (0)     1003      954 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    33949 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/external_config.py
+-rw-rw-r--   0 root         (0)     1003     4402 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/format_options.py
+-rw-rw-r--   0 root         (0)     1003     1554 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/iam.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.149804 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/
+-rw-rw-r--   0 root         (0)     1003     3270 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35713 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/base.py
+-rw-rw-r--   0 root         (0)     1003    10125 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/copy_.py
+-rw-rw-r--   0 root         (0)     1003     9573 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/extract.py
+-rw-rw-r--   0 root         (0)     1003    32445 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/load.py
+-rw-rw-r--   0 root         (0)     1003    80201 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/query.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.149804 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/
+-rw-rw-r--   0 root         (0)     1003      775 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.149804 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/
+-rw-rw-r--   0 root         (0)     1003     1252 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/__init__.py
+-rw-rw-r--   0 root         (0)     1003      779 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     7948 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/lexer.py
+-rw-rw-r--   0 root         (0)     1003    15999 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/parser.py
+-rw-rw-r--   0 root         (0)     1003     5151 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/visitors.py
+-rw-rw-r--   0 root         (0)     1003    28101 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/magics.py
+-rw-rw-r--   0 root         (0)     1003    14826 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/model.py
+-rw-rw-r--   0 root         (0)     1003     4848 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/py.typed
+-rw-rw-r--   0 root         (0)     1003    34707 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/query.py
+-rw-rw-r--   0 root         (0)     1003     2621 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/retry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.149804 google-cloud-bigquery-3.9.0/google/cloud/bigquery/routine/
+-rw-rw-r--   0 root         (0)     1003     1037 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/routine/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18466 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/routine/routine.py
+-rw-rw-r--   0 root         (0)     1003    18603 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/schema.py
+-rw-rw-r--   0 root         (0)     1003    12081 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/standard_sql.py
+-rw-rw-r--   0 root         (0)     1003   104940 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/table.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.149804 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/
+-rw-rw-r--   0 root         (0)     1003     1782 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.153805 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1385 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1399 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/encryption_config.py
+-rw-rw-r--   0 root         (0)     1003    75103 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/model.py
+-rw-rw-r--   0 root         (0)     1003     1539 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/model_reference.py
+-rw-rw-r--   0 root         (0)     1003     4428 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/standard_sql.py
+-rw-rw-r--   0 root         (0)     1003     2509 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/table_reference.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.153805 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/
+-rw-r--r--   0 root         (0)     1003     5828 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4953 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003     1351 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-03-28 16:33:35.000000 google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003      238 2023-03-28 16:33:35.173806 google-cloud-bigquery-3.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     5239 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.153805 google-cloud-bigquery-3.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.153805 google-cloud-bigquery-3.9.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003     4306 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/characters.json
+-rw-rw-r--   0 root         (0)     1003     3546 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/characters.jsonl
+-rw-rw-r--   0 root         (0)     1003      308 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/colors.avro
+-rw-rw-r--   0 root         (0)     1003      307 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/numeric_38_12.parquet
+-rw-rw-r--   0 root         (0)     1003       55 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/people.csv
+-rw-rw-r--   0 root         (0)     1003      745 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/scalars.jsonl
+-rw-rw-r--   0 root         (0)     1003     2206 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/scalars_extreme.jsonl
+-rw-rw-r--   0 root         (0)     1003     1141 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/scalars_schema.json
+-rw-rw-r--   0 root         (0)     1003     2027 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/data/schema.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/scrub_datasets.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.157805 google-cloud-bigquery-3.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      575 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5086 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003     3411 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/helpers.py
+-rw-rw-r--   0 root         (0)     1003     6362 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_arrow.py
+-rw-rw-r--   0 root         (0)     1003    97205 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_client.py
+-rw-rw-r--   0 root         (0)     1003     2465 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_job_retry.py
+-rw-rw-r--   0 root         (0)     1003     4455 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_list_rows.py
+-rw-rw-r--   0 root         (0)     1003     2924 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_magics.py
+-rw-rw-r--   0 root         (0)     1003    47476 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003    16388 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_query.py
+-rw-rw-r--   0 root         (0)     1003      998 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/system/test_structs.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.165806 google-cloud-bigquery-3.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.165806 google-cloud-bigquery-3.9.0/tests/unit/_helpers/
+-rw-rw-r--   0 root         (0)     1003        0 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/_helpers/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5960 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/_helpers/test_from_json.py
+-rw-rw-r--   0 root         (0)     1003     1486 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/conftest.py
+-rw-rw-r--   0 root         (0)     1003     2391 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.169806 google-cloud-bigquery-3.9.0/tests/unit/job/
+-rw-rw-r--   0 root         (0)     1003      574 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6046 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/helpers.py
+-rw-rw-r--   0 root         (0)     1003    43583 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_base.py
+-rw-rw-r--   0 root         (0)     1003    20461 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_copy.py
+-rw-rw-r--   0 root         (0)     1003    17397 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_extract.py
+-rw-rw-r--   0 root         (0)     1003    35138 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_load.py
+-rw-rw-r--   0 root         (0)     1003    32315 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_load_config.py
+-rw-rw-r--   0 root         (0)     1003    81646 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_query.py
+-rw-rw-r--   0 root         (0)     1003    12758 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_query_config.py
+-rw-rw-r--   0 root         (0)     1003    37499 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_query_pandas.py
+-rw-rw-r--   0 root         (0)     1003    15882 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/job/test_query_stats.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.169806 google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/
+-rw-rw-r--   0 root         (0)     1003      574 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1073 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/test_lexer.py
+-rw-rw-r--   0 root         (0)     1003     7546 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/test_parser.py
+-rw-rw-r--   0 root         (0)     1003     1075 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/test_visitors.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.169806 google-cloud-bigquery-3.9.0/tests/unit/model/
+-rw-rw-r--   0 root         (0)     1003        0 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/model/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14162 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/model/test_model.py
+-rw-rw-r--   0 root         (0)     1003     4413 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/model/test_model_reference.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-28 16:33:35.169806 google-cloud-bigquery-3.9.0/tests/unit/routine/
+-rw-rw-r--   0 root         (0)     1003        0 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/routine/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18313 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/routine/test_routine.py
+-rw-rw-r--   0 root         (0)     1003     3088 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/routine/test_routine_argument.py
+-rw-rw-r--   0 root         (0)     1003     4509 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/routine/test_routine_reference.py
+-rw-rw-r--   0 root         (0)     1003    48444 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003     5927 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test__http.py
+-rw-rw-r--   0 root         (0)     1003    11322 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test__job_helpers.py
+-rw-rw-r--   0 root         (0)     1003    70630 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test__pandas_helpers.py
+-rw-rw-r--   0 root         (0)     1003   347092 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003    12326 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_create_dataset.py
+-rw-rw-r--   0 root         (0)     1003    40670 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_dataset.py
+-rw-rw-r--   0 root         (0)     1003    26678 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_dbapi__helpers.py
+-rw-rw-r--   0 root         (0)     1003     8884 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_dbapi_connection.py
+-rw-rw-r--   0 root         (0)     1003    31974 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_dbapi_cursor.py
+-rw-rw-r--   0 root         (0)     1003     2039 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_dbapi_types.py
+-rw-rw-r--   0 root         (0)     1003     2798 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_delete_dataset.py
+-rw-rw-r--   0 root         (0)     1003     4433 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_encryption_configuration.py
+-rw-rw-r--   0 root         (0)     1003    33532 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_external_config.py
+-rw-rw-r--   0 root         (0)     1003     2124 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_format_options.py
+-rw-rw-r--   0 root         (0)     1003     8550 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_job_retry.py
+-rw-rw-r--   0 root         (0)     1003      985 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_legacy_types.py
+-rw-rw-r--   0 root         (0)     1003     4104 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_list_datasets.py
+-rw-rw-r--   0 root         (0)     1003     9475 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_list_jobs.py
+-rw-rw-r--   0 root         (0)     1003     2970 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_list_models.py
+-rw-rw-r--   0 root         (0)     1003     3822 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_list_projects.py
+-rw-rw-r--   0 root         (0)     1003     3074 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_list_routines.py
+-rw-rw-r--   0 root         (0)     1003     5826 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_list_tables.py
+-rw-rw-r--   0 root         (0)     1003    74919 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_magics.py
+-rw-rw-r--   0 root         (0)     1003     9718 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003    58111 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_query.py
+-rw-rw-r--   0 root         (0)     1003     4306 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_retry.py
+-rw-rw-r--   0 root         (0)     1003    36266 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_schema.py
+-rw-rw-r--   0 root         (0)     1003     2054 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_signature_compatibility.py
+-rw-rw-r--   0 root         (0)     1003    20124 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_standard_sql_types.py
+-rw-rw-r--   0 root         (0)     1003   195640 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_table.py
+-rw-rw-r--   0 root         (0)     1003     7665 2023-03-28 16:31:24.000000 google-cloud-bigquery-3.9.0/tests/unit/test_table_pandas.py
```

### Comparing `google-cloud-bigquery-3.8.0/LICENSE` & `google-cloud-bigquery-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/MANIFEST.in` & `google-cloud-bigquery-3.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/PKG-INFO` & `google-cloud-bigquery-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery
-Version: 3.8.0
+Version: 3.9.0
 Summary: Google BigQuery API client library
 Home-page: https://github.com/googleapis/python-bigquery
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-3.8.0/README.rst` & `google-cloud-bigquery-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/__init__.py` & `google-cloud-bigquery-3.9.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/_helpers.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/_http.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/_http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/_job_helpers.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/_job_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/_pandas_helpers.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/_pandas_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,15 +477,15 @@
             bq_schema_unused.discard(bq_field.name)
             continue
 
         # Otherwise, try to automatically determine the type based on the
         # pandas dtype.
         bq_type = _PANDAS_DTYPE_TO_BQ.get(dtype.name)
         if bq_type is None:
-            sample_data = _first_valid(dataframe[column])
+            sample_data = _first_valid(dataframe.reset_index()[column])
             if (
                 isinstance(sample_data, _BaseGeometry)
                 and sample_data is not None  # Paranoia
             ):
                 bq_type = "GEOGRAPHY"
         bq_field = schema.SchemaField(column, bq_type)
         bq_schema_out.append(bq_field)
@@ -540,15 +540,15 @@
     unknown_type_fields = []
 
     for field in current_bq_schema:
         if field.field_type is not None:
             augmented_schema.append(field)
             continue
 
-        arrow_table = pyarrow.array(dataframe[field.name])
+        arrow_table = pyarrow.array(dataframe.reset_index()[field.name])
 
         if pyarrow.types.is_list(arrow_table.type):
             # `pyarrow.ListType`
             detected_mode = "REPEATED"
             detected_type = ARROW_SCALAR_IDS_TO_BQ.get(arrow_table.values.type.id)
 
             # For timezone-naive datetimes, pyarrow assumes the UTC timezone and adds
```

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/_tqdm_helpers.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/_tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/client.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dataset.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/_helpers.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/connection.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/cursor.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,24 @@
         # default to None, allowing the backend to automatically determine the
         # most appropriate size.
         self.arraysize = None
         self._query_data = None
         self._query_job = None
         self._closed = False
 
+    @property
+    def query_job(self):
+        """google.cloud.bigquery.job.query.QueryJob: The query job created by
+        the last ``execute*()`` call.
+
+        .. note::
+            If the last ``execute*()`` call was ``executemany()``, this is the
+            last job created by ``executemany()``."""
+        return self._query_job
+
     def close(self):
         """Mark the cursor as closed, preventing its further use."""
         self._closed = True
 
     def _set_description(self, schema):
         """Set description from schema.
```

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/exceptions.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/dbapi/types.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/encryption_configuration.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/encryption_configuration.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/enums.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/enums.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/exceptions.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/external_config.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/external_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/format_options.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/format_options.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/iam.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/iam.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/base.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/copy_.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/copy_.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/extract.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/extract.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/load.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/load.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/job/query.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/job/query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/exceptions.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/lexer.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/parser.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/line_arg_parser/visitors.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/line_arg_parser/visitors.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/magics/magics.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/magics/magics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/model.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/model.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/opentelemetry_tracing.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/query.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/retry.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/routine/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/routine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/routine/routine.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/routine/routine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/schema.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/standard_sql.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/standard_sql.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/table.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery/version.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "3.8.0"
+__version__ = "3.9.0"
```

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/__init__.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/encryption_config.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/encryption_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/model.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/model.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/model_reference.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/model_reference.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/standard_sql.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/standard_sql.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google/cloud/bigquery_v2/types/table_reference.py` & `google-cloud-bigquery-3.9.0/google/cloud/bigquery_v2/types/table_reference.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/PKG-INFO` & `google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery
-Version: 3.8.0
+Version: 3.9.0
 Summary: Google BigQuery API client library
 Home-page: https://github.com/googleapis/python-bigquery
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/SOURCES.txt` & `google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/google_cloud_bigquery.egg-info/requires.txt` & `google-cloud-bigquery-3.9.0/google_cloud_bigquery.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/setup.py` & `google-cloud-bigquery-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/__init__.py` & `google-cloud-bigquery-3.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/data/characters.json` & `google-cloud-bigquery-3.9.0/tests/data/characters.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/data/characters.jsonl` & `google-cloud-bigquery-3.9.0/tests/data/characters.jsonl`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/data/scalars.jsonl` & `google-cloud-bigquery-3.9.0/tests/data/scalars.jsonl`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/data/scalars_extreme.jsonl` & `google-cloud-bigquery-3.9.0/tests/data/scalars_extreme.jsonl`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/data/scalars_schema.json` & `google-cloud-bigquery-3.9.0/tests/data/scalars_schema.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/data/schema.json` & `google-cloud-bigquery-3.9.0/tests/data/schema.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/scrub_datasets.py` & `google-cloud-bigquery-3.9.0/tests/scrub_datasets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/__init__.py` & `google-cloud-bigquery-3.9.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/conftest.py` & `google-cloud-bigquery-3.9.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/helpers.py` & `google-cloud-bigquery-3.9.0/tests/system/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_arrow.py` & `google-cloud-bigquery-3.9.0/tests/system/test_arrow.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_client.py` & `google-cloud-bigquery-3.9.0/tests/system/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_job_retry.py` & `google-cloud-bigquery-3.9.0/tests/system/test_job_retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_list_rows.py` & `google-cloud-bigquery-3.9.0/tests/system/test_list_rows.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_magics.py` & `google-cloud-bigquery-3.9.0/tests/system/test_magics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_pandas.py` & `google-cloud-bigquery-3.9.0/tests/system/test_pandas.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_query.py` & `google-cloud-bigquery-3.9.0/tests/system/test_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/system/test_structs.py` & `google-cloud-bigquery-3.9.0/tests/system/test_structs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/__init__.py` & `google-cloud-bigquery-3.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/_helpers/test_from_json.py` & `google-cloud-bigquery-3.9.0/tests/unit/_helpers/test_from_json.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/conftest.py` & `google-cloud-bigquery-3.9.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/helpers.py` & `google-cloud-bigquery-3.9.0/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/__init__.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/helpers.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_base.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_copy.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_copy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_extract.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_extract.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_load.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_load.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_load_config.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_load_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_query.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_query_config.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_query_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_query_pandas.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_query_pandas.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/job/test_query_stats.py` & `google-cloud-bigquery-3.9.0/tests/unit/job/test_query_stats.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/__init__.py` & `google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/test_lexer.py` & `google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/test_parser.py` & `google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/line_arg_parser/test_visitors.py` & `google-cloud-bigquery-3.9.0/tests/unit/line_arg_parser/test_visitors.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/model/test_model.py` & `google-cloud-bigquery-3.9.0/tests/unit/model/test_model.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/model/test_model_reference.py` & `google-cloud-bigquery-3.9.0/tests/unit/model/test_model_reference.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/routine/test_routine.py` & `google-cloud-bigquery-3.9.0/tests/unit/routine/test_routine.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/routine/test_routine_argument.py` & `google-cloud-bigquery-3.9.0/tests/unit/routine/test_routine_argument.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/routine/test_routine_reference.py` & `google-cloud-bigquery-3.9.0/tests/unit/routine/test_routine_reference.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test__helpers.py` & `google-cloud-bigquery-3.9.0/tests/unit/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test__http.py` & `google-cloud-bigquery-3.9.0/tests/unit/test__http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test__job_helpers.py` & `google-cloud-bigquery-3.9.0/tests/unit/test__job_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test__pandas_helpers.py` & `google-cloud-bigquery-3.9.0/tests/unit/test__pandas_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -927,40 +927,14 @@
         ("b_series", pandas.api.types.pandas_dtype("float64")),
         ("c_series", pandas.api.types.pandas_dtype("object")),
     ]
     assert columns_and_indexes == expected
 
 
 @pytest.mark.skipif(pandas is None, reason="Requires `pandas`")
-def test_dataframe_to_bq_schema_dict_sequence(module_under_test):
-    df_data = collections.OrderedDict(
-        [
-            ("str_column", ["hello", "world"]),
-            ("int_column", [42, 8]),
-            ("bool_column", [True, False]),
-        ]
-    )
-    dataframe = pandas.DataFrame(df_data)
-
-    dict_schema = [
-        {"name": "str_column", "type": "STRING", "mode": "NULLABLE"},
-        {"name": "bool_column", "type": "BOOL", "mode": "REQUIRED"},
-    ]
-
-    returned_schema = module_under_test.dataframe_to_bq_schema(dataframe, dict_schema)
-
-    expected_schema = (
-        schema.SchemaField("str_column", "STRING", "NULLABLE"),
-        schema.SchemaField("int_column", "INTEGER", "NULLABLE"),
-        schema.SchemaField("bool_column", "BOOL", "REQUIRED"),
-    )
-    assert returned_schema == expected_schema
-
-
-@pytest.mark.skipif(pandas is None, reason="Requires `pandas`")
 def test_dataframe_to_arrow_with_multiindex(module_under_test):
     bq_schema = (
         schema.SchemaField("str_index", "STRING"),
         # int_index is intentionally omitted, to verify that it's okay to be
         # missing indexes from the schema.
         schema.SchemaField("dt_index", "DATETIME"),
         schema.SchemaField("int_col", "INTEGER"),
@@ -1187,14 +1161,94 @@
 
     call_args = fake_write_table.call_args
     assert call_args is not None
     assert call_args.kwargs.get("compression") == "ZSTD"
 
 
 @pytest.mark.skipif(pandas is None, reason="Requires `pandas`")
+def test_dataframe_to_bq_schema_w_named_index(module_under_test):
+    df_data = collections.OrderedDict(
+        [
+            ("str_column", ["hello", "world"]),
+            ("int_column", [42, 8]),
+            ("bool_column", [True, False]),
+        ]
+    )
+    index = pandas.Index(["a", "b"], name="str_index")
+    dataframe = pandas.DataFrame(df_data, index=index)
+
+    returned_schema = module_under_test.dataframe_to_bq_schema(dataframe, [])
+
+    expected_schema = (
+        schema.SchemaField("str_index", "STRING", "NULLABLE"),
+        schema.SchemaField("str_column", "STRING", "NULLABLE"),
+        schema.SchemaField("int_column", "INTEGER", "NULLABLE"),
+        schema.SchemaField("bool_column", "BOOLEAN", "NULLABLE"),
+    )
+    assert returned_schema == expected_schema
+
+
+@pytest.mark.skipif(pandas is None, reason="Requires `pandas`")
+def test_dataframe_to_bq_schema_w_multiindex(module_under_test):
+    df_data = collections.OrderedDict(
+        [
+            ("str_column", ["hello", "world"]),
+            ("int_column", [42, 8]),
+            ("bool_column", [True, False]),
+        ]
+    )
+    index = pandas.MultiIndex.from_tuples(
+        [
+            ("a", 0, datetime.datetime(1999, 12, 31, 23, 59, 59, 999999)),
+            ("a", 0, datetime.datetime(2000, 1, 1, 0, 0, 0)),
+        ],
+        names=["str_index", "int_index", "dt_index"],
+    )
+    dataframe = pandas.DataFrame(df_data, index=index)
+
+    returned_schema = module_under_test.dataframe_to_bq_schema(dataframe, [])
+
+    expected_schema = (
+        schema.SchemaField("str_index", "STRING", "NULLABLE"),
+        schema.SchemaField("int_index", "INTEGER", "NULLABLE"),
+        schema.SchemaField("dt_index", "DATETIME", "NULLABLE"),
+        schema.SchemaField("str_column", "STRING", "NULLABLE"),
+        schema.SchemaField("int_column", "INTEGER", "NULLABLE"),
+        schema.SchemaField("bool_column", "BOOLEAN", "NULLABLE"),
+    )
+    assert returned_schema == expected_schema
+
+
+@pytest.mark.skipif(pandas is None, reason="Requires `pandas`")
+def test_dataframe_to_bq_schema_w_bq_schema(module_under_test):
+    df_data = collections.OrderedDict(
+        [
+            ("str_column", ["hello", "world"]),
+            ("int_column", [42, 8]),
+            ("bool_column", [True, False]),
+        ]
+    )
+    dataframe = pandas.DataFrame(df_data)
+
+    dict_schema = [
+        {"name": "str_column", "type": "STRING", "mode": "NULLABLE"},
+        {"name": "bool_column", "type": "BOOL", "mode": "REQUIRED"},
+    ]
+
+    returned_schema = module_under_test.dataframe_to_bq_schema(dataframe, dict_schema)
+
+    expected_schema = (
+        schema.SchemaField("str_column", "STRING", "NULLABLE"),
+        schema.SchemaField("int_column", "INTEGER", "NULLABLE"),
+        schema.SchemaField("bool_column", "BOOL", "REQUIRED"),
+    )
+    assert returned_schema == expected_schema
+
+
+@pytest.mark.skipif(pandas is None, reason="Requires `pandas`")
 def test_dataframe_to_bq_schema_fallback_needed_wo_pyarrow(module_under_test):
     dataframe = pandas.DataFrame(
         data=[
             {"id": 10, "status": "FOO", "execution_date": datetime.date(2019, 5, 10)},
             {"id": 20, "status": "BAR", "created_at": datetime.date(2018, 9, 12)},
         ]
     )
```

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_client.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_create_dataset.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_dataset.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_dbapi__helpers.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_dbapi__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_dbapi_connection.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_dbapi_connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_dbapi_cursor.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_dbapi_cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -658,14 +658,37 @@
 
         self.assertEqual(
             list(cursor),
             [],
             "Iterating again over the same results should produce no rows.",
         )
 
+    def test_query_job_wo_execute(self):
+        from google.cloud.bigquery import dbapi
+
+        connection = dbapi.connect(self._mock_client())
+        cursor = connection.cursor()
+        self.assertIsNone(cursor.query_job)
+
+    def test_query_job_w_execute(self):
+        from google.cloud.bigquery import dbapi, QueryJob
+
+        connection = dbapi.connect(self._mock_client())
+        cursor = connection.cursor()
+        cursor.execute("SELECT 1;")
+        self.assertIsInstance(cursor.query_job, QueryJob)
+
+    def test_query_job_w_executemany(self):
+        from google.cloud.bigquery import dbapi, QueryJob
+
+        connection = dbapi.connect(self._mock_client())
+        cursor = connection.cursor()
+        cursor.executemany("SELECT %s;", (("1",), ("2",)))
+        self.assertIsInstance(cursor.query_job, QueryJob)
+
     def test__format_operation_w_dict(self):
         from google.cloud.bigquery.dbapi import cursor
 
         parameter_types = {}
         formatted_operation, parameter_types = cursor._format_operation(
             "SELECT %(somevalue)s, %(a `weird` one:STRING)s;",
             {"somevalue": "hi", "a `weird` one": "world"},
```

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_dbapi_types.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_dbapi_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_delete_dataset.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_delete_dataset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_encryption_configuration.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_encryption_configuration.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_external_config.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_external_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_format_options.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_format_options.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_job_retry.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_job_retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_legacy_types.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_legacy_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_list_datasets.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_list_datasets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_list_jobs.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_list_jobs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_list_models.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_list_models.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_list_projects.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_list_projects.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_list_routines.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_list_routines.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_list_tables.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_list_tables.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_magics.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_magics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_opentelemetry_tracing.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_query.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_retry.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_schema.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_signature_compatibility.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_signature_compatibility.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_standard_sql_types.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_standard_sql_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_table.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-3.8.0/tests/unit/test_table_pandas.py` & `google-cloud-bigquery-3.9.0/tests/unit/test_table_pandas.py`

 * *Files identical despite different names*

