# Comparing `tmp/promptflow_vectordb-0.2.6-py3-none-any.whl.zip` & `tmp/promptflow_vectordb-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,140 +1,141 @@
-Zip file size: 108499 bytes, number of entries: 138
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/__init__.py
--rw-rw-rw-  2.0 fat       18 b- defN 24-Mar-18 20:28 promptflow_vectordb/_version.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/connections/__init__.py
--rw-rw-rw-  2.0 fat      255 b- defN 24-Mar-18 20:28 promptflow_vectordb/connections/pinecone.py
--rw-rw-rw-  2.0 fat      251 b- defN 24-Mar-18 20:28 promptflow_vectordb/connections/qdrant.py
--rw-rw-rw-  2.0 fat      255 b- defN 24-Mar-18 20:28 promptflow_vectordb/connections/weaviate.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/__init__.py
--rw-rw-rw-  2.0 fat     7570 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddingstore_core.py
--rw-rw-rw-  2.0 fat      847 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/__init__.py
--rw-rw-rw-  2.0 fat     6006 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/config.py
--rw-rw-rw-  2.0 fat      514 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/constants.py
--rw-rw-rw-  2.0 fat      398 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/entities.py
--rw-rw-rw-  2.0 fat     3492 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/exceptions.py
--rw-rw-rw-  2.0 fat     1458 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/identifier_converter.py
--rw-rw-rw-  2.0 fat      536 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/secret.py
--rw-rw-rw-  2.0 fat     1693 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/telemetry.py
--rw-rw-rw-  2.0 fat     1370 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/contracts/types.py
--rw-rw-rw-  2.0 fat      109 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/__init__.py
--rw-rw-rw-  2.0 fat     1215 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/aoai_embedding.py
--rw-rw-rw-  2.0 fat      690 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/customized_embedding.py
--rw-rw-rw-  2.0 fat      165 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/embedding.py
--rw-rw-rw-  2.0 fat     1554 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/embedding_factory.py
--rw-rw-rw-  2.0 fat      467 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/empty_embedding.py
--rw-rw-rw-  2.0 fat      784 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/embeddings/openai_embedding.py
--rw-rw-rw-  2.0 fat       97 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/engine/__init__.py
--rw-rw-rw-  2.0 fat     1504 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/engine/engine.py
--rw-rw-rw-  2.0 fat     1950 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/engine/engine_factory.py
--rw-rw-rw-  2.0 fat     4207 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/engine/langchain_engine.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/logging/__init__.py
--rw-rw-rw-  2.0 fat     5505 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/logging/handlers.py
--rw-rw-rw-  2.0 fat     5224 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/logging/loggers.py
--rw-rw-rw-  2.0 fat     4304 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/logging/utils.py
--rw-rw-rw-  2.0 fat      124 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/__init__.py
--rw-rw-rw-  2.0 fat     1560 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/aml_data_store_client.py
--rw-rw-rw-  2.0 fat     4682 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/azure_blob_client.py
--rw-rw-rw-  2.0 fat     2936 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/github_client.py
--rw-rw-rw-  2.0 fat     3344 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/http_client.py
--rw-rw-rw-  2.0 fat      661 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/remote_client.py
--rw-rw-rw-  2.0 fat     2799 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/remote_client/remote_client_factory.py
--rw-rw-rw-  2.0 fat       94 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/store/__init__.py
--rw-rw-rw-  2.0 fat     1610 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/store/in_memory_store.py
--rw-rw-rw-  2.0 fat     5351 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/store/local_based_store.py
--rw-rw-rw-  2.0 fat     4852 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/store/remote_based_store.py
--rw-rw-rw-  2.0 fat     1239 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/store/store.py
--rw-rw-rw-  2.0 fat     1323 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/store/store_factory.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/__init__.py
--rw-rw-rw-  2.0 fat     7724 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/aml_helpers.py
--rw-rw-rw-  2.0 fat     1794 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/azure_helpers.py
--rw-rw-rw-  2.0 fat     1560 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/common_utils.py
--rw-rw-rw-  2.0 fat      853 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/global_instance_manager.py
--rw-rw-rw-  2.0 fat      663 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/index_factory.py
--rw-rw-rw-  2.0 fat     3284 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/path_utils.py
--rw-rw-rw-  2.0 fat     1397 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/retry_utils.py
--rw-rw-rw-  2.0 fat     2319 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/secret_manager.py
--rw-rw-rw-  2.0 fat      472 b- defN 24-Mar-18 20:28 promptflow_vectordb/core/utils/singleton_meta.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/client/__init__.py
--rw-rw-rw-  2.0 fat     4003 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/client/embeddingstore_client.py
--rw-rw-rw-  2.0 fat       93 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/__init__.py
--rw-rw-rw-  2.0 fat      473 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/agent.py
--rw-rw-rw-  2.0 fat     2014 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/agent_factory.py
--rw-rw-rw-  2.0 fat     3093 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/cog_search_client.py
--rw-rw-rw-  2.0 fat      762 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/file_based_agent.py
--rw-rw-rw-  2.0 fat     4747 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/milvus_client.py
--rw-rw-rw-  2.0 fat     4552 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/pinecone_client.py
--rw-rw-rw-  2.0 fat     2518 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/qdrant_client.py
--rw-rw-rw-  2.0 fat     3135 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/rest_based_agent.py
--rw-rw-rw-  2.0 fat     2655 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/client/agent/weaviate_client.py
--rw-rw-rw-  2.0 fat      367 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/__init__.py
--rw-rw-rw-  2.0 fat     4333 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/config.py
--rw-rw-rw-  2.0 fat      665 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/constants.py
--rw-rw-rw-  2.0 fat      370 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/errors.py
--rw-rw-rw-  2.0 fat     2990 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/request_obj.py
--rw-rw-rw-  2.0 fat      779 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/telemetry.py
--rw-rw-rw-  2.0 fat      330 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/contracts/types.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/service/server/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/server/rest/__init__.py
--rw-rw-rw-  2.0 fat     7170 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/server/rest/app.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/server/utils/__init__.py
--rw-rw-rw-  2.0 fat     7892 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/server/utils/store_request_manager.py
--rw-rw-rw-  2.0 fat     1123 b- defN 24-Mar-18 20:29 promptflow_vectordb/service/server/utils/sys_utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/__init__.py
--rw-rw-rw-  2.0 fat     4283 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup.py
--rw-rw-rw-  2.0 fat     3752 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/faiss_index_lookup.py
--rw-rw-rw-  2.0 fat      852 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/tools_manager.py
--rw-rw-rw-  2.0 fat     4411 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/vector_db_lookup.py
--rw-rw-rw-  2.0 fat     2758 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/vector_index_lookup.py
--rw-rw-rw-  2.0 fat      101 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/__init__.py
--rw-rw-rw-  2.0 fat      309 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/adapter.py
--rw-rw-rw-  2.0 fat     1609 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/adapter_factory.py
--rw-rw-rw-  2.0 fat     4658 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/connection_based_adapter.py
--rw-rw-rw-  2.0 fat      975 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/local_faiss_adapter.py
--rw-rw-rw-  2.0 fat    12674 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/ml_index_adapter.py
--rw-rw-rw-  2.0 fat      974 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/adapter/remote_store_faiss_adapter.py
--rw-rw-rw-  2.0 fat      143 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/__init__.py
--rw-rw-rw-  2.0 fat      537 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler.py
--rw-rw-rw-  2.0 fat     1169 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler_factory.py
--rw-rw-rw-  2.0 fat      635 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/env_connection_handler.py
--rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/keyvault_connection_hander.py
--rw-rw-rw-  2.0 fat     2515 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/workspace_connection_handler.py
--rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_extensions/__init__.py
--rw-rw-rw-  2.0 fat     4241 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_extensions/acs.py
--rw-rw-rw-  2.0 fat     1887 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_extensions/utils.py
--rw-rw-rw-  2.0 fat      613 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/__init__.py
--rw-rw-rw-  2.0 fat     4040 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/acs.py
--rw-rw-rw-  2.0 fat      533 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/constants.py
--rw-rw-rw-  2.0 fat     4124 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py
--rw-rw-rw-  2.0 fat     1819 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/index_types.py
--rw-rw-rw-  2.0 fat      478 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/indices.py
--rw-rw-rw-  2.0 fat    12709 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/mapping.py
--rw-rw-rw-  2.0 fat     2005 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py
--rw-rw-rw-  2.0 fat     1937 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py
--rw-rw-rw-  2.0 fat     1814 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/query_types.py
--rw-rw-rw-  2.0 fat     2379 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/common_index_lookup_utils/utils.py
--rw-rw-rw-  2.0 fat       89 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/__init__.py
--rw-rw-rw-  2.0 fat     5050 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/config.py
--rw-rw-rw-  2.0 fat      230 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/constants.py
--rw-rw-rw-  2.0 fat     1512 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/ml_index_yaml_config.py
--rw-rw-rw-  2.0 fat      899 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/telemetry.py
--rw-rw-rw-  2.0 fat      942 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/types.py
--rw-rw-rw-  2.0 fat      322 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/contracts/ui_config.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/__init__.py
--rw-rw-rw-  2.0 fat     1539 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/logging.py
--rw-rw-rw-  2.0 fat     3616 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/pf_exception_helpers.py
--rw-rw-rw-  2.0 fat     3372 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/pf_runtime_utils.py
--rw-rw-rw-  2.0 fat      497 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/profiling.py
--rw-rw-rw-  2.0 fat     1944 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/store_core_provider.py
--rw-rw-rw-  2.0 fat     2549 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/workspace_connection_manager.py
--rw-rw-rw-  2.0 fat      889 b- defN 24-Mar-18 20:28 promptflow_vectordb/tool/utils/yaml_parser.py
--rw-rw-rw-  2.0 fat    11513 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml
--rw-rw-rw-  2.0 fat      457 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/yamls/azure/vector_index_lookup.yaml
--rw-rw-rw-  2.0 fat      443 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml
--rw-rw-rw-  2.0 fat     1507 b- defN 24-Mar-18 20:29 promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml
--rw-rw-rw-  2.0 fat     2953 b- defN 24-Mar-18 20:43 promptflow_vectordb-0.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-18 20:43 promptflow_vectordb-0.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      200 b- defN 24-Mar-18 20:43 promptflow_vectordb-0.2.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-18 20:43 promptflow_vectordb-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    14919 b- defN 24-Mar-18 20:43 promptflow_vectordb-0.2.6.dist-info/RECORD
-138 files, 294870 bytes uncompressed, 83589 bytes compressed:  71.7%
+Zip file size: 109816 bytes, number of entries: 139
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/__init__.py
+-rw-rw-rw-  2.0 fat       18 b- defN 24-Apr-01 18:19 promptflow_vectordb/_version.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/connections/__init__.py
+-rw-rw-rw-  2.0 fat      255 b- defN 24-Apr-01 18:19 promptflow_vectordb/connections/pinecone.py
+-rw-rw-rw-  2.0 fat      251 b- defN 24-Apr-01 18:19 promptflow_vectordb/connections/qdrant.py
+-rw-rw-rw-  2.0 fat      255 b- defN 24-Apr-01 18:19 promptflow_vectordb/connections/weaviate.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/__init__.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddingstore_core.py
+-rw-rw-rw-  2.0 fat      847 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     6006 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/config.py
+-rw-rw-rw-  2.0 fat      514 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/constants.py
+-rw-rw-rw-  2.0 fat      398 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/entities.py
+-rw-rw-rw-  2.0 fat     3492 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/exceptions.py
+-rw-rw-rw-  2.0 fat     1458 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/identifier_converter.py
+-rw-rw-rw-  2.0 fat      536 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/secret.py
+-rw-rw-rw-  2.0 fat     1693 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/telemetry.py
+-rw-rw-rw-  2.0 fat     1370 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/contracts/types.py
+-rw-rw-rw-  2.0 fat      109 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/__init__.py
+-rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/aoai_embedding.py
+-rw-rw-rw-  2.0 fat      690 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/customized_embedding.py
+-rw-rw-rw-  2.0 fat      165 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/embedding.py
+-rw-rw-rw-  2.0 fat     1554 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/embedding_factory.py
+-rw-rw-rw-  2.0 fat      467 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/empty_embedding.py
+-rw-rw-rw-  2.0 fat      784 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/embeddings/openai_embedding.py
+-rw-rw-rw-  2.0 fat       97 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/engine/__init__.py
+-rw-rw-rw-  2.0 fat     1504 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/engine/engine.py
+-rw-rw-rw-  2.0 fat     1950 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/engine/engine_factory.py
+-rw-rw-rw-  2.0 fat     4207 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/engine/langchain_engine.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/logging/__init__.py
+-rw-rw-rw-  2.0 fat     5505 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/logging/handlers.py
+-rw-rw-rw-  2.0 fat     5224 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/logging/loggers.py
+-rw-rw-rw-  2.0 fat     4304 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/logging/utils.py
+-rw-rw-rw-  2.0 fat      124 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/__init__.py
+-rw-rw-rw-  2.0 fat     1560 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/aml_data_store_client.py
+-rw-rw-rw-  2.0 fat     4682 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/azure_blob_client.py
+-rw-rw-rw-  2.0 fat     2936 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/github_client.py
+-rw-rw-rw-  2.0 fat     3344 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/http_client.py
+-rw-rw-rw-  2.0 fat      661 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/remote_client.py
+-rw-rw-rw-  2.0 fat     2799 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/remote_client/remote_client_factory.py
+-rw-rw-rw-  2.0 fat       94 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/store/__init__.py
+-rw-rw-rw-  2.0 fat     1610 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/store/in_memory_store.py
+-rw-rw-rw-  2.0 fat     5351 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/store/local_based_store.py
+-rw-rw-rw-  2.0 fat     4852 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/store/remote_based_store.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/store/store.py
+-rw-rw-rw-  2.0 fat     1323 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/store/store_factory.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/__init__.py
+-rw-rw-rw-  2.0 fat     7724 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/aml_helpers.py
+-rw-rw-rw-  2.0 fat     1794 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/azure_helpers.py
+-rw-rw-rw-  2.0 fat     1560 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/common_utils.py
+-rw-rw-rw-  2.0 fat      853 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/global_instance_manager.py
+-rw-rw-rw-  2.0 fat      663 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/index_factory.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/path_utils.py
+-rw-rw-rw-  2.0 fat     1397 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/retry_utils.py
+-rw-rw-rw-  2.0 fat     2319 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/secret_manager.py
+-rw-rw-rw-  2.0 fat      472 b- defN 24-Apr-01 18:19 promptflow_vectordb/core/utils/singleton_meta.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/__init__.py
+-rw-rw-rw-  2.0 fat     4003 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/embeddingstore_client.py
+-rw-rw-rw-  2.0 fat       93 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/__init__.py
+-rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/agent.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/agent_factory.py
+-rw-rw-rw-  2.0 fat     3093 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/cog_search_client.py
+-rw-rw-rw-  2.0 fat      762 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/file_based_agent.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/milvus_client.py
+-rw-rw-rw-  2.0 fat     4552 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/pinecone_client.py
+-rw-rw-rw-  2.0 fat     2518 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/qdrant_client.py
+-rw-rw-rw-  2.0 fat     3135 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/rest_based_agent.py
+-rw-rw-rw-  2.0 fat     2655 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/client/agent/weaviate_client.py
+-rw-rw-rw-  2.0 fat      367 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     4333 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/config.py
+-rw-rw-rw-  2.0 fat      665 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/constants.py
+-rw-rw-rw-  2.0 fat      370 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/errors.py
+-rw-rw-rw-  2.0 fat     2990 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/request_obj.py
+-rw-rw-rw-  2.0 fat      779 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/telemetry.py
+-rw-rw-rw-  2.0 fat      330 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/contracts/types.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/server/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/server/rest/__init__.py
+-rw-rw-rw-  2.0 fat     7170 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/server/rest/app.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/server/utils/__init__.py
+-rw-rw-rw-  2.0 fat     7892 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/server/utils/store_request_manager.py
+-rw-rw-rw-  2.0 fat     1123 b- defN 24-Apr-01 18:19 promptflow_vectordb/service/server/utils/sys_utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/__init__.py
+-rw-rw-rw-  2.0 fat     4013 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup.py
+-rw-rw-rw-  2.0 fat     3752 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/faiss_index_lookup.py
+-rw-rw-rw-  2.0 fat      852 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/tools_manager.py
+-rw-rw-rw-  2.0 fat     4411 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/vector_db_lookup.py
+-rw-rw-rw-  2.0 fat     2758 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/vector_index_lookup.py
+-rw-rw-rw-  2.0 fat      101 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/__init__.py
+-rw-rw-rw-  2.0 fat      309 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/adapter.py
+-rw-rw-rw-  2.0 fat     1609 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/adapter_factory.py
+-rw-rw-rw-  2.0 fat     4658 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/connection_based_adapter.py
+-rw-rw-rw-  2.0 fat      975 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/local_faiss_adapter.py
+-rw-rw-rw-  2.0 fat    12674 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_adapter.py
+-rw-rw-rw-  2.0 fat      974 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/remote_store_faiss_adapter.py
+-rw-rw-rw-  2.0 fat      143 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/__init__.py
+-rw-rw-rw-  2.0 fat      537 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler.py
+-rw-rw-rw-  2.0 fat     1169 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler_factory.py
+-rw-rw-rw-  2.0 fat      635 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/env_connection_handler.py
+-rw-rw-rw-  2.0 fat     1188 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/keyvault_connection_hander.py
+-rw-rw-rw-  2.0 fat     2515 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/workspace_connection_handler.py
+-rw-rw-rw-  2.0 fat       51 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_extensions/__init__.py
+-rw-rw-rw-  2.0 fat     4348 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_extensions/acs.py
+-rw-rw-rw-  2.0 fat     2417 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_extensions/utils.py
+-rw-rw-rw-  2.0 fat      656 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/__init__.py
+-rw-rw-rw-  2.0 fat     4040 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/acs.py
+-rw-rw-rw-  2.0 fat      911 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/constants.py
+-rw-rw-rw-  2.0 fat     6088 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/index_types.py
+-rw-rw-rw-  2.0 fat      478 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/indices.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/logger.py
+-rw-rw-rw-  2.0 fat    13580 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/mapping.py
+-rw-rw-rw-  2.0 fat     2005 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py
+-rw-rw-rw-  2.0 fat     1937 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py
+-rw-rw-rw-  2.0 fat     1814 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/query_types.py
+-rw-rw-rw-  2.0 fat     2184 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/common_index_lookup_utils/utils.py
+-rw-rw-rw-  2.0 fat       89 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     5050 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/config.py
+-rw-rw-rw-  2.0 fat      230 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/constants.py
+-rw-rw-rw-  2.0 fat     1512 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/ml_index_yaml_config.py
+-rw-rw-rw-  2.0 fat      899 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/telemetry.py
+-rw-rw-rw-  2.0 fat      942 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/types.py
+-rw-rw-rw-  2.0 fat      322 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/contracts/ui_config.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1539 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/logging.py
+-rw-rw-rw-  2.0 fat     3616 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/pf_exception_helpers.py
+-rw-rw-rw-  2.0 fat     3372 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/pf_runtime_utils.py
+-rw-rw-rw-  2.0 fat      747 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/profiling.py
+-rw-rw-rw-  2.0 fat     1944 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/store_core_provider.py
+-rw-rw-rw-  2.0 fat     2549 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/workspace_connection_manager.py
+-rw-rw-rw-  2.0 fat      889 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/utils/yaml_parser.py
+-rw-rw-rw-  2.0 fat    12054 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml
+-rw-rw-rw-  2.0 fat      457 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/yamls/azure/vector_index_lookup.yaml
+-rw-rw-rw-  2.0 fat      443 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml
+-rw-rw-rw-  2.0 fat     1507 b- defN 24-Apr-01 18:19 promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml
+-rw-rw-rw-  2.0 fat     3224 b- defN 24-Apr-01 18:24 promptflow_vectordb-0.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 18:24 promptflow_vectordb-0.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      200 b- defN 24-Apr-01 18:24 promptflow_vectordb-0.2.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-01 18:24 promptflow_vectordb-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    15036 b- defN 24-Apr-01 18:24 promptflow_vectordb-0.2.7.dist-info/RECORD
+139 files, 300639 bytes uncompressed, 84710 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -321,14 +321,17 @@
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/index_types.py
 Comment: 
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/indices.py
 Comment: 
 
