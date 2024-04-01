# Comparing `tmp/dcicsnovault-9.1.1.tar.gz` & `tmp/dcicsnovault-9.9.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-9.1.1.tar", max compression
+gzip compressed data, was "dcicsnovault-9.9.9.0b0.tar", max compression
```

## Comparing `dcicsnovault-9.1.1.tar` & `dcicsnovault-9.9.9.0b0.tar`

### file list

```diff
@@ -1,189 +1,193 @@
--rw-r--r--   0        0        0     1135 2023-08-03 17:06:56.199490 dcicsnovault-9.1.1/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-08-03 17:06:56.199490 dcicsnovault-9.1.1/README.rst
--rw-r--r--   0        0        0     5549 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/pyproject.toml
--rw-r--r--   0        0        0     4901 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/aggregated_items.py
--rw-r--r--   0        0        0     9383 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/app.py
--rw-r--r--   0        0        0      358 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/appdefs.py
--rw-r--r--   0        0        0    11879 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/attachment.py
--rw-r--r--   0        0        0    26425 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/authentication.py
--rw-r--r--   0        0        0     4692 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6876 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5839 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2438 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-08-03 17:06:56.207491 dcicsnovault-9.1.1/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/custom_embed.py
--rw-r--r--   0        0        0     7282 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0    11485 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/indexing_views.py
--rw-r--r--   0        0        0     6889 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/common.py
--rw-r--r--   0        0        0     1294 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/exceptions.py
--rw-r--r--   0        0        0    26153 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_listener.py
--rw-r--r--   0        0        0      586 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_listener_base.py
--rw-r--r--   0        0        0      692 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_message.py
--rw-r--r--   0        0        0    12257 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_message_handler_decorator.py
--rw-r--r--   0        0        0     3760 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_message_handler_default.py
--rw-r--r--   0        0        0     1107 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_processor_decorator.py
--rw-r--r--   0        0        0      863 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/ingestion_processors.py
--rw-r--r--   0        0        0     8586 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/ingestion/queue_utils.py
--rw-r--r--   0        0        0      774 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/jsonld_context.py
--rw-r--r--   0        0        0    32979 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/loadxl.py
--rw-r--r--   0        0        0     4847 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/local_roles.py
--rw-r--r--   0        0        0     2425 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/memlimit.py
--rw-r--r--   0        0        0      229 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/mime_types.py
--rw-r--r--   0        0        0      895 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/predicates.py
--rw-r--r--   0        0        0       98 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project/access_key.py
--rw-r--r--   0        0        0     1520 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project/authentication.py
--rw-r--r--   0        0        0      378 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project/authorization.py
--rw-r--r--   0        0        0      289 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project/ingestion.py
--rw-r--r--   0        0        0      228 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project/loadxl.py
--rw-r--r--   0        0        0      378 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project/renderers.py
--rw-r--r--   0        0        0      107 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project_app.py
--rw-r--r--   0        0        0      879 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/project_defs.py
--rw-r--r--   0        0        0       95 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22536 2023-08-03 17:06:56.211490 dcicsnovault-9.1.1/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/resource_views.py
--rw-r--r--   0        0        0    26761 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/resources.py
--rw-r--r--   0        0        0     9867 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/root.py
--rw-r--r--   0        0        0      986 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schema_formats.py
--rw-r--r--   0        0        0     3450 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schema_graph.py
--rw-r--r--   0        0        0    18330 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0     5407 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schemas/ingestion_submission.json
--rw-r--r--   0        0        0    18744 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/search/search.py
--rw-r--r--   0        0        0    17915 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/search/search_utils.py
--rw-r--r--   0        0        0     2644 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/server_defaults.py
--rw-r--r--   0        0        0     1615 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/server_defaults_misc.py
--rw-r--r--   0        0        0      983 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/server_defaults_user.py
--rw-r--r--   0        0        0      522 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2199 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-08-03 17:06:56.215490 dcicsnovault-9.1.1/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3186 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0     8173 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_ingestion_message_handler_decorator.py
--rw-r--r--   0        0        0      384 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_ingestion_processor.py
--rw-r--r--   0        0        0    28258 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     9709 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_renderers.py
--rw-r--r--   0        0        0     1194 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     1291 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_util.py
--rw-r--r--   0        0        0    19246 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4620 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/__init__.py
--rw-r--r--   0        0        0     5132 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/access_key.py
--rw-r--r--   0        0        0     1169 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/acl.py
--rw-r--r--   0        0        0     8751 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/filter_set.py
--rw-r--r--   0        0        0    11521 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/ingestion.py
--rw-r--r--   0        0        0     5638 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-08-03 17:06:56.219491 dcicsnovault-9.1.1/snovault/upgrader.py
--rw-r--r--   0        0        0    63565 2023-08-03 17:06:56.223491 dcicsnovault-9.1.1/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-08-03 17:06:56.223491 dcicsnovault-9.1.1/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-08-03 17:06:56.223491 dcicsnovault-9.1.1/snovault/validators.py
--rw-r--r--   0        0        0     9133 1970-01-01 00:00:00.000000 dcicsnovault-9.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-08-03 13:44:04.654938 dcicsnovault-9.9.9.0b0/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-08-03 13:44:04.654938 dcicsnovault-9.9.9.0b0/README.rst
+-rw-r--r--   0        0        0     5539 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/pyproject.toml
+-rw-r--r--   0        0        0     4901 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     9383 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/app.py
+-rw-r--r--   0        0        0      358 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/appdefs.py
+-rw-r--r--   0        0        0    11879 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/attachment.py
+-rw-r--r--   0        0        0    26351 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/authentication.py
+-rw-r--r--   0        0        0     4692 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6876 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5839 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2438 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7282 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-08-03 13:44:04.662938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0    11485 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/indexing_views.py
+-rw-r--r--   0        0        0     6889 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/common.py
+-rw-r--r--   0        0        0     1294 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/exceptions.py
+-rw-r--r--   0        0        0    26153 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_listener.py
+-rw-r--r--   0        0        0      586 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_listener_base.py
+-rw-r--r--   0        0        0      692 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_message.py
+-rw-r--r--   0        0        0    12257 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_message_handler_decorator.py
+-rw-r--r--   0        0        0     3760 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_message_handler_default.py
+-rw-r--r--   0        0        0     1107 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_processor_decorator.py
+-rw-r--r--   0        0        0      863 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_processors.py
+-rw-r--r--   0        0        0     8586 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/ingestion/queue_utils.py
+-rw-r--r--   0        0        0      774 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    32979 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/loadxl.py
+-rw-r--r--   0        0        0     4847 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/local_roles.py
+-rw-r--r--   0        0        0     2425 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/memlimit.py
+-rw-r--r--   0        0        0      229 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/mime_types.py
+-rw-r--r--   0        0        0      895 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/predicates.py
+-rw-r--r--   0        0        0       98 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project/access_key.py
+-rw-r--r--   0        0        0     1520 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project/authentication.py
+-rw-r--r--   0        0        0      378 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project/authorization.py
+-rw-r--r--   0        0        0      289 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project/ingestion.py
+-rw-r--r--   0        0        0      228 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project/loadxl.py
+-rw-r--r--   0        0        0      378 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project/renderers.py
+-rw-r--r--   0        0        0      107 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project_app.py
+-rw-r--r--   0        0        0      879 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/project_defs.py
+-rw-r--r--   0        0        0       95 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22536 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/resource_views.py
+-rw-r--r--   0        0        0    26761 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/resources.py
+-rw-r--r--   0        0        0     9867 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/root.py
+-rw-r--r--   0        0        0      971 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schema_formats.py
+-rw-r--r--   0        0        0     3450 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schema_graph.py
+-rw-r--r--   0        0        0    20821 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schema_utils.py
+-rw-r--r--   0        0        0     5023 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schema_validation.py
+-rw-r--r--   0        0        0     4358 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schema_views.py
+-rw-r--r--   0        0        0     1861 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5104 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0     5413 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schemas/ingestion_submission.json
+-rw-r--r--   0        0        0    18746 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19606 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-08-03 13:44:04.666938 dcicsnovault-9.9.9.0b0/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/search/search.py
+-rw-r--r--   0        0        0    17915 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     2645 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/server_defaults.py
+-rw-r--r--   0        0        0     1616 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/server_defaults_misc.py
+-rw-r--r--   0        0        0      984 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/server_defaults_user.py
+-rw-r--r--   0        0        0      522 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/storage.py
+-rw-r--r--   0        0        0      393 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      363 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2530 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      509 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      946 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      534 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0     1029 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1143 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      955 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      344 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      760 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      616 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      793 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      760 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      535 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      355 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkedSchemaField.json
+-rw-r--r--   0        0        0      372 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      906 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3727 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1685 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      639 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2199 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3186 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-08-03 13:44:04.670938 dcicsnovault-9.9.9.0b0/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0     8173 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_ingestion_message_handler_decorator.py
+-rw-r--r--   0        0        0      384 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_ingestion_processor.py
+-rw-r--r--   0        0        0    28258 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     9709 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_renderers.py
+-rw-r--r--   0        0        0    10108 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_schema_utils.py
+-rw-r--r--   0        0        0     1194 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     1291 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_util.py
+-rw-r--r--   0        0        0     7088 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_validator.py
+-rw-r--r--   0        0        0    19246 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4620 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34543 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5132 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/access_key.py
+-rw-r--r--   0        0        0     1169 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/acl.py
+-rw-r--r--   0        0        0     8751 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/filter_set.py
+-rw-r--r--   0        0        0    11521 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/ingestion.py
+-rw-r--r--   0        0        0     5638 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/upgrader.py
+-rw-r--r--   0        0        0    63565 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-08-03 13:44:04.674938 dcicsnovault-9.9.9.0b0/snovault/validators.py
+-rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 dcicsnovault-9.9.9.0b0/PKG-INFO
```

### Comparing `dcicsnovault-9.1.1/LICENSE.txt` & `dcicsnovault-9.9.9.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/README.rst` & `dcicsnovault-9.9.9.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/pyproject.toml` & `dcicsnovault-9.9.9.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "9.1.1"
+version = "9.9.9.0b0"
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
@@ -42,15 +42,14 @@
 elasticsearch = "7.13.4"  # versions >= 7.14.0 lock out AWS ES
 elasticsearch_dsl = "^7.4.0"
 #dcicutils = "7.4.4.5b21"
 dcicutils = "^7.5.0"
 future = ">=0.15.2,<1"
 html5lib = ">=1.1"  # experimental, should be OK now that we're not using moto server
 humanfriendly = "^1.44.9"
