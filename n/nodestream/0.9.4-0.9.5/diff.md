# Comparing `tmp/nodestream-0.9.4.tar.gz` & `tmp/nodestream-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream-0.9.4.tar", max compression
+gzip compressed data, was "nodestream-0.9.5.tar", max compression
```

## Comparing `nodestream-0.9.4.tar` & `nodestream-0.9.5.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0    11358 2023-11-17 14:58:42.828466 nodestream-0.9.4/LICENSE
--rw-r--r--   0        0        0     1774 2023-11-17 14:58:42.829181 nodestream-0.9.4/README.md
--rw-r--r--   0        0        0        0 2023-11-17 14:58:42.847363 nodestream-0.9.4/nodestream/__init__.py
--rw-r--r--   0        0        0      120 2023-11-17 14:58:42.847966 nodestream-0.9.4/nodestream/cli/__init__.py
--rw-r--r--   0        0        0      833 2023-11-17 14:58:42.848344 nodestream-0.9.4/nodestream/cli/application.py
--rw-r--r--   0        0        0      429 2023-12-08 21:42:10.791877 nodestream-0.9.4/nodestream/cli/commands/__init__.py
--rw-r--r--   0        0        0      780 2023-11-17 14:58:42.849267 nodestream-0.9.4/nodestream/cli/commands/audit_command.py
--rw-r--r--   0        0        0     4292 2023-12-08 21:42:10.792271 nodestream-0.9.4/nodestream/cli/commands/copy.py
--rw-r--r--   0        0        0      879 2023-11-17 14:58:42.849669 nodestream-0.9.4/nodestream/cli/commands/new.py
--rw-r--r--   0        0        0     1387 2023-11-17 14:58:42.850053 nodestream-0.9.4/nodestream/cli/commands/nodestream_command.py
--rw-r--r--   0        0        0     1213 2023-11-17 14:58:42.850402 nodestream-0.9.4/nodestream/cli/commands/print_schema.py
--rw-r--r--   0        0        0      893 2023-11-17 14:58:42.850768 nodestream-0.9.4/nodestream/cli/commands/remove.py
--rw-r--r--   0        0        0     1479 2023-11-17 14:58:42.851103 nodestream-0.9.4/nodestream/cli/commands/run.py
--rw-r--r--   0        0        0     1426 2023-11-17 14:58:42.851450 nodestream-0.9.4/nodestream/cli/commands/scaffold.py
--rw-r--r--   0        0        0      622 2023-11-17 14:58:42.851977 nodestream-0.9.4/nodestream/cli/commands/shared_options.py
--rw-r--r--   0        0        0      596 2023-11-17 14:58:42.852319 nodestream-0.9.4/nodestream/cli/commands/show.py
--rw-r--r--   0        0        0      962 2023-12-08 21:42:10.793352 nodestream-0.9.4/nodestream/cli/operations/__init__.py
--rw-r--r--   0        0        0      988 2023-11-17 14:58:42.853307 nodestream-0.9.4/nodestream/cli/operations/add_pipeline_to_project.py
--rw-r--r--   0        0        0      438 2023-11-17 14:58:42.853643 nodestream-0.9.4/nodestream/cli/operations/commit_project_to_disk.py
--rw-r--r--   0        0        0     1843 2023-11-17 14:58:42.854019 nodestream-0.9.4/nodestream/cli/operations/generate_pipeline_scaffold.py
--rw-r--r--   0        0        0     1153 2023-11-17 14:58:42.854373 nodestream-0.9.4/nodestream/cli/operations/initialize_logger.py
--rw-r--r--   0        0        0      267 2023-11-17 14:58:42.854748 nodestream-0.9.4/nodestream/cli/operations/initialize_project.py
--rw-r--r--   0        0        0      384 2023-11-17 14:58:42.855091 nodestream-0.9.4/nodestream/cli/operations/operation.py
--rw-r--r--   0        0        0     1251 2023-11-17 14:58:42.855416 nodestream-0.9.4/nodestream/cli/operations/print_project_schema.py
--rw-r--r--   0        0        0      533 2023-11-17 14:58:42.855796 nodestream-0.9.4/nodestream/cli/operations/remove_pipeline_from_project.py
--rw-r--r--   0        0        0     1145 2023-11-17 14:58:42.856140 nodestream-0.9.4/nodestream/cli/operations/run_audit.py
--rw-r--r--   0        0        0     1288 2023-12-08 21:42:10.794031 nodestream-0.9.4/nodestream/cli/operations/run_copy.py
--rw-r--r--   0        0        0     4636 2023-12-18 19:07:38.219165 nodestream-0.9.4/nodestream/cli/operations/run_pipeline.py
--rw-r--r--   0        0        0      866 2023-11-17 14:58:42.856960 nodestream-0.9.4/nodestream/cli/operations/run_project_cookiecutter.py
--rw-r--r--   0        0        0     2436 2023-11-17 14:58:42.857318 nodestream-0.9.4/nodestream/cli/operations/show_pipelines.py
--rw-r--r--   0        0        0      622 2023-12-08 21:42:10.794794 nodestream-0.9.4/nodestream/compat.py
--rw-r--r--   0        0        0      326 2023-12-08 21:42:10.796267 nodestream-0.9.4/nodestream/databases/__init__.py
--rw-r--r--   0        0        0     2578 2023-12-08 21:42:10.796728 nodestream-0.9.4/nodestream/databases/copy.py
--rw-r--r--   0        0        0     1349 2023-12-08 21:42:10.797452 nodestream-0.9.4/nodestream/databases/database_connector.py
--rw-r--r--   0        0        0     3401 2023-12-08 21:42:10.798127 nodestream-0.9.4/nodestream/databases/debounced_ingest_strategy.py
--rw-r--r--   0        0        0     2628 2023-11-17 14:58:42.858835 nodestream-0.9.4/nodestream/databases/ingest_strategy.py
--rw-r--r--   0        0        0       94 2023-11-17 14:58:42.859335 nodestream-0.9.4/nodestream/databases/neo4j/__init__.py
--rw-r--r--   0        0        0     1952 2023-12-08 21:42:10.798853 nodestream-0.9.4/nodestream/databases/neo4j/database_connector.py
--rw-r--r--   0        0        0     2005 2023-12-08 21:42:10.799522 nodestream-0.9.4/nodestream/databases/neo4j/extractor.py
--rw-r--r--   0        0        0     2710 2023-11-17 14:58:42.860386 nodestream-0.9.4/nodestream/databases/neo4j/index_query_builder.py
--rw-r--r--   0        0        0     9693 2023-12-11 16:47:31.774972 nodestream-0.9.4/nodestream/databases/neo4j/ingest_query_builder.py
--rw-r--r--   0        0        0     1788 2023-11-17 14:58:42.861089 nodestream-0.9.4/nodestream/databases/neo4j/query.py
--rw-r--r--   0        0        0     3326 2023-12-18 19:07:41.885249 nodestream-0.9.4/nodestream/databases/neo4j/query_executor.py
--rw-r--r--   0        0        0     2679 2023-12-08 21:42:10.800852 nodestream-0.9.4/nodestream/databases/neo4j/type_retriever.py
--rw-r--r--   0        0        0     3472 2023-12-08 21:42:10.801788 nodestream-0.9.4/nodestream/databases/operation_debouncer.py
--rw-r--r--   0        0        0     1691 2023-12-08 21:42:10.802445 nodestream-0.9.4/nodestream/databases/query_executor.py
--rw-r--r--   0        0        0     2044 2023-11-17 14:58:42.862747 nodestream-0.9.4/nodestream/databases/query_executor_with_statistics.py
--rw-r--r--   0        0        0     1667 2023-12-08 21:42:10.803100 nodestream-0.9.4/nodestream/databases/writer.py
--rw-r--r--   0        0        0     3566 2023-12-18 19:07:38.221862 nodestream-0.9.4/nodestream/file_io.py
--rw-r--r--   0        0        0      137 2023-11-17 14:58:42.863932 nodestream-0.9.4/nodestream/interpreting/__init__.py
--rw-r--r--   0        0        0      574 2023-11-17 14:58:42.864570 nodestream-0.9.4/nodestream/interpreting/interpretations/__init__.py
--rw-r--r--   0        0        0     1369 2023-11-17 14:58:42.864997 nodestream-0.9.4/nodestream/interpreting/interpretations/extract_variables_interpretation.py
--rw-r--r--   0        0        0      948 2023-11-17 14:58:42.865419 nodestream-0.9.4/nodestream/interpreting/interpretations/interpretation.py
--rw-r--r--   0        0        0     1262 2023-11-17 14:58:42.865772 nodestream-0.9.4/nodestream/interpreting/interpretations/properties_interpretation.py
--rw-r--r--   0        0        0    10429 2023-12-08 21:42:10.804042 nodestream-0.9.4/nodestream/interpreting/interpretations/relationship_interpretation.py
--rw-r--r--   0        0        0     4469 2023-11-17 14:58:42.866522 nodestream-0.9.4/nodestream/interpreting/interpretations/source_node_interpretation.py
--rw-r--r--   0        0        0     2627 2023-11-17 14:58:42.866885 nodestream-0.9.4/nodestream/interpreting/interpretations/switch_interpretation.py
--rw-r--r--   0        0        0     4820 2023-11-17 14:58:42.867267 nodestream-0.9.4/nodestream/interpreting/interpreter.py
--rw-r--r--   0        0        0     1744 2023-11-17 14:58:42.867653 nodestream-0.9.4/nodestream/interpreting/record_decomposers.py
--rw-r--r--   0        0        0      787 2023-12-08 21:42:10.804907 nodestream-0.9.4/nodestream/model/__init__.py
--rw-r--r--   0        0        0      381 2023-12-08 21:42:10.805230 nodestream-0.9.4/nodestream/model/creation_rules.py
--rw-r--r--   0        0        0     3739 2023-12-08 21:42:10.805861 nodestream-0.9.4/nodestream/model/desired_ingestion.py
--rw-r--r--   0        0        0     7728 2023-12-08 21:42:10.806571 nodestream-0.9.4/nodestream/model/graph_objects.py
--rw-r--r--   0        0        0      873 2023-11-17 14:58:42.869395 nodestream-0.9.4/nodestream/model/ingestion_hooks.py
--rw-r--r--   0        0        0      851 2023-11-17 14:58:42.870093 nodestream-0.9.4/nodestream/model/ttl.py
--rw-r--r--   0        0        0     1023 2023-12-18 19:07:38.222883 nodestream-0.9.4/nodestream/pipeline/__init__.py
--rw-r--r--   0        0        0      321 2023-12-18 19:07:38.223798 nodestream-0.9.4/nodestream/pipeline/argument_resolvers/__init__.py
--rw-r--r--   0        0        0      531 2023-12-18 19:07:38.225181 nodestream-0.9.4/nodestream/pipeline/argument_resolvers/argument_resolver.py
--rw-r--r--   0        0        0      604 2023-12-18 19:07:38.226112 nodestream-0.9.4/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py
--rw-r--r--   0        0        0      676 2023-12-18 19:07:38.226726 nodestream-0.9.4/nodestream/pipeline/argument_resolvers/include_file_resolver.py
--rw-r--r--   0        0        0     2474 2023-12-18 19:07:38.227326 nodestream-0.9.4/nodestream/pipeline/class_loader.py
--rw-r--r--   0        0        0      386 2023-11-17 14:58:42.873460 nodestream-0.9.4/nodestream/pipeline/extractors/__init__.py
--rw-r--r--   0        0        0     1306 2023-11-17 14:58:42.873891 nodestream-0.9.4/nodestream/pipeline/extractors/apis.py
--rw-r--r--   0        0        0      678 2023-11-17 14:58:42.874261 nodestream-0.9.4/nodestream/pipeline/extractors/extractor.py
--rw-r--r--   0        0        0     4307 2023-11-17 14:58:42.874642 nodestream-0.9.4/nodestream/pipeline/extractors/files.py
--rw-r--r--   0        0        0      546 2023-11-17 14:58:42.875029 nodestream-0.9.4/nodestream/pipeline/extractors/iterable.py
--rw-r--r--   0        0        0        0 2023-11-17 14:58:42.875566 nodestream-0.9.4/nodestream/pipeline/extractors/stores/__init__.py
--rw-r--r--   0        0        0      130 2023-11-17 14:58:42.876203 nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/__init__.py
--rw-r--r--   0        0        0     4613 2023-11-17 14:58:42.876573 nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/athena_extractor.py
--rw-r--r--   0        0        0     2503 2023-11-17 14:58:42.876968 nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/credential_utils.py
--rw-r--r--   0        0        0     3267 2023-11-17 14:58:42.877377 nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/s3_extractor.py
--rw-r--r--   0        0        0      231 2023-11-17 14:58:42.878039 nodestream-0.9.4/nodestream/pipeline/extractors/streams/__init__.py
--rw-r--r--   0        0        0     3167 2023-12-08 21:42:10.807977 nodestream-0.9.4/nodestream/pipeline/extractors/streams/extractor.py
--rw-r--r--   0        0        0     3529 2023-12-08 21:42:10.808632 nodestream-0.9.4/nodestream/pipeline/extractors/streams/kafka.py
--rw-r--r--   0        0        0      646 2023-11-17 14:58:42.879187 nodestream-0.9.4/nodestream/pipeline/extractors/ttls.py
--rw-r--r--   0        0        0     5015 2023-12-08 21:42:10.809368 nodestream-0.9.4/nodestream/pipeline/filters.py
--rw-r--r--   0        0        0       22 2023-11-17 14:58:42.879884 nodestream-0.9.4/nodestream/pipeline/flush.py
--rw-r--r--   0        0        0      869 2023-11-17 14:58:42.880257 nodestream-0.9.4/nodestream/pipeline/meta.py
--rw-r--r--   0        0        0      327 2023-11-17 14:58:42.880817 nodestream-0.9.4/nodestream/pipeline/normalizers/__init__.py
--rw-r--r--   0        0        0      240 2023-11-17 14:58:42.881345 nodestream-0.9.4/nodestream/pipeline/normalizers/lowercase_strings.py
--rw-r--r--   0        0        0     1845 2023-11-17 14:58:42.881723 nodestream-0.9.4/nodestream/pipeline/normalizers/normalizer.py
--rw-r--r--   0        0        0      249 2023-11-17 14:58:42.882157 nodestream-0.9.4/nodestream/pipeline/normalizers/remove_trailing_dots.py
--rw-r--r--   0        0        0      236 2023-11-17 14:58:42.882533 nodestream-0.9.4/nodestream/pipeline/normalizers/trim_whitespace.py
--rw-r--r--   0        0        0     8514 2023-12-13 17:19:01.784515 nodestream-0.9.4/nodestream/pipeline/pipeline.py
--rw-r--r--   0        0        0     4532 2023-12-18 19:07:38.228054 nodestream-0.9.4/nodestream/pipeline/pipeline_file_loader.py
--rw-r--r--   0        0        0     1993 2023-11-17 14:58:42.883715 nodestream-0.9.4/nodestream/pipeline/progress_reporter.py
--rw-r--r--   0        0        0     1244 2023-12-18 19:07:38.230243 nodestream-0.9.4/nodestream/pipeline/scope_config.py
--rw-r--r--   0        0        0      742 2023-11-17 14:58:42.884395 nodestream-0.9.4/nodestream/pipeline/step.py
--rw-r--r--   0        0        0      243 2023-12-08 21:42:10.810008 nodestream-0.9.4/nodestream/pipeline/transformers/__init__.py
--rw-r--r--   0        0        0      686 2023-11-17 14:58:42.885383 nodestream-0.9.4/nodestream/pipeline/transformers/expand_json_field.py
--rw-r--r--   0        0        0     5334 2023-12-18 19:07:41.886185 nodestream-0.9.4/nodestream/pipeline/transformers/transformer.py
--rw-r--r--   0        0        0      451 2023-11-17 14:58:42.886109 nodestream-0.9.4/nodestream/pipeline/transformers/value_projection.py
--rw-r--r--   0        0        0      883 2023-12-08 21:42:10.811914 nodestream-0.9.4/nodestream/pipeline/value_providers/__init__.py
--rw-r--r--   0        0        0     1171 2023-11-17 14:58:42.887150 nodestream-0.9.4/nodestream/pipeline/value_providers/context.py
--rw-r--r--   0        0        0     1551 2023-11-17 14:58:42.887493 nodestream-0.9.4/nodestream/pipeline/value_providers/jmespath_value_provider.py
--rw-r--r--   0        0        0     1493 2023-11-17 14:58:42.887900 nodestream-0.9.4/nodestream/pipeline/value_providers/mapping_value_provider.py
--rw-r--r--   0        0        0     1258 2023-11-17 14:58:42.888275 nodestream-0.9.4/nodestream/pipeline/value_providers/regex_value_provider.py
--rw-r--r--   0        0        0      968 2023-12-08 21:42:10.812415 nodestream-0.9.4/nodestream/pipeline/value_providers/split_value_provider.py
--rw-r--r--   0        0        0      774 2023-11-17 14:58:42.888613 nodestream-0.9.4/nodestream/pipeline/value_providers/static_value_provider.py
--rw-r--r--   0        0        0     1484 2023-11-17 14:58:42.888959 nodestream-0.9.4/nodestream/pipeline/value_providers/string_format_value_provider.py
--rw-r--r--   0        0        0     2279 2023-11-17 14:58:42.889298 nodestream-0.9.4/nodestream/pipeline/value_providers/value_provider.py
--rw-r--r--   0        0        0     1123 2023-11-17 14:58:42.889610 nodestream-0.9.4/nodestream/pipeline/value_providers/variable_value_provider.py
--rw-r--r--   0        0        0     1726 2023-11-17 14:58:42.889950 nodestream-0.9.4/nodestream/pipeline/writers.py
--rw-r--r--   0        0        0      790 2023-11-17 14:58:42.890290 nodestream-0.9.4/nodestream/pluggable.py
--rw-r--r--   0        0        0      331 2023-11-17 14:58:42.890803 nodestream-0.9.4/nodestream/project/__init__.py
--rw-r--r--   0        0        0      304 2023-11-17 14:58:42.891388 nodestream-0.9.4/nodestream/project/audits/__init__.py
--rw-r--r--   0        0        0     1623 2023-11-17 14:58:42.891764 nodestream-0.9.4/nodestream/project/audits/audit.py
--rw-r--r--   0        0        0      375 2023-11-17 14:58:42.892095 nodestream-0.9.4/nodestream/project/audits/audit_printer.py
--rw-r--r--   0        0        0     1751 2023-11-17 14:58:42.892454 nodestream-0.9.4/nodestream/project/audits/audit_referencial_integrity.py
--rw-r--r--   0        0        0     1641 2023-11-17 14:58:42.892821 nodestream-0.9.4/nodestream/project/audits/audit_ttls.py
--rw-r--r--   0        0        0     4146 2023-12-18 19:07:38.232341 nodestream-0.9.4/nodestream/project/pipeline_definition.py
--rw-r--r--   0        0        0     5445 2023-12-18 19:07:38.232925 nodestream-0.9.4/nodestream/project/pipeline_scope.py
--rw-r--r--   0        0        0    11050 2023-12-18 19:07:38.233495 nodestream-0.9.4/nodestream/project/project.py
--rw-r--r--   0        0        0     2370 2023-12-18 19:07:38.234027 nodestream-0.9.4/nodestream/project/run_request.py
--rw-r--r--   0        0        0      630 2023-12-18 19:07:38.234645 nodestream-0.9.4/nodestream/project/target.py
--rw-r--r--   0        0        0        0 2023-11-17 14:58:42.895384 nodestream-0.9.4/nodestream/schema/__init__.py
--rw-r--r--   0        0        0     1408 2023-11-17 14:58:42.895796 nodestream-0.9.4/nodestream/schema/indexes.py
--rw-r--r--   0        0        0      437 2023-11-17 14:58:42.896412 nodestream-0.9.4/nodestream/schema/printers/__init__.py
--rw-r--r--   0        0        0     1305 2023-11-17 14:58:42.896836 nodestream-0.9.4/nodestream/schema/printers/graph_schema_extraction.py
--rw-r--r--   0        0        0     5710 2023-11-17 14:58:42.897211 nodestream-0.9.4/nodestream/schema/printers/graphql_schema_printer.py
--rw-r--r--   0        0        0      272 2023-11-17 14:58:42.897606 nodestream-0.9.4/nodestream/schema/printers/plain_text_schema_printer.py
--rw-r--r--   0        0        0      853 2023-11-17 14:58:42.897992 nodestream-0.9.4/nodestream/schema/printers/schema_printer.py
--rw-r--r--   0        0        0    13990 2023-11-17 14:58:42.898391 nodestream-0.9.4/nodestream/schema/schema.py
--rw-r--r--   0        0        0     1879 2023-11-17 14:58:42.898831 nodestream-0.9.4/nodestream/subclass_registry.py
--rw-r--r--   0        0        0     3095 2023-12-18 19:08:07.578984 nodestream-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 nodestream-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-11-20 15:59:03.647873 nodestream-0.9.5/LICENSE
+-rw-r--r--   0        0        0     1774 2023-08-11 18:14:53.687256 nodestream-0.9.5/README.md
+-rw-r--r--   0        0        0        0 2023-08-11 18:14:53.698877 nodestream-0.9.5/nodestream/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-11 18:14:53.699354 nodestream-0.9.5/nodestream/cli/__init__.py
+-rw-r--r--   0        0        0      833 2023-11-20 15:59:17.063951 nodestream-0.9.5/nodestream/cli/application.py
+-rw-r--r--   0        0        0      429 2023-11-20 18:02:12.753136 nodestream-0.9.5/nodestream/cli/commands/__init__.py
+-rw-r--r--   0        0        0      780 2023-08-11 18:14:53.700554 nodestream-0.9.5/nodestream/cli/commands/audit_command.py
+-rw-r--r--   0        0        0     4292 2023-12-06 21:15:32.794586 nodestream-0.9.5/nodestream/cli/commands/copy.py
+-rw-r--r--   0        0        0      879 2023-08-11 18:14:53.701088 nodestream-0.9.5/nodestream/cli/commands/new.py
+-rw-r--r--   0        0        0     1387 2023-11-20 15:59:17.065322 nodestream-0.9.5/nodestream/cli/commands/nodestream_command.py
+-rw-r--r--   0        0        0     1213 2023-08-11 18:14:53.701798 nodestream-0.9.5/nodestream/cli/commands/print_schema.py
+-rw-r--r--   0        0        0      893 2023-08-11 18:14:53.701932 nodestream-0.9.5/nodestream/cli/commands/remove.py
+-rw-r--r--   0        0        0     1479 2023-12-04 20:33:43.484115 nodestream-0.9.5/nodestream/cli/commands/run.py
+-rw-r--r--   0        0        0     1426 2023-08-11 18:14:53.702809 nodestream-0.9.5/nodestream/cli/commands/scaffold.py
+-rw-r--r--   0        0        0      622 2023-12-04 20:33:43.487231 nodestream-0.9.5/nodestream/cli/commands/shared_options.py
+-rw-r--r--   0        0        0      596 2023-08-11 18:14:53.703023 nodestream-0.9.5/nodestream/cli/commands/show.py
+-rw-r--r--   0        0        0      962 2023-11-20 18:02:12.755453 nodestream-0.9.5/nodestream/cli/operations/__init__.py
+-rw-r--r--   0        0        0      988 2023-08-11 18:14:53.703717 nodestream-0.9.5/nodestream/cli/operations/add_pipeline_to_project.py
+-rw-r--r--   0        0        0      438 2023-08-11 18:14:53.704236 nodestream-0.9.5/nodestream/cli/operations/commit_project_to_disk.py
+-rw-r--r--   0        0        0     1843 2023-11-20 15:59:17.067293 nodestream-0.9.5/nodestream/cli/operations/generate_pipeline_scaffold.py
+-rw-r--r--   0        0        0     1153 2023-11-20 15:59:03.651212 nodestream-0.9.5/nodestream/cli/operations/initialize_logger.py
+-rw-r--r--   0        0        0      267 2023-08-11 18:14:53.705095 nodestream-0.9.5/nodestream/cli/operations/initialize_project.py
+-rw-r--r--   0        0        0      384 2023-08-11 18:14:53.705251 nodestream-0.9.5/nodestream/cli/operations/operation.py
+-rw-r--r--   0        0        0     1251 2023-09-12 22:33:21.735532 nodestream-0.9.5/nodestream/cli/operations/print_project_schema.py
+-rw-r--r--   0        0        0      533 2023-08-11 18:14:53.705735 nodestream-0.9.5/nodestream/cli/operations/remove_pipeline_from_project.py
+-rw-r--r--   0        0        0     1145 2023-08-11 18:14:53.705859 nodestream-0.9.5/nodestream/cli/operations/run_audit.py
+-rw-r--r--   0        0        0     1288 2023-12-06 21:15:32.795839 nodestream-0.9.5/nodestream/cli/operations/run_copy.py
+-rw-r--r--   0        0        0     4636 2023-12-04 20:33:43.493234 nodestream-0.9.5/nodestream/cli/operations/run_pipeline.py
+-rw-r--r--   0        0        0      866 2023-08-11 18:14:53.706422 nodestream-0.9.5/nodestream/cli/operations/run_project_cookiecutter.py
+-rw-r--r--   0        0        0     2436 2023-08-11 18:14:53.707141 nodestream-0.9.5/nodestream/cli/operations/show_pipelines.py
+-rw-r--r--   0        0        0      622 2023-12-08 00:16:47.186050 nodestream-0.9.5/nodestream/compat.py
+-rw-r--r--   0        0        0      326 2023-11-20 18:02:12.759281 nodestream-0.9.5/nodestream/databases/__init__.py
+-rw-r--r--   0        0        0     2578 2023-12-06 21:15:32.797043 nodestream-0.9.5/nodestream/databases/copy.py
+-rw-r--r--   0        0        0     1349 2023-11-20 18:02:12.761844 nodestream-0.9.5/nodestream/databases/database_connector.py
+-rw-r--r--   0        0        0     3401 2023-12-04 20:34:57.311397 nodestream-0.9.5/nodestream/databases/debounced_ingest_strategy.py
+-rw-r--r--   0        0        0     2628 2023-08-11 18:14:53.707910 nodestream-0.9.5/nodestream/databases/ingest_strategy.py
+-rw-r--r--   0        0        0       94 2023-09-07 14:02:55.138774 nodestream-0.9.5/nodestream/databases/neo4j/__init__.py
+-rw-r--r--   0        0        0     1952 2023-11-20 18:02:12.764764 nodestream-0.9.5/nodestream/databases/neo4j/database_connector.py
+-rw-r--r--   0        0        0     2005 2023-11-20 18:02:12.765863 nodestream-0.9.5/nodestream/databases/neo4j/extractor.py
+-rw-r--r--   0        0        0     2710 2023-08-11 18:14:53.708927 nodestream-0.9.5/nodestream/databases/neo4j/index_query_builder.py
+-rw-r--r--   0        0        0     9693 2023-12-18 17:28:14.553580 nodestream-0.9.5/nodestream/databases/neo4j/ingest_query_builder.py
+-rw-r--r--   0        0        0     1788 2023-11-20 15:59:17.072535 nodestream-0.9.5/nodestream/databases/neo4j/query.py
+-rw-r--r--   0        0        0     3326 2023-12-18 17:28:14.555058 nodestream-0.9.5/nodestream/databases/neo4j/query_executor.py
+-rw-r--r--   0        0        0     2679 2023-12-06 21:15:32.798179 nodestream-0.9.5/nodestream/databases/neo4j/type_retriever.py
+-rw-r--r--   0        0        0     3472 2023-11-20 18:02:12.769032 nodestream-0.9.5/nodestream/databases/operation_debouncer.py
+-rw-r--r--   0        0        0     1691 2023-11-20 18:02:12.770492 nodestream-0.9.5/nodestream/databases/query_executor.py
+-rw-r--r--   0        0        0     2044 2023-08-11 18:14:53.711009 nodestream-0.9.5/nodestream/databases/query_executor_with_statistics.py
+-rw-r--r--   0        0        0     1667 2023-11-20 18:02:12.771534 nodestream-0.9.5/nodestream/databases/writer.py
+-rw-r--r--   0        0        0     3566 2023-08-11 18:14:53.711763 nodestream-0.9.5/nodestream/file_io.py
+-rw-r--r--   0        0        0      137 2023-08-11 18:14:53.711900 nodestream-0.9.5/nodestream/interpreting/__init__.py
+-rw-r--r--   0        0        0      574 2023-08-11 18:14:53.712074 nodestream-0.9.5/nodestream/interpreting/interpretations/__init__.py
+-rw-r--r--   0        0        0     1369 2023-08-11 18:14:53.712274 nodestream-0.9.5/nodestream/interpreting/interpretations/extract_variables_interpretation.py
+-rw-r--r--   0        0        0      948 2023-11-20 17:16:08.192247 nodestream-0.9.5/nodestream/interpreting/interpretations/interpretation.py
+-rw-r--r--   0        0        0     1262 2023-08-11 18:14:53.713029 nodestream-0.9.5/nodestream/interpreting/interpretations/properties_interpretation.py
+-rw-r--r--   0        0        0    10429 2023-11-20 18:02:12.772517 nodestream-0.9.5/nodestream/interpreting/interpretations/relationship_interpretation.py
+-rw-r--r--   0        0        0     4469 2023-08-11 18:14:53.713347 nodestream-0.9.5/nodestream/interpreting/interpretations/source_node_interpretation.py
+-rw-r--r--   0        0        0     2627 2023-09-21 21:16:04.380022 nodestream-0.9.5/nodestream/interpreting/interpretations/switch_interpretation.py
+-rw-r--r--   0        0        0     4820 2023-10-04 19:47:46.896130 nodestream-0.9.5/nodestream/interpreting/interpreter.py
+-rw-r--r--   0        0        0     1744 2023-08-11 18:14:53.714052 nodestream-0.9.5/nodestream/interpreting/record_decomposers.py
+-rw-r--r--   0        0        0      787 2023-11-20 18:02:12.773763 nodestream-0.9.5/nodestream/model/__init__.py
+-rw-r--r--   0        0        0      381 2023-11-20 18:02:12.774838 nodestream-0.9.5/nodestream/model/creation_rules.py
+-rw-r--r--   0        0        0     3739 2023-12-06 21:15:38.477676 nodestream-0.9.5/nodestream/model/desired_ingestion.py
+-rw-r--r--   0        0        0     7728 2023-11-20 18:02:12.777372 nodestream-0.9.5/nodestream/model/graph_objects.py
+-rw-r--r--   0        0        0      873 2023-08-11 18:14:53.714662 nodestream-0.9.5/nodestream/model/ingestion_hooks.py
+-rw-r--r--   0        0        0      851 2023-08-11 18:14:53.715350 nodestream-0.9.5/nodestream/model/ttl.py
+-rw-r--r--   0        0        0     1023 2023-11-20 17:47:37.303126 nodestream-0.9.5/nodestream/pipeline/__init__.py
+-rw-r--r--   0        0        0      321 2023-11-20 16:11:21.352524 nodestream-0.9.5/nodestream/pipeline/argument_resolvers/__init__.py
+-rw-r--r--   0        0        0      531 2023-08-11 18:14:53.716081 nodestream-0.9.5/nodestream/pipeline/argument_resolvers/argument_resolver.py
+-rw-r--r--   0        0        0      604 2023-09-12 22:33:21.742651 nodestream-0.9.5/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py
+-rw-r--r--   0        0        0      676 2023-09-07 14:02:55.148412 nodestream-0.9.5/nodestream/pipeline/argument_resolvers/include_file_resolver.py
+-rw-r--r--   0        0        0     2474 2023-11-20 15:59:03.656965 nodestream-0.9.5/nodestream/pipeline/class_loader.py
+-rw-r--r--   0        0        0      386 2023-11-20 15:59:17.073445 nodestream-0.9.5/nodestream/pipeline/extractors/__init__.py
+-rw-r--r--   0        0        0     1306 2023-09-07 14:02:55.150562 nodestream-0.9.5/nodestream/pipeline/extractors/apis.py
+-rw-r--r--   0        0        0      678 2023-08-11 18:14:53.717834 nodestream-0.9.5/nodestream/pipeline/extractors/extractor.py
+-rw-r--r--   0        0        0     4307 2023-11-20 15:59:17.074403 nodestream-0.9.5/nodestream/pipeline/extractors/files.py
+-rw-r--r--   0        0        0      546 2023-08-11 18:14:53.718249 nodestream-0.9.5/nodestream/pipeline/extractors/iterable.py
+-rw-r--r--   0        0        0        0 2023-08-11 18:14:53.718323 nodestream-0.9.5/nodestream/pipeline/extractors/stores/__init__.py
+-rw-r--r--   0        0        0      130 2023-08-11 18:14:53.718446 nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/__init__.py
+-rw-r--r--   0        0        0     4613 2023-11-20 15:59:17.074897 nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/athena_extractor.py
+-rw-r--r--   0        0        0     2503 2023-11-20 15:59:03.658841 nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/credential_utils.py
+-rw-r--r--   0        0        0     3267 2023-09-12 22:33:21.743997 nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/s3_extractor.py
+-rw-r--r--   0        0        0      231 2023-08-11 18:14:53.719372 nodestream-0.9.5/nodestream/pipeline/extractors/streams/__init__.py
+-rw-r--r--   0        0        0     3167 2023-11-20 15:59:17.075374 nodestream-0.9.5/nodestream/pipeline/extractors/streams/extractor.py
+-rw-r--r--   0        0        0     3529 2023-11-20 15:59:17.075882 nodestream-0.9.5/nodestream/pipeline/extractors/streams/kafka.py
+-rw-r--r--   0        0        0      646 2023-08-11 18:14:53.719963 nodestream-0.9.5/nodestream/pipeline/extractors/ttls.py
+-rw-r--r--   0        0        0     5015 2023-11-20 17:47:37.305197 nodestream-0.9.5/nodestream/pipeline/filters.py
+-rw-r--r--   0        0        0       22 2023-08-11 18:14:53.720151 nodestream-0.9.5/nodestream/pipeline/flush.py
+-rw-r--r--   0        0        0      869 2023-08-11 18:14:53.720419 nodestream-0.9.5/nodestream/pipeline/meta.py
+-rw-r--r--   0        0        0      327 2023-08-11 18:14:53.720615 nodestream-0.9.5/nodestream/pipeline/normalizers/__init__.py
+-rw-r--r--   0        0        0      240 2023-08-11 18:14:53.721142 nodestream-0.9.5/nodestream/pipeline/normalizers/lowercase_strings.py
+-rw-r--r--   0        0        0     1845 2023-08-11 18:14:53.721523 nodestream-0.9.5/nodestream/pipeline/normalizers/normalizer.py
+-rw-r--r--   0        0        0      249 2023-08-11 18:14:53.721987 nodestream-0.9.5/nodestream/pipeline/normalizers/remove_trailing_dots.py
+-rw-r--r--   0        0        0      236 2023-08-11 18:14:53.722315 nodestream-0.9.5/nodestream/pipeline/normalizers/trim_whitespace.py
+-rw-r--r--   0        0        0     9714 2023-12-20 18:43:09.926406 nodestream-0.9.5/nodestream/pipeline/pipeline.py
+-rw-r--r--   0        0        0     4532 2023-11-20 15:59:17.077596 nodestream-0.9.5/nodestream/pipeline/pipeline_file_loader.py
+-rw-r--r--   0        0        0     1993 2023-11-20 15:59:17.078026 nodestream-0.9.5/nodestream/pipeline/progress_reporter.py
+-rw-r--r--   0        0        0     1244 2023-09-13 22:35:56.141344 nodestream-0.9.5/nodestream/pipeline/scope_config.py
+-rw-r--r--   0        0        0      742 2023-08-11 18:14:53.723648 nodestream-0.9.5/nodestream/pipeline/step.py
+-rw-r--r--   0        0        0      243 2023-12-18 17:28:14.559313 nodestream-0.9.5/nodestream/pipeline/transformers/__init__.py
+-rw-r--r--   0        0        0      686 2023-08-11 18:14:53.724497 nodestream-0.9.5/nodestream/pipeline/transformers/expand_json_field.py
+-rw-r--r--   0        0        0     5334 2023-12-18 17:28:14.560888 nodestream-0.9.5/nodestream/pipeline/transformers/transformer.py
+-rw-r--r--   0        0        0      451 2023-08-11 18:14:53.724819 nodestream-0.9.5/nodestream/pipeline/transformers/value_projection.py
+-rw-r--r--   0        0        0      883 2023-11-20 15:59:17.079291 nodestream-0.9.5/nodestream/pipeline/value_providers/__init__.py
+-rw-r--r--   0        0        0     1171 2023-08-11 18:14:53.725380 nodestream-0.9.5/nodestream/pipeline/value_providers/context.py
+-rw-r--r--   0        0        0     1551 2023-11-20 15:59:17.080353 nodestream-0.9.5/nodestream/pipeline/value_providers/jmespath_value_provider.py
+-rw-r--r--   0        0        0     1493 2023-11-20 15:59:17.081245 nodestream-0.9.5/nodestream/pipeline/value_providers/mapping_value_provider.py
+-rw-r--r--   0        0        0     1258 2023-11-20 15:59:17.082057 nodestream-0.9.5/nodestream/pipeline/value_providers/regex_value_provider.py
+-rw-r--r--   0        0        0      968 2023-11-20 15:59:17.082330 nodestream-0.9.5/nodestream/pipeline/value_providers/split_value_provider.py
+-rw-r--r--   0        0        0      774 2023-11-20 15:59:17.083344 nodestream-0.9.5/nodestream/pipeline/value_providers/static_value_provider.py
+-rw-r--r--   0        0        0     1484 2023-11-20 15:59:17.084437 nodestream-0.9.5/nodestream/pipeline/value_providers/string_format_value_provider.py
+-rw-r--r--   0        0        0     2279 2023-08-11 18:14:53.726993 nodestream-0.9.5/nodestream/pipeline/value_providers/value_provider.py
+-rw-r--r--   0        0        0     1123 2023-11-20 15:59:17.085312 nodestream-0.9.5/nodestream/pipeline/value_providers/variable_value_provider.py
+-rw-r--r--   0        0        0     1726 2023-08-11 18:14:53.727484 nodestream-0.9.5/nodestream/pipeline/writers.py
+-rw-r--r--   0        0        0      790 2023-09-13 22:35:56.142474 nodestream-0.9.5/nodestream/pluggable.py
+-rw-r--r--   0        0        0      331 2023-11-20 15:59:17.086104 nodestream-0.9.5/nodestream/project/__init__.py
+-rw-r--r--   0        0        0      304 2023-08-11 18:14:53.728781 nodestream-0.9.5/nodestream/project/audits/__init__.py
+-rw-r--r--   0        0        0     1623 2023-08-11 18:14:53.729262 nodestream-0.9.5/nodestream/project/audits/audit.py
+-rw-r--r--   0        0        0      375 2023-08-11 18:14:53.729600 nodestream-0.9.5/nodestream/project/audits/audit_printer.py
+-rw-r--r--   0        0        0     1751 2023-08-11 18:14:53.729939 nodestream-0.9.5/nodestream/project/audits/audit_referencial_integrity.py
+-rw-r--r--   0        0        0     1641 2023-08-11 18:14:53.730432 nodestream-0.9.5/nodestream/project/audits/audit_ttls.py
+-rw-r--r--   0        0        0     4146 2023-09-13 22:35:56.143006 nodestream-0.9.5/nodestream/project/pipeline_definition.py
+-rw-r--r--   0        0        0     5445 2023-11-20 15:59:03.660506 nodestream-0.9.5/nodestream/project/pipeline_scope.py
+-rw-r--r--   0        0        0    11050 2023-12-07 19:00:42.232349 nodestream-0.9.5/nodestream/project/project.py
+-rw-r--r--   0        0        0     2370 2023-09-13 22:35:56.146497 nodestream-0.9.5/nodestream/project/run_request.py
+-rw-r--r--   0        0        0      630 2023-11-20 18:02:12.778604 nodestream-0.9.5/nodestream/project/target.py
+-rw-r--r--   0        0        0        0 2023-08-11 18:14:53.731765 nodestream-0.9.5/nodestream/schema/__init__.py
+-rw-r--r--   0        0        0     1408 2023-08-11 18:14:53.731908 nodestream-0.9.5/nodestream/schema/indexes.py
+-rw-r--r--   0        0        0      437 2023-09-07 14:02:55.164486 nodestream-0.9.5/nodestream/schema/printers/__init__.py
+-rw-r--r--   0        0        0     1305 2023-09-07 14:02:55.165333 nodestream-0.9.5/nodestream/schema/printers/graph_schema_extraction.py
+-rw-r--r--   0        0        0     5710 2023-08-11 18:14:53.732900 nodestream-0.9.5/nodestream/schema/printers/graphql_schema_printer.py
+-rw-r--r--   0        0        0      272 2023-08-11 18:14:53.733372 nodestream-0.9.5/nodestream/schema/printers/plain_text_schema_printer.py
+-rw-r--r--   0        0        0      853 2023-09-12 22:33:21.751368 nodestream-0.9.5/nodestream/schema/printers/schema_printer.py
+-rw-r--r--   0        0        0    13990 2023-09-07 14:02:55.167382 nodestream-0.9.5/nodestream/schema/schema.py
+-rw-r--r--   0        0        0     1879 2023-11-20 17:16:08.194056 nodestream-0.9.5/nodestream/subclass_registry.py
+-rw-r--r--   0        0        0     3095 2023-12-20 18:43:28.025211 nodestream-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 nodestream-0.9.5/PKG-INFO
```

### Comparing `nodestream-0.9.4/LICENSE` & `nodestream-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/README.md` & `nodestream-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/application.py` & `nodestream-0.9.5/nodestream/cli/application.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/audit_command.py` & `nodestream-0.9.5/nodestream/cli/commands/audit_command.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/copy.py` & `nodestream-0.9.5/nodestream/cli/commands/copy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/new.py` & `nodestream-0.9.5/nodestream/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/nodestream_command.py` & `nodestream-0.9.5/nodestream/cli/commands/nodestream_command.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/print_schema.py` & `nodestream-0.9.5/nodestream/cli/commands/print_schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/remove.py` & `nodestream-0.9.5/nodestream/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/run.py` & `nodestream-0.9.5/nodestream/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/scaffold.py` & `nodestream-0.9.5/nodestream/cli/commands/scaffold.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/shared_options.py` & `nodestream-0.9.5/nodestream/cli/commands/shared_options.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/commands/show.py` & `nodestream-0.9.5/nodestream/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/__init__.py` & `nodestream-0.9.5/nodestream/cli/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/add_pipeline_to_project.py` & `nodestream-0.9.5/nodestream/cli/operations/add_pipeline_to_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/generate_pipeline_scaffold.py` & `nodestream-0.9.5/nodestream/cli/operations/generate_pipeline_scaffold.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/initialize_logger.py` & `nodestream-0.9.5/nodestream/cli/operations/initialize_logger.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/print_project_schema.py` & `nodestream-0.9.5/nodestream/cli/operations/print_project_schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/remove_pipeline_from_project.py` & `nodestream-0.9.5/nodestream/cli/operations/remove_pipeline_from_project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/run_audit.py` & `nodestream-0.9.5/nodestream/cli/operations/run_audit.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/run_copy.py` & `nodestream-0.9.5/nodestream/cli/operations/run_copy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/run_pipeline.py` & `nodestream-0.9.5/nodestream/cli/operations/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/run_project_cookiecutter.py` & `nodestream-0.9.5/nodestream/cli/operations/run_project_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/cli/operations/show_pipelines.py` & `nodestream-0.9.5/nodestream/cli/operations/show_pipelines.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/compat.py` & `nodestream-0.9.5/nodestream/compat.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/copy.py` & `nodestream-0.9.5/nodestream/databases/copy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/database_connector.py` & `nodestream-0.9.5/nodestream/databases/database_connector.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/debounced_ingest_strategy.py` & `nodestream-0.9.5/nodestream/databases/debounced_ingest_strategy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/ingest_strategy.py` & `nodestream-0.9.5/nodestream/databases/ingest_strategy.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/database_connector.py` & `nodestream-0.9.5/nodestream/databases/neo4j/database_connector.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/extractor.py` & `nodestream-0.9.5/nodestream/databases/neo4j/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/index_query_builder.py` & `nodestream-0.9.5/nodestream/databases/neo4j/index_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/ingest_query_builder.py` & `nodestream-0.9.5/nodestream/databases/neo4j/ingest_query_builder.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/query.py` & `nodestream-0.9.5/nodestream/databases/neo4j/query.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/query_executor.py` & `nodestream-0.9.5/nodestream/databases/neo4j/query_executor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/neo4j/type_retriever.py` & `nodestream-0.9.5/nodestream/databases/neo4j/type_retriever.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/operation_debouncer.py` & `nodestream-0.9.5/nodestream/databases/operation_debouncer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/query_executor.py` & `nodestream-0.9.5/nodestream/databases/query_executor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/query_executor_with_statistics.py` & `nodestream-0.9.5/nodestream/databases/query_executor_with_statistics.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/databases/writer.py` & `nodestream-0.9.5/nodestream/databases/writer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/file_io.py` & `nodestream-0.9.5/nodestream/file_io.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/__init__.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/extract_variables_interpretation.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/extract_variables_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/interpretation.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/properties_interpretation.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/properties_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/relationship_interpretation.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/relationship_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/source_node_interpretation.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/source_node_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpretations/switch_interpretation.py` & `nodestream-0.9.5/nodestream/interpreting/interpretations/switch_interpretation.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/interpreter.py` & `nodestream-0.9.5/nodestream/interpreting/interpreter.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/interpreting/record_decomposers.py` & `nodestream-0.9.5/nodestream/interpreting/record_decomposers.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/model/__init__.py` & `nodestream-0.9.5/nodestream/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/model/desired_ingestion.py` & `nodestream-0.9.5/nodestream/model/desired_ingestion.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/model/graph_objects.py` & `nodestream-0.9.5/nodestream/model/graph_objects.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/model/ingestion_hooks.py` & `nodestream-0.9.5/nodestream/model/ingestion_hooks.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/model/ttl.py` & `nodestream-0.9.5/nodestream/model/ttl.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/__init__.py` & `nodestream-0.9.5/nodestream/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/argument_resolvers/argument_resolver.py` & `nodestream-0.9.5/nodestream/pipeline/argument_resolvers/argument_resolver.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py` & `nodestream-0.9.5/nodestream/pipeline/argument_resolvers/environment_variable_resolver.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/argument_resolvers/include_file_resolver.py` & `nodestream-0.9.5/nodestream/pipeline/argument_resolvers/include_file_resolver.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/class_loader.py` & `nodestream-0.9.5/nodestream/pipeline/class_loader.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/apis.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/apis.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/extractor.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/files.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/files.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/iterable.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/iterable.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/athena_extractor.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/athena_extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/credential_utils.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/credential_utils.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/stores/aws/s3_extractor.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/stores/aws/s3_extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/streams/extractor.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/streams/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/streams/kafka.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/streams/kafka.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/extractors/ttls.py` & `nodestream-0.9.5/nodestream/pipeline/extractors/ttls.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/filters.py` & `nodestream-0.9.5/nodestream/pipeline/filters.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/meta.py` & `nodestream-0.9.5/nodestream/pipeline/meta.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/normalizers/normalizer.py` & `nodestream-0.9.5/nodestream/pipeline/normalizers/normalizer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/pipeline.py` & `nodestream-0.9.5/nodestream/pipeline/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 class DoneObject:
     pass
 
 
 START_EXCEPTION = "Exception in Start Process:"
 WORK_BODY_EXCEPTION = "Exception in Work Body:"
 STOP_EXCEPTION = "Exception in Stop Process:"
