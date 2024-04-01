# Comparing `tmp/datacontract-cli-0.9.6.post2.tar.gz` & `tmp/datacontract-cli-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacontract-cli-0.9.6.post2.tar", last modified: Mon Mar  4 10:13:54 2024, max compression
+gzip compressed data, was "datacontract-cli-0.9.7.tar", last modified: Fri Mar 15 16:00:43 2024, max compression
```

## Comparing `datacontract-cli-0.9.6.post2.tar` & `datacontract-cli-0.9.7.tar`

### file list

```diff
@@ -1,103 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.373720 datacontract-cli-0.9.6.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-03-04 10:13:54.373720 datacontract-cli-0.9.6.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24832 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.361720 datacontract-cli-0.9.6.post2/datacontract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.361720 datacontract-cli-0.9.6.post2/datacontract/breaking/
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/breaking/breaking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/breaking/breaking_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/data_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.361720 datacontract-cli-0.9.6.post2/datacontract/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.361720 datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/check_that_datacontract_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.361720 datacontract-cli-0.9.6.post2/datacontract/engines/fastjsonschema/
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/fastjsonschema/check_jsonschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.361720 datacontract-cli-0.9.6.post2/datacontract/engines/fastjsonschema/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/fastjsonschema/s3/s3_read_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/engines/soda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/check_soda_execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/export/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/export/avro_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/export/dbt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/export/jsonschema_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/export/odcs_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/export/rdf_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/export/sodacl_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/imports/sql_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/init/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/init/download_datacontract_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/integration/publish_datamesh_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/lint/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.365720 datacontract-cli-0.9.6.post2/datacontract/lint/linters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/linters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/linters/example_model_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/lint/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.369720 datacontract-cli-0.9.6.post2/datacontract/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/model/breaking_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/model/data_contract_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/model/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/datacontract/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.373720 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-03-04 10:13:54.000000 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-04 10:13:54.000000 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:13:54.000000 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-04 10:13:54.000000 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-04 10:13:54.000000 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-04 10:13:54.000000 datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 10:13:54.373720 datacontract-cli-0.9.6.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:13:54.373720 datacontract-cli-0.9.6.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_breaking.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_download_datacontract_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_examples_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_examples_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_examples_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_kafka_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_local_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_s3_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_s3_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_s3_json_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_s3_json_multiple_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_s3_json_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_examples_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_dbt_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_dbt_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_dbt_staging_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_odcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_export_sodacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_import_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_integration_datameshmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_linters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-04 10:12:11.000000 datacontract-cli-0.9.6.post2/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.744598 datacontract-cli-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-03-15 16:00:43.744598 datacontract-cli-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26914 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/breaking/
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/breaking/breaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/breaking/breaking_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19880 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/data_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/engines/datacontract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/datacontract/check_that_datacontract_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/engines/fastjsonschema/
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/fastjsonschema/check_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/engines/fastjsonschema/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/fastjsonschema/s3/s3_read_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/engines/soda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/check_soda_execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.724598 datacontract-cli-0.9.7/datacontract/engines/soda/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/engines/soda/connections/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.728598 datacontract-cli-0.9.7/datacontract/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/avro_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/avro_idl_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/dbt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/jsonschema_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/odcs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/protobuf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/rdf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/sodacl_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/sql_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/sql_type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/export/terraform_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.728598 datacontract-cli-0.9.7/datacontract/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/imports/avro_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/imports/sql_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.728598 datacontract-cli-0.9.7/datacontract/init/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/init/download_datacontract_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.728598 datacontract-cli-0.9.7/datacontract/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/integration/publish_datamesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/integration/publish_opentelemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.728598 datacontract-cli-0.9.7/datacontract/lint/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.732598 datacontract-cli-0.9.7/datacontract/lint/linters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/description_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/example_model_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/field_pattern_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/field_reference_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/notice_period_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/primary_field_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/quality_schema_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/linters/valid_constraints_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/lint/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.732598 datacontract-cli-0.9.7/datacontract/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/model/breaking_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/model/data_contract_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/model/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/datacontract/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.740598 datacontract-cli-0.9.7/datacontract_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-03-15 16:00:43.000000 datacontract-cli-0.9.7/datacontract_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-15 16:00:43.000000 datacontract-cli-0.9.7/datacontract_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:00:43.000000 datacontract-cli-0.9.7/datacontract_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-15 16:00:43.000000 datacontract-cli-0.9.7/datacontract_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-15 16:00:43.000000 datacontract-cli-0.9.7/datacontract_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-15 16:00:43.000000 datacontract-cli-0.9.7/datacontract_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 16:00:43.744598 datacontract-cli-0.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:43.740598 datacontract-cli-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_breaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36122 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_description_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_documentation_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_download_datacontract_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_example_model_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_examples_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_examples_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_examples_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_examples_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_kafka_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_local_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_s3_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_s3_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_s3_json_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_s3_json_multiple_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_s3_json_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_examples_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_avro_idl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_dbt_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_dbt_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_dbt_staging_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_odcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_sodacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_export_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_field_constraint_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_field_pattern_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_field_reference_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_import_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_import_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_integration_datameshmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_integration_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_notice_period_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_primary_field_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_quality_schema_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-15 15:59:26.000000 datacontract-cli-0.9.7/tests/test_web.py
```

### Comparing `datacontract-cli-0.9.6.post2/LICENSE` & `datacontract-cli-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/PKG-INFO` & `datacontract-cli-0.9.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacontract-cli
-Version: 0.9.6.post2
+Version: 0.9.7
 Summary: Test data contracts
 Author-email: Jochen Christ <jochen.christ@innoq.com>, Stefan Negele <stefan.negele@innoq.com>
 Project-URL: Homepage, https://cli.datacontract.com
 Project-URL: Issues, https://github.com/datacontract/cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Requires-Dist: soda-core-spark-df~=3.2.1
 Requires-Dist: snowflake-connector-python[pandas]<3.8,>=3.6
 Requires-Dist: duckdb==0.10.0
 Requires-Dist: fastjsonschema~=2.19.1
 Requires-Dist: python-dotenv~=1.0.0
 Requires-Dist: s3fs==2024.2.0
 Requires-Dist: rdflib==7.0.0
+Requires-Dist: avro==1.11.3
 Provides-Extra: dev
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: testcontainers-minio; extra == "dev"
 Requires-Dist: testcontainers-postgres; extra == "dev"
 Requires-Dist: testcontainers-kafka; extra == "dev"
 