-jsonschema_serialize_fork = "^2.1.1"
 netaddr = ">=0.8.0,<1"
 passlib = "^1.7.4"
 pillow = "^9.5.0"
 psutil = "^5.9.0"
 psycopg2-binary = "^2.9.1"
 PyBrowserID = ">=0.10.0,<1"
 pyjwt = "^2.6.0"
@@ -79,14 +78,15 @@
 WebOb = "^1.8.7"
 WebTest = "^2.0.35"
 WSGIProxy2 = "0.4.2"
 xlrd = "^1.0.0"
 "zope.deprecation" = "^4.4.0"
 "zope.interface" = ">=4.7.2,<6"
 "zope.sqlalchemy" = "1.6"
+jsonschema = "^4.18.4"
 
 [tool.poetry.dev-dependencies]
 botocore-stubs = ">=1.29.119"  # no particular version required, but this speeds up search
 boto3-stubs = ">=1.26.119"  # no particular version required, but this speeds up search
 coverage = ">=6.2"
 codacy-coverage = ">=1.3.11"
 # When we add coverage, this must be loaded manually in GA workflow for coverage because a dependency on 2to3
```

### Comparing `dcicsnovault-9.1.1/snovault/__init__.py` & `dcicsnovault-9.9.9.0b0/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/aggregated_items.py` & `dcicsnovault-9.9.9.0b0/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/app.py` & `dcicsnovault-9.9.9.0b0/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/attachment.py` & `dcicsnovault-9.9.9.0b0/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/authentication.py` & `dcicsnovault-9.9.9.0b0/snovault/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,18 +568,18 @@
     id_token = jwt.encode(
         jwt_contents,
         auth0_secret,
         algorithm=JWT_ENCODING_ALGORITHM
     )
 
     is_https = request.scheme == "https"
-    token_value = id_token.decode('utf-8') if isinstance(id_token, bytes) else id_token
+
     request.response.set_cookie(
         "jwtToken",
-        value=token_value,
+        value=id_token.decode('utf-8'),
         domain=request.domain,
         path="/",
         httponly=True,
         samesite="strict",
         overwrite=True,
         secure=is_https
     )