+Filename: promptflow_vectordb/tool/common_index_lookup_utils/logger.py
+Comment: 
+
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/mapping.py
 Comment: 
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py
 Comment: 
 
 Filename: promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py
@@ -393,23 +396,23 @@
 
 Filename: promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml
 Comment: 
 
 Filename: promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml
 Comment: 
 
-Filename: promptflow_vectordb-0.2.6.dist-info/METADATA
+Filename: promptflow_vectordb-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: promptflow_vectordb-0.2.6.dist-info/WHEEL
+Filename: promptflow_vectordb-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow_vectordb-0.2.6.dist-info/entry_points.txt
+Filename: promptflow_vectordb-0.2.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: promptflow_vectordb-0.2.6.dist-info/top_level.txt
+Filename: promptflow_vectordb-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: promptflow_vectordb-0.2.6.dist-info/RECORD
+Filename: promptflow_vectordb-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow_vectordb/_version.py

```diff
@@ -1 +1 @@
-VERSION = "0.2.6"
+VERSION = "0.2.7"
```

## promptflow_vectordb/tool/common_index_lookup.py

```diff
@@ -1,95 +1,84 @@
-from .utils.profiling import measure_execution_time
-from .common_index_lookup_extensions import build_search_func
-
-from azureml.rag.mlindex import MLIndex
-from azureml.rag.utils.logging import enable_stdout_logging
-from concurrent.futures import ThreadPoolExecutor
 import contextvars
-from functools import lru_cache
 import json
-import logging
+from concurrent.futures import ThreadPoolExecutor
+from functools import lru_cache
+from typing import List, Union
+
+from azureml.rag.mlindex import MLIndex
 from opentelemetry import trace
-import os
 from promptflow import tool
 from promptflow.exceptions import UserErrorException
 from ruamel.yaml import YAML
-from typing import List, Union
+
+from ..core.logging.utils import LoggingUtils
+from .common_index_lookup_extensions import build_search_func
+from .common_index_lookup_utils.constants import LoggingEvents
+from .common_index_lookup_utils.logger import promptflow_logger
+from .utils.profiling import measure_execution_time
 
 tracer = trace.get_tracer(__name__)
 yaml = YAML()
 
-__LOG_LEVEL_ENV_KEY = 'PF_LOGGING_LEVEL'
-try:
-    __LOG_LEVEL_MAPPINGS = logging.getLevelNamesMapping()
-except AttributeError:
-    # logging.getLevelNamesMapping was only introduced in 3.11; fallback for older versions
-    __LOG_LEVEL_MAPPINGS = {
-        'CRITICAL': logging.CRITICAL,
-        'ERROR': logging.ERROR,
-        'WARNING': logging.WARNING,
-        'INFO': logging.INFO,
-        'DEBUG': logging.DEBUG,
-    }
-
 
 @lru_cache(maxsize=32)
 def _get_search_func(mlindex_content: str, top_k: int, query_type: str):
-    with measure_execution_time('search_function_construction'):
+    with measure_execution_time(LoggingEvents.SearchFunctionConstruction):
         mlindex_config = yaml.load(mlindex_content)
         index = MLIndex(mlindex_config=mlindex_config)
         search_func = build_search_func(index, top_k, query_type)
 
-    with measure_execution_time('telemetry_wrapper_construction'):
+    with measure_execution_time(LoggingEvents.TelemetryWrapperConstruction):
+
         def telemetry_wrapper(query: str):
             with tracer.start_as_current_span("search") as span:
                 span.set_attribute("span_type", "Retrieval")
                 span.set_attribute("retrieval.query", query)
-                with measure_execution_time('search_function_inner_execution'):
+                with measure_execution_time(LoggingEvents.SearchFunctionInnerExecution):
                     search_result = search_func(query)
 
                 try:
                     loggable_results = [
                         {
                             "document.content": doc.page_content,
                             "document.score": score,
-                            "document.metadata": doc.metadata
+                            "document.metadata": doc.metadata,
                         }
-                        for doc, score in search_result]
-                    span.set_attribute("retrieval.documents", json.dumps(loggable_results))
+                        for doc, score in search_result
+                    ]
+                    span.set_attribute(
+                        "retrieval.documents", json.dumps(loggable_results)
+                    )
                 except Exception as ex:
-                    span.set_attribute("retrieval.documents.serialization_error", str(ex))
+                    span.set_attribute(
+                        "retrieval.documents.serialization_error", str(ex)
+                    )
                 return search_result
 
         return telemetry_wrapper
 
 
 def _set_context_vars(context: contextvars.Context):
     for var, value in context.items():
         var.set(value)
 
 
-@lru_cache(maxsize=1)
-def _set_log_level(log_level):
-    enable_stdout_logging(log_level)
-
-    root = logging.getLogger()
-    root.setLevel(log_level)
-
-
 @tool
+@LoggingUtils.log_event(
+    package_name=__package__,
+    event_name=LoggingEvents.AzureMLRagSearch,
+    logger=promptflow_logger,
+    flush=True,
+)
 def search(
     mlindex_content: str,
     queries: Union[str, List[str]],
     top_k: int,
     query_type: str,
 ) -> List[List[dict]]:
-    log_level = __LOG_LEVEL_MAPPINGS.get(os.getenv(__LOG_LEVEL_ENV_KEY), logging.INFO)
-    _set_log_level(log_level)
-
     if isinstance(queries, str):
         queries = [queries]
         unwrap = True
     elif isinstance(queries, list) and all([isinstance(q, str) for q in queries]):
         unwrap = False
     elif isinstance(queries, list) and all([isinstance(q, float) for q in queries]):
         raise UserErrorException(
@@ -100,21 +89,24 @@
         raise UserErrorException(
             "Expected input type to be either `str` or `List[str]`."
         )
 
     search_func = _get_search_func(mlindex_content, top_k, query_type)
 
     parent_context = contextvars.copy_context()
-    with measure_execution_time('search_function_execution'):
-        with ThreadPoolExecutor(initializer=_set_context_vars, initargs=(parent_context,)) as search_executor:
+    with measure_execution_time(LoggingEvents.SearchFunctionExecution):
+        with ThreadPoolExecutor(
+            initializer=_set_context_vars, initargs=(parent_context,)
+        ) as search_executor:
             search_results = search_executor.map(search_func, queries)
-            results = [[
-                {
-                    'text': doc.page_content,
-                    'metadata': doc.metadata,
-                    'score': score
-                } for doc, score in search_result] for search_result in search_results]
+            results = [
+                [
+                    {"text": doc.page_content, "metadata": doc.metadata, "score": score}
+                    for doc, score in search_result
+                ]
+                for search_result in search_results
+            ]
 
     if unwrap and len(results) == 1:
         return results[0]
     else:
         return results
```