@@ -48,14 +49,15 @@
     <img alt="Stars" src="https://img.shields.io/github/stars/datacontract/cli" /></a>
   <a href="https://datacontract.com/slack" rel="nofollow"><img src="https://camo.githubusercontent.com/5ade1fd1e76a6ab860802cdd2941fe2501e2ca2cb534e5d8968dbf864c13d33d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f736c61636b2d6a6f696e5f636861742d77686974652e7376673f6c6f676f3d736c61636b267374796c653d736f6369616c" alt="Slack Status" data-canonical-src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&amp;style=social" style="max-width: 100%;"></a>
 </p>
 
 The `datacontract` CLI is an open source command-line tool for working with [Data Contracts](https://datacontract.com/).
 It uses data contract YAML files to lint the data contract, connect to data sources and execute schema and quality tests, detect breaking changes, and export to different formats. The tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD pipeline, or directly as a Python library.
 
+![Main features of the Data Contract CLI](datacontractcli.png)
 
 ## Getting started
 
 Let's look at this data contract:
 [https://datacontract.com/examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/orders-latest/datacontract.yaml)
 
 We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, and _quality_ attributes that describe the expected freshness and number of rows.
@@ -119,26 +121,29 @@
 
 # execute schema and quality checks on the examples within the contract
 $ datacontract test --examples datacontract.yaml
 
 # find differences between to data contracts (Coming Soon)
 $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml
 
-# fail pipeline on breaking changes  (Coming Soon)
+# find differences between to data contracts categorized into error, warning, and info.
+$ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml
+
+# fail pipeline on breaking changes. Uses changelog internally and showing only error and warning.
 $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
 
-# export model as jsonschema
+# export model as jsonschema (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql (coming soon), sodacl, terraform)
 $ datacontract export --format jsonschema datacontract.yaml
 
-# export model as dbt
-$ datacontract export --format dbt datacontract.yaml
-
 # import sql
 $ datacontract import --format sql --source my_ddl.sql
 
+# import avro
+$ datacontract import --format avro --source avro_schema.avsc
+
 # import protobuf as model (Coming Soon)
 $ datacontract import --format protobuf --source my_protobuf_file.proto datacontract.yaml
 ```
 
 ## Programmatic (Python)
 ```python
 from datacontract.data_contract import DataContract
@@ -156,17 +161,43 @@
 
 ```bash
 # Fetch current data contract, execute tests on production, and publish result to data mesh manager
 $ EXPORT DATAMESH_MANAGER_API_KEY=xxx
 $ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
 ```
 
+## Scenario: Integration with OpenTelemetry
+
+If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
 
+The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
 
+| datacontract.cli.test.result | Description                           |
+|-------|---------------------------------------|
+| 0     | test run passed, no warnings          |
+| 1     | test run has warnings                 |
+| 2     | test run failed                       |
+| 3     | test run not possible due to an error |
+| 4     | test status unknown                   |
+
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to open telemetry
+$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
+$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
+$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret (Optional, when using SaaS Products)
+$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf (Optional, because it is the default value)
+# Send to OpenTelemetry
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
+```
 
+Current limitations:
+- no gRPC support
+- currently, only ConsoleExporter and OTLP Exporter
+- Metrics only, no logs yet (but loosely planned)
 
 ## Installation
 
 Choose the most appropriate installation method for your needs:
 
 ### pip
 Python 3.11 recommended.
@@ -457,17 +488,19 @@
 | `odcs`             | Export to Open Data Contract Standard (ODCS)            | ✅      | 
 | `sodacl`           | Export to SodaCL quality checks in YAML format          | ✅      |
 | `dbt`              | Export to dbt models in YAML format                     | ✅      |
 | `dbt-sources`      | Export to dbt sources in YAML format                    | ✅      |
 | `dbt-staging-sql`  | Export to dbt staging SQL models                        | ✅      |
 | `rdf`              | Export data contract to RDF representation in N3 format | ✅      |
 | `avro`             | Export to AVRO models                                   | ✅      |
+| `protobuf`         | Export to Protobuf                                      | ✅      |
+| `terraform`        | Export to terraform resources                           | ✅      |
+| `sql`              | Export to SQL DDL                                       | ✅      |
+| `sql-query`        | Export to SQL Query                                     | ✅      |
 | `pydantic`         | Export to pydantic models                               | TBD    |
-| `sql`              | Export to SQL DDL                                       | TBD    |
-| `protobuf`         | Export to Protobuf                                      | TBD    |
 | Missing something? | Please create an issue on GitHub                        | TBD    |
 
 #### RDF
 
 The export function converts a given data contract into a RDF representation. You have the option to 
 add a base_url which will be used as the default prefix to resolve relative IRIs inside the document.
 
@@ -499,15 +532,15 @@
 
 Available import options:
 
 | Type               | Description                                    | Status  |
 |--------------------|------------------------------------------------|---------|
 | `sql`              | Import from SQL DDL                            | ✅       | 
 | `protobuf`         | Import from Protobuf schemas                   | TBD     |
-| `avro`             | Import from AVRO schemas                       | TBD     |
+| `avro`             | Import from AVRO schemas                       | ✅     |
 | `jsonschema`       | Import from JSON Schemas                       | TBD     |
 | `dbt`              | Import from dbt models                         | TBD     |
 | `odcs`             | Import from Open Data Contract Standard (ODCS) | TBD     |
 | Missing something? | Please create an issue on GitHub               | TBD     |
 
 ## Development Setup
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.6.post2 Summary: Test
-data contracts Author-email: Jochen Christ
+Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.7 Summary: Test data
+contracts Author-email: Jochen Christ
 innoq.com>, Stefan Negele
 innoq.com> Project-URL: Homepage, https://cli.datacontract.com Project-URL:
 Issues, https://github.com/datacontract/cli/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 typer[all]~=0.9.0 Requires-Dist: pydantic<2.7.0,>=2.5.3 Requires-Dist:
@@ -12,39 +12,40 @@
 Requires-Dist: rich~=13.7.0 Requires-Dist: simple-ddl-parser==1.0.3 Requires-
 Dist: soda-core-bigquery~=3.2.1 Requires-Dist: soda-core-duckdb~=3.2.1
 Requires-Dist: soda-core-postgres~=3.2.1 Requires-Dist: soda-core-
 snowflake~=3.2.1 Requires-Dist: soda-core-spark[databricks]~=3.2.1 Requires-
 Dist: soda-core-spark-df~=3.2.1 Requires-Dist: snowflake-connector-python
 [pandas]<3.8,>=3.6 Requires-Dist: duckdb==0.10.0 Requires-Dist:
 fastjsonschema~=2.19.1 Requires-Dist: python-dotenv~=1.0.0 Requires-Dist:
-s3fs==2024.2.0 Requires-Dist: rdflib==7.0.0 Provides-Extra: dev Requires-Dist:
-httpx==0.27.0; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: testcontainers-minio; extra == "dev" Requires-Dist: testcontainers-
-postgres; extra == "dev" Requires-Dist: testcontainers-kafka; extra == "dev" #
-Data Contract CLI
+s3fs==2024.2.0 Requires-Dist: rdflib==7.0.0 Requires-Dist: avro==1.11.3
+Provides-Extra: dev Requires-Dist: httpx==0.27.0; extra == "dev" Requires-Dist:
+pytest; extra == "dev" Requires-Dist: testcontainers-minio; extra == "dev"
+Requires-Dist: testcontainers-postgres; extra == "dev" Requires-Dist:
+testcontainers-kafka; extra == "dev" # Data Contract CLI
 _[_T_e_s_t_ _W_o_r_k_f_l_o_w_]_[_S_t_a_r_s_]_[_S_l_a_c_k_ _S_t_a_t_u_s_]
 The `datacontract` CLI is an open source command-line tool for working with
 [Data Contracts](https://datacontract.com/). It uses data contract YAML files
 to lint the data contract, connect to data sources and execute schema and
 quality tests, detect breaking changes, and export to different formats. The
 tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD
-pipeline, or directly as a Python library. ## Getting started Let's look at
-this data contract: [https://datacontract.com/examples/orders-latest/
-datacontract.yaml](https://datacontract.com/examples/orders-latest/
-datacontract.yaml) We have a _servers_ section with endpoint details to the S3
-bucket, _models_ for the structure of the data, and _quality_ attributes that
-describe the expected freshness and number of rows. This data contract contains
-all information to connect to S3 and check that the actual data meets the
-defined schema and quality requirements. We can use this information to test if
-the actual data set in S3 is compliant to the data contract. Let's use [pip]
-(https://pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the
-[Docker image](#docker), if you prefer). ```bash $ python3 -m pip install
-datacontract-cli ``` We run the tests: ```bash $ datacontract test https://
-datacontract.com/examples/orders-latest/datacontract.yaml # returns: Testing
-https://datacontract.com/examples/orders-latest/datacontract.yaml
+pipeline, or directly as a Python library. ![Main features of the Data Contract
+CLI](datacontractcli.png) ## Getting started Let's look at this data contract:
+[https://datacontract.com/examples/orders-latest/datacontract.yaml](https://
+datacontract.com/examples/orders-latest/datacontract.yaml) We have a _servers_
+section with endpoint details to the S3 bucket, _models_ for the structure of
+the data, and _quality_ attributes that describe the expected freshness and
+number of rows. This data contract contains all information to connect to S3
+and check that the actual data meets the defined schema and quality
+requirements. We can use this information to test if the actual data set in S3
+is compliant to the data contract. Let's use [pip](https://pip.pypa.io/en/
+stable/getting-started/) to install the CLI (or use the [Docker image]
+(#docker), if you prefer). ```bash $ python3 -m pip install datacontract-cli
+``` We run the tests: ```bash $ datacontract test https://datacontract.com/
+examples/orders-latest/datacontract.yaml # returns: Testing https://
+datacontract.com/examples/orders-latest/datacontract.yaml
 â­âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââ¬ââââââââââ®
 â Result â Check â Field â Details â
 ââââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â passed â Check that JSON has valid schema â orders â â â passed
 â Check that JSON has valid schema â line_items â â â passed â
 Check that field order_id is present â orders â â â passed â Check
 that field order_timestamp is present â orders â â â passed â Check
@@ -75,54 +76,76 @@
 with the schema, and all quality attributes are met. ## Usage ```bash # create
 a new data contract from example and write it to datacontract.yaml $
 datacontract init datacontract.yaml # lint the datacontract.yaml $ datacontract
 lint datacontract.yaml # execute schema and quality checks $ datacontract test
 datacontract.yaml # execute schema and quality checks on the examples within
 the contract $ datacontract test --examples datacontract.yaml # find
 differences between to data contracts (Coming Soon) $ datacontract diff
-datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes
-(Coming Soon) $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
-# export model as jsonschema $ datacontract export --format jsonschema
-datacontract.yaml # export model as dbt $ datacontract export --format dbt
+datacontract-v1.yaml datacontract-v2.yaml # find differences between to data
+contracts categorized into error, warning, and info. $ datacontract changelog
+datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes.
+Uses changelog internally and showing only error and warning. $ datacontract
+breaking datacontract-v1.yaml datacontract-v2.yaml # export model as jsonschema
+(other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf,
+sql (coming soon), sodacl, terraform) $ datacontract export --format jsonschema
 datacontract.yaml # import sql $ datacontract import --format sql --source
-my_ddl.sql # import protobuf as model (Coming Soon) $ datacontract import --
-format protobuf --source my_protobuf_file.proto datacontract.yaml ``` ##
+my_ddl.sql # import avro $ datacontract import --format avro --source
+avro_schema.avsc # import protobuf as model (Coming Soon) $ datacontract import
+--format protobuf --source my_protobuf_file.proto datacontract.yaml ``` ##
 Programmatic (Python) ```python from datacontract.data_contract import
 DataContract data_contract = DataContract
 (data_contract_file="datacontract.yaml") run = data_contract.test() if not
 run.has_passed(): print("Data quality validation failed.") # Abort pipeline,
 alert, or take corrective actions... ``` ## Scenario: Integration with Data
 Mesh Manager If you use [Data Mesh Manager](https://datamesh-manager.com/), you
 can use the data contract URL and append the `--publish` option to send and
 display the test results. Set an environment variable for your API key. ```bash
 # Fetch current data contract, execute tests on production, and publish result
 to data mesh manager $ EXPORT DATAMESH_MANAGER_API_KEY=xxx $ datacontract test
 https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-
 4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ##
-Installation Choose the most appropriate installation method for your needs:
-### pip Python 3.11 recommended. Python 3.12 available as pre-release release
-candidate for 0.9.3 ```bash python3 -m pip install datacontract-cli ``` ###
-pipx pipx installs into an isolated environment. ```bash pipx install
-datacontract-cli ``` ### Docker ```bash docker pull datacontract/cli docker run
---rm -v ${PWD}:/home/datacontract datacontract/cli ``` Or via an alias that
-automatically uses the latest version: ```bash alias datacontract='docker run -
--rm -v "${PWD}:/home/datacontract" datacontract/cli:latest' ``` ##
-Documentation ### Tests Data Contract CLI can connect to data sources and run
-schema and quality tests to verify that the data contract is valid. ```bash $
-datacontract test --server production datacontract.yaml ``` To connect to the
-databases the `server` block in the datacontract.yaml is used to set up the
-connection. In addition, credentials, such as username and passwords, may be
-defined with environment variables. The application uses different engines,
-based on the server `type`. | Type | Format | Description | Status | Engines |
-|--------------|------------|--------------------------------------------------
--------------------------|-------------|-------------------------------------
-| | `s3` | `parquet` | Works for any S3-compliant endpoint., e.g., AWS S3, GCS,
-MinIO, Ceph, ... | â | soda-core-duckdb | | `s3` | `json` | Support for
-`new_line` delimited JSON files and one JSON record per file. | â |
-fastjsonschema
+Scenario: Integration with OpenTelemetry If you use OpenTelemetry, you can use
+the data contract URL and append the `--publish-to-opentelemetry` option to
+send the test results to your OLTP-compatible instance, e.g., Prometheus. The
+metric name is "datacontract.cli.test.result" and it uses the following
+encoding for the result: | datacontract.cli.test.result | Description | |------
+-|---------------------------------------| | 0 | test run passed, no warnings |
+| 1 | test run has warnings | | 2 | test run failed | | 3 | test run not
+possible due to an error | | 4 | test status unknown | ```bash # Fetch current
+data contract, execute tests on production, and publish result to open
+telemetry $ EXPORT OTEL_SERVICE_NAME=datacontract-cli $ EXPORT
+OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-
+cloud.com:443 $ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret
+(Optional, when using SaaS Products) $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/
+protobuf (Optional, because it is the default value) # Send to OpenTelemetry $
+datacontract test https://demo.datamesh-manager.com/demo279750347121/
+datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server
+production --publish-to-opentelemetry ``` Current limitations: - no gRPC
+support - currently, only ConsoleExporter and OTLP Exporter - Metrics only, no
+logs yet (but loosely planned) ## Installation Choose the most appropriate
+installation method for your needs: ### pip Python 3.11 recommended. Python
+3.12 available as pre-release release candidate for 0.9.3 ```bash python3 -
+m pip install datacontract-cli ``` ### pipx pipx installs into an isolated
+environment. ```bash pipx install datacontract-cli ``` ### Docker ```bash
+docker pull datacontract/cli docker run --rm -v ${PWD}:/home/datacontract
+datacontract/cli ``` Or via an alias that automatically uses the latest
+version: ```bash alias datacontract='docker run --rm -v "${PWD}:/home/
+datacontract" datacontract/cli:latest' ``` ## Documentation ### Tests Data
+Contract CLI can connect to data sources and run schema and quality tests to
+verify that the data contract is valid. ```bash $ datacontract test --server
+production datacontract.yaml ``` To connect to the databases the `server` block
+in the datacontract.yaml is used to set up the connection. In addition,
+credentials, such as username and passwords, may be defined with environment
+variables. The application uses different engines, based on the server `type`.
+| Type | Format | Description | Status | Engines | |--------------|------------
+|---------------------------------------------------------------------------|--
+-----------|-------------------------------------| | `s3` | `parquet` | Works
+for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | â |
+soda-core-duckdb | | `s3` | `json` | Support for `new_line` delimited JSON
+files and one JSON record per file. | â | fastjsonschema
 soda-core-duckdb | | `s3` | `csv` | | â | soda-core-duckdb | | `s3` | `delta`
 | | Coming soon | TBD | | `postgres` | n/a | | â | soda-core-postgres | |
 `snowflake` | n/a | | â | soda-core-snowflake | | `bigquery` | n/a | | â |
 soda-core-bigquery | | `redshift` | n/a | | Coming soon | TBD | | `databricks`
 | n/a | Support for Databricks SQL with Unity catalog and Hive metastore. | â
 | soda-core-spark | | `databricks` | n/a | Support for Spark for programmatic
 use in Notebooks. | â | soda-core-spark-df | | `kafka` | `json` |
@@ -208,47 +231,49 @@
 ----|---------------------------------------------------------|--------| |
 `jsonschema` | Export to JSON Schema | â | | `odcs` | Export to Open Data
 Contract Standard (ODCS) | â | | `sodacl` | Export to SodaCL quality checks
 in YAML format | â | | `dbt` | Export to dbt models in YAML format | â | |
 `dbt-sources` | Export to dbt sources in YAML format | â | | `dbt-staging-
 sql` | Export to dbt staging SQL models | â | | `rdf` | Export data contract
 to RDF representation in N3 format | â | | `avro` | Export to AVRO models |
-â | | `pydantic` | Export to pydantic models | TBD | | `sql` | Export to SQL
-DDL | TBD | | `protobuf` | Export to Protobuf | TBD | | Missing something? |
-Please create an issue on GitHub | TBD | #### RDF The export function converts
-a given data contract into a RDF representation. You have the option to add a
-base_url which will be used as the default prefix to resolve relative IRIs
-inside the document. ```shell datacontract export --format rdf --rdf-base
-https://www.example.com/ datacontract.yaml ``` The data contract is mapped onto
-the following concepts of a yet to be defined Data Contract Ontology named
-https://datacontract.com/DataContractSpecification/ : - DataContract - Server -
-Model Having the data contract inside an RDF Graph gives us access the
-following use cases: - Interoperability with other data contract specification
-formats - Store data contracts inside a knowledge graph - Enhance a semantic
-search to find and retrieve data contracts - Linking model elements to already
-established ontologies and knowledge - Using full power of OWL to reason about
-the graph structure of data contracts - Apply graph algorithms on multiple data
-contracts (Find similar data contracts, find "gatekeeper" data products, find
-the true domain owner of a field attribute) ### Imports ```bash # Example
-import from SQL DDL datacontract import --format sql --source my_ddl.sql ```
-Available import options: | Type | Description | Status | |--------------------
-|------------------------------------------------|---------| | `sql` | Import
-from SQL DDL | â | | `protobuf` | Import from Protobuf schemas | TBD | |
-`avro` | Import from AVRO schemas | TBD | | `jsonschema` | Import from JSON
-Schemas | TBD | | `dbt` | Import from dbt models | TBD | | `odcs` | Import from
-Open Data Contract Standard (ODCS) | TBD | | Missing something? | Please create
-an issue on GitHub | TBD | ## Development Setup Python base interpreter should
-be 3.11.x (unless working on 3.12 release candidate). ```bash # create venv
-python3 -m venv venv source venv/bin/activate # Install Requirements pip
-install --upgrade pip setuptools wheel pip install -e '.[dev]' cd tests/ pytest
-``` Release ```bash git tag v0.9.0 git push origin v0.9.0 python3 -m pip
-install --upgrade build twine rm -r dist/ python3 -m build # for now only
-test.pypi.org python3 -m twine upload --repository testpypi dist/* ``` Docker
-Build ```bash docker build -t datacontract/cli . docker run --rm -v ${PWD}:/
-home/datacontract datacontract/cli ``` ## Release Steps 1. Update the version
-in `pyproject.toml` 2. Have a look at the `CHANGELOG.md` 3. Create release
-commit manually 4. Execute `./release` 5. Wait until GitHub Release is created
-6. Add the release notes to the GitHub Release ## Contribution We are happy to
-receive your contributions. Propose your change in an issue or directly create
-a pull request with your improvements. ## License [MIT License](LICENSE) ##
-Credits Created by [Stefan Negele](https://www.linkedin.com/in/stefan-negele-
-573153112/) and [Jochen Christ](https://www.linkedin.com/in/jochenchrist/).
+â | | `protobuf` | Export to Protobuf | â | | `terraform` | Export to
+terraform resources | â | | `sql` | Export to SQL DDL | â | | `sql-query` |
+Export to SQL Query | â | | `pydantic` | Export to pydantic models | TBD | |
+Missing something? | Please create an issue on GitHub | TBD | #### RDF The
+export function converts a given data contract into a RDF representation. You
+have the option to add a base_url which will be used as the default prefix to
+resolve relative IRIs inside the document. ```shell datacontract export --
+format rdf --rdf-base https://www.example.com/ datacontract.yaml ``` The data
+contract is mapped onto the following concepts of a yet to be defined Data
+Contract Ontology named https://datacontract.com/DataContractSpecification/ : -
+DataContract - Server - Model Having the data contract inside an RDF Graph
+gives us access the following use cases: - Interoperability with other data
+contract specification formats - Store data contracts inside a knowledge graph
+- Enhance a semantic search to find and retrieve data contracts - Linking model
+elements to already established ontologies and knowledge - Using full power of
+OWL to reason about the graph structure of data contracts - Apply graph
+algorithms on multiple data contracts (Find similar data contracts, find
+"gatekeeper" data products, find the true domain owner of a field attribute)
+### Imports ```bash # Example import from SQL DDL datacontract import --format
+sql --source my_ddl.sql ``` Available import options: | Type | Description |
+Status | |--------------------|------------------------------------------------
+|---------| | `sql` | Import from SQL DDL | â | | `protobuf` | Import from
+Protobuf schemas | TBD | | `avro` | Import from AVRO schemas | â | |
+`jsonschema` | Import from JSON Schemas | TBD | | `dbt` | Import from dbt
+models | TBD | | `odcs` | Import from Open Data Contract Standard (ODCS) | TBD
+| | Missing something? | Please create an issue on GitHub | TBD | ##
+Development Setup Python base interpreter should be 3.11.x (unless working on
+3.12 release candidate). ```bash # create venv python3 -m venv venv source
+venv/bin/activate # Install Requirements pip install --upgrade pip setuptools
+wheel pip install -e '.[dev]' cd tests/ pytest ``` Release ```bash git tag
+v0.9.0 git push origin v0.9.0 python3 -m pip install --upgrade build twine rm -
+r dist/ python3 -m build # for now only test.pypi.org python3 -m twine upload -
+-repository testpypi dist/* ``` Docker Build ```bash docker build -
+t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract datacontract/
+cli ``` ## Release Steps 1. Update the version in `pyproject.toml` 2. Have a
+look at the `CHANGELOG.md` 3. Create release commit manually 4. Execute `./
+release` 5. Wait until GitHub Release is created 6. Add the release notes to
+the GitHub Release ## Contribution We are happy to receive your contributions.
+Propose your change in an issue or directly create a pull request with your
+improvements. ## License [MIT License](LICENSE) ## Credits Created by [Stefan
+Negele](https://www.linkedin.com/in/stefan-negele-573153112/) and [Jochen
+Christ](https://www.linkedin.com/in/jochenchrist/).
```

### Comparing `datacontract-cli-0.9.6.post2/README.md` & `datacontract-cli-0.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     <img alt="Stars" src="https://img.shields.io/github/stars/datacontract/cli" /></a>
   <a href="https://datacontract.com/slack" rel="nofollow"><img src="https://camo.githubusercontent.com/5ade1fd1e76a6ab860802cdd2941fe2501e2ca2cb534e5d8968dbf864c13d33d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f736c61636b2d6a6f696e5f636861742d77686974652e7376673f6c6f676f3d736c61636b267374796c653d736f6369616c" alt="Slack Status" data-canonical-src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&amp;style=social" style="max-width: 100%;"></a>
 </p>
 
 The `datacontract` CLI is an open source command-line tool for working with [Data Contracts](https://datacontract.com/).
 It uses data contract YAML files to lint the data contract, connect to data sources and execute schema and quality tests, detect breaking changes, and export to different formats. The tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD pipeline, or directly as a Python library.
 
+![Main features of the Data Contract CLI](datacontractcli.png)
 
 ## Getting started
 
 Let's look at this data contract:
 [https://datacontract.com/examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/orders-latest/datacontract.yaml)
 
 We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, and _quality_ attributes that describe the expected freshness and number of rows.
@@ -78,26 +79,29 @@
 
 # execute schema and quality checks on the examples within the contract
 $ datacontract test --examples datacontract.yaml
 
 # find differences between to data contracts (Coming Soon)
 $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml
 
-# fail pipeline on breaking changes  (Coming Soon)
+# find differences between to data contracts categorized into error, warning, and info.
+$ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml
+
+# fail pipeline on breaking changes. Uses changelog internally and showing only error and warning.
 $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
 
-# export model as jsonschema
+# export model as jsonschema (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql (coming soon), sodacl, terraform)
 $ datacontract export --format jsonschema datacontract.yaml
 
-# export model as dbt
-$ datacontract export --format dbt datacontract.yaml
-
 # import sql
 $ datacontract import --format sql --source my_ddl.sql
 
+# import avro
+$ datacontract import --format avro --source avro_schema.avsc
+
 # import protobuf as model (Coming Soon)
 $ datacontract import --format protobuf --source my_protobuf_file.proto datacontract.yaml
 ```
 
 ## Programmatic (Python)
 ```python
 from datacontract.data_contract import DataContract
@@ -115,17 +119,43 @@
 
 ```bash
 # Fetch current data contract, execute tests on production, and publish result to data mesh manager
 $ EXPORT DATAMESH_MANAGER_API_KEY=xxx
 $ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
 ```
 
+## Scenario: Integration with OpenTelemetry
+
+If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
 
+The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
 
+| datacontract.cli.test.result | Description                           |
+|-------|---------------------------------------|
+| 0     | test run passed, no warnings          |
+| 1     | test run has warnings                 |
+| 2     | test run failed                       |
+| 3     | test run not possible due to an error |
+| 4     | test status unknown                   |
+
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to open telemetry
+$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
+$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
+$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret (Optional, when using SaaS Products)
+$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf (Optional, because it is the default value)
+# Send to OpenTelemetry
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
+```
 
+Current limitations:
+- no gRPC support
+- currently, only ConsoleExporter and OTLP Exporter
+- Metrics only, no logs yet (but loosely planned)
 
 ## Installation
 
 Choose the most appropriate installation method for your needs:
 
 ### pip
 Python 3.11 recommended.
@@ -416,17 +446,19 @@
 | `odcs`             | Export to Open Data Contract Standard (ODCS)            | ✅      | 
 | `sodacl`           | Export to SodaCL quality checks in YAML format          | ✅      |
 | `dbt`              | Export to dbt models in YAML format                     | ✅      |
 | `dbt-sources`      | Export to dbt sources in YAML format                    | ✅      |
 | `dbt-staging-sql`  | Export to dbt staging SQL models                        | ✅      |
 | `rdf`              | Export data contract to RDF representation in N3 format | ✅      |
 | `avro`             | Export to AVRO models                                   | ✅      |
+| `protobuf`         | Export to Protobuf                                      | ✅      |
+| `terraform`        | Export to terraform resources                           | ✅      |
+| `sql`              | Export to SQL DDL                                       | ✅      |
+| `sql-query`        | Export to SQL Query                                     | ✅      |
 | `pydantic`         | Export to pydantic models                               | TBD    |
-| `sql`              | Export to SQL DDL                                       | TBD    |
-| `protobuf`         | Export to Protobuf                                      | TBD    |
 | Missing something? | Please create an issue on GitHub                        | TBD    |
 
 #### RDF
 
 The export function converts a given data contract into a RDF representation. You have the option to 
 add a base_url which will be used as the default prefix to resolve relative IRIs inside the document.
 
@@ -458,15 +490,15 @@
 
 Available import options:
 
 | Type               | Description                                    | Status  |
 |--------------------|------------------------------------------------|---------|
 | `sql`              | Import from SQL DDL                            | ✅       | 
 | `protobuf`         | Import from Protobuf schemas                   | TBD     |
-| `avro`             | Import from AVRO schemas                       | TBD     |
+| `avro`             | Import from AVRO schemas                       | ✅     |
 | `jsonschema`       | Import from JSON Schemas                       | TBD     |
 | `dbt`              | Import from dbt models                         | TBD     |
 | `odcs`             | Import from Open Data Contract Standard (ODCS) | TBD     |
 | Missing something? | Please create an issue on GitHub               | TBD     |
 
 ## Development Setup
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
 # Data Contract CLI
 _[_T_e_s_t_ _W_o_r_k_f_l_o_w_]_[_S_t_a_r_s_]_[_S_l_a_c_k_ _S_t_a_t_u_s_]
 The `datacontract` CLI is an open source command-line tool for working with
 [Data Contracts](https://datacontract.com/). It uses data contract YAML files
 to lint the data contract, connect to data sources and execute schema and
 quality tests, detect breaking changes, and export to different formats. The
 tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD
-pipeline, or directly as a Python library. ## Getting started Let's look at
-this data contract: [https://datacontract.com/examples/orders-latest/
-datacontract.yaml](https://datacontract.com/examples/orders-latest/
-datacontract.yaml) We have a _servers_ section with endpoint details to the S3
-bucket, _models_ for the structure of the data, and _quality_ attributes that
-describe the expected freshness and number of rows. This data contract contains
-all information to connect to S3 and check that the actual data meets the
-defined schema and quality requirements. We can use this information to test if
-the actual data set in S3 is compliant to the data contract. Let's use [pip]
-(https://pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the
-[Docker image](#docker), if you prefer). ```bash $ python3 -m pip install
-datacontract-cli ``` We run the tests: ```bash $ datacontract test https://
-datacontract.com/examples/orders-latest/datacontract.yaml # returns: Testing
-https://datacontract.com/examples/orders-latest/datacontract.yaml
+pipeline, or directly as a Python library. ![Main features of the Data Contract
+CLI](datacontractcli.png) ## Getting started Let's look at this data contract:
+[https://datacontract.com/examples/orders-latest/datacontract.yaml](https://
+datacontract.com/examples/orders-latest/datacontract.yaml) We have a _servers_
+section with endpoint details to the S3 bucket, _models_ for the structure of
+the data, and _quality_ attributes that describe the expected freshness and
+number of rows. This data contract contains all information to connect to S3
+and check that the actual data meets the defined schema and quality
+requirements. We can use this information to test if the actual data set in S3
+is compliant to the data contract. Let's use [pip](https://pip.pypa.io/en/
+stable/getting-started/) to install the CLI (or use the [Docker image]
+(#docker), if you prefer). ```bash $ python3 -m pip install datacontract-cli
+``` We run the tests: ```bash $ datacontract test https://datacontract.com/
+examples/orders-latest/datacontract.yaml # returns: Testing https://
+datacontract.com/examples/orders-latest/datacontract.yaml
 â­âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââ¬ââââââââââ®
 â Result â Check â Field â Details â
 ââââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â passed â Check that JSON has valid schema â orders â â â passed
 â Check that JSON has valid schema â line_items â â â passed â
 Check that field order_id is present â orders â â â passed â Check
 that field order_timestamp is present â orders â â â passed â Check
@@ -53,54 +54,76 @@
 with the schema, and all quality attributes are met. ## Usage ```bash # create
 a new data contract from example and write it to datacontract.yaml $
 datacontract init datacontract.yaml # lint the datacontract.yaml $ datacontract
 lint datacontract.yaml # execute schema and quality checks $ datacontract test
 datacontract.yaml # execute schema and quality checks on the examples within
 the contract $ datacontract test --examples datacontract.yaml # find
 differences between to data contracts (Coming Soon) $ datacontract diff
-datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes
-(Coming Soon) $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
-# export model as jsonschema $ datacontract export --format jsonschema
-datacontract.yaml # export model as dbt $ datacontract export --format dbt
+datacontract-v1.yaml datacontract-v2.yaml # find differences between to data
+contracts categorized into error, warning, and info. $ datacontract changelog
+datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes.
+Uses changelog internally and showing only error and warning. $ datacontract
+breaking datacontract-v1.yaml datacontract-v2.yaml # export model as jsonschema
+(other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf,
+sql (coming soon), sodacl, terraform) $ datacontract export --format jsonschema
 datacontract.yaml # import sql $ datacontract import --format sql --source
-my_ddl.sql # import protobuf as model (Coming Soon) $ datacontract import --
-format protobuf --source my_protobuf_file.proto datacontract.yaml ``` ##
+my_ddl.sql # import avro $ datacontract import --format avro --source
+avro_schema.avsc # import protobuf as model (Coming Soon) $ datacontract import
+--format protobuf --source my_protobuf_file.proto datacontract.yaml ``` ##
 Programmatic (Python) ```python from datacontract.data_contract import
 DataContract data_contract = DataContract
 (data_contract_file="datacontract.yaml") run = data_contract.test() if not
 run.has_passed(): print("Data quality validation failed.") # Abort pipeline,
 alert, or take corrective actions... ``` ## Scenario: Integration with Data
 Mesh Manager If you use [Data Mesh Manager](https://datamesh-manager.com/), you
 can use the data contract URL and append the `--publish` option to send and
 display the test results. Set an environment variable for your API key. ```bash
 # Fetch current data contract, execute tests on production, and publish result
 to data mesh manager $ EXPORT DATAMESH_MANAGER_API_KEY=xxx $ datacontract test
 https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-
 4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ##
-Installation Choose the most appropriate installation method for your needs:
-### pip Python 3.11 recommended. Python 3.12 available as pre-release release
-candidate for 0.9.3 ```bash python3 -m pip install datacontract-cli ``` ###
-pipx pipx installs into an isolated environment. ```bash pipx install
-datacontract-cli ``` ### Docker ```bash docker pull datacontract/cli docker run
---rm -v ${PWD}:/home/datacontract datacontract/cli ``` Or via an alias that
-automatically uses the latest version: ```bash alias datacontract='docker run -
--rm -v "${PWD}:/home/datacontract" datacontract/cli:latest' ``` ##
-Documentation ### Tests Data Contract CLI can connect to data sources and run
-schema and quality tests to verify that the data contract is valid. ```bash $
-datacontract test --server production datacontract.yaml ``` To connect to the
-databases the `server` block in the datacontract.yaml is used to set up the
-connection. In addition, credentials, such as username and passwords, may be
-defined with environment variables. The application uses different engines,
-based on the server `type`. | Type | Format | Description | Status | Engines |
-|--------------|------------|--------------------------------------------------
--------------------------|-------------|-------------------------------------
-| | `s3` | `parquet` | Works for any S3-compliant endpoint., e.g., AWS S3, GCS,
-MinIO, Ceph, ... | â | soda-core-duckdb | | `s3` | `json` | Support for
-`new_line` delimited JSON files and one JSON record per file. | â |
-fastjsonschema
+Scenario: Integration with OpenTelemetry If you use OpenTelemetry, you can use
+the data contract URL and append the `--publish-to-opentelemetry` option to
+send the test results to your OLTP-compatible instance, e.g., Prometheus. The
+metric name is "datacontract.cli.test.result" and it uses the following
+encoding for the result: | datacontract.cli.test.result | Description | |------
+-|---------------------------------------| | 0 | test run passed, no warnings |
+| 1 | test run has warnings | | 2 | test run failed | | 3 | test run not
+possible due to an error | | 4 | test status unknown | ```bash # Fetch current
+data contract, execute tests on production, and publish result to open
+telemetry $ EXPORT OTEL_SERVICE_NAME=datacontract-cli $ EXPORT
+OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-
+cloud.com:443 $ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret
+(Optional, when using SaaS Products) $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/
+protobuf (Optional, because it is the default value) # Send to OpenTelemetry $
+datacontract test https://demo.datamesh-manager.com/demo279750347121/
+datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server
+production --publish-to-opentelemetry ``` Current limitations: - no gRPC
+support - currently, only ConsoleExporter and OTLP Exporter - Metrics only, no
+logs yet (but loosely planned) ## Installation Choose the most appropriate
+installation method for your needs: ### pip Python 3.11 recommended. Python
+3.12 available as pre-release release candidate for 0.9.3 ```bash python3 -
+m pip install datacontract-cli ``` ### pipx pipx installs into an isolated
+environment. ```bash pipx install datacontract-cli ``` ### Docker ```bash
+docker pull datacontract/cli docker run --rm -v ${PWD}:/home/datacontract
+datacontract/cli ``` Or via an alias that automatically uses the latest
+version: ```bash alias datacontract='docker run --rm -v "${PWD}:/home/
+datacontract" datacontract/cli:latest' ``` ## Documentation ### Tests Data
+Contract CLI can connect to data sources and run schema and quality tests to
+verify that the data contract is valid. ```bash $ datacontract test --server
+production datacontract.yaml ``` To connect to the databases the `server` block
+in the datacontract.yaml is used to set up the connection. In addition,
+credentials, such as username and passwords, may be defined with environment
+variables. The application uses different engines, based on the server `type`.
+| Type | Format | Description | Status | Engines | |--------------|------------
+|---------------------------------------------------------------------------|--
+-----------|-------------------------------------| | `s3` | `parquet` | Works
+for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | â |
+soda-core-duckdb | | `s3` | `json` | Support for `new_line` delimited JSON
+files and one JSON record per file. | â | fastjsonschema
 soda-core-duckdb | | `s3` | `csv` | | â | soda-core-duckdb | | `s3` | `delta`
 | | Coming soon | TBD | | `postgres` | n/a | | â | soda-core-postgres | |
 `snowflake` | n/a | | â | soda-core-snowflake | | `bigquery` | n/a | | â |
 soda-core-bigquery | | `redshift` | n/a | | Coming soon | TBD | | `databricks`
 | n/a | Support for Databricks SQL with Unity catalog and Hive metastore. | â
 | soda-core-spark | | `databricks` | n/a | Support for Spark for programmatic
 use in Notebooks. | â | soda-core-spark-df | | `kafka` | `json` |
@@ -186,47 +209,49 @@
 ----|---------------------------------------------------------|--------| |
 `jsonschema` | Export to JSON Schema | â | | `odcs` | Export to Open Data
 Contract Standard (ODCS) | â | | `sodacl` | Export to SodaCL quality checks
 in YAML format | â | | `dbt` | Export to dbt models in YAML format | â | |
 `dbt-sources` | Export to dbt sources in YAML format | â | | `dbt-staging-
 sql` | Export to dbt staging SQL models | â | | `rdf` | Export data contract
 to RDF representation in N3 format | â | | `avro` | Export to AVRO models |
-â | | `pydantic` | Export to pydantic models | TBD | | `sql` | Export to SQL
-DDL | TBD | | `protobuf` | Export to Protobuf | TBD | | Missing something? |
-Please create an issue on GitHub | TBD | #### RDF The export function converts
-a given data contract into a RDF representation. You have the option to add a
-base_url which will be used as the default prefix to resolve relative IRIs
-inside the document. ```shell datacontract export --format rdf --rdf-base
-https://www.example.com/ datacontract.yaml ``` The data contract is mapped onto
-the following concepts of a yet to be defined Data Contract Ontology named
-https://datacontract.com/DataContractSpecification/ : - DataContract - Server -
-Model Having the data contract inside an RDF Graph gives us access the
-following use cases: - Interoperability with other data contract specification
-formats - Store data contracts inside a knowledge graph - Enhance a semantic
-search to find and retrieve data contracts - Linking model elements to already
-established ontologies and knowledge - Using full power of OWL to reason about
-the graph structure of data contracts - Apply graph algorithms on multiple data
-contracts (Find similar data contracts, find "gatekeeper" data products, find
-the true domain owner of a field attribute) ### Imports ```bash # Example
-import from SQL DDL datacontract import --format sql --source my_ddl.sql ```
-Available import options: | Type | Description | Status | |--------------------
-|------------------------------------------------|---------| | `sql` | Import
-from SQL DDL | â | | `protobuf` | Import from Protobuf schemas | TBD | |
-`avro` | Import from AVRO schemas | TBD | | `jsonschema` | Import from JSON
-Schemas | TBD | | `dbt` | Import from dbt models | TBD | | `odcs` | Import from
-Open Data Contract Standard (ODCS) | TBD | | Missing something? | Please create
-an issue on GitHub | TBD | ## Development Setup Python base interpreter should
-be 3.11.x (unless working on 3.12 release candidate). ```bash # create venv
-python3 -m venv venv source venv/bin/activate # Install Requirements pip
-install --upgrade pip setuptools wheel pip install -e '.[dev]' cd tests/ pytest
-``` Release ```bash git tag v0.9.0 git push origin v0.9.0 python3 -m pip
-install --upgrade build twine rm -r dist/ python3 -m build # for now only
-test.pypi.org python3 -m twine upload --repository testpypi dist/* ``` Docker
-Build ```bash docker build -t datacontract/cli . docker run --rm -v ${PWD}:/
-home/datacontract datacontract/cli ``` ## Release Steps 1. Update the version
-in `pyproject.toml` 2. Have a look at the `CHANGELOG.md` 3. Create release
-commit manually 4. Execute `./release` 5. Wait until GitHub Release is created
-6. Add the release notes to the GitHub Release ## Contribution We are happy to
-receive your contributions. Propose your change in an issue or directly create
-a pull request with your improvements. ## License [MIT License](LICENSE) ##
-Credits Created by [Stefan Negele](https://www.linkedin.com/in/stefan-negele-
-573153112/) and [Jochen Christ](https://www.linkedin.com/in/jochenchrist/).
+â | | `protobuf` | Export to Protobuf | â | | `terraform` | Export to
+terraform resources | â | | `sql` | Export to SQL DDL | â | | `sql-query` |
+Export to SQL Query | â | | `pydantic` | Export to pydantic models | TBD | |
+Missing something? | Please create an issue on GitHub | TBD | #### RDF The
+export function converts a given data contract into a RDF representation. You
+have the option to add a base_url which will be used as the default prefix to
+resolve relative IRIs inside the document. ```shell datacontract export --
+format rdf --rdf-base https://www.example.com/ datacontract.yaml ``` The data
+contract is mapped onto the following concepts of a yet to be defined Data
+Contract Ontology named https://datacontract.com/DataContractSpecification/ : -
+DataContract - Server - Model Having the data contract inside an RDF Graph
+gives us access the following use cases: - Interoperability with other data
+contract specification formats - Store data contracts inside a knowledge graph
+- Enhance a semantic search to find and retrieve data contracts - Linking model
+elements to already established ontologies and knowledge - Using full power of
+OWL to reason about the graph structure of data contracts - Apply graph
+algorithms on multiple data contracts (Find similar data contracts, find
+"gatekeeper" data products, find the true domain owner of a field attribute)
+### Imports ```bash # Example import from SQL DDL datacontract import --format
+sql --source my_ddl.sql ``` Available import options: | Type | Description |
+Status | |--------------------|------------------------------------------------
+|---------| | `sql` | Import from SQL DDL | â | | `protobuf` | Import from
+Protobuf schemas | TBD | | `avro` | Import from AVRO schemas | â | |
+`jsonschema` | Import from JSON Schemas | TBD | | `dbt` | Import from dbt
+models | TBD | | `odcs` | Import from Open Data Contract Standard (ODCS) | TBD
+| | Missing something? | Please create an issue on GitHub | TBD | ##
+Development Setup Python base interpreter should be 3.11.x (unless working on
+3.12 release candidate). ```bash # create venv python3 -m venv venv source
+venv/bin/activate # Install Requirements pip install --upgrade pip setuptools
+wheel pip install -e '.[dev]' cd tests/ pytest ``` Release ```bash git tag
+v0.9.0 git push origin v0.9.0 python3 -m pip install --upgrade build twine rm -
+r dist/ python3 -m build # for now only test.pypi.org python3 -m twine upload -
+-repository testpypi dist/* ``` Docker Build ```bash docker build -
+t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract datacontract/
+cli ``` ## Release Steps 1. Update the version in `pyproject.toml` 2. Have a
+look at the `CHANGELOG.md` 3. Create release commit manually 4. Execute `./
+release` 5. Wait until GitHub Release is created 6. Add the release notes to
+the GitHub Release ## Contribution We are happy to receive your contributions.
+Propose your change in an issue or directly create a pull request with your
+improvements. ## License [MIT License](LICENSE) ## Credits Created by [Stefan
+Negele](https://www.linkedin.com/in/stefan-negele-573153112/) and [Jochen
+Christ](https://www.linkedin.com/in/jochenchrist/).
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/breaking/breaking.py` & `datacontract-cli-0.9.7/datacontract/breaking/breaking.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,115 @@
 from datacontract.breaking.breaking_rules import BreakingRules
-from datacontract.model.breaking_change import BreakingChanges, BreakingChange, Location
-from datacontract.model.data_contract_specification import Field, Model
+from datacontract.model.breaking_change import BreakingChanges, BreakingChange, Location, Severity
+from datacontract.model.data_contract_specification import Field, Model, Quality
+
+
+def quality_breaking_changes(
+    old_quality: Quality,
+    new_quality: Quality,
+    new_path: str,
+    include_severities: [Severity],
+) -> list[BreakingChange]:
+    results = list[BreakingChange]()
+
+    if not old_quality and new_quality:
+        rule_name = "quality_added"
+        severity = _get_rule(rule_name)
+        description = "added quality"
+
+        if severity in include_severities:
+            results.append(
+                BreakingChange(
+                    description=description,
+                    check_name=rule_name,
+                    severity=severity,
+                    location=Location(
+                        path=new_path,
+                        composition=["quality"]
+                    )))
+    elif old_quality and not new_quality:
+        rule_name = "quality_removed"
+        severity = _get_rule(rule_name)
+        description = "removed quality"
+
+        if severity in include_severities:
+            results.append(
+                BreakingChange(
+                    description=description,
+                    check_name=rule_name,
+                    severity=severity,
+                    location=Location(
+                        path=new_path,
+                        composition=["quality"]
+                    )))
+
+    elif old_quality and new_quality:
+        if old_quality.type != new_quality.type:
+            rule_name = "quality_type_updated"
+            severity = _get_rule(rule_name)
+            description = f"changed from `{old_quality.type}` to `{new_quality.type}`"
+
+            if severity in include_severities:
+                results.append(
+                    BreakingChange(
+                        description=description,
+                        check_name=rule_name,
+                        severity=severity,
+                        location=Location(
+                            path=new_path,
+                            composition=["quality", "type"]
+                        )))
+
+        if old_quality.specification != new_quality.specification:
+            rule_name = "quality_specification_updated"
+            severity = _get_rule(rule_name)
+            description = f"changed from `{old_quality.specification}` to `{new_quality.specification}`"
+            if severity in include_severities:
+                results.append(
+                    BreakingChange(
+                        description=description,
+                        check_name=rule_name,
+                        severity=severity,
+                        location=Location(
+                            path=new_path,
+                            composition=["quality", "specification"]
+                        )))
+
+    return results
 
 
 def models_breaking_changes(
     old_models: dict[str, Model],
     new_models: dict[str, Model],
-    new_path: str
-) -> BreakingChanges:
+    new_path: str,
+    include_severities: [Severity],
+) -> list[BreakingChange]:
     composition = ["models"]
     results = list[BreakingChange]()
 
     for model_name, new_model in new_models.items():
         if model_name not in old_models.keys():
             rule_name = "model_added"
             severity = _get_rule(rule_name)
-            if severity != "info":
+            if severity in include_severities:
                 results.append(
                     BreakingChange(
                         description="added the model",
                         check_name=rule_name,
                         severity=severity,
                         location=Location(
                             path=new_path,
                             composition=composition + [model_name]
                         )))
 
     for model_name, old_model in old_models.items():
         if model_name not in new_models.keys():
             rule_name = "model_removed"
             severity = _get_rule(rule_name)
-            if severity != "info":
+            if severity in include_severities:
                 results.append(
                     BreakingChange(
                         description="removed the model",
                         check_name=rule_name,
                         severity=severity,
                         location=Location(
                             path=new_path,
@@ -43,25 +118,27 @@
             continue
 
         results.extend(
             model_breaking_changes(
                 old_model=old_model,
                 new_model=new_models[model_name],
                 new_path=new_path,
-                composition=composition + [model_name]
+                composition=composition + [model_name],
+                include_severities=include_severities,
             ))
 
-    return BreakingChanges(breaking_changes=results)
+    return results
 
 
 def model_breaking_changes(
     old_model: Model,
     new_model: Model,
     new_path: str,
-    composition: list[str]
+    composition: list[str],
+    include_severities: [Severity]
 ) -> list[BreakingChange]:
     results = list[BreakingChange]()
 
     model_definition_fields = vars(new_model)
 
     for model_definition_field in model_definition_fields.keys():
         if model_definition_field == "fields":
@@ -83,15 +160,15 @@
 
         elif old_value != new_value:
             rule_name = f"model_{model_definition_field}_updated"
             description = f"changed from `{old_value}` to `{new_value}`"
 
         if rule_name is not None:
             severity = _get_rule(rule_name)
-            if severity != "info":
+            if severity in include_severities:
                 results.append(
                     BreakingChange(
                         description=description,
                         check_name=rule_name,
                         severity=severity,
                         location=Location(
                             path=new_path,
@@ -99,48 +176,50 @@
                         )))
 
     results.extend(
         fields_breaking_changes(
             old_fields=old_model.fields,
             new_fields=new_model.fields,
             new_path=new_path,
-            composition=composition
+            composition=composition + ["fields"],
+            include_severities=include_severities,
         ))
 
     return results
 
 
 def fields_breaking_changes(
     old_fields: dict[str, Field],
     new_fields: dict[str, Field],
     new_path: str,
-    composition: list[str]
+    composition: list[str],
+    include_severities: [Severity]
 ) -> list[BreakingChange]:
     results = list[BreakingChange]()
 
     for field_name, new_field in new_fields.items():
         if field_name not in old_fields.keys():
             rule_name = "field_added"
             severity = _get_rule(rule_name)
-            if severity != "info":
+            if severity in include_severities:
                 results.append(
                     BreakingChange(
                         description="added the field",
                         check_name=rule_name,
                         severity=severity,
                         location=Location(
                             path=new_path,
                             composition=composition + [field_name]
                         )))
 
     for field_name, old_field in old_fields.items():
         if field_name not in new_fields.keys():
             rule_name = "field_removed"
             severity = _get_rule(rule_name)
-            if severity != "info":
+            if severity in include_severities:
                 results.append(
                     BreakingChange(
                         description='removed the field',
                         check_name=rule_name,
                         severity=severity,
                         location=Location(
                             path=new_path,
@@ -150,91 +229,97 @@
 
         results.extend(
             field_breaking_changes(
                 old_field=old_field,
                 new_field=new_fields[field_name],
                 composition=composition + [field_name],
                 new_path=new_path,
+                include_severities=include_severities,
             ))
     return results
 
 
 def field_breaking_changes(
     old_field: Field,
     new_field: Field,
     composition: list[str],
     new_path: str,
+    include_severities: [Severity],
 ) -> list[BreakingChange]:
     results = list[BreakingChange]()
 
     field_definition_fields = vars(new_field)
     for field_definition_field in field_definition_fields.keys():
-
-        # TODO(torbenkeller): handle ref case
-        if field_definition_field == "ref":
+        if field_definition_field == "ref_obj":
             continue
 
         old_value = getattr(old_field, field_definition_field)
         new_value = getattr(new_field, field_definition_field)
 
         if field_definition_field == "fields":
             results.extend(
                 fields_breaking_changes(
                     old_fields=old_field.fields,
                     new_fields=new_field.fields,
                     new_path=new_path,
-                    composition=composition + [field_definition_field]
+                    composition=composition + [field_definition_field],
+                    include_severities=include_severities,
                 )
             )
             continue
 
         rule_name = None
         description = None
 
         # logic for enum, tags and other arrays
         if type(old_value) is list and type(new_value) is list:
             if not old_value and new_value:
-                rule_name = f"field_{field_definition_field}_added"
+                rule_name = f"field_{_camel_to_snake(field_definition_field)}_added"
                 description = f"added with value: `{new_value}`"
             elif old_value and not new_value:
-                rule_name = f"field_{field_definition_field}_removed"
+                rule_name = f"field_{_camel_to_snake(field_definition_field)}_removed"
                 description = "removed field property"
             elif sorted(old_value) != sorted(new_value):
-                rule_name = f"field_{field_definition_field}_updated"
+                rule_name = f"field_{_camel_to_snake(field_definition_field)}_updated"
                 description = f"changed from `{old_value}` to `{new_value}`"
 
         # logic for normal fields
         elif old_value is None and new_value is not None:
-            rule_name = f"field_{field_definition_field}_added"
+            rule_name = f"field_{_camel_to_snake(field_definition_field)}_added"
             description = f"added with value: `{str(new_value).lower() if type(new_value) is bool else new_value}`"
 
         elif old_value is not None and new_value is None:
-            rule_name = f"field_{field_definition_field}_removed"
+            rule_name = f"field_{_camel_to_snake(field_definition_field)}_removed"
             description = "removed field property"
 
         elif old_value != new_value:
-            rule_name = f"field_{field_definition_field}_updated"
+            rule_name = f"field_{_camel_to_snake(field_definition_field)}_updated"
             description = (f"changed from `{str(old_value).lower() if type(old_value) is bool else old_value}` "
                            f"to `{str(new_value).lower() if type(new_value) is bool else new_value}`")
 
         if rule_name is not None:
             severity = _get_rule(rule_name)
-            if severity != "info":
+            field_schema_name = "$ref" if field_definition_field == "ref" else field_definition_field
+            if severity in include_severities:
                 results.append(
                     BreakingChange(
                         description=description,
                         check_name=rule_name,
                         severity=severity,
                         location=Location(
                             path=new_path,
-                            composition=composition + [field_definition_field]
+                            composition=composition + [field_schema_name]
                         )))
 
     return results
 
 
-def _get_rule(rule_name):
+def _get_rule(rule_name) -> Severity:
     try:
         return getattr(BreakingRules, rule_name)
     except AttributeError:
         print(f'WARNING: Breaking Rule not found for {rule_name}!')
-        return 'error'
+        return Severity.ERROR
+
+
+def _camel_to_snake(s):
+    return ''.join(['_' + c.lower() if c.isupper() else c for c in s]).lstrip('_')
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/cli.py` & `datacontract-cli-0.9.7/datacontract/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -96,59 +96,81 @@
              "Use the key of the server object in the data contract yaml file "
              "to refer to a server, e.g., `production`, or `all` for all "
              "servers (default).")] = "all",
     examples: Annotated[bool, typer.Option(
         help="Run the schema and quality tests on the example data within the data contract.")] = None,
     publish: Annotated[str, typer.Option(
         help="The url to publish the results after the test")] = None,
+    publish_to_opentelemetry: Annotated[bool, typer.Option(
+        help="Publish the results to opentelemetry. Use environment variables to configure the OTLP endpoint, headers, etc.")] = False,
     logs: Annotated[bool, typer.Option(
         help="Print logs")] = False,
 ):
     """
     Run schema and quality tests on configured servers.
     """
     print(f"Testing {location}")
     if server == "all":
         server = None
-    run = DataContract(data_contract_file=location, schema_location=schema, publish_url=publish, server=server,
-                       examples=examples).test()
+    run = DataContract(data_contract_file=location,
+                       schema_location=schema,
+                       publish_url=publish,
+                       publish_to_opentelemetry=publish_to_opentelemetry,
+                       server=server,
+                       examples=examples,
+                       ).test()
     if logs:
         _print_logs(run)
     _handle_result(run)
 
 
 class ExportFormat(str, Enum):
     jsonschema = "jsonschema"
     sodacl = "sodacl"
     dbt = "dbt"
     dbt_sources = "dbt-sources"
     dbt_staging_sql = "dbt-staging-sql"
     odcs = "odcs"
     rdf = "rdf"
     avro = "avro"
+    protobuf = "protobuf"
+    terraform = "terraform"
+    avro_idl = "avro-idl"
+    sql = "sql"
+    sql_query = "sql-query"
 
 
 @app.command()
 def export(
     format: Annotated[ExportFormat, typer.Option(help="The export format.")],
     server: Annotated[str, typer.Option(help="The server name to export.")] = None,
-    rdf_base: Annotated[Optional[str], typer.Option(help="[rdf] The base URI used to generate the RDF graph.")] = None,
+    model: Annotated[str, typer.Option(help="Use the key of the model in the data contract yaml file "
+                                            "to refer to a model, e.g., `orders`, or `all` for all "
+                                            "models (default).")] = "all",
+    rdf_base: Annotated[Optional[str], typer.Option(help="[rdf] The base URI used to generate the RDF graph.", rich_help_panel="RDF Options")] = None,
+    sql_server_type: Annotated[Optional[str], typer.Option(help="[sql] The server type to determine the sql dialect. By default, it uses 'auto' to automatically detect the sql dialect via the specified servers in the data contract.", rich_help_panel="SQL Options")] = "auto",
     location: Annotated[
         str, typer.Argument(help="The location (url or path) of the data contract yaml.")] = "datacontract.yaml",
 ):
     """
     Convert data contract to a specific format. Prints to stdout.
     """
     # TODO exception handling
-    result = DataContract(data_contract_file=location, server=server).export(format, rdf_base)
+    result = DataContract(data_contract_file=location, server=server).export(
+        export_format=format,
+        model=model,
+        rdf_base=rdf_base,
+        sql_server_type=sql_server_type,
+    )
     print(result)
 
 
 class ImportFormat(str, Enum):
     sql = "sql"
+    avro = "avro"
 
 
 @app.command(name="import")
 def import_(
     format: Annotated[ImportFormat, typer.Option(help="The format of the source file.")],
     source: Annotated[str, typer.Option(help="The path to the file that should be imported.")],
 ):
@@ -165,20 +187,73 @@
     location_new: Annotated[str, typer.Argument(help="The location (url or path) of the new data contract yaml.")],
 ):
     """
     Identifies breaking changes between data contracts. Prints to stdout.
     """
 
     # TODO exception handling
-    result = DataContract(data_contract_file=location_old).breaking(DataContract(data_contract_file=location_new))
-    print(str(result))
+    result = DataContract(
+        data_contract_file=location_old,
+        inline_definitions=True
+    ).breaking(
+        DataContract(
+            data_contract_file=location_new,
+            inline_definitions=True
+        ))
+
+    print(result.breaking_str())
+
     if not result.passed_checks():
         raise typer.Exit(code=1)
 
 
+@app.command()
+def changelog(
+    location_old: Annotated[str, typer.Argument(help="The location (url or path) of the old data contract yaml.")],
+    location_new: Annotated[str, typer.Argument(help="The location (url or path) of the new data contract yaml.")],
+):
+    """
+    Generate a changelog between data contracts. Prints to stdout.
+    """
+
+    # TODO exception handling
+    result = DataContract(
+        data_contract_file=location_old,
+        inline_definitions=True
+    ).changelog(
+        DataContract(
+            data_contract_file=location_new,
+            inline_definitions=True
+        ))
+
+    print(result.changelog_str())
+
+
+@app.command()
+def diff(
+    location_old: Annotated[str, typer.Argument(help="The location (url or path) of the old data contract yaml.")],
+    location_new: Annotated[str, typer.Argument(help="The location (url or path) of the new data contract yaml.")],
+):
+    """
+    PLACEHOLDER. Currently works as 'changelog' does.
+    """
+
+    # TODO change to diff output, not the changelog entries
+    result = DataContract(
+        data_contract_file=location_old,
+        inline_definitions=True
+    ).changelog(
+        DataContract(
+            data_contract_file=location_new,
+            inline_definitions=True
+        ))
+
+    print(result.changelog_str())
+
+
 def _handle_result(run):
     _print_table(run)
     if run.result == "passed":
         print(
             f"🟢 data contract is valid. Run {len(run.checks)} checks. Took {(run.timestampEnd - run.timestampStart).total_seconds()} seconds.")
     else:
         print("🔴 data contract is invalid, found the following errors:")
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py` & `datacontract-cli-0.9.7/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/check_that_datacontract_file_exists.py` & `datacontract-cli-0.9.7/datacontract/engines/datacontract/check_that_datacontract_file_exists.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py` & `datacontract-cli-0.9.7/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/fastjsonschema/check_jsonschema.py` & `datacontract-cli-0.9.7/datacontract/engines/fastjsonschema/check_jsonschema.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/fastjsonschema/s3/s3_read_files.py` & `datacontract-cli-0.9.7/datacontract/engines/fastjsonschema/s3/s3_read_files.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/check_soda_execute.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/check_soda_execute.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/bigquery.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/bigquery.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/dask.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/dask.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/databricks.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/databricks.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/duckdb.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/duckdb.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/kafka.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/kafka.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/postgres.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/postgres.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/engines/soda/connections/snowflake.py` & `datacontract-cli-0.9.7/datacontract/engines/soda/connections/snowflake.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/export/avro_converter.py` & `datacontract-cli-0.9.7/datacontract/export/avro_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/export/dbt_converter.py` & `datacontract-cli-0.9.7/datacontract/export/dbt_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from typing import Dict
 
 import yaml
 
+from datacontract.export.sql_type_converter import convert_to_sql_type
 from datacontract.model.data_contract_specification import \
     DataContractSpecification, Model, Field
 
 
-# snowflake data types:
-# https://docs.snowflake.com/en/sql-reference/data-types.html
+
 
 
 def to_dbt_models_yaml(data_contract_spec: DataContractSpecification):
     dbt = {
         "version": 2,
         "models": [],
     }
     for model_key, model_value in data_contract_spec.models.items():
         dbt_model = _to_dbt_model(model_key, model_value, data_contract_spec)
         dbt["models"].append(dbt_model)
-    return yaml.dump(dbt, indent=2, sort_keys=False)
+    return yaml.dump(dbt, indent=2, sort_keys=False, allow_unicode=True)
 
 
-def to_dbt_staging_sql(data_contract_spec: DataContractSpecification):
+def to_dbt_staging_sql(data_contract_spec: DataContractSpecification, model_name: str, model_value: Model) -> str:
     if data_contract_spec.models is None or len(data_contract_spec.models.items()) != 1:
         print(f"Export to dbt-staging-sql currently only works with exactly one model in the data contract.")
         return ""
 
     id = data_contract_spec.id
-    model_name, model = next(iter(data_contract_spec.models.items()))
     columns = []
-    for field_name, field in model.fields.items():
+    for field_name, field in model_value.fields.items():
         # TODO escape SQL reserved key words, probably dependent on server type
         columns.append(field_name)
     return f"""
     select 
         {", ".join(columns)}
     from {{{{ source('{id}', '{model_name}') }}}}
 """
@@ -58,15 +57,15 @@
     if found_server is not None:
         source["database"] = found_server.database
         source["schema"] = found_server.schema_
 
     for model_key, model_value in data_contract_spec.models.items():
         dbt_model = _to_dbt_source_table(model_key, model_value)
         source["tables"].append(dbt_model)
-    return yaml.dump(dbt, indent=2, sort_keys=False)
+    return yaml.dump(dbt, indent=2, sort_keys=False, allow_unicode=True)
 
 
 def _to_dbt_source_table(model_key, model_value: Model) -> dict:
     dbt_model = {
         "name": model_key,
     }
 
@@ -129,15 +128,15 @@
         column["name"] = field_name
         columns.append(column)
     return columns
 
 
 def _to_column(field: Field, supports_constraints: bool, supports_datatype: bool) -> dict:
     column = {}
-    dbt_type = _convert_type_to_snowflake(field.type)
+    dbt_type = convert_to_sql_type(field, "snowflake")
     if dbt_type is not None:
         if supports_datatype:
             column["data_type"] = dbt_type
         else:
             column.setdefault("tests", []).append(
                 {"dbt_expectations.dbt_expectations.expect_column_values_to_be_of_type": {
                     "column_type": dbt_type}})
@@ -169,74 +168,39 @@
         column.setdefault("meta", {})["classification"] = field.classification
     if field.tags is not None and len(field.tags) > 0:
         column.setdefault("tags", []).extend(field.tags)
     if field.pattern is not None:
         # Beware, the data contract pattern is a regex, not a like pattern
         column.setdefault("tests", []).append(
             {"dbt_expectations.expect_column_values_to_match_regex": {"regex": field.pattern}})
-    if field.minimum is not None or field.maximum is not None and field.minimumExclusive is None and field.maximumExclusive is None:
+    if field.minimum is not None or field.maximum is not None and field.exclusiveMinimum is None and field.exclusiveMaximum is None:
         range_test = {}
         if field.minimum is not None:
             range_test["min_value"] = field.minimum
         if field.maximum is not None:
             range_test["max_value"] = field.maximum
         column.setdefault("tests", []).append({"dbt_expectations.expect_column_values_to_be_between": range_test})
-    elif field.minimumExclusive is not None or field.maximumExclusive is not None and field.minimum is None and field.maximum is None:
+    elif field.exclusiveMinimum is not None or field.exclusiveMaximum is not None and field.minimum is None and field.maximum is None:
         range_test = {}
-        if field.minimumExclusive is not None:
-            range_test["min_value"] = field.minimumExclusive
-        if field.maximumExclusive is not None:
-            range_test["max_value"] = field.maximumExclusive
+        if field.exclusiveMinimum is not None:
+            range_test["min_value"] = field.exclusiveMinimum
+        if field.exclusiveMaximum is not None:
+            range_test["max_value"] = field.exclusiveMaximum
         range_test["strictly"] = True
         column.setdefault("tests", []).append({"dbt_expectations.expect_column_values_to_be_between": range_test})
     else:
         if field.minimum is not None:
             column.setdefault("tests", []).append(
                 {"dbt_expectations.expect_column_values_to_be_between": {"min_value": field.minimum}})
         if field.maximum is not None:
             column.setdefault("tests", []).append(
                 {"dbt_expectations.expect_column_values_to_be_between": {"max_value": field.maximum}})
-        if field.minimumExclusive is not None:
+        if field.exclusiveMinimum is not None:
             column.setdefault("tests", []).append({"dbt_expectations.expect_column_values_to_be_between": {
-                "min_value": field.minimumExclusive, "strictly": True}})
-        if field.maximumExclusive is not None:
+                "min_value": field.exclusiveMinimum, "strictly": True}})
+        if field.exclusiveMaximum is not None:
             column.setdefault("tests", []).append({"dbt_expectations.expect_column_values_to_be_between": {
-                "max_value": field.maximumExclusive, "strictly": True}})
+                "max_value": field.exclusiveMaximum, "strictly": True}})
 
     # TODO: all constraints
     return column
 
-
-def _convert_type_to_snowflake(type) -> None | str:
-    # currently optimized for snowflake
-    # LEARNING: data contract has no direct support for CHAR,CHARACTER
-    # LEARNING: data contract has no support for "date-time", "datetime", "time"
-    # LEARNING: No precision and scale support in data contract
-    # LEARNING: no support for any
-    # GEOGRAPHY and GEOMETRY are not supported by the mapping
-    if type is None:
-        return None
-    if type.lower() in ["string", "varchar", "text"]:
-        return type.upper()  # STRING, TEXT, VARCHAR are all the same in snowflake
-    if type.lower() in ["timestamp", "timestamp_tz"]:
-        return "TIMESTAMP_TZ"
-    if type.lower() in ["timestamp_ntz"]:
-        return "TIMESTAMP_NTZ"
-    if type.lower() in ["date"]:
-        return "DATE"
-    if type.lower() in ["time"]:
-        return "TIME"
-    if type.lower() in ["number", "decimal", "numeric"]:
-        return "NUMBER"  # precision and scale not supported by data contract
-    if type.lower() in ["float", "double"]:
-        return "FLOAT"
-    if type.lower() in ["integer", "int", "long", "bigint"]:
-        return "NUMBER"  # always NUMBER(38,0)
-    if type.lower() in ["boolean"]:
-        return "BOOLEAN"
-    if type.lower() in ["object", "record", "struct"]:
-        return "OBJECT"
-    if type.lower() in ["bytes"]:
-        return "BINARY"
-    if type.lower() in ["array"]:
-        return "ARRAY"
-    return None
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/export/jsonschema_converter.py` & `datacontract-cli-0.9.7/datacontract/export/jsonschema_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/export/odcs_converter.py` & `datacontract-cli-0.9.7/datacontract/export/odcs_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     odcs["type"] = "tables" # required, TODO read from models.type?
     odcs["dataset"] = []
 
     for model_key, model_value in data_contract_spec.models.items():
         odcs_table = to_odcs_table(model_key, model_value)
         odcs["dataset"].append(odcs_table)
-    return yaml.dump(odcs, indent=2, sort_keys=False)
+    return yaml.dump(odcs, indent=2, sort_keys=False, allow_unicode=True)
 
 
 def to_odcs_table(model_key, model_value: Model) -> dict:
     odcs_table = {
         "table": model_key,
         "physicalName": model_key,
         "columns": [],
@@ -87,18 +87,18 @@
         column["tags"].append(f"maxLength:{field.maxLength}")
     if field.pattern is not None:
         column["tags"].append(f"pattern:{field.pattern}")
     if field.minimum is not None:
         column["tags"].append(f"minimum:{field.minimum}")
     if field.maximum is not None:
         column["tags"].append(f"maximum:{field.maximum}")
-    if field.minimumExclusive is not None:
-        column["tags"].append(f"minimumExclusive:{field.minimumExclusive}")
-    if field.maximumExclusive is not None:
-        column["tags"].append(f"maximumExclusive:{field.maximumExclusive}")
+    if field.exclusiveMinimum is not None:
+        column["tags"].append(f"exclusiveMinimum:{field.exclusiveMinimum}")
+    if field.exclusiveMaximum is not None:
+        column["tags"].append(f"exclusiveMaximum:{field.exclusiveMaximum}")
     if not column["tags"]:
         del column["tags"]
 
     # todo enum
     return column
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/export/rdf_converter.py` & `datacontract-cli-0.9.7/datacontract/export/rdf_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                              "pii", "classification", "data", "enum", "minimum", "maximum", "patterns"]
 
 
 def is_uriref(property_name):
     return property_name in ["model", "domain", "owner"]
 
 
-def to_rdf_n3(data_contract_spec: DataContractSpecification, base) -> Graph:
+def to_rdf_n3(data_contract_spec: DataContractSpecification, base) -> str:
     return to_rdf(data_contract_spec, base).serialize(format="n3")
 
 def to_rdf(data_contract_spec: DataContractSpecification, base) -> Graph:
     if base is not None:
         g = Graph(base=base)
     else:
         g = Graph(base=Namespace(""))
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/export/sodacl_converter.py` & `datacontract-cli-0.9.7/datacontract/export/sodacl_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/imports/sql_importer.py` & `datacontract-cli-0.9.7/datacontract/imports/sql_importer.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/integration/publish_datamesh_manager.py` & `datacontract-cli-0.9.7/datacontract/integration/publish_datamesh_manager.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/lint/lint.py` & `datacontract-cli-0.9.7/datacontract/lint/lint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from dataclasses import dataclass, field
-from typing import Sequence, Any
+from typing import Sequence, Any, cast
 import abc
 
 from ..model.data_contract_specification import DataContractSpecification
 from datacontract.model.run import Check
 
 """This module contains linter definitions for linting a data contract.
 
@@ -27,15 +27,15 @@
 
 @dataclass
 class LinterMessage:
     """A single linter message with attached severity and optional "model" that
     caused the message.
 
     Attributes:
-       outcome: The outcome of the linting, either ERROR or WARNING.
+       outcome: The outcome of the linting, either ERROR or WARNING. Linting outcomes with level WARNING are discarded for now.
        message: A message describing the error or warning in more detail.
        model: The model that caused the lint to fail. Is optional.
 
     """
     outcome: LintSeverity
     message: str
     model: Any = None
@@ -58,21 +58,29 @@
       linter: The linter that produced these results
       results: A list of linting results. Multiple identical linting
           results can be present in the list. An empty list means that
           the linter ran without producing warnings or errors.
     """
     results: Sequence[LinterMessage] = field(default_factory=list)
 
+    @classmethod
+    def erroneous(cls, message, model=None):
+        return cls([LinterMessage.error(message, model)])
+
+    @classmethod
+    def cautious(cls, message, model=None):
+        return cls([LinterMessage.warning(message, model)])
+
     def with_warning(self, message, model=None):
         result = LinterMessage.warning(message, model)
-        return LinterResult(self.results + [result])
+        return LinterResult(cast(list[LinterMessage],self.results) + [result])
 
     def with_error(self, message, model=None):
         result = LinterMessage.error(message, model)
-        return LinterResult(self.results + [result])
+        return LinterResult(cast(list[LinterMessage], self.results) + [result])
 
     def has_errors(self) -> bool:
         return any(map(lambda result: result.outcome == LintSeverity.ERROR,
                        self.results))
 
     def has_warnings(self) -> bool:
         return any(map(lambda result: result.outcome == LintSeverity.WARNING,
@@ -85,42 +93,54 @@
     def warning_results(self) -> Sequence[LinterMessage]:
         return [result for result in self.results
                 if result.outcome == LintSeverity.WARNING]
 
     def no_errors_or_warnings(self) -> bool:
         return len(self.results) == 0
 
+    def combine(self, other: 'LinterResult') -> 'LinterResult':
+        return LinterResult(cast(list[Any], self.results) +
+                            cast(list[Any], other.results))
+
 
 class Linter(abc.ABC):
     @property
     @abc.abstractmethod
     def name(self) -> str:
+        """Human-readable name of the linter."""
+        pass
+
+    @property
+    @abc.abstractmethod
+    def id(self) -> str:
+        """A linter ID for configuration (i.e. enabling and disabling)."""
         pass
 
     @abc.abstractmethod
     def lint_implementation(self, contract: DataContractSpecification) -> LinterResult:
         pass
 
     def lint(self, contract: DataContractSpecification) -> list[Check]:
+        """Call with a data contract to get a list of check results from the linter."""
         result = self.lint_implementation(contract)
         checks = []
         if not result.error_results():
             checks.append(Check(
                 type="lint",
-                name=f"Linter '{self.name()}'",
+                name=f"Linter '{self.name}'",
                 result="passed",
                 engine="datacontract"
             ))
         else:
             # All linter messages are treated as warnings. Severity is
             # currently ignored, but could be used in filtering in the future
             # Linter messages with level WARNING are currently ignored, but might
             # be logged or printed in the future.
             for lint_error in result.error_results():
                 checks.append(Check(
                     type="lint",
-                    name=f"Linter '{self.name()}'",
+                    name=f"Linter '{self.name}'",
                     result="warning",
                     engine="datacontract",
                     reason=lint_error.message
                 ))
         return checks
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/lint/linters/example_model_linter.py` & `datacontract-cli-0.9.7/datacontract/lint/linters/example_model_linter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,64 +4,89 @@
 import io
 
 from ..lint import Linter, LinterResult
 from datacontract.model.data_contract_specification import DataContractSpecification, Example
 
 
 class ExampleModelLinter(Linter):
+
+    @property
     def name(self) -> str:
         return "Example(s) match model"
 
+    @property
+    def id(self) -> str:
+        return "example-model"
+
     @staticmethod
     def get_example_headers(example: Example) -> list[str]:
-        match example.type:
-            case "csv":
-                dialect = csv.Sniffer().sniff(example.data)
-                data = io.StringIO(example.data)
-                reader = csv.reader(data, dialect=dialect)
-                return next(reader)
-            case "yaml":
-                data = yaml.safe_load(example.data)
-                return data.keys()
-            case "json":
-                data = json.loads(example.data)
-                return data.keys()
+        if isinstance(example.data, str):
+            match example.type:
+                case "csv":
+                    dialect = csv.Sniffer().sniff(example.data)
+                    data = io.StringIO(example.data)
+                    reader = csv.reader(data, dialect=dialect)
+                    return next(reader)
+                case "yaml":
+                    data = yaml.safe_load(example.data)
+                    return data.keys()
+                case "json":
+                    data = json.loads(example.data)
+                    return data.keys()
+                case _:
+                    # This is checked in lint_implementation, so shouldn't happen.
+                    raise NotImplementedError(f"Unknown type {example.type}")
+        else:
+            # Checked in lint_implementation, shouldn't happen.
+            raise NotImplementedError("Can't lint object examples.") 
 
     def lint_implementation(
         self,
-        data_contract_yaml: DataContractSpecification
+        contract: DataContractSpecification
     ) -> LinterResult:
-        """Check whether the example(s) match the model."""
+        """Check whether the example(s) headers match the model.
+
+          This linter checks whether the example's fields match the model
+          fields, and whether all required fields of the model are present in
+          the example.
+        """
         result = LinterResult()
-        examples = data_contract_yaml.examples
-        models = data_contract_yaml.models
+        examples = contract.examples
+        models = contract.models
         examples_with_model = []
         for (index, example) in enumerate(examples):
             if example.model not in models:
                 result = result.with_error(
                     f"Example {index + 1} has non-existent model '{example.model}'")
             else:
                 examples_with_model.append(
                     (index, example, models.get(example.model)))
         for (index, example, model) in examples_with_model:
             if example.type == "custom":
                 result = result.with_warning(f"Example {index + 1} has type"
                                              " \"custom\", cannot check model"
                                              " conformance")
+            elif not isinstance(example.data, str):
+                result = result.with_warning(f"Example {index + 1} is not a "
+                    "string example, can only lint string examples for now.")
             elif model.type == "object":
                 result = result.with_warning(
                     f"Example {index + 1} uses a "
                     f"model '{example.model}' with type 'object'. Linting is "
                     "currently only supported for 'table' models")
             else:
-                headers = self.get_example_headers(example)
-                for example_header in headers:
-                    if example_header not in model.fields:
-                        result = result.with_error(
-                            f"Example {index + 1} has field '{example_header}'"
-                            f" that's not contained in model '{example.model}'")
-                for (field_name, field_value) in model.fields.items():
-                    if field_name not in headers and field_value.required:
-                        result = result.with_error(
-                            f"Example {index + 1} is missing field '{field_name}'"
-                            f" required by model '{example.model}'")
+                if example.type in ("csv", "yaml", "json"):
+                    headers = self.get_example_headers(example)
+                    for example_header in headers:
+                        if example_header not in model.fields:
+                            result = result.with_error(
+                                f"Example {index + 1} has field '{example_header}'"
+                                f" that's not contained in model '{example.model}'")
+                    for (field_name, field_value) in model.fields.items():
+                        if field_name not in headers and field_value.required:
+                            result = result.with_error(
+                                f"Example {index + 1} is missing field '{field_name}'"
+                                f" required by model '{example.model}'")
+                else:
+                    result = result.with_error(f"Example {index + 1} has unknown type"                        
+                                               f"{example.type}")
         return result
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/lint/schema.py` & `datacontract-cli-0.9.7/datacontract/lint/schema.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/lint/urls.py` & `datacontract-cli-0.9.7/datacontract/lint/urls.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/model/data_contract_specification.py` & `datacontract-cli-0.9.7/datacontract/model/data_contract_specification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,128 @@
 import os
 from typing import List, Dict
 
-import pydantic
+import pydantic as pyd
 import yaml
-from pydantic import BaseModel
 
 
-class Contact(BaseModel):
+class Contact(pyd.BaseModel):
     name: str = None
     url: str = None
     email: str = None
 
 
-class Server(BaseModel):
+class Server(pyd.BaseModel):
     type: str = None
     format: str = None
     project: str = None
     dataset: str = None
     path: str = None
     delimiter: str = None
     endpointUrl: str = None
     location: str = None
     account: str = None
     database: str = None
-    schema_: str = pydantic.fields.Field(default=None, alias='schema')
+    schema_: str = pyd.Field(default=None, alias='schema')
     host: str = None
     port: int = None
     catalog: str = None
     topic: str = None
     http_path: str = None # Use ENV variable
     token: str = None     # Use ENV variable
     dataProductId: str = None
     outputPortId: str = None
 
 
-class Terms(BaseModel):
+class Terms(pyd.BaseModel):
     usage: str = None
     limitations: str = None
     billing: str = None
     noticePeriod: str = None
 
 
-class Field(BaseModel):
-    ref: str = None
+class Definition(pyd.BaseModel):
+    domain: str = None
+    name: str = None
+    title: str = None
+    description: str = None
+    type: str = None
+    enum: List[str] = []
+    format: str = None
+    minLength: int = None
+    maxLength: int = None
+    pattern: str = None
+    minimum: int = None
+    exclusiveMinimum: int = None
+    maximum: int = None
+    exclusiveMaximum: int = None
+    pii: bool = None
+    classification: str = None
+    tags: List[str] = []
+
+
+class Field(pyd.BaseModel):
+    ref: str = pyd.Field(default=None, alias="$ref")
+    ref_obj: Definition = pyd.Field(default=None, exclude=True)
     type: str = None
     format: str = None
     required: bool = None
     primary: bool = None
     unique: bool = None
+    references: str = None
     description: str = None
     pii: bool = None
     classification: str = None
     pattern: str = None
     minLength: int = None
     maxLength: int = None
     minimum: int = None
-    minimumExclusive: int = None
+    exclusiveMinimum: int = None
     maximum: int = None
-    maximumExclusive: int = None
+    exclusiveMaximum: int = None
     enum: List[str] = []
     tags: List[str] = []
     fields: Dict[str, 'Field'] = {}
-
-    @property
-    def ref(self):
-        return self.schema.get("$ref")
+    items: 'Field' = None
 
 
-class Model(BaseModel):
+class Model(pyd.BaseModel):
     description: str = None
     type: str = None
     fields: Dict[str, Field] = {}
 
 
-class Info(BaseModel):
+class Info(pyd.BaseModel):
     title: str = None
     version: str = None
     description: str = None
     owner: str = None
     contact: Contact = None
 
 
-class Example(BaseModel):
+class Example(pyd.BaseModel):
     type: str = None
     description: str = None
     model: str = None
     data: str | object = None
 
 
-class Quality(BaseModel):
+class Quality(pyd.BaseModel):
     type: str = None
     specification: str | object = None
 
 
-class DataContractSpecification(BaseModel):
+class DataContractSpecification(pyd.BaseModel):
     dataContractSpecification: str = None
     id: str = None
     info: Info = None
     servers: Dict[str, Server] = {}
     terms: Terms = None
     models: Dict[str, Model] = {}
+    definitions: Dict[str, Definition] = {}
     # schema: Dict[str, str]
     examples: List[Example] = []
     quality: Quality = None
 
     @classmethod
     def from_file(cls, file):
         if not os.path.exists(file):
@@ -114,8 +133,8 @@
 
     @classmethod
     def from_string(cls, data_contract_str):
         data = yaml.safe_load(data_contract_str)
         return DataContractSpecification(**data)
 
     def to_yaml(self):
-        return yaml.dump(self.model_dump(exclude_defaults=True, exclude_none=True), sort_keys=False)
+        return yaml.dump(self.model_dump(exclude_defaults=True, exclude_none=True), sort_keys=False, allow_unicode=True)
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract/model/exceptions.py` & `datacontract-cli-0.9.7/datacontract/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/datacontract/model/run.py` & `datacontract-cli-0.9.7/datacontract/model/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     dataContractId: Optional[str] = None
     dataContractVersion: Optional[str] = None
     dataProductId: Optional[str] = None
     outputPortId: Optional[str] = None
     server: Optional[str] = None
     timestampStart: datetime
     timestampEnd: datetime
-    result: str = "unknown"
+    result: str = "unknown" # passed, warning, failed, error, unknown
     checks: List[Check]
     logs: List[Log]
 
     def has_passed(self):
         self.calculate_result()
         return self.result == "passed"
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/PKG-INFO` & `datacontract-cli-0.9.7/datacontract_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacontract-cli
-Version: 0.9.6.post2
+Version: 0.9.7
 Summary: Test data contracts
 Author-email: Jochen Christ <jochen.christ@innoq.com>, Stefan Negele <stefan.negele@innoq.com>
 Project-URL: Homepage, https://cli.datacontract.com
 Project-URL: Issues, https://github.com/datacontract/cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Requires-Dist: soda-core-spark-df~=3.2.1
 Requires-Dist: snowflake-connector-python[pandas]<3.8,>=3.6
 Requires-Dist: duckdb==0.10.0
 Requires-Dist: fastjsonschema~=2.19.1
 Requires-Dist: python-dotenv~=1.0.0
 Requires-Dist: s3fs==2024.2.0
 Requires-Dist: rdflib==7.0.0
+Requires-Dist: avro==1.11.3
 Provides-Extra: dev
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: testcontainers-minio; extra == "dev"
 Requires-Dist: testcontainers-postgres; extra == "dev"
 Requires-Dist: testcontainers-kafka; extra == "dev"
 
@@ -48,14 +49,15 @@
     <img alt="Stars" src="https://img.shields.io/github/stars/datacontract/cli" /></a>
   <a href="https://datacontract.com/slack" rel="nofollow"><img src="https://camo.githubusercontent.com/5ade1fd1e76a6ab860802cdd2941fe2501e2ca2cb534e5d8968dbf864c13d33d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f736c61636b2d6a6f696e5f636861742d77686974652e7376673f6c6f676f3d736c61636b267374796c653d736f6369616c" alt="Slack Status" data-canonical-src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&amp;style=social" style="max-width: 100%;"></a>
 </p>
 
 The `datacontract` CLI is an open source command-line tool for working with [Data Contracts](https://datacontract.com/).
 It uses data contract YAML files to lint the data contract, connect to data sources and execute schema and quality tests, detect breaking changes, and export to different formats. The tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD pipeline, or directly as a Python library.
 
+![Main features of the Data Contract CLI](datacontractcli.png)
 
 ## Getting started
 
 Let's look at this data contract:
 [https://datacontract.com/examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/orders-latest/datacontract.yaml)
 
 We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, and _quality_ attributes that describe the expected freshness and number of rows.
@@ -119,26 +121,29 @@
 
 # execute schema and quality checks on the examples within the contract
 $ datacontract test --examples datacontract.yaml
 
 # find differences between to data contracts (Coming Soon)
 $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml
 
-# fail pipeline on breaking changes  (Coming Soon)
+# find differences between to data contracts categorized into error, warning, and info.
+$ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml
+
+# fail pipeline on breaking changes. Uses changelog internally and showing only error and warning.
 $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
 
-# export model as jsonschema
+# export model as jsonschema (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql (coming soon), sodacl, terraform)
 $ datacontract export --format jsonschema datacontract.yaml
 
-# export model as dbt
-$ datacontract export --format dbt datacontract.yaml
-
 # import sql
 $ datacontract import --format sql --source my_ddl.sql
 
+# import avro
+$ datacontract import --format avro --source avro_schema.avsc
+
 # import protobuf as model (Coming Soon)
 $ datacontract import --format protobuf --source my_protobuf_file.proto datacontract.yaml
 ```
 
 ## Programmatic (Python)
 ```python
 from datacontract.data_contract import DataContract
@@ -156,17 +161,43 @@
 
 ```bash
 # Fetch current data contract, execute tests on production, and publish result to data mesh manager
 $ EXPORT DATAMESH_MANAGER_API_KEY=xxx
 $ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
 ```
 
+## Scenario: Integration with OpenTelemetry
+
+If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
 
+The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
 
+| datacontract.cli.test.result | Description                           |
+|-------|---------------------------------------|
+| 0     | test run passed, no warnings          |
+| 1     | test run has warnings                 |
+| 2     | test run failed                       |
+| 3     | test run not possible due to an error |
+| 4     | test status unknown                   |
+
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to open telemetry
+$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
+$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
+$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret (Optional, when using SaaS Products)
+$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf (Optional, because it is the default value)
+# Send to OpenTelemetry
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
+```
 
+Current limitations:
+- no gRPC support
+- currently, only ConsoleExporter and OTLP Exporter
+- Metrics only, no logs yet (but loosely planned)
 
 ## Installation
 
 Choose the most appropriate installation method for your needs:
 
 ### pip
 Python 3.11 recommended.
@@ -457,17 +488,19 @@
 | `odcs`             | Export to Open Data Contract Standard (ODCS)            | ✅      | 
 | `sodacl`           | Export to SodaCL quality checks in YAML format          | ✅      |
 | `dbt`              | Export to dbt models in YAML format                     | ✅      |
 | `dbt-sources`      | Export to dbt sources in YAML format                    | ✅      |
 | `dbt-staging-sql`  | Export to dbt staging SQL models                        | ✅      |
 | `rdf`              | Export data contract to RDF representation in N3 format | ✅      |
 | `avro`             | Export to AVRO models                                   | ✅      |
+| `protobuf`         | Export to Protobuf                                      | ✅      |
+| `terraform`        | Export to terraform resources                           | ✅      |
+| `sql`              | Export to SQL DDL                                       | ✅      |
+| `sql-query`        | Export to SQL Query                                     | ✅      |
 | `pydantic`         | Export to pydantic models                               | TBD    |
-| `sql`              | Export to SQL DDL                                       | TBD    |
-| `protobuf`         | Export to Protobuf                                      | TBD    |
 | Missing something? | Please create an issue on GitHub                        | TBD    |
 
 #### RDF
 
 The export function converts a given data contract into a RDF representation. You have the option to 
 add a base_url which will be used as the default prefix to resolve relative IRIs inside the document.
 
@@ -499,15 +532,15 @@
 
 Available import options:
 
 | Type               | Description                                    | Status  |
 |--------------------|------------------------------------------------|---------|
 | `sql`              | Import from SQL DDL                            | ✅       | 
 | `protobuf`         | Import from Protobuf schemas                   | TBD     |
-| `avro`             | Import from AVRO schemas                       | TBD     |
+| `avro`             | Import from AVRO schemas                       | ✅     |
 | `jsonschema`       | Import from JSON Schemas                       | TBD     |
 | `dbt`              | Import from dbt models                         | TBD     |
 | `odcs`             | Import from Open Data Contract Standard (ODCS) | TBD     |
 | Missing something? | Please create an issue on GitHub               | TBD     |
 
 ## Development Setup
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.6.post2 Summary: Test
-data contracts Author-email: Jochen Christ
+Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.7 Summary: Test data
+contracts Author-email: Jochen Christ
 innoq.com>, Stefan Negele
 innoq.com> Project-URL: Homepage, https://cli.datacontract.com Project-URL:
 Issues, https://github.com/datacontract/cli/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 typer[all]~=0.9.0 Requires-Dist: pydantic<2.7.0,>=2.5.3 Requires-Dist:
@@ -12,39 +12,40 @@
 Requires-Dist: rich~=13.7.0 Requires-Dist: simple-ddl-parser==1.0.3 Requires-
 Dist: soda-core-bigquery~=3.2.1 Requires-Dist: soda-core-duckdb~=3.2.1
 Requires-Dist: soda-core-postgres~=3.2.1 Requires-Dist: soda-core-
 snowflake~=3.2.1 Requires-Dist: soda-core-spark[databricks]~=3.2.1 Requires-
 Dist: soda-core-spark-df~=3.2.1 Requires-Dist: snowflake-connector-python
 [pandas]<3.8,>=3.6 Requires-Dist: duckdb==0.10.0 Requires-Dist:
 fastjsonschema~=2.19.1 Requires-Dist: python-dotenv~=1.0.0 Requires-Dist:
-s3fs==2024.2.0 Requires-Dist: rdflib==7.0.0 Provides-Extra: dev Requires-Dist:
-httpx==0.27.0; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-
-Dist: testcontainers-minio; extra == "dev" Requires-Dist: testcontainers-
-postgres; extra == "dev" Requires-Dist: testcontainers-kafka; extra == "dev" #
-Data Contract CLI
+s3fs==2024.2.0 Requires-Dist: rdflib==7.0.0 Requires-Dist: avro==1.11.3
+Provides-Extra: dev Requires-Dist: httpx==0.27.0; extra == "dev" Requires-Dist:
+pytest; extra == "dev" Requires-Dist: testcontainers-minio; extra == "dev"
+Requires-Dist: testcontainers-postgres; extra == "dev" Requires-Dist:
+testcontainers-kafka; extra == "dev" # Data Contract CLI
 _[_T_e_s_t_ _W_o_r_k_f_l_o_w_]_[_S_t_a_r_s_]_[_S_l_a_c_k_ _S_t_a_t_u_s_]
 The `datacontract` CLI is an open source command-line tool for working with
 [Data Contracts](https://datacontract.com/). It uses data contract YAML files
 to lint the data contract, connect to data sources and execute schema and
 quality tests, detect breaking changes, and export to different formats. The
 tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD
-pipeline, or directly as a Python library. ## Getting started Let's look at
-this data contract: [https://datacontract.com/examples/orders-latest/
-datacontract.yaml](https://datacontract.com/examples/orders-latest/
-datacontract.yaml) We have a _servers_ section with endpoint details to the S3
-bucket, _models_ for the structure of the data, and _quality_ attributes that
-describe the expected freshness and number of rows. This data contract contains
-all information to connect to S3 and check that the actual data meets the
-defined schema and quality requirements. We can use this information to test if
-the actual data set in S3 is compliant to the data contract. Let's use [pip]
-(https://pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the
-[Docker image](#docker), if you prefer). ```bash $ python3 -m pip install
-datacontract-cli ``` We run the tests: ```bash $ datacontract test https://
-datacontract.com/examples/orders-latest/datacontract.yaml # returns: Testing
-https://datacontract.com/examples/orders-latest/datacontract.yaml
+pipeline, or directly as a Python library. ![Main features of the Data Contract
+CLI](datacontractcli.png) ## Getting started Let's look at this data contract:
+[https://datacontract.com/examples/orders-latest/datacontract.yaml](https://
+datacontract.com/examples/orders-latest/datacontract.yaml) We have a _servers_
+section with endpoint details to the S3 bucket, _models_ for the structure of
+the data, and _quality_ attributes that describe the expected freshness and
+number of rows. This data contract contains all information to connect to S3
+and check that the actual data meets the defined schema and quality
+requirements. We can use this information to test if the actual data set in S3
+is compliant to the data contract. Let's use [pip](https://pip.pypa.io/en/
+stable/getting-started/) to install the CLI (or use the [Docker image]
+(#docker), if you prefer). ```bash $ python3 -m pip install datacontract-cli
+``` We run the tests: ```bash $ datacontract test https://datacontract.com/
+examples/orders-latest/datacontract.yaml # returns: Testing https://
+datacontract.com/examples/orders-latest/datacontract.yaml
 â­âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââ¬ââââââââââ®
 â Result â Check â Field â Details â
 ââââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â passed â Check that JSON has valid schema â orders â â â passed
 â Check that JSON has valid schema â line_items â â â passed â
 Check that field order_id is present â orders â â â passed â Check
 that field order_timestamp is present â orders â â â passed â Check
@@ -75,54 +76,76 @@
 with the schema, and all quality attributes are met. ## Usage ```bash # create
 a new data contract from example and write it to datacontract.yaml $
 datacontract init datacontract.yaml # lint the datacontract.yaml $ datacontract
 lint datacontract.yaml # execute schema and quality checks $ datacontract test
 datacontract.yaml # execute schema and quality checks on the examples within
 the contract $ datacontract test --examples datacontract.yaml # find
 differences between to data contracts (Coming Soon) $ datacontract diff
-datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes
-(Coming Soon) $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
-# export model as jsonschema $ datacontract export --format jsonschema
-datacontract.yaml # export model as dbt $ datacontract export --format dbt
+datacontract-v1.yaml datacontract-v2.yaml # find differences between to data
+contracts categorized into error, warning, and info. $ datacontract changelog
+datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes.
+Uses changelog internally and showing only error and warning. $ datacontract
+breaking datacontract-v1.yaml datacontract-v2.yaml # export model as jsonschema
+(other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf,
+sql (coming soon), sodacl, terraform) $ datacontract export --format jsonschema
 datacontract.yaml # import sql $ datacontract import --format sql --source
-my_ddl.sql # import protobuf as model (Coming Soon) $ datacontract import --
-format protobuf --source my_protobuf_file.proto datacontract.yaml ``` ##
+my_ddl.sql # import avro $ datacontract import --format avro --source
+avro_schema.avsc # import protobuf as model (Coming Soon) $ datacontract import
+--format protobuf --source my_protobuf_file.proto datacontract.yaml ``` ##
 Programmatic (Python) ```python from datacontract.data_contract import
 DataContract data_contract = DataContract
 (data_contract_file="datacontract.yaml") run = data_contract.test() if not
 run.has_passed(): print("Data quality validation failed.") # Abort pipeline,
 alert, or take corrective actions... ``` ## Scenario: Integration with Data
 Mesh Manager If you use [Data Mesh Manager](https://datamesh-manager.com/), you
 can use the data contract URL and append the `--publish` option to send and
 display the test results. Set an environment variable for your API key. ```bash
 # Fetch current data contract, execute tests on production, and publish result
 to data mesh manager $ EXPORT DATAMESH_MANAGER_API_KEY=xxx $ datacontract test
 https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-
 4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ##
-Installation Choose the most appropriate installation method for your needs:
-### pip Python 3.11 recommended. Python 3.12 available as pre-release release
-candidate for 0.9.3 ```bash python3 -m pip install datacontract-cli ``` ###
-pipx pipx installs into an isolated environment. ```bash pipx install
-datacontract-cli ``` ### Docker ```bash docker pull datacontract/cli docker run
---rm -v ${PWD}:/home/datacontract datacontract/cli ``` Or via an alias that
-automatically uses the latest version: ```bash alias datacontract='docker run -
--rm -v "${PWD}:/home/datacontract" datacontract/cli:latest' ``` ##
-Documentation ### Tests Data Contract CLI can connect to data sources and run
-schema and quality tests to verify that the data contract is valid. ```bash $
-datacontract test --server production datacontract.yaml ``` To connect to the
-databases the `server` block in the datacontract.yaml is used to set up the
-connection. In addition, credentials, such as username and passwords, may be
-defined with environment variables. The application uses different engines,
-based on the server `type`. | Type | Format | Description | Status | Engines |
-|--------------|------------|--------------------------------------------------
--------------------------|-------------|-------------------------------------
-| | `s3` | `parquet` | Works for any S3-compliant endpoint., e.g., AWS S3, GCS,
-MinIO, Ceph, ... | â | soda-core-duckdb | | `s3` | `json` | Support for
-`new_line` delimited JSON files and one JSON record per file. | â |
-fastjsonschema
+Scenario: Integration with OpenTelemetry If you use OpenTelemetry, you can use
+the data contract URL and append the `--publish-to-opentelemetry` option to
+send the test results to your OLTP-compatible instance, e.g., Prometheus. The
+metric name is "datacontract.cli.test.result" and it uses the following
+encoding for the result: | datacontract.cli.test.result | Description | |------
+-|---------------------------------------| | 0 | test run passed, no warnings |
+| 1 | test run has warnings | | 2 | test run failed | | 3 | test run not
+possible due to an error | | 4 | test status unknown | ```bash # Fetch current
+data contract, execute tests on production, and publish result to open
+telemetry $ EXPORT OTEL_SERVICE_NAME=datacontract-cli $ EXPORT
+OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-
+cloud.com:443 $ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret
+(Optional, when using SaaS Products) $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/
+protobuf (Optional, because it is the default value) # Send to OpenTelemetry $
+datacontract test https://demo.datamesh-manager.com/demo279750347121/
+datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server
+production --publish-to-opentelemetry ``` Current limitations: - no gRPC
+support - currently, only ConsoleExporter and OTLP Exporter - Metrics only, no
+logs yet (but loosely planned) ## Installation Choose the most appropriate
+installation method for your needs: ### pip Python 3.11 recommended. Python
+3.12 available as pre-release release candidate for 0.9.3 ```bash python3 -
+m pip install datacontract-cli ``` ### pipx pipx installs into an isolated
+environment. ```bash pipx install datacontract-cli ``` ### Docker ```bash
+docker pull datacontract/cli docker run --rm -v ${PWD}:/home/datacontract
+datacontract/cli ``` Or via an alias that automatically uses the latest
+version: ```bash alias datacontract='docker run --rm -v "${PWD}:/home/
+datacontract" datacontract/cli:latest' ``` ## Documentation ### Tests Data
+Contract CLI can connect to data sources and run schema and quality tests to
+verify that the data contract is valid. ```bash $ datacontract test --server
+production datacontract.yaml ``` To connect to the databases the `server` block
+in the datacontract.yaml is used to set up the connection. In addition,
+credentials, such as username and passwords, may be defined with environment
+variables. The application uses different engines, based on the server `type`.
+| Type | Format | Description | Status | Engines | |--------------|------------
+|---------------------------------------------------------------------------|--
+-----------|-------------------------------------| | `s3` | `parquet` | Works
+for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | â |
+soda-core-duckdb | | `s3` | `json` | Support for `new_line` delimited JSON
+files and one JSON record per file. | â | fastjsonschema
 soda-core-duckdb | | `s3` | `csv` | | â | soda-core-duckdb | | `s3` | `delta`
 | | Coming soon | TBD | | `postgres` | n/a | | â | soda-core-postgres | |
 `snowflake` | n/a | | â | soda-core-snowflake | | `bigquery` | n/a | | â |
 soda-core-bigquery | | `redshift` | n/a | | Coming soon | TBD | | `databricks`
 | n/a | Support for Databricks SQL with Unity catalog and Hive metastore. | â
 | soda-core-spark | | `databricks` | n/a | Support for Spark for programmatic
 use in Notebooks. | â | soda-core-spark-df | | `kafka` | `json` |
@@ -208,47 +231,49 @@
 ----|---------------------------------------------------------|--------| |
 `jsonschema` | Export to JSON Schema | â | | `odcs` | Export to Open Data
 Contract Standard (ODCS) | â | | `sodacl` | Export to SodaCL quality checks
 in YAML format | â | | `dbt` | Export to dbt models in YAML format | â | |
 `dbt-sources` | Export to dbt sources in YAML format | â | | `dbt-staging-
 sql` | Export to dbt staging SQL models | â | | `rdf` | Export data contract
 to RDF representation in N3 format | â | | `avro` | Export to AVRO models |
-â | | `pydantic` | Export to pydantic models | TBD | | `sql` | Export to SQL
-DDL | TBD | | `protobuf` | Export to Protobuf | TBD | | Missing something? |
-Please create an issue on GitHub | TBD | #### RDF The export function converts
-a given data contract into a RDF representation. You have the option to add a
-base_url which will be used as the default prefix to resolve relative IRIs
-inside the document. ```shell datacontract export --format rdf --rdf-base
-https://www.example.com/ datacontract.yaml ``` The data contract is mapped onto
-the following concepts of a yet to be defined Data Contract Ontology named
-https://datacontract.com/DataContractSpecification/ : - DataContract - Server -
-Model Having the data contract inside an RDF Graph gives us access the
-following use cases: - Interoperability with other data contract specification
-formats - Store data contracts inside a knowledge graph - Enhance a semantic
-search to find and retrieve data contracts - Linking model elements to already
-established ontologies and knowledge - Using full power of OWL to reason about
-the graph structure of data contracts - Apply graph algorithms on multiple data
-contracts (Find similar data contracts, find "gatekeeper" data products, find
-the true domain owner of a field attribute) ### Imports ```bash # Example
-import from SQL DDL datacontract import --format sql --source my_ddl.sql ```
-Available import options: | Type | Description | Status | |--------------------
-|------------------------------------------------|---------| | `sql` | Import
-from SQL DDL | â | | `protobuf` | Import from Protobuf schemas | TBD | |
-`avro` | Import from AVRO schemas | TBD | | `jsonschema` | Import from JSON
-Schemas | TBD | | `dbt` | Import from dbt models | TBD | | `odcs` | Import from
-Open Data Contract Standard (ODCS) | TBD | | Missing something? | Please create
-an issue on GitHub | TBD | ## Development Setup Python base interpreter should
-be 3.11.x (unless working on 3.12 release candidate). ```bash # create venv
-python3 -m venv venv source venv/bin/activate # Install Requirements pip
-install --upgrade pip setuptools wheel pip install -e '.[dev]' cd tests/ pytest
-``` Release ```bash git tag v0.9.0 git push origin v0.9.0 python3 -m pip
-install --upgrade build twine rm -r dist/ python3 -m build # for now only
-test.pypi.org python3 -m twine upload --repository testpypi dist/* ``` Docker
-Build ```bash docker build -t datacontract/cli . docker run --rm -v ${PWD}:/
-home/datacontract datacontract/cli ``` ## Release Steps 1. Update the version
-in `pyproject.toml` 2. Have a look at the `CHANGELOG.md` 3. Create release
-commit manually 4. Execute `./release` 5. Wait until GitHub Release is created
-6. Add the release notes to the GitHub Release ## Contribution We are happy to
-receive your contributions. Propose your change in an issue or directly create
-a pull request with your improvements. ## License [MIT License](LICENSE) ##
-Credits Created by [Stefan Negele](https://www.linkedin.com/in/stefan-negele-
-573153112/) and [Jochen Christ](https://www.linkedin.com/in/jochenchrist/).
+â | | `protobuf` | Export to Protobuf | â | | `terraform` | Export to
+terraform resources | â | | `sql` | Export to SQL DDL | â | | `sql-query` |
+Export to SQL Query | â | | `pydantic` | Export to pydantic models | TBD | |
+Missing something? | Please create an issue on GitHub | TBD | #### RDF The
+export function converts a given data contract into a RDF representation. You
+have the option to add a base_url which will be used as the default prefix to
+resolve relative IRIs inside the document. ```shell datacontract export --
+format rdf --rdf-base https://www.example.com/ datacontract.yaml ``` The data
+contract is mapped onto the following concepts of a yet to be defined Data
+Contract Ontology named https://datacontract.com/DataContractSpecification/ : -
+DataContract - Server - Model Having the data contract inside an RDF Graph
+gives us access the following use cases: - Interoperability with other data
+contract specification formats - Store data contracts inside a knowledge graph
+- Enhance a semantic search to find and retrieve data contracts - Linking model
+elements to already established ontologies and knowledge - Using full power of
+OWL to reason about the graph structure of data contracts - Apply graph
+algorithms on multiple data contracts (Find similar data contracts, find
+"gatekeeper" data products, find the true domain owner of a field attribute)
+### Imports ```bash # Example import from SQL DDL datacontract import --format
+sql --source my_ddl.sql ``` Available import options: | Type | Description |
+Status | |--------------------|------------------------------------------------
+|---------| | `sql` | Import from SQL DDL | â | | `protobuf` | Import from
+Protobuf schemas | TBD | | `avro` | Import from AVRO schemas | â | |
+`jsonschema` | Import from JSON Schemas | TBD | | `dbt` | Import from dbt
+models | TBD | | `odcs` | Import from Open Data Contract Standard (ODCS) | TBD
+| | Missing something? | Please create an issue on GitHub | TBD | ##
+Development Setup Python base interpreter should be 3.11.x (unless working on
+3.12 release candidate). ```bash # create venv python3 -m venv venv source
+venv/bin/activate # Install Requirements pip install --upgrade pip setuptools
+wheel pip install -e '.[dev]' cd tests/ pytest ``` Release ```bash git tag
+v0.9.0 git push origin v0.9.0 python3 -m pip install --upgrade build twine rm -
+r dist/ python3 -m build # for now only test.pypi.org python3 -m twine upload -
+-repository testpypi dist/* ``` Docker Build ```bash docker build -
+t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract datacontract/
+cli ``` ## Release Steps 1. Update the version in `pyproject.toml` 2. Have a
+look at the `CHANGELOG.md` 3. Create release commit manually 4. Execute `./
+release` 5. Wait until GitHub Release is created 6. Add the release notes to
+the GitHub Release ## Contribution We are happy to receive your contributions.
+Propose your change in an issue or directly create a pull request with your
+improvements. ## License [MIT License](LICENSE) ## Credits Created by [Stefan
+Negele](https://www.linkedin.com/in/stefan-negele-573153112/) and [Jochen
+Christ](https://www.linkedin.com/in/jochenchrist/).
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/SOURCES.txt` & `datacontract-cli-0.9.7/datacontract_cli.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,65 +19,96 @@
 datacontract/engines/soda/connections/dask.py
 datacontract/engines/soda/connections/databricks.py
 datacontract/engines/soda/connections/duckdb.py
 datacontract/engines/soda/connections/kafka.py
 datacontract/engines/soda/connections/postgres.py
 datacontract/engines/soda/connections/snowflake.py
 datacontract/export/avro_converter.py
+datacontract/export/avro_idl_converter.py
 datacontract/export/dbt_converter.py
 datacontract/export/jsonschema_converter.py
 datacontract/export/odcs_converter.py
+datacontract/export/protobuf_converter.py
 datacontract/export/rdf_converter.py
 datacontract/export/sodacl_converter.py
+datacontract/export/sql_converter.py
+datacontract/export/sql_type_converter.py
+datacontract/export/terraform_converter.py
+datacontract/imports/avro_importer.py
 datacontract/imports/sql_importer.py
 datacontract/init/download_datacontract_file.py
 datacontract/integration/publish_datamesh_manager.py
+datacontract/integration/publish_opentelemetry.py
 datacontract/lint/files.py
 datacontract/lint/lint.py
 datacontract/lint/resolve.py
 datacontract/lint/schema.py
 datacontract/lint/urls.py
 datacontract/lint/linters/__init__.py
+datacontract/lint/linters/description_linter.py
 datacontract/lint/linters/example_model_linter.py
+datacontract/lint/linters/field_pattern_linter.py
+datacontract/lint/linters/field_reference_linter.py
+datacontract/lint/linters/notice_period_linter.py
+datacontract/lint/linters/primary_field_linter.py
+datacontract/lint/linters/quality_schema_linter.py
+datacontract/lint/linters/valid_constraints_linter.py
 datacontract/model/breaking_change.py
 datacontract/model/data_contract_specification.py
 datacontract/model/exceptions.py
 datacontract/model/run.py
 datacontract_cli.egg-info/PKG-INFO
 datacontract_cli.egg-info/SOURCES.txt
 datacontract_cli.egg-info/dependency_links.txt
 datacontract_cli.egg-info/entry_points.txt
 datacontract_cli.egg-info/requires.txt
 datacontract_cli.egg-info/top_level.txt
 tests/test_breaking.py
+tests/test_changelog.py
 tests/test_cli.py
+tests/test_description_linter.py
+tests/test_documentation_linter.py
 tests/test_download_datacontract_file.py
+tests/test_example_model_linter.py
 tests/test_examples_bigquery.py
 tests/test_examples_databricks.py
 tests/test_examples_examples_csv.py
 tests/test_examples_examples_inline.py
 tests/test_examples_examples_json.py
+tests/test_examples_examples_missing.py
 tests/test_examples_kafka.py
 tests/test_examples_kafka_remote.py
 tests/test_examples_local_json.py
 tests/test_examples_parquet.py
 tests/test_examples_postgres.py
 tests/test_examples_s3_csv.py
 tests/test_examples_s3_json.py
 tests/test_examples_s3_json_complex.py
 tests/test_examples_s3_json_multiple_models.py
 tests/test_examples_s3_json_remote.py
 tests/test_examples_snowflake.py
 tests/test_export_avro.py
+tests/test_export_avro_idl.py
 tests/test_export_dbt_models.py
 tests/test_export_dbt_sources.py
 tests/test_export_dbt_staging_sql.py
 tests/test_export_jsonschema.py
 tests/test_export_odcs.py
+tests/test_export_protobuf.py
 tests/test_export_rdf.py
 tests/test_export_sodacl.py
+tests/test_export_sql.py
+tests/test_export_sql_query.py
+tests/test_export_terraform.py
+tests/test_field_constraint_linter.py
+tests/test_field_pattern_linter.py
+tests/test_field_reference_linter.py
+tests/test_import_avro.py
 tests/test_import_sql.py
 tests/test_integration_datameshmanager.py
+tests/test_integration_opentelemetry.py
 tests/test_lint.py
-tests/test_linters.py
+tests/test_notice_period_linter.py
+tests/test_primary_field_linter.py
+tests/test_quality_schema_linter.py
 tests/test_schema.py
 tests/test_web.py
```

### Comparing `datacontract-cli-0.9.6.post2/datacontract_cli.egg-info/requires.txt` & `datacontract-cli-0.9.7/datacontract_cli.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 soda-core-spark-df~=3.2.1
 snowflake-connector-python[pandas]<3.8,>=3.6
 duckdb==0.10.0
 fastjsonschema~=2.19.1
 python-dotenv~=1.0.0
 s3fs==2024.2.0
 rdflib==7.0.0
+avro==1.11.3
 
 [dev]
 httpx==0.27.0
 pytest
 testcontainers-minio
 testcontainers-postgres
 testcontainers-kafka
```

### Comparing `datacontract-cli-0.9.6.post2/pyproject.toml` & `datacontract-cli-0.9.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datacontract-cli"
-version = "0.9.6-2"
+version = "0.9.7"
 description = "Test data contracts"
 readme = "README.md"
 authors = [
   { name = "Jochen Christ", email = "jochen.christ@innoq.com" },
   { name = "Stefan Negele", email = "stefan.negele@innoq.com" },
 ]
 classifiers = [
@@ -31,14 +31,15 @@
   "soda-core-spark-df~=3.2.1",
   "snowflake-connector-python[pandas]>=3.6,<3.8",
   "duckdb==0.10.0",
   "fastjsonschema~=2.19.1",
   "python-dotenv~=1.0.0",
   "s3fs==2024.2.0",
   "rdflib==7.0.0",
+  "avro==1.11.3",
 ]
 
 [project.optional-dependencies]
 dev = [
   "httpx==0.27.0",
   "pytest",
   "testcontainers-minio",
```

### Comparing `datacontract-cli-0.9.6.post2/tests/test_download_datacontract_file.py` & `datacontract-cli-0.9.7/tests/test_download_datacontract_file.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_bigquery.py` & `datacontract-cli-0.9.7/tests/test_examples_bigquery.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_databricks.py` & `datacontract-cli-0.9.7/tests/test_examples_databricks.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_examples_csv.py` & `datacontract-cli-0.9.7/tests/test_examples_examples_csv.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_examples_inline.py` & `datacontract-cli-0.9.7/tests/test_examples_examples_inline.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_examples_json.py` & `datacontract-cli-0.9.7/tests/test_examples_examples_json.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_kafka.py` & `datacontract-cli-0.9.7/tests/test_examples_kafka.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_kafka_remote.py` & `datacontract-cli-0.9.7/tests/test_examples_kafka_remote.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_local_json.py` & `datacontract-cli-0.9.7/tests/test_examples_local_json.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_parquet.py` & `datacontract-cli-0.9.7/tests/test_examples_parquet.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_postgres.py` & `datacontract-cli-0.9.7/tests/test_examples_postgres.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_s3_csv.py` & `datacontract-cli-0.9.7/tests/test_examples_s3_csv.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_s3_json.py` & `datacontract-cli-0.9.7/tests/test_examples_s3_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,18 +39,7 @@
     minio_client.make_bucket(bucket_name)
     with open(file_name, "rb") as file:
         minio_client.put_object(bucket_name, file_name, file, os.path.getsize(file_name))
     with open(datacontract) as data_contract_file:
         data_contract_str = data_contract_file.read()
     data_contract_str = data_contract_str.replace("__S3_ENDPOINT_URL__", s3_endpoint_url)
     return data_contract_str
-
-def _prepare_s3_files(minio_container):
-    s3_endpoint_url = f"http://{minio_container.get_container_host_ip()}:{minio_container.get_exposed_port(9000)}"
-    minio_client = minio_container.get_client()
-    minio_client.make_bucket(bucket_name)
-    with open(file_name, "rb") as file:
-        minio_client.put_object(bucket_name, file_name, file, os.path.getsize(file_name))
-    with open(datacontract) as data_contract_file:
-        data_contract_str = data_contract_file.read()
-    data_contract_str = data_contract_str.replace("__S3_ENDPOINT_URL__", s3_endpoint_url)
-    return data_contract_str
```

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_s3_json_complex.py` & `datacontract-cli-0.9.7/tests/test_examples_s3_json_complex.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_s3_json_multiple_models.py` & `datacontract-cli-0.9.7/tests/test_examples_s3_json_multiple_models.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_s3_json_remote.py` & `datacontract-cli-0.9.7/tests/test_examples_s3_json_remote.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 logging.basicConfig(level=logging.INFO, force=True)
 
 datacontract = "examples/s3-json-remote/datacontract.yaml"
 
 
 def test_examples_s3_json():
+    if 'AWS_ACCESS_KEY_ID' in os.environ:
+        del os.environ['AWS_ACCESS_KEY_ID']
+    if 'AWS_SECRET_ACCESS_KEY' in os.environ:
+        del os.environ['AWS_SECRET_ACCESS_KEY']
     if 'DATACONTRACT_S3_ACCESS_KEY_ID' in os.environ:
         del os.environ['DATACONTRACT_S3_ACCESS_KEY_ID']
     if 'DATACONTRACT_S3_SECRET_ACCESS_KEY' in os.environ:
         del os.environ['DATACONTRACT_S3_SECRET_ACCESS_KEY']
     data_contract = DataContract(data_contract_file=datacontract)
 
     run = data_contract.test()
```

### Comparing `datacontract-cli-0.9.6.post2/tests/test_examples_snowflake.py` & `datacontract-cli-0.9.7/tests/test_examples_snowflake.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_avro.py` & `datacontract-cli-0.9.7/tests/test_export_avro.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_dbt_models.py` & `datacontract-cli-0.9.7/tests/test_export_dbt_models.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_dbt_sources.py` & `datacontract-cli-0.9.7/tests/test_export_dbt_sources.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_dbt_staging_sql.py` & `datacontract-cli-0.9.7/tests/test_export_dbt_staging_sql.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 select 
     order_id,
     order_total,
     order_status
 from {{ source('orders-unit-test', 'orders') }}
 """
 
-    result = to_dbt_staging_sql(data_contract)
+    result = to_dbt_staging_sql(data_contract, "orders", data_contract.models.get("orders"))
 
     assert yaml.safe_load(result) == yaml.safe_load(expected)
```

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_jsonschema.py` & `datacontract-cli-0.9.7/tests/test_export_jsonschema.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_odcs.py` & `datacontract-cli-0.9.7/tests/test_export_odcs.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_rdf.py` & `datacontract-cli-0.9.7/tests/test_export_rdf.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_export_sodacl.py` & `datacontract-cli-0.9.7/tests/test_export_sodacl.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_import_sql.py` & `datacontract-cli-0.9.7/tests/test_import_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     assert result.exit_code == 0
 
 
 def test_import_sql():
     result = DataContract().import_from_source("sql", sql_file_path)
 
     expected = '''
-dataContractSpecification: 0.9.2
+dataContractSpecification: 0.9.3
 id: my-data-contract-id
 info:
   title: My Data Contract
   version: 0.0.1
 models:
   my_table:
     type: table
@@ -45,8 +45,9 @@
         type: integer
         required: true
       field_three:
         type: timestamp
     '''
     print("Result", result.to_yaml())
     assert yaml.safe_load(result.to_yaml()) == yaml.safe_load(expected)
-    assert DataContract(data_contract_str=expected).lint().has_passed()
+    # Disable linters so we don't get "missing description" warnings
+    assert DataContract(data_contract_str=expected).lint(enabled_linters=set()).has_passed()
```

### Comparing `datacontract-cli-0.9.6.post2/tests/test_integration_datameshmanager.py` & `datacontract-cli-0.9.7/tests/test_integration_datameshmanager.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_lint.py` & `datacontract-cli-0.9.7/tests/test_lint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from typer.testing import CliRunner
 
 from datacontract.cli import app
-from datacontract.data_contract import DataContract
+from datacontract.data_contract import DataContract, DataContractSpecification
 
 logging.basicConfig(level=logging.INFO, force=True)
 
 runner = CliRunner()
 
 
 def test_lint_valid_data_contract():
@@ -25,15 +25,15 @@
     run = data_contract.lint()
 
     assert run.result == "failed"
 
 
 def test_lint_cli_valid():
     data_contract_file = "examples/lint/valid_datacontract.yaml"
-    expected_output = "🟢 data contract is valid. Run 2 checks."
+    expected_output = "🟢 data contract is valid. Run 9 checks."
 
     result = runner.invoke(app, ["lint", data_contract_file])
 
     assert result.exit_code == 0
     assert expected_output in result.stdout
 
 
@@ -49,8 +49,14 @@
 
 def test_lint_custom_schema():
     data_contract_file = "examples/lint/custom_datacontract.yaml"
     schema_file = "examples/lint/custom_datacontract.schema.json"
     data_contract = DataContract(data_contract_file=data_contract_file, schema_location=schema_file)
 
     run = data_contract.lint()
-    assert run.result == "passed"
+    assert run.result == "passed"
+
+
+def test_lint_with_references():
+    data_contract = DataContract(data_contract_file="examples/lint/valid_datacontract_references.yaml",
+                                 inline_definitions=True)
+    DataContractSpecification.model_validate(data_contract.get_data_contract_specification())
```

### Comparing `datacontract-cli-0.9.6.post2/tests/test_linters.py` & `datacontract-cli-0.9.7/tests/test_example_model_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.6.post2/tests/test_schema.py` & `datacontract-cli-0.9.7/tests/test_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,44 +11,42 @@
     """
     data_contract = DataContract(data_contract_str="""
 dataContractSpecification: 0.9.2
 id: urn:datacontract:checkout:orders-latest
 info:
   title: Orders Latest
   version: 1.0.0
-schema:
-  type: json-schema
-  specification:
-    orders:
-      description: One record per order. Includes cancelled and deleted orders.
-      type: object
-      properties:
-        order_id:
-          type: string
-          description: Primary key of the orders table
-        order_timestamp:
-          type: string
-          format: date-time
-          description: The business timestamp in UTC when the order was successfully registered in the source system and the payment was successful.
-        order_total:
-          type: integer
-          description: Total amount of the order in the smallest monetary unit (e.g., cents).
-    line_items:
-      type: object
-      properties:
-        lines_item_id:
-          type: string
-          description: Primary key of the lines_item_id table
-        order_id:
-          type: string
-          description: Foreign key to the orders table
-        sku:
-          type: string
-          description: The purchased article number""")
+models:
+  orders:
+    description: One record per order. Includes cancelled and deleted orders.
+    type: object
+    fields:
+      order_id:
+        type: string
+        description: Primary key of the orders table
+      order_timestamp:
+        type: string
+        format: date-time
+        description: The business timestamp in UTC when the order was successfully registered in the source system and the payment was successful.
+      order_total:
+        type: integer
+        description: Total amount of the order in the smallest monetary unit (e.g., cents).
+  line_items:
+    type: object
+    fields:
+      lines_item_id:
+        type: string
+        description: Primary key of the lines_item_id table
+      order_id:
+        type: string
+        description: Foreign key to the orders table
+      sku:
+        type: string
+        description: The purchased article number""")
 
     data_contract.lint()
     data_contract.test()
     data_contract.export(export_format="odcs")
     data_contract.export(export_format="dbt-model")
     data_contract.export(export_format="dbt-source")
-    data_contract.export(export_format="dbt-staging-sql")
-    data_contract.export(export_format="jsonschema")
+    data_contract.export(export_format="dbt-staging-sql", model="orders")
+    data_contract.export(export_format="jsonschema", model="orders")
```