```

### Comparing `dcicsnovault-9.1.1/snovault/authorization.py` & `dcicsnovault-9.9.9.0b0/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/batchupgrade.py` & `dcicsnovault-9.9.9.0b0/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/cache.py` & `dcicsnovault-9.9.9.0b0/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/calculated.py` & `dcicsnovault-9.9.9.0b0/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/check_rendering.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/es_index_data.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/jsonld_rdf.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/list_db_tables.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/list_db_tables.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/load_access_keys.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/load_data.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/load_data_by_type.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/prepare_template.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/prepare_template.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/profile.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/purge_item_type.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/commands/wipe_test_indices.py` & `dcicsnovault-9.9.9.0b0/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/config.py` & `dcicsnovault-9.9.9.0b0/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/connection.py` & `dcicsnovault-9.9.9.0b0/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/crud_views.py` & `dcicsnovault-9.9.9.0b0/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/custom_embed.py` & `dcicsnovault-9.9.9.0b0/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/dev_servers.py` & `dcicsnovault-9.9.9.0b0/snovault/dev_servers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/drs.py` & `dcicsnovault-9.9.9.0b0/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/edw_hash.py` & `dcicsnovault-9.9.9.0b0/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/__init__.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/cached_views.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/esstorage.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/indexer.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-9.9.9.0b0/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/embed.py` & `dcicsnovault-9.9.9.0b0/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/etag.py` & `dcicsnovault-9.9.9.0b0/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/indexing_views.py` & `dcicsnovault-9.9.9.0b0/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/common.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/common.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/exceptions.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_listener.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_listener_base.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_listener_base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_message.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_message.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_message_handler_decorator.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_message_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_message_handler_default.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_message_handler_default.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_processor_decorator.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_processor_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/ingestion_processors.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/ingestion_processors.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/ingestion/queue_utils.py` & `dcicsnovault-9.9.9.0b0/snovault/ingestion/queue_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/interfaces.py` & `dcicsnovault-9.9.9.0b0/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/invalidation.py` & `dcicsnovault-9.9.9.0b0/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/json_renderer.py` & `dcicsnovault-9.9.9.0b0/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/jsongraph.py` & `dcicsnovault-9.9.9.0b0/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/jsonld_context.py` & `dcicsnovault-9.9.9.0b0/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/loadxl.py` & `dcicsnovault-9.9.9.0b0/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/local_roles.py` & `dcicsnovault-9.9.9.0b0/snovault/local_roles.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/memlimit.py` & `dcicsnovault-9.9.9.0b0/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/nginx-dev.conf` & `dcicsnovault-9.9.9.0b0/snovault/nginx-dev.conf`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/parallel.py` & `dcicsnovault-9.9.9.0b0/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/predicates.py` & `dcicsnovault-9.9.9.0b0/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/project/authentication.py` & `dcicsnovault-9.9.9.0b0/snovault/project/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/project_defs.py` & `dcicsnovault-9.9.9.0b0/snovault/project_defs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/redis/redis_connection.py` & `dcicsnovault-9.9.9.0b0/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/renderers.py` & `dcicsnovault-9.9.9.0b0/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/resource_views.py` & `dcicsnovault-9.9.9.0b0/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/resources.py` & `dcicsnovault-9.9.9.0b0/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/root.py` & `dcicsnovault-9.9.9.0b0/snovault/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/schema_formats.py` & `dcicsnovault-9.9.9.0b0/snovault/schema_formats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from jsonschema_serialize_fork import FormatChecker
+from jsonschema import FormatChecker
 from .server_defaults import (
     ACCESSION_PREFIX,
     ACCESSION_TEST_PREFIX,
 )
 
 
 # Codes we allow for testing go here.
```

### Comparing `dcicsnovault-9.1.1/snovault/schema_graph.py` & `dcicsnovault-9.9.9.0b0/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/schema_utils.py` & `dcicsnovault-9.9.9.0b0/snovault/schema_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import collections
 import io
 import json
 import uuid
 
 from datetime import datetime
 from dcicutils.misc_utils import ignored
-from jsonschema_serialize_fork import (
-    Draft4Validator,
-    FormatChecker,
-    RefResolver,
-)
-from jsonschema_serialize_fork.exceptions import ValidationError
+from snovault.schema_validation import SerializingSchemaValidator
+from jsonschema import FormatChecker
+from jsonschema import RefResolver
+from jsonschema.exceptions import ValidationError
 import os
 from pyramid.path import AssetResolver, caller_package
 from pyramid.threadlocal import get_current_request
 from pyramid.traversal import find_resource
 from uuid import UUID
 from .project_app import app_project
 from .util import ensurelist
@@ -37,16 +35,18 @@
 #           server_default = None
 #       It feels like the function should still get defined. -kmp 17-Feb-2023
 def server_default(func):
     SERVER_DEFAULTS[func.__name__] = func
 
 
 class NoRemoteResolver(RefResolver):
+    """ This has been modified to allow remote resolution that does not involve an http, https or ftp url
+        ie: local remote resolution """
     def resolve_remote(self, uri):
-        raise ValueError('Resolution disallowed for: %s' % uri)
+        raise ValueError(f'Resolution disallowed for: {uri}')
 
 
 def favor_app_specific_schema(schema: str) -> str:
     """
     If the given schema refers to a schema (file) which exists in the app-specific schemas
     package/directory then favor that version of the file over the local version by returning
     a reference to that schema; otherwise just returns the given schema.
@@ -78,21 +78,21 @@
     element THEN returns: file:///full-path-to/encoded/schemas/mixins.json#/modified
 
     This uses the dcicutils.project_utils mechanism to get the app-specific file/path name.
     """
     def json_file_contains_element(json_filename: str, json_element: str) -> bool:
         """
         If the given JSON file exists and contains the given JSON element name then
-        returns True, otherwise returnes False. The given JSON element may or may 
+        returns True, otherwise returnes False. The given JSON element may or may
         not begin with a slash. Currently only looks at one single top-level element.
         """
         if json_filename and json_element:
             try:
                 with io.open(json_filename, "r") as json_f:
-                    json_content = json.load(json_f) 
+                    json_content = json.load(json_f)
                     json_element = json_element.strip("/")
                     if json_element:
                         if json_content.get(json_element):
                             return True
             except Exception:
                 pass
         return False
@@ -107,14 +107,72 @@
                 if json_file_contains_element(app_specific_schema_filename, schema_element):
                     schema_ref = f"file://{app_specific_schema_filename}#{schema_element}"
             else:
                 schema_ref = f"file://{app_specific_schema_filename}"
     return schema_ref
 
 