## promptflow_vectordb/tool/common_index_lookup_extensions/acs.py

```diff
@@ -1,76 +1,71 @@
 import json
 from langchain.docstore.document import Document
-from langchain.vectorstores import AzureSearch
 from typing import Dict, List, Optional, Tuple
 
 
 def simple_search_with_score(
         query: str,
-        store: AzureSearch,
+        store: "langchain.vectorstores.AzureSearch",
         k: int = 4,
+        field_mapping: Dict[str, str] = None,
         filters: Optional[str] = None
 ) -> List[Tuple[Document, float]]:
-    from langchain.vectorstores.azuresearch import (
-        FIELDS_CONTENT,
-        FIELDS_CONTENT_VECTOR,
-        FIELDS_METADATA,
-    )
+    content_field = (field_mapping or {}).get("content") or "content"
+    embedding_field = (field_mapping or {}).get("embedding") or "contentVector"
+    metadata_field = (field_mapping or {}).get("metadata") or "meta_json_string"
 
     results = store.client.search(
         search_text=query,
         query_type='simple',
         filter=filters,
         top=k,
     )
 
     # Convert results to Document objects
     docs = [
         (
             Document(
-                page_content=result.pop(FIELDS_CONTENT),
-                metadata=json.loads(result[FIELDS_METADATA])
-                if FIELDS_METADATA in result
-                else {
-                    k: v for k, v in result.items() if k != FIELDS_CONTENT_VECTOR
-                },
+                page_content=result.pop(content_field),
+                metadata=json.loads(result[metadata_field])
+                if metadata_field in result
+                else {k: v for k, v in result.items() if k != embedding_field},
             ),
             float(result['@search.score']),
         )
         for result in results
     ]
 
     return docs
 
 
 def semantic_search_with_score(
-        query: str, store:
-        AzureSearch,
+        query: str,
+        store: "langchain.vectorstores.AzureSearch",
         k: int = 4,
         hybrid: bool = False,
+        field_mapping: Dict[str, str] = None,
         filters: Optional[str] = None
 ) -> List[Tuple[Document, float]]:
-    from langchain.vectorstores.azuresearch import (
-        FIELDS_CONTENT,
-        FIELDS_CONTENT_VECTOR,
-        FIELDS_METADATA,
-    )
+    content_field = (field_mapping or {}).get("content") or "content"
+    embedding_field = (field_mapping or {}).get("embedding") or "contentVector"
+    metadata_field = (field_mapping or {}).get("metadata") or "meta_json_string"
 
     if hybrid:
         from azure.search.documents.models import Vector
         import numpy as np
         results = store.client.search(
             search_text=query,
             vectors=[
                 Vector(
                     value=np.array(
                         store.embedding_function(query), dtype=np.float32
                     ).tolist(),
                     k=50,
-                    fields=FIELDS_CONTENT_VECTOR,
+                    fields=embedding_field,
                 )
             ],
             filter=filters,
             query_type='semantic',
             query_language=store.semantic_query_language,
             semantic_configuration_name=store.semantic_configuration_name,
             query_caption='extractive',
@@ -97,24 +92,20 @@
             'text': semantic_answer.text,
             'highlights': semantic_answer.highlights,
         }
 
     docs = [
         (
             Document(
-                page_content=result.pop(FIELDS_CONTENT),
+                page_content=result.pop(content_field),
                 metadata={
                     **(
-                        json.loads(result[FIELDS_METADATA])
-                        if FIELDS_METADATA in result
-                        else {
-                            k: v
-                            for k, v in result.items()
-                            if k != FIELDS_CONTENT_VECTOR
-                        }
+                        json.loads(result[metadata_field])
+                        if metadata_field in result
+                        else {k: v for k, v in result.items() if k != embedding_field}
                     ),
                     **{
                         'captions': {
                             'text': result.get('@search.captions', [{}])[0].text,
                             'highlights': result.get('@search.captions', [{}])[
                                 0
                             ].highlights,
```