+OUTBOX_POLL_TIME = 0.1
 
 
 class StepException(Exception):
     """
     Exception Format:
         Exceptions in StepExecutor {exec_num} ({step_name})
             Exception in Start
@@ -60,14 +61,18 @@
             for sentence in [
                 "\t\t" + sentence + "\n" for sentence in sub_message.split("\n")
             ]:
                 message += sentence
         return f"Exceptions in {self.identifier}:\n" + message
 
 
+class ForwardProgressHalted(Exception):
+    pass
+
+
 class PipelineException(Exception):
     """
     Exception in Pipeline:
         Output from StepException 0
         Output from StepException 1
     """
 
@@ -86,23 +91,33 @@
             "\t" + sentence + "\n" for sentence in sub_message.split("\n")
         ]:
             message += sentence
 
         return "Exceptions in Pipeline:\n" + message
 
 
+class PipelineState:
+    def __init__(self) -> None:
+        self.has_fatal_error = False
+
+    def signal_fatal_error(self):
+        self.has_fatal_error = True
+
+
 class StepExecutor:
     def __init__(
         self,
+        pipeline_state: PipelineState,
         upstream: Optional["StepExecutor"],
         step: Step,
         outbox_size: int = 0,
         step_index: Optional[int] = 0,
         progress_reporter: Optional[PipelineProgressReporter] = None,
     ) -> None:
+        self.pipeline_state = pipeline_state
         self.outbox = asyncio.Queue(maxsize=outbox_size)
         self.upstream = upstream
         self.done = False
         self.step = step
         self.step_index = step_index
         self.progress_reporter = progress_reporter
         self.end_of_line = False
@@ -120,31 +135,47 @@
         if self.progress_reporter:
             self.progress_reporter.on_start_callback()
 
     def set_end_of_line(self, progress_reporter: Optional[PipelineProgressReporter]):
         self.progress_reporter = progress_reporter
         self.end_of_line = True
 
+    def pipeline_has_died(self) -> bool:
+        return self.pipeline_state.has_fatal_error
+
+    async def submit_object_or_die_trying(self, obj):
+        should_continue = True
+        while should_continue:
+            try:
+                await asyncio.wait_for(self.outbox.put(obj), timeout=OUTBOX_POLL_TIME)
+                should_continue = False
+            except asyncio.TimeoutError:
+                # We timed out, now we need to check if the pipeline has died and if so, raise an exception.
+                if self.pipeline_has_died():
+                    raise ForwardProgressHalted(
+                        "Because of a fatal error in the pipeline, this step can no longer continue."
+                    )
+
     async def stop(self):
         self.done = True
-        await self.outbox.put(DoneObject)
+        await self.submit_object_or_die_trying(DoneObject)
         await self.step.finish()
 
         if self.progress_reporter:
             self.progress_reporter.on_finish_callback(get_context())
 
     async def work_body(self):
         if self.upstream is None:
             upstream = empty_async_generator()
         else:
             upstream = self.upstream.outbox_generator()
         results = self.step.handle_async_record_stream(upstream)
         async for index, record in enumerate_async(results):
             if not self.end_of_line:
-                await self.outbox.put(record)
+                await self.submit_object_or_die_trying(record)
             if self.progress_reporter:
                 self.progress_reporter.report(index, record)
 
     def try_start(self):
         # Start only calls some callbacks on the reporter.
         # If this fails, we can just log the error and move on.
         try:
@@ -185,14 +216,15 @@
                 stack_info=True,
                 extra={"step": self.step.__class__.__name__},
             )
             self.exceptions[STOP_EXCEPTION] = stop_exception
 
     def raise_encountered_exceptions(self):
         if self.exceptions:
+            self.pipeline_state.signal_fatal_error()
             raise StepException(errors=self.exceptions, identifier=self.identifier)
 
     async def work_loop(self):
         self.try_start()
         await self.try_work_body()
         await self.try_stop()
         self.raise_encountered_exceptions()
@@ -210,16 +242,18 @@
         self.errors = []
 
     def build_steps_into_tasks(
         self, progress_reporter: Optional[PipelineProgressReporter] = None
     ):
         current_executor = None
         tasks = []
+        state = PipelineState()
         for step_index, step in enumerate(self.steps):
             current_executor = StepExecutor(
+                pipeline_state=state,
                 upstream=current_executor,
                 step=step,
                 outbox_size=self.step_outbox_size,
                 step_index=step_index,
             )
             tasks.append(asyncio.create_task(current_executor.work_loop()))
         current_executor.set_end_of_line(progress_reporter)
```

### Comparing `nodestream-0.9.4/nodestream/pipeline/pipeline_file_loader.py` & `nodestream-0.9.5/nodestream/pipeline/pipeline_file_loader.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/progress_reporter.py` & `nodestream-0.9.5/nodestream/pipeline/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/scope_config.py` & `nodestream-0.9.5/nodestream/pipeline/scope_config.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/step.py` & `nodestream-0.9.5/nodestream/pipeline/step.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/transformers/expand_json_field.py` & `nodestream-0.9.5/nodestream/pipeline/transformers/expand_json_field.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/transformers/transformer.py` & `nodestream-0.9.5/nodestream/pipeline/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/__init__.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/context.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/context.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/jmespath_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/jmespath_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/mapping_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/mapping_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/regex_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/regex_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/split_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/split_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/static_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/static_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/string_format_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/string_format_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/value_providers/variable_value_provider.py` & `nodestream-0.9.5/nodestream/pipeline/value_providers/variable_value_provider.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pipeline/writers.py` & `nodestream-0.9.5/nodestream/pipeline/writers.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/pluggable.py` & `nodestream-0.9.5/nodestream/pluggable.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/audits/audit.py` & `nodestream-0.9.5/nodestream/project/audits/audit.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/audits/audit_referencial_integrity.py` & `nodestream-0.9.5/nodestream/project/audits/audit_referencial_integrity.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/audits/audit_ttls.py` & `nodestream-0.9.5/nodestream/project/audits/audit_ttls.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/pipeline_definition.py` & `nodestream-0.9.5/nodestream/project/pipeline_definition.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/pipeline_scope.py` & `nodestream-0.9.5/nodestream/project/pipeline_scope.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/project.py` & `nodestream-0.9.5/nodestream/project/project.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/run_request.py` & `nodestream-0.9.5/nodestream/project/run_request.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/project/target.py` & `nodestream-0.9.5/nodestream/project/target.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/schema/indexes.py` & `nodestream-0.9.5/nodestream/schema/indexes.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/schema/printers/graph_schema_extraction.py` & `nodestream-0.9.5/nodestream/schema/printers/graph_schema_extraction.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/schema/printers/graphql_schema_printer.py` & `nodestream-0.9.5/nodestream/schema/printers/graphql_schema_printer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/schema/printers/schema_printer.py` & `nodestream-0.9.5/nodestream/schema/printers/schema_printer.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/schema/schema.py` & `nodestream-0.9.5/nodestream/schema/schema.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/nodestream/subclass_registry.py` & `nodestream-0.9.5/nodestream/subclass_registry.py`

 * *Files identical despite different names*

### Comparing `nodestream-0.9.4/pyproject.toml` & `nodestream-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nodestream"
-version = "0.9.4"
+version = "0.9.5"
 description = "A Fast, Declarative ETL for Graph Databases."
 license = "GPL-3.0-only"
 authors = [
     "Zach Probst <Zach_Probst@intuit.com>"
 ]
 readme = "README.md"
```

### Comparing `nodestream-0.9.4/PKG-INFO` & `nodestream-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodestream
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Fast, Declarative ETL for Graph Databases.
 Home-page: https://github.com/nodestream-proj/nodestream
 License: GPL-3.0-only
 Keywords: etl,neo4j,declarative,data,kafka,ingest
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
```