+def resolve_merge_ref(ref, resolver):
+    with resolver.resolving(ref) as resolved:
+        if not isinstance(resolved, dict):
+            raise ValueError(
+                f'Schema ref {ref} must resolve dict, not {type(resolved)}'
+            )
+        return resolved
+
+
+def _update_resolved_data(resolved_data, value, resolver):
+    # Assumes resolved value is dictionary.
+    resolved_data.update(
+        # Recurse here in case the resolved value has refs.
+        resolve_merge_refs(
+            # Actually get the ref value.
+            resolve_merge_ref(value, resolver),
+            resolver
+        )
+    )
+
+
+def _handle_list_or_string_value(resolved_data, value, resolver):
+    if isinstance(value, list):
+        for v in value:
+            _update_resolved_data(resolved_data, v, resolver)
+    else:
+        _update_resolved_data(resolved_data, value, resolver)
+
+
+def resolve_merge_refs(data, resolver):
+    if isinstance(data, dict):
+        # Return copy.
+        resolved_data = {}
+        for k, v in data.items():
+            if k == '$merge':
+                _handle_list_or_string_value(resolved_data, v, resolver)
+            else:
+                resolved_data[k] = resolve_merge_refs(v, resolver)
+    elif isinstance(data, list):
+        # Return copy.
+        resolved_data = [
+            resolve_merge_refs(v, resolver)
+            for v in data
+        ]
+    else:
+        # Assumes we're only dealing with other JSON types
+        # like string, number, boolean, null, not other
+        # types like tuples, sets, functions, classes, etc.,
+        # which would require a deep copy.
+        resolved_data = data
+    return resolved_data
+
+
+def fill_in_schema_merge_refs(schema, resolver):
+    """ Resolves $merge properties, custom $ref implementation from IGVF SNO2-6 """
+    return resolve_merge_refs(schema, resolver)
+
+
 def mixinSchemas(schema, resolver, key_name='properties'):
     mixinKeyName = 'mixin' + key_name.capitalize()
     mixins = schema.get(mixinKeyName)
     if mixins is None:
         return schema
     properties = collections.OrderedDict()
     bases = []
@@ -206,18 +264,14 @@
             if (submits_for is not None and
                     not any(UUID(uuid) == item.uuid for uuid in submits_for) and
                     not request.has_permission('submit_for_any')):
                 error = "%r is not in user submits_for" % instance
                 yield ValidationError(error)
                 return
 
-    # And normalize the value to a uuid
-    if validator._serialize:
-        validator._validated[-1] = str(item.uuid)
-
 
 class IgnoreUnchanged(ValidationError):
     pass
 
 
 def requestMethod(validator, requestMethod, instance, schema):
     ignored(instance, schema)
@@ -283,16 +337,16 @@
         return schema.get('type') == 'array' and schema_is_object(schema.get('items', {}))
 
     if (not schema_is_sub_embedded(schema)
             or (not schema_is_array_of_objects(schema) and not schema_is_object(schema))):
         yield ValidationError('submission of calculatedProperty disallowed')
 
 
-class SchemaValidator(Draft4Validator):
-    VALIDATORS = Draft4Validator.VALIDATORS.copy()
+class SchemaValidator(SerializingSchemaValidator):
+    VALIDATORS = SerializingSchemaValidator.VALIDATORS.copy()
     VALIDATORS['calculatedProperty'] = calculatedProperty
     VALIDATORS['linkTo'] = linkTo
     VALIDATORS['permission'] = permission
     VALIDATORS['requestMethod'] = requestMethod
     VALIDATORS['validators'] = validators
     SERVER_DEFAULTS = SERVER_DEFAULTS
 
@@ -316,17 +370,18 @@
         mixinSchemas(
             mixinSchemas(mixinSchemas(schema, resolver, 'properties'), resolver, 'facets'),
             resolver,
             'aggregations'
         ),
         resolver, 'columns'
     )
+    schema = fill_in_schema_merge_refs(schema, resolver)
 
     # SchemaValidator is not thread safe for now
-    SchemaValidator(schema, resolver=resolver, serialize=True)
+    SchemaValidator(schema, resolver=resolver)
     return schema
 
 
 def validate(schema, data, current=None, validate_current=False):
     """
     Validate the given data using a schema. Optionally provide current data
     to allow IgnoreUnchanged validation errors. If validate_current is set,
@@ -340,15 +395,15 @@
         current (dict): existing item contents
         validate_current (bool): whether to validate against current
 
     Returns:
         dict validated contents, list of errors
     """
     resolver = NoRemoteResolver.from_schema(schema)
-    sv = SchemaValidator(schema, resolver=resolver, serialize=True, format_checker=format_checker)
+    sv = SchemaValidator(schema, resolver=resolver, format_checker=format_checker)
     validated, errors = sv.serialize(data)
     # validate against current contents if validate_current is set
     if current and validate_current:
         validated_curr, errors_curr = sv.serialize(current)
         data_errors_detail = {str(err.path): err.message for err in errors}
         # add errors from validation of current if they are not in existing
         # error paths or already exist but have a different message
@@ -377,14 +432,26 @@
                         validated_value = validated_value[key]
                 except Exception:
                     validated_value = None  # not found
                 # TODO: Should this test be indented left by 4 spaces so that the other arms of the 'if' affect it?
                 #       Right now those other arms set seemingly-unused variables. -kmp 7-Aug-2022
                 if validated_value == current_value:
                     continue  # value is unchanged between data/current; ignore
+        # Also ignore requestMethod and permission errors from defaults.
+        if isinstance(error, IgnoreUnchanged):
+            current_value = data
+            try:
+                for key in error.path:
+                    # If it's in original data then either user passed it in
+                    # or it's from PATCH object with unchanged data. If it's
+                    # unchanged then it's already been skipped above.
+                    current_value = current_value[key]
+            except KeyError:
+                # If it's not in original data then it's filled in by defaults.
+                continue
         filtered_errors.append(error)
 
     return validated, filtered_errors
 
 
 def validate_request(schema, request, data=None, current=None):
     if data is None:
@@ -448,15 +515,14 @@
     for name in set(b.keys()).difference(a.keys()):
         combined[name] = b[name]
     return combined
 
 
 # for integrated tests
 def utc_now_str():
