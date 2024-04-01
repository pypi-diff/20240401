# Comparing `tmp/deltalake-0.8.1.tar.gz` & `tmp/deltalake-0.9.0.tar.gz`

## Comparing `deltalake-0.8.1.tar` & `deltalake-0.9.0.tar`

### file list

```diff
@@ -1,442 +1,452 @@
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 deltalake-0.8.1/local_dependencies/glibc_version/Cargo.toml
--rw-r--r--   0     1001      123      476 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/glibc_version/README.md
--rw-r--r--   0     1001      123     3361 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/glibc_version/src/lib.rs
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 deltalake-0.8.1/local_dependencies/dynamodb_lock/Cargo.toml
--rw-r--r--   0     1001      123     1096 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/dynamodb_lock/README.md
--rw-r--r--   0     1001      123    32277 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/dynamodb_lock/src/lib.rs
--rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 deltalake-0.8.1/local_dependencies/deltalake/Cargo.toml
--rw-r--r--   0     1001      123      340 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/.gitignore
--rw-r--r--   0     1001      123       24 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/.ignore
--rw-r--r--   0     1001      123     2439 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/README.md
--rw-r--r--   0     1001      123      977 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/benches/read_checkpoint.rs
--rw-r--r--   0     1001      123     1003 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/build.rs
--rw-r--r--   0     1001      123     2592 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/examples/basic_operations.rs
--rw-r--r--   0     1001      123      247 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/examples/read_delta_table.rs
--rw-r--r--   0     1001      123     6871 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/examples/recordbatch-writer.rs
--rw-r--r--   0     1001      123    30521 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/mod.rs
--rw-r--r--   0     1001      123     2355 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/boolean.rs
--rw-r--r--   0     1001      123     1260 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/dictionary/binary.rs
--rw-r--r--   0     1001      123       49 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/dictionary/mod.rs
--rw-r--r--   0     1001      123      583 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/dictionary/primitive.rs
--rw-r--r--   0     1001      123     3752 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/map.rs
--rw-r--r--   0     1001      123    28191 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/mod.rs
--rw-r--r--   0     1001      123     5964 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/primitive.rs
--rw-r--r--   0     1001      123      335 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/stats.rs
--rw-r--r--   0     1001      123     9710 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/string.rs
--rw-r--r--   0     1001      123     4764 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/validity.rs
--rw-r--r--   0     1001      123    24286 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet_read/mod.rs
--rw-r--r--   0     1001      123    16483 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/builder.rs
--rw-r--r--   0     1001      123    29987 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/checkpoints.rs
--rw-r--r--   0     1001      123     3344 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/data_catalog/glue/mod.rs
--rw-r--r--   0     1001      123     2566 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/data_catalog/mod.rs
--rw-r--r--   0     1001      123    62503 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/delta.rs
--rw-r--r--   0     1001      123    32714 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/delta_arrow.rs
--rw-r--r--   0     1001      123    21414 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/delta_config.rs
--rw-r--r--   0     1001      123    47405 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/delta_datafusion.rs
--rw-r--r--   0     1001      123     4034 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/lib.rs
--rw-r--r--   0     1001      123    15843 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/create.rs
--rw-r--r--   0     1001      123     7631 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/filesystem_check.rs
--rw-r--r--   0     1001      123     5566 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/load.rs
--rw-r--r--   0     1001      123     4855 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/mod.rs
--rw-r--r--   0     1001      123    16796 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/optimize.rs
--rw-r--r--   0     1001      123     8052 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/transaction.rs
--rw-r--r--   0     1001      123    12001 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/vacuum.rs
--rw-r--r--   0     1001      123    23128 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/write.rs
--rw-r--r--   0     1001      123    17586 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/operations/writer.rs
--rw-r--r--   0     1001      123     8772 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/partitions.rs
--rw-r--r--   0     1001      123    13412 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/schema.rs
--rw-r--r--   0     1001      123     8705 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/storage/config.rs
--rw-r--r--   0     1001      123    12652 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/storage/file.rs
--rw-r--r--   0     1001      123    13098 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/storage/mod.rs
--rw-r--r--   0     1001      123    29088 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/storage/s3.rs
--rw-r--r--   0     1001      123     3260 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/storage/utils.rs
--rw-r--r--   0     1001      123    16379 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/table_state.rs
--rw-r--r--   0     1001      123    22608 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/table_state_arrow.rs
--rw-r--r--   0     1001      123    16092 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/test_utils.rs
--rw-r--r--   0     1001      123     5711 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/time_utils.rs
--rw-r--r--   0     1001      123    19681 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/writer/json.rs
--rw-r--r--   0     1001      123     4856 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/writer/mod.rs
--rw-r--r--   0     1001      123    19433 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/writer/record_batch.rs
--rw-r--r--   0     1001      123    27191 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/writer/stats.rs
--rw-r--r--   0     1001      123     6074 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/writer/test_utils.rs
--rw-r--r--   0     1001      123    13247 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/src/writer/utils.rs
--rw-r--r--   0     1001      123    14612 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/add_actions_test.rs
--rw-r--r--   0     1001      123    15687 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/checkpoint_writer.rs
--rw-r--r--   0     1001      123     5177 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/command_filesystem_check.rs
--rw-r--r--   0     1001      123    14677 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/command_optimize.rs
--rw-r--r--   0     1001      123     7511 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/command_vacuum.rs
--rw-r--r--   0     1001      123     1163 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/commit_info_format.rs
--rw-r--r--   0     1001      123     2668 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/common/adls.rs
--rw-r--r--   0     1001      123      635 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/common/clock.rs
--rw-r--r--   0     1001      123      781 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/common/datafusion.rs
--rw-r--r--   0     1001      123     5492 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/common/mod.rs
--rw-r--r--   0     1001      123     4351 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/common/s3.rs
--rw-r--r--   0     1001      123      900 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/common/schemas.rs
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/.s3-optimization-0
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/.s3-optimization-1
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/.s3-optimization-2
--rw-r--r--   0     1001      123       92 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/00000000000000000000.crc
--rw-r--r--   0     1001      123     5624 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123   690424 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00000-a496f40c-e091-413a-85f9-b1b69d4b3b4e-c000.snappy.parquet
--rw-r--r--   0     1001      123   786636 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00001-9d9d980b-c500-4f0b-bb96-771a515fbccc-c000.snappy.parquet
--rw-r--r--   0     1001      123   838642 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00002-8826af84-73bd-49a6-a4b9-e39ffed9c15a-c000.snappy.parquet
--rw-r--r--   0     1001      123   879637 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00003-539aff30-2349-4b0d-9726-c18630c6ad90-c000.snappy.parquet
--rw-r--r--   0     1001      123   890662 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00004-1bb9c3e3-c5b0-4d60-8420-23261f58a5eb-c000.snappy.parquet
--rw-r--r--   0     1001      123   895702 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00005-4d47f8ff-94db-4d32-806c-781a1cf123d2-c000.snappy.parquet
--rw-r--r--   0     1001      123   883342 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00006-d0ec7722-b30c-4e1c-92cd-b4fe8d3bb954-c000.snappy.parquet
--rw-r--r--   0     1001      123   325440 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00007-4582392f-9fc2-41b0-ba97-a74b3afc8239-c000.snappy.parquet
--rw-r--r--   0     1001      123      252 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123    15330 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000002.checkpoint.parquet
--rw-r--r--   0     1001      123      251 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123       39 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/_last_checkpoint
--rw-r--r--   0     1001      123       28 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/.gitignore
--rw-r--r--   0     1001      123     1180 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000003.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000004.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000005.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000006.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000007.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000008.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000009.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000010.json
--rw-r--r--   0     1001      123     1083 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000011.json
--rw-r--r--   0     1001      123     1083 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000012.json
--rw-r--r--   0     1001      123       13 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_tombstones/.gitignore
--rw-r--r--   0     1001      123    25261 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.checkpoint.parquet
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000006.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000007.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000008.json
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000009.json
--rw-r--r--   0     1001      123    28176 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.checkpoint.parquet
--rw-r--r--   0     1001      123     1082 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.json
--rw-r--r--   0     1001      123     1083 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000011.json
--rw-r--r--   0     1001      123     1083 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000012.json
--rw-r--r--   0     1001      123       35 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/concurrent_workers/_delta_log/.gitignore
--rw-r--r--   0     1001      123      549 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/concurrent_workers/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-7c2deba3-1994-4fb8-bc07-d46c948aa415-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-cb6b150b-30b8-4662-ad28-ff32ddab96d2-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00001-c373a5bd-85f0-4758-815e-7eb62007a15c-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000000.json.c6b312ca-665d-46ab-93a9-9f87ad2baa92.tmp.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000001.json.641a776e-6e56-4423-a9b0-7efc9e58826a.tmp.crc
--rw-r--r--   0     1001      123       20 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000002.json.e64807e6-437c-44c9-abd2-50e6514d236e.tmp.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000003.json.b374eda7-fa09-48ce-b06c-56025163f6ae.tmp.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/.._last_checkpoint.477ba875-7a14-4e57-9973-1349c21a152c.tmp.crc
--rw-r--r--   0     1001      123      112 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/.00000000000000000003.checkpoint.parquet.crc
--rw-r--r--   0     1001      123      848 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      499 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123     1071 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123    12898 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000003.checkpoint.parquet
--rw-r--r--   0     1001      123      487 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000003.json
--rw-r--r--   0     1001      123       24 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/_last_checkpoint
--rw-r--r--   0     1001      123      396 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet
--rw-r--r--   0     1001      123      396 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-7c2deba3-1994-4fb8-bc07-d46c948aa415-c000.snappy.parquet
--rw-r--r--   0     1001      123      396 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet
--rw-r--r--   0     1001      123      404 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-cb6b150b-30b8-4662-ad28-ff32ddab96d2-c000.snappy.parquet
--rw-r--r--   0     1001      123      400 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet
--rw-r--r--   0     1001      123      400 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet
--rw-r--r--   0     1001      123      400 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00001-c373a5bd-85f0-4758-815e-7eb62007a15c-c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/.part-00000-b0cc5102-6177-4d60-80d3-b5d170011621-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/.part-00007-02b8c308-e5a7-41a8-a653-cb5594582017-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      925 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      590 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      304 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/part-00000-b0cc5102-6177-4d60-80d3-b5d170011621-c000.snappy.parquet
--rw-r--r--   0     1001      123      475 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/part-00007-02b8c308-e5a7-41a8-a653-cb5594582017-c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/.part-00000-04ec9591-0b73-459e-8d18-ba5711d6cbe1-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/.part-00000-c9b90f86-73e6-46c8-93ba-ff6bfaf892a1-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/.part-00001-911a94a2-43f6-4acb-8620-5e68c2654989-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/_change_data/.gitkeep
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_index/.gitkeep
--rw-r--r--   0     1001      123     1154 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      750 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      440 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/part-00000-04ec9591-0b73-459e-8d18-ba5711d6cbe1-c000.snappy.parquet
--rw-r--r--   0     1001      123      440 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/part-00000-c9b90f86-73e6-46c8-93ba-ff6bfaf892a1-c000.snappy.parquet
--rw-r--r--   0     1001      123      445 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/part-00001-911a94a2-43f6-4acb-8620-5e68c2654989-c000.snappy.parquet
--rw-r--r--   0     1001      123       16 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-date/.part-00000-d22c627d-9655-4153-9527-f8995620fa42-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      833 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-date/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      685 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-date/part-00000-d22c627d-9655-4153-9527-f8995620fa42-c000.snappy.parquet
--rw-r--r--   0     1001      123     1044 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      460 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/k=A/part-00000-b1f1dbbb-70bc-4970-893f-9bb772bf246e.c000.snappy.parquet
--rw-r--r--   0     1001      123      460 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/k=__HIVE_DEFAULT_PARTITION__/part-00001-8474ac85-360b-4f58-b3ea-23990c71b932.c000.snappy.parquet
--rw-r--r--   0     1001      123     1138 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=10/y=10.0/.part-00015-24eb4845-2d25-4448-b3bb-5ed7f12635ab.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      402 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=10/y=10.0/part-00015-24eb4845-2d25-4448-b3bb-5ed7f12635ab.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=9/y=9.9/.part-00007-3c50fba1-4264-446c-9c67-d8e24a1ccf83.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      402 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=9/y=9.9/part-00007-3c50fba1-4264-446c-9c67-d8e24a1ccf83.c000.snappy.parquet
--rw-r--r--   0     1001      123     2235 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=1/day=1/.part-00000-8eafa330-3be9-4a39-ad78-fd13c2027c7e.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      414 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=1/day=1/part-00000-8eafa330-3be9-4a39-ad78-fd13c2027c7e.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=3/.part-00000-94d16827-f2fd-42cd-a060-f67ccc63ced9.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      414 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=3/part-00000-94d16827-f2fd-42cd-a060-f67ccc63ced9.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=5/.part-00000-89cdd4c8-2af7-4add-8ea3-3990b2f027b5.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      414 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=5/part-00000-89cdd4c8-2af7-4add-8ea3-3990b2f027b5.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=20/.part-00000-9275fdf4-3961-4184-baa0-1c8a2bb98104.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      407 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=20/part-00000-9275fdf4-3961-4184-baa0-1c8a2bb98104.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=4/.part-00000-6dc763c0-3e8b-4d52-b19e-1f92af3fbb25.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      414 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=4/part-00000-6dc763c0-3e8b-4d52-b19e-1f92af3fbb25.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=4/day=5/.part-00000-c5856301-3439-4032-a6fc-22b7bc92bebb.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      414 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=4/day=5/part-00000-c5856301-3439-4032-a6fc-22b7bc92bebb.c000.snappy.parquet
--rw-r--r--   0     1001      123     1037 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=A%2FA/.part-00007-b350e235-2832-45df-9918-6cab4f7578f7.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      460 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=A%2FA/part-00007-b350e235-2832-45df-9918-6cab4f7578f7.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=B%20B/.part-00015-e9abbc6f-85e9-457b-be8e-e9f5b8a22890.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      460 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=B%20B/part-00015-e9abbc6f-85e9-457b-be8e-e9f5b8a22890.c000.snappy.parquet
--rw-r--r--   0     1001      123     1890 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.crc
--rw-r--r--   0     1001      123     1040 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123     3636 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.crc
--rw-r--r--   0     1001      123     3826 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.json
--rw-r--r--   0     1001      123     3638 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.crc
--rw-r--r--   0     1001      123     1694 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.json
--rw-r--r--   0     1001      123    30676 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.checkpoint.parquet
--rw-r--r--   0     1001      123     3721 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.crc
--rw-r--r--   0     1001      123     3958 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.json
--rw-r--r--   0     1001      123     3721 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.crc
--rw-r--r--   0     1001      123     1697 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.json
--rw-r--r--   0     1001      123     3721 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.crc
--rw-r--r--   0     1001      123     1697 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.json
--rw-r--r--   0     1001      123       25 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/_last_checkpoint
--rw-r--r--   0     1001      123     5488 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-1c2d1a32-02dc-484f-87ff-4328ea56045d-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-28925d3a-bdf2-411e-bca9-b067444cbcb0-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-6630b7c4-0aca-405b-be86-68a812f2e4c8-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-74151571-7ec6-4bd6-9293-b5daab2ce667-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-7a509247-4f58-4453-9202-51d75dee59af-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-8e0aefe1-6645-4601-ac29-68cba64023b5-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-b26ba634-874c-45b0-a7ff-2f0395a53966-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-c4c8caec-299d-42a4-b50c-5a4bf724c037-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-ce300400-58ff-4b8f-8ba9-49422fdf9f2e-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e1262b3e-2959-4910-aea9-4eaf92f0c68c-c000.snappy.parquet
--rw-r--r--   0     1001      123     5489 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e8e3753f-e2f6-4c9f-98f9-8f3d346727ba-c000.snappy.parquet
--rw-r--r--   0     1001      123     5731 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-f73ff835-0571-4d67-ac43-4fbf948bfb9b-c000.snappy.parquet
--rw-r--r--   0     1001      123       24 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123     1778 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=4/c2=c/.part-00003-f525f459-34f9-46f5-82d6-d42121d883fd.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      452 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=4/c2=c/part-00003-f525f459-34f9-46f5-82d6-d42121d883fd.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=5/c2=b/.part-00007-4e73fa3b-2c88-424a-8051-f8b54328ffdb.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      452 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=5/c2=b/part-00007-4e73fa3b-2c88-424a-8051-f8b54328ffdb.c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=6/c2=a/.part-00011-10619b10-b691-4fd0-acc4-2a9608499d7c.c000.snappy.parquet.crc
--rw-r--r--   0     1001      123      452 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=6/c2=a/part-00011-10619b10-b691-4fd0-acc4-2a9608499d7c.c000.snappy.parquet
--rw-r--r--   0     1001      123       40 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/.part-00000-182665f0-30df-470d-a5cb-8d9d483ed390-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       40 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/.part-00001-2e274fe7-eb75-4b73-8c72-423ee747abc0-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123     2213 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123     3627 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00000-182665f0-30df-470d-a5cb-8d9d483ed390-c000.snappy.parquet
--rw-r--r--   0     1001      123     3644 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00001-2e274fe7-eb75-4b73-8c72-423ee747abc0-c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/.part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/.part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/.part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/.part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       35 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/_delta_log/.gitignore
--rw-r--r--   0     1001      123      549 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      396 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet
--rw-r--r--   0     1001      123      396 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet
--rw-r--r--   0     1001      123      400 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet
--rw-r--r--   0     1001      123      400 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00000-2befed33-c358-4768-a43c-3eda0d2a499d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00000-a72b1fb3-f2df-41fe-a8f0-e65b746382dd-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00000-a922ea3b-ffc2-4ca1-9074-a278c24c4449-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00000-c1777d7d-89d9-4790-b38a-6ee7e24456b1-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00000-f17fcbf5-e0dc-40ba-adae-ce66d1fcaef6-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00001-7891c33d-cedc-47c3-88a6-abcfb049d3b4-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00001-bb70d2ba-c196-4df2-9c85-f34969ad3aa9-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00001-c506e79a-0bf8-4e2b-a42b-9731b2e490ae-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00003-508ae4aa-801c-4c2c-a923-f6f89930a5c1-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00003-53f42606-6cda-4f13-8d07-599a21197296-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00004-315835fe-fb44-4562-98f6-5e6cfa3ae45d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00004-80938522-09c0-420c-861f-5a649e3d9674-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00004-95c9bc2c-ac85-4581-b3cc-84502b0c314f-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00005-94a0861b-6455-4bd9-a080-73e02491c643-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00006-46f2ff20-eb5d-4dda-8498-7bfb2940713b-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00006-63ce9deb-bc0f-482d-b9a1-7e717b67f294-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00007-3a0e4727-de0d-41b6-81ef-5223cf40f025-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00007-94f725e2-3963-4b00-9e83-e31021a93cf9-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00011-42f838f9-a911-40af-98f5-2fccfa1b123f-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00045-332fe409-7705-45b1-8d34-a0018cf73b70-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00049-d3095817-de74-49c1-a888-81565a40161d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00058-b462c4cb-0c48-4148-8475-e21d2a2935f8-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00068-90650739-6a8e-492b-9403-53e33b3778ac-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00069-c78b4dd8-f955-4643-816f-cbd30a3f8c1b-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00077-2fcb1c7c-5390-48ee-93f6-0acf11199a0d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00107-3f6c2aa0-fc28-4f4c-be15-135e15b398f4-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00112-07fd790a-11dc-4fde-9acd-623e740be992-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00116-bc66759e-6381-4f34-8cd4-6688aad8585d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00121-d8bc3e53-d2f2-48ce-9909-78da7294ffbd-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00128-b31c3b81-24da-4a90-a8b4-578c9e9a218d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00140-e9b1971d-d708-43fb-b07f-975d2226b800-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00143-03ceb88e-5283-4193-aa43-993cdf937fd3-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00150-ec6643fc-4963-4871-9613-f5ad1940b689-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00154-4630673a-5227-48fb-a03d-e356fcd1564a-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00164-bf40481c-4afd-4c02-befa-90f056c2d77a-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/.part-00190-8ac0ae67-fb1d-461d-a3d3-8dc112766ff5-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123     1522 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123     4449 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123     4307 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123      816 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000003.json
--rw-r--r--   0     1001      123      649 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000004.json
--rw-r--r--   0     1001      123      262 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00000-2befed33-c358-4768-a43c-3eda0d2a499d-c000.snappy.parquet
--rw-r--r--   0     1001      123      262 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00000-a72b1fb3-f2df-41fe-a8f0-e65b746382dd-c000.snappy.parquet
--rw-r--r--   0     1001      123      262 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00000-a922ea3b-ffc2-4ca1-9074-a278c24c4449-c000.snappy.parquet
--rw-r--r--   0     1001      123      262 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00000-c1777d7d-89d9-4790-b38a-6ee7e24456b1-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00000-f17fcbf5-e0dc-40ba-adae-ce66d1fcaef6-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00001-7891c33d-cedc-47c3-88a6-abcfb049d3b4-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00001-bb70d2ba-c196-4df2-9c85-f34969ad3aa9-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00001-c506e79a-0bf8-4e2b-a42b-9731b2e490ae-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00003-508ae4aa-801c-4c2c-a923-f6f89930a5c1-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00003-53f42606-6cda-4f13-8d07-599a21197296-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00004-315835fe-fb44-4562-98f6-5e6cfa3ae45d-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00004-80938522-09c0-420c-861f-5a649e3d9674-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00004-95c9bc2c-ac85-4581-b3cc-84502b0c314f-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00005-94a0861b-6455-4bd9-a080-73e02491c643-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00006-46f2ff20-eb5d-4dda-8498-7bfb2940713b-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00006-63ce9deb-bc0f-482d-b9a1-7e717b67f294-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00007-3a0e4727-de0d-41b6-81ef-5223cf40f025-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00007-94f725e2-3963-4b00-9e83-e31021a93cf9-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00011-42f838f9-a911-40af-98f5-2fccfa1b123f-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00045-332fe409-7705-45b1-8d34-a0018cf73b70-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00049-d3095817-de74-49c1-a888-81565a40161d-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00058-b462c4cb-0c48-4148-8475-e21d2a2935f8-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00068-90650739-6a8e-492b-9403-53e33b3778ac-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00069-c78b4dd8-f955-4643-816f-cbd30a3f8c1b-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00077-2fcb1c7c-5390-48ee-93f6-0acf11199a0d-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00107-3f6c2aa0-fc28-4f4c-be15-135e15b398f4-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00112-07fd790a-11dc-4fde-9acd-623e740be992-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00116-bc66759e-6381-4f34-8cd4-6688aad8585d-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00121-d8bc3e53-d2f2-48ce-9909-78da7294ffbd-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00128-b31c3b81-24da-4a90-a8b4-578c9e9a218d-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00140-e9b1971d-d708-43fb-b07f-975d2226b800-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00143-03ceb88e-5283-4193-aa43-993cdf937fd3-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00150-ec6643fc-4963-4871-9613-f5ad1940b689-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00154-4630673a-5227-48fb-a03d-e356fcd1564a-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00164-bf40481c-4afd-4c02-befa-90f056c2d77a-c000.snappy.parquet
--rw-r--r--   0     1001      123      429 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/part-00190-8ac0ae67-fb1d-461d-a3d3-8dc112766ff5-c000.snappy.parquet
--rw-r--r--   0     1001      123     1155 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_change_data/cdc-00000-a846ce80-2eec-484d-bef7-0e63557786ca.c000.snappy.parquet
--rw-r--r--   0     1001      123     1997 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.crc
--rw-r--r--   0     1001      123     1052 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123     2476 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.crc
--rw-r--r--   0     1001      123      991 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123     2477 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.crc
--rw-r--r--   0     1001      123     1618 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123     1026 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-7444aec4-710a-4a4c-8abe-3323499043e9.c000.snappy.parquet
--rw-r--r--   0     1001      123      815 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-996384f7-3fc5-4a5f-9921-6e56269ec2c9-c000.snappy.parquet
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-136c36f5-639d-4e95-bb0f-15cde3fb14eb-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-1abe25d3-0da6-46c5-98c1-7a69872fd797-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-3810fbe0-9892-431d-bcfd-7de5788dfe8d-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-3fa65c69-4e55-4b18-a195-5f1ae583e553-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-72ecc4d6-2e44-4df4-99e6-23f1ac2b7b7c-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-7d239c98-d74b-4b02-b3f6-9f256992c633-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-8e7dc8c1-337b-40b8-a411-46d4295da531-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-9afd9224-729f-4420-a05e-8032113a6568-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-e93060ad-9c8c-4170-a9da-7c6f53f6406b-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-e9c6df9a-e585-4c70-bc1f-de9bd8ae025b-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       12 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-f0e955c5-a1e3-4eec-834e-dcc098fc9005-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       96 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/.00000000000000000010.checkpoint.parquet.crc
--rw-r--r--   0     1001      123      752 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000002.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000003.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000004.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000005.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000006.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000007.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000008.json
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000009.json
--rw-r--r--   0     1001      123    11088 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000010.checkpoint.parquet
--rw-r--r--   0     1001      123      408 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000010.json
--rw-r--r--   0     1001      123       25 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/_last_checkpoint
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-136c36f5-639d-4e95-bb0f-15cde3fb14eb-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-1abe25d3-0da6-46c5-98c1-7a69872fd797-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-3810fbe0-9892-431d-bcfd-7de5788dfe8d-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-3fa65c69-4e55-4b18-a195-5f1ae583e553-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-72ecc4d6-2e44-4df4-99e6-23f1ac2b7b7c-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-7d239c98-d74b-4b02-b3f6-9f256992c633-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-8e7dc8c1-337b-40b8-a411-46d4295da531-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-9afd9224-729f-4420-a05e-8032113a6568-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-e93060ad-9c8c-4170-a9da-7c6f53f6406b-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-e9c6df9a-e585-4c70-bc1f-de9bd8ae025b-c000.snappy.parquet
--rw-r--r--   0     1001      123      442 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-f0e955c5-a1e3-4eec-834e-dcc098fc9005-c000.snappy.parquet
--rw-r--r--   0     1001      123       89 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/_delta_log/00000000000000000000.crc
--rw-r--r--   0     1001      123     2017 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123     1201 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00000-a9dd181d-61aa-491d-b3c9-3eea548de6cb-c000.snappy.parquet
--rw-r--r--   0     1001      123     1201 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00001-f804d355-db40-4e13-a624-ddd50ce7f5c4-c000.snappy.parquet
--rw-r--r--   0     1001      123    25227 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/datafusion_test.rs
--rw-r--r--   0     1001      123     3325 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/fs_common/mod.rs
--rw-r--r--   0     1001      123     3361 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/integration_checkpoint.rs
--rw-r--r--   0     1001      123     9351 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/integration_commit.rs
--rw-r--r--   0     1001      123     4774 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/integration_concurrent_writes.rs
--rw-r--r--   0     1001      123     2369 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/integration_datafusion.rs
--rw-r--r--   0     1001      123    13887 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/integration_object_store.rs
--rw-r--r--   0     1001      123     7012 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/integration_read.rs
--rw-r--r--   0     1001      123     4640 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/read_delta_partitions_test.rs
--rw-r--r--   0     1001      123    20058 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/read_delta_test.rs
--rw-r--r--   0     1001      123     8330 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/repair_s3_rename_test.rs
--rw-r--r--   0     1001      123     2335 2023-03-13 22:51:30.000000 deltalake-0.8.1/local_dependencies/deltalake/tests/time_travel.rs
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 deltalake-0.8.1/Cargo.toml
--rw-r--r--   0     1001      123      223 2023-03-13 22:51:30.000000 deltalake-0.8.1/.cargo/config
--rw-r--r--   0     1001      123      207 2023-03-13 22:51:30.000000 deltalake-0.8.1/.gitignore
--rw-r--r--   0     1001      123     1328 2023-03-13 22:51:30.000000 deltalake-0.8.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123    10257 2023-03-13 22:51:30.000000 deltalake-0.8.1/LICENSE.txt
--rw-r--r--   0     1001      123     2926 2023-03-13 22:51:30.000000 deltalake-0.8.1/Makefile
--rw-r--r--   0     1001      123     3151 2023-03-13 22:51:30.000000 deltalake-0.8.1/README.md
--rw-r--r--   0     1001      123      233 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/__init__.py
--rw-r--r--   0     1001      123     7086 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/_internal.pyi
--rw-r--r--   0     1001      123      146 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/data_catalog.py
--rw-r--r--   0     1001      123     2012 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/fs.py
--rw-r--r--   0     1001      123     1503 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/schema.py
--rw-r--r--   0     1001      123    20092 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/table.py
--rw-r--r--   0     1001      123    18675 2023-03-13 22:51:30.000000 deltalake-0.8.1/deltalake/writer.py
--rw-r--r--   0     1001      123      638 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/Makefile
--rw-r--r--   0     1001      123      799 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/make.bat
--rw-r--r--   0     1001      123     1576 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/_ext/edit_on_github.py
--rw-r--r--   0     1001      123       70 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/_static/.gitignore
--rw-r--r--   0     1001      123      832 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/api_reference.rst
--rw-r--r--   0     1001      123     3328 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/conf.py
--rw-r--r--   0     1001      123     1289 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/index.rst
--rw-r--r--   0     1001      123      295 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/installation.rst
--rw-r--r--   0     1001      123    17736 2023-03-13 22:51:30.000000 deltalake-0.8.1/docs/source/usage.rst
--rw-r--r--   0     1001      123     2350 2023-03-13 22:51:30.000000 deltalake-0.8.1/pyproject.toml
--rw-r--r--   0     1001      123    17824 2023-03-13 22:51:30.000000 deltalake-0.8.1/src/filesystem.rs
--rw-r--r--   0     1001      123    29194 2023-03-13 22:51:30.000000 deltalake-0.8.1/src/lib.rs
--rw-r--r--   0     1001      123    35627 2023-03-13 22:51:30.000000 deltalake-0.8.1/src/schema.rs
--rw-r--r--   0     1001      123     2674 2023-03-13 22:51:30.000000 deltalake-0.8.1/src/utils.rs
--rw-r--r--   0     1001      123       39 2023-03-13 22:51:30.000000 deltalake-0.8.1/stubs/pandas/__init__.pyi
--rw-r--r--   0     1001      123      460 2023-03-13 22:51:30.000000 deltalake-0.8.1/stubs/pyarrow/__init__.pyi
--rw-r--r--   0     1001      123      186 2023-03-13 22:51:30.000000 deltalake-0.8.1/stubs/pyarrow/dataset.pyi
--rw-r--r--   0     1001      123      157 2023-03-13 22:51:30.000000 deltalake-0.8.1/stubs/pyarrow/fs.pyi
--rw-r--r--   0     1001      123       47 2023-03-13 22:51:30.000000 deltalake-0.8.1/stubs/pyarrow/lib.pyi
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/__init__.py
--rw-r--r--   0     1001      123     6551 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/conftest.py
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/data_acceptance/__init__.py
--rw-r--r--   0     1001      123     3094 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/data_acceptance/test_reader.py
--rw-r--r--   0     1001      123        0 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/pyspark_integration/__init__.py
--rw-r--r--   0     1001      123     3368 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/pyspark_integration/test_write_to_pyspark.py
--rw-r--r--   0     1001      123     1944 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/pyspark_integration/test_writer_readable.py
--rw-r--r--   0     1001      123     1324 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/pyspark_integration/utils.py
--rw-r--r--   0     1001      123     1974 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_benchmark.py
--rw-r--r--   0     1001      123      813 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_checkpoint.py
--rw-r--r--   0     1001      123     5330 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_file_system_handler.py
--rw-r--r--   0     1001      123     8557 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_fs.py
--rw-r--r--   0     1001      123     6699 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_schema.py
--rw-r--r--   0     1001      123    19416 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_table_read.py
--rw-r--r--   0     1001      123     2304 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_vacuum.py
--rw-r--r--   0     1001      123      150 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_version.py
--rw-r--r--   0     1001      123    24537 2023-03-13 22:51:30.000000 deltalake-0.8.1/tests/test_writer.py
--rw-r--r--   0        0        0   107906 2023-03-13 22:53:40.000000 deltalake-0.8.1/Cargo.lock
--rw-r--r--   0        0        0     4806 1970-01-01 00:00:00.000000 deltalake-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 deltalake-0.9.0/local_dependencies/glibc_version/Cargo.toml
+-rw-r--r--   0     1001      123      476 2023-05-06 16:45:02.000000 deltalake-0.9.0/local_dependencies/glibc_version/README.md
+-rw-r--r--   0     1001      123     3361 2023-05-06 16:45:02.000000 deltalake-0.9.0/local_dependencies/glibc_version/src/lib.rs
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 deltalake-0.9.0/local_dependencies/dynamodb_lock/Cargo.toml
+-rw-r--r--   0     1001      123     1096 2023-05-06 16:45:02.000000 deltalake-0.9.0/local_dependencies/dynamodb_lock/README.md
+-rw-r--r--   0     1001      123    32277 2023-05-06 16:45:02.000000 deltalake-0.9.0/local_dependencies/dynamodb_lock/src/lib.rs
+-rw-r--r--   0        0        0     4258 1970-01-01 00:00:00.000000 deltalake-0.9.0/local_dependencies/deltalake/Cargo.toml
+-rw-r--r--   0     1001      123      340 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/.gitignore
+-rw-r--r--   0     1001      123       24 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/.ignore
+-rw-r--r--   0     1001      123     2609 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/README.md
+-rw-r--r--   0     1001      123      977 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/benches/read_checkpoint.rs
+-rw-r--r--   0     1001      123     1003 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/build.rs
+-rw-r--r--   0     1001      123     2592 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/examples/basic_operations.rs
+-rw-r--r--   0     1001      123      247 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/examples/read_delta_table.rs
+-rw-r--r--   0     1001      123     6265 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/examples/recordbatch-writer.rs
+-rw-r--r--   0     1001      123    31227 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/mod.rs
+-rw-r--r--   0     1001      123     2355 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/boolean.rs
+-rw-r--r--   0     1001      123     1260 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/dictionary/binary.rs
+-rw-r--r--   0     1001      123       49 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/dictionary/mod.rs
+-rw-r--r--   0     1001      123      583 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/dictionary/primitive.rs
+-rw-r--r--   0     1001      123     3752 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/map.rs
+-rw-r--r--   0     1001      123    28191 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/mod.rs
+-rw-r--r--   0     1001      123     5964 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/primitive.rs
+-rw-r--r--   0     1001      123      335 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/stats.rs
+-rw-r--r--   0     1001      123     9710 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/string.rs
+-rw-r--r--   0     1001      123     4764 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/validity.rs
+-rw-r--r--   0     1001      123    24286 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet_read/mod.rs
+-rw-r--r--   0     1001      123    21036 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/builder.rs
+-rw-r--r--   0     1001      123    30294 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/checkpoints.rs
+-rw-r--r--   0     1001      123     3344 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/data_catalog/glue/mod.rs
+-rw-r--r--   0     1001      123     3532 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/data_catalog/mod.rs
+-rw-r--r--   0     1001      123     4074 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/data_catalog/unity/mod.rs
+-rw-r--r--   0     1001      123    64211 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/delta.rs
+-rw-r--r--   0     1001      123    39814 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/delta_arrow.rs
+-rw-r--r--   0     1001      123    21445 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/delta_config.rs
+-rw-r--r--   0     1001      123    47522 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/delta_datafusion.rs
+-rw-r--r--   0     1001      123     4065 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/lib.rs
+-rw-r--r--   0     1001      123    15865 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/create.rs
+-rw-r--r--   0     1001      123     7508 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/filesystem_check.rs
+-rw-r--r--   0     1001      123     5596 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/load.rs
+-rw-r--r--   0     1001      123     4809 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/mod.rs
+-rw-r--r--   0     1001      123    16906 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/optimize.rs
+-rw-r--r--   0     1001      123    33350 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/transaction/conflict_checker.rs
+-rw-r--r--   0     1001      123     9228 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/transaction/mod.rs
+-rw-r--r--   0     1001      123    15681 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/transaction/state.rs
+-rw-r--r--   0     1001      123     4734 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/transaction/test_utils.rs
+-rw-r--r--   0     1001      123    12001 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/vacuum.rs
+-rw-r--r--   0     1001      123    22477 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/write.rs
+-rw-r--r--   0     1001      123    17586 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/operations/writer.rs
+-rw-r--r--   0     1001      123     8772 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/partitions.rs
+-rw-r--r--   0     1001      123    13599 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/schema.rs
+-rw-r--r--   0     1001      123     9223 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/storage/config.rs
+-rw-r--r--   0     1001      123    13427 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/storage/file.rs
+-rw-r--r--   0     1001      123    12837 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/storage/mod.rs
+-rw-r--r--   0     1001      123    29088 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/storage/s3.rs
+-rw-r--r--   0     1001      123     4014 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/storage/utils.rs
+-rw-r--r--   0     1001      123    16534 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/table_state.rs
+-rw-r--r--   0     1001      123    22608 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/table_state_arrow.rs
+-rw-r--r--   0     1001      123    19711 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/test_utils.rs
+-rw-r--r--   0     1001      123     5711 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/time_utils.rs
+-rw-r--r--   0     1001      123    19681 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/writer/json.rs
+-rw-r--r--   0     1001      123     4885 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/writer/mod.rs
+-rw-r--r--   0     1001      123    19433 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/writer/record_batch.rs
+-rw-r--r--   0     1001      123    27191 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/writer/stats.rs
+-rw-r--r--   0     1001      123     6096 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/writer/test_utils.rs
+-rw-r--r--   0     1001      123    13553 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/src/writer/utils.rs
+-rw-r--r--   0     1001      123    14612 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/add_actions_test.rs
+-rw-r--r--   0     1001      123    15687 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/checkpoint_writer.rs
+-rw-r--r--   0     1001      123     6432 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/command_filesystem_check.rs
+-rw-r--r--   0     1001      123    14096 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/command_optimize.rs
+-rw-r--r--   0     1001      123     7511 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/command_vacuum.rs
+-rw-r--r--   0     1001      123     1176 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/commit_info_format.rs
+-rw-r--r--   0     1001      123     2668 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/adls.rs
+-rw-r--r--   0     1001      123      635 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/clock.rs
+-rw-r--r--   0     1001      123      655 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/datafusion.rs
+-rw-r--r--   0     1001      123      433 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/hdfs.rs
+-rw-r--r--   0     1001      123     5624 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/mod.rs
+-rw-r--r--   0     1001      123     4351 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/s3.rs
+-rw-r--r--   0     1001      123      900 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/common/schemas.rs
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/.s3-optimization-0
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/.s3-optimization-1
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/.s3-optimization-2
+-rw-r--r--   0     1001      123       92 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/00000000000000000000.crc
+-rw-r--r--   0     1001      123     5624 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123   690424 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00000-a496f40c-e091-413a-85f9-b1b69d4b3b4e-c000.snappy.parquet
+-rw-r--r--   0     1001      123   786636 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00001-9d9d980b-c500-4f0b-bb96-771a515fbccc-c000.snappy.parquet
+-rw-r--r--   0     1001      123   838642 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00002-8826af84-73bd-49a6-a4b9-e39ffed9c15a-c000.snappy.parquet
+-rw-r--r--   0     1001      123   879637 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00003-539aff30-2349-4b0d-9726-c18630c6ad90-c000.snappy.parquet
+-rw-r--r--   0     1001      123   890662 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00004-1bb9c3e3-c5b0-4d60-8420-23261f58a5eb-c000.snappy.parquet
+-rw-r--r--   0     1001      123   895702 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00005-4d47f8ff-94db-4d32-806c-781a1cf123d2-c000.snappy.parquet
+-rw-r--r--   0     1001      123   883342 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00006-d0ec7722-b30c-4e1c-92cd-b4fe8d3bb954-c000.snappy.parquet
+-rw-r--r--   0     1001      123   325440 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00007-4582392f-9fc2-41b0-ba97-a74b3afc8239-c000.snappy.parquet
+-rw-r--r--   0     1001      123      252 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123    15330 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000002.checkpoint.parquet
+-rw-r--r--   0     1001      123      251 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123       39 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/_last_checkpoint
+-rw-r--r--   0     1001      123       28 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/.gitignore
+-rw-r--r--   0     1001      123     1180 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000003.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000004.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000005.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000006.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000007.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000008.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000009.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000010.json
+-rw-r--r--   0     1001      123     1083 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000011.json
+-rw-r--r--   0     1001      123     1083 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000012.json
+-rw-r--r--   0     1001      123       13 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_tombstones/.gitignore
+-rw-r--r--   0     1001      123    25261 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.checkpoint.parquet
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000006.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000007.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000008.json
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000009.json
+-rw-r--r--   0     1001      123    28176 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.checkpoint.parquet
+-rw-r--r--   0     1001      123     1082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.json
+-rw-r--r--   0     1001      123     1083 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000011.json
+-rw-r--r--   0     1001      123     1083 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000012.json
+-rw-r--r--   0     1001      123       35 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/concurrent_workers/_delta_log/.gitignore
+-rw-r--r--   0     1001      123      549 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/concurrent_workers/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-7c2deba3-1994-4fb8-bc07-d46c948aa415-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00000-cb6b150b-30b8-4662-ad28-ff32ddab96d2-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/.part-00001-c373a5bd-85f0-4758-815e-7eb62007a15c-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000000.json.c6b312ca-665d-46ab-93a9-9f87ad2baa92.tmp.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000001.json.641a776e-6e56-4423-a9b0-7efc9e58826a.tmp.crc
+-rw-r--r--   0     1001      123       20 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000002.json.e64807e6-437c-44c9-abd2-50e6514d236e.tmp.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/..00000000000000000003.json.b374eda7-fa09-48ce-b06c-56025163f6ae.tmp.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/.._last_checkpoint.477ba875-7a14-4e57-9973-1349c21a152c.tmp.crc
+-rw-r--r--   0     1001      123      112 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/.00000000000000000003.checkpoint.parquet.crc
+-rw-r--r--   0     1001      123      848 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      499 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123     1071 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123    12898 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000003.checkpoint.parquet
+-rw-r--r--   0     1001      123      487 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000003.json
+-rw-r--r--   0     1001      123       24 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/_last_checkpoint
+-rw-r--r--   0     1001      123      396 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet
+-rw-r--r--   0     1001      123      396 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-7c2deba3-1994-4fb8-bc07-d46c948aa415-c000.snappy.parquet
+-rw-r--r--   0     1001      123      396 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet
+-rw-r--r--   0     1001      123      404 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00000-cb6b150b-30b8-4662-ad28-ff32ddab96d2-c000.snappy.parquet
+-rw-r--r--   0     1001      123      400 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet
+-rw-r--r--   0     1001      123      400 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet
+-rw-r--r--   0     1001      123      400 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/part-00001-c373a5bd-85f0-4758-815e-7eb62007a15c-c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/.part-00000-b0cc5102-6177-4d60-80d3-b5d170011621-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/.part-00007-02b8c308-e5a7-41a8-a653-cb5594582017-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      925 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      590 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      304 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/part-00000-b0cc5102-6177-4d60-80d3-b5d170011621-c000.snappy.parquet
+-rw-r--r--   0     1001      123      475 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/part-00007-02b8c308-e5a7-41a8-a653-cb5594582017-c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/.part-00000-04ec9591-0b73-459e-8d18-ba5711d6cbe1-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/.part-00000-c9b90f86-73e6-46c8-93ba-ff6bfaf892a1-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/.part-00001-911a94a2-43f6-4acb-8620-5e68c2654989-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/_change_data/.gitkeep
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_index/.gitkeep
+-rw-r--r--   0     1001      123     1154 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      750 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      440 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/part-00000-04ec9591-0b73-459e-8d18-ba5711d6cbe1-c000.snappy.parquet
+-rw-r--r--   0     1001      123      440 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/part-00000-c9b90f86-73e6-46c8-93ba-ff6bfaf892a1-c000.snappy.parquet
+-rw-r--r--   0     1001      123      445 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/part-00001-911a94a2-43f6-4acb-8620-5e68c2654989-c000.snappy.parquet
+-rw-r--r--   0     1001      123       16 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-date/.part-00000-d22c627d-9655-4153-9527-f8995620fa42-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      833 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-date/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      685 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-date/part-00000-d22c627d-9655-4153-9527-f8995620fa42-c000.snappy.parquet
+-rw-r--r--   0     1001      123     1044 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      460 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/k=A/part-00000-b1f1dbbb-70bc-4970-893f-9bb772bf246e.c000.snappy.parquet
+-rw-r--r--   0     1001      123      460 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/k=__HIVE_DEFAULT_PARTITION__/part-00001-8474ac85-360b-4f58-b3ea-23990c71b932.c000.snappy.parquet
+-rw-r--r--   0     1001      123     1138 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=10/y=10.0/.part-00015-24eb4845-2d25-4448-b3bb-5ed7f12635ab.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      402 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=10/y=10.0/part-00015-24eb4845-2d25-4448-b3bb-5ed7f12635ab.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=9/y=9.9/.part-00007-3c50fba1-4264-446c-9c67-d8e24a1ccf83.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      402 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/x=9/y=9.9/part-00007-3c50fba1-4264-446c-9c67-d8e24a1ccf83.c000.snappy.parquet
+-rw-r--r--   0     1001      123     2235 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=1/day=1/.part-00000-8eafa330-3be9-4a39-ad78-fd13c2027c7e.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      414 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=1/day=1/part-00000-8eafa330-3be9-4a39-ad78-fd13c2027c7e.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=3/.part-00000-94d16827-f2fd-42cd-a060-f67ccc63ced9.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      414 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=3/part-00000-94d16827-f2fd-42cd-a060-f67ccc63ced9.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=5/.part-00000-89cdd4c8-2af7-4add-8ea3-3990b2f027b5.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      414 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2020/month=2/day=5/part-00000-89cdd4c8-2af7-4add-8ea3-3990b2f027b5.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=20/.part-00000-9275fdf4-3961-4184-baa0-1c8a2bb98104.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      407 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=20/part-00000-9275fdf4-3961-4184-baa0-1c8a2bb98104.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=4/.part-00000-6dc763c0-3e8b-4d52-b19e-1f92af3fbb25.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      414 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=12/day=4/part-00000-6dc763c0-3e8b-4d52-b19e-1f92af3fbb25.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=4/day=5/.part-00000-c5856301-3439-4032-a6fc-22b7bc92bebb.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      414 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/year=2021/month=4/day=5/part-00000-c5856301-3439-4032-a6fc-22b7bc92bebb.c000.snappy.parquet
+-rw-r--r--   0     1001      123     1037 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=A%2FA/.part-00007-b350e235-2832-45df-9918-6cab4f7578f7.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      460 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=A%2FA/part-00007-b350e235-2832-45df-9918-6cab4f7578f7.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=B%20B/.part-00015-e9abbc6f-85e9-457b-be8e-e9f5b8a22890.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      460 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/x=B%20B/part-00015-e9abbc6f-85e9-457b-be8e-e9f5b8a22890.c000.snappy.parquet
+-rw-r--r--   0     1001      123     1890 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.crc
+-rw-r--r--   0     1001      123     1040 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     3636 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.crc
+-rw-r--r--   0     1001      123     3826 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.json
+-rw-r--r--   0     1001      123     3638 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.crc
+-rw-r--r--   0     1001      123     1694 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.json
+-rw-r--r--   0     1001      123    30676 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.checkpoint.parquet
+-rw-r--r--   0     1001      123     3721 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.crc
+-rw-r--r--   0     1001      123     3958 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.json
+-rw-r--r--   0     1001      123     3721 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.crc
+-rw-r--r--   0     1001      123     1697 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.json
+-rw-r--r--   0     1001      123     3721 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.crc
+-rw-r--r--   0     1001      123     1697 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.json
+-rw-r--r--   0     1001      123       25 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/_last_checkpoint
+-rw-r--r--   0     1001      123     5488 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-1c2d1a32-02dc-484f-87ff-4328ea56045d-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-28925d3a-bdf2-411e-bca9-b067444cbcb0-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-6630b7c4-0aca-405b-be86-68a812f2e4c8-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-74151571-7ec6-4bd6-9293-b5daab2ce667-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-7a509247-4f58-4453-9202-51d75dee59af-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-8e0aefe1-6645-4601-ac29-68cba64023b5-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-b26ba634-874c-45b0-a7ff-2f0395a53966-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-c4c8caec-299d-42a4-b50c-5a4bf724c037-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-ce300400-58ff-4b8f-8ba9-49422fdf9f2e-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e1262b3e-2959-4910-aea9-4eaf92f0c68c-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5489 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e8e3753f-e2f6-4c9f-98f9-8f3d346727ba-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5731 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-f73ff835-0571-4d67-ac43-4fbf948bfb9b-c000.snappy.parquet
+-rw-r--r--   0     1001      123       24 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123     1778 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=4/c2=c/.part-00003-f525f459-34f9-46f5-82d6-d42121d883fd.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      452 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=4/c2=c/part-00003-f525f459-34f9-46f5-82d6-d42121d883fd.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=5/c2=b/.part-00007-4e73fa3b-2c88-424a-8051-f8b54328ffdb.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      452 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=5/c2=b/part-00007-4e73fa3b-2c88-424a-8051-f8b54328ffdb.c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=6/c2=a/.part-00011-10619b10-b691-4fd0-acc4-2a9608499d7c.c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123      452 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/c1=6/c2=a/part-00011-10619b10-b691-4fd0-acc4-2a9608499d7c.c000.snappy.parquet
+-rw-r--r--   0     1001      123       40 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/.part-00000-182665f0-30df-470d-a5cb-8d9d483ed390-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       40 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/.part-00001-2e274fe7-eb75-4b73-8c72-423ee747abc0-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123     2213 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     3627 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00000-182665f0-30df-470d-a5cb-8d9d483ed390-c000.snappy.parquet
+-rw-r--r--   0     1001      123     3644 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00001-2e274fe7-eb75-4b73-8c72-423ee747abc0-c000.snappy.parquet
+-rw-r--r--   0     1001      123     1155 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/http_requests/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     2156 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/http_requests/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123     3780 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/http_requests/date=2023-04-13/part-00000-e853fe2e-6f42-450c-8af1-4145b73a96c7-c000.snappy.parquet
+-rw-r--r--   0     1001      123     5976 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/http_requests/date=2023-04-14/part-00000-731ab1b3-85a8-4bc3-92e5-96347fe3fd84-c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/.part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/.part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/.part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/.part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       35 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/_delta_log/.gitignore
+-rw-r--r--   0     1001      123      549 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      396 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/part-00000-512e1537-8aaa-4193-b8b4-bef3de0de409-c000.snappy.parquet
+-rw-r--r--   0     1001      123      396 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/part-00000-b44fcdb0-8b06-4f3a-8606-f8311a96f6dc-c000.snappy.parquet
+-rw-r--r--   0     1001      123      400 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/part-00001-185eca06-e017-4dea-ae49-fc48b973e37e-c000.snappy.parquet
+-rw-r--r--   0     1001      123      400 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/part-00001-4327c977-2734-4477-9507-7ccf67924649-c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00000-2befed33-c358-4768-a43c-3eda0d2a499d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00000-a72b1fb3-f2df-41fe-a8f0-e65b746382dd-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00000-a922ea3b-ffc2-4ca1-9074-a278c24c4449-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00000-c1777d7d-89d9-4790-b38a-6ee7e24456b1-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00000-f17fcbf5-e0dc-40ba-adae-ce66d1fcaef6-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00001-7891c33d-cedc-47c3-88a6-abcfb049d3b4-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00001-bb70d2ba-c196-4df2-9c85-f34969ad3aa9-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00001-c506e79a-0bf8-4e2b-a42b-9731b2e490ae-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00003-508ae4aa-801c-4c2c-a923-f6f89930a5c1-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00003-53f42606-6cda-4f13-8d07-599a21197296-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00004-315835fe-fb44-4562-98f6-5e6cfa3ae45d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00004-80938522-09c0-420c-861f-5a649e3d9674-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00004-95c9bc2c-ac85-4581-b3cc-84502b0c314f-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00005-94a0861b-6455-4bd9-a080-73e02491c643-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00006-46f2ff20-eb5d-4dda-8498-7bfb2940713b-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00006-63ce9deb-bc0f-482d-b9a1-7e717b67f294-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00007-3a0e4727-de0d-41b6-81ef-5223cf40f025-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00007-94f725e2-3963-4b00-9e83-e31021a93cf9-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00011-42f838f9-a911-40af-98f5-2fccfa1b123f-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00045-332fe409-7705-45b1-8d34-a0018cf73b70-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00049-d3095817-de74-49c1-a888-81565a40161d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00058-b462c4cb-0c48-4148-8475-e21d2a2935f8-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00068-90650739-6a8e-492b-9403-53e33b3778ac-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00069-c78b4dd8-f955-4643-816f-cbd30a3f8c1b-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00077-2fcb1c7c-5390-48ee-93f6-0acf11199a0d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00107-3f6c2aa0-fc28-4f4c-be15-135e15b398f4-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00112-07fd790a-11dc-4fde-9acd-623e740be992-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00116-bc66759e-6381-4f34-8cd4-6688aad8585d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00121-d8bc3e53-d2f2-48ce-9909-78da7294ffbd-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00128-b31c3b81-24da-4a90-a8b4-578c9e9a218d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00140-e9b1971d-d708-43fb-b07f-975d2226b800-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00143-03ceb88e-5283-4193-aa43-993cdf937fd3-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00150-ec6643fc-4963-4871-9613-f5ad1940b689-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00154-4630673a-5227-48fb-a03d-e356fcd1564a-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00164-bf40481c-4afd-4c02-befa-90f056c2d77a-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/.part-00190-8ac0ae67-fb1d-461d-a3d3-8dc112766ff5-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123     1522 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     4449 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123     4307 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123      816 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000003.json
+-rw-r--r--   0     1001      123      649 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000004.json
+-rw-r--r--   0     1001      123      262 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00000-2befed33-c358-4768-a43c-3eda0d2a499d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      262 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00000-a72b1fb3-f2df-41fe-a8f0-e65b746382dd-c000.snappy.parquet
+-rw-r--r--   0     1001      123      262 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00000-a922ea3b-ffc2-4ca1-9074-a278c24c4449-c000.snappy.parquet
+-rw-r--r--   0     1001      123      262 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00000-c1777d7d-89d9-4790-b38a-6ee7e24456b1-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00000-f17fcbf5-e0dc-40ba-adae-ce66d1fcaef6-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00001-7891c33d-cedc-47c3-88a6-abcfb049d3b4-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00001-bb70d2ba-c196-4df2-9c85-f34969ad3aa9-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00001-c506e79a-0bf8-4e2b-a42b-9731b2e490ae-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00003-508ae4aa-801c-4c2c-a923-f6f89930a5c1-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00003-53f42606-6cda-4f13-8d07-599a21197296-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00004-315835fe-fb44-4562-98f6-5e6cfa3ae45d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00004-80938522-09c0-420c-861f-5a649e3d9674-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00004-95c9bc2c-ac85-4581-b3cc-84502b0c314f-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00005-94a0861b-6455-4bd9-a080-73e02491c643-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00006-46f2ff20-eb5d-4dda-8498-7bfb2940713b-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00006-63ce9deb-bc0f-482d-b9a1-7e717b67f294-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00007-3a0e4727-de0d-41b6-81ef-5223cf40f025-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00007-94f725e2-3963-4b00-9e83-e31021a93cf9-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00011-42f838f9-a911-40af-98f5-2fccfa1b123f-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00045-332fe409-7705-45b1-8d34-a0018cf73b70-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00049-d3095817-de74-49c1-a888-81565a40161d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00058-b462c4cb-0c48-4148-8475-e21d2a2935f8-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00068-90650739-6a8e-492b-9403-53e33b3778ac-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00069-c78b4dd8-f955-4643-816f-cbd30a3f8c1b-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00077-2fcb1c7c-5390-48ee-93f6-0acf11199a0d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00107-3f6c2aa0-fc28-4f4c-be15-135e15b398f4-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00112-07fd790a-11dc-4fde-9acd-623e740be992-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00116-bc66759e-6381-4f34-8cd4-6688aad8585d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00121-d8bc3e53-d2f2-48ce-9909-78da7294ffbd-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00128-b31c3b81-24da-4a90-a8b4-578c9e9a218d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00140-e9b1971d-d708-43fb-b07f-975d2226b800-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00143-03ceb88e-5283-4193-aa43-993cdf937fd3-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00150-ec6643fc-4963-4871-9613-f5ad1940b689-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00154-4630673a-5227-48fb-a03d-e356fcd1564a-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00164-bf40481c-4afd-4c02-befa-90f056c2d77a-c000.snappy.parquet
+-rw-r--r--   0     1001      123      429 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/part-00190-8ac0ae67-fb1d-461d-a3d3-8dc112766ff5-c000.snappy.parquet
+-rw-r--r--   0     1001      123     1155 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_change_data/cdc-00000-a846ce80-2eec-484d-bef7-0e63557786ca.c000.snappy.parquet
+-rw-r--r--   0     1001      123     1997 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.crc
+-rw-r--r--   0     1001      123     1052 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     2476 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.crc
+-rw-r--r--   0     1001      123      991 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123     2477 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.crc
+-rw-r--r--   0     1001      123     1618 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123     1026 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-7444aec4-710a-4a4c-8abe-3323499043e9.c000.snappy.parquet
+-rw-r--r--   0     1001      123      815 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-996384f7-3fc5-4a5f-9921-6e56269ec2c9-c000.snappy.parquet
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-136c36f5-639d-4e95-bb0f-15cde3fb14eb-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-1abe25d3-0da6-46c5-98c1-7a69872fd797-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-3810fbe0-9892-431d-bcfd-7de5788dfe8d-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-3fa65c69-4e55-4b18-a195-5f1ae583e553-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-72ecc4d6-2e44-4df4-99e6-23f1ac2b7b7c-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-7d239c98-d74b-4b02-b3f6-9f256992c633-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-8e7dc8c1-337b-40b8-a411-46d4295da531-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-9afd9224-729f-4420-a05e-8032113a6568-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-e93060ad-9c8c-4170-a9da-7c6f53f6406b-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-e9c6df9a-e585-4c70-bc1f-de9bd8ae025b-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       12 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/.part-00000-f0e955c5-a1e3-4eec-834e-dcc098fc9005-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       96 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/.00000000000000000010.checkpoint.parquet.crc
+-rw-r--r--   0     1001      123      752 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000002.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000003.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000004.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000005.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000006.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000007.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000008.json
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000009.json
+-rw-r--r--   0     1001      123    11088 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000010.checkpoint.parquet
+-rw-r--r--   0     1001      123      408 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000010.json
+-rw-r--r--   0     1001      123       25 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/_last_checkpoint
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-136c36f5-639d-4e95-bb0f-15cde3fb14eb-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-1abe25d3-0da6-46c5-98c1-7a69872fd797-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-3810fbe0-9892-431d-bcfd-7de5788dfe8d-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-3fa65c69-4e55-4b18-a195-5f1ae583e553-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-72ecc4d6-2e44-4df4-99e6-23f1ac2b7b7c-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-7d239c98-d74b-4b02-b3f6-9f256992c633-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-8e7dc8c1-337b-40b8-a411-46d4295da531-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-9afd9224-729f-4420-a05e-8032113a6568-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-e93060ad-9c8c-4170-a9da-7c6f53f6406b-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-e9c6df9a-e585-4c70-bc1f-de9bd8ae025b-c000.snappy.parquet
+-rw-r--r--   0     1001      123      442 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/part-00000-f0e955c5-a1e3-4eec-834e-dcc098fc9005-c000.snappy.parquet
+-rw-r--r--   0     1001      123       89 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/_delta_log/00000000000000000000.crc
+-rw-r--r--   0     1001      123     2017 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123     1201 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00000-a9dd181d-61aa-491d-b3c9-3eea548de6cb-c000.snappy.parquet
+-rw-r--r--   0     1001      123     1201 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00001-f804d355-db40-4e13-a624-ddd50ce7f5c4-c000.snappy.parquet
+-rw-r--r--   0     1001      123    30082 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/datafusion_test.rs
+-rw-r--r--   0     1001      123     3347 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/fs_common/mod.rs
+-rw-r--r--   0     1001      123     3593 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/integration_checkpoint.rs
+-rw-r--r--   0     1001      123     9501 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/integration_commit.rs
+-rw-r--r--   0     1001      123     5068 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/integration_concurrent_writes.rs
+-rw-r--r--   0     1001      123     2527 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/integration_datafusion.rs
+-rw-r--r--   0     1001      123    14975 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/integration_object_store.rs
+-rw-r--r--   0     1001      123     9370 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/integration_read.rs
+-rw-r--r--   0     1001      123     5313 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/read_delta_partitions_test.rs
+-rw-r--r--   0     1001      123    20058 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/read_delta_test.rs
+-rw-r--r--   0     1001      123     8330 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/repair_s3_rename_test.rs
+-rw-r--r--   0     1001      123     2335 2023-05-06 16:45:03.000000 deltalake-0.9.0/local_dependencies/deltalake/tests/time_travel.rs
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 deltalake-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      123      223 2023-05-06 16:45:02.000000 deltalake-0.9.0/.cargo/config
+-rw-r--r--   0     1001      123      207 2023-05-06 16:45:02.000000 deltalake-0.9.0/.gitignore
+-rw-r--r--   0     1001      123     1328 2023-05-06 16:45:02.000000 deltalake-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123    10257 2023-05-06 16:45:02.000000 deltalake-0.9.0/LICENSE.txt
+-rw-r--r--   0     1001      123     2926 2023-05-06 16:45:02.000000 deltalake-0.9.0/Makefile
+-rw-r--r--   0     1001      123     3151 2023-05-06 16:45:02.000000 deltalake-0.9.0/README.md
+-rw-r--r--   0     1001      123      246 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/__init__.py
+-rw-r--r--   0     1001      123     7134 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/_internal.pyi
+-rw-r--r--   0     1001      123      176 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/data_catalog.py
+-rw-r--r--   0     1001      123     2012 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/fs.py
+-rw-r--r--   0     1001      123     1503 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/schema.py
+-rw-r--r--   0     1001      123    21161 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/table.py
+-rw-r--r--   0     1001      123    19065 2023-05-06 16:45:02.000000 deltalake-0.9.0/deltalake/writer.py
+-rw-r--r--   0     1001      123      638 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/Makefile
+-rw-r--r--   0     1001      123      799 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/make.bat
+-rw-r--r--   0     1001      123     1576 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/_ext/edit_on_github.py
+-rw-r--r--   0     1001      123       70 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/_static/.gitignore
+-rw-r--r--   0     1001      123      832 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/api_reference.rst
+-rw-r--r--   0     1001      123     3328 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/conf.py
+-rw-r--r--   0     1001      123     1289 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/index.rst
+-rw-r--r--   0     1001      123      295 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/installation.rst
+-rw-r--r--   0     1001      123    19320 2023-05-06 16:45:02.000000 deltalake-0.9.0/docs/source/usage.rst
+-rw-r--r--   0     1001      123     2352 2023-05-06 16:45:02.000000 deltalake-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      123    17824 2023-05-06 16:45:02.000000 deltalake-0.9.0/src/filesystem.rs
+-rw-r--r--   0     1001      123    30225 2023-05-06 16:45:03.000000 deltalake-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      123    38293 2023-05-06 16:45:03.000000 deltalake-0.9.0/src/schema.rs
+-rw-r--r--   0     1001      123     2674 2023-05-06 16:45:03.000000 deltalake-0.9.0/src/utils.rs
+-rw-r--r--   0     1001      123       39 2023-05-06 16:45:03.000000 deltalake-0.9.0/stubs/pandas/__init__.pyi
+-rw-r--r--   0     1001      123      460 2023-05-06 16:45:03.000000 deltalake-0.9.0/stubs/pyarrow/__init__.pyi
+-rw-r--r--   0     1001      123      186 2023-05-06 16:45:03.000000 deltalake-0.9.0/stubs/pyarrow/dataset.pyi
+-rw-r--r--   0     1001      123      157 2023-05-06 16:45:03.000000 deltalake-0.9.0/stubs/pyarrow/fs.pyi
+-rw-r--r--   0     1001      123       47 2023-05-06 16:45:03.000000 deltalake-0.9.0/stubs/pyarrow/lib.pyi
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/__init__.py
+-rw-r--r--   0     1001      123     6551 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/conftest.py
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/data_acceptance/__init__.py
+-rw-r--r--   0     1001      123     3094 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/data_acceptance/test_reader.py
+-rw-r--r--   0     1001      123        0 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/pyspark_integration/__init__.py
+-rw-r--r--   0     1001      123     3368 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/pyspark_integration/test_write_to_pyspark.py
+-rw-r--r--   0     1001      123     1944 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/pyspark_integration/test_writer_readable.py
+-rw-r--r--   0     1001      123     1324 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/pyspark_integration/utils.py
+-rw-r--r--   0     1001      123     1974 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_benchmark.py
+-rw-r--r--   0     1001      123      813 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_checkpoint.py
+-rw-r--r--   0     1001      123     5330 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_file_system_handler.py
+-rw-r--r--   0     1001      123     8557 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_fs.py
+-rw-r--r--   0     1001      123      903 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_optimize.py
+-rw-r--r--   0     1001      123     6699 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_schema.py
+-rw-r--r--   0     1001      123    19392 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_table_read.py
+-rw-r--r--   0     1001      123     2304 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_vacuum.py
+-rw-r--r--   0     1001      123      150 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_version.py
+-rw-r--r--   0     1001      123    27316 2023-05-06 16:45:03.000000 deltalake-0.9.0/tests/test_writer.py
+-rw-r--r--   0        0        0   118345 2023-05-06 16:47:17.000000 deltalake-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 deltalake-0.9.0/PKG-INFO
```

### Comparing `deltalake-0.8.1/local_dependencies/glibc_version/src/lib.rs` & `deltalake-0.9.0/local_dependencies/glibc_version/src/lib.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/dynamodb_lock/Cargo.toml` & `deltalake-0.9.0/local_dependencies/dynamodb_lock/Cargo.toml`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/dynamodb_lock/README.md` & `deltalake-0.9.0/local_dependencies/dynamodb_lock/README.md`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/dynamodb_lock/src/lib.rs` & `deltalake-0.9.0/local_dependencies/dynamodb_lock/src/lib.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/Cargo.toml` & `deltalake-0.9.0/local_dependencies/deltalake/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 [package]
 name = "deltalake"
-version = "0.8.0"
+version = "0.10.0"
 rust-version = "1.64"
 authors = ["Qingping Hou <dave2008713@gmail.com>"]
 homepage = "https://github.com/delta-io/delta.rs"
 license = "Apache-2.0"
 keywords = ["deltalake", "delta", "datalake"]
 description = "Native Delta Lake implementation in Rust"
 documentation = "https://docs.rs/deltalake"
 repository = "https://github.com/delta-io/delta.rs"
 readme = "README.md"
 edition = "2021"
 
 [dependencies]
-arrow = { version = "33.0.0", optional = true }
+arrow = { version = "37", optional = true }
+arrow-array = { version = "37", optional = true }
+arrow-cast = { version = "37", optional = true }
+arrow-schema = { version = "37", optional = true }
 async-trait = "0.1"
 bytes = "1"
 chrono = { version = "0.4.22", default-features = false, features = ["clock"] }
 cfg-if = "1"
+datafusion-objectstore-hdfs = { version = "0.1.3", default-features = false, features = [
+    "hdfs3",
+    "try_spawn_blocking",
+], optional = true }
 errno = "0.3"
 futures = "0.3"
 itertools = "0.10"
 lazy_static = "1"
 log = "0"
 libc = ">=0.2.90, <1"
 num-bigint = "0.4"
 num-traits = "0.2.15"
-object_store = "0.5.3"
+object_store = "0.5.6"
 once_cell = "1.16.0"
 parking_lot = "0.12"
-parquet = { version = "33", features = [
+parquet = { version = "37", features = [
     "async",
     "object_store",
 ], optional = true }
 parquet2 = { version = "0.17", optional = true }
 percent-encoding = "2"
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
@@ -48,19 +55,28 @@
 rusoto_credential = { version = "0.47", optional = true }
 rusoto_sts = { version = "0.47", default-features = false, optional = true }
 rusoto_dynamodb = { version = "0.47", default-features = false, optional = true }
 
 # Glue
 rusoto_glue = { version = "0.47", default-features = false, optional = true }
 
+# Unity
+reqwest = { version = "0.11", default-features = false, features = ["rustls-tls", "json"], optional = true }
+reqwest-middleware = { version = "0.2.1", optional = true }
+reqwest-retry = { version = "0.2.2", optional = true }
+
 # Datafusion
-datafusion = { version = "19", optional = true }
-datafusion-expr = { version = "19", optional = true }
-datafusion-common = { version = "19", optional = true }
-datafusion-proto = { version = "19", optional = true }
+datafusion = { version = "23", optional = true }
+datafusion-expr = { version = "23", optional = true }
+datafusion-common = { version = "23", optional = true }
+datafusion-proto = { version = "23", optional = true }
+datafusion-sql = { version = "23", optional = true }
+datafusion-physical-expr = { version = "23", optional = true }
+
+sqlparser = { version = "0.33", optional = true }
 
 # NOTE dependencies only for integration tests
 fs_extra = { version = "1.2.0", optional = true }
 tempdir = { version = "0", optional = true }
 
 [dependencies.dynamodb_lock]
 path = "../dynamodb_lock"
@@ -68,26 +84,37 @@
 default-features = false
 optional = true
 
 [build-dependencies]
 glibc_version = { path = "../glibc_version", version = "0.1" }
 
 [features]
+azure = ["object_store/azure"]
+arrow = ["dep:arrow", "arrow-array", "arrow-cast", "arrow-schema"]
 default = ["arrow", "parquet"]
 datafusion = [
     "dep:datafusion",
     "datafusion-expr",
     "datafusion-common",
     "datafusion-proto",
+    "datafusion-physical-expr",
+    "datafusion-sql",
+    "sqlparser",
     "arrow",
     "parquet",
 ]
 datafusion-ext = ["datafusion"]
-azure = ["object_store/azure"]
 gcs = ["object_store/gcp"]
+glue = ["s3", "rusoto_glue/rustls"]
+glue-native-tls = ["s3-native-tls", "rusoto_glue"]
+hdfs = ["datafusion-objectstore-hdfs"]
+# used only for integration testing
+integration_test = ["fs_extra", "tempdir"]
+json = ["parquet/json"]
+python = ["arrow/pyarrow"]
 s3-native-tls = [
     "rusoto_core/native-tls",
     "rusoto_credential",
     "rusoto_sts/native-tls",
     "rusoto_dynamodb/native-tls",
     "dynamodb_lock/native-tls",
     "object_store/aws",
@@ -98,20 +125,19 @@
     "rusoto_credential",
     "rusoto_sts/rustls",
     "rusoto_dynamodb/rustls",
     "dynamodb_lock/rustls",
     "object_store/aws",
     "object_store/aws_profile",
 ]
-glue-native-tls = ["s3-native-tls", "rusoto_glue"]
-glue = ["s3", "rusoto_glue/rustls"]
-python = ["arrow/pyarrow"]
-
-# used only for integration testing
-integration_test = ["fs_extra", "tempdir"]
+unity-experimental = [
+    "reqwest",
+    "reqwest-middleware",
+    "reqwest-retry",
+]
 
 [[bench]]
 name = "read_checkpoint"
 harness = false
 
 [[example]]
 name = "basic_operations"
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/README.md` & `deltalake-0.9.0/local_dependencies/deltalake/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,23 @@
 
 ```bash
 cargo run --example read_delta_table
 ```
 
 ## Optional cargo package features
 
-- `s3` - enable the S3 storage backend to work with Delta Tables in AWS S3. Uses [rustls](https://github.com/ctz/rustls).
-- `s3-native-tls` - enable the S3 storage backend but rely on OpenSSL.
-- `glue` - enable the Glue data catalog to work with Delta Tables with AWS Glue.
 - `azure` - enable the Azure storage backend to work with Delta Tables in Azure Data Lake Storage Gen2 accounts.
-- `gcs` - enable the Google storage backend to work with Delta Tables in Google Cloud Storage.
 - `datafusion` - enable the `datafusion::datasource::TableProvider` trait implementation for Delta Tables, allowing them to be queried using [DataFusion](https://github.com/apache/arrow-datafusion).
 - `datafusion-ext` - DEPRECATED: alias for `datafusion` feature
+- `gcs` - enable the Google storage backend to work with Delta Tables in Google Cloud Storage.
+- `glue` - enable the Glue data catalog to work with Delta Tables with AWS Glue.
+- `hdfs` - enable the HDFS storage backend to work with Delta Tables in HDFS.
+- `json` - enable the JSON feature of the `parquet` crate for better JSON interoperability.
 - `parquet2` - use parquet2 for checkpoint deserialization. Since `arrow` and `parquet` features are enabled by default for backwards compatibility, this feature needs to be used with `--no-default-features`.
+- `s3` - enable the S3 storage backend to work with Delta Tables in AWS S3. Uses [rustls](https://github.com/ctz/rustls).
+- `s3-native-tls` - enable the S3 storage backend but rely on OpenSSL.
 
 ## Development
 
 To run s3 integration tests from local machine, we use docker-compose to stand
 up AWS local stack. To spin up the test environment run `docker-compose up` in
 the root of the `delta-rs` repo.
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/benches/read_checkpoint.rs` & `deltalake-0.9.0/local_dependencies/deltalake/benches/read_checkpoint.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/build.rs` & `deltalake-0.9.0/local_dependencies/deltalake/build.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/examples/basic_operations.rs` & `deltalake-0.9.0/local_dependencies/deltalake/examples/basic_operations.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/examples/recordbatch-writer.rs` & `deltalake-0.9.0/local_dependencies/deltalake/examples/recordbatch-writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
  *
  *
  * This example was originally posted by @rtyler in:
  *      <https://github.com/buoyant-data/demo-recordbatch-writer>
  */
 
 use chrono::prelude::*;
-use deltalake::action::*;
 use deltalake::arrow::array::*;
 use deltalake::arrow::record_batch::RecordBatch;
 use deltalake::writer::{DeltaWriter, RecordBatchWriter};
 use deltalake::*;
 use log::*;
 
 use object_store::path::Path;
@@ -71,16 +70,16 @@
     timestamp: DateTime<Utc>,
     temp: Fahrenheit,
     lat: f64,
     long: f64,
 }
 
 impl WeatherRecord {
-    fn schema() -> Schema {
-        Schema::new(vec![
+    fn columns() -> Vec<SchemaField> {
+        vec![
             SchemaField::new(
                 "timestamp".to_string(),
                 SchemaDataType::primitive("timestamp".to_string()),
                 true,
                 HashMap::new(),
             ),
             SchemaField::new(
@@ -97,15 +96,15 @@
             ),
             SchemaField::new(
                 "long".to_string(),
                 SchemaDataType::primitive("double".to_string()),
                 true,
                 HashMap::new(),
             ),
-        ])
+        ]
     }
 }
 
 impl Default for WeatherRecord {
     fn default() -> Self {
         Self {
             timestamp: Utc::now(),
@@ -185,35 +184,19 @@
 }
 
 /*
  * Pilfered from writer/test_utils.rs in delta-rs. This code will basically create a new Delta
  * Table in an existing directory that doesn't currently contain a Delta table
  */
 async fn create_initialized_table(table_path: &Path) -> DeltaTable {
-    let mut table = DeltaTableBuilder::from_uri(table_path).build().unwrap();
-    let table_schema = WeatherRecord::schema();
-    let mut commit_info = serde_json::Map::<String, serde_json::Value>::new();
-    commit_info.insert(
-        "operation".to_string(),
-        serde_json::Value::String("CREATE TABLE".to_string()),
-    );
-    commit_info.insert(
-        "userName".to_string(),
-        serde_json::Value::String("test user".to_string()),
-    );
-
-    let protocol = Protocol {
-        min_reader_version: 1,
-        min_writer_version: 1,
-    };
-
-    let metadata = DeltaTableMetaData::new(None, None, None, table_schema, vec![], HashMap::new());
-
-    table
-        .create(metadata, protocol, Some(commit_info), None)
+    let table = DeltaOps::try_from_uri(table_path)
+        .await
+        .unwrap()
+        .create()
+        .with_columns(WeatherRecord::columns())
         .await
         .unwrap();
 
     table
 }
 
 #[cfg(test)]
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -540,14 +540,21 @@
         /// The save mode used during the write.
         mode: SaveMode,
         /// The columns the write is partitioned by.
         partition_by: Option<Vec<String>>,
         /// The predicate used during the write.
         predicate: Option<String>,
     },
+
+    /// Delete data matching predicate from delta table
+    Delete {
+        /// The condition the to be deleted data must match
+        predicate: Option<String>,
+    },
+
     /// Represents a Delta `StreamingUpdate` operation.
     #[serde(rename_all = "camelCase")]
     StreamingUpdate {
         /// The output mode the streaming writer is using.
         output_mode: OutputMode,
         /// The query id of the streaming writer.
         query_id: String,
@@ -576,14 +583,15 @@
         // operation names taken from https://learn.microsoft.com/en-us/azure/databricks/delta/history#--operation-metrics-keys
         match &self {
             DeltaOperation::Create { mode, .. } if matches!(mode, SaveMode::Overwrite) => {
                 "CREATE OR REPLACE TABLE"
             }
             DeltaOperation::Create { .. } => "CREATE TABLE",
             DeltaOperation::Write { .. } => "WRITE",
+            DeltaOperation::Delete { .. } => "DELETE",
             DeltaOperation::StreamingUpdate { .. } => "STREAMING UPDATE",
             DeltaOperation::Optimize { .. } => "OPTIMIZE",
             DeltaOperation::FileSystemCheck { .. } => "FSCK",
         }
     }
 
     /// Parameters configured for operation.
@@ -618,15 +626,16 @@
     /// Denotes if the operation changes the data contained in the table
     pub fn changes_data(&self) -> bool {
         match self {
             Self::Optimize { .. } => false,
             Self::Create { .. }
             | Self::FileSystemCheck {}
             | Self::StreamingUpdate { .. }
-            | Self::Write { .. } => true,
+            | Self::Write { .. }
+            | Self::Delete { .. } => true,
         }
     }
 
     /// Retrieve basic commit information to be added to Delta commits
     pub fn get_commit_info(&self) -> CommitInfo {
         // TODO infer additional info from operation parameters ...
         CommitInfo {
@@ -637,17 +646,28 @@
     }
 
     /// Get predicate expression applied when the operation reads data from the table.
     pub fn read_predicate(&self) -> Option<String> {
         match self {
             // TODO add more operations
             Self::Write { predicate, .. } => predicate.clone(),
+            Self::Delete { predicate, .. } => predicate.clone(),
             _ => None,
         }
     }
+
+    /// Denotes if the operation reads the entire table
+    pub fn read_whole_table(&self) -> bool {
+        match self {
+            // TODO just adding one operation example, as currently none of the
+            // implemented operations scan the entire table.
+            Self::Write { predicate, .. } if predicate.is_none() => false,
+            _ => false,
+        }
+    }
 }
 
 /// The SaveMode used when performing a DeltaOperation
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub enum SaveMode {
     /// Files will be appended to the target location.
     Append,
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/boolean.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/boolean.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/dictionary/binary.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/dictionary/binary.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/dictionary/primitive.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/dictionary/primitive.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/map.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/map.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/mod.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/primitive.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/primitive.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/string.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/string.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet2_read/validity.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet2_read/validity.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/action/parquet_read/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/action/parquet_read/mod.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/builder.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/builder.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 //! Create or load DeltaTables
 
 use std::collections::HashMap;
+use std::path::PathBuf;
 use std::sync::Arc;
 
 use crate::delta::{DeltaResult, DeltaTable, DeltaTableError};
 use crate::schema::DeltaDataTypeVersion;
 use crate::storage::config::StorageOptions;
 use crate::storage::{DeltaObjectStore, ObjectStoreRef};
 
@@ -341,55 +342,190 @@
 
 #[allow(dead_code)]
 pub(crate) fn str_option(map: &HashMap<String, String>, key: &str) -> Option<String> {
     map.get(key)
         .map_or_else(|| std::env::var(key).ok(), |v| Some(v.to_owned()))
 }
 
+lazy_static::lazy_static! {
+    static ref KNOWN_SCHEMES: Vec<&'static str> =
+        Vec::from([
+            "file", "memory", "az", "abfs", "abfss", "azure", "wasb", "adl", "s3", "s3a", "gs", "hdfs",
+            "https", "http",
+        ]);
+}
+
+/// Attempt to create a Url from given table location.
+///
+/// The location could be:
+///  * A valid URL, which will be parsed and returned
+///  * A path to a directory, which will be created and then converted to a URL.
+///
+/// If it is a local path, it will be created if it doesn't exist.
+///
+/// Extra slashes will be removed from the end path as well.
+///
+/// Will return an error if the location is not valid. For example,
 pub(crate) fn ensure_table_uri(table_uri: impl AsRef<str>) -> DeltaResult<Url> {
     let table_uri = table_uri.as_ref();
-    if let Ok(path) = std::fs::canonicalize(table_uri) {
-        return Url::from_directory_path(path)
-            .map_err(|_| DeltaTableError::InvalidTableLocation(table_uri.to_string()));
-    }
-    if let Ok(url) = Url::parse(table_uri) {
-        return Ok(match url.scheme() {
-            "file" => url,
-            _ => {
-                let mut new_url = url.clone();
-                new_url.set_path(url.path().trim_end_matches('/'));
-                new_url
+
+    enum UriType {
+        LocalPath(PathBuf),
+        Url(Url),
+    }
+    let uri_type: UriType = if let Ok(url) = Url::parse(table_uri) {
+        if url.scheme() == "file" {
+            UriType::LocalPath(url.to_file_path().map_err(|err| {
+                let msg = format!("Invalid table location: {}\nError: {:?}", table_uri, err);
+                DeltaTableError::InvalidTableLocation(msg)
+            })?)
+        // NOTE this check is required to support absolute windows paths which may properly parse as url
+        } else if KNOWN_SCHEMES.contains(&url.scheme()) {
+            UriType::Url(url)
+        } else {
+            UriType::LocalPath(PathBuf::from(table_uri))
+        }
+    } else {
+        UriType::LocalPath(PathBuf::from(table_uri))
+    };
+
+    // If it is a local path, we need to create it if it does not exist.
+    let mut url = match uri_type {
+        UriType::LocalPath(path) => {
+            if !path.exists() {
+                std::fs::create_dir_all(&path).map_err(|err| {
+                    let msg = format!(
+                        "Could not create local directory: {}\nError: {:?}",
+                        table_uri, err
+                    );
+                    DeltaTableError::InvalidTableLocation(msg)
+                })?;
             }
-        });
-    }
-    // The table uri still might be a relative paths that does not exist.
-    std::fs::create_dir_all(table_uri)
-        .map_err(|_| DeltaTableError::InvalidTableLocation(table_uri.to_string()))?;
-    let path = std::fs::canonicalize(table_uri)
-        .map_err(|_| DeltaTableError::InvalidTableLocation(table_uri.to_string()))?;
-    Url::from_directory_path(path)
-        .map_err(|_| DeltaTableError::InvalidTableLocation(table_uri.to_string()))
+            let path = std::fs::canonicalize(path).map_err(|err| {
+                let msg = format!("Invalid table location: {}\nError: {:?}", table_uri, err);
+                DeltaTableError::InvalidTableLocation(msg)
+            })?;
+            Url::from_directory_path(path).map_err(|_| {
+                let msg = format!(
+                    "Could not construct a URL from canonicalized path: {}.\n\
+                    Something must be very wrong with the table path.",
+                    table_uri
+                );
+                DeltaTableError::InvalidTableLocation(msg)
+            })?
+        }
+        UriType::Url(url) => url,
+    };
+
+    let trimmed_path = url.path().trim_end_matches('/').to_owned();
+    url.set_path(&trimmed_path);
+    Ok(url)
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use std::path::Path;
 
     #[test]
     fn test_ensure_table_uri() {
         // parse an exisiting relative directory
         let uri = ensure_table_uri(".");
         assert!(uri.is_ok());
         let _uri = ensure_table_uri("./nonexistent");
         assert!(uri.is_ok());
         let uri = ensure_table_uri("s3://container/path");
         assert!(uri.is_ok());
-        let uri = ensure_table_uri("file:///").unwrap();
-        assert_eq!("file:///", uri.as_str());
-        let uri = ensure_table_uri("memory://").unwrap();
-        assert_eq!("memory://", uri.as_str());
-        let uri = ensure_table_uri("s3://tests/data/delta-0.8.0/").unwrap();
-        assert_eq!("s3://tests/data/delta-0.8.0", uri.as_str());
-        let _uri = ensure_table_uri("s3://tests/data/delta-0.8.0//").unwrap();
-        assert_eq!("s3://tests/data/delta-0.8.0", uri.as_str())
+
+        // These cases should all roundtrip to themselves
+        cfg_if::cfg_if! {
+            if #[cfg(windows)] {
+                let roundtrip_cases = &[
+                    "s3://tests/data/delta-0.8.0",
+                    "memory://",
+                    "s3://bucket/my%20table", // Doesn't double-encode
+                ];
+            } else {
+                let roundtrip_cases = &[
+                    "s3://tests/data/delta-0.8.0",
+                    "memory://",
+                    "file:///",
+                    "s3://bucket/my%20table", // Doesn't double-encode
+                ];
+            }
+        }
+
+        for case in roundtrip_cases {
+            let uri = ensure_table_uri(case).unwrap();
+            assert_eq!(case, &uri.as_str());
+        }
+
+        // Other cases
+        let map_cases = &[
+            // extra slashes are removed
+            (
+                "s3://tests/data/delta-0.8.0//",
+                "s3://tests/data/delta-0.8.0",
+            ),
+            ("s3://bucket/my table", "s3://bucket/my%20table"),
+        ];
+
+        for (case, expected) in map_cases {
+            let uri = ensure_table_uri(case).unwrap();
+            assert_eq!(expected, &uri.as_str());
+        }
+    }
+
+    #[test]
+    #[cfg(windows)]
+    fn test_windows_uri() {
+        let map_cases = &[
+            // extra slashes are removed
+            ("c:/", "file:///C:"),
+        ];
+
+        for (case, expected) in map_cases {
+            let uri = ensure_table_uri(case).unwrap();
+            assert_eq!(expected, &uri.as_str());
+        }
+    }
+
+    #[test]
+    fn test_ensure_table_uri_path() {
+        let tmp_dir = tempdir::TempDir::new("test").unwrap();
+        let tmp_path = std::fs::canonicalize(tmp_dir.path()).unwrap();
+        let paths = &[
+            tmp_path.join("data/delta-0.8.0"),
+            tmp_path.join("space in path"),
+            tmp_path.join("special&chars/你好/😊"),
+        ];
+
+        for path in paths {
+            let expected = Url::from_directory_path(path).unwrap();
+            let uri = ensure_table_uri(path.as_os_str().to_str().unwrap()).unwrap();
+            assert_eq!(expected.as_str().trim_end_matches('/'), uri.as_str());
+            assert!(path.exists());
+        }
+
+        // Creates non-existent relative directories
+        let relative_path = Path::new("_tmp/test %3F");
+        assert!(!relative_path.exists());
+        ensure_table_uri(relative_path.as_os_str().to_str().unwrap()).unwrap();
+        assert!(relative_path.exists());
+        std::fs::remove_dir_all(relative_path).unwrap();
+    }
+
+    #[test]
+    fn test_ensure_table_uri_url() {
+        // Urls should round trips as-is
+        let expected = Url::parse("s3://tests/data/delta-0.8.0").unwrap();
+        let url = ensure_table_uri(&expected).unwrap();
+        assert_eq!(expected, url);
+
+        let tmp_dir = tempdir::TempDir::new("test").unwrap();
+        let tmp_path = std::fs::canonicalize(tmp_dir.path()).unwrap();
+        let path = tmp_path.join("data/delta-0.8.0");
+        let expected = Url::from_directory_path(path).unwrap();
+        let url = ensure_table_uri(&expected).unwrap();
+        assert_eq!(expected.as_str().trim_end_matches('/'), url.as_str());
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/checkpoints.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/checkpoints.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 //! Implementation for writing delta checkpoints.
 
 use arrow::datatypes::Schema as ArrowSchema;
+// NOTE: Temporarily allowing these deprecated imports pending the completion of:
+// <https://github.com/apache/arrow-rs/pull/3979>
 use arrow::error::ArrowError;
+#[allow(deprecated)]
 use arrow::json::reader::{Decoder, DecoderOptions};
 use chrono::{DateTime, Datelike, Duration, Utc};
 use futures::StreamExt;
 use lazy_static::lazy_static;
 use log::*;
 use object_store::{path::Path, Error as ObjectStoreError, ObjectMeta, ObjectStore};
 use parquet::arrow::ArrowWriter;
@@ -295,14 +298,17 @@
 
             maybe_delete_files.push(current_file.clone());
             last_file = current_file;
         }
     }
 }
 
+// NOTE: Temporarily allowing these deprecated imports pending the completion of:
+// <https://github.com/apache/arrow-rs/pull/3979>
+#[allow(deprecated)]
 fn parquet_bytes_from_state(state: &DeltaTableState) -> Result<bytes::Bytes, CheckpointError> {
     let current_metadata = state
         .current_metadata()
         .ok_or(CheckpointError::MissingMetaData)?;
 
     let partition_col_data_types = current_metadata.get_partition_col_data_types();
 
@@ -378,14 +384,15 @@
         use_extended_remove_schema,
     );
 
     debug!("Writing to checkpoint parquet buffer...");
     // Write the Checkpoint parquet file.
     let mut bytes = vec![];
     let mut writer = ArrowWriter::try_new(&mut bytes, arrow_schema.clone(), None)?;
+
     let options = DecoderOptions::new().with_batch_size(CHECKPOINT_RECORD_BATCH_SIZE);
     let decoder = Decoder::new(arrow_schema, options);
     while let Some(batch) = decoder.next_batch(&mut jsons)? {
         writer.write(&batch)?;
     }
     let _ = writer.close()?;
     debug!("Finished writing checkpoint parquet buffer.");
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/data_catalog/glue/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/data_catalog/glue/mod.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/data_catalog/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/data_catalog/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 //! Catalog abstraction for Delta Table
 
 use std::fmt::Debug;
 
 #[cfg(feature = "glue")]
 pub mod glue;
 
+#[cfg(feature = "unity-experimental")]
+pub mod unity;
+
 /// Error enum that represents a CatalogError.
 #[derive(thiserror::Error, Debug)]
 pub enum DataCatalogError {
     /// Missing metadata in the catalog
     #[cfg(feature = "glue")]
     #[error("Missing Metadata {metadata} in the Data Catalog ")]
     MissingMetadata {
@@ -39,14 +42,36 @@
     #[error("Failed to retrieve AWS credentials: {source}")]
     AWSCredentials {
         /// The underlying Rusoto CredentialsError
         #[from]
         source: rusoto_credential::CredentialsError,
     },
 
+    /// Error caused by missing environment variable for Unity Catalog.
+    #[cfg(feature = "unity-experimental")]
+    #[error("Missing Unity Catalog environment variable: {var_name}")]
+    MissingEnvVar {
+        /// Variable name
+        var_name: String,
+    },
+
+    /// Error caused by invalid access token value
+    #[cfg(feature = "unity-experimental")]
+    #[error("Invalid Databricks personal access token")]
+    InvalidAccessToken,
+
+    /// Databricks API client error
+    #[cfg(feature = "unity-experimental")]
+    #[error("API client error: {source}")]
+    APIClientError {
+        /// The underlying unity::GetTableError
+        #[from]
+        source: unity::GetTableError,
+    },
+
     /// Error representing an invalid Data Catalog.
     #[error("This data catalog doesn't exist: {data_catalog}")]
     InvalidDataCatalog {
         /// The catalog input
         data_catalog: String,
     },
 }
@@ -66,14 +91,18 @@
 /// Get the Data Catalog
 pub fn get_data_catalog(data_catalog: &str) -> Result<Box<dyn DataCatalog>, DataCatalogError> {
     match data_catalog {
         #[cfg(feature = "gcp")]
         "gcp" => unimplemented!("GCP Data Catalog is not implemented"),
         #[cfg(feature = "azure")]
         "azure" => unimplemented!("Azure Data Catalog is not implemented"),
+        #[cfg(feature = "hdfs")]
+        "hdfs" => unimplemented!("HDFS Data Catalog is not implemented"),
         #[cfg(feature = "glue")]
         "glue" => Ok(Box::new(glue::GlueDataCatalog::new()?)),
+        #[cfg(feature = "unity-experimental")]
+        "unity" => Ok(Box::new(unity::UnityCatalog::new()?)),
         _ => Err(DataCatalogError::InvalidDataCatalog {
             data_catalog: data_catalog.to_string(),
         }),
     }
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/delta.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/delta.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 use super::action;
 use super::action::{Action, DeltaOperation};
 use super::partitions::PartitionFilter;
 use super::schema::*;
 use super::table_state::DeltaTableState;
 use crate::action::{Add, Stats};
 use crate::delta_config::DeltaConfigError;
+use crate::operations::transaction::TransactionError;
 use crate::operations::vacuum::VacuumBuilder;
 use crate::storage::{commit_uri_from_version, ObjectStoreRef};
 
 use chrono::{DateTime, Duration, Utc};
 use futures::StreamExt;
 use lazy_static::lazy_static;
 use log::debug;
@@ -199,31 +200,43 @@
     },
     /// Error returned when a invalid partition filter was found.
     #[error("Invalid partition filter found: {}.", .partition_filter)]
     InvalidPartitionFilter {
         /// The invalid partition filter used.
         partition_filter: String,
     },
+    /// Error returned when a partition filter uses a nonpartitioned column.
+    #[error("Tried to filter partitions on non-partitioned columns: {:#?}", .nonpartitioned_columns)]
+    ColumnsNotPartitioned {
+        /// The columns used in the partition filter that is not partitioned
+        nonpartitioned_columns: Vec<String>,
+    },
     /// Error returned when a line from log record is invalid.
     #[error("Failed to read line from log record")]
     Io {
         /// Source error details returned while reading the log record.
         #[from]
         source: std::io::Error,
     },
+    /// Error raised while commititng transaction
+    #[error("Transaction failed: {source}")]
+    Transaction {
+        /// The source error
+        source: TransactionError,
+    },
     /// Error returned when transaction is failed to be committed because given version already exists.
     #[error("Delta transaction failed, version {0} already exists.")]
     VersionAlreadyExists(DeltaDataTypeVersion),
     /// Error returned when user attempts to commit actions that don't belong to the next version.
     #[error("Delta transaction failed, version {0} does not follow {1}")]
     VersionMismatch(DeltaDataTypeVersion, DeltaDataTypeVersion),
     /// A Feature is missing to perform operation
     #[error("Delta-rs must be build with feature '{feature}' to support loading from: {url}.")]
     MissingFeature {
-        /// Name of the missiing feature
+        /// Name of the missing feature
         feature: &'static str,
         /// Storage location url
         url: String,
     },
     /// A Feature is missing to perform operation
     #[error("Cannot infer storage location from: {0}")]
     InvalidTableLocation(String),
@@ -246,14 +259,22 @@
     #[error("Generic error: {source}")]
     GenericError {
         /// Source error
         source: Box<dyn std::error::Error + Send + Sync + 'static>,
     },
 }
 
+impl From<object_store::path::Error> for DeltaTableError {
+    fn from(err: object_store::path::Error) -> Self {
+        Self::GenericError {
+            source: Box::new(err),
+        }
+    }
+}
+
 /// Delta table metadata
 #[derive(Serialize, Deserialize, Clone, Debug, PartialEq)]
 pub struct DeltaTableMetaData {
     /// Unique identifier for this table
     pub id: Guid,
     /// User-provided identifier for this table
     pub name: Option<String>,
@@ -1087,14 +1108,18 @@
             .state
             .current_metadata()
             .ok_or(DeltaTableError::NoMetadata)?
             .get_configuration())
     }
 
     /// Vacuum the delta table. See [`VacuumBuilder`] for more information.
+    #[deprecated(
+        since = "0.10.0",
+        note = "use DelaOps from operations module to create a Vacuum operation."
+    )]
     pub async fn vacuum(
         &mut self,
         retention_hours: Option<u64>,
         dry_run: bool,
         enforce_retention_duration: bool,
     ) -> Result<Vec<String>, DeltaTableError> {
         let mut plan = VacuumBuilder::new(self.object_store(), self.state.clone())
@@ -1108,26 +1133,36 @@
         self.state = table.state;
         Ok(metrics.files_deleted)
     }
 
     /// Creates a new DeltaTransaction for the DeltaTable.
     /// The transaction holds a mutable reference to the DeltaTable, preventing other references
     /// until the transaction is dropped.
+    #[deprecated(
+        since = "0.10.0",
+        note = "use 'commit' function from operations module to commit to Delta table."
+    )]
+    #[allow(deprecated)]
     pub fn create_transaction(
         &mut self,
         options: Option<DeltaTransactionOptions>,
     ) -> DeltaTransaction {
         DeltaTransaction::new(self, options)
     }
 
     /// Tries to commit a prepared commit file. Returns `DeltaTableError::VersionAlreadyExists`
     /// if the given `version` already exists. The caller should handle the retry logic itself.
     /// This is low-level transaction API. If user does not want to maintain the commit loop then
     /// the `DeltaTransaction.commit` is desired to be used as it handles `try_commit_transaction`
     /// with retry logic.
+    #[deprecated(
+        since = "0.10.0",
+        note = "use 'commit' function from operations module to commite to Delta table."
+    )]
+    #[allow(deprecated)]
     pub async fn try_commit_transaction(
         &mut self,
         commit: &PreparedCommit,
         version: DeltaDataTypeVersion,
     ) -> Result<DeltaDataTypeVersion, DeltaTableError> {
         // move temporary commit file to delta log directory
         // rely on storage to fail if the file already exists -
@@ -1143,14 +1178,19 @@
 
         self.update().await?;
 
         Ok(version)
     }
 
     /// Create a DeltaTable with version 0 given the provided MetaData, Protocol, and CommitInfo
+    #[deprecated(
+        since = "0.10.0",
+        note = "use DelaOps from operations module to create a Create operation."
+    )]
+    #[allow(deprecated)]
     pub async fn create(
         &mut self,
         metadata: DeltaTableMetaData,
         protocol: action::Protocol,
         commit_info: Option<Map<String, Value>>,
         add_actions: Option<Vec<action::Add>>,
     ) -> Result<(), DeltaTableError> {
@@ -1297,20 +1337,25 @@
 /// Clients that may need to do conflict resolution if the Delta version changes should use
 /// the `prepare_commit` and `try_commit_transaction` methods and manage the Delta version
 /// themselves so that they can resolve data conflicts that may occur between Delta versions.
 ///
 /// Please not that in case of non-retryable error the temporary commit file such as
 /// `_delta_log/_commit_<uuid>.json` will orphaned in storage.
 #[derive(Debug)]
+#[deprecated(
+    since = "0.10.0",
+    note = "use 'commit' function from operations module to commit to Delta table."
+)]
 pub struct DeltaTransaction<'a> {
     delta_table: &'a mut DeltaTable,
     actions: Vec<Action>,
     options: DeltaTransactionOptions,
 }
 
+#[allow(deprecated)]
 impl<'a> DeltaTransaction<'a> {
     /// Creates a new delta transaction.
     /// Holds a mutable reference to the delta table to prevent outside mutation while a transaction commit is in progress.
     /// Transaction behavior may be customized by passing an instance of `DeltaTransactionOptions`.
     pub fn new(delta_table: &'a mut DeltaTable, options: Option<DeltaTransactionOptions>) -> Self {
         DeltaTransaction {
             delta_table,
@@ -1352,15 +1397,14 @@
         //     _ => false,
         // });
         // let isolation_level = if no_data_changed {
         //     IsolationLevel::SnapshotIsolation
         // } else {
         //     IsolationLevel::Serializable
         // };
-
         let prepared_commit = self.prepare_commit(operation, app_metadata).await?;
 
         // try to commit in a loop in case other writers write the next version first
         let version = self.try_commit_loop(&prepared_commit).await?;
 
         Ok(version)
     }
@@ -1405,14 +1449,15 @@
         let path = Path::from_iter(["_delta_log", &file_name]);
 
         self.delta_table.storage.put(&path, log_entry).await?;
 
         Ok(PreparedCommit { uri: path })
     }
 
+    #[allow(deprecated)]
     async fn try_commit_loop(
         &mut self,
         commit: &PreparedCommit,
     ) -> Result<DeltaDataTypeVersion, DeltaTableError> {
         let mut attempt_number: u32 = 0;
         loop {
             self.delta_table.update().await?;
@@ -1448,14 +1493,18 @@
         }
     }
 }
 
 /// Holds the uri to prepared commit temporary file created with `DeltaTransaction.prepare_commit`.
 /// Once created, the actual commit could be executed with `DeltaTransaction.try_commit`.
 #[derive(Debug)]
+#[deprecated(
+    since = "0.10.0",
+    note = "use 'commit' function from operations module to commit to Delta table."
+)]
 pub struct PreparedCommit {
     uri: Path,
 }
 
 fn log_entry_from_actions(actions: &[Action]) -> Result<String, serde_json::Error> {
     let mut jsons = Vec::<String>::new();
 
@@ -1599,14 +1648,15 @@
             serde_json::Value::String("CREATE TABLE".to_string()),
         );
         commit_info.insert(
             "userName".to_string(),
             serde_json::Value::String("test user".to_string()),
         );
         // Action
+        #[allow(deprecated)]
         dt.create(delta_md.clone(), protocol.clone(), Some(commit_info), None)
             .await
             .unwrap();
         (delta_md, protocol, dt, tmp_dir)
     }
 
     #[tokio::test]
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/delta_arrow.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/delta_arrow.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 //! Conversion between Delta Table schema and Arrow schema
 
 use crate::schema;
 use arrow::datatypes::{
-    DataType as ArrowDataType, Field as ArrowField, Schema as ArrowSchema,
-    SchemaRef as ArrowSchemaRef, TimeUnit,
+    DataType as ArrowDataType, Field as ArrowField, FieldRef as ArrowFieldRef,
+    Schema as ArrowSchema, SchemaRef as ArrowSchemaRef, TimeUnit,
 };
 use arrow::error::ArrowError;
 use lazy_static::lazy_static;
 use regex::Regex;
 use std::convert::TryFrom;
+use std::sync::Arc;
 
 impl TryFrom<&schema::Schema> for ArrowSchema {
     type Error = ArrowError;
 
     fn try_from(s: &schema::Schema) -> Result<Self, ArrowError> {
         let fields = s
             .get_fields()
@@ -60,22 +61,25 @@
 
 impl TryFrom<&schema::SchemaTypeMap> for ArrowField {
     type Error = ArrowError;
 
     fn try_from(a: &schema::SchemaTypeMap) -> Result<Self, ArrowError> {
         Ok(ArrowField::new(
             "entries",
-            ArrowDataType::Struct(vec![
-                ArrowField::new("key", ArrowDataType::try_from(a.get_key_type())?, false),
-                ArrowField::new(
-                    "value",
-                    ArrowDataType::try_from(a.get_value_type())?,
-                    a.get_value_contains_null(),
-                ),
-            ]),
+            ArrowDataType::Struct(
+                vec![
+                    ArrowField::new("key", ArrowDataType::try_from(a.get_key_type())?, false),
+                    ArrowField::new(
+                        "value",
+                        ArrowDataType::try_from(a.get_value_type())?,
+                        a.get_value_contains_null(),
+                    ),
+                ]
+                .into(),
+            ),
             false, // always non-null
         ))
     }
 }
 
 impl TryFrom<&schema::SchemaDataType> for ArrowDataType {
     type Error = ArrowError;
@@ -127,57 +131,61 @@
                     ))),
                 }
             }
             schema::SchemaDataType::r#struct(s) => Ok(ArrowDataType::Struct(
                 s.get_fields()
                     .iter()
                     .map(<ArrowField as TryFrom<&schema::SchemaField>>::try_from)
-                    .collect::<Result<Vec<ArrowField>, ArrowError>>()?,
+                    .collect::<Result<Vec<ArrowField>, ArrowError>>()?
+                    .into(),
             )),
             schema::SchemaDataType::array(a) => {
-                Ok(ArrowDataType::List(Box::new(<ArrowField as TryFrom<
+                Ok(ArrowDataType::List(Arc::new(<ArrowField as TryFrom<
                     &schema::SchemaTypeArray,
                 >>::try_from(
                     a
                 )?)))
             }
             schema::SchemaDataType::map(m) => Ok(ArrowDataType::Map(
-                Box::new(ArrowField::new(
-                    "key_value",
-                    ArrowDataType::Struct(vec![
-                        ArrowField::new(
-                            "key",
-                            <ArrowDataType as TryFrom<&schema::SchemaDataType>>::try_from(
-                                m.get_key_type(),
-                            )?,
-                            false,
-                        ),
-                        ArrowField::new(
-                            "value",
-                            <ArrowDataType as TryFrom<&schema::SchemaDataType>>::try_from(
-                                m.get_value_type(),
-                            )?,
-                            m.get_value_contains_null(),
-                        ),
-                    ]),
-                    false,
+                Arc::new(ArrowField::new(
+                    "entries",
+                    ArrowDataType::Struct(
+                        vec![
+                            ArrowField::new(
+                                "keys",
+                                <ArrowDataType as TryFrom<&schema::SchemaDataType>>::try_from(
+                                    m.get_key_type(),
+                                )?,
+                                false,
+                            ),
+                            ArrowField::new(
+                                "values",
+                                <ArrowDataType as TryFrom<&schema::SchemaDataType>>::try_from(
+                                    m.get_value_type(),
+                                )?,
+                                m.get_value_contains_null(),
+                            ),
+                        ]
+                        .into(),
+                    ),
+                    true,
                 )),
                 false,
             )),
         }
     }
 }
 
 impl TryFrom<&ArrowSchema> for schema::Schema {
     type Error = ArrowError;
     fn try_from(arrow_schema: &ArrowSchema) -> Result<Self, ArrowError> {
         let new_fields: Result<Vec<schema::SchemaField>, _> = arrow_schema
             .fields()
             .iter()
-            .map(|field| field.try_into())
+            .map(|field| field.as_ref().try_into())
             .collect();
         Ok(schema::Schema::new(new_fields?))
     }
 }
 
 impl TryFrom<ArrowSchemaRef> for schema::Schema {
     type Error = ArrowError;
@@ -204,50 +212,70 @@
 }
 
 impl TryFrom<&ArrowDataType> for schema::SchemaDataType {
     type Error = ArrowError;
     fn try_from(arrow_datatype: &ArrowDataType) -> Result<Self, ArrowError> {
         match arrow_datatype {
             ArrowDataType::Utf8 => Ok(schema::SchemaDataType::primitive("string".to_string())),
+            ArrowDataType::LargeUtf8 => Ok(schema::SchemaDataType::primitive("string".to_string())),
             ArrowDataType::Int64 => Ok(schema::SchemaDataType::primitive("long".to_string())), // undocumented type
             ArrowDataType::Int32 => Ok(schema::SchemaDataType::primitive("integer".to_string())),
             ArrowDataType::Int16 => Ok(schema::SchemaDataType::primitive("short".to_string())),
             ArrowDataType::Int8 => Ok(schema::SchemaDataType::primitive("byte".to_string())),
+            ArrowDataType::UInt64 => Ok(schema::SchemaDataType::primitive("long".to_string())), // undocumented type
+            ArrowDataType::UInt32 => Ok(schema::SchemaDataType::primitive("integer".to_string())),
+            ArrowDataType::UInt16 => Ok(schema::SchemaDataType::primitive("short".to_string())),
+            ArrowDataType::UInt8 => Ok(schema::SchemaDataType::primitive("byte".to_string())),
             ArrowDataType::Float32 => Ok(schema::SchemaDataType::primitive("float".to_string())),
             ArrowDataType::Float64 => Ok(schema::SchemaDataType::primitive("double".to_string())),
             ArrowDataType::Boolean => Ok(schema::SchemaDataType::primitive("boolean".to_string())),
             ArrowDataType::Binary => Ok(schema::SchemaDataType::primitive("binary".to_string())),
+            ArrowDataType::FixedSizeBinary(_) => {
+                Ok(schema::SchemaDataType::primitive("binary".to_string()))
+            }
+            ArrowDataType::LargeBinary => {
+                Ok(schema::SchemaDataType::primitive("binary".to_string()))
+            }
             ArrowDataType::Decimal128(p, s) => Ok(schema::SchemaDataType::primitive(format!(
                 "decimal({p},{s})"
             ))),
             ArrowDataType::Decimal256(p, s) => Ok(schema::SchemaDataType::primitive(format!(
                 "decimal({p},{s})"
             ))),
             ArrowDataType::Date32 => Ok(schema::SchemaDataType::primitive("date".to_string())),
+            ArrowDataType::Date64 => Ok(schema::SchemaDataType::primitive("date".to_string())),
             ArrowDataType::Timestamp(TimeUnit::Microsecond, None) => {
                 Ok(schema::SchemaDataType::primitive("timestamp".to_string()))
             }
             ArrowDataType::Timestamp(TimeUnit::Microsecond, Some(tz))
                 if tz.eq_ignore_ascii_case("utc") =>
             {
                 Ok(schema::SchemaDataType::primitive("timestamp".to_string()))
             }
             ArrowDataType::Struct(fields) => {
-                let converted_fields: Result<Vec<schema::SchemaField>, _> =
-                    fields.iter().map(|field| field.try_into()).collect();
+                let converted_fields: Result<Vec<schema::SchemaField>, _> = fields
+                    .iter()
+                    .map(|field| field.as_ref().try_into())
+                    .collect();
                 Ok(schema::SchemaDataType::r#struct(
                     schema::SchemaTypeStruct::new(converted_fields?),
                 ))
             }
             ArrowDataType::List(field) => {
                 Ok(schema::SchemaDataType::array(schema::SchemaTypeArray::new(
                     Box::new((*field).data_type().try_into()?),
                     (*field).is_nullable(),
                 )))
             }
+            ArrowDataType::LargeList(field) => {
+                Ok(schema::SchemaDataType::array(schema::SchemaTypeArray::new(
+                    Box::new((*field).data_type().try_into()?),
+                    (*field).is_nullable(),
+                )))
+            }
             ArrowDataType::FixedSizeList(field, _) => {
                 Ok(schema::SchemaDataType::array(schema::SchemaTypeArray::new(
                     Box::new((*field).data_type().try_into()?),
                     (*field).is_nullable(),
                 )))
             }
             ArrowDataType::Map(field, _) => {
@@ -284,116 +312,148 @@
     partition_columns: &[String],
     use_extended_remove_schema: bool,
 ) -> ArrowSchemaRef {
     lazy_static! {
         static ref SCHEMA_FIELDS: Vec<ArrowField> = vec![
             ArrowField::new(
                 "metaData",
-                ArrowDataType::Struct(vec![
-                    ArrowField::new("id", ArrowDataType::Utf8, true),
-                    ArrowField::new("name", ArrowDataType::Utf8, true),
-                    ArrowField::new("description", ArrowDataType::Utf8, true),
-                    ArrowField::new("schemaString", ArrowDataType::Utf8, true),
-                    ArrowField::new("createdTime", ArrowDataType::Int64, true),
-                    ArrowField::new(
-                        "partitionColumns",
-                        ArrowDataType::List(Box::new(ArrowField::new(
-                            "element",
-                            ArrowDataType::Utf8,
+                ArrowDataType::Struct(
+                    vec![
+                        ArrowField::new("id", ArrowDataType::Utf8, true),
+                        ArrowField::new("name", ArrowDataType::Utf8, true),
+                        ArrowField::new("description", ArrowDataType::Utf8, true),
+                        ArrowField::new("schemaString", ArrowDataType::Utf8, true),
+                        ArrowField::new("createdTime", ArrowDataType::Int64, true),
+                        ArrowField::new(
+                            "partitionColumns",
+                            ArrowDataType::List(Arc::new(ArrowField::new(
+                                "element",
+                                ArrowDataType::Utf8,
+                                true
+                            ))),
                             true
-                        ))),
-                        true
-                    ),
-                    ArrowField::new(
-                        "configuration",
-                        ArrowDataType::Map(
-                            Box::new(ArrowField::new(
-                                "key_value",
-                                ArrowDataType::Struct(vec![
-                                    ArrowField::new("key", ArrowDataType::Utf8, false),
-                                    ArrowField::new("value", ArrowDataType::Utf8, true),
-                                ]),
-                                false
-                            )),
-                            false
                         ),
-                        true
-                    ),
-                    ArrowField::new(
-                        "format",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("provider", ArrowDataType::Utf8, true),
-                            ArrowField::new(
-                                "options",
-                                ArrowDataType::Map(
-                                    Box::new(ArrowField::new(
-                                        "key_value",
-                                        ArrowDataType::Struct(vec![
+                        ArrowField::new(
+                            "configuration",
+                            ArrowDataType::Map(
+                                Arc::new(ArrowField::new(
+                                    "key_value",
+                                    ArrowDataType::Struct(
+                                        vec![
                                             ArrowField::new("key", ArrowDataType::Utf8, false),
                                             ArrowField::new("value", ArrowDataType::Utf8, true),
-                                        ]),
-                                        false
-                                    )),
+                                        ]
+                                        .into()
+                                    ),
                                     false
-                                ),
+                                )),
                                 false
-                            )
-                        ]),
-                        true
-                    ),
-                ]),
+                            ),
+                            true
+                        ),
+                        ArrowField::new(
+                            "format",
+                            ArrowDataType::Struct(
+                                vec![
+                                    ArrowField::new("provider", ArrowDataType::Utf8, true),
+                                    ArrowField::new(
+                                        "options",
+                                        ArrowDataType::Map(
+                                            Arc::new(ArrowField::new(
+                                                "key_value",
+                                                ArrowDataType::Struct(
+                                                    vec![
+                                                        ArrowField::new(
+                                                            "key",
+                                                            ArrowDataType::Utf8,
+                                                            false
+                                                        ),
+                                                        ArrowField::new(
+                                                            "value",
+                                                            ArrowDataType::Utf8,
+                                                            true
+                                                        ),
+                                                    ]
+                                                    .into()
+                                                ),
+                                                false
+                                            )),
+                                            false
+                                        ),
+                                        false
+                                    )
+                                ]
+                                .into()
+                            ),
+                            true
+                        ),
+                    ]
+                    .into()
+                ),
                 true
             ),
             ArrowField::new(
                 "protocol",
-                ArrowDataType::Struct(vec![
-                    ArrowField::new("minReaderVersion", ArrowDataType::Int32, true),
-                    ArrowField::new("minWriterVersion", ArrowDataType::Int32, true),
-                ]),
+                ArrowDataType::Struct(
+                    vec![
+                        ArrowField::new("minReaderVersion", ArrowDataType::Int32, true),
+                        ArrowField::new("minWriterVersion", ArrowDataType::Int32, true),
+                    ]
+                    .into()
+                ),
                 true
             ),
             ArrowField::new(
                 "txn",
-                ArrowDataType::Struct(vec![
-                    ArrowField::new("appId", ArrowDataType::Utf8, true),
-                    ArrowField::new("version", ArrowDataType::Int64, true),
-                ]),
+                ArrowDataType::Struct(
+                    vec![
+                        ArrowField::new("appId", ArrowDataType::Utf8, true),
+                        ArrowField::new("version", ArrowDataType::Int64, true),
+                    ]
+                    .into()
+                ),
                 true
             ),
         ];
         static ref ADD_FIELDS: Vec<ArrowField> = vec![
             ArrowField::new("path", ArrowDataType::Utf8, true),
             ArrowField::new("size", ArrowDataType::Int64, true),
             ArrowField::new("modificationTime", ArrowDataType::Int64, true),
             ArrowField::new("dataChange", ArrowDataType::Boolean, true),
             ArrowField::new("stats", ArrowDataType::Utf8, true),
             ArrowField::new(
                 "partitionValues",
                 ArrowDataType::Map(
-                    Box::new(ArrowField::new(
+                    Arc::new(ArrowField::new(
                         "key_value",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("key", ArrowDataType::Utf8, false),
-                            ArrowField::new("value", ArrowDataType::Utf8, true),
-                        ]),
+                        ArrowDataType::Struct(
+                            vec![
+                                ArrowField::new("key", ArrowDataType::Utf8, false),
+                                ArrowField::new("value", ArrowDataType::Utf8, true),
+                            ]
+                            .into()
+                        ),
                         false
                     )),
                     false
                 ),
                 true
             ),
             ArrowField::new(
                 "tags",
                 ArrowDataType::Map(
-                    Box::new(ArrowField::new(
+                    Arc::new(ArrowField::new(
                         "key_value",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("key", ArrowDataType::Utf8, false),
-                            ArrowField::new("value", ArrowDataType::Utf8, true),
-                        ]),
+                        ArrowDataType::Struct(
+                            vec![
+                                ArrowField::new("key", ArrowDataType::Utf8, false),
+                                ArrowField::new("value", ArrowDataType::Utf8, true),
+                            ]
+                            .into()
+                        ),
                         false
                     )),
                     false
                 ),
                 true
             )
         ];
@@ -404,103 +464,116 @@
             ArrowField::new("extendedFileMetadata", ArrowDataType::Boolean, true),
         ];
         static ref REMOVE_EXTENDED_FILE_METADATA_FIELDS: Vec<ArrowField> = vec![
             ArrowField::new("size", ArrowDataType::Int64, true),
             ArrowField::new(
                 "partitionValues",
                 ArrowDataType::Map(
-                    Box::new(ArrowField::new(
+                    Arc::new(ArrowField::new(
                         "key_value",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("key", ArrowDataType::Utf8, false),
-                            ArrowField::new("value", ArrowDataType::Utf8, true),
-                        ]),
+                        ArrowDataType::Struct(
+                            vec![
+                                ArrowField::new("key", ArrowDataType::Utf8, false),
+                                ArrowField::new("value", ArrowDataType::Utf8, true),
+                            ]
+                            .into()
+                        ),
                         false
                     )),
                     false
                 ),
                 true
             ),
             ArrowField::new(
                 "tags",
                 ArrowDataType::Map(
-                    Box::new(ArrowField::new(
+                    Arc::new(ArrowField::new(
                         "key_value",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("key", ArrowDataType::Utf8, false),
-                            ArrowField::new("value", ArrowDataType::Utf8, true),
-                        ]),
+                        ArrowDataType::Struct(
+                            vec![
+                                ArrowField::new("key", ArrowDataType::Utf8, false),
+                                ArrowField::new("value", ArrowDataType::Utf8, true),
+                            ]
+                            .into()
+                        ),
                         false
                     )),
                     false
                 ),
                 true
             )
         ];
     }
 
     // create add fields according to the specific data table schema
-    let (partition_fields, non_partition_fields): (Vec<ArrowField>, Vec<ArrowField>) = table_schema
-        .fields()
-        .iter()
-        .map(|f| f.to_owned())
-        .partition(|field| partition_columns.contains(field.name()));
+    let (partition_fields, non_partition_fields): (Vec<ArrowFieldRef>, Vec<ArrowFieldRef>) =
+        table_schema
+            .fields()
+            .iter()
+            .map(|field| field.to_owned())
+            .partition(|field| partition_columns.contains(field.name()));
+
     let mut stats_parsed_fields: Vec<ArrowField> =
         vec![ArrowField::new("numRecords", ArrowDataType::Int64, true)];
     if !non_partition_fields.is_empty() {
         let mut max_min_vec = Vec::new();
         non_partition_fields
             .iter()
             .for_each(|f| max_min_schema_for_fields(&mut max_min_vec, f));
 
-        stats_parsed_fields.extend(
-            ["minValues", "maxValues"].into_iter().map(|name| {
-                ArrowField::new(name, ArrowDataType::Struct(max_min_vec.clone()), true)
-            }),
-        );
+        stats_parsed_fields.extend(["minValues", "maxValues"].into_iter().map(|name| {
+            ArrowField::new(
+                name,
+                ArrowDataType::Struct(max_min_vec.clone().into()),
+                true,
+            )
+        }));
 
         let mut null_count_vec = Vec::new();
         non_partition_fields
             .iter()
             .for_each(|f| null_count_schema_for_fields(&mut null_count_vec, f));
-        let null_count_struct =
-            ArrowField::new("nullCount", ArrowDataType::Struct(null_count_vec), true);
+        let null_count_struct = ArrowField::new(
+            "nullCount",
+            ArrowDataType::Struct(null_count_vec.into()),
+            true,
+        );
 
         stats_parsed_fields.push(null_count_struct);
     }
     let mut add_fields = ADD_FIELDS.clone();
     add_fields.push(ArrowField::new(
         "stats_parsed",
-        ArrowDataType::Struct(stats_parsed_fields),
+        ArrowDataType::Struct(stats_parsed_fields.into()),
         true,
     ));
     if !partition_fields.is_empty() {
         add_fields.push(ArrowField::new(
             "partitionValues_parsed",
-            ArrowDataType::Struct(partition_fields),
+            ArrowDataType::Struct(partition_fields.into()),
             true,
         ));
     }
 
     // create remove fields with or without extendedFileMetadata
     let mut remove_fields = REMOVE_FIELDS.clone();
     if use_extended_remove_schema {
         remove_fields.extend(REMOVE_EXTENDED_FILE_METADATA_FIELDS.clone());
     }
 
     // include add and remove fields in checkpoint schema
     let mut schema_fields = SCHEMA_FIELDS.clone();
     schema_fields.push(ArrowField::new(
         "add",
-        ArrowDataType::Struct(add_fields),
+        ArrowDataType::Struct(add_fields.into()),
         true,
     ));
     schema_fields.push(ArrowField::new(
         "remove",
-        ArrowDataType::Struct(remove_fields),
+        ArrowDataType::Struct(remove_fields.into()),
         true,
     ));
 
     let arrow_schema = ArrowSchema::new(schema_fields);
 
     std::sync::Arc::new(arrow_schema)
 }
@@ -512,15 +585,15 @@
 
             for f in struct_fields {
                 max_min_schema_for_fields(&mut child_dest, f);
             }
 
             dest.push(ArrowField::new(
                 f.name(),
-                ArrowDataType::Struct(child_dest),
+                ArrowDataType::Struct(child_dest.into()),
                 true,
             ));
         }
         // don't compute min or max for list or map types
         ArrowDataType::List(_) | ArrowDataType::Map(_, _) => { /* noop */ }
         _ => {
             let f = f.clone();
@@ -536,29 +609,30 @@
 
             for f in struct_fields {
                 null_count_schema_for_fields(&mut child_dest, f);
             }
 
             dest.push(ArrowField::new(
                 f.name(),
-                ArrowDataType::Struct(child_dest),
+                ArrowDataType::Struct(child_dest.into()),
                 true,
             ));
         }
         _ => {
             let f = ArrowField::new(f.name(), ArrowDataType::Int64, true);
             dest.push(f);
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::collections::HashMap;
+    use std::sync::Arc;
 
     #[test]
     fn delta_log_schema_for_table_test() {
         // NOTE: We should future proof the checkpoint schema in case action schema changes.
         // See https://github.com/delta-io/delta-rs/issues/287
 
         let table_schema = ArrowSchema::new(vec![
@@ -594,15 +668,18 @@
             .iter()
             .map(|f| (f.name().to_owned(), f.clone()))
             .collect();
         let partition_values_parsed = add_field_map.get("partitionValues_parsed").unwrap();
         if let ArrowDataType::Struct(fields) = partition_values_parsed.data_type() {
             assert_eq!(1, fields.len());
             let field = fields.get(0).unwrap().to_owned();
-            assert_eq!(ArrowField::new("pcol", ArrowDataType::Int32, true), field);
+            assert_eq!(
+                Arc::new(ArrowField::new("pcol", ArrowDataType::Int32, true)),
+                field
+            );
         } else {
             unreachable!();
         }
         let stats_parsed = add_field_map.get("stats_parsed").unwrap();
         if let ArrowDataType::Struct(fields) = stats_parsed.data_type() {
             assert_eq!(4, fields.len());
 
@@ -618,15 +695,15 @@
                             assert_eq!(1, fields.len());
                             let field = fields.get(0).unwrap().to_owned();
                             let data_type = if k == "nullCount" {
                                 ArrowDataType::Int64
                             } else {
                                 ArrowDataType::Int32
                             };
-                            assert_eq!(ArrowField::new("col1", data_type, true), field);
+                            assert_eq!(Arc::new(ArrowField::new("col1", data_type, true)), field);
                         }
                         _ => unreachable!(),
                     },
                     "numRecords" => {}
                     _ => panic!(),
                 }
             }
@@ -722,49 +799,124 @@
             crate::SchemaDataType::primitive("timestamp".to_string())
         );
     }
 
     #[test]
     fn test_delta_from_arrow_timestamp_type_with_tz() {
         let timestamp_field =
-            ArrowDataType::Timestamp(TimeUnit::Microsecond, Some("UTC".to_string()));
+            ArrowDataType::Timestamp(TimeUnit::Microsecond, Some("UTC".to_string().into()));
         assert_eq!(
             <crate::SchemaDataType as TryFrom<&ArrowDataType>>::try_from(&timestamp_field).unwrap(),
             crate::SchemaDataType::primitive("timestamp".to_string())
         );
     }
 
     #[test]
+    fn test_delta_from_arrow_map_type() {
+        let arrow_map = ArrowDataType::Map(
+            Arc::new(ArrowField::new(
+                "key_value",
+                ArrowDataType::Struct(
+                    vec![
+                        ArrowField::new("key", ArrowDataType::Int8, false),
+                        ArrowField::new("value", ArrowDataType::Binary, true),
+                    ]
+                    .into(),
+                ),
+                true,
+            )),
+            false,
+        );
+        let converted_map: crate::SchemaDataType = (&arrow_map).try_into().unwrap();
+
+        assert_eq!(
+            converted_map,
+            crate::SchemaDataType::map(crate::SchemaTypeMap::new(
+                Box::new(crate::SchemaDataType::primitive("byte".to_string())),
+                Box::new(crate::SchemaDataType::primitive("binary".to_string())),
+                true,
+            ))
+        );
+    }
+
+    #[test]
+    fn test_record_batch_from_map_type() {
+        let keys = vec!["0", "1", "5", "6", "7"];
+        let values: Vec<&[u8]> = vec![
+            b"test_val_1",
+            b"test_val_2",
+            b"long_test_val_3",
+            b"4",
+            b"test_val_5",
+        ];
+        let entry_offsets = vec![0u32, 1, 1, 4, 5, 5];
+        let num_rows = keys.len();
+
+        let map_array = arrow::array::MapArray::new_from_strings(
+            keys.into_iter(),
+            &arrow::array::BinaryArray::from(values),
+            entry_offsets.as_slice(),
+        )
+        .expect("Could not create a map array");
+
+        let schema = <arrow::datatypes::Schema as TryFrom<&crate::Schema>>::try_from(
+            &crate::Schema::new(vec![crate::SchemaField::new(
+                "example".to_string(),
+                crate::SchemaDataType::map(crate::SchemaTypeMap::new(
+                    Box::new(crate::SchemaDataType::primitive("string".to_string())),
+                    Box::new(crate::SchemaDataType::primitive("binary".to_string())),
+                    false,
+                )),
+                false,
+                HashMap::new(),
+            )]),
+        )
+        .expect("Could not get schema");
+
+        let record_batch =
+            arrow::record_batch::RecordBatch::try_new(Arc::new(schema), vec![Arc::new(map_array)])
+                .expect("Failed to create RecordBatch");
+
+        assert_eq!(record_batch.num_columns(), 1);
+        assert_eq!(record_batch.num_rows(), num_rows);
+    }
+
+    #[test]
     fn test_max_min_schema_for_fields() {
         let mut max_min_vec: Vec<ArrowField> = Vec::new();
         let fields = [
             ArrowField::new("simple", ArrowDataType::Int32, true),
             ArrowField::new(
                 "struct",
-                ArrowDataType::Struct(vec![ArrowField::new("simple", ArrowDataType::Int32, true)]),
+                ArrowDataType::Struct(
+                    vec![ArrowField::new("simple", ArrowDataType::Int32, true)].into(),
+                ),
                 true,
             ),
             ArrowField::new(
                 "list",
-                ArrowDataType::List(Box::new(ArrowField::new(
+                ArrowDataType::List(Arc::new(ArrowField::new(
                     "simple",
                     ArrowDataType::Int32,
                     true,
                 ))),
                 true,
             ),
             ArrowField::new(
                 "map",
                 ArrowDataType::Map(
-                    Box::new(ArrowField::new(
+                    Arc::new(ArrowField::new(
                         "struct",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("key", ArrowDataType::Int32, true),
-                            ArrowField::new("value", ArrowDataType::Int32, true),
-                        ]),
+                        ArrowDataType::Struct(
+                            vec![
+                                ArrowField::new("key", ArrowDataType::Int32, true),
+                                ArrowField::new("value", ArrowDataType::Int32, true),
+                            ]
+                            .into(),
+                        ),
                         true,
                     )),
                     true,
                 ),
                 true,
             ),
         ];
@@ -783,53 +935,81 @@
         let mut null_count_vec: Vec<ArrowField> = Vec::new();
         let fields = [
             ArrowField::new("int32", ArrowDataType::Int32, true),
             ArrowField::new("int64", ArrowDataType::Int64, true),
             ArrowField::new("Utf8", ArrowDataType::Utf8, true),
             ArrowField::new(
                 "list",
-                ArrowDataType::List(Box::new(ArrowField::new(
+                ArrowDataType::List(Arc::new(ArrowField::new(
                     "simple",
                     ArrowDataType::Int32,
                     true,
                 ))),
                 true,
             ),
             ArrowField::new(
                 "map",
                 ArrowDataType::Map(
-                    Box::new(ArrowField::new(
+                    Arc::new(ArrowField::new(
                         "struct",
-                        ArrowDataType::Struct(vec![
-                            ArrowField::new("key", ArrowDataType::Int32, true),
-                            ArrowField::new("value", ArrowDataType::Int32, true),
-                        ]),
+                        ArrowDataType::Struct(
+                            vec![
+                                ArrowField::new("key", ArrowDataType::Int32, true),
+                                ArrowField::new("value", ArrowDataType::Int32, true),
+                            ]
+                            .into(),
+                        ),
                         true,
                     )),
                     true,
                 ),
                 true,
             ),
             ArrowField::new(
                 "struct",
-                ArrowDataType::Struct(vec![ArrowField::new("int32", ArrowDataType::Int32, true)]),
+                ArrowDataType::Struct(
+                    vec![ArrowField::new("int32", ArrowDataType::Int32, true)].into(),
+                ),
                 true,
             ),
         ];
         let expected = vec![
             ArrowField::new(fields[0].name(), ArrowDataType::Int64, true),
             ArrowField::new(fields[1].name(), ArrowDataType::Int64, true),
             ArrowField::new(fields[2].name(), ArrowDataType::Int64, true),
             ArrowField::new(fields[3].name(), ArrowDataType::Int64, true),
             ArrowField::new(fields[4].name(), ArrowDataType::Int64, true),
             ArrowField::new(
                 fields[5].name(),
-                ArrowDataType::Struct(vec![ArrowField::new("int32", ArrowDataType::Int64, true)]),
+                ArrowDataType::Struct(
+                    vec![ArrowField::new("int32", ArrowDataType::Int64, true)].into(),
+                ),
                 true,
             ),
         ];
         fields
             .iter()
             .for_each(|f| null_count_schema_for_fields(&mut null_count_vec, f));
         assert_eq!(null_count_vec, expected);
     }
+
+    /*
+     * This test validates the trait implementation of
+     * TryFrom<&Arc<ArrowField>> for schema::SchemaField which is required with Arrow 37 since
+     * iterators on Fields will give an &Arc<ArrowField>
+     */
+    #[test]
+    fn tryfrom_arrowfieldref_with_structs() {
+        let field = Arc::new(ArrowField::new(
+            "test_struct",
+            ArrowDataType::Struct(
+                vec![
+                    ArrowField::new("key", ArrowDataType::Int32, true),
+                    ArrowField::new("value", ArrowDataType::Int32, true),
+                ]
+                .into(),
+            ),
+            true,
+        ));
+        let _converted: schema::SchemaField = field.as_ref().try_into().unwrap();
+    }
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/delta_config.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/delta_config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use serde::{Deserialize, Serialize};
 
 use crate::DeltaTableError;
 
 /// Typed property keys that can be defined on a delta table
 /// <https://docs.delta.io/latest/table-properties.html#delta-table-properties-reference>
 /// <https://learn.microsoft.com/en-us/azure/databricks/delta/table-properties>
+#[derive(PartialEq, Eq, Hash)]
 pub enum DeltaConfigKey {
     /// true for this Delta table to be append-only. If append-only,
     /// existing records cannot be deleted, and existing values cannot be updated.
     AppendOnly,
 
     /// true for Delta Lake to automatically optimize the layout of the files for this Delta table.
     AutoOptimizeAutoCompact,
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/delta_datafusion.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/delta_datafusion.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,30 @@
 use datafusion::datasource::{listing::PartitionedFile, MemTable, TableProvider, TableType};
 use datafusion::execution::context::{SessionContext, SessionState, TaskContext};
 use datafusion::execution::runtime_env::RuntimeEnv;
 use datafusion::execution::FunctionRegistry;
 use datafusion::optimizer::utils::conjunction;
 use datafusion::physical_expr::PhysicalSortExpr;
 use datafusion::physical_optimizer::pruning::{PruningPredicate, PruningStatistics};
-use datafusion::physical_plan::file_format::{partition_type_wrap, FileScanConfig};
+use datafusion::physical_plan::file_format::FileScanConfig;
 use datafusion::physical_plan::{
     ColumnStatistics, ExecutionPlan, Partitioning, SendableRecordBatchStream, Statistics,
 };
 use datafusion_common::scalar::ScalarValue;
-use datafusion_common::{Column, DataFusionError, Result as DataFusionResult};
+use datafusion_common::{Column, DataFusionError, Result as DataFusionResult, ToDFSchema};
 use datafusion_expr::logical_plan::CreateExternalTable;
 use datafusion_expr::{Expr, Extension, LogicalPlan, TableProviderFilterPushDown};
+use datafusion_physical_expr::execution_props::ExecutionProps;
+use datafusion_physical_expr::{create_physical_expr, PhysicalExpr};
 use datafusion_proto::logical_plan::LogicalExtensionCodec;
 use datafusion_proto::physical_plan::PhysicalExtensionCodec;
-use object_store::{path::Path, ObjectMeta};
+use object_store::ObjectMeta;
 use url::Url;
 
 use crate::builder::ensure_table_uri;
-use crate::schema;
 use crate::{action, open_table, open_table_with_storage_options, SchemaDataType};
 use crate::{DeltaResult, Invariant};
 use crate::{DeltaTable, DeltaTableError};
 
 impl From<DeltaTableError> for DataFusionError {
     fn from(err: DeltaTableError) -> Self {
         match err {
@@ -333,32 +334,25 @@
 }
 
 // each delta table must register a specific object store, since paths are internally
 // handled relative to the table root.
 fn register_store(table: &DeltaTable, env: Arc<RuntimeEnv>) {
     let object_store_url = table.storage.object_store_url();
     let url: &Url = object_store_url.as_ref();
-    env.register_object_store(
-        url.scheme(),
-        url.host_str().unwrap_or_default(),
-        table.object_store(),
-    );
+    env.register_object_store(url, table.object_store());
 }
 
 #[async_trait]
 impl TableProvider for DeltaTable {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn schema(&self) -> Arc<ArrowSchema> {
-        Arc::new(
-            <ArrowSchema as TryFrom<&schema::Schema>>::try_from(DeltaTable::schema(self).unwrap())
-                .unwrap(),
-        )
+        self.state.arrow_schema().unwrap()
     }
 
     fn table_type(&self) -> TableType {
         TableType::Base
     }
 
     fn get_table_definition(&self) -> Option<&str> {
@@ -372,29 +366,31 @@
     async fn scan(
         &self,
         session: &SessionState,
         projection: Option<&Vec<usize>>,
         filters: &[Expr],
         limit: Option<usize>,
     ) -> DataFusionResult<Arc<dyn ExecutionPlan>> {
-        let schema = Arc::new(<ArrowSchema as TryFrom<&schema::Schema>>::try_from(
-            DeltaTable::schema(self).unwrap(),
-        )?);
+        let schema = self
+            .state
+            .physical_arrow_schema(self.object_store())
+            .await?;
 
         register_store(self, session.runtime_env().clone());
 
+        let filter_expr = conjunction(filters.iter().cloned())
+            .map(|expr| logical_expr_to_physical_expr(&expr, &schema));
+
         // TODO we group files together by their partition values. If the table is partitioned
         // and partitions are somewhat evenly distributed, probably not the worst choice ...
         // However we may want to do some additional balancing in case we are far off from the above.
         let mut file_groups: HashMap<Vec<ScalarValue>, Vec<PartitionedFile>> = HashMap::new();
-        if let Some(Some(predicate)) =
-            (!filters.is_empty()).then_some(conjunction(filters.iter().cloned()))
-        {
-            let pruning_predicate = PruningPredicate::try_new(predicate, schema.clone())?;
-            let files_to_prune = pruning_predicate.prune(self)?;
+        if let Some(predicate) = &filter_expr {
+            let pruning_predicate = PruningPredicate::try_new(predicate.clone(), schema.clone())?;
+            let files_to_prune = pruning_predicate.prune(&self.state)?;
             self.get_state()
                 .files()
                 .iter()
                 .zip(files_to_prune.into_iter())
                 .for_each(|(action, keep_file)| {
                     if keep_file {
                         let part = partitioned_file_from_action(action, &schema);
@@ -417,40 +413,37 @@
         let table_partition_cols = self.get_metadata()?.partition_columns.clone();
         let file_schema = Arc::new(ArrowSchema::new(
             schema
                 .fields()
                 .iter()
                 .filter(|f| !table_partition_cols.contains(f.name()))
                 .cloned()
-                .collect(),
+                .collect::<Vec<arrow::datatypes::FieldRef>>(),
         ));
 
+        let table_partition_cols = table_partition_cols
+            .iter()
+            .map(|c| Ok((c.to_owned(), schema.field_with_name(c)?.data_type().clone())))
+            .collect::<Result<Vec<_>, ArrowError>>()?;
+
         let parquet_scan = ParquetFormat::new()
             .create_physical_plan(
                 session,
                 FileScanConfig {
                     object_store_url: self.storage.object_store_url(),
                     file_schema,
                     file_groups: file_groups.into_values().collect(),
                     statistics: self.datafusion_table_statistics(),
                     projection: projection.cloned(),
                     limit,
-                    table_partition_cols: table_partition_cols
-                        .iter()
-                        .map(|c| {
-                            Ok((
-                                c.to_owned(),
-                                partition_type_wrap(schema.field_with_name(c)?.data_type().clone()),
-                            ))
-                        })
-                        .collect::<Result<Vec<_>, ArrowError>>()?,
+                    table_partition_cols,
                     output_ordering: None,
                     infinite_source: false,
                 },
-                filters,
+                filter_expr.as_ref(),
             )
             .await?;
 
         Ok(Arc::new(DeltaScan {
             table_uri: ensure_table_uri(self.table_uri())?.as_str().into(),
             parquet_scan,
         }))
@@ -555,15 +548,15 @@
                 TimeUnit::Microsecond => ScalarValue::TimestampMicrosecond(None, tz),
                 TimeUnit::Nanosecond => ScalarValue::TimestampNanosecond(None, tz),
             })
         }
         //Unsupported types...
         ArrowDataType::Float16
         | ArrowDataType::Decimal256(_, _)
-        | ArrowDataType::Union(_, _, _)
+        | ArrowDataType::Union(_, _)
         | ArrowDataType::Dictionary(_, _)
         | ArrowDataType::LargeList(_)
         | ArrowDataType::Struct(_)
         | ArrowDataType::List(_)
         | ArrowDataType::FixedSizeList(_, _)
         | ArrowDataType::Time32(_)
         | ArrowDataType::Time64(_)
@@ -597,17 +590,16 @@
     let ts_ns = (action.modification_time % 1000) * 1_000_000;
     let last_modified = DateTime::<Utc>::from_utc(
         NaiveDateTime::from_timestamp_opt(ts_secs, ts_ns as u32).unwrap(),
         Utc,
     );
     PartitionedFile {
         object_meta: ObjectMeta {
-            location: Path::from(action.path.clone()),
             last_modified,
-            size: action.size as usize,
+            ..action.try_into().unwrap()
         },
         partition_values,
         range: None,
         extensions: None,
     }
 }
 
@@ -626,15 +618,15 @@
         serde_json::Value::String(s) => Some(ScalarValue::from(s.as_str())),
         serde_json::Value::Array(_) => None,
         serde_json::Value::Object(_) => None,
         serde_json::Value::Null => None,
     }
 }
 
-fn to_correct_scalar_value(
+pub(crate) fn to_correct_scalar_value(
     stat_val: &serde_json::Value,
     field_dt: &ArrowDataType,
 ) -> Option<ScalarValue> {
     match stat_val {
         serde_json::Value::Array(_) => None,
         serde_json::Value::Object(_) => None,
         serde_json::Value::Null => get_null_of_arrow_type(field_dt).ok(),
@@ -769,14 +761,23 @@
                 right
             );
             None
         }
     }
 }
 
+pub(crate) fn logical_expr_to_physical_expr(
+    expr: &Expr,
+    schema: &ArrowSchema,
+) -> Arc<dyn PhysicalExpr> {
+    let df_schema = schema.clone().to_dfschema().unwrap();
+    let execution_props = ExecutionProps::new();
+    create_physical_expr(expr, &df_schema, schema, &execution_props).unwrap()
+}
+
 /// Responsible for checking batches of data conform to table's invariants.
 #[derive(Clone)]
 pub struct DeltaDataChecker {
     invariants: Vec<Invariant>,
     ctx: SessionContext,
 }
 
@@ -946,14 +947,15 @@
     use arrow::array::StructArray;
     use arrow::datatypes::{DataType, Field, Schema};
     use chrono::{TimeZone, Utc};
     use datafusion::from_slice::FromSlice;
     use datafusion::physical_plan::empty::EmptyExec;
     use datafusion_proto::physical_plan::AsExecutionPlan;
     use datafusion_proto::protobuf;
+    use object_store::path::Path;
     use serde_json::json;
     use std::ops::Deref;
 
     use super::*;
 
     // test deserialization of serialized partition values.
     // https://github.com/delta-io/delta/blob/master/PROTOCOL.md#partition-value-serialization
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/lib.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 pub mod delta_datafusion;
 #[cfg(all(feature = "arrow", feature = "parquet"))]
 pub mod writer;
 
 pub use self::builder::*;
 pub use self::data_catalog::{get_data_catalog, DataCatalog, DataCatalogError};
 pub use self::delta::*;
+pub use self::delta_config::*;
 pub use self::partitions::*;
 pub use self::schema::*;
 pub use object_store::{path::Path, Error as ObjectStoreError, ObjectMeta, ObjectStore};
 pub use operations::DeltaOps;
 
 // convenience exports for consumers to avoid aligning crate versions
 #[cfg(feature = "arrow")]
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/create.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/create.rs`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,19 @@
             nullable,
             metadata.unwrap_or_default(),
         ));
         self
     }
 
     /// Specify columns to append to schema
-    pub fn with_columns(mut self, columns: impl IntoIterator<Item = SchemaField>) -> Self {
-        self.columns.extend(columns);
+    pub fn with_columns(
+        mut self,
+        columns: impl IntoIterator<Item = impl Into<SchemaField>>,
+    ) -> Self {
+        self.columns.extend(columns.into_iter().map(|c| c.into()));
         self
     }
 
     /// Specify table partitioning
     pub fn with_partition_columns(
         mut self,
         partition_columns: impl IntoIterator<Item = impl Into<String>>,
@@ -265,15 +268,15 @@
         let mut actions = vec![
             Action::protocol(protocol),
             Action::metaData(MetaData::try_from(metadata)?),
         ];
         actions.extend(
             self.actions
                 .into_iter()
-                .filter(|a| matches!(a, Action::protocol(_))),
+                .filter(|a| !matches!(a, Action::protocol(_))),
         );
 
         Ok((table, actions, operation))
     }
 }
 
 impl std::future::IntoFuture for CreateBuilder {
@@ -281,15 +284,14 @@
     type IntoFuture = BoxFuture<'static, Self::Output>;
 
     fn into_future(self) -> Self::IntoFuture {
         let this = self;
 
         Box::pin(async move {
             let mode = this.mode.clone();
-            let metadata = this.metadata.clone();
             let (mut table, actions, operation) = this.into_table_and_actions()?;
             if table.object_store().is_delta_table_location().await? {
                 match mode {
                     SaveMode::ErrorIfExists => return Err(CreateError::TableAlreadyExists.into()),
                     SaveMode::Append => return Err(CreateError::AppendNotAllowed.into()),
                     SaveMode::Ignore => {
                         table.load().await?;
@@ -298,18 +300,18 @@
                     SaveMode::Overwrite => {
                         todo!("Overwriting on create not yet implemented. Use 'write' operation instead.")
                     }
                 }
             }
             let version = commit(
                 table.object_store().as_ref(),
-                0,
                 &actions,
                 operation,
-                metadata,
+                &table.state,
+                None,
             )
             .await?;
             table.load_version(version).await?;
 
             Ok(table)
         })
     }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/filesystem_check.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/filesystem_check.rs`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 //! let mut table = open_table("../path/to/table")?;
 //! let (table, metrics) = FileSystemCheckBuilder::new(table.object_store(), table.state).await?;
 //! ````
 use crate::action::{Action, Add, DeltaOperation, Remove};
 use crate::operations::transaction::commit;
 use crate::storage::DeltaObjectStore;
 use crate::table_state::DeltaTableState;
-use crate::DeltaDataTypeVersion;
 use crate::{DeltaDataTypeLong, DeltaResult, DeltaTable, DeltaTableError};
 use futures::future::BoxFuture;
 use futures::StreamExt;
 pub use object_store::path::Path;
 use object_store::ObjectStore;
 use std::collections::HashMap;
 use std::fmt::Debug;
@@ -29,15 +28,15 @@
 use url::{ParseError, Url};
 
 /// Audit the Delta Table's active files with the underlying file system.
 /// See this module's documentaiton for more information
 #[derive(Debug)]
 pub struct FileSystemCheckBuilder {
     /// A snapshot of the to-be-checked table's state
-    state: DeltaTableState,
+    snapshot: DeltaTableState,
     /// Delta object store for handling data files
     store: Arc<DeltaObjectStore>,
     /// Don't remove actions to the table log. Just determine which files can be removed
     dry_run: bool,
 }
 
 /// Details of the FSCK operation including which files were removed from the log
@@ -46,16 +45,14 @@
     /// Was this a dry run
     pub dry_run: bool,
     /// Files that wrere removed successfully
     pub files_removed: Vec<String>,
 }
 
 struct FileSystemCheckPlan {
-    /// Version of the snapshot provided
-    version: DeltaDataTypeVersion,
     /// Delta object store for handling data files
     store: Arc<DeltaObjectStore>,
     /// Files that no longer exists in undlying ObjectStore but have active add actions
     pub files_to_remove: Vec<Add>,
 }
 
 fn is_absolute_path(path: &str) -> DeltaResult<bool> {
@@ -69,33 +66,32 @@
     }
 }
 
 impl FileSystemCheckBuilder {
     /// Create a new [`FileSystemCheckBuilder`]
     pub fn new(store: Arc<DeltaObjectStore>, state: DeltaTableState) -> Self {
         FileSystemCheckBuilder {
-            state,
+            snapshot: state,
             store,
             dry_run: false,
         }
     }
 
     /// Only determine which add actions should be removed. A dry run will not commit actions to the Delta log
     pub fn with_dry_run(mut self, dry_run: bool) -> Self {
         self.dry_run = dry_run;
         self
     }
 
     async fn create_fsck_plan(&self) -> DeltaResult<FileSystemCheckPlan> {
         let mut files_relative: HashMap<&str, &Add> =
-            HashMap::with_capacity(self.state.files().len());
-        let version = self.state.version();
+            HashMap::with_capacity(self.snapshot.files().len());
         let store = self.store.clone();
 
-        for active in self.state.files() {
+        for active in self.snapshot.files() {
             if is_absolute_path(&active.path)? {
                 return Err(DeltaTableError::Generic(
                     "Filesystem check does not support absolute paths".to_string(),
                 ));
             } else {
                 files_relative.insert(&active.path, active);
             }
@@ -114,33 +110,30 @@
         let files_to_remove: Vec<Add> = files_relative
             .into_values()
             .map(|file| file.to_owned())
             .collect();
 
         Ok(FileSystemCheckPlan {
             files_to_remove,
-            version,
             store,
         })
     }
 }
 
 impl FileSystemCheckPlan {
-    pub async fn execute(self) -> DeltaResult<FileSystemCheckMetrics> {
+    pub async fn execute(self, snapshot: &DeltaTableState) -> DeltaResult<FileSystemCheckMetrics> {
         if self.files_to_remove.is_empty() {
             return Ok(FileSystemCheckMetrics {
                 dry_run: false,
                 files_removed: Vec::new(),
             });
         }
 
         let mut actions = Vec::with_capacity(self.files_to_remove.len());
         let mut removed_file_paths = Vec::with_capacity(self.files_to_remove.len());
-        let version = self.version;
-        let store = &self.store;
 
         for file in self.files_to_remove {
             let deletion_time = SystemTime::now().duration_since(UNIX_EPOCH).unwrap();
             let deletion_time = deletion_time.as_millis() as DeltaDataTypeLong;
             removed_file_paths.push(file.path.clone());
             actions.push(Action::remove(Remove {
                 path: file.path,
@@ -150,18 +143,19 @@
                 partition_values: Some(file.partition_values),
                 size: Some(file.size),
                 tags: file.tags,
             }));
         }
 
         commit(
-            store,
-            version + 1,
+            self.store.as_ref(),
             &actions,
             DeltaOperation::FileSystemCheck {},
+            snapshot,
+            // TODO pass through metadata
             None,
         )
         .await?;
 
         Ok(FileSystemCheckMetrics {
             dry_run: false,
             files_removed: removed_file_paths,
@@ -176,24 +170,24 @@
     fn into_future(self) -> Self::IntoFuture {
         let this = self;
 
         Box::pin(async move {
             let plan = this.create_fsck_plan().await?;
             if this.dry_run {
                 return Ok((
-                    DeltaTable::new_with_state(this.store, this.state),
+                    DeltaTable::new_with_state(this.store, this.snapshot),
                     FileSystemCheckMetrics {
                         files_removed: plan.files_to_remove.into_iter().map(|f| f.path).collect(),
                         dry_run: true,
                     },
                 ));
             }
 
-            let metrics = plan.execute().await?;
-            let mut table = DeltaTable::new_with_state(this.store, this.state);
+            let metrics = plan.execute(&this.snapshot).await?;
+            let mut table = DeltaTable::new_with_state(this.store, this.snapshot);
             table.update().await?;
             Ok((table, metrics))
         })
     }
 }
 
 #[cfg(test)]
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/load.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/common/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,188 @@
+#![allow(dead_code, unused_variables, deprecated)]
+
+use bytes::Bytes;
+use deltalake::action::{self, Add, Remove};
+use deltalake::builder::DeltaTableBuilder;
+use deltalake::storage::DeltaObjectStore;
+use deltalake::{DeltaTable, DeltaTableConfig, DeltaTableMetaData, Schema};
+use object_store::{path::Path, ObjectStore};
+use serde_json::{Map, Value};
+use std::any::Any;
 use std::collections::HashMap;
 use std::sync::Arc;
+use tempdir::TempDir;
 
-use crate::storage::DeltaObjectStore;
-use crate::{builder::ensure_table_uri, DeltaResult, DeltaTable};
+#[cfg(feature = "azure")]
+pub mod adls;
+pub mod clock;
+#[cfg(feature = "datafusion")]
+pub mod datafusion;
+#[cfg(feature = "hdfs")]
+pub mod hdfs;
+#[cfg(any(feature = "s3", feature = "s3-native-tls"))]
+pub mod s3;
+pub mod schemas;
+
+#[derive(Default)]
+pub struct TestContext {
+    /// The main table under test
+    pub table: Option<DeltaTable>,
+    pub backend: Option<Arc<DeltaObjectStore>>,
+    /// The configuration used to create the backend.
+    pub config: HashMap<String, String>,
+    /// An object when it is dropped will clean up any temporary resources created for the test
+    pub storage_context: Option<Box<dyn Any>>,
+}
 
-use datafusion::datasource::TableProvider;
-use datafusion::execution::context::{SessionContext, TaskContext};
-use datafusion::physical_plan::coalesce_partitions::CoalescePartitionsExec;
-use datafusion::physical_plan::{ExecutionPlan, SendableRecordBatchStream};
-use futures::future::BoxFuture;
-
-#[derive(Debug, Clone)]
-pub struct LoadBuilder {
-    location: Option<String>,
-    columns: Option<Vec<String>>,
-    storage_options: Option<HashMap<String, String>>,
-    object_store: Option<Arc<DeltaObjectStore>>,
-}
-
-impl Default for LoadBuilder {
-    fn default() -> Self {
-        Self::new()
-    }
+pub struct LocalFS {
+    pub tmp_dir: TempDir,
 }
 
-impl LoadBuilder {
-    /// Create a new [`LoadBuilder`]
-    pub fn new() -> Self {
-        Self {
-            location: None,
-            columns: None,
-            storage_options: None,
-            object_store: None,
+impl TestContext {
+    pub async fn from_env() -> Self {
+        let backend = std::env::var("DELTA_RS_TEST_BACKEND");
+        let backend_ref = backend.as_ref().map(|s| s.as_str());
+        match backend_ref {
+            Ok("LOCALFS") | Err(std::env::VarError::NotPresent) => setup_local_context().await,
+            #[cfg(feature = "azure")]
+            Ok("AZURE_GEN2") => adls::setup_azure_gen2_context().await,
+            #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
+            Ok("S3_LOCAL_STACK") => s3::setup_s3_context().await,
+            #[cfg(feature = "hdfs")]
+            Ok("HDFS") => hdfs::setup_hdfs_context(),
+            _ => panic!("Invalid backend for delta-rs tests"),
         }
     }
 
-    /// Specify the path to the location where table data is stored,
-    /// which could be a path on distributed storage.
-    pub fn with_location(mut self, location: impl Into<String>) -> Self {
-        self.location = Some(location.into());
-        self
-    }
-
-    /// Specify column selection to load
-    pub fn with_columns(mut self, columns: impl IntoIterator<Item = impl Into<String>>) -> Self {
-        self.columns = Some(columns.into_iter().map(|s| s.into()).collect());
-        self
-    }
-
-    /// Set options used to initialize storage backend
-    ///
-    /// Options may be passed in the HashMap or set as environment variables.
-    ///
-    /// [crate::builder::s3_storage_options] describes the available options for the AWS or S3-compliant backend.
-    /// [dynamodb_lock::DynamoDbLockClient] describes additional options for the AWS atomic rename client.
-    /// [crate::builder::azure_storage_options] describes the available options for the Azure backend.
-    /// [crate::builder::gcp_storage_options] describes the available options for the Google Cloud Platform backend.
-    pub fn with_storage_options(mut self, storage_options: HashMap<String, String>) -> Self {
-        self.storage_options = Some(storage_options);
-        self
-    }
-
-    /// Provide a [`DeltaObjectStore`] instance, that points at table location
-    pub fn with_object_store(mut self, object_store: Arc<DeltaObjectStore>) -> Self {
-        self.object_store = Some(object_store);
-        self
-    }
-}
-
-impl std::future::IntoFuture for LoadBuilder {
-    type Output = DeltaResult<(DeltaTable, SendableRecordBatchStream)>;
-    type IntoFuture = BoxFuture<'static, Self::Output>;
-
-    fn into_future(self) -> Self::IntoFuture {
-        let this = self;
-
-        Box::pin(async move {
-            let object_store = this.object_store.unwrap();
-            let url = ensure_table_uri(object_store.root_uri())?;
-            let store = object_store.storage_backend().clone();
-            let mut table = DeltaTable::new(object_store, Default::default());
-            table.load().await?;
-
-            let ctx = SessionContext::new();
-            ctx.state()
-                .runtime_env()
-                .register_object_store(url.scheme(), "", store);
-            let scan_plan = table.scan(&ctx.state(), None, &[], None).await?;
-            let plan = CoalescePartitionsExec::new(scan_plan);
-            let task_ctx = Arc::new(TaskContext::from(&ctx.state()));
-            let stream = plan.execute(0, task_ctx)?;
-            Ok((table, stream))
-        })
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use crate::operations::{collect_sendable_stream, DeltaOps};
-    use crate::writer::test_utils::{get_record_batch, TestResult};
-    use crate::DeltaTableBuilder;
-    use datafusion::assert_batches_sorted_eq;
-
-    #[tokio::test]
-    async fn test_load_local() -> TestResult {
-        let table = DeltaTableBuilder::from_uri("./tests/data/delta-0.8.0")
-            .load()
-            .await
-            .unwrap();
-
-        let (_table, stream) = DeltaOps(table).load().await?;
-        let data = collect_sendable_stream(stream).await?;
-
-        let expected = vec![
-            "+-------+",
-            "| value |",
-            "+-------+",
-            "| 0     |",
-            "| 1     |",
-            "| 2     |",
-            "| 4     |",
-            "+-------+",
-        ];
-
-        assert_batches_sorted_eq!(&expected, &data);
-        Ok(())
-    }
-
-    #[tokio::test]
-    async fn test_write_load() -> TestResult {
-        let batch = get_record_batch(None, false);
-        let table = DeltaOps::new_in_memory().write(vec![batch.clone()]).await?;
-
-        let (_table, stream) = DeltaOps(table).load().await?;
-        let data = collect_sendable_stream(stream).await?;
-
-        let expected = vec![
-            "+----+-------+------------+",
-            "| id | value | modified   |",
-            "+----+-------+------------+",
-            "| A  | 1     | 2021-02-02 |",
-            "| B  | 2     | 2021-02-02 |",
-            "| A  | 3     | 2021-02-02 |",
-            "| B  | 4     | 2021-02-01 |",
-            "| A  | 5     | 2021-02-01 |",
-            "| A  | 6     | 2021-02-01 |",
-            "| A  | 7     | 2021-02-01 |",
-            "| B  | 8     | 2021-02-01 |",
-            "| B  | 9     | 2021-02-01 |",
-            "| A  | 10    | 2021-02-01 |",
-            "| A  | 11    | 2021-02-01 |",
-            "+----+-------+------------+",
-        ];
-
-        assert_batches_sorted_eq!(&expected, &data);
-        assert_eq!(batch.schema(), data[0].schema());
-        Ok(())
+    pub fn get_storage(&mut self) -> Arc<DeltaObjectStore> {
+        if self.backend.is_none() {
+            self.backend = Some(self.new_storage())
+        }
+
+        self.backend.as_ref().unwrap().clone()
+    }
+
+    fn new_storage(&self) -> Arc<DeltaObjectStore> {
+        let config = self.config.clone();
+        let uri = config.get("URI").unwrap().to_string();
+        DeltaTableBuilder::from_uri(uri)
+            .with_storage_options(config)
+            .build_storage()
+            .unwrap()
+    }
+
+    //Create and set a new table from the provided schema
+    pub async fn create_table_from_schema(
+        &mut self,
+        schema: Schema,
+        partitions: &[&str],
+    ) -> DeltaTable {
+        let p = partitions
+            .iter()
+            .map(|s| s.to_string())
+            .collect::<Vec<String>>();
+        let table_meta = DeltaTableMetaData::new(
+            Some("delta-rs_test_table".to_owned()),
+            Some("Table created by delta-rs tests".to_owned()),
+            None,
+            schema.clone(),
+            p,
+            HashMap::new(),
+        );
+
+        let backend = self.new_storage();
+        let mut dt = DeltaTable::new(backend, DeltaTableConfig::default());
+        let mut commit_info = Map::<String, Value>::new();
+
+        let protocol = action::Protocol {
+            min_reader_version: 1,
+            min_writer_version: 2,
+        };
+
+        commit_info.insert(
+            "operation".to_string(),
+            serde_json::Value::String("CREATE TABLE".to_string()),
+        );
+        dt.create(
+            table_meta.clone(),
+            protocol.clone(),
+            Some(commit_info),
+            None,
+        )
+        .await
+        .unwrap();
+
+        dt
+    }
+}
+
+pub async fn setup_local_context() -> TestContext {
+    let tmp_dir = tempdir::TempDir::new("delta-rs_tests").unwrap();
+    let mut config = HashMap::new();
+    config.insert(
+        "URI".to_owned(),
+        tmp_dir.path().to_str().to_owned().unwrap().to_string(),
+    );
+
+    let localfs = LocalFS { tmp_dir };
+
+    TestContext {
+        storage_context: Some(Box::new(localfs)),
+        config,
+        ..TestContext::default()
     }
 }
+
+pub async fn add_file(
+    table: &mut DeltaTable,
+    path: &Path,
+    data: Bytes,
+    partition_values: &[(&str, Option<&str>)],
+    create_time: i64,
+    commit_to_log: bool,
+) {
+    let backend = table.object_store();
+    backend.put(path, data.clone()).await.unwrap();
+
+    if commit_to_log {
+        let mut part_values = HashMap::new();
+        for v in partition_values {
+            part_values.insert(v.0.to_string(), v.1.map(|v| v.to_string()));
+        }
+
+        let add = Add {
+            path: path.as_ref().into(),
+            size: data.len() as i64,
+            modification_time: create_time,
+            partition_values: part_values,
+            data_change: true,
+            ..Default::default()
+        };
+        let mut transaction = table.create_transaction(None);
+        transaction.add_action(action::Action::add(add));
+        transaction.commit(None, None).await.unwrap();
+    }
+}
+
+pub async fn remove_file(
+    table: &mut DeltaTable,
+    path: &str,
+    partition_values: &[(&str, Option<&str>)],
+    deletion_timestamp: i64,
+) {
+    let mut part_values = HashMap::new();
+    for v in partition_values {
+        part_values.insert(v.0.to_string(), v.1.map(|v| v.to_string()));
+    }
+
+    let remove = Remove {
+        path: path.into(),
+        deletion_timestamp: Some(deletion_timestamp),
+        partition_values: Some(part_values),
+        data_change: true,
+        ..Default::default()
+    };
+    let mut transaction = table.create_transaction(None);
+    transaction.add_action(action::Action::remove(remove));
+    transaction.commit(None, None).await.unwrap();
+}
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -98,24 +98,22 @@
         CreateBuilder::default().with_object_store(self.0.object_store())
     }
 
     /// Load data from a DeltaTable
     #[cfg(feature = "datafusion")]
     #[must_use]
     pub fn load(self) -> LoadBuilder {
-        LoadBuilder::default().with_object_store(self.0.object_store())
+        LoadBuilder::new(self.0.object_store(), self.0.state)
     }
 
     /// Write data to Delta table
     #[cfg(feature = "datafusion")]
     #[must_use]
     pub fn write(self, batches: impl IntoIterator<Item = RecordBatch>) -> WriteBuilder {
-        WriteBuilder::default()
-            .with_input_batches(batches)
-            .with_object_store(self.0.object_store())
+        WriteBuilder::new(self.0.object_store(), self.0.state).with_input_batches(batches)
     }
 
     /// Vacuum stale files from delta table
     #[must_use]
     pub fn vacuum(self) -> VacuumBuilder {
         VacuumBuilder::new(self.0.object_store(), self.0.state)
     }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/optimize.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/optimize.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 //! Optimize a Delta Table
 //!
 //! Perform bin-packing on a Delta Table which merges small files into a large
 //! file. Bin-packing reduces the number of API calls required for read
 //! operations.
 //!
-//! *WARNING:* Currently Optimize only supports append-only workflows. Use with
-//! other workflows may corrupt your table state.
+//! Optimize will fail if a concurrent write operation removes files from the
+//! table (such as in an overwrite). It will always succeed if concurrent writers
+//! are only appending.
 //!
 //! Optimize increments the table's version and creates remove actions for
 //! optimized files. Optimize does not delete files from storage. To delete
 //! files that were removed, call `vacuum` on [`DeltaTable`].
 //!
 //! See [`OptimizeBuilder`] for configuration.
 //!
@@ -169,15 +170,15 @@
                 .unwrap_or_else(|| WriterProperties::builder().build());
             let plan = create_merge_plan(
                 &this.snapshot,
                 this.filters,
                 this.target_size.to_owned(),
                 writer_properties,
             )?;
-            let metrics = plan.execute(this.store.clone()).await?;
+            let metrics = plan.execute(this.store.clone(), &this.snapshot).await?;
             let mut table = DeltaTable::new_with_state(this.store, this.snapshot);
             table.update().await?;
             Ok((table, metrics))
         })
     }
 }
 
@@ -266,15 +267,19 @@
     writer_properties: WriterProperties,
     /// Version of the table at beginning of optimization. Used for conflict resolution.
     read_table_version: DeltaDataTypeVersion,
 }
 
 impl MergePlan {
     /// Peform the operations outlined in the plan.
-    pub async fn execute(self, object_store: ObjectStoreRef) -> Result<Metrics, DeltaTableError> {
+    pub async fn execute(
+        self,
+        object_store: ObjectStoreRef,
+        snapshot: &DeltaTableState,
+    ) -> Result<Metrics, DeltaTableError> {
         let mut actions = vec![];
         let mut metrics = self.metrics;
 
         // TODO since we are now async in read and write, should we parallelize this?
         for (_partition_path, merge_partition) in self.operations.iter() {
             let partition_values = &merge_partition.partition_values;
             let bins = &merge_partition.bins;
@@ -364,17 +369,17 @@
             let maybe_map_metrics = serde_json::to_value(metrics.clone());
             if let Ok(map) = maybe_map_metrics {
                 metadata.insert("operationMetrics".to_owned(), map);
             }
 
             commit(
                 object_store.as_ref(),
-                self.read_table_version + 1,
                 &actions,
                 self.input_parameters.into(),
+                snapshot,
                 Some(metadata),
             )
             .await?;
         }
 
         Ok(metrics)
     }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/transaction.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/transaction/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 //! Delta transactions
-use crate::action::{Action, DeltaOperation};
-use crate::storage::DeltaObjectStore;
-use crate::{crate_version, DeltaDataTypeVersion, DeltaResult, DeltaTableError};
-
 use chrono::Utc;
+use conflict_checker::ConflictChecker;
 use object_store::path::Path;
 use object_store::{Error as ObjectStoreError, ObjectStore};
 use serde_json::{Map, Value};
 
+use crate::action::{Action, CommitInfo, DeltaOperation};
+use crate::storage::commit_uri_from_version;
+use crate::table_state::DeltaTableState;
+use crate::{crate_version, DeltaDataTypeVersion, DeltaResult, DeltaTableError};
+
+mod conflict_checker;
+#[cfg(feature = "datafusion")]
+mod state;
+#[cfg(test)]
+pub(crate) mod test_utils;
+
+use self::conflict_checker::{CommitConflictError, TransactionInfo, WinningCommitSummary};
+
 const DELTA_LOG_FOLDER: &str = "_delta_log";
 
+/// Error raised while commititng transaction
 #[derive(thiserror::Error, Debug)]
-pub(crate) enum TransactionError {
+pub enum TransactionError {
+    /// Version already exists
     #[error("Tried committing existing table version: {0}")]
     VersionAlreadyExists(DeltaDataTypeVersion),
 
     /// Error returned when reading the delta log object failed.
     #[error("Error serializing commit log to json: {json_err}")]
     SerializeLogJson {
         /// Commit log record JSON serialization error.
@@ -25,36 +37,37 @@
     /// Error returned when reading the delta log object failed.
     #[error("Log storage error: {}", .source)]
     ObjectStore {
         /// Storage error details when reading the delta log object failed.
         #[from]
         source: ObjectStoreError,
     },
+    /// Error returned when a commit conflict ocurred
+    #[error("Failed to commit transaction: {0}")]
+    CommitConflict(#[from] CommitConflictError),
+    /// Error returned when maximum number of commit trioals is exceeded
+    #[error("Failed to commit transaction: {0}")]
+    MaxCommitAttempts(i32),
 }
 
 impl From<TransactionError> for DeltaTableError {
     fn from(err: TransactionError) -> Self {
         match err {
             TransactionError::VersionAlreadyExists(version) => {
                 DeltaTableError::VersionAlreadyExists(version)
             }
             TransactionError::SerializeLogJson { json_err } => {
                 DeltaTableError::SerializeLogJson { json_err }
             }
             TransactionError::ObjectStore { source } => DeltaTableError::ObjectStore { source },
+            other => DeltaTableError::Transaction { source: other },
         }
     }
 }
 
-/// Return the uri of commit version.
-fn commit_uri_from_version(version: DeltaDataTypeVersion) -> Path {
-    let version = format!("{version:020}.json");
-    Path::from_iter([DELTA_LOG_FOLDER, &version])
-}
-
 // Convert actions to their json representation
 fn log_entry_from_actions<'a>(
     actions: impl IntoIterator<Item = &'a Action>,
 ) -> Result<String, TransactionError> {
     let mut jsons = Vec::<String>::new();
     for action in actions {
         let json = serde_json::to_string(action)
@@ -109,21 +122,21 @@
     let file_name = format!("_commit_{token}.json.tmp");
     let path = Path::from_iter([DELTA_LOG_FOLDER, &file_name]);
     storage.put(&path, log_entry).await?;
 
     Ok(path)
 }
 
-/// Tries to commit a prepared commit file. Returns [`DeltaTableError::VersionAlreadyExists`]
+/// Tries to commit a prepared commit file. Returns [DeltaTableError::VersionAlreadyExists]
 /// if the given `version` already exists. The caller should handle the retry logic itself.
 /// This is low-level transaction API. If user does not want to maintain the commit loop then
 /// the `DeltaTransaction.commit` is desired to be used as it handles `try_commit_transaction`
 /// with retry logic.
 async fn try_commit_transaction(
-    storage: &DeltaObjectStore,
+    storage: &dyn ObjectStore,
     tmp_commit: &Path,
     version: DeltaDataTypeVersion,
 ) -> Result<DeltaDataTypeVersion, TransactionError> {
     // move temporary commit file to delta log directory
     // rely on storage to fail if the file already exists -
     storage
         .rename_if_not_exists(tmp_commit, &commit_uri_from_version(version))
@@ -133,85 +146,98 @@
                 TransactionError::VersionAlreadyExists(version)
             }
             _ => TransactionError::from(err),
         })?;
     Ok(version)
 }
 
-pub(crate) async fn commit(
-    storage: &DeltaObjectStore,
-    version: DeltaDataTypeVersion,
+/// Commit a transaction, with up to 5 retries. This is low-level transaction API.
+///
+/// Will error early if the a concurrent transaction has already been committed
+/// and conflicts with this transaction.
+pub async fn commit(
+    storage: &dyn ObjectStore,
     actions: &Vec<Action>,
     operation: DeltaOperation,
+    read_snapshot: &DeltaTableState,
     app_metadata: Option<Map<String, Value>>,
 ) -> DeltaResult<DeltaDataTypeVersion> {
     let tmp_commit = prepare_commit(storage, &operation, actions, app_metadata).await?;
-    match try_commit_transaction(storage, &tmp_commit, version).await {
-        Ok(version) => Ok(version),
-        Err(TransactionError::VersionAlreadyExists(version)) => {
-            storage.delete(&tmp_commit).await?;
-            Err(DeltaTableError::VersionAlreadyExists(version))
+
+    let max_attempts = 5;
+    let mut attempt_number = 1;
+
+    while attempt_number <= max_attempts {
+        let version = read_snapshot.version() + attempt_number;
+        match try_commit_transaction(storage, &tmp_commit, version).await {
+            Ok(version) => return Ok(version),
+            Err(TransactionError::VersionAlreadyExists(version)) => {
+                let summary = WinningCommitSummary::try_new(storage, version - 1, version).await?;
+                let transaction_info = TransactionInfo::try_new(
+                    read_snapshot,
+                    operation.read_predicate(),
+                    actions,
+                    // TODO allow tainting whole table
+                    false,
+                )?;
+                let conflict_checker =
+                    ConflictChecker::new(transaction_info, summary, Some(&operation));
+                match conflict_checker.check_conflicts() {
+                    Ok(_) => {
+                        attempt_number += 1;
+                    }
+                    Err(err) => {
+                        storage.delete(&tmp_commit).await?;
+                        return Err(TransactionError::CommitConflict(err).into());
+                    }
+                };
+            }
+            Err(err) => {
+                storage.delete(&tmp_commit).await?;
+                return Err(err.into());
+            }
         }
-        Err(err) => Err(err.into()),
     }
+
+    Err(TransactionError::MaxCommitAttempts(max_attempts as i32).into())
 }
 
 #[cfg(all(test, feature = "parquet"))]
 mod tests {
+    use self::test_utils::init_table_actions;
     use super::*;
-    use crate::action::{DeltaOperation, Protocol, SaveMode};
-    use crate::storage::utils::flatten_list_stream;
-    use crate::writer::test_utils::get_delta_metadata;
-    use crate::{DeltaTable, DeltaTableBuilder};
+    use object_store::memory::InMemory;
 
     #[test]
-    fn test_commit_version() {
+    fn test_commit_uri_from_version() {
         let version = commit_uri_from_version(0);
         assert_eq!(version, Path::from("_delta_log/00000000000000000000.json"));
         let version = commit_uri_from_version(123);
         assert_eq!(version, Path::from("_delta_log/00000000000000000123.json"))
     }
 
+    #[test]
+    fn test_log_entry_from_actions() {
+        let actions = init_table_actions();
+        let entry = log_entry_from_actions(&actions).unwrap();
+        let lines: Vec<_> = entry.lines().collect();
+        // writes every action to a line
+        assert_eq!(actions.len(), lines.len())
+    }
+
     #[tokio::test]
-    async fn test_commits_writes_file() {
-        let metadata = get_delta_metadata(&[]);
-        let operation = DeltaOperation::Create {
-            mode: SaveMode::Append,
-            location: "memory://".into(),
-            protocol: Protocol {
-                min_reader_version: 1,
-                min_writer_version: 1,
-            },
-            metadata,
-        };
-
-        let commit_path = Path::from("_delta_log/00000000000000000000.json");
-        let storage = DeltaTableBuilder::from_uri("memory://")
-            .build_storage()
-            .unwrap();
-
-        // successfully write in clean location
-        commit(storage.as_ref(), 0, &vec![], operation.clone(), None)
-            .await
-            .unwrap();
-        let head = storage.head(&commit_path).await;
-        assert!(head.is_ok());
-        assert_eq!(head.as_ref().unwrap().location, commit_path);
-
-        // fail on overwriting
-        let failed_commit = commit(storage.as_ref(), 0, &vec![], operation, None).await;
-        assert!(failed_commit.is_err());
-        assert!(matches!(
-            failed_commit.unwrap_err(),
-            DeltaTableError::VersionAlreadyExists(_)
-        ));
-
-        // check we clean up after ourselves
-        let objects = flatten_list_stream(storage.as_ref(), None).await.unwrap();
-        assert_eq!(objects.len(), 1);
-
-        // table can be loaded
-        let mut table = DeltaTable::new(storage, Default::default());
-        table.load().await.unwrap();
-        assert_eq!(table.version(), 0)
+    async fn test_try_commit_transaction() {
+        let store = InMemory::new();
+        let tmp_path = Path::from("_delta_log/tmp");
+        let version_path = Path::from("_delta_log/00000000000000000000.json");
+        store.put(&tmp_path, bytes::Bytes::new()).await.unwrap();
+        store.put(&version_path, bytes::Bytes::new()).await.unwrap();
+
+        // fails if file version already exists
+        let res = try_commit_transaction(&store, &tmp_path, 0).await;
+        assert!(res.is_err());
+
+        // succeeds for next version
+        let res = try_commit_transaction(&store, &tmp_path, 1).await.unwrap();
+        assert_eq!(res, 1);
     }
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/vacuum.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/vacuum.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/write.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/write.rs`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,33 @@
 //!    will result in an exception.
 //!  - The partition columns, if present, are validated against the existing metadata. If not
 //!    present, then the partitioning of the table is respected.
 //!
 //! In combination with `Overwrite`, a `replaceWhere` option can be used to transactionally
 //! replace data that matches a predicate.
 
-// https://github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/delta/commands/WriteIntoDelta.scala
-
 use std::collections::HashMap;
 use std::sync::Arc;
 use std::time::{SystemTime, UNIX_EPOCH};
 
 use super::writer::{DeltaWriter, WriterConfig};
 use super::MAX_SUPPORTED_WRITER_VERSION;
 use super::{transaction::commit, CreateBuilder};
 use crate::action::{Action, Add, DeltaOperation, Remove, SaveMode};
-use crate::builder::DeltaTableBuilder;
 use crate::delta::{DeltaResult, DeltaTable, DeltaTableError};
 use crate::delta_datafusion::DeltaDataChecker;
 use crate::schema::Schema;
 use crate::storage::DeltaObjectStore;
+use crate::table_state::DeltaTableState;
 use crate::writer::record_batch::divide_by_partition_values;
 use crate::writer::utils::PartitionPath;
 
-use arrow::datatypes::{DataType, SchemaRef as ArrowSchemaRef};
-use arrow::record_batch::RecordBatch;
+use arrow_array::RecordBatch;
+use arrow_cast::{can_cast_types, cast};
+use arrow_schema::{Schema as ArrowSchema, SchemaRef as ArrowSchemaRef};
 use datafusion::execution::context::{SessionContext, SessionState, TaskContext};
 use datafusion::physical_plan::{memory::MemoryExec, ExecutionPlan};
 use futures::future::BoxFuture;
 use futures::StreamExt;
 
 #[derive(thiserror::Error, Debug)]
 enum WriteError {
@@ -72,69 +71,53 @@
         }
     }
 }
 
 /// Write data into a DeltaTable
 #[derive(Debug, Clone)]
 pub struct WriteBuilder {
+    /// A snapshot of the to-be-loaded table's state
+    snapshot: DeltaTableState,
+    /// Delta object store for handling data files
+    store: Arc<DeltaObjectStore>,
     /// The input plan
     input: Option<Arc<dyn ExecutionPlan>>,
     /// Datafusion session state relevant for executing the input plan
     state: Option<SessionState>,
-    /// Location where the table is stored
-    location: Option<String>,
     /// SaveMode defines how to treat data already written to table location
     mode: SaveMode,
     /// Column names for table partitioning
     partition_columns: Option<Vec<String>>,
     /// When using `Overwrite` mode, replace data that matches a predicate
     predicate: Option<String>,
     /// Size above which we will write a buffered parquet file to disk.
     target_file_size: Option<usize>,
     /// Number of records to be written in single batch to underlying writer
     write_batch_size: Option<usize>,
-    /// An object store to be used as backend for delta table
-    object_store: Option<Arc<DeltaObjectStore>>,
-    /// Storage options used to create a new storage backend
-    storage_options: Option<HashMap<String, String>>,
     /// RecordBatches to be written into the table
     batches: Option<Vec<RecordBatch>>,
 }
 
-impl Default for WriteBuilder {
-    fn default() -> Self {
-        Self::new()
-    }
-}
-
 impl WriteBuilder {
     /// Create a new [`WriteBuilder`]
-    pub fn new() -> Self {
+    pub fn new(store: Arc<DeltaObjectStore>, snapshot: DeltaTableState) -> Self {
         Self {
+            snapshot,
+            store,
             input: None,
             state: None,
-            location: None,
             mode: SaveMode::Append,
             partition_columns: None,
             predicate: None,
-            storage_options: None,
             target_file_size: None,
             write_batch_size: None,
-            object_store: None,
             batches: None,
         }
     }
 
-    /// Specify the path to the location where table data is stored,
-    /// which could be a path on distributed storage.
-    pub fn with_location(mut self, location: impl Into<String>) -> Self {
-        self.location = Some(location.into());
-        self
-    }
-
     /// Specify the behavior when a table exists at location
     pub fn with_save_mode(mut self, save_mode: SaveMode) -> Self {
         self.mode = save_mode;
         self
     }
 
     /// When using `Overwrite` mode, replace data that matches a predicate
@@ -167,159 +150,128 @@
 
     /// Execution plan that produces the data to be written to the delta table
     pub fn with_input_batches(mut self, batches: impl IntoIterator<Item = RecordBatch>) -> Self {
         self.batches = Some(batches.into_iter().collect());
         self
     }
 
-    /// Set options used to initialize storage backend
-    ///
-    /// Options may be passed in the HashMap or set as environment variables.
-    pub fn with_storage_options(mut self, storage_options: HashMap<String, String>) -> Self {
-        self.storage_options = Some(storage_options);
-        self
-    }
-
-    /// Provide a [`DeltaObjectStore`] instance, that points at table location
-    pub fn with_object_store(mut self, object_store: Arc<DeltaObjectStore>) -> Self {
-        self.object_store = Some(object_store);
-        self
-    }
-
     /// Specify the target file size for data files written to the delta table.
     pub fn with_target_file_size(mut self, target_file_size: usize) -> Self {
         self.target_file_size = Some(target_file_size);
         self
     }
 
     /// Specify the target batch size for row groups written to parquet files.
     pub fn with_write_batch_size(mut self, write_batch_size: usize) -> Self {
         self.write_batch_size = Some(write_batch_size);
         self
     }
+
+    async fn check_preconditions(&self) -> DeltaResult<Vec<Action>> {
+        match self.store.is_delta_table_location().await? {
+            true => {
+                let min_writer = self.snapshot.min_writer_version();
+                if min_writer > MAX_SUPPORTED_WRITER_VERSION {
+                    Err(WriteError::UnsupportedWriterVersion(min_writer).into())
+                } else {
+                    match self.mode {
+                        SaveMode::ErrorIfExists => {
+                            Err(WriteError::AlreadyExists(self.store.root_uri()).into())
+                        }
+                        _ => Ok(vec![]),
+                    }
+                }
+            }
+            false => {
+                let schema: Schema = if let Some(plan) = &self.input {
+                    Ok(plan.schema().try_into()?)
+                } else if let Some(batches) = &self.batches {
+                    if batches.is_empty() {
+                        return Err(WriteError::MissingData.into());
+                    }
+                    Ok(batches[0].schema().try_into()?)
+                } else {
+                    Err(WriteError::MissingData)
+                }?;
+                let mut builder = CreateBuilder::new()
+                    .with_object_store(self.store.clone())
+                    .with_columns(schema.get_fields().clone());
+                if let Some(partition_columns) = self.partition_columns.as_ref() {
+                    builder = builder.with_partition_columns(partition_columns.clone())
+                }
+                let (_, actions, _) = builder.into_table_and_actions()?;
+                Ok(actions)
+            }
+        }
+    }
 }
 
 impl std::future::IntoFuture for WriteBuilder {
     type Output = DeltaResult<DeltaTable>;
     type IntoFuture = BoxFuture<'static, Self::Output>;
 
     fn into_future(self) -> Self::IntoFuture {
-        let this = self;
-
-        fn schema_to_vec_name_type(schema: ArrowSchemaRef) -> Vec<(String, DataType)> {
-            schema
-                .fields()
-                .iter()
-                .map(|f| (f.name().to_owned(), f.data_type().clone()))
-                .collect::<Vec<_>>()
-        }
-
-        fn schema_eq(l: ArrowSchemaRef, r: ArrowSchemaRef) -> bool {
-            schema_to_vec_name_type(l) == schema_to_vec_name_type(r)
-        }
+        let mut this = self;
 
         Box::pin(async move {
-            let object_store = if let Some(store) = this.object_store {
-                Ok(store)
-            } else {
-                DeltaTableBuilder::from_uri(this.location.unwrap())
-                    .with_storage_options(this.storage_options.unwrap_or_default())
-                    .build_storage()
-            }?;
+            // Create table actions to initialize table in case it does not yet exist and should be created
+            let mut actions = this.check_preconditions().await?;
 
-            // TODO we can find a more optimized config. Of course we want to pass in the state anyhow..
-            let mut table = DeltaTable::new(object_store.clone(), Default::default());
-            let mut actions = match table.load().await {
-                Err(DeltaTableError::NotATable(_)) => {
-                    let schema: Schema = if let Some(plan) = &this.input {
-                        Ok(plan.schema().try_into()?)
-                    } else if let Some(batches) = &this.batches {
-                        if batches.is_empty() {
-                            return Err(WriteError::MissingData.into());
-                        }
-                        Ok(batches[0].schema().try_into()?)
-                    } else {
-                        Err(WriteError::MissingData)
-                    }?;
-                    let mut builder = CreateBuilder::new()
-                        .with_object_store(table.object_store())
-                        .with_columns(schema.get_fields().clone());
-                    if let Some(partition_columns) = this.partition_columns.as_ref() {
-                        builder = builder.with_partition_columns(partition_columns.clone())
-                    }
-                    let (_, actions, _) = builder.into_table_and_actions()?;
-                    Ok(actions)
-                }
-                Ok(_) => {
-                    if table.get_min_writer_version() > MAX_SUPPORTED_WRITER_VERSION {
-                        Err(
-                            WriteError::UnsupportedWriterVersion(table.get_min_writer_version())
-                                .into(),
-                        )
-                    } else {
-                        match this.mode {
-                            SaveMode::ErrorIfExists => {
-                                Err(WriteError::AlreadyExists(table.table_uri()).into())
-                            }
-                            _ => Ok(vec![]),
-                        }
-                    }
-                }
-                Err(err) => Err(err),
-            }?;
+            let active_partitions = this
+                .snapshot
+                .current_metadata()
+                .map(|meta| meta.partition_columns.clone());
 
             // validate partition columns
-            let partition_columns = if let Ok(meta) = table.get_metadata() {
+            let partition_columns = if let Some(active_part) = active_partitions {
                 if let Some(ref partition_columns) = this.partition_columns {
-                    if &meta.partition_columns != partition_columns {
+                    if &active_part != partition_columns {
                         Err(WriteError::PartitionColumnMismatch {
-                            expected: table.get_metadata()?.partition_columns.clone(),
+                            expected: active_part,
                             got: partition_columns.to_vec(),
                         })
                     } else {
                         Ok(partition_columns.clone())
                     }
                 } else {
-                    Ok(meta.partition_columns.clone())
+                    Ok(active_part)
                 }
             } else {
                 Ok(this.partition_columns.unwrap_or_default())
             }?;
 
             let plan = if let Some(plan) = this.input {
                 Ok(plan)
             } else if let Some(batches) = this.batches {
                 if batches.is_empty() {
                     Err(WriteError::MissingData)
                 } else {
                     let schema = batches[0].schema();
-
-                    if let Ok(meta) = table.get_metadata() {
-                        // NOTE the schema generated from the delta schema will have the delta field metadata included,
-                        // so we need to compare the field names and datatypes instead.
-                        // TODO update comparison logic, once we have column mappings supported.
-                        let curr_schema: ArrowSchemaRef = Arc::new((&meta.schema).try_into()?);
-
-                        if !schema_eq(curr_schema, schema.clone()) {
-                            return Err(DeltaTableError::Generic(
-                                "Updating table schema not yet implemented".to_string(),
-                            ));
-                        }
+                    let table_schema = this
+                        .snapshot
+                        .physical_arrow_schema(this.store.clone())
+                        .await
+                        .or_else(|_| this.snapshot.arrow_schema())
+                        .unwrap_or(schema.clone());
+
+                    if !can_cast_batch(schema.as_ref(), table_schema.as_ref()) {
+                        return Err(DeltaTableError::Generic(
+                            "Updating table schema not yet implemented".to_string(),
+                        ));
                     };
 
                     let data = if !partition_columns.is_empty() {
                         // TODO partitioning should probably happen in its own plan ...
                         let mut partitions: HashMap<String, Vec<RecordBatch>> = HashMap::new();
                         for batch in batches {
                             let divided = divide_by_partition_values(
                                 schema.clone(),
                                 partition_columns.clone(),
                                 &batch,
-                            )
-                            .unwrap();
+                            )?;
                             for part in divided {
                                 let key = PartitionPath::from_hashmap(
                                     &partition_columns,
                                     &part.partition_values,
                                 )
                                 .map_err(DeltaTableError::from)?
                                 .into();
@@ -341,17 +293,18 @@
                     Ok(Arc::new(MemoryExec::try_new(&data, schema, None)?)
                         as Arc<dyn ExecutionPlan>)
                 }
             } else {
                 Err(WriteError::MissingData)
             }?;
 
-            let invariants = table
-                .get_metadata()
-                .and_then(|meta| meta.schema.get_invariants())
+            let invariants = this
+                .snapshot
+                .current_metadata()
+                .and_then(|meta| meta.schema.get_invariants().ok())
                 .unwrap_or_default();
             let checker = DeltaDataChecker::new(invariants);
 
             // Write data to disk
             let mut tasks = vec![];
             for i in 0..plan.output_partitioning().partition_count() {
                 let inner_plan = plan.clone();
@@ -364,23 +317,25 @@
                 let config = WriterConfig::new(
                     inner_plan.schema(),
                     partition_columns.clone(),
                     None,
                     this.target_file_size,
                     this.write_batch_size,
                 );
-                let mut writer = DeltaWriter::new(object_store.clone(), config);
+                let mut writer = DeltaWriter::new(this.store.clone(), config);
                 let checker_stream = checker.clone();
+                let schema = inner_plan.schema().clone();
                 let mut stream = inner_plan.execute(i, task_ctx)?;
                 let handle: tokio::task::JoinHandle<DeltaResult<Vec<Add>>> =
                     tokio::task::spawn(async move {
                         while let Some(maybe_batch) = stream.next().await {
                             let batch = maybe_batch?;
                             checker_stream.check_batch(&batch).await?;
-                            writer.write(&batch).await?;
+                            let arr = cast_record_batch(&batch, schema.clone())?;
+                            writer.write(&arr).await?;
                         }
                         writer.close().await
                     });
 
                 tasks.push(handle);
             }
 
@@ -392,14 +347,15 @@
                 .map_err(|err| WriteError::WriteTask { source: err })?
                 .into_iter()
                 .collect::<Result<Vec<_>, _>>()?
                 .concat()
                 .into_iter()
                 .map(Action::add)
                 .collect::<Vec<_>>();
+
             actions.extend(add_actions);
 
             // Collect remove actions if we are overwriting the table
             if matches!(this.mode, SaveMode::Overwrite) {
                 // This should never error, since now() will always be larger than UNIX_EPOCH
                 let deletion_timestamp = SystemTime::now()
                     .duration_since(UNIX_EPOCH)
@@ -420,52 +376,88 @@
                 };
 
                 match this.predicate {
                     Some(_pred) => {
                         todo!("Overwriting data based on predicate is not yet implemented")
                     }
                     _ => {
-                        let remove_actions = table
-                            .get_state()
+                        let remove_actions = this
+                            .snapshot
                             .files()
                             .iter()
                             .map(to_remove_action)
                             .collect::<Vec<_>>();
                         actions.extend(remove_actions);
                     }
                 }
             };
 
-            // Finally, commit ...
-            let operation = DeltaOperation::Write {
-                mode: this.mode,
-                partition_by: if !partition_columns.is_empty() {
-                    Some(partition_columns)
-                } else {
-                    None
-                },
-                predicate: this.predicate,
-            };
-            let _version = commit(
-                &table.storage,
-                table.version() + 1,
+            let version = commit(
+                this.store.as_ref(),
                 &actions,
-                operation,
+                DeltaOperation::Write {
+                    mode: this.mode,
+                    partition_by: if !partition_columns.is_empty() {
+                        Some(partition_columns)
+                    } else {
+                        None
+                    },
+                    predicate: this.predicate,
+                },
+                &this.snapshot,
+                // TODO pass through metadata
                 None,
             )
             .await?;
-            table.update().await?;
+
+            // TODO we do not have the table config available, but since we are merging only our newly
+            // created actions, it may be safe to assume, that we want to include all actions.
+            // then again, having only some tombstones may be misleading.
+            this.snapshot
+                .merge(DeltaTableState::from_actions(actions, version)?, true, true);
 
             // TODO should we build checkpoints based on config?
 
-            Ok(table)
+            Ok(DeltaTable::new_with_state(this.store, this.snapshot))
         })
     }
 }
 
+fn can_cast_batch(from_schema: &ArrowSchema, to_schema: &ArrowSchema) -> bool {
+    if from_schema.fields.len() != to_schema.fields.len() {
+        return false;
+    }
+    from_schema.all_fields().iter().all(|f| {
+        if let Ok(target_field) = to_schema.field_with_name(f.name()) {
+            can_cast_types(f.data_type(), target_field.data_type())
+        } else {
+            false
+        }
+    })
+}
+
+fn cast_record_batch(
+    batch: &RecordBatch,
+    target_schema: ArrowSchemaRef,
+) -> DeltaResult<RecordBatch> {
+    let columns = target_schema
+        .all_fields()
+        .iter()
+        .map(|f| {
+            let col = batch.column_by_name(f.name()).unwrap();
+            if !col.data_type().equals_datatype(f.data_type()) {
+                cast(col, f.data_type())
+            } else {
+                Ok(col.clone())
+            }
+        })
+        .collect::<Result<Vec<_>, _>>()?;
+    Ok(RecordBatch::try_new(target_schema, columns)?)
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::operations::DeltaOps;
     use crate::writer::test_utils::{get_delta_schema, get_record_batch};
     use serde_json::json;
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/operations/writer.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/operations/writer.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/partitions.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/partitions.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/schema.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/schema.rs`

 * *Files 4% similar despite different names*

```diff
@@ -296,14 +296,15 @@
     ///  * byte: i8
     ///  * float: f32
     ///  * double: f64
     ///  * boolean: bool
     ///  * binary: a sequence of binary data
     ///  * date: A calendar date, represented as a year-month-day triple without a timezone
     ///  * timestamp: Microsecond precision timestamp without a timezone
+    ///  * decimal: Signed decimal number with fixed precision (maximum number of digits) and scale (number of digits on right side of dot), where the precision and scale can be up to 38
     primitive(String),
     /// Variant representing a struct.
     r#struct(SchemaTypeStruct),
     /// Variant representing an array.
     array(SchemaTypeArray),
     /// Variant representing a map.
     map(SchemaTypeMap),
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/storage/config.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/storage/config.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 //! Configuration handling for defining Storage backends for DeltaTables.
 use super::file::FileStorageBackend;
 use super::utils::str_is_truthy;
 use crate::{DeltaResult, DeltaTableError};
 use object_store::memory::InMemory;
 use object_store::path::Path;
-use object_store::prefix::PrefixObjectStore;
-use object_store::DynObjectStore;
+use object_store::prefix::PrefixStore;
+use object_store::{DynObjectStore, ObjectStore};
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::sync::Arc;
 use url::Url;
 
 #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
 use super::s3::{S3StorageBackend, S3StorageOptions};
+#[cfg(feature = "hdfs")]
+use datafusion_objectstore_hdfs::object_store::hdfs::HadoopFileSystem;
 #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
 use object_store::aws::{AmazonS3Builder, AmazonS3ConfigKey};
 #[cfg(feature = "azure")]
-use object_store::azure::{AzureConfigKey, MicrosoftAzure, MicrosoftAzureBuilder};
+use object_store::azure::{AzureConfigKey, MicrosoftAzureBuilder};
 #[cfg(feature = "gcs")]
-use object_store::gcp::{GoogleCloudStorage, GoogleCloudStorageBuilder, GoogleConfigKey};
+use object_store::gcp::{GoogleCloudStorageBuilder, GoogleConfigKey};
 #[cfg(any(
     feature = "s3",
     feature = "s3-native-tls",
     feature = "gcs",
     feature = "azure"
 ))]
 use std::str::FromStr;
 
 /// Options used for configuring backend storage
-#[derive(Clone, Debug, Serialize, Deserialize)]
+#[derive(Clone, Debug, Serialize, Deserialize, Default)]
 pub struct StorageOptions(pub HashMap<String, String>);
 
 impl StorageOptions {
     /// Create a new instance of [`StorageOptions`]
     pub fn new(options: HashMap<String, String>) -> Self {
         let mut options = options;
         if let Ok(value) = std::env::var("AZURE_STORAGE_ALLOW_HTTP") {
@@ -92,141 +94,196 @@
 }
 
 impl From<HashMap<String, String>> for StorageOptions {
     fn from(value: HashMap<String, String>) -> Self {
         Self::new(value)
     }
 }
+pub(crate) fn configure_store(
+    url: &Url,
+    options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    match url.scheme() {
+        "file" => try_configure_local(
+            url.to_file_path()
+                .map_err(|_| DeltaTableError::InvalidTableLocation(url.to_string()))?
+                .to_str()
+                .ok_or_else(|| DeltaTableError::InvalidTableLocation(url.to_string()))?,
+        ),
+        "memory" => try_configure_memory(url),
+        "az" | "abfs" | "abfss" | "azure" | "wasb" | "adl" => try_configure_azure(url, options),
+        "s3" | "s3a" => try_configure_s3(url, options),
+        "gs" => try_configure_gcs(url, options),
+        "hdfs" => try_configure_hdfs(url, options),
+        "https" => {
+            let host = url.host_str().unwrap_or_default();
+            if host.contains("amazonaws.com") {
+                try_configure_s3(url, options)
+            } else if host.contains("dfs.core.windows.net")
+                || host.contains("blob.core.windows.net")
+            {
+                try_configure_azure(url, options)
+            } else {
+                Err(DeltaTableError::Generic(format!(
+                    "unsupported url: {}",
+                    url.as_str()
+                )))
+            }
+        }
+        _ => Err(DeltaTableError::Generic(format!(
+            "unsupported url: {}",
+            url.as_str()
+        ))),
+    }
+}
 
-pub(crate) enum ObjectStoreImpl {
-    Local(FileStorageBackend),
-    InMemory(InMemory),
-    #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
-    S3(S3StorageBackend),
-    #[cfg(feature = "gcs")]
-    Google(GoogleCloudStorage),
-    #[cfg(feature = "azure")]
-    Azure(MicrosoftAzure),
+fn try_configure_local<P: AsRef<str>>(path: P) -> DeltaResult<Arc<DynObjectStore>> {
+    Ok(Arc::new(FileStorageBackend::try_new(path.as_ref())?))
 }
 
-impl ObjectStoreImpl {
-    pub(crate) fn into_prefix(self, prefix: Path) -> Arc<DynObjectStore> {
-        match self {
-            ObjectStoreImpl::Local(store) => Arc::new(PrefixObjectStore::new(store, prefix)),
-            ObjectStoreImpl::InMemory(store) => Arc::new(PrefixObjectStore::new(store, prefix)),
-            #[cfg(feature = "azure")]
-            ObjectStoreImpl::Azure(store) => Arc::new(PrefixObjectStore::new(store, prefix)),
-            #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
-            ObjectStoreImpl::S3(store) => Arc::new(PrefixObjectStore::new(store, prefix)),
-            #[cfg(feature = "gcs")]
-            ObjectStoreImpl::Google(store) => Arc::new(PrefixObjectStore::new(store, prefix)),
-        }
-    }
+fn try_configure_memory(storage_url: &Url) -> DeltaResult<Arc<DynObjectStore>> {
+    url_prefix_handler(InMemory::new(), storage_url)
+}
 
-    pub(crate) fn into_store(self) -> Arc<DynObjectStore> {
-        match self {
-            ObjectStoreImpl::Local(store) => Arc::new(store),
-            ObjectStoreImpl::InMemory(store) => Arc::new(store),
-            #[cfg(feature = "azure")]
-            ObjectStoreImpl::Azure(store) => Arc::new(store),
-            #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
-            ObjectStoreImpl::S3(store) => Arc::new(store),
-            #[cfg(feature = "gcs")]
-            ObjectStoreImpl::Google(store) => Arc::new(store),
-        }
-    }
+#[cfg(feature = "gcs")]
+fn try_configure_gcs(
+    storage_url: &Url,
+    options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    let store = GoogleCloudStorageBuilder::from_env()
+        .with_url(storage_url.as_ref())
+        .try_with_options(&options.as_gcs_options())?
+        .build()?;
+    url_prefix_handler(store, storage_url)
 }
 
-pub(crate) enum ObjectStoreKind {
-    Local,
-    InMemory,
-    S3,
-    Google,
-    Azure,
-}
-
-impl ObjectStoreKind {
-    pub fn parse_url(url: &Url) -> DeltaResult<Self> {
-        match url.scheme() {
-            "file" => Ok(ObjectStoreKind::Local),
-            "memory" => Ok(ObjectStoreKind::InMemory),
-            "az" | "abfs" | "abfss" | "azure" | "wasb" | "adl" => Ok(ObjectStoreKind::Azure),
-            "s3" | "s3a" => Ok(ObjectStoreKind::S3),
-            "gs" => Ok(ObjectStoreKind::Google),
-            "https" => {
-                let host = url.host_str().unwrap_or_default();
-                if host.contains("amazonaws.com") {
-                    Ok(ObjectStoreKind::S3)
-                } else if host.contains("dfs.core.windows.net")
-                    || host.contains("blob.core.windows.net")
-                {
-                    Ok(ObjectStoreKind::Azure)
-                } else {
-                    Err(DeltaTableError::Generic(format!(
-                        "unsupported url: {}",
-                        url.as_str()
-                    )))
-                }
-            }
-            _ => Err(DeltaTableError::Generic(format!(
-                "unsupported url: {}",
-                url.as_str()
-            ))),
-        }
+#[cfg(not(feature = "gcs"))]
+fn try_configure_gcs(
+    storage_url: &Url,
+    _options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    Err(DeltaTableError::MissingFeature {
+        feature: "gcs",
+        url: storage_url.as_ref().into(),
+    })
+}
+
+#[cfg(feature = "azure")]
+fn try_configure_azure(
+    storage_url: &Url,
+    options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    let store = MicrosoftAzureBuilder::from_env()
+        .with_url(storage_url.as_ref())
+        .try_with_options(&options.as_azure_options())?
+        .with_allow_http(options.allow_http())
+        .build()?;
+    url_prefix_handler(store, storage_url)
+}
+
+#[cfg(not(feature = "azure"))]
+fn try_configure_azure(
+    storage_url: &Url,
+    _options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    Err(DeltaTableError::MissingFeature {
+        feature: "azure",
+        url: storage_url.as_ref().into(),
+    })
+}
+
+#[cfg(any(feature = "s3", feature = "s3-native-tls"))]
+fn try_configure_s3(
+    storage_url: &Url,
+    options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    let amazon_s3 = AmazonS3Builder::from_env()
+        .with_url(storage_url.as_ref())
+        .try_with_options(&options.as_s3_options())?
+        .with_allow_http(options.allow_http())
+        .build()?;
+    let store =
+        S3StorageBackend::try_new(Arc::new(amazon_s3), S3StorageOptions::from_map(&options.0))?;
+    url_prefix_handler(store, storage_url)
+}
+
+#[cfg(not(any(feature = "s3", feature = "s3-native-tls")))]
+fn try_configure_s3(
+    storage_url: &Url,
+    _options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    Err(DeltaTableError::MissingFeature {
+        feature: "s3",
+        url: storage_url.as_ref().into(),
+    })
+}
+
+#[cfg(feature = "hdfs")]
+fn try_configure_hdfs(
+    storage_url: &Url,
+    _options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    let store = HadoopFileSystem::new(storage_url.as_ref()).ok_or_else(|| {
+        DeltaTableError::Generic(format!(
+            "failed to create HadoopFileSystem for {}",
+            storage_url.as_ref()
+        ))
+    })?;
+    url_prefix_handler(store, storage_url)
+}
+
+#[cfg(not(feature = "hdfs"))]
+fn try_configure_hdfs(
+    storage_url: &Url,
+    _options: &StorageOptions,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    Err(DeltaTableError::MissingFeature {
+        feature: "hdfs",
+        url: storage_url.as_ref().into(),
+    })
+}
+
+fn url_prefix_handler<T: ObjectStore>(
+    store: T,
+    storage_url: &Url,
+) -> DeltaResult<Arc<DynObjectStore>> {
+    let prefix = Path::parse(storage_url.path())?;
+    if prefix != Path::from("/") {
+        Ok(Arc::new(PrefixStore::new(store, prefix)))
+    } else {
+        Ok(Arc::new(store))
     }
+}
 
-    pub fn into_impl(
-        self,
-        storage_url: impl AsRef<str>,
-        options: impl Into<StorageOptions>,
-    ) -> DeltaResult<ObjectStoreImpl> {
-        let _options = options.into();
-        match self {
-            ObjectStoreKind::Local => Ok(ObjectStoreImpl::Local(FileStorageBackend::new())),
-            ObjectStoreKind::InMemory => Ok(ObjectStoreImpl::InMemory(InMemory::new())),
-            #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
-            ObjectStoreKind::S3 => {
-                let store = AmazonS3Builder::from_env()
-                    .with_url(storage_url.as_ref())
-                    .try_with_options(&_options.as_s3_options())?
-                    .with_allow_http(_options.allow_http())
-                    .build()?;
-                Ok(ObjectStoreImpl::S3(S3StorageBackend::try_new(
-                    Arc::new(store),
-                    S3StorageOptions::from_map(&_options.0),
-                )?))
-            }
-            #[cfg(not(any(feature = "s3", feature = "s3-native-tls")))]
-            ObjectStoreKind::S3 => Err(DeltaTableError::MissingFeature {
-                feature: "s3",
-                url: storage_url.as_ref().into(),
-            }),
-            #[cfg(feature = "azure")]
-            ObjectStoreKind::Azure => {
-                let store = MicrosoftAzureBuilder::from_env()
-                    .with_url(storage_url.as_ref())
-                    .try_with_options(&_options.as_azure_options())?
-                    .with_allow_http(_options.allow_http())
-                    .build()?;
-                Ok(ObjectStoreImpl::Azure(store))
-            }
-            #[cfg(not(feature = "azure"))]
-            ObjectStoreKind::Azure => Err(DeltaTableError::MissingFeature {
-                feature: "azure",
-                url: storage_url.as_ref().into(),
-            }),
-            #[cfg(feature = "gcs")]
-            ObjectStoreKind::Google => {
-                let store = GoogleCloudStorageBuilder::from_env()
-                    .with_url(storage_url.as_ref())
-                    .try_with_options(&_options.as_gcs_options())?
-                    .build()?;
-                Ok(ObjectStoreImpl::Google(store))
-            }
-            #[cfg(not(feature = "gcs"))]
-            ObjectStoreKind::Google => Err(DeltaTableError::MissingFeature {
-                feature: "gcs",
-                url: storage_url.as_ref().into(),
-            }),
-        }
+#[cfg(test)]
+mod test {
+    use crate::ensure_table_uri;
+
+    use super::*;
+
+    #[tokio::test]
+    async fn test_configure_store_local() -> Result<(), Box<dyn std::error::Error + 'static>> {
+        let temp_dir = tempfile::tempdir().unwrap();
+        let temp_dir_path = temp_dir.path();
+        let path = temp_dir_path.join("test space 😁");
+
+        let table_uri = ensure_table_uri(path.as_os_str().to_str().unwrap()).unwrap();
+
+        let store = configure_store(&table_uri, &StorageOptions::default()).unwrap();
+
+        let contents = b"test";
+        let key = "test.txt";
+        let file_path = path.join(key);
+        std::fs::write(&file_path, contents).unwrap();
+
+        let res = store
+            .get(&object_store::path::Path::from(key))
+            .await
+            .unwrap()
+            .bytes()
+            .await
+            .unwrap();
+        assert_eq!(res.as_ref(), contents);
+
+        Ok(())
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/storage/file.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/storage/file.rs`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     local::LocalFileSystem, path::Path as ObjectStorePath, Error as ObjectStoreError, GetResult,
     ListResult, MultipartId, ObjectMeta as ObjStoreObjectMeta, ObjectStore,
     Result as ObjectStoreResult,
 };
 use std::ops::Range;
 use std::sync::Arc;
 use tokio::io::AsyncWrite;
+use url::Url;
 
 const STORE_NAME: &str = "DeltaLocalObjectStore";
 
 /// Error raised by storage lock client
 #[derive(thiserror::Error, Debug)]
 #[allow(dead_code)]
 pub(self) enum LocalFileSystemError {
@@ -89,47 +90,63 @@
 ///   *  ext4 requires >= Linux 3.15
 ///   *  btrfs, shmem, and cif requires >= Linux 3.17
 ///   *  xfs requires >= Linux 4.0
 ///   *  ext2, minix, reiserfs, jfs, vfat, and bpf requires >= Linux 4.9
 /// * Darwin is supported but not fully tested.
 /// Patches welcome.
 /// * Support for other platforms are not implemented at the moment.
-#[derive(Debug, Default)]
+#[derive(Debug)]
 pub struct FileStorageBackend {
     inner: Arc<LocalFileSystem>,
+    root_url: Arc<Url>,
 }
 
 impl FileStorageBackend {
     /// Creates a new FileStorageBackend.
-    pub fn new() -> Self {
-        Self {
-            inner: Arc::new(LocalFileSystem::default()),
-        }
+    pub fn try_new(path: impl AsRef<std::path::Path>) -> ObjectStoreResult<Self> {
+        Ok(Self {
+            root_url: Arc::new(Self::path_to_root_url(path.as_ref())?),
+            inner: Arc::new(LocalFileSystem::new_with_prefix(path)?),
+        })
+    }
+
+    fn path_to_root_url(path: &std::path::Path) -> ObjectStoreResult<Url> {
+        let root_path =
+            std::fs::canonicalize(path).map_err(|e| object_store::Error::InvalidPath {
+                source: object_store::path::Error::Canonicalize {
+                    path: path.into(),
+                    source: e,
+                },
+            })?;
+
+        Url::from_file_path(root_path).map_err(|_| object_store::Error::InvalidPath {
+            source: object_store::path::Error::InvalidPath { path: path.into() },
+        })
+    }
+
+    /// Return an absolute filesystem path of the given location
+    fn path_to_filesystem(&self, location: &ObjectStorePath) -> String {
+        let mut url = self.root_url.as_ref().clone();
+        url.path_segments_mut()
+            .expect("url path")
+            // technically not necessary as Path ignores empty segments
+            // but avoids creating paths with "//" which look odd in error messages.
+            .pop_if_empty()
+            .extend(location.parts());
+
+        url.to_file_path().unwrap().to_str().unwrap().to_owned()
     }
 }
 
 impl std::fmt::Display for FileStorageBackend {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "FileStorageBackend")
     }
 }
 
-/// Return an absolute filesystem path of the given location
-fn path_to_filesystem(location: &ObjectStorePath) -> String {
-    let mut url = url::Url::parse("file:///").unwrap();
-    url.path_segments_mut()
-        .expect("url path")
-        // technically not necessary as Path ignores empty segments
-        // but avoids creating paths with "//" which look odd in error messages.
-        .pop_if_empty()
-        .extend(location.parts());
-
-    url.to_file_path().unwrap().to_str().unwrap().to_owned()
-}
-
 #[async_trait::async_trait]
 impl ObjectStore for FileStorageBackend {
     async fn put(&self, location: &ObjectStorePath, bytes: Bytes) -> ObjectStoreResult<()> {
         self.inner.put(location, bytes).await
     }
 
     async fn get(&self, location: &ObjectStorePath) -> ObjectStoreResult<GetResult> {
@@ -179,16 +196,16 @@
     }
 
     async fn rename_if_not_exists(
         &self,
         from: &ObjectStorePath,
         to: &ObjectStorePath,
     ) -> ObjectStoreResult<()> {
-        let path_from = path_to_filesystem(from);
-        let path_to = path_to_filesystem(to);
+        let path_from = self.path_to_filesystem(from);
+        let path_to = self.path_to_filesystem(to);
         Ok(rename_noreplace(path_from.as_ref(), path_to.as_ref()).await?)
     }
 
     async fn put_multipart(
         &self,
         location: &ObjectStorePath,
     ) -> ObjectStoreResult<(MultipartId, Box<dyn AsyncWrite + Unpin + Send>)> {
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/storage/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/storage/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //! Object storage backend abstraction layer for Delta Table transaction logs and data
 
 pub mod config;
 pub mod file;
 pub mod utils;
 
-use self::config::{ObjectStoreKind, StorageOptions};
+use self::config::StorageOptions;
 use crate::{DeltaDataTypeVersion, DeltaResult};
 
 use bytes::Bytes;
 use futures::{stream::BoxStream, StreamExt};
 use lazy_static::lazy_static;
 use serde::de::{Error, SeqAccess, Visitor};
 use serde::ser::SerializeSeq;
@@ -85,35 +85,29 @@
     /// Try creating a new instance of [`DeltaObjectStore`]
     ///
     /// # Arguments
     ///
     /// * `location` - A url pointing to the root of the delta table.
     /// * `options` - Options passed to underlying builders. See [`with_storage_options`](crate::builder::DeltaTableBuilder::with_storage_options)
     pub fn try_new(location: Url, options: impl Into<StorageOptions> + Clone) -> DeltaResult<Self> {
-        let prefix = Path::from(location.path());
-        let root_store =
-            ObjectStoreKind::parse_url(&location)?.into_impl(location.as_ref(), options.clone())?;
-        let storage = if prefix != Path::from("/") {
-            root_store.into_prefix(prefix)
-        } else {
-            root_store.into_store()
-        };
+        let options = options.into();
+        let storage = config::configure_store(&location, &options)?;
         Ok(Self {
             storage,
             location,
-            options: options.into(),
+            options,
         })
     }
 
     /// Get a reference to the underlying storage backend
     pub fn storage_backend(&self) -> Arc<DynObjectStore> {
         self.storage.clone()
     }
 
-    /// Storage options used to intialize storage backend
+    /// Storage options used to initialize storage backend
     pub fn storage_options(&self) -> &StorageOptions {
         &self.options
     }
 
     /// Get fully qualified uri for table root
     pub fn root_uri(&self) -> String {
         self.to_uri(&Path::from(""))
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/storage/s3.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/storage/s3.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/storage/utils.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/storage/utils.rs`

 * *Files 13% similar despite different names*

```diff
@@ -87,14 +87,41 @@
                         value.modification_time
                     )),
                 },
             )?,
             Utc,
         );
         Ok(Self {
-            // TODO this won't work for absoute paths, since Paths are always relative to store.
-            location: Path::from(value.path.as_str()),
+            // TODO this won't work for absolute paths, since Paths are always relative to store.
+            location: Path::parse(value.path.as_str())?,
             last_modified,
             size: value.size as usize,
         })
     }
 }
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_object_meta_from_add_action() {
+        let add = Add {
+            path: "x=A%252FA/part-00007-b350e235-2832-45df-9918-6cab4f7578f7.c000.snappy.parquet"
+                .to_string(),
+            size: 123,
+            modification_time: 123456789,
+            ..Default::default()
+        };
+
+        let meta: ObjectMeta = (&add).try_into().unwrap();
+        assert_eq!(
+            meta.location,
+            Path::parse(
+                "x=A%252FA/part-00007-b350e235-2832-45df-9918-6cab4f7578f7.c000.snappy.parquet"
+            )
+            .unwrap()
+        );
+        assert_eq!(meta.size, 123);
+        assert_eq!(meta.last_modified.timestamp_millis(), 123456789);
+    }
+}
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/table_state.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/table_state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -364,20 +364,24 @@
 
     /// Obtain Add actions for files that match the filter
     pub fn get_active_add_actions_by_partitions<'a>(
         &'a self,
         filters: &'a [PartitionFilter<'a, &'a str>],
     ) -> Result<impl Iterator<Item = &'a Add> + '_, DeltaTableError> {
         let current_metadata = self.current_metadata().ok_or(DeltaTableError::NoMetadata)?;
-        if !filters
+
+        let nonpartitioned_columns: Vec<String> = filters
             .iter()
-            .all(|f| current_metadata.partition_columns.contains(&f.key.into()))
-        {
-            return Err(DeltaTableError::InvalidPartitionFilter {
-                partition_filter: format!("{filters:?}"),
+            .filter(|f| !current_metadata.partition_columns.contains(&f.key.into()))
+            .map(|f| f.key.to_string())
+            .collect();
+
+        if !nonpartitioned_columns.is_empty() {
+            return Err(DeltaTableError::ColumnsNotPartitioned {
+                nonpartitioned_columns: { nonpartitioned_columns },
             });
         }
 
         let partition_col_data_types: HashMap<&str, &SchemaDataType> = current_metadata
             .get_partition_col_data_types()
             .into_iter()
             .collect();
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/table_state_arrow.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/table_state_arrow.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/test_utils.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/test_utils.rs`

 * *Files 17% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         }
         integration.create_bucket(&bucket)?;
         let store_uri = match integration {
             StorageIntegration::Amazon => format!("s3://{}", &bucket),
             StorageIntegration::Microsoft => format!("az://{}", &bucket),
             StorageIntegration::Google => format!("gs://{}", &bucket),
             StorageIntegration::Local => format!("file://{}", &bucket),
+            StorageIntegration::Hdfs => format!("hdfs://localhost:9000/{}", &bucket),
         };
         // the "storage_backend" will always point to the root ofg the object store.
         // TODO should we provide the store via object_Store builders?
         let store = match integration {
             StorageIntegration::Local => Arc::new(
                 object_store::local::LocalFileSystem::new_with_prefix(tmp_dir.path())?,
             ),
@@ -81,14 +82,15 @@
     /// Get the URI for initializing a store at the root
     pub fn root_uri(&self) -> String {
         match self.integration {
             StorageIntegration::Amazon => format!("s3://{}", &self.bucket),
             StorageIntegration::Microsoft => format!("az://{}", &self.bucket),
             StorageIntegration::Google => format!("gs://{}", &self.bucket),
             StorageIntegration::Local => format!("file://{}", &self.bucket),
+            StorageIntegration::Hdfs => format!("hdfs://localhost:9000/{}", &self.bucket),
         }
     }
 
     pub fn table_builder(&self, table: TestTables) -> DeltaTableBuilder {
         let name = table.as_name();
         let table_uri = format!("{}/{}", self.root_uri(), &name);
         DeltaTableBuilder::from_uri(table_uri).with_allow_http(true)
@@ -112,14 +114,22 @@
             StorageIntegration::Local => {
                 let mut options = CopyOptions::new();
                 options.content_only = true;
                 let dest_path = self.tmp_dir.path().join(name.as_ref());
                 std::fs::create_dir_all(&dest_path)?;
                 copy(table.as_path(), &dest_path, &options)?;
             }
+            StorageIntegration::Amazon => {
+                let dest = format!("{}/{}", self.root_uri(), name.as_ref());
+                s3_cli::copy_directory(table.as_path(), dest)?;
+            }
+            StorageIntegration::Microsoft => {
+                let dest = format!("{}/{}", self.bucket, name.as_ref());
+                az_cli::copy_directory(table.as_path(), dest)?;
+            }
             _ => {
                 let from = table.as_path().as_str().to_owned();
                 let to = format!("{}/{}", self.root_uri(), name.as_ref());
                 copy_table(from, None, to, None, true).await?;
             }
         };
         Ok(())
@@ -136,33 +146,38 @@
             StorageIntegration::Microsoft => {
                 az_cli::delete_container(&self.bucket).unwrap();
             }
             StorageIntegration::Google => {
                 gs_cli::delete_bucket(&self.bucket).unwrap();
             }
             StorageIntegration::Local => (),
+            StorageIntegration::Hdfs => {
+                hdfs_cli::delete_dir(&self.bucket).unwrap();
+            }
         };
     }
 }
 
 /// Kinds of storage integration
 pub enum StorageIntegration {
     Amazon,
     Microsoft,
     Google,
     Local,
+    Hdfs,
 }
 
 impl StorageIntegration {
     fn prepare_env(&self) {
         match self {
             Self::Microsoft => az_cli::prepare_env(),
             Self::Amazon => s3_cli::prepare_env(),
             Self::Google => gs_cli::prepare_env(),
             Self::Local => (),
+            Self::Hdfs => (),
         }
     }
 
     fn create_bucket(&self, name: impl AsRef<str>) -> std::io::Result<()> {
         match self {
             Self::Microsoft => {
                 az_cli::create_container(name)?;
@@ -178,24 +193,29 @@
                 Ok(())
             }
             Self::Google => {
                 gs_cli::create_bucket(name)?;
                 Ok(())
             }
             Self::Local => Ok(()),
+            Self::Hdfs => {
+                hdfs_cli::create_dir(name)?;
+                Ok(())
+            }
         }
     }
 }
 
 /// Reference tables from the test data folder
 pub enum TestTables {
     Simple,
     SimpleCommit,
     Golden,
     Delta0_8_0Partitioned,
+    Delta0_8_0SpecialPartitioned,
     Custom(String),
 }
 
 impl TestTables {
     fn as_path(&self) -> String {
         // env "CARGO_MANIFEST_DIR" is "the directory containing the manifest of your package",
         // set by `cargo run` or `cargo test`, see:
@@ -211,25 +231,31 @@
                 .unwrap()
                 .to_owned(),
             Self::Delta0_8_0Partitioned => data_path
                 .join("delta-0.8.0-partitioned")
                 .to_str()
                 .unwrap()
                 .to_owned(),
+            Self::Delta0_8_0SpecialPartitioned => data_path
+                .join("delta-0.8.0-special-partition")
+                .to_str()
+                .unwrap()
+                .to_owned(),
             // the data path for upload does not apply to custom tables.
             Self::Custom(_) => todo!(),
         }
     }
 
     pub fn as_name(&self) -> String {
         match self {
             Self::Simple => "simple".into(),
             Self::SimpleCommit => "simple_commit".into(),
             Self::Golden => "golden".into(),
             Self::Delta0_8_0Partitioned => "delta-0.8.0-partitioned".into(),
+            Self::Delta0_8_0SpecialPartitioned => "delta-0.8.0-special-partition".into(),
             Self::Custom(name) => name.to_owned(),
         }
     }
 }
 
 /// Set environment variable if it is not set
 pub fn set_env_if_not_set(key: impl AsRef<str>, value: impl AsRef<str>) {
@@ -269,14 +295,34 @@
                 container_name.as_ref(),
             ])
             .spawn()
             .expect("az command is installed");
         child.wait()
     }
 
+    /// copy directory
+    pub fn copy_directory(
+        source: impl AsRef<str>,
+        destination: impl AsRef<str>,
+    ) -> std::io::Result<ExitStatus> {
+        let mut child = Command::new("az")
+            .args([
+                "storage",
+                "blob",
+                "upload-batch",
+                "-s",
+                source.as_ref(),
+                "-d",
+                destination.as_ref(),
+            ])
+            .spawn()
+            .expect("az command is installed");
+        child.wait()
+    }
+
     /// prepare_env
     pub fn prepare_env() {
         set_env_if_not_set("AZURE_STORAGE_USE_EMULATOR", "1");
         set_env_if_not_set("AZURE_STORAGE_ACCOUNT_NAME", "devstoreaccount1");
         set_env_if_not_set("AZURE_STORAGE_ACCOUNT_KEY", "Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==");
         set_env_if_not_set(
             "AZURE_STORAGE_CONNECTION_STRING",
@@ -326,14 +372,36 @@
                 "--force",
             ])
             .spawn()
             .expect("aws command is installed");
         child.wait()
     }
 
+    /// copy directory
+    pub fn copy_directory(
+        source: impl AsRef<str>,
+        destination: impl AsRef<str>,
+    ) -> std::io::Result<ExitStatus> {
+        let endpoint = std::env::var(s3_storage_options::AWS_ENDPOINT_URL)
+            .expect("variable ENDPOINT must be set to connect to S3");
+        let mut child = Command::new("aws")
+            .args([
+                "s3",
+                "cp",
+                source.as_ref(),
+                destination.as_ref(),
+                "--endpoint-url",
+                &endpoint,
+                "--recursive",
+            ])
+            .spawn()
+            .expect("aws command is installed");
+        child.wait()
+    }
+
     /// prepare_env
     pub fn prepare_env() {
         set_env_if_not_set(
             s3_storage_options::AWS_ENDPOINT_URL,
             "http://localhost:4566",
         );
         set_env_if_not_set(s3_storage_options::AWS_ACCESS_KEY_ID, "deltalake");
@@ -443,7 +511,49 @@
 
     /// prepare_env
     pub fn prepare_env() {
         set_env_if_not_set("GOOGLE_BASE_URL", "http://localhost:4443");
         set_env_if_not_set("GOOGLE_ENDPOINT_URL", "http://localhost:4443/storage/v1/b");
     }
 }
+
+/// small wrapper around hdfs cli
+pub mod hdfs_cli {
+    use std::env;
+    use std::path::PathBuf;
+    use std::process::{Command, ExitStatus};
+
+    fn hdfs_cli_path() -> PathBuf {
+        let hadoop_home =
+            env::var("HADOOP_HOME").expect("HADOOP_HOME environment variable not set");
+        PathBuf::from(hadoop_home).join("bin").join("hdfs")
+    }
+
+    pub fn create_dir(dir_name: impl AsRef<str>) -> std::io::Result<ExitStatus> {
+        let path = hdfs_cli_path();
+        let mut child = Command::new(path)
+            .args([
+                "dfs",
+                "-mkdir",
+                "-p",
+                format!("/{}", dir_name.as_ref()).as_str(),
+            ])
+            .spawn()
+            .expect("hdfs command is installed");
+        child.wait()
+    }
+
+    pub fn delete_dir(dir_name: impl AsRef<str>) -> std::io::Result<ExitStatus> {
+        let path = hdfs_cli_path();
+        let mut child = Command::new(path)
+            .args([
+                "dfs",
+                "-rm",
+                "-r",
+                "-f",
+                format!("/{}", dir_name.as_ref()).as_str(),
+            ])
+            .spawn()
+            .expect("hdfs command is installed");
+        child.wait()
+    }
+}
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/time_utils.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/time_utils.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/writer/json.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/writer/json.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/writer/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/writer/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -124,13 +124,14 @@
     /// Flush the internal write buffers to files in the delta table folder structure.
     /// and commit the changes to the Delta log, creating a new table version.
     async fn flush_and_commit(
         &mut self,
         table: &mut DeltaTable,
     ) -> Result<DeltaDataTypeVersion, DeltaTableError> {
         let mut adds = self.flush().await?;
+        #[allow(deprecated)]
         let mut tx = table.create_transaction(None);
         tx.add_actions(adds.drain(..).map(Action::add).collect());
         let version = tx.commit(None, None).await?;
         Ok(version)
     }
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/writer/record_batch.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/writer/record_batch.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/writer/stats.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/writer/stats.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/writer/test_utils.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/writer/test_utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#![allow(deprecated)]
 //! Utilities for writing unit tests
 use super::*;
 use crate::{
     action::Protocol, schema::Schema, DeltaTable, DeltaTableBuilder, DeltaTableMetaData,
     SchemaDataType, SchemaField,
 };
 use arrow::record_batch::RecordBatch;
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/src/writer/utils.rs` & `deltalake-0.9.0/local_dependencies/deltalake/src/writer/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 };
 use arrow::datatypes::{
     DataType, Date32Type, Date64Type, Int16Type, Int32Type, Int64Type, Int8Type,
     Schema as ArrowSchema, SchemaRef as ArrowSchemaRef, TimeUnit, TimestampMicrosecondType,
     TimestampMillisecondType, TimestampNanosecondType, TimestampSecondType, UInt16Type, UInt32Type,
     UInt64Type, UInt8Type,
 };
+// NOTE: Temporarily allowing these deprecated imports pending the completion of:
+// <https://github.com/apache/arrow-rs/pull/3979>
+#[allow(deprecated)]
 use arrow::json::reader::{Decoder, DecoderOptions};
 use arrow::record_batch::*;
 use object_store::path::Path;
 use parking_lot::RwLock;
 use serde_json::Value;
 use uuid::Uuid;
 
@@ -100,14 +103,17 @@
         return Ok(Path::from(file_name));
     }
 
     let partition_key = PartitionPath::from_hashmap(partition_columns, partition_values)?;
     Ok(Path::from(format!("{partition_key}/{file_name}")))
 }
 
+// NOTE: Temporarily allowing these deprecated imports pending the completion of:
+// <https://github.com/apache/arrow-rs/pull/3979>
+#[allow(deprecated)]
 /// Convert a vector of json values to a RecordBatch
 pub fn record_batch_from_message(
     arrow_schema: Arc<ArrowSchema>,
     message_buffer: &[Value],
 ) -> Result<RecordBatch, DeltaTableError> {
     let mut value_iter = message_buffer.iter().map(|j| Ok(j.to_owned()));
     let options = DecoderOptions::new().with_batch_size(message_buffer.len());
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/add_actions_test.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/add_actions_test.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/checkpoint_writer.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/checkpoint_writer.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/command_filesystem_check.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/command_filesystem_check.rs`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 #[cfg(feature = "gcs")]
 #[tokio::test]
 #[serial]
 async fn test_filesystem_check_gcp() -> TestResult {
     Ok(test_filesystem_check(StorageIntegration::Google).await?)
 }
 
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+#[serial]
+async fn test_filesystem_check_hdfs() -> TestResult {
+    Ok(test_filesystem_check(StorageIntegration::Hdfs).await?)
+}
+
 async fn test_filesystem_check(storage: StorageIntegration) -> TestResult {
     let context = IntegrationContext::new(storage)?;
     context.load_table(TestTables::Simple).await?;
     let file = "part-00000-2befed33-c358-4768-a43c-3eda0d2a499d-c000.snappy.parquet";
     let path = Path::from_iter([&TestTables::Simple.as_name(), file]);
 
     // Delete an active file from underlying storage without an update to the log to simulate an external fault
@@ -109,15 +116,15 @@
     let remove = table.state.all_tombstones().get(file).unwrap();
     assert_eq!(remove.data_change, true);
     Ok(())
 }
 
 #[tokio::test]
 #[serial]
-async fn test_filesystem_check_outdated() -> TestResult {
+async fn test_filesystem_check_fails_for_concurrent_delete() -> TestResult {
     // Validate failure when a non dry only executes on the latest version
     let context = IntegrationContext::new(StorageIntegration::Local)?;
     context.load_table(TestTables::Simple).await?;
     let file = "part-00003-53f42606-6cda-4f13-8d07-599a21197296-c000.snappy.parquet";
     let path = Path::from_iter([&TestTables::Simple.as_name(), file]);
 
     // Delete an active file from underlying storage without an update to the log to simulate an external fault
@@ -128,14 +135,42 @@
         .with_version(2)
         .load()
         .await?;
 
     let op = DeltaOps::from(table);
     let res = op.filesystem_check().with_dry_run(false).await;
 
+    // TODO check more specific error
+    assert!(matches!(res, Err(DeltaTableError::Transaction { .. })));
+
+    Ok(())
+}
+
+#[tokio::test]
+#[serial]
+#[ignore = "should this actually fail? with conflcit resolution, we are re-trying again."]
+async fn test_filesystem_check_outdated() -> TestResult {
+    // Validate failure when a non dry only executes on the latest version
+    let context = IntegrationContext::new(StorageIntegration::Local)?;
+    context.load_table(TestTables::Simple).await?;
+    let file = "part-00007-3a0e4727-de0d-41b6-81ef-5223cf40f025-c000.snappy.parquet";
+    let path = Path::from_iter([&TestTables::Simple.as_name(), file]);
+
+    // Delete an active file from underlying storage without an update to the log to simulate an external fault
+    context.object_store().delete(&path).await?;
+
+    let table = context
+        .table_builder(TestTables::Simple)
+        .with_version(2)
+        .load()
+        .await?;
+
+    let op = DeltaOps::from(table);
+    let res = op.filesystem_check().with_dry_run(false).await;
+    println!("{:?}", res);
     if let Err(DeltaTableError::VersionAlreadyExists(version)) = res {
         assert!(version == 3);
     } else {
         assert!(false);
     }
 
     Ok(())
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/command_optimize.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/command_optimize.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,38 +2,34 @@
 
 use arrow::datatypes::Schema as ArrowSchema;
 use arrow::{
     array::{Int32Array, StringArray},
     datatypes::{DataType, Field},
     record_batch::RecordBatch,
 };
-use deltalake::action::{Action, Protocol, Remove};
-use deltalake::builder::DeltaTableBuilder;
+use deltalake::action::{Action, Remove};
 use deltalake::operations::optimize::{create_merge_plan, MetricDetails, Metrics};
 use deltalake::operations::DeltaOps;
 use deltalake::writer::{DeltaWriter, RecordBatchWriter};
-use deltalake::{
-    DeltaTable, DeltaTableError, DeltaTableMetaData, PartitionFilter, Schema, SchemaDataType,
-    SchemaField,
-};
+use deltalake::{DeltaTable, DeltaTableError, PartitionFilter, SchemaDataType, SchemaField};
 use parquet::file::properties::WriterProperties;
 use rand::prelude::*;
-use serde_json::{json, Map, Value};
+use serde_json::json;
 use std::time::SystemTime;
 use std::time::UNIX_EPOCH;
 use std::{collections::HashMap, error::Error, sync::Arc};
 use tempdir::TempDir;
 
 struct Context {
     pub tmp_dir: TempDir,
     pub table: DeltaTable,
 }
 
 async fn setup_test(partitioned: bool) -> Result<Context, Box<dyn Error>> {
-    let schema = Schema::new(vec![
+    let columns = vec![
         SchemaField::new(
             "x".to_owned(),
             SchemaDataType::primitive("integer".to_owned()),
             false,
             HashMap::new(),
         ),
         SchemaField::new(
@@ -44,53 +40,30 @@
         ),
         SchemaField::new(
             "date".to_owned(),
             SchemaDataType::primitive("string".to_owned()),
             false,
             HashMap::new(),
         ),
-    ]);
+    ];
 
-    let p = if partitioned {
+    let partition_columns = if partitioned {
         vec!["date".to_owned()]
     } else {
         vec![]
     };
 
-    let table_meta = DeltaTableMetaData::new(
-        Some("opt_table".to_owned()),
-        Some("Table for optimize tests".to_owned()),
-        None,
-        schema.clone(),
-        p,
-        HashMap::new(),
-    );
-
     let tmp_dir = tempdir::TempDir::new("opt_table").unwrap();
-    let p = tmp_dir.path().to_str().to_owned().unwrap();
-    let mut dt = DeltaTableBuilder::from_uri(p).build()?;
-
-    let mut commit_info = Map::<String, Value>::new();
-
-    let protocol = Protocol {
-        min_reader_version: 1,
-        min_writer_version: 2,
-    };
-
-    commit_info.insert(
-        "operation".to_string(),
-        serde_json::Value::String("CREATE TABLE".to_string()),
-    );
-    dt.create(
-        table_meta.clone(),
-        protocol.clone(),
-        Some(commit_info),
-        None,
-    )
-    .await?;
+    let table_uri = tmp_dir.path().to_str().to_owned().unwrap();
+    let dt = DeltaOps::try_from_uri(table_uri)
+        .await?
+        .create()
+        .with_columns(columns)
+        .with_partition_columns(partition_columns)
+        .await?;
 
     Ok(Context { tmp_dir, table: dt })
 }
 
 fn generate_random_batch<T: Into<String>>(
     rows: usize,
     partition: T,
@@ -310,25 +283,25 @@
         data_change: true,
         extended_file_metadata: None,
         size: Some(add.size),
         partition_values: Some(add.partition_values.clone()),
         tags: Some(HashMap::new()),
     };
 
+    #[allow(deprecated)]
     let mut transaction = other_dt.create_transaction(None);
     transaction.add_action(Action::remove(remove));
     transaction.commit(None, None).await?;
 
-    let maybe_metrics = plan.execute(dt.object_store()).await;
+    let maybe_metrics = plan.execute(dt.object_store(), &dt.state).await;
     assert!(maybe_metrics.is_err());
     assert_eq!(dt.version(), version + 1);
     Ok(())
 }
 
-#[ignore = "we do not yet re-try in operations commits."]
 #[tokio::test]
 /// Validate that optimize succeeds when only add actions occur for a optimized partition
 async fn test_no_conflict_for_append_actions() -> Result<(), Box<dyn Error>> {
     let context = setup_test(true).await?;
     let mut dt = context.table;
     let mut writer = RecordBatchWriter::for_table(&dt)?;
 
@@ -363,17 +336,19 @@
     write(
         &mut writer,
         &mut other_dt,
         tuples_to_batch(vec![(3, 2), (3, 3), (3, 4)], "2022-05-22")?,
     )
     .await?;
 
-    let metrics = plan.execute(dt.object_store()).await?;
+    let metrics = plan.execute(dt.object_store(), &dt.state).await?;
     assert_eq!(metrics.num_files_added, 1);
     assert_eq!(metrics.num_files_removed, 2);
+
+    dt.update().await.unwrap();
     assert_eq!(dt.version(), version + 2);
     Ok(())
 }
 
 #[tokio::test]
 #[ignore]
 /// Validate that bin packing is idempotent.
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/command_vacuum.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/command_vacuum.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/commit_info_format.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/commit_info_format.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#[allow(dead_code)]
+#![allow(dead_code, deprecated)]
 mod fs_common;
 
 use deltalake::action::{Action, DeltaOperation, SaveMode};
 use serde_json::json;
 use std::error::Error;
 use tempdir::TempDir;
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/common/adls.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/common/adls.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/common/clock.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/common/clock.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/common/datafusion.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/common/datafusion.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-use datafusion::datasource::datasource::TableProviderFactory;
-use datafusion::execution::context::SessionContext;
+use datafusion::execution::context::{SessionContext, SessionState};
 use datafusion::execution::runtime_env::{RuntimeConfig, RuntimeEnv};
 use datafusion::prelude::SessionConfig;
 use deltalake::delta_datafusion::DeltaTableFactory;
-use std::collections::HashMap;
 use std::sync::Arc;
 
 pub fn context_with_delta_table_factory() -> SessionContext {
-    let mut table_factories: HashMap<String, Arc<dyn TableProviderFactory>> = HashMap::new();
-    table_factories.insert("DELTATABLE".to_string(), Arc::new(DeltaTableFactory {}));
-    let cfg = RuntimeConfig::new().with_table_factories(table_factories);
+    let cfg = RuntimeConfig::new();
     let env = RuntimeEnv::new(cfg).unwrap();
     let ses = SessionConfig::new();
-    SessionContext::with_config_rt(ses, Arc::new(env))
+    let mut state = SessionState::with_config_rt(ses, Arc::new(env));
+    state
+        .table_factories_mut()
+        .insert("DELTATABLE".to_string(), Arc::new(DeltaTableFactory {}));
+    SessionContext::with_state(state)
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/common/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/integration_concurrent_writes.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,170 @@
-#![allow(dead_code)]
-#![allow(unused_variables)]
+#![cfg(feature = "integration_test")]
 
-use bytes::Bytes;
-use deltalake::action::{self, Add, Remove};
-use deltalake::builder::DeltaTableBuilder;
-use deltalake::storage::DeltaObjectStore;
-use deltalake::{DeltaTable, DeltaTableConfig, DeltaTableMetaData, Schema};
-use object_store::{path::Path, ObjectStore};
-use serde_json::{Map, Value};
-use std::any::Any;
+use deltalake::test_utils::{IntegrationContext, StorageIntegration, TestResult, TestTables};
+use deltalake::{
+    action, DeltaTable, DeltaTableBuilder, DeltaTableMetaData, Schema, SchemaDataType, SchemaField,
+};
 use std::collections::HashMap;
-use std::sync::Arc;
-use tempdir::TempDir;
-
-#[cfg(feature = "azure")]
-pub mod adls;
-pub mod clock;
-#[cfg(feature = "datafusion")]
-pub mod datafusion;
-#[cfg(any(feature = "s3", feature = "s3-native-tls"))]
-pub mod s3;
-pub mod schemas;
-
-#[derive(Default)]
-pub struct TestContext {
-    /// The main table under test
-    pub table: Option<DeltaTable>,
-    pub backend: Option<Arc<DeltaObjectStore>>,
-    /// The configuration used to create the backend.
-    pub config: HashMap<String, String>,
-    /// An object when it is dropped will clean up any temporary resources created for the test
-    pub storage_context: Option<Box<dyn Any>>,
-}
-
-pub struct LocalFS {
-    pub tmp_dir: TempDir,
-}
-
-impl TestContext {
-    pub async fn from_env() -> Self {
-        let backend = std::env::var("DELTA_RS_TEST_BACKEND");
-        let backend_ref = backend.as_ref().map(|s| s.as_str());
-        match backend_ref {
-            Ok("LOCALFS") | Err(std::env::VarError::NotPresent) => setup_local_context().await,
-            #[cfg(feature = "azure")]
-            Ok("AZURE_GEN2") => adls::setup_azure_gen2_context().await,
-            #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
-            Ok("S3_LOCAL_STACK") => s3::setup_s3_context().await,
-            _ => panic!("Invalid backend for delta-rs tests"),
-        }
-    }
-
-    pub fn get_storage(&mut self) -> Arc<DeltaObjectStore> {
-        if self.backend.is_none() {
-            self.backend = Some(self.new_storage())
-        }
-
-        self.backend.as_ref().unwrap().clone()
-    }
+use std::future::Future;
+use std::iter::FromIterator;
+use std::time::Duration;
+
+#[tokio::test]
+async fn test_concurrent_writes_local() -> TestResult {
+    test_concurrent_writes(StorageIntegration::Local).await?;
+    Ok(())
+}
 
-    fn new_storage(&self) -> Arc<DeltaObjectStore> {
-        let config = self.config.clone();
-        let uri = config.get("URI").unwrap().to_string();
-        DeltaTableBuilder::from_uri(uri)
-            .with_storage_options(config)
-            .build_storage()
-            .unwrap()
-    }
-
-    //Create and set a new table from the provided schema
-    pub async fn create_table_from_schema(
-        &mut self,
-        schema: Schema,
-        partitions: &[&str],
-    ) -> DeltaTable {
-        let p = partitions
-            .iter()
-            .map(|s| s.to_string())
-            .collect::<Vec<String>>();
-        let table_meta = DeltaTableMetaData::new(
-            Some("delta-rs_test_table".to_owned()),
-            Some("Table created by delta-rs tests".to_owned()),
-            None,
-            schema.clone(),
-            p,
-            HashMap::new(),
-        );
-
-        let backend = self.new_storage();
-        let mut dt = DeltaTable::new(backend, DeltaTableConfig::default());
-        let mut commit_info = Map::<String, Value>::new();
-
-        let protocol = action::Protocol {
-            min_reader_version: 1,
-            min_writer_version: 2,
-        };
-
-        commit_info.insert(
-            "operation".to_string(),
-            serde_json::Value::String("CREATE TABLE".to_string()),
-        );
-        dt.create(
-            table_meta.clone(),
-            protocol.clone(),
-            Some(commit_info),
-            None,
-        )
-        .await
-        .unwrap();
-
-        dt
-    }
+#[cfg(feature = "s3")]
+#[tokio::test]
+async fn concurrent_writes_s3() -> TestResult {
+    test_concurrent_writes(StorageIntegration::Amazon).await?;
+    Ok(())
 }
 
-pub async fn setup_local_context() -> TestContext {
-    let tmp_dir = tempdir::TempDir::new("delta-rs_tests").unwrap();
-    let mut config = HashMap::new();
-    config.insert(
-        "URI".to_owned(),
-        tmp_dir.path().to_str().to_owned().unwrap().to_string(),
+#[cfg(feature = "azure")]
+#[tokio::test]
+async fn test_concurrent_writes_azure() -> TestResult {
+    test_concurrent_writes(StorageIntegration::Microsoft).await?;
+    Ok(())
+}
+
+// tracked via https://github.com/datafusion-contrib/datafusion-objectstore-hdfs/issues/13
+#[ignore]
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+async fn test_concurrent_writes_hdfs() -> TestResult {
+    test_concurrent_writes(StorageIntegration::Hdfs).await?;
+    Ok(())
+}
+
+async fn test_concurrent_writes(integration: StorageIntegration) -> TestResult {
+    let context = IntegrationContext::new(integration)?;
+    let (_table, table_uri) = prepare_table(&context).await?;
+    run_test(|name| Worker::new(&table_uri, name)).await;
+    Ok(())
+}
+
+async fn prepare_table(
+    context: &IntegrationContext,
+) -> Result<(DeltaTable, String), Box<dyn std::error::Error + 'static>> {
+    let schema = Schema::new(vec![SchemaField::new(
+        "Id".to_string(),
+        SchemaDataType::primitive("integer".to_string()),
+        true,
+        HashMap::new(),
+    )]);
+    let metadata = DeltaTableMetaData::new(
+        Some("Azure Test Table".to_string()),
+        None,
+        None,
+        schema,
+        vec![],
+        HashMap::new(),
     );
+    let protocol = action::Protocol {
+        min_reader_version: 1,
+        min_writer_version: 2,
+    };
 
-    let localfs = LocalFS { tmp_dir };
-
-    TestContext {
-        storage_context: Some(Box::new(localfs)),
-        config,
-        ..TestContext::default()
+    let table_uri = context.uri_for_table(TestTables::Custom("concurrent_workers".into()));
+    let mut table = DeltaTableBuilder::from_uri(&table_uri)
+        .with_allow_http(true)
+        .build()?;
+    table.create(metadata, protocol, None, None).await?;
+
+    assert_eq!(0, table.version());
+    assert_eq!(1, table.get_min_reader_version());
+    assert_eq!(2, table.get_min_writer_version());
+    assert_eq!(0, table.get_files().len());
+
+    Ok((table, table_uri))
+}
+
+const WORKERS: i64 = 5;
+const COMMITS: i64 = 3;
+
+async fn run_test<F, Fut>(create_worker: F)
+where
+    F: Fn(String) -> Fut,
+    Fut: Future<Output = Worker>,
+{
+    let mut workers = Vec::new();
+    for w in 0..WORKERS {
+        workers.push(create_worker(format!("w{}", w)).await);
+    }
+
+    let mut futures = Vec::new();
+    for mut w in workers {
+        let run = tokio::spawn(async move { w.commit_sequence(COMMITS).await });
+        futures.push(run)
+    }
+
+    let mut map = HashMap::new();
+    for f in futures {
+        map.extend(f.await.unwrap());
+    }
+
+    // to ensure that there's been no collisions between workers of acquiring the same version
+    assert_eq!(map.len() as i64, WORKERS * COMMITS);
+
+    // check that we have unique and ascending versions committed
+    let mut versions = Vec::from_iter(map.keys().map(|x| x.clone()));
+    versions.sort();
+    assert_eq!(versions, Vec::from_iter(1i64..=WORKERS * COMMITS));
+
+    // check that each file for each worker is committed as expected
+    let mut files = Vec::from_iter(map.values().map(|x| x.clone()));
+    files.sort();
+    let mut expected = Vec::new();
+    for w in 0..WORKERS {
+        for c in 0..COMMITS {
+            expected.push(format!("w{}-{}", w, c))
+        }
     }
+    assert_eq!(files, expected);
 }
 
-pub async fn add_file(
-    table: &mut DeltaTable,
-    path: &Path,
-    data: Bytes,
-    partition_values: &[(&str, Option<&str>)],
-    create_time: i64,
-    commit_to_log: bool,
-) {
-    let backend = table.object_store();
-    backend.put(path, data.clone()).await.unwrap();
-
-    if commit_to_log {
-        let mut part_values = HashMap::new();
-        for v in partition_values {
-            part_values.insert(v.0.to_string(), v.1.map(|v| v.to_string()));
+pub struct Worker {
+    pub table: DeltaTable,
+    pub name: String,
+}
+
+impl Worker {
+    pub async fn new(path: &str, name: String) -> Self {
+        std::env::set_var("DYNAMO_LOCK_OWNER_NAME", &name);
+        let table = DeltaTableBuilder::from_uri(path)
+            .with_allow_http(true)
+            .build()
+            .unwrap();
+        Self { table, name }
+    }
+
+    async fn commit_sequence(&mut self, n: i64) -> HashMap<i64, String> {
+        let mut result = HashMap::new();
+        for i in 0..n {
+            let name = format!("{}-{}", self.name, i);
+            let v = self.commit_file(&name).await;
+            result.insert(v, name);
+            tokio::time::sleep(Duration::from_millis(100)).await;
         }
 
-        let add = Add {
-            path: path.as_ref().into(),
-            size: data.len() as i64,
-            modification_time: create_time,
-            partition_values: part_values,
-            data_change: true,
-            ..Default::default()
-        };
-        let mut transaction = table.create_transaction(None);
-        transaction.add_action(action::Action::add(add));
-        transaction.commit(None, None).await.unwrap();
+        result
     }
-}
 
-pub async fn remove_file(
-    table: &mut DeltaTable,
-    path: &str,
-    partition_values: &[(&str, Option<&str>)],
-    deletion_timestamp: i64,
-) {
-    let mut part_values = HashMap::new();
-    for v in partition_values {
-        part_values.insert(v.0.to_string(), v.1.map(|v| v.to_string()));
-    }
-
-    let remove = Remove {
-        path: path.into(),
-        deletion_timestamp: Some(deletion_timestamp),
-        partition_values: Some(part_values),
-        data_change: true,
-        ..Default::default()
-    };
-    let mut transaction = table.create_transaction(None);
-    transaction.add_action(action::Action::remove(remove));
-    transaction.commit(None, None).await.unwrap();
+    async fn commit_file(&mut self, name: &str) -> i64 {
+        let mut tx = self.table.create_transaction(None);
+        tx.add_action(action::Action::add(action::Add {
+            path: format!("{}.parquet", name),
+            size: 396,
+            partition_values: HashMap::new(),
+            partition_values_parsed: None,
+            modification_time: 1564524294000,
+            data_change: true,
+            stats: None,
+            stats_parsed: None,
+            tags: None,
+        }));
+        tx.commit(None, None).await.unwrap()
+    }
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/common/s3.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/common/s3.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/common/schemas.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/common/schemas.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00000-a496f40c-e091-413a-85f9-b1b69d4b3b4e-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00000-a496f40c-e091-413a-85f9-b1b69d4b3b4e-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00001-9d9d980b-c500-4f0b-bb96-771a515fbccc-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00001-9d9d980b-c500-4f0b-bb96-771a515fbccc-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00002-8826af84-73bd-49a6-a4b9-e39ffed9c15a-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00002-8826af84-73bd-49a6-a4b9-e39ffed9c15a-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00003-539aff30-2349-4b0d-9726-c18630c6ad90-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00003-539aff30-2349-4b0d-9726-c18630c6ad90-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00004-1bb9c3e3-c5b0-4d60-8420-23261f58a5eb-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00004-1bb9c3e3-c5b0-4d60-8420-23261f58a5eb-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00005-4d47f8ff-94db-4d32-806c-781a1cf123d2-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00005-4d47f8ff-94db-4d32-806c-781a1cf123d2-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00006-d0ec7722-b30c-4e1c-92cd-b4fe8d3bb954-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00006-d0ec7722-b30c-4e1c-92cd-b4fe8d3bb954-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00007-4582392f-9fc2-41b0-ba97-a74b3afc8239-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/COVID-19_NYT/part-00007-4582392f-9fc2-41b0-ba97-a74b3afc8239-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000002.checkpoint.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoint_with_partitions/_delta_log/00000000000000000002.checkpoint.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000001.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000002.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000002.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000003.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000003.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000004.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000004.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000005.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000005.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000006.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000006.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000007.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000007.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000008.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000008.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000009.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000009.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000010.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000010.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000011.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000011.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000012.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints/_delta_log/00000000000000000012.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.checkpoint.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.checkpoint.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000005.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000006.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000006.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000007.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000007.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000008.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000008.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000009.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000009.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.checkpoint.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.checkpoint.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000010.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000011.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000011.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000012.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/checkpoints_vacuumed/_delta_log/00000000000000000012.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/concurrent_workers/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/concurrent_workers/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000002.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000002.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000003.checkpoint.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.2.0/_delta_log/00000000000000000003.checkpoint.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000001.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8-empty/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000001.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-date/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-date/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-date/part-00000-d22c627d-9655-4153-9527-f8995620fa42-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-date/part-00000-d22c627d-9655-4153-9527-f8995620fa42-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-null-partition/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-numeric-partition/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-partitioned/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-0.8.0-special-partition/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000002.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000003.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000004.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000005.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000006.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000007.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000008.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000009.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.checkpoint.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.checkpoint.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000010.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000011.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/_delta_log/00000000000000000012.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-1c2d1a32-02dc-484f-87ff-4328ea56045d-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-1c2d1a32-02dc-484f-87ff-4328ea56045d-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-28925d3a-bdf2-411e-bca9-b067444cbcb0-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-28925d3a-bdf2-411e-bca9-b067444cbcb0-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-6630b7c4-0aca-405b-be86-68a812f2e4c8-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-6630b7c4-0aca-405b-be86-68a812f2e4c8-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-74151571-7ec6-4bd6-9293-b5daab2ce667-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-74151571-7ec6-4bd6-9293-b5daab2ce667-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-7a509247-4f58-4453-9202-51d75dee59af-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-7a509247-4f58-4453-9202-51d75dee59af-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-8e0aefe1-6645-4601-ac29-68cba64023b5-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-8e0aefe1-6645-4601-ac29-68cba64023b5-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-b26ba634-874c-45b0-a7ff-2f0395a53966-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-b26ba634-874c-45b0-a7ff-2f0395a53966-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-c4c8caec-299d-42a4-b50c-5a4bf724c037-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-c4c8caec-299d-42a4-b50c-5a4bf724c037-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-ce300400-58ff-4b8f-8ba9-49422fdf9f2e-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-ce300400-58ff-4b8f-8ba9-49422fdf9f2e-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e1262b3e-2959-4910-aea9-4eaf92f0c68c-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e1262b3e-2959-4910-aea9-4eaf92f0c68c-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e8e3753f-e2f6-4c9f-98f9-8f3d346727ba-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-e8e3753f-e2f6-4c9f-98f9-8f3d346727ba-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-f73ff835-0571-4d67-ac43-4fbf948bfb9b-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-1.2.1-only-struct-stats/part-00000-f73ff835-0571-4d67-ac43-4fbf948bfb9b-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/delta-2.2.0-partitioned-types/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00000-182665f0-30df-470d-a5cb-8d9d483ed390-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00000-182665f0-30df-470d-a5cb-8d9d483ed390-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00001-2e274fe7-eb75-4b73-8c72-423ee747abc0-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/golden/data-reader-array-primitives/part-00001-2e274fe7-eb75-4b73-8c72-423ee747abc0-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_commit/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_commit/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000001.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000002.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000002.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000003.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000003.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000004.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table/_delta_log/00000000000000000004.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_change_data/cdc-00000-a846ce80-2eec-484d-bef7-0e63557786ca.c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_change_data/cdc-00000-a846ce80-2eec-484d-bef7-0e63557786ca.c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.crc` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.crc`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/_delta_log/00000000000000000002.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-7444aec4-710a-4a4c-8abe-3323499043e9.c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-7444aec4-710a-4a4c-8abe-3323499043e9.c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-996384f7-3fc5-4a5f-9921-6e56269ec2c9-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_cdc/part-00000-996384f7-3fc5-4a5f-9921-6e56269ec2c9-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000010.checkpoint.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/simple_table_with_checkpoint/_delta_log/00000000000000000010.checkpoint.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/_delta_log/00000000000000000000.json` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00000-a9dd181d-61aa-491d-b3c9-3eea548de6cb-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00000-a9dd181d-61aa-491d-b3c9-3eea548de6cb-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00001-f804d355-db40-4e13-a624-ddd50ce7f5c4-c000.snappy.parquet` & `deltalake-0.9.0/local_dependencies/deltalake/tests/data/table_with_edge_timestamps/part-00001-f804d355-db40-4e13-a624-ddd50ce7f5c4-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/datafusion_test.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/datafusion_test.rs`

 * *Files 11% similar despite different names*

```diff
@@ -184,44 +184,42 @@
         .with_location("memory://target")
         .with_columns(fields)
         .with_table_name("target")
         .await?;
 
     // Trying to execute the write from the input plan without providing Datafusion with a session
     // state containing the referenced object store in the registry results in an error.
-    assert!(WriteBuilder::new()
-        .with_input_execution_plan(source_scan.clone())
-        .with_object_store(target_table.object_store())
-        .await
-        .unwrap_err()
-        .to_string()
-        .contains("No suitable object store found for delta-rs://"));
+    assert!(
+        WriteBuilder::new(target_table.object_store(), target_table.state.clone())
+            .with_input_execution_plan(source_scan.clone())
+            .await
+            .unwrap_err()
+            .to_string()
+            .contains("No suitable object store found for delta-rs://")
+    );
 
     // Register the missing source table object store
     let source_uri = source_scan
         .as_any()
         .downcast_ref::<DeltaScan>()
         .unwrap()
         .table_uri
         .clone();
     let source_location = Url::parse(&source_uri).unwrap();
     let source_store = DeltaObjectStore::try_new(source_location, HashMap::new()).unwrap();
     let object_store_url = source_store.object_store_url();
     let source_store_url: &Url = object_store_url.as_ref();
-    state.runtime_env().register_object_store(
-        source_store_url.scheme(),
-        source_store_url.host_str().unwrap_or_default(),
-        Arc::from(source_store),
-    );
+    state
+        .runtime_env()
+        .register_object_store(source_store_url, Arc::from(source_store));
 
     // Execute write to the target table with the proper state
-    let target_table = WriteBuilder::new()
+    let target_table = WriteBuilder::new(target_table.object_store(), target_table.state.clone())
         .with_input_execution_plan(source_scan)
         .with_input_session_state(state)
-        .with_object_store(target_table.object_store())
         .await?;
     ctx.register_table("target", Arc::new(target_table))?;
 
     // Check results
     let batches = ctx.sql("SELECT * FROM target").await?.collect().await?;
     let expected = vec![
         "+------------+-----------+",
@@ -339,15 +337,15 @@
     if scan.output_partitioning().partition_count() > 0 {
         let plan = CoalescePartitionsExec::new(scan);
         let task_ctx = Arc::new(TaskContext::from(state));
         let _result = collect(plan.execute(0, task_ctx)?).await?;
         visit_execution_plan(&plan, &mut metrics).unwrap();
     }
 
-    return Ok(metrics);
+    Ok(metrics)
 }
 
 fn create_all_types_batch(not_null_rows: usize, null_rows: usize, offset: usize) -> RecordBatch {
     let mut decimal_builder = Decimal128Builder::with_capacity(not_null_rows + null_rows);
     for x in 0..not_null_rows {
         decimal_builder.append_value(((x + offset) * 100) as i128);
     }
@@ -456,14 +454,38 @@
             column,
             file1_value: expression_builder(1),
             file2_value: expression_builder(5),
             file3_value: expression_builder(8),
             non_existent_value: expression_builder(3),
         }
     }
+
+    fn new_wrapped<F>(column: &'static str, expression_builder: F) -> Self
+    where
+        F: Fn(i64) -> Expr,
+    {
+        TestCase {
+            column,
+            file1_value: wrap_expression(expression_builder(1)),
+            file2_value: wrap_expression(expression_builder(5)),
+            file3_value: wrap_expression(expression_builder(8)),
+            non_existent_value: wrap_expression(expression_builder(3)),
+        }
+    }
+}
+
+fn wrap_expression(e: Expr) -> Expr {
+    let value = match e {
+        Expr::Literal(lit) => lit,
+        _ => unreachable!(),
+    };
+    Expr::Literal(ScalarValue::Dictionary(
+        Box::new(ArrowDataType::UInt16),
+        Box::new(value),
+    ))
 }
 
 #[tokio::test]
 async fn test_files_scanned() -> Result<()> {
     // Validate that datafusion prunes files based on file statistics
     // Do not scan files when we know it does not contain the requested records
     use datafusion::prelude::*;
@@ -484,38 +506,35 @@
     let batch = create_all_types_batch(3, 0, 4);
     let table = append_to_table(table, batch).await;
 
     let batch = create_all_types_batch(3, 0, 7);
     let table = append_to_table(table, batch).await;
 
     let metrics = get_scan_metrics(&table, &state, &[]).await?;
-    assert!(metrics.num_scanned_files() == 3);
+    assert_eq!(metrics.num_scanned_files(), 3);
 
-    // (Column name, value from file 1, value from file 2, value from file 3, non existant value)
+    // (Column name, value from file 1, value from file 2, value from file 3, non existent value)
     let tests = [
         TestCase::new("utf8", |value| lit(value.to_string())),
-        TestCase::new("int64", |value| lit(value)),
+        TestCase::new("int64", lit),
         TestCase::new("int32", |value| lit(value as i32)),
         TestCase::new("int16", |value| lit(value as i16)),
         TestCase::new("int8", |value| lit(value as i8)),
         TestCase::new("float64", |value| lit(value as f64)),
         TestCase::new("float32", |value| lit(value as f32)),
         TestCase::new("timestamp", |value| {
-            lit(ScalarValue::TimestampMicrosecond(
-                Some(value * 1_000_000),
-                None,
-            ))
+            lit(TimestampMicrosecond(Some(value * 1_000_000), None))
         }),
         // TODO: I think decimal statistics are being written to the log incorrectly. The underlying i128 is written
-        // not the proper string representation as specified by the percision and scale
+        // not the proper string representation as specified by the precision and scale
         TestCase::new("decimal", |value| {
             lit(Decimal128(Some((value * 100).into()), 10, 2))
         }),
-        // TODO: The writer does not write complete statistiics for date columns
-        TestCase::new("date", |value| lit(ScalarValue::Date32(Some(value as i32)))),
+        // TODO: The writer does not write complete statistics for date columns
+        TestCase::new("date", |value| lit(Date32(Some(value as i32)))),
         // TODO: The writer does not write complete statistics for binary columns
         TestCase::new("binary", |value| lit(value.to_string().as_bytes())),
     ];
 
     for test in &tests {
         let TestCase {
             column,
@@ -528,27 +547,27 @@
         // TODO: The following types don't have proper stats written.
         // See issue #1208 for decimal type
         // See issue #1209 for dates
         // Min and Max is not calculated for binary columns. This matches the Spark writer
         if column == "decimal" || column == "date" || column == "binary" {
             continue;
         }
-        println!("Test Column: {}", column);
+        println!("Test Column: {} value: {}", column, file1_value);
 
         // Equality
         let e = col(column).eq(file1_value.clone());
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 1);
 
         // Value does not exist
         let e = col(column).eq(non_existent_value.clone());
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 0);
 
-        // Conjuction
+        // Conjunction
         let e = col(column)
             .gt(file1_value.clone())
             .and(col(column).lt(file2_value.clone()));
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 2);
 
         // Disjunction
@@ -569,14 +588,36 @@
     let metrics = get_scan_metrics(&table, &state, &[e]).await?;
     assert_eq!(metrics.num_scanned_files(), 1);
 
     let e = col("boolean").eq(lit(false));
     let metrics = get_scan_metrics(&table, &state, &[e]).await?;
     assert_eq!(metrics.num_scanned_files(), 1);
 
+    let tests = [
+        TestCase::new_wrapped("utf8", |value| lit(value.to_string())),
+        TestCase::new_wrapped("int64", lit),
+        TestCase::new_wrapped("int32", |value| lit(value as i32)),
+        TestCase::new_wrapped("int16", |value| lit(value as i16)),
+        TestCase::new_wrapped("int8", |value| lit(value as i8)),
+        TestCase::new_wrapped("float64", |value| lit(value as f64)),
+        TestCase::new_wrapped("float32", |value| lit(value as f32)),
+        TestCase::new_wrapped("timestamp", |value| {
+            lit(TimestampMicrosecond(Some(value * 1_000_000), None))
+        }),
+        // TODO: I think decimal statistics are being written to the log incorrectly. The underlying i128 is written
+        // not the proper string representation as specified by the precision and scale
+        TestCase::new_wrapped("decimal", |value| {
+            lit(Decimal128(Some((value * 100).into()), 10, 2))
+        }),
+        // TODO: The writer does not write complete statistics for date columns
+        TestCase::new_wrapped("date", |value| lit(Date32(Some(value as i32)))),
+        // TODO: The writer does not write complete statistics for binary columns
+        TestCase::new_wrapped("binary", |value| lit(value.to_string().as_bytes())),
+    ];
+
     // Ensure that tables with stats and partition columns can be pruned
     for test in tests {
         let TestCase {
             column,
             file1_value,
             file2_value,
             file3_value,
@@ -591,15 +632,14 @@
             || column == "decimal"
             || column == "binary"
             || column == "timestamp"
             || column == "date"
         {
             continue;
         }
-        println!("test {}", column);
 
         let partitions = vec![column.to_owned()];
         let batch = create_all_types_batch(3, 0, 0);
         let (_tmp, table) = prepare_table(vec![batch], SaveMode::Overwrite, partitions).await;
 
         let batch = create_all_types_batch(3, 0, 4);
         let table = append_to_table(table, batch).await;
@@ -613,34 +653,35 @@
         assert_eq!(metrics.num_scanned_files(), 1);
 
         // Value does not exist
         let e = col(column).eq(non_existent_value);
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 0);
 
-        // Conjuction
+        // Conjunction
         let e = col(column)
             .gt(file1_value.clone())
             .and(col(column).lt(file2_value));
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 2);
 
         // Disjunction
         let e = col(column).lt(file1_value).or(col(column).gt(file3_value));
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 2);
 
+        // TODO how to get an expression with the right datatypes eludes me ..
         // Validate null pruning
-        let batch = create_all_types_batch(5, 2, 0);
-        let partitions = vec![column.to_owned()];
-        let (_tmp, table) = prepare_table(vec![batch], SaveMode::Overwrite, partitions).await;
-
-        let e = col(column).is_null();
-        let metrics = get_scan_metrics(&table, &state, &[e]).await?;
-        assert_eq!(metrics.num_scanned_files(), 1);
+        // let batch = create_all_types_batch(5, 2, 0);
+        // let partitions = vec![column.to_owned()];
+        // let (_tmp, table) = prepare_table(vec![batch], SaveMode::Overwrite, partitions).await;
+
+        // let e = col(column).is_null();
+        // let metrics = get_scan_metrics(&table, &state, &[e]).await?;
+        // assert_eq!(metrics.num_scanned_files(), 1);
 
         /*  logically we should be able to prune the null partition but Datafusion's current implementation prevents this */
         /*
         let e = col(column).is_not_null();
         let metrics = get_scan_metrics(&table, &state, &[e]).await?;
         assert_eq!(metrics.num_scanned_files(), 5);
         */
@@ -658,37 +699,37 @@
     assert_eq!(metrics.num_scanned_files(), 1);
 
     let e = col("boolean").eq(lit(false));
     let metrics = get_scan_metrics(&table, &state, &[e]).await?;
     assert_eq!(metrics.num_scanned_files(), 1);
 
     // Ensure that tables without stats and partition columns can be pruned for just partitions
-    let table = deltalake::open_table("./tests/data/delta-0.8.0-null-partition").await?;
+    // let table = deltalake::open_table("./tests/data/delta-0.8.0-null-partition").await?;
 
     /*
     // Logically this should prune. See above
     let e = col("k").eq(lit("A")).and(col("k").is_not_null());
     let metrics = get_scan_metrics(&table, &state, &[e]).await.unwrap();
     println!("{:?}", metrics);
     assert!(metrics.num_scanned_files() == 1);
 
     let e = col("k").eq(lit("B"));
     let metrics = get_scan_metrics(&table, &state, &[e]).await?;
     assert!(metrics.num_scanned_files() == 1);
     */
 
     // Check pruning for null partitions
-    let e = col("k").is_null();
-    let metrics = get_scan_metrics(&table, &state, &[e]).await?;
-    assert!(metrics.num_scanned_files() == 1);
+    // let e = col("k").is_null();
+    // let metrics = get_scan_metrics(&table, &state, &[e]).await?;
+    // assert_eq!(metrics.num_scanned_files(), 1);
 
     // Check pruning for null partitions. Since there are no record count statistics pruning cannot be done
-    let e = col("k").is_not_null();
-    let metrics = get_scan_metrics(&table, &state, &[e]).await?;
-    assert!(metrics.num_scanned_files() == 2);
+    // let e = col("k").is_not_null();
+    // let metrics = get_scan_metrics(&table, &state, &[e]).await?;
+    // assert_eq!(metrics.num_scanned_files(), 2);
 
     Ok(())
 }
 
 #[tokio::test]
 async fn test_datafusion_partitioned_types() -> Result<()> {
     let ctx = SessionContext::new();
@@ -727,11 +768,108 @@
                 Box::new(ArrowDataType::UInt16),
                 Box::new(ArrowDataType::Utf8),
             ),
             false,
         ),
     ]);
 
-    assert_eq!(Arc::new(expected_schema), batches[0].schema());
+    assert_eq!(
+        Arc::new(expected_schema),
+        Arc::new(
+            batches[0]
+                .schema()
+                .as_ref()
+                .clone()
+                .with_metadata(Default::default())
+        )
+    );
+
+    Ok(())
+}
+
+#[tokio::test]
+async fn test_datafusion_scan_timestamps() -> Result<()> {
+    let ctx = SessionContext::new();
+    let table = deltalake::open_table("./tests/data/table_with_edge_timestamps")
+        .await
+        .unwrap();
+    ctx.register_table("demo", Arc::new(table))?;
+
+    let batches = ctx.sql("SELECT * FROM demo").await?.collect().await?;
+
+    let expected = vec![
+        "+-------------------------------+---------------------+------------+",
+        "| BIG_DATE                      | NORMAL_DATE         | SOME_VALUE |",
+        "+-------------------------------+---------------------+------------+",
+        "| 1816-03-28T05:56:08.066277376 | 2022-02-01T00:00:00 | 2          |",
+        "| 1816-03-29T05:56:08.066277376 | 2022-01-01T00:00:00 | 1          |",
+        "+-------------------------------+---------------------+------------+",
+    ];
+
+    assert_batches_sorted_eq!(&expected, &batches);
+
+    Ok(())
+}
+
+#[tokio::test]
+async fn test_issue_1292_datafusion_sql_projection() -> Result<()> {
+    let ctx = SessionContext::new();
+    let table = deltalake::open_table("./tests/data/http_requests")
+        .await
+        .unwrap();
+    ctx.register_table("http_requests", Arc::new(table))?;
+
+    let batches = ctx
+        .sql("SELECT \"ClientRequestURI\" FROM http_requests LIMIT 5")
+        .await?
+        .collect()
+        .await?;
+
+    let expected = vec![
+        "+------------------+",
+        "| ClientRequestURI |",
+        "+------------------+",
+        "| /                |",
+        "| /                |",
+        "| /                |",
+        "| /                |",
+        "| /                |",
+        "+------------------+",
+    ];
+
+    assert_batches_sorted_eq!(&expected, &batches);
+
+    Ok(())
+}
+
+#[tokio::test]
+async fn test_issue_1291_datafusion_sql_partitioned_data() -> Result<()> {
+    let ctx = SessionContext::new();
+    let table = deltalake::open_table("./tests/data/http_requests")
+        .await
+        .unwrap();
+    ctx.register_table("http_requests", Arc::new(table))?;
+
+    let batches = ctx
+        .sql(
+            "SELECT \"ClientRequestURI\", date FROM http_requests WHERE date > '2023-04-13' LIMIT 5",
+        )
+        .await?
+        .collect()
+        .await?;
+
+    let expected = vec![
+        "+------------------+------------+",
+        "| ClientRequestURI | date       |",
+        "+------------------+------------+",
+        "| /                | 2023-04-14 |",
+        "| /                | 2023-04-14 |",
+        "| /                | 2023-04-14 |",
+        "| /                | 2023-04-14 |",
+        "| /                | 2023-04-14 |",
+        "+------------------+------------+",
+    ];
+
+    assert_batches_sorted_eq!(&expected, &batches);
 
     Ok(())
 }
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/fs_common/mod.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/fs_common/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#![allow(deprecated)]
 use chrono::Utc;
 use deltalake::action::{Action, Add, Protocol, Remove};
 use deltalake::{
     builder::DeltaTableBuilder, DeltaTable, DeltaTableMetaData, Schema, SchemaDataType, SchemaField,
 };
 use serde_json::Value;
 use std::collections::HashMap;
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/integration_checkpoint.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/integration_checkpoint.rs`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,23 @@
 #[serial]
 async fn cleanup_metadata_gcp_test() -> TestResult {
     let context = IntegrationContext::new(StorageIntegration::Google)?;
     cleanup_metadata_test(&context).await?;
     Ok(())
 }
 
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+#[serial]
+async fn cleanup_metadata_hdfs_test() -> TestResult {
+    let context = IntegrationContext::new(StorageIntegration::Hdfs)?;
+    cleanup_metadata_test(&context).await?;
+    Ok(())
+}
+
 // Last-Modified for S3 could not be altered by user, hence using system pauses which makes
 // test to run longer but reliable
 async fn cleanup_metadata_test(context: &IntegrationContext) -> TestResult {
     let table_uri = context.root_uri();
     let object_store = DeltaTableBuilder::from_uri(table_uri)
         .with_allow_http(true)
         .build_storage()?;
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/integration_commit.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/integration_commit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,21 @@
 #[cfg(feature = "gcs")]
 #[tokio::test]
 #[serial]
 async fn test_commit_tables_gcp() {
     commit_tables(StorageIntegration::Google).await.unwrap();
 }
 
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+#[serial]
+async fn test_commit_tables_hdfs() {
+    commit_tables(StorageIntegration::Hdfs).await.unwrap();
+}
+
 #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
 #[tokio::test]
 #[serial]
 async fn test_two_commits_s3_fails_with_no_lock() -> TestResult {
     std::env::set_var("AWS_S3_LOCKING_PROVIDER", "none  ");
     let context = IntegrationContext::new(StorageIntegration::Amazon)?;
     context.load_table(TestTables::SimpleCommit).await?;
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/integration_datafusion.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/integration_datafusion.rs`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 #[cfg(feature = "gcs")]
 #[tokio::test]
 #[serial]
 async fn test_datafusion_gcp() -> TestResult {
     Ok(test_datafusion(StorageIntegration::Google).await?)
 }
 
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+#[serial]
+async fn test_datafusion_hdfs() -> TestResult {
+    Ok(test_datafusion(StorageIntegration::Hdfs).await?)
+}
+
 async fn test_datafusion(storage: StorageIntegration) -> TestResult {
     let context = IntegrationContext::new(storage)?;
     context.load_table(TestTables::Simple).await?;
 
     simple_query(&context).await?;
 
     Ok(())
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/integration_object_store.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/integration_object_store.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![cfg(feature = "integration_test")]
 
 use bytes::Bytes;
 use deltalake::storage::utils::flatten_list_stream;
 use deltalake::test_utils::{IntegrationContext, StorageIntegration, TestResult};
-use deltalake::DeltaTableBuilder;
+use deltalake::{DeltaTableBuilder, ObjectStore};
 use object_store::{path::Path, DynObjectStore, Error as ObjectStoreError};
 use serial_test::serial;
 
 #[tokio::test]
 #[serial]
 async fn test_object_store_local() -> TestResult {
     test_object_store(StorageIntegration::Local, false).await?;
@@ -18,14 +18,15 @@
 #[tokio::test]
 #[serial]
 async fn test_object_store_azure() -> TestResult {
     test_object_store(StorageIntegration::Microsoft, false).await?;
     Ok(())
 }
 
+#[cfg(feature = "s3")]
 #[tokio::test]
 #[serial]
 async fn test_object_store_aws() -> TestResult {
     test_object_store(StorageIntegration::Amazon, true).await?;
     Ok(())
 }
 
@@ -35,14 +36,22 @@
 #[tokio::test]
 #[serial]
 async fn test_object_store_google() -> TestResult {
     test_object_store(StorageIntegration::Google, false).await?;
     Ok(())
 }
 
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+#[serial]
+async fn test_object_store_hdfs() -> TestResult {
+    test_object_store(StorageIntegration::Hdfs, false).await?;
+    Ok(())
+}
+
 async fn test_object_store(integration: StorageIntegration, skip_copy: bool) -> TestResult {
     let context = IntegrationContext::new(integration)?;
     let delta_store = DeltaTableBuilder::from_uri(&context.root_uri())
         .with_allow_http(true)
         .build_storage()?;
 
     put_get_delete_list(delta_store.as_ref()).await?;
@@ -403,7 +412,33 @@
     let paths = flatten_list_stream(storage, None).await?;
 
     for f in &paths {
         let _ = storage.delete(f).await?;
     }
     Ok(())
 }
+
+#[tokio::test]
+#[serial]
+async fn test_object_store_prefixes_local() -> TestResult {
+    test_object_store_prefixes(StorageIntegration::Local).await?;
+    Ok(())
+}
+
+async fn test_object_store_prefixes(integration: StorageIntegration) -> TestResult {
+    let context = IntegrationContext::new(integration)?;
+    let prefixes = &["table path", "table path/hello%3F", "你好/😊"];
+    for prefix in prefixes {
+        let rooturi = format!("{}/{}", context.root_uri(), prefix);
+        let delta_store = DeltaTableBuilder::from_uri(&rooturi)
+            .with_allow_http(true)
+            .build_storage()?;
+
+        let contents = Bytes::from("cats");
+        let path = Path::from("test");
+        delta_store.put(&path, contents.clone()).await?;
+        let data = delta_store.get(&path).await?.bytes().await?;
+        assert_eq!(&data, &contents);
+    }
+
+    Ok(())
+}
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/integration_read.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/integration_read.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,133 @@
 #![cfg(feature = "integration_test")]
 
 use deltalake::test_utils::{IntegrationContext, StorageIntegration, TestResult, TestTables};
-use deltalake::DeltaTableBuilder;
+use deltalake::{DeltaTableBuilder, ObjectStore};
 #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
 use dynamodb_lock::dynamo_lock_options;
 #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
 use maplit::hashmap;
 use object_store::path::Path;
 use serial_test::serial;
 
+static TEST_PREFIXES: &[&str] = &["my table", "你好/😊"];
+
+/// TEST_PREFIXES as they should appear in object stores.
+static TEST_PREFIXES_ENCODED: &[&str] = &["my%20table", "%E4%BD%A0%E5%A5%BD/%F0%9F%98%8A"];
+
 #[tokio::test]
 #[serial]
 async fn test_read_tables_local() -> TestResult {
-    Ok(read_tables(StorageIntegration::Local).await?)
+    read_tables(StorageIntegration::Local).await?;
+
+    for prefix in TEST_PREFIXES {
+        read_table_paths(StorageIntegration::Local, prefix, prefix).await?;
+    }
+
+    Ok(())
 }
 
 #[cfg(feature = "azure")]
 #[tokio::test]
 #[serial]
 async fn test_read_tables_azure() -> TestResult {
-    Ok(read_tables(StorageIntegration::Microsoft).await?)
+    read_tables(StorageIntegration::Microsoft).await?;
+
+    for (prefix, prefix_encoded) in TEST_PREFIXES.iter().zip(TEST_PREFIXES_ENCODED.iter()) {
+        read_table_paths(StorageIntegration::Microsoft, prefix, prefix_encoded).await?;
+    }
+
+    Ok(())
+}
+
+#[cfg(feature = "hdfs")]
+#[tokio::test]
+#[serial]
+async fn test_read_tables_hdfs() -> TestResult {
+    Ok(read_tables(StorageIntegration::Hdfs).await?)
 }
 
 #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
 #[tokio::test]
 #[serial]
 async fn test_read_tables_aws() -> TestResult {
-    Ok(read_tables(StorageIntegration::Amazon).await?)
+    read_tables(StorageIntegration::Amazon).await?;
+
+    for (prefix, prefix_encoded) in TEST_PREFIXES.iter().zip(TEST_PREFIXES_ENCODED.iter()) {
+        read_table_paths(StorageIntegration::Amazon, prefix, prefix_encoded).await?;
+    }
+
+    Ok(())
 }
 
 async fn read_tables(storage: StorageIntegration) -> TestResult {
     let context = IntegrationContext::new(storage)?;
     context.load_table(TestTables::Simple).await?;
     context.load_table(TestTables::Golden).await?;
+    context
+        .load_table(TestTables::Delta0_8_0SpecialPartitioned)
+        .await?;
 
     read_simple_table(&context).await?;
     read_simple_table_with_version(&context).await?;
     read_golden(&context).await?;
 
     Ok(())
 }
 
+async fn read_table_paths(
+    storage: StorageIntegration,
+    table_root: &str,
+    upload_path: &str,
+) -> TestResult {
+    let context = IntegrationContext::new(storage)?;
+    context
+        .load_table_with_name(TestTables::Delta0_8_0SpecialPartitioned, upload_path)
+        .await?;
+
+    verify_store(&context, table_root).await?;
+
+    read_encoded_table(&context, table_root).await?;
+
+    Ok(())
+}
+
+async fn verify_store(integration: &IntegrationContext, root_path: &str) -> TestResult {
+    let table_uri = format!("{}/{}", integration.root_uri(), root_path);
+    let storage = DeltaTableBuilder::from_uri(table_uri.clone())
+        .with_allow_http(true)
+        .build_storage()?;
+
+    let files = storage.list_with_delimiter(None).await?;
+    assert_eq!(
+        vec![
+            Path::parse("_delta_log").unwrap(),
+            Path::parse("x=A%2FA").unwrap(),
+            Path::parse("x=B%20B").unwrap(),
+        ],
+        files.common_prefixes
+    );
+
+    Ok(())
+}
+
+async fn read_encoded_table(integration: &IntegrationContext, root_path: &str) -> TestResult {
+    let table_uri = format!("{}/{}", integration.root_uri(), root_path);
+
+    let table = DeltaTableBuilder::from_uri(table_uri)
+        .with_allow_http(true)
+        .load()
+        .await?;
+
+    assert_eq!(table.version(), 0);
+    assert_eq!(table.get_files().len(), 2);
+
+    Ok(())
+}
+
 async fn read_simple_table(integration: &IntegrationContext) -> TestResult {
     let table_uri = integration.uri_for_table(TestTables::Simple);
     // the s3 options don't hurt us for other integrations ...
     #[cfg(any(feature = "s3", feature = "s3-native-tls"))]
     let table = DeltaTableBuilder::from_uri(table_uri).with_allow_http(true).with_storage_options(hashmap! {
         dynamo_lock_options::DYNAMO_LOCK_OWNER_NAME.to_string() => "s3::deltars/simple".to_string(),
     }).load().await?;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/read_delta_partitions_test.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/read_delta_partitions_test.rs`

 * *Files 16% similar despite different names*

```diff
@@ -143,7 +143,31 @@
         .join("00000000000000000002.checkpoint.parquet");
     assert!(cp.exists());
 
     // verify that table loads from checkpoint and handles null partitions
     let table = deltalake::open_table(&table.table_uri()).await.unwrap();
     assert_eq!(table.version(), 2);
 }
+
+#[cfg(feature = "datafusion")]
+#[tokio::test]
+async fn load_from_delta_8_0_table_with_special_partition() {
+    use datafusion::physical_plan::SendableRecordBatchStream;
+    use deltalake::{DeltaOps, DeltaTable};
+    use futures::{future, StreamExt};
+
+    let table = deltalake::open_table("./tests/data/delta-0.8.0-special-partition")
+        .await
+        .unwrap();
+
+    let (_, stream): (DeltaTable, SendableRecordBatchStream) = DeltaOps(table)
+        .load()
+        .with_columns(vec!["x", "y"])
+        .await
+        .unwrap();
+    stream
+        .for_each(|batch| {
+            assert!(batch.is_ok());
+            future::ready(())
+        })
+        .await;
+}
```

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/read_delta_test.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/read_delta_test.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/repair_s3_rename_test.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/repair_s3_rename_test.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/local_dependencies/deltalake/tests/time_travel.rs` & `deltalake-0.9.0/local_dependencies/deltalake/tests/time_travel.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/Cargo.toml` & `deltalake-0.9.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "deltalake-python"
-version = "0.8.1"
+version = "0.9.0"
 authors = ["Qingping Hou <dave2008713@gmail.com>"]
 homepage = "https://github.com/delta-io/delta-rs"
 license = "Apache-2.0"
 description = "Native Delta Lake Python binding based on delta-rs with Pandas integration"
 readme = "README.md"
 edition = "2021"
 keywords = ["deltalake", "delta", "datalake", "pandas", "arrow"]
@@ -14,15 +14,15 @@
 crate-type = ["cdylib"]
 doc = false
 
 [package.metadata.maturin]
 name = "deltalake._internal"
 
 [dependencies]
-arrow-schema = { version = "33", features = ["serde"] }
+arrow-schema = { version = "36", features = ["serde"] }
 chrono = "0"
 env_logger = "0"
 futures = "0.3"
 lazy_static = "1"
 regex = "1"
 serde = "1"
 serde_json = "1"
@@ -35,13 +35,13 @@
 [dependencies.pyo3]
 version = "0.18"
 features = ["extension-module", "abi3", "abi3-py37"]
 
 [dependencies.deltalake]
 path = "local_dependencies/deltalake"
 version = "0"
-features = ["azure", "gcs", "python", "datafusion"]
+features = ["azure", "gcs", "python", "datafusion", "unity-experimental"]
 
 [features]
 default = ["rustls"]
 native-tls = ["deltalake/s3-native-tls", "deltalake/glue-native-tls"]
 rustls = ["deltalake/s3", "deltalake/glue"]
```

### Comparing `deltalake-0.8.1/CONTRIBUTING.md` & `deltalake-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/LICENSE.txt` & `deltalake-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/Makefile` & `deltalake-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/README.md` & `deltalake-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/deltalake/_internal.pyi` & `deltalake-0.9.0/deltalake/_internal.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     from typing_extensions import Literal
 
 import pyarrow as pa
 import pyarrow.fs as fs
 
 from deltalake.writer import AddAction
 
+__version__: str
+
 RawDeltaTable: Any
 rust_core_version: Callable[[], str]
 
 class PyDeltaTableError(BaseException): ...
 
 write_new_deltalake: Callable[
     [
@@ -122,15 +124,15 @@
     def __init__(self, fields: List[Field]) -> None: ...
     fields: List[Field]
     invariants: List[Tuple[str, str]]
 
     def to_json(self) -> str: ...
     @staticmethod
     def from_json(json: str) -> "Schema": ...
-    def to_pyarrow(self) -> pa.Schema: ...
+    def to_pyarrow(self, as_large_types: bool = False) -> pa.Schema: ...
     @staticmethod
     def from_pyarrow(type: pa.Schema) -> "Schema": ...
 
 class ObjectInputFile:
     @property
     def closed(self) -> bool: ...
     @property
```

### Comparing `deltalake-0.8.1/deltalake/fs.py` & `deltalake-0.9.0/deltalake/fs.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/deltalake/schema.py` & `deltalake-0.9.0/deltalake/schema.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/deltalake/table.py` & `deltalake-0.9.0/deltalake/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -309,14 +309,38 @@
         """
         if retention_hours:
             if retention_hours < 0:
                 raise ValueError("The retention periods should be positive.")
 
         return self._table.vacuum(dry_run, retention_hours, enforce_retention_duration)
 
+    def optimize(
+        self,
+        partition_filters: Optional[List[Tuple[str, str, Any]]] = None,
+        target_size: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Compacts small files to reduce the total number of files in the table.
+
+        This operation is idempotent; if run twice on the same table (assuming it has
+        not been updated) it will do nothing the second time.
+
+        If this operation happens concurrently with any operations other than append,
+        it will fail.
+
+        :param partition_filters: the partition filters that will be used for getting the matched files
+        :param target_size: desired file size after bin-packing files, in bytes. If not
+          provided, will attempt to read the table configuration value ``delta.targetFileSize``.
+          If that value isn't set, will use default value of 256MB.
+        :return: the metrics from optimize
+        """
+        metrics = self._table.optimize(partition_filters, target_size)
+        self.update_incremental()
+        return json.loads(metrics)
+
     def pyarrow_schema(self) -> pyarrow.Schema:
         """
         Get the current schema of the DeltaTable with the Parquet PyArrow format.
 
         DEPRECATED: use DeltaTable.schema().to_pyarrow() instead.
 
         :return: the current Schema with the Parquet PyArrow format
@@ -461,19 +485,19 @@
         Examples:
 
         >>> from deltalake import DeltaTable, write_deltalake
         >>> import pyarrow as pa
         >>> data = pa.table({"x": [1, 2, 3], "y": [4, 5, 6]})
         >>> write_deltalake("tmp", data, partition_by=["x"])
         >>> dt = DeltaTable("tmp")
-        >>> dt.get_add_actions_df().to_pandas()
+        >>> dt.get_add_actions().to_pandas()
                                                                 path  size_bytes       modification_time  data_change partition_values  num_records null_count       min       max
         0  x=2/0-91820cbf-f698-45fb-886d-5d5f5669530b-0.p...         565 1970-01-20 08:40:08.071         True         {'x': 2}            1   {'y': 0}  {'y': 5}  {'y': 5}
         1  x=3/0-91820cbf-f698-45fb-886d-5d5f5669530b-0.p...         565 1970-01-20 08:40:08.071         True         {'x': 3}            1   {'y': 0}  {'y': 6}  {'y': 6}
         2  x=1/0-91820cbf-f698-45fb-886d-5d5f5669530b-0.p...         565 1970-01-20 08:40:08.071         True         {'x': 1}            1   {'y': 0}  {'y': 4}  {'y': 4}
-        >>> dt.get_add_actions_df(flatten=True).to_pandas()
+        >>> dt.get_add_actions(flatten=True).to_pandas()
                                                                 path  size_bytes       modification_time  data_change  partition.x  num_records  null_count.y  min.y  max.y
         0  x=2/0-91820cbf-f698-45fb-886d-5d5f5669530b-0.p...         565 1970-01-20 08:40:08.071         True            2            1             0      5      5
         1  x=3/0-91820cbf-f698-45fb-886d-5d5f5669530b-0.p...         565 1970-01-20 08:40:08.071         True            3            1             0      6      6
         2  x=1/0-91820cbf-f698-45fb-886d-5d5f5669530b-0.p...         565 1970-01-20 08:40:08.071         True            1            1             0      4      4
         """
         return self._table.get_add_actions(flatten)
```

### Comparing `deltalake-0.8.1/deltalake/writer.py` & `deltalake-0.9.0/deltalake/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,19 @@
         pa.Table,
         pa.RecordBatch,
         Iterable[pa.RecordBatch],
         RecordBatchReader,
     ],
     *,
     schema: Optional[pa.Schema] = None,
-    partition_by: Optional[List[str]] = None,
+    partition_by: Optional[Union[List[str], str]] = None,
     filesystem: Optional[pa_fs.FileSystem] = None,
     mode: Literal["error", "append", "overwrite", "ignore"] = "error",
     file_options: Optional[ds.ParquetFileWriteOptions] = None,
+    max_partitions: Optional[int] = None,
     max_open_files: int = 1024,
     max_rows_per_file: int = 10 * 1024 * 1024,
     min_rows_per_group: int = 64 * 1024,
     max_rows_per_group: int = 128 * 1024,
     name: Optional[str] = None,
     description: Optional[str] = None,
     configuration: Optional[Mapping[str, Optional[str]]] = None,
@@ -110,14 +111,15 @@
         If 'append', will add new data.
         If 'overwrite', will replace table with new data.
         If 'ignore', will not write anything if table already exists.
     :param file_options: Optional write options for Parquet (ParquetFileWriteOptions).
         Can be provided with defaults using ParquetFileWriteOptions().make_write_options().
         Please refer to https://github.com/apache/arrow/blob/master/python/pyarrow/_dataset_parquet.pyx#L492-L533
         for the list of available options
+    :param max_partitions: the maximum number of partitions that will be used.
     :param max_open_files: Limits the maximum number of
         files that can be left open while writing. If an attempt is made to open
         too many files then the least recently used file will be closed.
         If this setting is set too low you may end up fragmenting your
         data into many small files.
     :param max_rows_per_file: Maximum number of rows per file.
         If greater than 0 then this will limit how many rows are placed in any single file.
@@ -140,14 +142,18 @@
         if schema is not None:
             data = pa.Table.from_pandas(data, schema=schema)
         else:
             data, schema = delta_arrow_schema_from_pandas(data)
 
     table, table_uri = try_get_table_and_table_uri(table_or_uri, storage_options)
 
+    # We need to write against the latest table version
+    if table:
+        table.update_incremental()
+
     if schema is None:
         if isinstance(data, RecordBatchReader):
             schema = data.schema
         elif isinstance(data, Iterable):
             raise ValueError("You must provide schema if data is Iterable")
         else:
             schema = data.schema
@@ -160,14 +166,17 @@
     if filesystem is None:
         if table is not None:
             storage_options = table._storage_options or {}
             storage_options.update(storage_options or {})
 
         filesystem = pa_fs.PyFileSystem(DeltaStorageHandler(table_uri, storage_options))
 
+    if isinstance(partition_by, str):
+        partition_by = [partition_by]
+
     if table:  # already exists
         if schema != table.schema().to_pyarrow() and not (
             mode == "overwrite" and overwrite_schema
         ):
             raise ValueError(
                 "Schema of data does not match table schema\n"
                 f"Table schema:\n{schema}\nData Schema:\n{table.schema().to_pyarrow()}"
@@ -302,14 +311,15 @@
         existing_data_behavior="overwrite_or_ignore",
         file_options=file_options,
         max_open_files=max_open_files,
         max_rows_per_file=max_rows_per_file,
         min_rows_per_group=min_rows_per_group,
         max_rows_per_group=max_rows_per_group,
         filesystem=filesystem,
+        max_partitions=max_partitions,
     )
 
     if table is None:
         _write_new_deltalake(
             table_uri,
             schema,
             add_actions,
@@ -324,14 +334,15 @@
         table._table.create_write_transaction(
             add_actions,
             mode,
             partition_by or [],
             schema,
             partition_filters,
         )
+        table.update_incremental()
 
 
 def __enforce_append_only(
     table: Optional[DeltaTable],
     configuration: Optional[Mapping[str, Optional[str]]],
     mode: str,
 ) -> None:
```

### Comparing `deltalake-0.8.1/docs/Makefile` & `deltalake-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/docs/make.bat` & `deltalake-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/docs/source/_ext/edit_on_github.py` & `deltalake-0.9.0/docs/source/_ext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/docs/source/api_reference.rst` & `deltalake-0.9.0/docs/source/api_reference.rst`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/docs/source/conf.py` & `deltalake-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/docs/source/index.rst` & `deltalake-0.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/docs/source/usage.rst` & `deltalake-0.9.0/docs/source/usage.rst`

 * *Files 10% similar despite different names*

```diff
@@ -51,29 +51,42 @@
   * abfs://<container>/<path>
 
 **GCS**:
 
   * gs://<bucket>/<path>
 
 Alternatively, if you have a data catalog you can load it by reference to a 
-database and table name. Currently only AWS Glue is supported.
+database and table name. Currently supported are AWS Glue and Databricks Unity Catalog.
 
 For AWS Glue catalog, use AWS environment variables to authenticate.
 
 .. code-block:: python
 
     >>> from deltalake import DeltaTable
     >>> from deltalake import DataCatalog
     >>> database_name = "simple_database"
     >>> table_name = "simple_table"
     >>> data_catalog = DataCatalog.AWS
     >>> dt = DeltaTable.from_data_catalog(data_catalog=data_catalog, database_name=database_name, table_name=table_name)
     >>> dt.to_pyarrow_table().to_pydict()
     {'id': [5, 7, 9, 5, 6, 7, 8, 9]}
 
+For Databricks Unity Catalog authentication, use environment variables:
+  * DATABRICKS_WORKSPACE_URL (e.g. https://adb-62800498333851.30.azuredatabricks.net)
+  * DATABRICKS_ACCESS_TOKEN
+
+.. code-block:: python
+
+   >>> from deltalake import DataCatalog, DeltaTable
+   >>> catalog_name = 'main'
+   >>> schema_name = 'db_schema'
+   >>> table_name = 'db_table'
+   >>> data_catalog = DataCatalog.UNITY
+   >>> dt = DeltaTable.from_data_catalog(data_catalog=data_catalog, data_catalog_id=catalog_name, database_name=schema_name, table_name=table_name)
+
 .. _`s3 options`: https://docs.rs/object_store/latest/object_store/aws/enum.AmazonS3ConfigKey.html#variants
 .. _`azure options`: https://docs.rs/object_store/latest/object_store/azure/enum.AzureConfigKey.html#variants
 .. _`gcs options`: https://docs.rs/object_store/latest/object_store/gcp/enum.GoogleConfigKey.html#variants
 
 Custom Storage Backends
 ~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -141,15 +154,15 @@
 ~~~~~~~~
 
 The delta log maintains basic metadata about a table, including:
 
 * A unique ``id``
 * A ``name``, if provided
 * A ``description``, if provided
-* The list of ``partitionColumns``.
+* The list of ``partition_columns``.
 * The ``created_time`` of the table
 * A map of table ``configuration``. This includes fields such as ``delta.appendOnly``,
   which if ``true`` indicates the table is not meant to have data deleted from it.
 
 Get metadata from a table with the :meth:`DeltaTable.metadata` method:
 
 .. code-block:: python
@@ -395,15 +408,31 @@
      '../rust/tests/data/simple_table/part-00164-bf40481c-4afd-4c02-befa-90f056c2d77a-c000.snappy.parquet',
      ...]
     >>> dt.vacuum(dry_run=False) # Don't run this unless you are sure!
 
 Optimizing tables
 ~~~~~~~~~~~~~~~~~
 
-Optimizing tables is not currently supported.
+Optimizing a table will perform bin-packing on a Delta Table which merges small files
+into a large file. Bin-packing reduces the number of API calls required for read operations.
+Optimizing will increments the table's version and creates remove actions for optimized files.
+Optimize does not delete files from storage. To delete files that were removed, call :meth:`DeltaTable.vacuum`.
+
+Use :meth:`DeltaTable.optimize` to perform the optimize operation. Note that this method will fail if a
+concurrent writer performs an operation that removes any files (such as an overwrite).
+
+.. code-block:: python
+
+    >>> dt = DeltaTable("../rust/tests/data/simple_table")
+    >>> dt.optimize()
+    {'numFilesAdded': 1, 'numFilesRemoved': 5,
+     'filesAdded': {'min': 555, 'max': 555, 'avg': 555.0, 'totalFiles': 1, 'totalSize': 555},
+     'filesRemoved': {'min': 262, 'max': 429, 'avg': 362.2, 'totalFiles': 5, 'totalSize': 1811},
+     'partitionsOptimized': 1, 'numBatches': 1, 'totalConsideredFiles': 5,
+     'totalFilesSkipped': 0, 'preserveInsertionOrder': True}
 
 Writing Delta Tables
 --------------------
 
 .. py:currentmodule:: deltalake
 
 For overwrites and appends, use :py:func:`write_deltalake`. If the table does not
```

### Comparing `deltalake-0.8.1/pyproject.toml` & `deltalake-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 dependencies = [
     "pyarrow>=7",
     'typing-extensions;python_version<"3.8"',
 ]
 
 [project.optional-dependencies]
 pandas = [
-    "pandas"
+    "pandas<2"
 ]
 devel = [
     "mypy",
     "black",
     "ruff",
     "packaging>=20",
     "pytest",
```

### Comparing `deltalake-0.8.1/src/filesystem.rs` & `deltalake-0.9.0/src/filesystem.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/src/lib.rs` & `deltalake-0.9.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 use deltalake::arrow::compute::concat_batches;
 use deltalake::arrow::record_batch::RecordBatch;
 use deltalake::arrow::{self, datatypes::Schema as ArrowSchema};
 use deltalake::builder::DeltaTableBuilder;
 use deltalake::checkpoints::create_checkpoint;
 use deltalake::datafusion::prelude::SessionContext;
 use deltalake::delta_datafusion::DeltaDataChecker;
+use deltalake::operations::optimize::OptimizeBuilder;
+use deltalake::operations::transaction::commit;
 use deltalake::operations::vacuum::VacuumBuilder;
 use deltalake::partitions::PartitionFilter;
 use deltalake::{
-    DeltaDataTypeLong, DeltaDataTypeTimestamp, DeltaTableMetaData, DeltaTransactionOptions,
-    Invariant, Schema,
+    DeltaConfigKey, DeltaDataTypeLong, DeltaDataTypeTimestamp, DeltaOps, Invariant, Schema,
 };
 use pyo3::create_exception;
 use pyo3::exceptions::PyException;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::PyFrozenSet;
 use pyo3::types::PyType;
 use std::collections::HashMap;
 use std::collections::HashSet;
 use std::convert::TryFrom;
+use std::future::IntoFuture;
+use std::str::FromStr;
 use std::sync::Arc;
 use std::time::SystemTime;
 use std::time::UNIX_EPOCH;
 
 use crate::filesystem::FsConfig;
 use crate::schema::schema_to_pyobject;
 
@@ -308,37 +311,47 @@
         let (table, metrics) = rt()?
             .block_on(async { cmd.await })
             .map_err(PyDeltaTableError::from_raw)?;
         self._table.state = table.state;
         Ok(metrics.files_deleted)
     }
 
+    // Run the optimize command on the Delta Table: merge small files into a large file by bin-packing.
+    #[pyo3(signature = (partition_filters = None, target_size = None))]
+    pub fn optimize(
+        &mut self,
+        partition_filters: Option<Vec<(&str, &str, PartitionFilterValue)>>,
+        target_size: Option<DeltaDataTypeLong>,
+    ) -> PyResult<String> {
+        let mut cmd = OptimizeBuilder::new(self._table.object_store(), self._table.state.clone());
+        if let Some(size) = target_size {
+            cmd = cmd.with_target_size(size);
+        }
+        let converted_filters = convert_partition_filters(partition_filters.unwrap_or_default())
+            .map_err(PyDeltaTableError::from_raw)?;
+        cmd = cmd.with_filters(&converted_filters);
+
+        let (table, metrics) = rt()?
+            .block_on(async { cmd.await })
+            .map_err(PyDeltaTableError::from_raw)?;
+        self._table.state = table.state;
+        Ok(serde_json::to_string(&metrics).unwrap())
+    }
+
     // Run the History command on the Delta Table: Returns provenance information, including the operation, user, and so on, for each write to a table.
     pub fn history(&mut self, limit: Option<usize>) -> PyResult<Vec<String>> {
         let history = rt()?
             .block_on(self._table.history(limit))
             .map_err(PyDeltaTableError::from_raw)?;
         Ok(history
             .iter()
             .map(|c| serde_json::to_string(c).unwrap())
             .collect())
     }
 
-    pub fn arrow_schema_json(&self) -> PyResult<String> {
-        let schema = self
-            ._table
-            .get_schema()
-            .map_err(PyDeltaTableError::from_raw)?;
-        serde_json::to_string(
-            &<ArrowSchema as TryFrom<&deltalake::Schema>>::try_from(schema)
-                .map_err(PyDeltaTableError::from_arrow)?,
-        )
-        .map_err(|_| PyDeltaTableError::new_err("Got invalid table schema"))
-    }
-
     pub fn update_incremental(&mut self) -> PyResult<()> {
         rt()?
             .block_on(self._table.update_incremental(None))
             .map_err(PyDeltaTableError::from_raw)
     }
 
     pub fn dataset_partitions<'py>(
@@ -375,17 +388,15 @@
         &self,
         partitions_filters: Option<Vec<(&str, &str, PartitionFilterValue)>>,
         py: Python<'py>,
     ) -> PyResult<&'py PyFrozenSet> {
         let column_names: HashSet<&str> = self
             ._table
             .schema()
-            .ok_or(PyDeltaTableError::new_err(
-                "table does not yet have a schema",
-            ))?
+            .ok_or_else(|| PyDeltaTableError::new_err("table does not yet have a schema"))?
             .get_fields()
             .iter()
             .map(|field| field.get_name())
             .collect();
         let partition_columns: HashSet<&str> = self
             ._table
             .get_metadata()
@@ -510,25 +521,27 @@
                 // This should be unreachable from Python
                 if &schema != existing_schema {
                     PyDeltaTableError::new_err("Cannot change schema except in overwrite.");
                 }
             }
         }
 
-        let mut transaction = self
-            ._table
-            .create_transaction(Some(DeltaTransactionOptions::new(3)));
-        transaction.add_actions(actions);
+        let operation = DeltaOperation::Write {
+            mode,
+            partition_by: Some(partition_by),
+            predicate: None,
+        };
+        let store = self._table.object_store();
+
         rt()?
-            .block_on(transaction.commit(
-                Some(DeltaOperation::Write {
-                    mode,
-                    partition_by: Some(partition_by),
-                    predicate: None,
-                }),
+            .block_on(commit(
+                &*store,
+                &actions,
+                operation,
+                self._table.get_state(),
                 None,
             ))
             .map_err(PyDeltaTableError::from_raw)?;
 
         Ok(())
     }
 
@@ -750,41 +763,53 @@
     _mode: &str,
     partition_by: Vec<String>,
     name: Option<String>,
     description: Option<String>,
     configuration: Option<HashMap<String, Option<String>>>,
     storage_options: Option<HashMap<String, String>>,
 ) -> PyResult<()> {
-    let mut table = DeltaTableBuilder::from_uri(table_uri)
+    let table = DeltaTableBuilder::from_uri(table_uri)
         .with_storage_options(storage_options.unwrap_or_default())
         .build()
         .map_err(PyDeltaTableError::from_raw)?;
 
-    let metadata = DeltaTableMetaData::new(
-        name,
-        description,
-        None, // Format
-        (&schema.0)
-            .try_into()
-            .map_err(PyDeltaTableError::from_arrow)?,
-        partition_by,
-        configuration.unwrap_or_default(),
-    );
-
-    let fut = table.create(
-        metadata,
-        action::Protocol {
-            min_reader_version: 1,
-            min_writer_version: 1, // TODO: Make sure we comply with protocol
-        },
-        None, // TODO
-        Some(add_actions.iter().map(|add| add.into()).collect()),
-    );
+    let schema: Schema = (&schema.0)
+        .try_into()
+        .map_err(PyDeltaTableError::from_arrow)?;
 
-    rt()?.block_on(fut).map_err(PyDeltaTableError::from_raw)?;
+    let configuration = configuration
+        .unwrap_or_default()
+        .into_iter()
+        .filter_map(|(key, value)| {
+            if let Ok(key) = DeltaConfigKey::from_str(&key) {
+                Some((key, value))
+            } else {
+                None
+            }
+        })
+        .collect();
+
+    let mut builder = DeltaOps(table)
+        .create()
+        .with_columns(schema.get_fields().clone())
+        .with_partition_columns(partition_by)
+        .with_configuration(configuration)
+        .with_actions(add_actions.iter().map(|add| Action::add(add.into())));
+
+    if let Some(name) = &name {
+        builder = builder.with_table_name(name);
+    };
+
+    if let Some(description) = &description {
+        builder = builder.with_comment(description);
+    };
+
+    rt()?
+        .block_on(builder.into_future())
+        .map_err(PyDeltaTableError::from_raw)?;
 
     Ok(())
 }
 
 #[pyclass(name = "DeltaDataChecker", text_signature = "(invariants)")]
 struct PyDeltaDataChecker {
     inner: DeltaDataChecker,
@@ -818,15 +843,15 @@
     }
 }
 
 #[pymodule]
 // module name need to match project name
 fn _internal(py: Python, m: &PyModule) -> PyResult<()> {
     env_logger::Builder::from_env(env_logger::Env::default().default_filter_or("warn")).init();
-
+    m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add_function(pyo3::wrap_pyfunction!(rust_core_version, m)?)?;
     m.add_function(pyo3::wrap_pyfunction!(write_new_deltalake, m)?)?;
     m.add_function(pyo3::wrap_pyfunction!(batch_distinct, m)?)?;
     m.add_class::<RawDeltaTable>()?;
     m.add_class::<RawDeltaTableMetaData>()?;
     m.add_class::<PyDeltaDataChecker>()?;
     m.add("PyDeltaTableError", py.get_type::<PyDeltaTableError>())?;
```

### Comparing `deltalake-0.8.1/src/schema.rs` & `deltalake-0.9.0/src/schema.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 extern crate pyo3;
 
 use deltalake::arrow::datatypes::{
-    DataType as ArrowDataType, Field as ArrowField, Schema as ArrowSchema,
+    DataType as ArrowDataType, Field as ArrowField, FieldRef as ArrowFieldRef,
+    Schema as ArrowSchema,
 };
 use deltalake::arrow::error::ArrowError;
 use deltalake::arrow::pyarrow::PyArrowType;
 use deltalake::schema::{
     Schema, SchemaDataType, SchemaField, SchemaTypeArray, SchemaTypeMap, SchemaTypeStruct,
 };
 use lazy_static::lazy_static;
@@ -946,15 +947,15 @@
 /// Schema([Field(x, PrimitiveType("integer"), nullable=True), Field(y, PrimitiveType("string"), nullable=True)])
 ///
 /// Or create from a PyArrow schema:
 ///
 /// >>> import pyarrow as pa
 /// >>> Schema.from_pyarrow(pa.schema({"x": pa.int32(), "y": pa.string()}))
 /// Schema([Field(x, PrimitiveType("integer"), nullable=True), Field(y, PrimitiveType("string"), nullable=True)])
-#[pyclass(extends=StructType, name="Schema", module="deltalake.schema",
+#[pyclass(extends = StructType, name = "Schema", module = "deltalake.schema",
 text_signature = "(fields)")]
 pub struct PySchema;
 
 #[pymethods]
 impl PySchema {
     #[new]
     fn new(fields: Vec<PyRef<Field>>) -> PyResult<(Self, StructType)> {
@@ -1003,23 +1004,91 @@
         json_loads
             .call1((json.into_py(py),))
             .map(|obj| obj.to_object(py))
     }
 
     /// Return equivalent PyArrow schema
     ///
+    /// :param as_large_types: get schema with all variable size types (list,
+    ///   binary, string) as large variants (with int64 indices). This is for
+    ///   compatibility with systems like Polars that only support the large
+    ///   versions of Arrow types.
+    ///
     /// :rtype: pyarrow.Schema
-    #[pyo3(text_signature = "($self)")]
-    fn to_pyarrow(self_: PyRef<'_, Self>) -> PyResult<PyArrowType<ArrowSchema>> {
+    #[pyo3(signature = (as_large_types = false))]
+    fn to_pyarrow(
+        self_: PyRef<'_, Self>,
+        as_large_types: bool,
+    ) -> PyResult<PyArrowType<ArrowSchema>> {
         let super_ = self_.as_ref();
-        Ok(PyArrowType(
-            (&super_.inner_type.clone())
-                .try_into()
-                .map_err(|err: ArrowError| PyException::new_err(err.to_string()))?,
-        ))
+        let res: ArrowSchema = (&super_.inner_type.clone())
+            .try_into()
+            .map_err(|err: ArrowError| PyException::new_err(err.to_string()))?;
+
+        fn convert_to_large_type(field: ArrowFieldRef, dt: ArrowDataType) -> ArrowFieldRef {
+            let field = field.as_ref().clone();
+            match dt {
+                ArrowDataType::Utf8 => field.with_data_type(ArrowDataType::LargeUtf8).into(),
+
+                ArrowDataType::Binary => field.with_data_type(ArrowDataType::LargeBinary).into(),
+
+                ArrowDataType::List(f) => {
+                    let sub_field = convert_to_large_type(f.clone(), f.data_type().clone());
+                    field
+                        .with_data_type(ArrowDataType::LargeList(sub_field))
+                        .into()
+                }
+
+                ArrowDataType::FixedSizeList(f, size) => {
+                    let sub_field = convert_to_large_type(f.clone(), f.data_type().clone());
+                    field
+                        .with_data_type(ArrowDataType::FixedSizeList(sub_field, size))
+                        .into()
+                }
+
+                ArrowDataType::Map(f, sorted) => {
+                    let sub_field = convert_to_large_type(f.clone(), f.data_type().clone());
+                    field
+                        .with_data_type(ArrowDataType::Map(sub_field, sorted))
+                        .into()
+                }
+
+                ArrowDataType::Struct(fields) => {
+                    let sub_fields = fields
+                        .iter()
+                        .map(|f| {
+                            let dt: ArrowDataType = f.data_type().clone();
+                            convert_to_large_type(f.clone(), dt)
+                        })
+                        .collect();
+
+                    field
+                        .with_data_type(ArrowDataType::Struct(sub_fields))
+                        .into()
+                }
+
+                _ => field.into(),
+            }
+        }
+
+        if as_large_types {
+            let schema = ArrowSchema::new(
+                res.fields
+                    .iter()
+                    .map(|f| {
+                        let dt: ArrowDataType = f.data_type().clone();
+                        convert_to_large_type(f.clone(), dt)
+                    })
+                    .collect::<Vec<ArrowFieldRef>>(),
+            );
+
+            Ok(PyArrowType(schema))
+        } else {
+            Ok(PyArrowType(res))
+        }
     }
 
     /// Create from a PyArrow schema
     ///
     /// :param data_type: a PyArrow schema
     /// :type data_type: pyarrow.Schema
     /// :rtype: Schema
```

### Comparing `deltalake-0.8.1/src/utils.rs` & `deltalake-0.9.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/conftest.py` & `deltalake-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/data_acceptance/test_reader.py` & `deltalake-0.9.0/tests/data_acceptance/test_reader.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/pyspark_integration/test_write_to_pyspark.py` & `deltalake-0.9.0/tests/pyspark_integration/test_write_to_pyspark.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/pyspark_integration/test_writer_readable.py` & `deltalake-0.9.0/tests/pyspark_integration/test_writer_readable.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/pyspark_integration/utils.py` & `deltalake-0.9.0/tests/pyspark_integration/utils.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_benchmark.py` & `deltalake-0.9.0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_checkpoint.py` & `deltalake-0.9.0/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_file_system_handler.py` & `deltalake-0.9.0/tests/test_file_system_handler.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_fs.py` & `deltalake-0.9.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_schema.py` & `deltalake-0.9.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_table_read.py` & `deltalake-0.9.0/tests/test_table_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,16 +381,15 @@
     )
 
     partition_filters = [("unknown", "=", "3")]
     with pytest.raises(Exception) as exception:
         dt.files(partition_filters)
     assert (
         str(exception.value)
-        == 'Invalid partition filter found: [PartitionFilter { key: "unknown", value:'
-        ' Equal("3") }].'
+        == 'Tried to filter partitions on non-partitioned columns: [\n    "unknown",\n]'
     )
 
 
 @pytest.mark.pandas
 def test_delta_table_to_pandas():
     table_path = "../rust/tests/data/simple_table"
     dt = DeltaTable(table_path)
```

### Comparing `deltalake-0.8.1/tests/test_vacuum.py` & `deltalake-0.9.0/tests/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `deltalake-0.8.1/tests/test_writer.py` & `deltalake-0.9.0/tests/test_writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import itertools
 import json
 import os
 import pathlib
 import random
+import threading
 from datetime import date, datetime
 from typing import Any, Dict, Iterable, List
 from unittest.mock import Mock
 
 import pyarrow as pa
 import pyarrow.compute as pc
 import pytest
 from packaging import version
 from pyarrow.dataset import ParquetFileFormat, ParquetReadOptions
 from pyarrow.lib import RecordBatchReader
 
-from deltalake import DeltaTable, write_deltalake
+from deltalake import DeltaTable, PyDeltaTableError, write_deltalake
 from deltalake.table import ProtocolVersions
 from deltalake.writer import DeltaTableProtocolError, try_get_table_and_table_uri
 
 try:
     from pandas.testing import assert_frame_equal
 except ModuleNotFoundError:
     _has_pandas = False
@@ -113,16 +114,14 @@
     new_data = pa.table({"x": pa.array([1, 2, 3])})
 
     with pytest.raises(ValueError):
         write_deltalake(existing_table, new_data, mode="append", overwrite_schema=True)
 
     write_deltalake(existing_table, new_data, mode="overwrite", overwrite_schema=True)
 
-    existing_table.update_incremental()
-
     read_data = existing_table.to_pyarrow_table()
     assert new_data == read_data
     assert existing_table.schema().to_pyarrow() == new_data.schema
 
 
 def test_local_path(tmp_path: pathlib.Path, sample_data: pa.Table, monkeypatch):
     monkeypatch.chdir(tmp_path)  # Make tmp_path the working directory
@@ -139,24 +138,24 @@
 
 def test_roundtrip_metadata(tmp_path: pathlib.Path, sample_data: pa.Table):
     write_deltalake(
         tmp_path,
         sample_data,
         name="test_name",
         description="test_desc",
-        configuration={"configTest": "foobar"},
+        configuration={"delta.appendOnly": "false"},
     )
 
     delta_table = DeltaTable(tmp_path)
 
     metadata = delta_table.metadata()
 
     assert metadata.name == "test_name"
     assert metadata.description == "test_desc"
-    assert metadata.configuration == {"configTest": "foobar"}
+    assert metadata.configuration == {"delta.appendOnly": "false"}
 
 
 @pytest.mark.parametrize(
     "column",
     [
         "utf8",
         "int64",
@@ -169,15 +168,15 @@
         "binary",
         "date32",
     ],
 )
 def test_roundtrip_partitioned(
     tmp_path: pathlib.Path, sample_data: pa.Table, column: str
 ):
-    write_deltalake(tmp_path, sample_data, partition_by=[column])
+    write_deltalake(tmp_path, sample_data, partition_by=column)
 
     delta_table = DeltaTable(tmp_path)
     assert delta_table.schema().to_pyarrow() == sample_data.schema
 
     table = delta_table.to_pyarrow_table()
     table = table.take(pc.sort_indices(table["int64"]))
     assert table == sample_data
@@ -254,21 +253,21 @@
                 "If configuration has delta.appendOnly = 'true', mode must be"
                 f" 'append'. Mode is currently {mode}"
             ),
         ):
             write_deltalake(data_store_type, sample_data, mode=mode)
 
     expected = pa.concat_tables([sample_data, sample_data])
+
     assert table.to_pyarrow_table() == expected
     assert table.version() == 1
 
 
 def test_writer_with_table(existing_table: DeltaTable, sample_data: pa.Table):
     write_deltalake(existing_table, sample_data, mode="overwrite")
-    existing_table.update_incremental()
     assert existing_table.to_pyarrow_table() == sample_data
 
 
 def test_fails_wrong_partitioning(existing_table: DeltaTable, sample_data: pa.Table):
     with pytest.raises(AssertionError):
         write_deltalake(
             existing_table, sample_data, mode="append", partition_by="int32"
@@ -796,7 +795,95 @@
     value = b"\x00\\"
     table = pa.Table.from_pydict({"field_one": [value]})
     write_deltalake(tmp_path, table)
 
     dt = DeltaTable(tmp_path)
     out = dt.to_pyarrow_table()
     assert table == out
+
+
+def test_max_partitions_exceeding_fragment_should_fail(
+    tmp_path: pathlib.Path, sample_data_for_partitioning: pa.Table
+):
+    with pytest.raises(
+        ValueError,
+        match=r"Fragment would be written into \d+ partitions\. This exceeds the maximum of \d+",
+    ):
+        write_deltalake(
+            tmp_path,
+            sample_data_for_partitioning,
+            mode="overwrite",
+            max_partitions=1,
+            partition_by=["p1", "p2"],
+        )
+
+
+def test_large_arrow_types(tmp_path: pathlib.Path):
+    pylist = [
+        {"name": "Joey", "gender": b"M", "arr_type": ["x", "y"], "dict": {"a": b"M"}},
+        {"name": "Ivan", "gender": b"F", "arr_type": ["x", "z"]},
+    ]
+    schema = pa.schema(
+        [
+            pa.field("name", pa.large_string()),
+            pa.field("gender", pa.large_binary()),
+            pa.field("arr_type", pa.large_list(pa.large_string())),
+            pa.field("map_type", pa.map_(pa.large_string(), pa.large_binary())),
+            pa.field("struct", pa.struct([pa.field("sub", pa.large_string())])),
+        ]
+    )
+    table = pa.Table.from_pylist(pylist, schema=schema)
+
+    write_deltalake(tmp_path, table)
+
+    dt = DeltaTable(tmp_path)
+    assert table.schema == dt.schema().to_pyarrow(as_large_types=True)
+
+
+def test_uint_arrow_types(tmp_path: pathlib.Path):
+    pylist = [
+        {"num1": 3, "num2": 3, "num3": 3, "num4": 5},
+        {"num1": 1, "num2": 13, "num3": 35, "num4": 13},
+    ]
+    schema = pa.schema(
+        [
+            pa.field("num1", pa.uint8()),
+            pa.field("num2", pa.uint16()),
+            pa.field("num3", pa.uint32()),
+            pa.field("num4", pa.uint64()),
+        ]
+    )
+    table = pa.Table.from_pylist(pylist, schema=schema)
+
+    write_deltalake(tmp_path, table)
+
+
+def test_concurrency(existing_table: DeltaTable, sample_data: pa.Table):
+    exception = None
+
+    def comp():
+        nonlocal exception
+        dt = DeltaTable(existing_table.table_uri)
+        for _ in range(5):
+            # We should always be able to get a consistent table state
+            data = DeltaTable(dt.table_uri).to_pyarrow_table()
+            # If two overwrites delete the same file and then add their own
+            # concurrently, then this will fail.
+            assert data.num_rows == sample_data.num_rows
+            try:
+                write_deltalake(dt.table_uri, data, mode="overwrite")
+            except Exception as e:
+                exception = e
+
+    n_threads = 2
+    threads = [threading.Thread(target=comp) for _ in range(n_threads)]
+
+    for t in threads:
+        t.start()
+    for t in threads:
+        t.join()
+
+    assert isinstance(exception, PyDeltaTableError)
+    assert (
+        "a concurrent transaction deleted the same data your transaction deletes"
+        in str(exception)
+    )
```

### Comparing `deltalake-0.8.1/Cargo.lock` & `deltalake-0.9.0/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -58,240 +58,251 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arrayref"
-version = "0.3.6"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c527152e37cf757a3f78aae5a06fbeefdb07ccc535c980a3208ee3060dd544"
+checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "arrow"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3724c874f1517cf898cd1c3ad18ab5071edf893c48e73139ab1e16cf0f2affe"
+checksum = "1aea9fcb25bbb70f7f922f95b99ca29c1013dab47f6df61a6f24861842dd7f2e"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
  "arrow-data",
  "arrow-ipc",
  "arrow-json",
  "arrow-ord",
  "arrow-row",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "arrow-select",
  "arrow-string",
- "comfy-table",
  "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e958823b8383ca14d0a2e973de478dd7674cd9f72837f8c41c132a0fda6a4e5e"
+checksum = "8d967b42f7b12c91fd78acd396b20c2973b184c8866846674abbb00c963e93ab"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "chrono",
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db670eab50e76654065b5aed930f4367101fcddcb2223802007d1e0b4d5a2579"
+checksum = "3190f208ee7aa0f3596fa0098d42911dec5e123ca88c002a08b24877ad14c71e"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "chrono",
+ "chrono-tz",
  "half 2.2.1",
  "hashbrown 0.13.2",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f0e01c931882448c0407bd32311a624b9f099739e94e786af68adc97016b5f2"
+checksum = "5d33c733c5b6c44a0fc526f29c09546e04eb56772a7a21e48e602f368be381f6"
 dependencies = [
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bf35d78836c93f80d9362f3ccb47ff5e2c5ecfc270ff42cdf1ef80334961d44"
+checksum = "abd349520b6a1ed4924ae2afc9d23330a3044319e4ec3d5b124c09e4d440ae87"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "arrow-select",
  "chrono",
+ "comfy-table",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a6aa7c2531d89d01fed8c469a9b1bf97132a0bdf70b4724fe4bbb4537a50880"
+checksum = "c80af3c3e290a2a7e1cc518f1471dff331878cb4af9a5b088bf030b89debf649"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "chrono",
  "csv",
  "csv-core",
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea50db4d1e1e4c2da2bfdea7b6d2722eef64267d5ab680d815f7ae42428057f5"
+checksum = "b1c8361947aaa96d331da9df3f7a08bdd8ab805a449994c97f5c4d24c4b7e2cf"
 dependencies = [
  "arrow-buffer",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4042fe6585155d1ec28a8e4937ec901a3ca7a19a22b9f6cd3f551b935cd84f5"
+checksum = "9a46ee000b9fbd1e8db6e8b26acb8c760838512b39d8c9f9d73892cb55351d50"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "flatbuffers",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c907c4ab4f26970a3719dc06e78e8054a01d0c96da3664d23b941e201b33d2b"
+checksum = "4bf2366607be867ced681ad7f272371a5cf1fc2941328eef7b4fee14565166fb"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "chrono",
  "half 2.2.1",
  "indexmap",
  "lexical-core",
  "num",
+ "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e131b447242a32129efc7932f58ed8931b42f35d8701c1a08f9f524da13b1d3c"
+checksum = "304069901c867200e21ec868ae7521165875470ef2f1f6d58f979a443d63997e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "arrow-select",
+ "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b591ef70d76f4ac28dd7666093295fece0e5f9298f49af51ea49c001e1635bb6"
+checksum = "0d57fe8ceef3392fdd493269d8a2d589de17bafce151aacbffbddac7a57f441a"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "half 2.2.1",
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "33.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb327717d87eb94be5eff3b0cb8987f54059d343ee5235abf7f143c85f54cfc8"
+checksum = "d04f17f7b86ded0b5baf98fe6123391c4343e031acc3ccc5fa604cc180bff220"
 dependencies = [
- "bitflags",
  "serde",
 ]
 
 [[package]]
+name = "arrow-schema"
+version = "37.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a16b88a93ac8350f0200b1cd336a1f887315925b8dd7aa145a37b8bdbd8497a4"
+dependencies = [
+ "bitflags 2.2.1",
+]
+
+[[package]]
 name = "arrow-select"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79d3c389d1cea86793934f31594f914c8547d82e91e3411d4833ad0aac3266a7"
+checksum = "98e8a4d6ca37d5212439b24caad4d80743fcbb706706200dd174bb98e68fe9d8"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30ee67790496dd310ddbf5096870324431e89aa76453e010020ac29b1184d356"
+checksum = "cbb594efa397eb6a546f42b1f8df3d242ea84dbfda5232e06035dc2b2e2c8459"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "arrow-select",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "async-compression"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "942c7cd7ae39e91bde4820d74132e9862e62c2f386c3aa90ccf55949f5bad63a"
@@ -300,47 +311,49 @@
  "flate2",
  "futures-core",
  "futures-io",
  "memchr",
  "pin-project-lite",
  "tokio",
  "xz2",
+ "zstd 0.11.2+zstd.1.5.2",
+ "zstd-safe 5.0.2+zstd.1.5.2",
 ]
 
 [[package]]
 name = "async-stream"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad445822218ce64be7a341abfb0b1ea43b5c23aa83902542a4542e78309d8e5e"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
  "async-stream-impl",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-stream-impl"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4655ae1a7b0cdf149156f780c5bf3f1352bc53cbd9e0a361a7ef7b22947e965"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.66"
+version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b84f9ebcc6c1f5b8cb160f6990096a5c127f423fcb6e1ccc46c370cbdfb75dfc"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
@@ -374,15 +387,15 @@
  "aws-smithy-types",
  "aws-types",
  "bytes",
  "hex",
  "http",
  "hyper",
  "ring",
- "time 0.3.20",
+ "time 0.3.21",
  "tokio",
  "tower",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
@@ -493,28 +506,28 @@
  "aws-types",
  "http",
  "tracing",
 ]
 
 [[package]]
 name = "aws-sigv4"
-version = "0.54.1"
+version = "0.54.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdaf11005b7444e6cd66f600d09861a3aeb6eb89a0f003c7c9820dbab2d15297"
+checksum = "86529e7b64d902efea8fff52c1b2529368d04f90305cf632729e3713f6b57dc0"
 dependencies = [
  "aws-smithy-http",
  "form_urlencoded",
  "hex",
  "hmac 0.12.1",
  "http",
  "once_cell",
  "percent-encoding",
  "regex",
  "sha2 0.10.6",
- "time 0.3.20",
+ "time 0.3.21",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-async"
 version = "0.54.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -610,15 +623,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8161232eda10290f5136610a1eb9de56aceaccd70c963a26a260af20ac24794f"
 dependencies = [
  "base64-simd",
  "itoa",
  "num-integer",
  "ryu",
- "time 0.3.20",
+ "time 0.3.21",
 ]
 
 [[package]]
 name = "aws-smithy-xml"
 version = "0.54.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "343ffe9a9bb3f542675f4df0e0d5933513d6ad038ca3907ad1767ba690a99684"
@@ -661,20 +674,48 @@
 checksum = "339abbe78e73178762e23bea9dfd08e697eb3f3301cd4be981c0f78ba5859195"
 dependencies = [
  "outref",
  "vsimd",
 ]
 
 [[package]]
+name = "bindgen"
+version = "0.64.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4243e6031260db77ede97ad86c27e501d646a27ab57b59a574f725d98ab1fb4"
+dependencies = [
+ "bitflags 1.3.2",
+ "cexpr",
+ "clang-sys",
+ "lazy_static",
+ "lazycell",
+ "log",
+ "peeking_take_while",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "rustc-hash",
+ "shlex",
+ "syn 1.0.109",
+ "which",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24a6904aef64d73cf10ab17ebace7befb918b82164785cb89907993be7f83813"
+
+[[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
  "digest 0.10.6",
 ]
@@ -730,17 +771,17 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -793,14 +834,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
  "jobserver",
 ]
 
 [[package]]
+name = "cexpr"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
@@ -815,14 +865,36 @@
  "serde",
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
+name = "chrono-tz"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
+dependencies = [
+ "chrono",
+ "chrono-tz-build",
+ "phf",
+]
+
+[[package]]
+name = "chrono-tz-build"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9998fb9f7e9b2111641485bf8beb32f92945f97f92a3d061f744cfef335f751"
+dependencies = [
+ "parse-zoneinfo",
+ "phf",
+ "phf_codegen",
+]
+
+[[package]]
 name = "ciborium"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
@@ -842,20 +914,31 @@
 checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
 dependencies = [
  "ciborium-io",
  "half 1.8.2",
 ]
 
 [[package]]
+name = "clang-sys"
+version = "1.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
+dependencies = [
+ "glob",
+ "libc",
+ "libloading",
+]
+
+[[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "clap_lex",
  "indexmap",
  "textwrap",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -923,23 +1006,23 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -983,17 +1066,17 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -1087,89 +1170,92 @@
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a140f260e6f3f79013b8bfc65e7ce630c9ab4388c6a89c71e07226f49487b72"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da6383f459341ea689374bf0a42979739dc421874f112ff26f829b8040b8e613"
+checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90201c1a650e95ccff1c8c0bb5a343213bdd317c6e600a93075bca2eff54ec97"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b75aed41bb2e6367cae39e6326ef817a851db13c13e4f3263714ca3cfb8de56"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
  "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
- "parking_lot_core",
+ "parking_lot_core 0.9.7",
 ]
 
 [[package]]
 name = "datafusion"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12d462c103bd1cfd24f8e8a199986d89582af6280528e085c393c4be2ff25da7"
+checksum = "a8a7d4b334f4512ff2fdbce87f511f570ae895af1ac7c729e77c12583253b22a"
 dependencies = [
  "ahash",
  "arrow",
+ "arrow-array",
+ "arrow-schema 37.0.0",
  "async-compression",
  "async-trait",
  "bytes",
  "bzip2",
  "chrono",
  "dashmap",
  "datafusion-common",
+ "datafusion-execution",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-physical-expr",
  "datafusion-row",
  "datafusion-sql",
  "flate2",
  "futures",
@@ -1177,208 +1263,252 @@
  "hashbrown 0.13.2",
  "indexmap",
  "itertools",
  "lazy_static",
  "log",
  "num_cpus",
  "object_store",
- "parking_lot",
+ "parking_lot 0.12.1",
  "parquet",
- "paste",
  "percent-encoding",
  "pin-project-lite",
  "rand 0.8.5",
  "smallvec",
  "sqlparser",
  "tempfile",
  "tokio",
  "tokio-stream",
  "tokio-util",
  "url",
  "uuid",
  "xz2",
+ "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5babdbcf102862b1f1828c1ab41094e39ba881d5ece4cee2d481d528148f592"
+checksum = "80abfcb1dbc6390f952f21de9069e6177ad6318fcae5fbceabb50666d96533dd"
 dependencies = [
  "arrow",
+ "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
  "sqlparser",
 ]
 
 [[package]]
+name = "datafusion-execution"
+version = "23.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df2524f1b4b58319895b112809d2a59e54fa662d0e46330a455f22882c2cb7b9"
+dependencies = [
+ "dashmap",
+ "datafusion-common",
+ "datafusion-expr",
+ "hashbrown 0.13.2",
+ "log",
+ "object_store",
+ "parking_lot 0.12.1",
+ "rand 0.8.5",
+ "tempfile",
+ "url",
+]
+
+[[package]]
 name = "datafusion-expr"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90f0c34e87fa541a59d378dc7ee7c9c3dd1fcfa793eab09561b8b4cb35e1827a"
+checksum = "af8040b7a75b04685f4db0a1b11ffa93cd163c1bc13751df3f5cf76baabaf5a1"
 dependencies = [
  "ahash",
  "arrow",
  "datafusion-common",
- "log",
  "sqlparser",
 ]
 
 [[package]]
+name = "datafusion-objectstore-hdfs"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3dc19661bd4631b5e0efe537a9b40b721f1692d49b830fd9fb623a5fdd84779f"
+dependencies = [
+ "async-trait",
+ "bytes",
+ "chrono",
+ "fs-hdfs3",
+ "futures",
+ "object_store",
+ "tokio",
+]
+
+[[package]]
 name = "datafusion-optimizer"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d0c6d912b7b7e4637d85947222455cd948ea193ca454ebf649e7265fd10b048"
+checksum = "74ceae25accc0f640a4238283f55f3a9fd181d55398703a4330fb2c46261e6a2"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
  "hashbrown 0.13.2",
+ "itertools",
  "log",
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8000e8f8efafb810ff2943323bb48bd722ac5bb919fe302a66b832ed9c25245f"
+checksum = "df4cf228b312f2758cb78e93fe3d2dc602345028efdf7cfa5b338cb370d0a347"
 dependencies = [
  "ahash",
  "arrow",
+ "arrow-array",
  "arrow-buffer",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "blake2",
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-row",
  "half 2.2.1",
  "hashbrown 0.13.2",
  "indexmap",
  "itertools",
  "lazy_static",
+ "libc",
  "md-5 0.10.5",
- "num-traits",
  "paste",
+ "petgraph",
  "rand 0.8.5",
  "regex",
  "sha2 0.10.6",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-proto"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62ce9a56522f03ad8b98e48f6ae924d1af216e60f61da201080bb842daab80d"
+checksum = "ed1bd1e6a9e2aaff2accdaa835d194db678f04d1527a5e6180af8fbcf0bc1cb6"
 dependencies = [
  "arrow",
  "chrono",
  "datafusion",
  "datafusion-common",
  "datafusion-expr",
  "object_store",
- "parking_lot",
- "pbjson-build",
  "prost",
- "prost-build",
 ]
 
 [[package]]
 name = "datafusion-row"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e900f05d7e5666e8ab714a96a28cb6f143e62aa1d501ba1199024f8635c726c"
+checksum = "b52b486fb3d81bb132e400304be01af5aba0ad6737e3518045bb98944991fe32"
 dependencies = [
  "arrow",
  "datafusion-common",
  "paste",
  "rand 0.8.5",
 ]
 
 [[package]]
 name = "datafusion-sql"
-version = "19.0.0"
+version = "23.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "096f293799e8ae883e0f79f8ebaa51e4292e690ba45e0269b48ca9bd79f57094"
+checksum = "773e985c182e41cfd68f7a7b483ab6bfb68beaac241c348cd4b1bf9f9d61b762"
 dependencies = [
- "arrow-schema",
+ "arrow",
+ "arrow-schema 37.0.0",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
 ]
 
 [[package]]
 name = "deltalake"
-version = "0.8.0"
+version = "0.10.0"
 dependencies = [
  "anyhow",
  "arrow",
+ "arrow-array",
+ "arrow-cast",
+ "arrow-schema 37.0.0",
  "async-trait",
  "bytes",
  "cfg-if",
  "chrono",
  "criterion",
  "datafusion",
  "datafusion-common",
  "datafusion-expr",
+ "datafusion-objectstore-hdfs",
+ "datafusion-physical-expr",
  "datafusion-proto",
+ "datafusion-sql",
  "dotenvy",
  "dynamodb_lock",
- "errno 0.3.0",
+ "errno",
  "fs_extra",
  "futures",
  "glibc_version",
  "itertools",
  "lazy_static",
  "libc",
  "log",
  "maplit",
  "num-bigint",
  "num-traits",
  "object_store",
  "once_cell",
- "parking_lot",
+ "parking_lot 0.12.1",
  "parquet",
  "parquet2",
  "percent-encoding",
  "pretty_assertions",
  "rand 0.8.5",
  "regex",
+ "reqwest",
+ "reqwest-middleware",
+ "reqwest-retry",
  "rusoto_core",
  "rusoto_credential",
  "rusoto_dynamodb",
  "rusoto_glue",
  "rusoto_sts",
  "serde",
  "serde_json",
  "serial_test",
+ "sqlparser",
  "tempdir",
  "tempfile",
  "thiserror",
  "tokio",
  "url",
  "utime",
  "uuid",
 ]
 
 [[package]]
 name = "deltalake-python"
-version = "0.8.1"
+version = "0.9.0"
 dependencies = [
- "arrow-schema",
+ "arrow-schema 36.0.0",
  "chrono",
  "deltalake",
  "env_logger 0.10.0",
  "futures",
  "lazy_static",
  "pyo3",
  "regex",
@@ -1439,17 +1569,17 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "dotenvy"
-version = "0.15.6"
+version = "0.15.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03d8c417d7a8cb362e0c37e5d815f5eb7c37f79ff93707329d5a194e42e54ca0"
+checksum = "1aaf95b3e5c8f23aa320147307562d361db0ae0d51242340f558153b4eb2439b"
 
 [[package]]
 name = "dynamodb_lock"
 version = "0.4.3"
 dependencies = [
  "async-trait",
  "log",
@@ -1500,32 +1630,21 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -1557,23 +1676,23 @@
 
 [[package]]
 name = "flatbuffers"
 version = "23.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77f5399c2c9c50ae9418e522842ad362f61ee48b346ac106807bd355a8a7c619"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "rustc_version",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -1602,101 +1721,115 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "fs-hdfs3"
+version = "0.1.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "103220e69dd76c57fda4c5dc5156886937ab7292e3f6cf2293e83ca77822ae3c"
+dependencies = [
+ "bindgen",
+ "cc",
+ "lazy_static",
+ "libc",
+ "log",
+ "url",
+]
+
+[[package]]
 name = "fs_extra"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42703706b716c37f96a77aea830392ad231f44c9e9a67872fa5548707e11b11c"
 
 [[package]]
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
 
 [[package]]
 name = "futures"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "531ac96c6ff5fd7c62263c5e3c67a603af4fcaee2e1a0ae5565ba3a11e69e549"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1997dd9df74cdac935c76252744c1ed5794fac083242ea4fe77ef3ed60ba0f83"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -1704,31 +1837,33 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
+ "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "glibc_version"
 version = "0.1.2"
 dependencies = [
  "regex",
@@ -1738,17 +1873,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.16"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be7b54589b581f624f566bf5d8eb2bab1db736c51528720b6bd36b96b55924d"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1892,17 +2027,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.25"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc5e554ff619822309ffd57d8734d77cd5ce6238bc956f037ea06c58238c9899"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -1961,24 +2096,24 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
@@ -1995,17 +2130,17 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
@@ -2016,48 +2151,52 @@
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
 ]
 
 [[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.6"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfa919a82ea574332e2de6e74b4c36e74d41982b335080fa59d4ef31be20fdf3"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e22bd8629359895450b59ea7a776c850561b96a3b1d31321c1949d9e6c9146"
+checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.4"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21b6b32576413a8e69b90e952e4a026476040d81017b80445deda5f2d3921857"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -2109,17 +2248,17 @@
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
 
 [[package]]
 name = "lambda_runtime"
-version = "0.7.3"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd32d5799db2155ae4d47116bb3e169b59f531ced4d5762a10c2125bdd2bf134"
+checksum = "124a7d502e26b1ae9645bafd964d299d9c0d882cc8b3e228604d02bf0e13fc87"
 dependencies = [
  "async-stream",
  "bytes",
  "futures",
  "http",
  "hyper",
  "lambda_runtime_api_client",
@@ -2129,31 +2268,37 @@
  "tokio-stream",
  "tower",
  "tracing",
 ]
 
 [[package]]
 name = "lambda_runtime_api_client"
-version = "0.7.0"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7210012be904051520f0dc502140ba599bae3042b65b3737b87727f1aa88a7d6"
+checksum = "690c5ae01f3acac8c9c3348b556fc443054e9b7f1deaf53e9ebab716282bf0ed"
 dependencies = [
  "http",
  "hyper",
  "tokio",
  "tower-service",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
+name = "lazycell"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
+
+[[package]]
 name = "lexical-core"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2cde5de06e8d4c2faabc400238f9ae1c74d5412d03a7bd067645ccbc47070e46"
 dependencies = [
  "lexical-parse-float",
  "lexical-parse-integer",
@@ -2211,17 +2356,27 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.143"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "edc207893e85c5d6be840e969b496b53d94cec8be2d501b214f50daa97fa8024"
+
+[[package]]
+name = "libloading"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
+dependencies = [
+ "cfg-if",
+ "winapi",
+]
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -2232,17 +2387,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -2329,23 +2484,39 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
-version = "0.3.16"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
+
+[[package]]
+name = "mime_guess"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
+dependencies = [
+ "mime",
+ "unicase",
+]
+
+[[package]]
+name = "minimal-lexical"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a60c7ce501c71e03a9c9c0d35b861413ae925bd979cc7a4e30d060069aaac8d"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.6"
@@ -2355,20 +2526,14 @@
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
-name = "multimap"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
-
-[[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
 dependencies = [
  "lazy_static",
  "libc",
@@ -2379,14 +2544,24 @@
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "num"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
 dependencies = [
  "num-bigint",
  "num-complex",
@@ -2467,28 +2642,28 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "object_store"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1ea8f683b4f89a64181393742c041520a1a87e9775e6b4c0dd5a3281af05fc6"
+checksum = "ec9cd6ca25e796a49fa242876d1c4de36a24a6da5258e9f0bc062dbf5e81c53b"
 dependencies = [
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "aws-types",
  "base64 0.21.0",
  "bytes",
  "chrono",
  "futures",
  "itertools",
- "parking_lot",
+ "parking_lot 0.12.1",
  "percent-encoding",
  "quick-xml",
  "rand 0.8.5",
  "reqwest",
  "ring",
  "rustls-pemfile",
  "serde",
@@ -2516,60 +2691,59 @@
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
 name = "openssl"
-version = "0.10.45"
+version = "0.10.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b102428fd03bc5edf97f62620f7298614c45cedf287c271e7ed450bbaf83f2e1"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.1+1.1.1t"
+version = "111.25.3+1.1.1t"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ef9a9cc6ea7d9d5e7c4a913dc4b48d0e359eddf01af1dfec96ba7064b4aba10"
+checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.80"
+version = "0.9.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23bbbf7854cd45b83958ebe919f0e8e516793727652e27fda10a8384cfc790b7"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -2580,17 +2754,17 @@
 checksum = "7940cf2ca942593318d07fcf2596cdca60a85c9e7fab408a5e21a4f9dcd40d87"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "output_vt100"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "628223faebab4e3e40667ee0b2336d34a5b960ff60ea743ddfdbcf7770bcfb66"
 dependencies = [
@@ -2601,62 +2775,88 @@
 name = "outref"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4030760ffd992bef45b0ae3f10ce1aba99e33464c90d14dd7c039884963ddc7a"
 
 [[package]]
 name = "parking_lot"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+dependencies = [
+ "instant",
+ "lock_api",
+ "parking_lot_core 0.8.6",
+]
+
+[[package]]
+name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core",
+ "parking_lot_core 0.9.7",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+dependencies = [
+ "cfg-if",
+ "instant",
+ "libc",
+ "redox_syscall 0.2.16",
+ "smallvec",
+ "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "parquet"
-version = "33.0.0"
+version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1b076829801167d889795cd1957989055543430fa1469cb1f6e32b789bfc764"
+checksum = "b5022d98333271f4ca3e87bab760498e61726bf5a6ca919123c80517e20ded29"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
- "arrow-schema",
+ "arrow-schema 37.0.0",
  "arrow-select",
  "base64 0.21.0",
  "brotli",
  "bytes",
  "chrono",
  "flate2",
  "futures",
  "hashbrown 0.13.2",
  "lz4",
  "num",
  "num-bigint",
  "object_store",
  "paste",
  "seq-macro",
+ "serde_json",
  "snap",
  "thrift",
  "tokio",
  "twox-hash",
  "zstd 0.12.3+zstd.1.5.2",
 ]
 
@@ -2664,46 +2864,49 @@
 name = "parquet-format-safe"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
 
 [[package]]
 name = "parquet2"
-version = "0.17.1"
+version = "0.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aefc53bedbf9bbe0ff8912befafaafe30ced83851fb0aebe86696a9289ebb29e"
+checksum = "579fe5745f02cef3d5f236bfed216fd4693e49e4e920a13475c6132233283bce"
 dependencies = [
  "brotli",
  "flate2",
  "lz4",
  "parquet-format-safe",
  "seq-macro",
  "snap",
  "streaming-decompression",
  "xxhash-rust",
- "zstd 0.11.2+zstd.1.5.2",
+ "zstd 0.12.3+zstd.1.5.2",
+]
+
+[[package]]
+name = "parse-zoneinfo"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
+dependencies = [
+ "regex",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
-name = "pbjson-build"
-version = "0.5.1"
+name = "peeking_take_while"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdbb7b706f2afc610f3853550cdbbf6372fd324824a087806bd4480ea4996e24"
-dependencies = [
- "heck",
- "itertools",
- "prost",
- "prost-types",
-]
+checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
@@ -2714,14 +2917,52 @@
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
+name = "phf"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+dependencies = [
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_codegen"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a56ac890c5e3ca598bbdeaa99964edb5b0258a583a9eb6ef4e89fc85d9224770"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+dependencies = [
+ "phf_shared",
+ "rand 0.8.5",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
 name = "pin-project"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
 dependencies = [
  "pin-project-internal",
 ]
@@ -2730,15 +2971,15 @@
 name = "pin-project-internal"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -2747,17 +2988,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plotters"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
 dependencies = [
@@ -2808,163 +3049,122 @@
 checksum = "926d36b9553851b8b0005f1275891b392ee4d2d833852c417ed025477350fb9d"
 dependencies = [
  "env_logger 0.7.1",
  "log",
 ]
 
 [[package]]
-name = "prettyplease"
-version = "0.1.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ebcd279d20a4a0a2404a33056388e950504d891c855c7975b9a8fef75f3bf04"
-dependencies = [
- "proc-macro2",
- "syn",
-]
-
-[[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
-version = "0.11.8"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e48e50df39172a3e7eb17e14642445da64996989bc212b583015435d39a58537"
+checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
-name = "prost-build"
-version = "0.11.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3f8ad728fb08fe212df3c05169e940fbb6d9d16a877ddde14644a983ba2012e"
-dependencies = [
- "bytes",
- "heck",
- "itertools",
- "lazy_static",
- "log",
- "multimap",
- "petgraph",
- "prettyplease",
- "prost",
- "prost-types",
- "regex",
- "syn",
- "tempfile",
- "which",
-]
-
-[[package]]
 name = "prost-derive"
-version = "0.11.8"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ea9b0f8cbe5e15a8a042d030bd96668db28ecb567ec37d691971ff5731d2b1b"
+checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
- "syn",
-]
-
-[[package]]
-name = "prost-types"
-version = "0.11.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "379119666929a1afd7a043aa6cf96fa67a6dce9af60c88095a4686dbce4c9c88"
-dependencies = [
- "prost",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quick-xml"
-version = "0.27.1"
+version = "0.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffc053f057dd768a56f62cd7e434c42c831d296968997e9ac1f76ea7c2d14c41"
+checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
@@ -3066,59 +3266,74 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.14"
+version = "0.11.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21eed90ec8570952d53b772ecf8f206aa1ec9a3d76b2521c56c42973f2d91ee9"
+checksum = "13293b639a097af28fc8a90f22add145a9c954e49d77da06263d58cf44d5fb91"
 dependencies = [
  "base64 0.21.0",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -3127,14 +3342,15 @@
  "hyper",
  "hyper-rustls 0.23.2",
  "hyper-tls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
+ "mime_guess",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
  "rustls 0.20.8",
  "rustls-pemfile",
  "serde",
@@ -3151,14 +3367,63 @@
  "wasm-streams",
  "web-sys",
  "webpki-roots",
  "winreg",
 ]
 
 [[package]]
+name = "reqwest-middleware"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "99c50db2c7ccd815f976473dd7d0bde296f8c3b77c383acf4fc021cdcf10852b"
+dependencies = [
+ "anyhow",
+ "async-trait",
+ "http",
+ "reqwest",
+ "serde",
+ "task-local-extensions",
+ "thiserror",
+]
+
+[[package]]
+name = "reqwest-retry"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "48d0fd6ef4c6d23790399fe15efc8d12cd9f3d4133958f9bd7801ee5cbaec6c4"
+dependencies = [
+ "anyhow",
+ "async-trait",
+ "chrono",
+ "futures",
+ "getrandom",
+ "http",
+ "hyper",
+ "parking_lot 0.11.2",
+ "reqwest",
+ "reqwest-middleware",
+ "retry-policies",
+ "task-local-extensions",
+ "tokio",
+ "tracing",
+ "wasm-timer",
+]
+
+[[package]]
+name = "retry-policies"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e09bbcb5003282bcb688f0bae741b278e9c7e8f378f561522c9806c58e075d9b"
+dependencies = [
+ "anyhow",
+ "chrono",
+ "rand 0.8.5",
+]
+
+[[package]]
 name = "ring"
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
  "cc",
  "libc",
@@ -3292,34 +3557,40 @@
  "futures",
  "rusoto_core",
  "serde_urlencoded",
  "xml-rs",
 ]
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.9"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd5c6ff11fecd55b40746d1995a02f2eb375bf8c00d192d521ee09f42bef37bc"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
- "bitflags",
- "errno 0.2.8",
+ "bitflags 1.3.2",
+ "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35edb675feee39aec9c99fa5ff985081995a06d594114ae14cbe797ad7b7a6d7"
@@ -3440,15 +3711,15 @@
 
 [[package]]
 name = "security-framework"
 version = "2.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
@@ -3471,37 +3742,37 @@
 name = "seq-macro"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6b44e8fc93a14e66336d230954dda83d18b4605ccace8fe09bc7514a71ad0bc"
 
 [[package]]
 name = "serde"
-version = "1.0.155"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71f2b4817415c6d4210bfe1c7bfcf4801b2d904cb4d0e1a8fdb651013c9e86b8"
+checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.155"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d071a94a3fac4aff69d023a7f411e33f40f3483f8c5190b1953822b6b76d7630"
+checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3514,35 +3785,35 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serial_test"
-version = "1.0.0"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "538c30747ae860d6fb88330addbbd3e0ddbe46d662d032855596d8a8ca260611"
+checksum = "0e56dd856803e253c8f298af3f4d7eb0ae5e23a737252cd90bb4f3b435033b2d"
 dependencies = [
  "dashmap",
  "futures",
  "lazy_static",
  "log",
- "parking_lot",
+ "parking_lot 0.12.1",
  "serial_test_derive",
 ]
 
 [[package]]
 name = "serial_test_derive"
-version = "1.0.0"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "079a83df15f85d89a68d64ae1238f142f172b1fa915d0d76b26a7cba1b659a69"
+checksum = "91d129178576168c589c9ec973feedf7d3126c01ac2bf08795109aa35b69fb8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "sha2"
 version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d58a1e1bf39749807d89cf2d98ac2dfa0ff1cb3faa38fbb64dd88ac8013d800"
@@ -3577,14 +3848,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
@@ -3610,15 +3887,15 @@
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "475b3bbe5245c26f2d8a6f62d67c1f30eb9fffeccee721c45d162c3ebbdf81b2"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "snap"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e9f0ab6ef7eb7353d9119c170a436d1bf248eea575ac42d19d12f4e34130831"
@@ -3637,31 +3914,31 @@
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "sqlparser"
-version = "0.30.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db67dc6ef36edb658196c3fef0464a80b53dbbc194a904e81f9bd4190f9ecc5b"
+checksum = "355dc4d4b6207ca8a3434fc587db0a8016130a574dbcdbfb93d7f7b5bc5b211a"
 dependencies = [
  "log",
  "sqlparser_derive",
 ]
 
 [[package]]
 name = "sqlparser_derive"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55fe75cb4a364c7f7ae06c7dbbc8d84bddd85d6cdf9975963c3935bc1991761e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -3687,15 +3964,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
@@ -3708,40 +3985,60 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+
+[[package]]
+name = "task-local-extensions"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "ba323866e5d033818e3240feeb9f7db2c4296674e4d9e16b97b7bf8f490434e8"
+dependencies = [
+ "pin-utils",
+]
 
 [[package]]
 name = "tempdir"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15f2b5fb00ccdf689e0149d1b1b3c03fead81c2b37735d812fa8bddbbf41b6d8"
 dependencies = [
  "rand 0.4.6",
  "remove_dir_all",
 ]
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -3753,30 +4050,30 @@
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5ab016db510546d856297882807df8da66a16fb8c4101cb8b30054b0d5b2d9c"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5420d42e90af0c38c3290abcca25b9b3bdf379fc9f55c528f53a269d9c9a267e"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -3795,34 +4092,34 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
 dependencies = [
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
@@ -3855,41 +4152,40 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3918,28 +4214,28 @@
  "rustls 0.20.8",
  "tokio",
  "webpki 0.22.0",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.12"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fb52b74f05dbf495a8fba459fdc331812b96aa086d9eb78101fa0d4569c3313"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -3984,21 +4280,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
@@ -4025,18 +4321,27 @@
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
+name = "unicase"
+version = "2.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
+dependencies = [
+ "version_check",
+]
+
+[[package]]
 name = "unicode-bidi"
-version = "0.3.11"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524b68aca1d05e03fdf03fcdce2c6c94b6daf6d16861ddaa7e4f2b6638a9052c"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
@@ -4098,17 +4403,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "vcpkg"
@@ -4126,20 +4431,19 @@
 name = "vsimd"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c3082ca00d5a5ef149bb8b555a72ae84c9c59f7250f013ac822ac2e49b19c64"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4178,15 +4482,15 @@
 checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4212,15 +4516,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
@@ -4237,14 +4541,29 @@
  "js-sys",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
+name = "wasm-timer"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "be0ecb0db480561e9a7642b5d3e4187c128914e58aa84330b9493e3eb68c5e7f"
+dependencies = [
+ "futures",
+ "js-sys",
+ "parking_lot 0.11.2",
+ "pin-utils",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
 name = "web-sys"
 version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
@@ -4318,108 +4637,183 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "xml-rs"
-version = "0.8.4"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2d7d3948613f75c98fd9328cfdcc45acc4d360655289d0a7d4ec931392200a3"
+checksum = "374b609fb36c36ce3501094dc0548f7df5d8d102224b65bc59812e4a5425d571"
 
 [[package]]
 name = "xmlparser"
 version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
 
@@ -4442,17 +4836,17 @@
 name = "yansi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 
 [[package]]
 name = "zstd"
 version = "0.11.2+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
 dependencies = [
@@ -4461,40 +4855,40 @@
 
 [[package]]
 name = "zstd"
 version = "0.12.3+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
- "zstd-safe 6.0.4+zstd.1.5.4",
+ "zstd-safe 6.0.5+zstd.1.5.4",
 ]
 
 [[package]]
 name = "zstd-safe"
 version = "5.0.2+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.4+zstd.1.5.4"
+version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7afb4b54b8910cf5447638cb54bf4e8a65cbedd783af98b98c62ffe91f185543"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.7+zstd.1.5.4"
+version = "2.0.8+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94509c3ba2fe55294d752b79842c530ccfab760192521df74a081a78d2b3c7f5"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
```

### Comparing `deltalake-0.8.1/PKG-INFO` & `deltalake-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: deltalake
-Version: 0.8.1
+Version: 0.9.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: pyarrow>=7
 Requires-Dist: typing-extensions;python_version<"3.8"
 Requires-Dist: pyspark; extra == 'pyspark'
 Requires-Dist: delta-spark; extra == 'pyspark'
 Requires-Dist: numpy==1.22.2; extra == 'pyspark'
-Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: mypy; extra == 'devel'
 Requires-Dist: black; extra == 'devel'
 Requires-Dist: ruff; extra == 'devel'
 Requires-Dist: packaging>=20; extra == 'devel'
 Requires-Dist: pytest; extra == 'devel'
 Requires-Dist: pytest-mock; extra == 'devel'
 Requires-Dist: pytest-cov; extra == 'devel'
 Requires-Dist: pytest-timeout; extra == 'devel'
 Requires-Dist: sphinx<=4.5; extra == 'devel'
 Requires-Dist: sphinx-rtd-theme; extra == 'devel'
 Requires-Dist: toml; extra == 'devel'
 Requires-Dist: wheel; extra == 'devel'
 Requires-Dist: pytest-benchmark; extra == 'devel'
+Requires-Dist: pandas<2; extra == 'pandas'
 Provides-Extra: pyspark
-Provides-Extra: pandas
 Provides-Extra: devel
+Provides-Extra: pandas
 License-File: LICENSE.txt
 Summary: Native Delta Lake Python binding based on delta-rs with Pandas integration
 Keywords: deltalake,delta,datalake,pandas,arrow
 Home-Page: https://github.com/delta-io/delta-rs
 Author: Qingping Hou <dave2008713@gmail.com>
 Author-email: Qingping Hou <dave2008713@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://delta-io.github.io/delta-rs/python/
 Project-URL: repository, https://github.com/delta-io/delta-rs
+Project-URL: documentation, https://delta-io.github.io/delta-rs/python/
 
 # Deltalake-python
 
 [![PyPI](https://img.shields.io/pypi/v/deltalake.svg?style=flat-square)](https://pypi.org/project/deltalake/)
 [![userdoc](https://img.shields.io/badge/docs-user-blue)](https://delta-io.github.io/delta-rs/python/)
 [![apidoc](https://img.shields.io/badge/docs-api-blue)](https://delta-io.github.io/delta-rs/python/api_reference.html)
```