## promptflow_vectordb/tool/common_index_lookup_extensions/utils.py

```diff
@@ -1,15 +1,14 @@
 from .acs import simple_search_with_score, semantic_search_with_score
 
 from ..common_index_lookup_utils.constants import QueryTypes
 
 from azureml.rag import MLIndex
 import functools
 from langchain.docstore.document import Document
-from langchain.vectorstores import AzureSearch
 from typing import Callable, List, Tuple
 
 
 def build_search_func(index: MLIndex, top_k: int, query_type: str) -> Callable[[str], List[Tuple[Document, float]]]:
     # Override the embeddings section if we're making keyword queries.
     if query_type in {QueryTypes.Simple, QueryTypes.Semantic}:
         index.embeddings_config = {
@@ -17,29 +16,48 @@
             'kind': 'none'
         }
 
         # Temporary workaround for `as_langchain_vectorstore` throwing when field_mapping.embedding is None.
         if 'field_mapping' in index.index_config:
             index.index_config['field_mapping']['embedding'] = ''
 
+    index_kind = index.index_config.get("kind", "none")
     store = index.as_langchain_vectorstore()
 
-    if query_type == QueryTypes.Simple:
-        return functools.partial(simple_search_with_score, store=store, k=top_k)
+    if index_kind == 'acs':
+        if query_type == QueryTypes.Simple:
+            return functools.partial(
+                simple_search_with_score,
+                store=store,
+                k=top_k,
+                field_mapping=index.index_config.get('field_mapping')
+            )
+
+        if query_type == QueryTypes.Semantic:
+            return functools.partial(
+                semantic_search_with_score,
+                store=store,
+                k=top_k,
+                field_mapping=index.index_config.get('field_mapping'),
+                hybrid=False
+            )
 
-    if query_type == QueryTypes.Semantic:
-        return functools.partial(semantic_search_with_score, store=store, k=top_k, hybrid=False)
-
-    if query_type == QueryTypes.Vector:
-        if isinstance(store, AzureSearch):
+        if query_type == QueryTypes.Vector:
             # AzureSearch doesn't implement similiarity_search_with_score
             return functools.partial(store.vector_search_with_score, k=top_k)
-        else:
-            return functools.partial(store.similarity_search_with_score, k=top_k)
 
-    if query_type == QueryTypes.VectorSimpleHybrid:
-        return functools.partial(store.hybrid_search_with_score, k=top_k)
+        if query_type == QueryTypes.VectorSimpleHybrid:
+            return functools.partial(store.hybrid_search_with_score, k=top_k)
 
-    if query_type == QueryTypes.VectorSemanticHybrid:
-        return functools.partial(semantic_search_with_score, store=store, k=top_k, hybrid=True)
+        if query_type == QueryTypes.VectorSemanticHybrid:
+            return functools.partial(
+                semantic_search_with_score,
+                store=store,
+                k=top_k,
+                field_mapping=index.index_config.get('field_mapping'),
+                hybrid=True
+            )
+    else:
+        if query_type == QueryTypes.Vector:
+            return functools.partial(store.similarity_search_with_score, k=top_k)
 
-    raise ValueError(f'Unsupported query type: {query_type}')
+    raise ValueError(f'Unsupported query type: {query_type} for index kind {index_kind}.')
```