-    # from jsonschema_serialize_fork date-time format requires a timezone
     return datetime.utcnow().isoformat() + '+00:00'
 
 
 @server_default
 def userid(instance, subschema):  # args required by jsonschema-serialize-fork
     ignored(instance, subschema)
     return str(uuid.uuid4())
```

### Comparing `dcicsnovault-9.1.1/snovault/schema_views.py` & `dcicsnovault-9.9.9.0b0/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/schemas/access_key.json` & `dcicsnovault-9.9.9.0b0/snovault/schemas/access_key.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'$id'": "'/profiles/access_key.json'",*

 * * "'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * 'delete': "['id']"}*

```diff
@@ -1,16 +1,16 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
+    "$id": "/profiles/access_key.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "facets": {
         "user.display_title": {
             "title": "User Name"
         }
     },
-    "id": "/profiles/access_key.json",
     "mixinProperties": [
         {
             "$ref": "mixins.json#/schema_version"
         },
         {
             "$ref": "mixins.json#/uuid"
         },
```

### Comparing `dcicsnovault-9.1.1/snovault/schemas/filter_set.json` & `dcicsnovault-9.9.9.0b0/snovault/schemas/filter_set.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7727272727272727%*

 * *Differences: {"'$id'": "'/profiles/filter_set.json'",*

 * * "'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * 'delete': "['id']"}*

```diff
@@ -1,12 +1,12 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
+    "$id": "/profiles/filter_set.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "Filter Set for encapsulating multiple queries",
-    "id": "/profiles/filter_set.json",
     "identifyingProperties": [
         "uuid",
         "aliases"
     ],
     "mixinProperties": [
         {
             "$ref": "mixins.json#/schema_version"
```

### Comparing `dcicsnovault-9.1.1/snovault/schemas/ingestion_submission.json` & `dcicsnovault-9.9.9.0b0/snovault/schemas/ingestion_submission.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {"'$id'": "'/profiles/ingestion_submission.json'",*

 * * "'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * 'delete': "['id']"}*

```diff
@@ -1,12 +1,12 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
+    "$id": "/profiles/ingestion_submission.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "Schema for metadata related to ingestion requests submitted to CGAP.",
-    "id": "/profiles/ingestion_submission.json",
     "identifyingProperties": [
         "uuid",
         "aliases"
     ],
     "mixinFacets": [
         {
             "$ref": "mixins.json#/facets_common"
```

### Comparing `dcicsnovault-9.1.1/snovault/schemas/mixins.json` & `dcicsnovault-9.9.9.0b0/snovault/schemas/mixins.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992236024844721%*

 * *Differences: {"'uuid'": "{'uuid': {'requestMethod': ['POST']}}"}*

```diff
@@ -506,14 +506,16 @@
     "uuid": {
         "uuid": {
             "exclude_from": [
                 "FFedit-create"
             ],
             "format": "uuid",
             "permission": "restricted_fields",
-            "requestMethod": "POST",
+            "requestMethod": [
+                "POST"
+            ],
             "serverDefault": "uuid4",
             "title": "UUID",
             "type": "string"
         }
     }
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/schemas/user.json` & `dcicsnovault-9.9.9.0b0/snovault/schemas/user.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7727272727272727%*

 * *Differences: {"'$id'": "'/profiles/user.json'",*

 * * "'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * 'delete': "['id']"}*

```diff
@@ -1,17 +1,17 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
+    "$id": "/profiles/user.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "columns": {
         "job_title": {
             "default_hidden": true,
             "title": "Job Title"
         }
     },