## promptflow_vectordb/tool/common_index_lookup_utils/__init__.py

```diff
@@ -1,14 +1,15 @@
 from .acs import (  # noqa: F401
     list_acs_indices,
     list_acs_index_fields,
     list_acs_index_semantic_configurations)
 from .embeddings import (  # noqa: F401
     list_available_embedding_types,
     list_embedding_models,
-    list_aoai_embedding_deployments)
+    list_aoai_embedding_deployments,
+    list_serverless_embedding_connections)
 from .index_types import list_available_index_types  # noqa: F401
 from .indices import list_registered_mlindices  # noqa: F401
 from .pinecone import list_pinecone_connections, list_pinecone_indices  # noqa: F401
 from .query_types import list_available_query_types  # noqa: F401
 
 from .mapping import forward_mapping, reverse_mapping  # noqa: F401
```

## promptflow_vectordb/tool/common_index_lookup_utils/constants.py

```diff
@@ -1,21 +1,30 @@
 class IndexTypes(str):
-    AzureCognitiveSearch = 'Azure AI Search'
-    FAISS = 'FAISS'
-    Pinecone = 'Pinecone'
-    MLIndexAsset = 'Registered Index'
-    MLIndexPath = 'MLIndex file from path'
+    AzureCognitiveSearch = "Azure AI Search"
+    FAISS = "FAISS"
+    Pinecone = "Pinecone"
+    MLIndexAsset = "Registered Index"
+    MLIndexPath = "MLIndex file from path"
 
 
 class EmbeddingTypes(str):
-    NoEmbedding = 'None'
-    AzureOpenAI = 'Azure OpenAI'
-    OpenAI = 'OpenAI'
-    HuggingFace = 'Hugging Face'
+    NoEmbedding = "None"
+    AzureOpenAI = "Azure OpenAI"
+    OpenAI = "OpenAI"
+    HuggingFace = "Hugging Face"
+    ServerlessEndpoint = "Serverless Endpoint"
 
 
 class QueryTypes(str):
-    Simple = 'Keyword'
-    Semantic = 'Semantic'
-    Vector = 'Vector'
-    VectorSimpleHybrid = 'Hybrid (vector + keyword)'
-    VectorSemanticHybrid = 'Hybrid + semantic'
+    Simple = "Keyword"
+    Semantic = "Semantic"
+    Vector = "Vector"
+    VectorSimpleHybrid = "Hybrid (vector + keyword)"
+    VectorSemanticHybrid = "Hybrid + semantic"
+
+
+class LoggingEvents(str):
+    SearchFunctionConstruction = "search_function_construction"
+    SearchFunctionExecution = "search_function_execution"
+    SearchFunctionInnerExecution = "search_function_inner_execution"
+    AzureMLRagSearch = "azureml_rag_search"
+    TelemetryWrapperConstruction = "telemetry_wrapper_construction"
```

## promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py

```diff
@@ -19,19 +19,26 @@
         workspace_name=context.workspace_name,
         cls=lambda objs: objs,
         category=None,
         **context.ml_client.connections._scope_kwargs)
 
     workspace_contains_aoai_connection = False
     workspace_contains_oai_connection = False
+    workspace_contains_serverless_connection = False
     for connection in connections:
         if connection.properties.category == 'AzureOpenAI':
             workspace_contains_aoai_connection = True
 
-        if workspace_contains_aoai_connection and workspace_contains_oai_connection:
+        if connection.properties.category == 'Serverless':
+            if connection.properties.metadata.get('SERVED_MODEL_TYPE') in {None, 'embedding'}:
+                workspace_contains_serverless_connection = True
+
+        if workspace_contains_aoai_connection and \
+                workspace_contains_oai_connection and \
+                workspace_contains_serverless_connection:
             break
 
     embedding_types = []
 
     # This should be the set of index backends that support embedding-less querying (eg, Keyword).
     # At present, this includes only Azure Cog Search.
     if index_type in {IndexTypes.AzureCognitiveSearch}:
@@ -39,14 +46,18 @@
 
     if workspace_contains_aoai_connection:
         embedding_types.append({'value': EmbeddingTypes.AzureOpenAI, 'displayValue': EmbeddingTypes.AzureOpenAI})
 
     if workspace_contains_oai_connection:
         embedding_types.append({'value': EmbeddingTypes.OpenAI, 'displayValue': EmbeddingTypes.OpenAI})
 
+    if workspace_contains_serverless_connection:
+        embedding_types.append(
+            {'value': EmbeddingTypes.ServerlessEndpoint, 'displayValue': EmbeddingTypes.ServerlessEndpoint})
+
     if SentenceTransformerIsInstalled():
         embedding_types.append({'value': EmbeddingTypes.HuggingFace, 'displayValue': EmbeddingTypes.HuggingFace})
 
     return embedding_types
 
 
 @tool_ui_callback
@@ -93,7 +104,43 @@
             f'{depl.get("properties", dict()).get("model", dict()).get("version")}'
          in embedding_models]
 
     return [{
         'value': depl.get('name'),
         'display_value': depl.get('name'),
     } for depl in embedding_deployments]
+
+
+@tool_ui_callback
+def list_serverless_embedding_connections(context: CallbackContext) -> List[Dict[str, str]]:
+    connections = context.ml_client.connections._operation.list(
+        workspace_name=context.workspace_name,
+        cls=lambda objs: objs,
+        category='Serverless',
+        **context.ml_client.connections._scope_kwargs)
+
+    serverless_connections = []
+    for connection in connections:
+        if connection.properties.metadata.get('SERVED_MODEL_TYPE') in {None, 'embedding'}:
+            connection_entry = {
+                'value': connection.name,
+                'display_value': connection.name,
+            }
+
+            model_provider = connection.properties.metadata.get('MODEL_PROVIDER_NAME')
+            model_name = connection.properties.metadata.get('SERVED_MODEL_NAME')
+
+            if model_provider and model_name:
+                model_description = f'the {model_provider} "{model_name}"'
+            elif model_provider:
+                model_description = f'an unknown {model_provider}'
+            elif model_name:
+                model_description = f'the "{model_name}"'
+            else:
+                model_description = 'an unknown'
+
+            connection_entry['description'] = \
+                f'Serverless endpoint deployment of {model_description} embedding model.'
+
+            serverless_connections.append(connection_entry)
+
+    return serverless_connections
```

## promptflow_vectordb/tool/common_index_lookup_utils/mapping.py