-    "id": "/profiles/user.json",
     "identifyingProperties": [
         "uuid",
         "email",
         "aliases"
     ],
     "mixinProperties": [
         {
```

### Comparing `dcicsnovault-9.1.1/snovault/search/compound_search.py` & `dcicsnovault-9.9.9.0b0/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/search/lucene_builder.py` & `dcicsnovault-9.9.9.0b0/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/search/search.py` & `dcicsnovault-9.9.9.0b0/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/search/search_utils.py` & `dcicsnovault-9.9.9.0b0/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/server_defaults.py` & `dcicsnovault-9.9.9.0b0/snovault/server_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 import uuid
 
 from dcicutils.misc_utils import exported, utc_now_str
-from jsonschema_serialize_fork import NO_DEFAULT
+from snovault.schema_validation import NO_DEFAULT
 from pyramid.path import DottedNameResolver
 from pyramid.threadlocal import get_current_request
 from snovault.schema_utils import server_default
 from .interfaces import COLLECTIONS  # , ROOT
 from string import digits  # , ascii_uppercase
 from .project_app import app_project
 from .server_defaults_misc import add_last_modified, get_now
```

### Comparing `dcicsnovault-9.1.1/snovault/server_defaults_misc.py` & `dcicsnovault-9.9.9.0b0/snovault/server_defaults_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dcicutils.misc_utils import utc_now_str
-from jsonschema_serialize_fork import NO_DEFAULT
+from snovault.schema_validation import NO_DEFAULT
 from .server_defaults_user import get_userid
 
 
 def get_now():
     """ Wrapper for the server_default 'now' above so it is not called through SERVER_DEFAULTS in our code """
     return utc_now_str()
```

### Comparing `dcicsnovault-9.1.1/snovault/server_defaults_user.py` & `dcicsnovault-9.9.9.0b0/snovault/server_defaults_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Factored out of server_defaults to avoid circular dependencies now that get_userid is
 # used in resources.Item.is_update_by_admin_user (commonized from fourfront/cgap-portal),
 # since server_defaults imports schema_utils which imports resources which wants get_userid.
 
-from jsonschema_serialize_fork import NO_DEFAULT
+from snovault.schema_validation import NO_DEFAULT
 from pyramid.threadlocal import get_current_request
 from .interfaces import COLLECTIONS
 
 
 def _userid():
     request = get_current_request()
     for principal in request.effective_principals:
```

### Comparing `dcicsnovault-9.1.1/snovault/settings.py` & `dcicsnovault-9.9.9.0b0/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/sqlalchemy_tools.py` & `dcicsnovault-9.9.9.0b0/snovault/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/standalone_dev.py` & `dcicsnovault-9.9.9.0b0/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/stats.py` & `dcicsnovault-9.9.9.0b0/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/storage.py` & `dcicsnovault-9.9.9.0b0/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/EmbeddingTest.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8558673469387755%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'properties'": "{'schema_version': {'type': 'string'}}"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "columns": {
         "accession": {
             "title": "Accession"
         },
         "award": {
             "title": "Award"
         },
@@ -78,15 +79,15 @@
                     "type": "object"
                 }
             },
             "type": "object"
         },
         "schema_version": {
             "default": "1",
-            "type": "object"
+            "type": "string"
         },
         "uuid": {
             "type": "string"
         }
     },
     "required": [
         "title",
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3203125%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'additionalProperties'": 'False',*

 * * "'properties'": "{'name': OrderedDict([('type', 'string'), ('uniqueKey', True)]), 'target': "*

 * *                 "OrderedDict([('type', 'string'), ('linkTo', 'TestingLinkTargetSno')]), "*

 * *                 "'target_es': OrderedDict([('type', 'string'), ('linkTo', "*

 * *                 "'TestingLinkTargetElasticSearch')]), 'ppp': OrderedDict([('type', 'string'), "*

 * *                 "('linkTo', 'TestingPostPutPatchSno […]*

```diff
@@ -1,40 +1,34 @@
 {
-    "description": "Dummy Schema for testing an embeddable item",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "additionalProperties": false,
     "mixinProperties": [
         {
             "$ref": "mixins.json#/status"
         }
     ],
     "properties": {
-        "associates": {
-            "items": {
-                "properties": {
-                    "x": {
-                        "type": "string"
-                    },
-                    "y": {
-                        "type": "string"
-                    },
-                    "z": {
-                        "type": "string"
-                    }
-                },
-                "type": "object"
-            },
-            "type": "array"
+        "name": {
+            "type": "string",
+            "uniqueKey": true
         },
-        "schema_version": {
-            "default": "1",
-            "type": "object"
+        "ppp": {
+            "linkTo": "TestingPostPutPatchSno",
+            "type": "string"
+        },
+        "status": {
+            "type": "string"
+        },
+        "target": {
+            "linkTo": "TestingLinkTargetSno",
+            "type": "string"
+        },
+        "target_es": {
+            "linkTo": "TestingLinkTargetElasticSearch",
+            "type": "string"
         },
         "uuid": {
             "type": "string"
         }
     },
-    "required": [
-        "title",
-        "description"
-    ],
-    "title": "NestedObjectLinkTarget",
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "Biosample integrated testing type.",
     "mixinProperties": [
         {
             "$ref": "mixins.json#/status"
         }
     ],
     "properties": {
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5892857142857143%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'description'": "'Dummy Schema for testing an embeddable item'",*

 * * "'properties'": "{'associates': OrderedDict([('type', 'array'), ('items', OrderedDict([('type', "*

 * *                 "'object'), ('properties', OrderedDict([('x', OrderedDict([('type', 'string')])), "*

 * *                 "('y', OrderedDict([('type', 'string')])), ('z', OrderedDict([('type', "*

 * *                 "'string')]))]))]))]), delete: ['identifier', 'samples', 'sample_objects', […]*

```diff
@@ -1,55 +1,41 @@
 {
-    "description": "Biosource integrated testing type. This item contains an array of linkTo Biosamples.",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "description": "Dummy Schema for testing an embeddable item",
     "mixinProperties": [
         {
             "$ref": "mixins.json#/status"
         }
     ],
     "properties": {
-        "contributor": {
-            "linkTo": "TestingIndividualSno",
-            "type": "string"
-        },
-        "counter": {
-            "type": "string"
-        },
-        "identifier": {
-            "type": "string",
-            "uniqueKey": true
-        },
-        "sample_objects": {
+        "associates": {
             "items": {
                 "properties": {
-                    "associated_sample": {
-                        "linkTo": "TestingBiosampleSno",
+                    "x": {
                         "type": "string"
                     },
-                    "notes": {
+                    "y": {
+                        "type": "string"
+                    },
+                    "z": {
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
             "type": "array"
         },
-        "samples": {
-            "items": {
-                "linkTo": "TestingBiosampleSno",
-                "type": "string"
-            },
-            "type": "array"
-        },
         "schema_version": {
             "default": "1",
             "type": "string"
         },
         "uuid": {
             "type": "string"
         }
     },
     "required": [
-        "identifier"
+        "title",
+        "description"
     ],
-    "title": "Testing Biosource Sno",
+    "title": "NestedObjectLinkTarget",
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8315972222222222%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'properties'": "{'schema_version': {'type': 'string'}}"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "Test object that has calculated properties to test",
     "properties": {
         "bar": {
             "type": "string"
         },
         "foo": {
             "type": "string"
@@ -34,15 +35,15 @@
                 },
                 "type": "object"
             },
             "type": "array"
         },
         "schema_version": {
             "default": "1",
-            "type": "object"
+            "type": "string"
         }
     },
     "required": [
         "name",
         "foo",
         "bar",
         "nested",
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingServerDefault.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'properties'": "{replace: OrderedDict([('uuid', OrderedDict([('serverDefault', 'uuid4'), "*

 * *                 "('type', 'string')])), ('user', OrderedDict([('serverDefault', 'userid'), "*

 * *                 "('linkTo', 'User'), ('type', 'string')])), ('now', "*

 * *                 "OrderedDict([('serverDefault', 'now'), ('format', 'date-time'), ('type', "*

 * *                 "'string')])), ('accession', OrderedDict([('serverDefault', 'accession'), "*

 * *     […]*

```diff
@@ -1,37 +1,26 @@
 {
-    "mixinProperties": [
-        {
-            "$ref": "mixins.json#/status"
-        },
-        {
-            "$ref": "mixins.json#/submitted"
-        }
-    ],
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "properties": {
-        "attachment": {
-            "attachment": true,
-            "properties": {
-                "type": {
-                    "enum": [
-                        "image/png"
-                    ],
-                    "type": "string"
-                }
-            },
-            "type": "object"
+        "accession": {
+            "accessionType": "AB",
+            "format": "accession",
+            "serverDefault": "accession",
+            "type": "string"
+        },
+        "now": {
+            "format": "date-time",
+            "serverDefault": "now",
+            "type": "string"
+        },
+        "user": {
+            "linkTo": "User",
+            "serverDefault": "userid",
+            "type": "string"
         },
-        "attachment2": {
-            "attachment": true,
-            "properties": {
-                "type": {
-                    "enum": [
-                        "image/png"
-                    ],
-                    "type": "string"
-                }
-            },
-            "type": "object"
+        "uuid": {
+            "serverDefault": "uuid4",
+            "type": "string"
         }
     },
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5857142857142856%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'description'": "'Biosource integrated testing type. This item contains an array of linkTo "*

 * *                  "Biosamples.'",*

 * * "'properties'": "{'identifier': OrderedDict([('type', 'string'), ('uniqueKey', True)]), "*

 * *                 "'samples': OrderedDict([('type', 'array'), ('items', OrderedDict([('type', "*

 * *                 "'string'), ('linkTo', 'TestingBiosampleSno')]))]), 'sample_objects': "*

 * *                 "OrderedDict([('type', 'arr […]*

```diff
@@ -1,32 +1,56 @@
 {
-    "description": "Individual integrated testing type. Linked to by biosample and biosource",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "description": "Biosource integrated testing type. This item contains an array of linkTo Biosamples.",
     "mixinProperties": [
         {
             "$ref": "mixins.json#/status"
         }
     ],
     "properties": {
-        "full_name": {
+        "contributor": {
+            "linkTo": "TestingIndividualSno",
+            "type": "string"
+        },
+        "counter": {
+            "type": "string"
+        },
+        "identifier": {
             "type": "string",
             "uniqueKey": true
         },
-        "schema_version": {
-            "default": "1",
-            "type": "string"
+        "sample_objects": {
+            "items": {
+                "properties": {
+                    "associated_sample": {
+                        "linkTo": "TestingBiosampleSno",
+                        "type": "string"
+                    },
+                    "notes": {
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "type": "array"
         },
-        "specimen": {
-            "type": "string"
+        "samples": {
+            "items": {
+                "linkTo": "TestingBiosampleSno",
+                "type": "string"
+            },
+            "type": "array"
         },
-        "uid": {
+        "schema_version": {
+            "default": "1",
             "type": "string"
         },
         "uuid": {
             "type": "string"
         }
     },
     "required": [
-        "full_name"
+        "identifier"
     ],
-    "title": "Testing Individual Sno",
+    "title": "Testing Biosource Sno",
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.29464285714285715%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'description'": "'Test object that has an array of object field that passes the enable_nested "*

 * *                  "parameter.'",*

 * * "'properties'": "{'name': {'uniqueKey': True}, 'nested_options': OrderedDict([('type', 'array'), "*

 * *                 "('items', OrderedDict([('type', 'object'), ('enable_nested', True), "*

 * *                 "('properties', OrderedDict([('key', OrderedDict([('type', 'string')])), "*

 * *                 "('value', OrderedDi […]*

```diff
@@ -1,33 +1,44 @@
 {
-    "additionalProperties": false,
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "description": "Test object that has an array of object field that passes the enable_nested parameter.",
     "properties": {
         "name": {
-            "type": "string"
+            "type": "string",
+            "uniqueKey": true
         },
-        "status": {
-            "type": "string"
-        },
-        "targets": {
+        "nested_options": {
             "items": {
+                "enable_nested": true,
                 "properties": {
-                    "target": {
-                        "linkTo": "TestingLinkTargetSno",
+                    "key": {
                         "type": "string"
                     },
-                    "test_description": {
-                        "type": "string"
+                    "value": {
+                        "type": "number"
                     }
                 },
                 "type": "object"
             },
             "type": "array"
         },
-        "uuid": {
-            "type": "string"
+        "object_options": {
+            "items": {
+                "properties": {
+                    "obj_key": {
+                        "type": "string"
+                    },
+                    "obj_value": {
+                        "type": "number"
+                    }
+                },
+                "type": "object"
+            },
+            "type": "array"
         }
     },
     "required": [
-        "targets"
+        "name"
     ],
+    "title": "Testing Nested Enabled",
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.44940476190476186%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'properties'": "{'name': {delete: ['uniqueKey']}, 'targets': OrderedDict([('type', 'array'), "*

 * *                 "('items', OrderedDict([('type', 'object'), ('properties', "*

 * *                 "OrderedDict([('test_description', OrderedDict([('type', 'string')])), ('target', "*

 * *                 "OrderedDict([('type', 'string'), ('linkTo', 'TestingLinkTargetSno')]))]))]))]), "*

 * *                 "delete: ['target', 'target_es', 'ppp']}",*

 * * "'required' […]*

```diff
@@ -1,33 +1,34 @@
 {
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
-    "mixinProperties": [
-        {
-            "$ref": "mixins.json#/status"
-        }
-    ],
     "properties": {
         "name": {
-            "type": "string",
-            "uniqueKey": true
-        },
-        "ppp": {
-            "linkTo": "TestingPostPutPatchSno",
             "type": "string"
         },
         "status": {
             "type": "string"
         },
-        "target": {
-            "linkTo": "TestingLinkTargetSno",
-            "type": "string"
-        },
-        "target_es": {
-            "linkTo": "TestingLinkTargetElasticSearch",
-            "type": "string"
+        "targets": {
+            "items": {
+                "properties": {
+                    "target": {
+                        "linkTo": "TestingLinkTargetSno",
+                        "type": "string"
+                    },
+                    "test_description": {
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "type": "array"
         },
         "uuid": {
             "type": "string"
         }
     },
+    "required": [
+        "targets"
+    ],
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingNoteSno.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'$id'": "'/profiles/testing_note.json'",*

 * * "'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * 'delete': "['id']"}*

```diff
@@ -1,12 +1,12 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
+    "$id": "/profiles/testing_note.json",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "TestingNote, based on schema for technical review of variants from CGAP.",
-    "id": "/profiles/testing_note.json",
     "identifyingProperties": [
         "identifier"
     ],
     "mixinProperties": [
         {
             "$ref": "mixins.json#/status"
         }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "mixinProperties": [
         {
             "$ref": "mixins.json#/status"
         }
     ],
     "properties": {
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/TestingDownload.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'mixinProperties'": "[OrderedDict([('$ref', 'mixins.json#/status')]), OrderedDict([('$ref', "*

 * *                      "'mixins.json#/submitted')])]",*

 * * "'properties'": "{replace: OrderedDict([('attachment', OrderedDict([('type', 'object'), "*

 * *                 "('attachment', True), ('properties', OrderedDict([('type', OrderedDict([('type', "*

 * *                 "'string'), ('enum', ['image/png'])]))]))])), ('attachment2', "*

 * *                 "Ordered […]*

```diff
@@ -1,25 +1,38 @@
 {
-    "properties": {
-        "accession": {
-            "accessionType": "AB",
-            "format": "accession",
-            "serverDefault": "accession",
-            "type": "string"
-        },
-        "now": {
-            "format": "date-time",
-            "serverDefault": "now",
-            "type": "string"
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
+    "mixinProperties": [
+        {
+            "$ref": "mixins.json#/status"
         },
-        "user": {
-            "linkTo": "User",
-            "serverDefault": "userid",
-            "type": "string"
+        {
+            "$ref": "mixins.json#/submitted"
+        }
+    ],
+    "properties": {
+        "attachment": {
+            "attachment": true,
+            "properties": {
+                "type": {
+                    "enum": [
+                        "image/png"
+                    ],
+                    "type": "string"
+                }
+            },
+            "type": "object"
         },
-        "uuid": {
-            "serverDefault": "uuid4",
-            "type": "string"
+        "attachment2": {
+            "attachment": true,
+            "properties": {
+                "type": {
+                    "enum": [
+                        "image/png"
+                    ],
+                    "type": "string"
+                }
+            },
+            "type": "object"
         }
     },
     "type": "object"
 }
```

### Comparing `dcicsnovault-9.1.1/snovault/test_schemas/mixins.json` & `dcicsnovault-9.9.9.0b0/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/conftest.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/postgresql_fixture.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/pyramidfixtures.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/root.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/serverfixtures.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_attachment.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_authentication.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_calculated.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_create_mapping.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_drs.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_edw_hash.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_embed_utils.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_embedding.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_es_permissions.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_indexing.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_ingestion_message_handler_decorator.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_ingestion_message_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_key.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_link.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_logging.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_misc.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_post_put_patch.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_renderers.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_schemas.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_serverfixtures.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_standalone_dev.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_stats.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_storage.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_upgrader.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_util.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/test_views.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import pytest
 
 from base64 import b64encode
-from jsonschema_serialize_fork import Draft4Validator
+from jsonschema import Draft202012Validator
 from pyramid.compat import ascii_native_
 from uuid import uuid4
 
 from ..interfaces import TYPES
 from ..util import mappings_use_nested
 
 from .testing_views import (
@@ -344,27 +344,27 @@
 def test_home(testapp):
     testapp.get('/', status=200)
 
 
 @pytest.mark.parametrize('item_type', TYPE_NAMES)
 def test_profiles(testapp, item_type):
     res = testapp.get('/profiles/%s.json' % item_type).maybe_follow(status=200)
-    errors = Draft4Validator.check_schema(res.json)
+    errors = Draft202012Validator.check_schema(res.json)
     assert not errors
     # added from ..schema_views._annotated_schema
     assert 'rdfs:seeAlso' in res.json
     assert 'rdfs:subClassOf' in res.json
     assert 'children' in res.json
     assert res.json['isAbstract'] is False
 
 
 @pytest.mark.parametrize('item_type', ['AbstractItemTest'])
 def test_profiles_abstract(testapp, item_type):
     res = testapp.get('/profiles/%s.json' % item_type).maybe_follow(status=200)
-    errors = Draft4Validator.check_schema(res.json)
+    errors = Draft202012Validator.check_schema(res.json)
     assert not errors
     # added from ..schema_views._annotated_schema
     assert 'rdfs:seeAlso' in res.json
     # Item/item does not have subClass
     if item_type.lower() == 'item':
         assert 'rdfs:subClassOf' not in res.json
     else:
```

### Comparing `dcicsnovault-9.1.1/snovault/tests/testappfixtures.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/testing_upgrader.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tests/testing_views.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/testing_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,14 +529,15 @@
 class TestingServerDefault(Item):
     item_type = 'testing_server_default'
     schema = load_schema('snovault:test_schemas/TestingServerDefault.json')
 
 
 @collection('testing-dependencies')
 class TestingDependencies(Item):
+    """ BREAKING CHANGE - dependencies --> dependentRequired in schema """
     item_type = 'testing_dependencies'
     schema = load_schema('snovault:test_schemas/TestingDependencies.json')
 
 
 @view_config(name='testing-render-error', request_method='GET')
 def testing_render_error(request):
     return {
@@ -861,14 +862,26 @@
                 'type': 'string',
                 'uniqueKey': 'testing_accession',
             },
         }
     }
 
 
+@collection(
+    'testing-linked-schema-fields',
+    properties={
+        'title': 'Test Linked Schema Fields',
+        'description': 'Testing that we can link fields across schemas.',
+    },
+)
+class TestingLinkedSchemaField(Item):
+    item_type = 'testing_linked_schema_field'
+    schema = load_schema('snovault:test_schemas/TestingLinkedSchemaField.json')
+
+
 @collection('testing-hidden-facets')
 class TestingHiddenFacets(Item):
     """ Collection designed to test searching with hidden facets. Yes this is large, but this is a complex feature
         with many possible cases. """
     item_type = 'testing_hidden_facets'
     schema = {
         'type': 'object',
```

### Comparing `dcicsnovault-9.1.1/snovault/tests/toolfixtures.py` & `dcicsnovault-9.9.9.0b0/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/tools.py` & `dcicsnovault-9.9.9.0b0/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/typedsheets.py` & `dcicsnovault-9.9.9.0b0/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/typeinfo.py` & `dcicsnovault-9.9.9.0b0/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/types/access_key.py` & `dcicsnovault-9.9.9.0b0/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/types/acl.py` & `dcicsnovault-9.9.9.0b0/snovault/types/acl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/types/base.py` & `dcicsnovault-9.9.9.0b0/snovault/types/base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/types/filter_set.py` & `dcicsnovault-9.9.9.0b0/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/types/ingestion.py` & `dcicsnovault-9.9.9.0b0/snovault/types/ingestion.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/types/user.py` & `dcicsnovault-9.9.9.0b0/snovault/types/user.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/upgrader.py` & `dcicsnovault-9.9.9.0b0/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/util.py` & `dcicsnovault-9.9.9.0b0/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/validation.py` & `dcicsnovault-9.9.9.0b0/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/snovault/validators.py` & `dcicsnovault-9.9.9.0b0/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-9.1.1/PKG-INFO` & `dcicsnovault-9.9.9.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 9.1.1
+Version: 9.9.9.0b0
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -29,15 +29,15 @@
 Requires-Dist: botocore (>=1.26.133)
 Requires-Dist: dcicutils (>=7.5.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch_dsl (>=7.4.0,<8.0.0)
 Requires-Dist: future (>=0.15.2,<1)
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: humanfriendly (>=1.44.9,<2.0.0)
-Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
+Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: netaddr (>=0.8.0,<1)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pyramid (==1.10.4)
```