```diff
@@ -1,12 +1,13 @@
 from .constants import IndexTypes, EmbeddingTypes
 from .mlindex_client import MLIndexClient
 from .utils import CallbackContext, tool_ui_callback
 
 from azureml.rag.mlindex import MLIndex
+from azureml.rag.embeddings import EmbeddingsContainer
 from io import StringIO
 import os
 from ruamel.yaml import YAML
 from typing import Any, Dict
 import tempfile
 
 yaml = YAML()
@@ -30,14 +31,15 @@
     pinecone_content_field: str = None,
     pinecone_metadata_field: str = None,
     embedding_type: str = None,
     aoai_embedding_connection: str = None,
     oai_embedding_connection: str = None,
     embedding_model: str = None,
     embedding_deployment: str = None,
+    serverless_embedding_connection: str = None
 ) -> str:
     if index_type in {IndexTypes.MLIndexAsset, IndexTypes.MLIndexPath}:
         mlindex_client = MLIndexClient(context)
         if index_type == IndexTypes.MLIndexAsset:
 
             asset_id_parts = mlindex_asset_id.split('/')
             asset_name = asset_id_parts[7]
@@ -83,15 +85,16 @@
                 pinecone_metadata_field),
             'embeddings': get_embeddings_config(
                 context,
                 embedding_type,
                 aoai_embedding_connection,
                 oai_embedding_connection,
                 embedding_model,
-                embedding_deployment),
+                embedding_deployment,
+                serverless_embedding_connection),
         }
 
         mlindex = MLIndex(mlindex_config=mlindex_config)
         with tempfile.TemporaryDirectory() as staging_dir:
             mlindex.save(staging_dir, just_config=True)
             with open(os.path.join(staging_dir, 'MLIndex'), 'r', encoding='utf-8') as src:
                 return src.read()
@@ -167,14 +170,23 @@
                 .split("/")[-1],
                 "embedding_deployment": mlindex.embeddings_config.get("deployment"),
             }
         else:
             raise NotImplementedError(
                 '"azure" is the only supported value for embedding api_type.'
             )
+    elif embedding_kind == "serverless_endpoint":
+        mapped_embedding_args = {
+            "embedding_type": EmbeddingTypes.ServerlessEndpoint,
+            "serverless_embedding_connection": mlindex.embeddings_config.get(
+                "connection", {}
+            )
+            .get("id", "")
+            .split("/")[-1],
+        }
     elif embedding_kind == "hugging_face":
         mapped_embedding_args = {
             "embedding_type": EmbeddingTypes.HuggingFace,
             "embedding_model": mlindex.embedding_configs.get("model"),
         }
     else:
         raise NotImplementedError(
@@ -187,63 +199,85 @@
 def get_embeddings_config(
     context: CallbackContext,
     embedding_type: str = None,
     aoai_embedding_connection: str = None,
     oai_embedding_connection: str = None,
     embedding_model: str = None,
     embedding_deployment: str = None,
+    serverless_embedding_connection: str = None,
 ) -> Dict[str, Any]:
     if not embedding_type or embedding_type == EmbeddingTypes.NoEmbedding:
         return {
             "kind": "none",
             "schema_version": "2",
         }
 
-    if embedding_type == EmbeddingTypes.AzureOpenAI:
+    elif embedding_type == EmbeddingTypes.AzureOpenAI:
         selected_connection = context.ml_client.connections._operation.get(
             workspace_name=context.workspace_name,
             connection_name=aoai_embedding_connection,
             **context.ml_client.connections._scope_kwargs,
         )
 
         resolved_embedding_model = _get_embedding_model(
             context, selected_connection, embedding_deployment
         )
-        return {
+        embeddings_config = {
             "kind": "open_ai",
             "api_type": "azure",
             "api_base": selected_connection.properties.target,
             "api_version": selected_connection.properties.metadata.get(
                 "ApiVersion", "2023-03-15-preview"
             ),
             "batch_size": "1",
             "connection": {
                 "id": selected_connection.id,
             },
             "connection_type": "workspace_connection",
             "deployment": embedding_deployment,
             "model": resolved_embedding_model,
-            "dimension": _get_embedding_dimension(
-                embedding_type, resolved_embedding_model
-            ),
             "schema_version": "2",
         }
 
-    if embedding_type == EmbeddingTypes.OpenAI:
+    elif embedding_type == EmbeddingTypes.OpenAI:
         raise NotImplementedError()
 
-    if embedding_type == EmbeddingTypes.HuggingFace:
-        return {
+    elif embedding_type == EmbeddingTypes.ServerlessEndpoint:
+        selected_connection = context.ml_client.connections._operation.get(
+            workspace_name=context.workspace_name,
+            connection_name=serverless_embedding_connection,
+            **context.ml_client.connections._scope_kwargs,
+        )
+
+        embeddings_config = {
+            "kind": "serverless_endpoint",
+            "api_type": selected_connection.properties.metadata.get("MODEL_PROVIDER_NAME", "cohere").lower(),
+            "api_base": selected_connection.properties.target,
+            "model": selected_connection.properties.metadata.get("SERVED_MODEL_NAME", "cohere-embed-english"),
+            "batch_size": "1",
+            "connection": {
+                "id": selected_connection.id,
+            },
+            "connection_type": "workspace_connection",
+            "schema_version": "2",
+        }
+
+    elif embedding_type == EmbeddingTypes.HuggingFace:
+        embeddings_config = {
             "kind": "hugging_face",
-            "dimension": _get_embedding_dimension(embedding_type, embedding_model),
             "model": embedding_model,
             "schema_version": "2",
         }
 
-    raise ValueError(f"Unexpected embedding type: {embedding_type}")
+    else:
+        raise ValueError(f"Unexpected embedding type: {embedding_type}")
+
+    embedder = EmbeddingsContainer.from_metadata(embeddings_config.copy()).get_query_embed_fn()
+    embeddings_config["dimension"] = len(embedder("hello world!"))
+    return embeddings_config
 
 
 def _get_index_config(
     context: CallbackContext,
     index_type: str,
     acs_index_connection: str = None,
     acs_index_name: str = None,
@@ -325,25 +359,7 @@
     )
     auth_header = f'Bearer {context.credential.get_token("https://management.azure.com/.default").token}'
     deployment = context.http.get(
         deployment_url, headers={"Authorization": auth_header}
     ).json()
 
     return deployment.get("properties", {}).get("model", {}).get("name")
-
-
-def _get_embedding_dimension(embedding_type: str, embedding_model: str) -> int:
-    return {
-        EmbeddingTypes.AzureOpenAI: {
-            "text-embedding-ada-002": 1536,
-            "text-embedding-3-small": 1536,
-            "text-embedding-3-large": 3072,
-        },
-        EmbeddingTypes.OpenAI: {
-            "text-embedding-ada-002": 1536,
-            "text-embedding-3-small": 1536,
-            "text-embedding-3-large": 3072,
-        },
-        EmbeddingTypes.HuggingFace: {
-            "sentence-transformers/all-mpnet-base-v2": 768,
-        },
-    }[embedding_type][embedding_model]
```

## promptflow_vectordb/tool/common_index_lookup_utils/utils.py

```diff
@@ -48,15 +48,12 @@
 
     @property
     def http(self):
         return CallbackContext.__http_session
 
 
 def tool_ui_callback(func):
-    # FIXME: Commented line below meant for enabling unit testing, but it breaks the runtime.
-    # Uncomment this line to run common lookup tool unit tests locally.
-    # @functools.wraps(func)
     def wrapper(subscription_id, resource_group_name, workspace_name, *args, **kwargs):
         context = CallbackContext.get(subscription_id, resource_group_name, workspace_name)
         return func(context, *args, **kwargs)
 
     return wrapper
```

## promptflow_vectordb/tool/utils/profiling.py

```diff
@@ -1,18 +1,24 @@
 import contextlib
-import logging
 from time import perf_counter
 from typing import Callable
 
+from ..common_index_lookup_utils.logger import promptflow_logger
+
 
 @contextlib.contextmanager
 def measure_execution_time(activity_name: str, callback: Callable = None):
     try:
         start_time = perf_counter()
         yield
+    except Exception:
+        promptflow_logger._telemetry_logger.exception(
+            f"Exception occured in {activity_name}."
+        )
+        raise
     finally:
         end_time = perf_counter()
-        log_message = f'`{activity_name}` completed in {end_time - start_time} seconds.'
+        log_message = f"`{activity_name}` completed in {end_time - start_time} seconds."
         if callback:
             callback(log_message)
         else:
-            logging.info(log_message)
+            promptflow_logger.telemetry(msg=log_message, event_name=activity_name)
```

## promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml

```diff
@@ -98,14 +98,19 @@
           optional: true
           reference: ${inputs.embedding_model}
         - name: embedding_deployment
           type:
           - string
           optional: true
           reference: ${inputs.embedding_deployment}
+        - name: serverless_embedding_connection
+          type:
+          - string
+          optional: true
+          reference: ${inputs.serverless_embedding_connection}
         reverse_func_path: promptflow_vectordb.tool.common_index_lookup_utils.reverse_mapping
     queries:
       type: 
       - object
     top_k:
       default: 3
       type:
@@ -389,11 +394,22 @@
         - name: aoai_connection
           type:
           - AzurOpenAIConnection
           optional: false
           reference: ${inputs.aoai_embedding_connection}
       allow_manual_entry: false
       is_multi_select: false
+    serverless_embedding_connection:
+      input_type: uionly_hidden
+      type:
+      - string
+      enabled_by: embedding_type
+      enabled_by_value:
+      - Serverless Endpoint
+      dynamic_list:
+        func_path: promptflow_vectordb.tool.common_index_lookup_utils.list_serverless_embedding_connections
+      allow_manual_entry: false
+      is_multi_select: false
   module: promptflow_vectordb.tool.common_index_lookup
   name: Index Lookup
   description: Search an AzureML Vector Index for relevant results using one or more text queries.
   type: python
```

## Comparing `promptflow_vectordb-0.2.6.dist-info/METADATA` & `promptflow_vectordb-0.2.7.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptflow_vectordb
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prompt flow tools for accessing popular vector databases
 Author: Microsoft Corporation
 Author-email: aethercn@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Description-Content-Type: text/markdown
 Requires-Dist: psutil
@@ -28,14 +28,19 @@
 Provides-Extra: hugging_face
 Requires-Dist: azureml.rag[hugging_face] >=0.2.23 ; extra == 'hugging_face'
 
 # Introduction
 
 To store and search over unstructured data, a widely adopted approach is embedding data into vectors, stored and indexed in vector databases. The promptflow-vectordb SDK is designed for PromptFlow, provides essential tools for vector similarity search within popular vector databases, including  FAISS, Qdrant, Azure Congnitive Search, and more.
 
+## 0.2.7
+- Add support for Serverless Endpoint connections for embeddings in `Index Lookup`.
+- Add support for multiple instances of `Index Lookup` running in the same process without conflicts.
+- Auto-detect embedding vector length for supported embedding models.
+
 ## 0.2.6
 - Emit granular trace information from `Index Lookup` for use by Action Analyzer.
 
 ## 0.2.5
 - Introduce improved error messaging when input queries are of an unexpected type.
 - Mark `FAISS Index Lookup`, `Vector Index Lookup` and `Vector DB Lookup` as archived.
 - Add support for `text-embedding-3-small` and `text-embedding-3-large` embedding models.
```

## Comparing `promptflow_vectordb-0.2.6.dist-info/RECORD` & `promptflow_vectordb-0.2.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 promptflow_vectordb/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-promptflow_vectordb/_version.py,sha256=XC2MYZybet-wsd8zs6MBULy8nzAc7dUW0vmpI8ttNTI,18
+promptflow_vectordb/_version.py,sha256=ZQLNbaBb3Roa6Z5LEm--iZickCQhYJVSrDpqf4YBbzc,18
 promptflow_vectordb/connections/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/connections/pinecone.py,sha256=YwFvw1QaFtx3CGSOTwCK5Tm9SsamGKqYqetJslE5qvk,255
 promptflow_vectordb/connections/qdrant.py,sha256=SFAG6l66RcIle5YB0SHTDrbVAU_6a5PFJ525i0rwrm8,251
 promptflow_vectordb/connections/weaviate.py,sha256=Pi1GeyduGy4WdWhQShZmtBV5jXqJ7kE1e9GR6zlMDsw,255
 promptflow_vectordb/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/core/embeddingstore_core.py,sha256=wJvGBmf8R4jrexb0sg2typehDDqKpYOSzNylsP-p1tM,7570
 promptflow_vectordb/core/contracts/__init__.py,sha256=eFCBv6fY_BBu8mNEPtD99RQtSzSiKhDGHmxy0H-5NSw,847
@@ -76,15 +76,15 @@
 promptflow_vectordb/service/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/service/server/rest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/service/server/rest/app.py,sha256=cNm_gec3eQ97SQjKXTAklTsfnAgSt_qHfrB1W8bFttM,7170
 promptflow_vectordb/service/server/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/service/server/utils/store_request_manager.py,sha256=PkwL4jwDrNHZu3q2bjA-RUev6cRa9CHQ7KZttZuiRMs,7892
 promptflow_vectordb/service/server/utils/sys_utils.py,sha256=xnBWoydnVQsvg92SiifMpaid5TelpLZm4aTVfAXvrPo,1123
 promptflow_vectordb/tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-promptflow_vectordb/tool/common_index_lookup.py,sha256=AC0KiwinedIq0VE1d1c3-y9P7tKnRhc-h_lM9m_-Qqo,4283
+promptflow_vectordb/tool/common_index_lookup.py,sha256=zcso0x_3bwjbTaJNDwYU5_GEohZvfZhOBYH91bV_kpU,4013
 promptflow_vectordb/tool/faiss_index_lookup.py,sha256=a5F5tleL2A-htc1lxqPjyLB16Mt-j-Ap4Wg2arTvJcA,3752
 promptflow_vectordb/tool/tools_manager.py,sha256=wHtbtQo53fT9HAMBHtp8zIrEgBw-BCZ1Ogl9Ks1RsZQ,852
 promptflow_vectordb/tool/vector_db_lookup.py,sha256=ZN2T5SyzuoWYfsEzaKxnEKl3_xYOshpIdZNFLaK2m1o,4411
 promptflow_vectordb/tool/vector_index_lookup.py,sha256=BKfWhcqEjuTIsIUf2hmtVLoMcW8Ul9ZE5zwyFfMqadc,2758
 promptflow_vectordb/tool/adapter/__init__.py,sha256=MFWKX1_d679pLONjxH-hf59HKN8JbOrNfzhMMDOSLqw,101
 promptflow_vectordb/tool/adapter/adapter.py,sha256=RhRZqaJK6OrEngJqYjPTpaqIgPvI9faEkDQUH-1BT_M,309
 promptflow_vectordb/tool/adapter/adapter_factory.py,sha256=VgjbUI0L0OZLTwuQOzSDQtDq0fVl8Muh7f1FUxzOKdA,1609
@@ -95,44 +95,45 @@
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/__init__.py,sha256=hB9H4VgXSp1dLuMvy1xLYC1WEHzQanwhkYKpuQJS6BE,143
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler.py,sha256=tiZWVt19J58Azkq9D093EJ4zI26Zz0ranOZRfMkhTEo,537
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/connection_handler_factory.py,sha256=J-sP5ZqxDq1020kk0t1eiqhoJKovicGJDoxERQBUrxk,1169
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/env_connection_handler.py,sha256=HXWyQmXfa-pBgZBTcLEH3vIG2FifZEy0b6_oIbYE238,635
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/keyvault_connection_hander.py,sha256=VPRb1TZa5880ShojzepJRHWr_8mMCV7qWED25jKlqBs,1188
 promptflow_vectordb/tool/adapter/ml_index_connection_handlers/workspace_connection_handler.py,sha256=UO5uLeyPMT7HT8RWwwsDbck9nFNe5KQbsw7XG8yit0Y,2515
 promptflow_vectordb/tool/common_index_lookup_extensions/__init__.py,sha256=xhqpwJ_ZB7Lz959ivjcs74tPcbgA4EbSoLLDnPmmpQs,51
-promptflow_vectordb/tool/common_index_lookup_extensions/acs.py,sha256=I3WFXp0NZmqBKCl8gFamg3gOyRFQM4GP-VF9qUIdLtU,4241
-promptflow_vectordb/tool/common_index_lookup_extensions/utils.py,sha256=AaPa0IyEBk6NCZoCETDy67ItxBW-tiGjCYTMzzNStC0,1887
-promptflow_vectordb/tool/common_index_lookup_utils/__init__.py,sha256=6YRE7WUZdJrlk1HuEXpgL0Q4_JyvgI0BQqKWw-FfHg4,613
+promptflow_vectordb/tool/common_index_lookup_extensions/acs.py,sha256=h5CV4snde425ZZIaSslJofBPSfpnhnf4tVL3YicyuIE,4348
+promptflow_vectordb/tool/common_index_lookup_extensions/utils.py,sha256=MJ5GO-pnxB_GVWQfqaVJdLnewA5x_idGtPipq7C8cgA,2417
+promptflow_vectordb/tool/common_index_lookup_utils/__init__.py,sha256=IbjeUTAy8-RXws_6EJfON6iu4us6nX4knubh22XRUBQ,656
 promptflow_vectordb/tool/common_index_lookup_utils/acs.py,sha256=2xPq_okL9L7M249G0OyNz57gqIWE_DhYSHSWuoIZjIQ,4040
-promptflow_vectordb/tool/common_index_lookup_utils/constants.py,sha256=FJxoZ9YHJn-LIl7dC7rdEsVd1IPChnQG7QWqgjMSs2s,533
-promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py,sha256=8q3JHnd8tf2Wu-iSsJ6KpgOdGjf3BL1FtwrxVsIQy80,4124
+promptflow_vectordb/tool/common_index_lookup_utils/constants.py,sha256=klRhZNzHq_1TT1ZOg4FLoyFesuD27Mo_Z-tyP17aQjM,911
+promptflow_vectordb/tool/common_index_lookup_utils/embeddings.py,sha256=wjcW5elRF3AfwVyiUCstYVDgWnF1HRRK-wuDfmrosZI,6088
 promptflow_vectordb/tool/common_index_lookup_utils/index_types.py,sha256=IcBuYzA6A0bXlOOAyhdSpmAgUH5ZxBM6smd1JowdKMw,1819
 promptflow_vectordb/tool/common_index_lookup_utils/indices.py,sha256=cQwtBGCTUjDkF8DiuQayw8SpDL9HwiQ3LD2U1Gm6hjA,478
-promptflow_vectordb/tool/common_index_lookup_utils/mapping.py,sha256=rkWDEdD3bEkHP7RbJLa24GkqMNaB72wuczYnU66A-8I,12709
+promptflow_vectordb/tool/common_index_lookup_utils/logger.py,sha256=7r-n2cU2b5UIfTK4pqadnevGsBakTyDqg64RGZydJSA,1162
+promptflow_vectordb/tool/common_index_lookup_utils/mapping.py,sha256=wEVgv0QtTgCMA8hOni3LsF5iGZls4SzpI7J3Wzviffw,13580
 promptflow_vectordb/tool/common_index_lookup_utils/mlindex_client.py,sha256=pO9-S1z8Jq-7rxeW8JnOpkJ9dv_Ya2Zk29PlCaXdjnA,2005
 promptflow_vectordb/tool/common_index_lookup_utils/pinecone.py,sha256=0qkcSctepwqwbaR_CRQPYLxZ_WJPLn9mVrRvqG30hvk,1937
 promptflow_vectordb/tool/common_index_lookup_utils/query_types.py,sha256=RodyiPIkup5Yg1NVu6RG4Q3jevytkJz3IEjCk2pFh3w,1814
-promptflow_vectordb/tool/common_index_lookup_utils/utils.py,sha256=EgOnCXJ_0A_OdQRuzdW44ds4fLgDf8NsK1ZyQMzYnZI,2379
+promptflow_vectordb/tool/common_index_lookup_utils/utils.py,sha256=en77dbsII8K9THtWysQ-wu2UKCP8Cpd1qb0PVLb45_g,2184
 promptflow_vectordb/tool/contracts/__init__.py,sha256=w2wEJZosUreNBtCotdkW9ZsBQVI-GmbWqpzjQGoeS_U,89
 promptflow_vectordb/tool/contracts/config.py,sha256=1d3wN20-uiMRoZ_xwf428cD9S4-ffS00__3VD7bQ75Q,5050
 promptflow_vectordb/tool/contracts/constants.py,sha256=CjBL2-ra0LzzXQY09wjl5TvDG5C3d99MLkUPXKPlaHA,230
 promptflow_vectordb/tool/contracts/ml_index_yaml_config.py,sha256=W0CJN4ybNT8d5MihSClzxCr6Fe7A06702_NqFF3Ppzs,1512
 promptflow_vectordb/tool/contracts/telemetry.py,sha256=bmmaatq2s6GE5EoYdJZw9szHnMuMLLZg-v1zm-9s6UA,899
 promptflow_vectordb/tool/contracts/types.py,sha256=btKXaCm93vM0fy1VyG8bkuN6lNG_3U3LaqG7-brpNjY,942
 promptflow_vectordb/tool/contracts/ui_config.py,sha256=YihINPWcQpgqXMiVgQk_CevzpqzpYCCKp9FR73MG-Qo,322
 promptflow_vectordb/tool/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow_vectordb/tool/utils/logging.py,sha256=HGBxmKzEng5TtE9qjWcCezZr4WTRdfGh3lbkybVpqRo,1539
 promptflow_vectordb/tool/utils/pf_exception_helpers.py,sha256=s5GGRV3ic-KhP5LIn5xAetfsiuvCYfFcrpeaxdGB1XA,3616
 promptflow_vectordb/tool/utils/pf_runtime_utils.py,sha256=r9o1Aw5nY0GHEkmRVvwwWOBTknIABqUCe34UFvHxd-c,3372
-promptflow_vectordb/tool/utils/profiling.py,sha256=GJfvwi8HVmM89Y0tfgQHReCyiZr3fJN4U2ZdxBrJ2Co,497
+promptflow_vectordb/tool/utils/profiling.py,sha256=3QU7Jy5-U_LxZyy58OeVBvkKvMY464L9lnnYPAZV4F4,747
 promptflow_vectordb/tool/utils/store_core_provider.py,sha256=Iz9k8cxja2cjAGgf6CKBq9F_wh4FfN_vxtVmkZzCDxM,1944
 promptflow_vectordb/tool/utils/workspace_connection_manager.py,sha256=mIYvNUqy5VunR20j0I8g7B2hej1X8q7lkTQIcpix-Wk,2549
 promptflow_vectordb/tool/utils/yaml_parser.py,sha256=Mw76QJV7fOCJmyw6JJkHZO4Fg3rSxWH129JhpAlWFIs,889
-promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml,sha256=_JGjIK2eTP3kCMt6rxI29Vp2F9Mgx0_4fvRQGdzS56Y,11513
+promptflow_vectordb/tool/yamls/azure/common_index_lookup.yaml,sha256=ka_GzQjUjhG6SE_0W02fVpRe-5UMalPpaG3name-FP0,12054
 promptflow_vectordb/tool/yamls/azure/vector_index_lookup.yaml,sha256=Ps4XNBDz17ZNAl4Lg8huFCNnGMfH3Z_0PtfyhFItQT4,457
 promptflow_vectordb/tool/yamls/shared/faiss_index_lookup.yaml,sha256=A3FcLLu0XxQkLywq4A8ijCBo6tqSbdgt6dWwNemWoAg,443
 promptflow_vectordb/tool/yamls/shared/vector_db_lookup.yaml,sha256=grYJamNVbr5pAZePdfXJENPv1UMxnTnWI2gHt_e6phs,1507
-promptflow_vectordb-0.2.6.dist-info/METADATA,sha256=il5N1GpCwwtE7_t180-RdaChAWaQU0888hmiWIqnqMI,2953
-promptflow_vectordb-0.2.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-promptflow_vectordb-0.2.6.dist-info/entry_points.txt,sha256=U2bURx76LNRyrBkb-gksXN8hbaH1D4sMtrxcu8nzmDI,200
-promptflow_vectordb-0.2.6.dist-info/top_level.txt,sha256=AIbxh30bIFT76vitS0NSe96iRftM0tuVOo_HrZxRedw,20
-promptflow_vectordb-0.2.6.dist-info/RECORD,,
+promptflow_vectordb-0.2.7.dist-info/METADATA,sha256=rBLxiJNfKJD6xx3VasQtrkk7MIst1BtYzNeDkNTmW1E,3224
+promptflow_vectordb-0.2.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+promptflow_vectordb-0.2.7.dist-info/entry_points.txt,sha256=U2bURx76LNRyrBkb-gksXN8hbaH1D4sMtrxcu8nzmDI,200
+promptflow_vectordb-0.2.7.dist-info/top_level.txt,sha256=AIbxh30bIFT76vitS0NSe96iRftM0tuVOo_HrZxRedw,20
+promptflow_vectordb-0.2.7.dist-info/RECORD,,
```

