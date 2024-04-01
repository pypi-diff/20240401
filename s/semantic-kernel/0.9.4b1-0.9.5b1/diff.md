# Comparing `tmp/semantic_kernel-0.9.4b1.tar.gz` & `tmp/semantic_kernel-0.9.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.9.4b1.tar", max compression
+gzip compressed data, was "semantic_kernel-0.9.5b1.tar", max compression
```

## Comparing `semantic_kernel-0.9.4b1.tar` & `semantic_kernel-0.9.5b1.tar`

### file list

```diff
@@ -1,217 +1,227 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/pip/README.md
--rw-r--r--   0        0        0     5328 2024-03-20 18:24:28.753758 semantic_kernel-0.9.4b1/pyproject.toml
--rw-r--r--   0        0        0     1663 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      599 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3558 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      417 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1746 2024-03-13 15:37:17.045380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10227 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     3822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     2229 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1122 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6673 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2094 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8344 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3968 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1804 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     1433 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/__init__.py
--rw-r--r--   0        0        0     1340 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/azure_chat_message_content.py
--rw-r--r--   0        0        0     4221 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/azure_streaming_chat_message_content.py
--rw-r--r--   0        0        0     1992 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
--rw-r--r--   0        0        0     3380 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_chat_message_content.py
--rw-r--r--   0        0        0     6146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_streaming_chat_message_content.py
--rw-r--r--   0        0        0      844 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/tool_calls.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     2894 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     3972 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    15271 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    18940 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6244 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0      820 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py
--rw-r--r--   0        0        0     6987 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/utils.py
--rw-r--r--   0        0        0     3653 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1652 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6364 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0     9405 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      937 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0     7409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14863 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      132 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/openapi/__init__.py
--rw-r--r--   0        0        0    11461 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/openapi/kernel_openapi.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      689 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0    11449 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0     2744 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      211 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/chat_role.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0      515 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0     4751 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      732 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/streaming_kernel_content.py
--rw-r--r--   0        0        0     2681 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     1138 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      747 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3492 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4084 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2489 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     3495 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2673 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1804 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/events/__init__.py
--rw-r--r--   0        0        0     2068 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/events/function_invoked_event_args.py
--rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/events/function_invoking_event_args.py
--rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/events/kernel_events_args.py
--rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1201 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0      879 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2445 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1557 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0     8847 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     5065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     7582 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    14034 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1877 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0      541 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0     4471 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0     8397 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_plugin_collection.py
--rw-r--r--   0        0        0      769 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0    40620 2024-03-20 18:24:28.763758 semantic_kernel-0.9.4b1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      160 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6221 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3548 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     1181 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      126 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/action_planner/__init__.py
--rw-r--r--   0        0        0    11319 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/action_planner/action_planner.py
--rw-r--r--   0        0        0      392 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/action_planner/action_planner_config.py
--rw-r--r--   0        0        0      409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/action_planner/skprompt.txt
--rw-r--r--   0        0        0     8189 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/basic_planner.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0     9875 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      886 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2778 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      622 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5939 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4737 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4979 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      881 2024-03-13 15:37:17.055380 semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json
--rw-r--r--   0        0        0     2847 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
--rw-r--r--   0        0        0      243 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/__init__.py
--rw-r--r--   0        0        0    16293 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py
--rw-r--r--   0        0        0      982 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py
--rw-r--r--   0        0        0      371 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/system_step.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      434 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4134 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4676 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     7931 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     4772 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4303 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     3997 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2168 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     8379 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     9641 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.4b1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5205 1970-01-01 00:00:00.000000 semantic_kernel-0.9.4b1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.5b1/pip/README.md
+-rw-r--r--   0        0        0     5363 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/pyproject.toml
+-rw-r--r--   0        0        0     1663 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      599 2024-03-13 15:37:17.045380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3534 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      417 2024-03-13 15:37:17.045380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1746 2024-03-13 15:37:17.045380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0    10227 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     3822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     2229 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1122 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6673 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2094 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8390 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3968 2024-03-20 18:24:28.763758 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1804 2024-03-20 18:24:28.763758 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     1433 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/__init__.py
+-rw-r--r--   0        0        0     1510 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/azure_chat_message_content.py
+-rw-r--r--   0        0        0     4442 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/azure_streaming_chat_message_content.py
+-rw-r--r--   0        0        0     1992 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
+-rw-r--r--   0        0        0     2770 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_chat_message_content.py
+-rw-r--r--   0        0        0     4256 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_streaming_chat_message_content.py
+-rw-r--r--   0        0        0      844 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/tool_calls.py
+-rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     2894 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     3972 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    15466 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     8276 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     4815 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4731 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    18930 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     4797 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6244 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3016 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0      820 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py
+-rw-r--r--   0        0        0     6987 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/utils.py
+-rw-r--r--   0        0        0     3653 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1652 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6364 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    11819 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      242 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15787 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      213 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0     9405 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      937 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0     7409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      159 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    12786 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14863 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20518 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15281 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      188 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    11001 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      496 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0      965 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      336 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    13809 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2648 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.5b1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      574 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0    12112 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0     3360 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0     3278 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/chat_message_content_base.py
+-rw-r--r--   0        0        0      211 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/contents/chat_role.py
+-rw-r--r--   0        0        0      600 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0      515 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0     3326 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      564 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2602 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     1144 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      747 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3492 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     4084 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2489 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     3495 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2673 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8045 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1178 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1804 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/events/__init__.py
+-rw-r--r--   0        0        0     2068 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/events/function_invoked_event_args.py
+-rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/events/function_invoking_event_args.py
+-rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/events/kernel_events_args.py
+-rw-r--r--   0        0        0      537 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0      879 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2445 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1557 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0     8851 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     5065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0     7579 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    14009 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1877 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0      541 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0     4471 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0     8397 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_plugin_collection.py
+-rw-r--r--   0        0        0      769 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0    46851 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      160 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6273 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3548 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     1181 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/action_planner/__init__.py
+-rw-r--r--   0        0        0    11390 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/planners/action_planner/action_planner.py
+-rw-r--r--   0        0        0      392 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/action_planner/action_planner_config.py
+-rw-r--r--   0        0        0      409 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/action_planner/skprompt.txt
+-rw-r--r--   0        0        0     8189 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/basic_planner.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    10443 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1676 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      886 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2778 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      622 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5939 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4737 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4979 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      881 2024-03-13 15:37:17.055380 semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json
+-rw-r--r--   0        0        0     2847 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt
+-rw-r--r--   0        0        0      243 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    16293 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py
+-rw-r--r--   0        0        0      982 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py
+-rw-r--r--   0        0        0      371 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/system_step.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      644 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4134 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      340 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4676 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     7931 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0      623 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     4762 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4521 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2412 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     1701 2024-03-15 14:30:59.091994 semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2285 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     8379 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0    11120 2024-04-01 16:45:47.997053 semantic_kernel-0.9.5b1/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.5b1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 semantic_kernel-0.9.5b1/PKG-INFO
```

### Comparing `semantic_kernel-0.9.4b1/pip/README.md` & `semantic_kernel-0.9.5b1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/pyproject.toml` & `semantic_kernel-0.9.5b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.9.4b1"
+version = "0.9.5b1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
@@ -30,15 +30,15 @@
 prance = "^23.6.21.0"
 pydantic = "^2"
 motor = "^3.3.2"
 defusedxml = "^0.7.1"
 pybars4 = "^0.9.13"
 jinja2 = "^3.1.3"
 nest-asyncio = "^1.6.0"
-eval_type_backport = { version = "^0.1.3", markers = "python_version < '3.9'" }
+eval_type_backport = { version = "^0.1.3", markers = "python_version < '3.10'" }
 
 # Optional dependencies
 ipykernel = { version = "^6.21.1", optional = true}
 google-generativeai = { version = ">=0.1", markers = "python_version >= '3.9'", optional = true}
 grpcio-status = { version = "^1.53.0", markers = "python_version >= '3.9'", optional = true}
 transformers = { version = "^4.28.1", optional = true}
 sentence-transformers = { version = "^2.2.2", optional = true}
@@ -73,14 +73,15 @@
 ruff = "^0.3.2"
 ipykernel = "^6.29.3"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.5.post1"
 snoop = "^0.4.3"
 pytest-cov = ">=4.1.0"
 mypy = ">=1.9.0"
+types-PyYAML = "^6.0.12.20240311"
 
 [tool.poetry.group.unit-tests]
 optional = true
 
 [tool.poetry.group.unit-tests.dependencies]
 google-generativeai = { version = ">=0.1,<0.4", markers = "python_version >= '3.9'"}
 azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional, Type
+from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional
 
 from semantic_kernel.contents import ChatMessageContent
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
     from semantic_kernel.contents import StreamingChatMessageContent
     from semantic_kernel.contents.chat_history import ChatHistory
 
 
 class ChatCompletionClientBase(AIServiceClientBase, ABC):
-    def get_chat_message_content_class(self) -> Type[ChatMessageContent]:
-        """Get the chat message content types used by a class, default is ChatMessageContent."""
-        return ChatMessageContent
+    def get_chat_message_content_type(self) -> str:
+        """Get the chat message content types used by a class, default is 'ChatMessageContent'."""
+        return "ChatMessageContent"
 
     @abstractmethod
     async def complete_chat(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                         break
                     yield [
                         StreamingChatMessageContent(
                             choice_index=0,
                             inner_content=body,
                             ai_model_id=self.ai_model_id,
                             content=body.get("message", {"content": None}).get("content", None),
+                            role="assistant",
                         )
                     ]
                     if body.get("done"):
                         break
 
     async def complete(
         self,
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/azure_chat_message_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/azure_chat_message_content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
-from typing import Optional
+from typing import Literal, Optional
 
 from semantic_kernel.connectors.ai.open_ai.contents.open_ai_chat_message_content import OpenAIChatMessageContent
+from semantic_kernel.contents.const import AZURE_CHAT_MESSAGE_CONTENT
 
 
 class AzureChatMessageContent(OpenAIChatMessageContent):
     """This is the class for Azure OpenAI chat message response content.
 
     Args:
         inner_content: ChatCompletion - The inner content of the response,
@@ -20,8 +21,9 @@
         tool_calls: Optional[List[ToolCall]] - The tool calls that were generated by this response.
         tool_message: Optional[str] - The content of the tool message generated by the extensions API.
 
     Methods:
         __str__: Returns the content of the response.
     """
 
+    type: Literal[AZURE_CHAT_MESSAGE_CONTENT] = AZURE_CHAT_MESSAGE_CONTENT  # type: ignore
     tool_message: Optional[str] = None
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/azure_streaming_chat_message_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_streaming_chat_message_content.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
-from typing import Optional
 
-from semantic_kernel.connectors.ai.open_ai.contents.open_ai_streaming_chat_message_content import (
-    OpenAIStreamingChatMessageContent,
-)
+from typing import Any
+
+from semantic_kernel.connectors.ai.open_ai.contents.open_ai_chat_message_content import OpenAIChatMessageContent
+from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.exceptions import ContentAdditionException
 
 
-class AzureStreamingChatMessageContent(OpenAIStreamingChatMessageContent):
-    """This is the class for Azure OpenAI streaming chat message response content.
+class OpenAIStreamingChatMessageContent(StreamingContentMixin, OpenAIChatMessageContent):
+    """This is the class for OpenAI streaming chat message response content.
 
     The end-user will have to either do something directly or gather them and combine them into a
     new instance.
 
     Args:
         choice_index: int - The index of the choice that generated this response.
         inner_content: ChatCompletionChunk - The inner content of the response,
@@ -21,31 +21,33 @@
         ai_model_id: Optional[str] - The id of the AI model that generated this response.
         metadata: Dict[str, Any] - Any metadata that should be attached to the response.
         role: Optional[ChatRole] - The role of the chat message, defaults to ASSISTANT.
         content: Optional[str] - The text of the response.
         encoding: Optional[str] - The encoding of the text.
         function_call: Optional[FunctionCall] - The function call that was generated by this response.
         tool_calls: Optional[List[ToolCall]] - The tool calls that were generated by this response.
-        tool_message: Optional[str] - The content of the tool message generated by the extensions API.
 
     Methods:
         __str__: Returns the content of the response.
         __bytes__: Returns the content of the response encoded in the encoding.
         __add__: Combines two StreamingChatMessageContent instances.
     """
 
-    tool_message: Optional[str] = None
+    def __bytes__(self) -> bytes:
+        return self.content.encode(self.encoding if self.encoding else "utf-8") if self.content else b""
 
-    def __add__(self, other: "AzureStreamingChatMessageContent") -> "AzureStreamingChatMessageContent":
-        """When combining two AzureOpenAIStreamingChatMessageContent instances,
+    def __add__(self, other: Any) -> "OpenAIStreamingChatMessageContent":
+        """When combining two OpenAIStreamingChatMessageContent instances,
         the content fields are combined, as well as the arguments of the function or tool calls.
 
         The inner_content of the first one is used, ai_model_id and encoding should be the same,
         if role is set, they should be the same.
         """
+        if not isinstance(other, OpenAIStreamingChatMessageContent):
+            return self
         if self.choice_index != other.choice_index:
             raise ContentAdditionException("Cannot add StreamingChatMessageContent with different choice_index")
         if self.ai_model_id != other.ai_model_id:
             raise ContentAdditionException("Cannot add StreamingChatMessageContent from different ai_model_id")
         if self.encoding != other.encoding:
             raise ContentAdditionException("Cannot add StreamingChatMessageContent with different encoding")
         if self.role and other.role and self.role != other.role:
@@ -61,21 +63,20 @@
                         tc[last_tc_id] += new_tool
                     else:
                         tc[new_tool.id] = new_tool
         elif other.tool_calls:
             tc = {t.id: t for t in other.tool_calls}
         tc_list = list(tc.values())
 
-        return AzureStreamingChatMessageContent(
+        return OpenAIStreamingChatMessageContent(
             choice_index=self.choice_index,
             inner_content=self.inner_content,
             ai_model_id=self.ai_model_id,
             metadata=self.metadata,
             role=self.role,
             content=(self.content or "") + (other.content or ""),
             encoding=self.encoding,
             finish_reason=self.finish_reason or other.finish_reason,
             function_call=fc,
             tool_calls=tc_list,
             tool_call_id=self.tool_call_id or other.tool_call_id,
-            tool_message=(self.tool_message or "") + (other.tool_message or ""),
         )
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_chat_message_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_chat_message_content.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
-from typing import List, Optional
-from xml.etree.ElementTree import Element
+from typing import Any, List, Literal, Optional
 
-from openai.types.chat import ChatCompletion
+from pydantic import field_validator
 
 from semantic_kernel.connectors.ai.open_ai.contents.function_call import FunctionCall
 from semantic_kernel.connectors.ai.open_ai.contents.tool_calls import ToolCall
 from semantic_kernel.contents import ChatMessageContent
-from semantic_kernel.contents.chat_role import ChatRole
+from semantic_kernel.contents.const import OPENAI_CHAT_MESSAGE_CONTENT
 
 
 class OpenAIChatMessageContent(ChatMessageContent):
     """This is the class for OpenAI chat message response content.
 
     Args:
         inner_content: ChatCompletion - The inner content of the response,
@@ -25,53 +24,38 @@
         function_call: Optional[FunctionCall] - The function call that was generated by this response.
         tool_calls: Optional[List[ToolCall]] - The tool calls that were generated by this response.
 
     Methods:
         __str__: Returns the content of the response.
     """
 
-    inner_content: Optional[ChatCompletion] = None
+    type: Literal[OPENAI_CHAT_MESSAGE_CONTENT] = OPENAI_CHAT_MESSAGE_CONTENT  # type: ignore
     function_call: Optional[FunctionCall] = None
     tool_calls: Optional[List[ToolCall]] = None
     tool_call_id: Optional[str] = None
 
+    @field_validator("tool_calls", mode="before")
+    @classmethod
+    def _validate_tool_calls(cls, tool_calls: Any) -> Optional[List[ToolCall]]:
+        if not tool_calls:
+            return None
+        if isinstance(tool_calls, list):
+            for index, call in enumerate(tool_calls):
+                if not isinstance(call, ToolCall):
+                    tool_calls[index] = ToolCall.model_validate_json(call)
+            return tool_calls
+        if isinstance(tool_calls, str):
+            return [ToolCall.model_validate_json(call) for call in tool_calls.split("|")]
+
+    @field_validator("function_call", mode="before")
+    @classmethod
+    def _validate_function_call(cls, function_call: Any) -> Optional[FunctionCall]:
+        if not function_call:
+            return None
+        if isinstance(function_call, FunctionCall):
+            return function_call
+        return FunctionCall.model_validate_json(function_call)
+
     @staticmethod
     def ToolIdProperty():
         # Directly using the class name and the attribute name as strings
         return f"{ToolCall.__name__}.{ToolCall.id.__name__}"
-
-    def to_element(self, root_key: str) -> Element:
-        """Convert the OpenAIChatMessageContent to a prompt.
-
-        Returns:
-            str - The prompt from the ChatMessageContent.
-        """
-
-        root = Element(root_key)
-        root.set("role", self.role.value)
-        if self.function_call:
-            root.set("function_call", self.function_call.model_dump_json(exclude_none=True))
-        if self.tool_calls:
-            root.set("tool_calls", "|".join([call.model_dump_json(exclude_none=True) for call in self.tool_calls]))
-        if self.tool_call_id:
-            root.set("tool_call_id", self.tool_call_id)
-        root.text = self.content or ""
-        return root
-
-    @classmethod
-    def from_element(cls, element: Element) -> "ChatMessageContent":
-        """Create a new instance of OpenAIChatMessageContent from a prompt.
-
-        Args:
-            prompt: str - The prompt to create the ChatMessageContent from.
-
-        Returns:
-            ChatMessageContent - The new instance of ChatMessageContent.
-        """
-        args = {"role": element.get("role", ChatRole.USER.value), "content": element.text}
-        if function_call := element.get("function_call"):
-            args["function_call"] = FunctionCall.model_validate_json(function_call)
-        if tool_calls := element.get("tool_calls"):
-            args["tool_calls"] = [ToolCall.model_validate_json(call) for call in tool_calls.split("|")]
-        if tool_call_id := element.get("tool_call_id"):
-            args["tool_call_id"] = tool_call_id
-        return cls(**args)
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/open_ai_streaming_chat_message_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/azure_streaming_chat_message_content.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
-from typing import List, Optional
-from xml.etree.ElementTree import Element
+from typing import Any
 
-from defusedxml import ElementTree
-from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
-
-from semantic_kernel.connectors.ai.open_ai.contents.function_call import FunctionCall
-from semantic_kernel.connectors.ai.open_ai.contents.tool_calls import ToolCall
-from semantic_kernel.contents import StreamingChatMessageContent
-from semantic_kernel.contents.chat_role import ChatRole
+from semantic_kernel.connectors.ai.open_ai.contents.azure_chat_message_content import AzureChatMessageContent
+from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.exceptions import ContentAdditionException
 
 
-class OpenAIStreamingChatMessageContent(StreamingChatMessageContent):
-    """This is the class for OpenAI streaming chat message response content.
+class AzureStreamingChatMessageContent(StreamingContentMixin, AzureChatMessageContent):
+    """This is the class for Azure OpenAI streaming chat message response content.
 
     The end-user will have to either do something directly or gather them and combine them into a
     new instance.
 
     Args:
         choice_index: int - The index of the choice that generated this response.
         inner_content: ChatCompletionChunk - The inner content of the response,
@@ -26,33 +20,34 @@
         ai_model_id: Optional[str] - The id of the AI model that generated this response.
         metadata: Dict[str, Any] - Any metadata that should be attached to the response.
         role: Optional[ChatRole] - The role of the chat message, defaults to ASSISTANT.
         content: Optional[str] - The text of the response.
         encoding: Optional[str] - The encoding of the text.
         function_call: Optional[FunctionCall] - The function call that was generated by this response.
         tool_calls: Optional[List[ToolCall]] - The tool calls that were generated by this response.
+        tool_message: Optional[str] - The content of the tool message generated by the extensions API.
 
     Methods:
         __str__: Returns the content of the response.
         __bytes__: Returns the content of the response encoded in the encoding.
         __add__: Combines two StreamingChatMessageContent instances.
     """
 
-    inner_content: ChatCompletionChunk
-    function_call: Optional[FunctionCall] = None
-    tool_calls: Optional[List[ToolCall]] = None
-    tool_call_id: Optional[str] = None
+    def __bytes__(self) -> bytes:
+        return self.content.encode(self.encoding if self.encoding else "utf-8") if self.content else b""
 
-    def __add__(self, other: "OpenAIStreamingChatMessageContent") -> "OpenAIStreamingChatMessageContent":
-        """When combining two OpenAIStreamingChatMessageContent instances,
+    def __add__(self, other: Any) -> "AzureStreamingChatMessageContent":
+        """When combining two AzureOpenAIStreamingChatMessageContent instances,
         the content fields are combined, as well as the arguments of the function or tool calls.
 
         The inner_content of the first one is used, ai_model_id and encoding should be the same,
         if role is set, they should be the same.
         """
+        if not isinstance(other, AzureStreamingChatMessageContent):
+            return self
         if self.choice_index != other.choice_index:
             raise ContentAdditionException("Cannot add StreamingChatMessageContent with different choice_index")
         if self.ai_model_id != other.ai_model_id:
             raise ContentAdditionException("Cannot add StreamingChatMessageContent from different ai_model_id")
         if self.encoding != other.encoding:
             raise ContentAdditionException("Cannot add StreamingChatMessageContent with different encoding")
         if self.role and other.role and self.role != other.role:
@@ -68,58 +63,21 @@
                         tc[last_tc_id] += new_tool
                     else:
                         tc[new_tool.id] = new_tool
         elif other.tool_calls:
             tc = {t.id: t for t in other.tool_calls}
         tc_list = list(tc.values())
 
-        return OpenAIStreamingChatMessageContent(
+        return AzureStreamingChatMessageContent(
             choice_index=self.choice_index,
             inner_content=self.inner_content,
             ai_model_id=self.ai_model_id,
             metadata=self.metadata,
             role=self.role,
             content=(self.content or "") + (other.content or ""),
             encoding=self.encoding,
             finish_reason=self.finish_reason or other.finish_reason,
             function_call=fc,
             tool_calls=tc_list,
             tool_call_id=self.tool_call_id or other.tool_call_id,
+            tool_message=(self.tool_message or "") + (other.tool_message or ""),
         )
-
-    def to_prompt(self, root_key: str) -> str:
-        """Convert the OpenAIChatMessageContent to a prompt.
-
-        Returns:
-            str - The prompt from the ChatMessageContent.
-        """
-
-        root = Element(root_key)
-        if self.role:
-            root.set("role", self.role.value)
-        if self.function_call:
-            root.set("function_call", self.function_call.model_dump_json(exclude_none=True))
-        if self.tool_calls:
-            root.set("tool_calls", "|".join([call.model_dump_json(exclude_none=True) for call in self.tool_calls]))
-        if self.tool_call_id:
-            root.set("tool_call_id", self.tool_call_id)
-        root.text = self.content or ""
-        return ElementTree.tostring(root, encoding=self.encoding or "unicode", short_empty_elements=False)
-
-    @classmethod
-    def from_element(cls, element: Element) -> "StreamingChatMessageContent":
-        """Create a new instance of OpenAIChatMessageContent from a prompt.
-
-        Args:
-            prompt: str - The prompt to create the ChatMessageContent from.
-
-        Returns:
-            ChatMessageContent - The new instance of ChatMessageContent.
-        """
-        args = {"role": element.get("role", ChatRole.USER.value), "content": element.text}
-        if function_call := element.get("function_call"):
-            args["function_call"] = FunctionCall.model_validate_json(function_call)
-        if tool_calls := element.get("tool_calls"):
-            args["tool_calls"] = [ToolCall.model_validate_json(call) for call in tool_calls.split("|")]
-        if tool_call_id := element.get("tool_call_id"):
-            args["tool_call_id"] = tool_call_id
-        return cls(**args)
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/contents/tool_calls.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/contents/tool_calls.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         metadata = self._get_metadata_from_chat_choice(choice)
         metadata.update(chunk_metadata)
         return AzureStreamingChatMessageContent(
             choice_index=choice.index,
             inner_content=chunk,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
-            role=ChatRole(choice.delta.role) if choice.delta.role is not None else None,
+            role=ChatRole(choice.delta.role) if choice.delta.role else ChatRole.ASSISTANT,
             content=choice.delta.content,
             finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason is not None else None,
             function_call=self._get_function_call_from_chat_choice(choice),
             tool_calls=self._get_tool_calls_from_chat_choice(choice),
             tool_message=self._get_tool_message_from_chat_choice(choice),
         )
 
@@ -296,7 +296,11 @@
             content = choice.delta
         if content.model_extra is not None and "context" in content.model_extra:
             if "messages" in content.model_extra["context"]:
                 for message in content.model_extra["context"]["messages"]:
                     if "tool" in message["role"]:
                         return message["content"]
         return None
+
+    def get_chat_message_content_type(self) -> str:
+        """Get the chat message content types used by a class, default is 'ChatMessageContent'."""
+        return "AzureChatMessageContent"
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from copy import copy
-from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, AsyncIterable, Dict, List, Optional, Tuple, Union
 
 from openai import AsyncStream
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
@@ -45,17 +45,17 @@
     # most of the methods are overridden from the ChatCompletionClientBase class, otherwise it is mentioned
 
     # override from AIServiceClientBase
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return OpenAIChatPromptExecutionSettings
 
-    def get_chat_message_content_class(self) -> Type[ChatMessageContent]:
-        """Get the chat message content types used by a class, default is ChatMessageContent."""
-        return OpenAIChatMessageContent
+    def get_chat_message_content_type(self) -> str:
+        """Get the chat message content types used by a class, default is 'ChatMessageContent'."""
+        return "OpenAIChatMessageContent"
 
     async def complete_chat(
         self,
         chat_history: ChatHistory,
         settings: OpenAIPromptExecutionSettings,
         **kwargs: Any,
     ) -> List[OpenAIChatMessageContent]:
@@ -237,15 +237,15 @@
         metadata = self._get_metadata_from_chat_choice(choice)
         metadata.update(chunk_metadata)
         return OpenAIStreamingChatMessageContent(
             choice_index=choice.index,
             inner_content=chunk,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
-            role=ChatRole(choice.delta.role) if choice.delta.role else None,
+            role=ChatRole(choice.delta.role) if choice.delta.role else ChatRole.ASSISTANT,
             content=choice.delta.content,
             finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason else None,
             function_call=self._get_function_call_from_chat_choice(choice),
             tool_calls=self._get_tool_calls_from_chat_choice(choice),
         )
 
     def _get_metadata_from_chat_response(self, response: ChatCompletion) -> Dict[str, Any]:
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/services/tool_call_behavior.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/open_ai/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/open_ai/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/openapi/kernel_openapi.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,43 @@
+# Copyright (c) Microsoft. All rights reserved.
+
+from __future__ import annotations
+
 import json
 import logging
 import sys
-from typing import Dict, Mapping, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
-from urllib.parse import urljoin
+from urllib.parse import urljoin, urlparse, urlunparse
 
 import aiohttp
 import requests
 from openapi_core import Spec, unmarshal_request
 from openapi_core.contrib.requests import RequestsOpenAPIRequest
 from openapi_core.exceptions import OpenAPIError
 from prance import ResolvingParser
 
 from semantic_kernel.connectors.ai.open_ai.const import (
     USER_AGENT,
 )
-from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 from semantic_kernel.exceptions import ServiceInvalidRequestError
-from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
-from semantic_kernel.kernel import Kernel
+from semantic_kernel.functions.kernel_plugin import KernelPlugin
+
+if TYPE_CHECKING:
+    from semantic_kernel.connectors.openai_plugin.openai_function_execution_parameters import (
+        OpenAIFunctionExecutionParameters,
+    )
+    from semantic_kernel.connectors.openapi_plugin.openapi_function_execution_parameters import (
+        OpenAPIFunctionExecutionParameters,
+    )
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class PreparedRestApiRequest:
     def __init__(self, method: str, url: str, params=None, headers=None, request_body=None):
         self.method = method
@@ -42,17 +52,16 @@
             f"method={self.method}, "
             f"url={self.url}, "
             f"params={self.params}, "
             f"headers={self.headers}, "
             f"request_body={self.request_body})"
         )
 
-    def validate_request(self, spec: Spec, **kwargs):
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
+    def validate_request(self, spec: Spec):
+        """Validate the request against the OpenAPI spec."""
         request = requests.Request(
             self.method,
             self.url,
             params=self.params,
             headers=self.headers,
             json=self.request_body,
         )
@@ -68,47 +77,66 @@
 class RestApiOperation:
     def __init__(
         self,
         id: str,
         method: str,
         server_url: str,
         path: str,
-        summary: Optional[str] = None,
-        description: Optional[str] = None,
-        params: Optional[Mapping[str, str]] = None,
-        request_body: Optional[Mapping[str, str]] = None,
+        summary: str | None = None,
+        description: str | None = None,
+        params: Mapping[str, str] | None = None,
+        request_body: Mapping[str, str] | None = None,
     ):
         self.id = id
-        self.method = method
+        self.method = method.upper()
         self.server_url = server_url
         self.path = path
         self.summary = summary
         self.description = description
         self.params = params
         self.request_body = request_body
 
-    """
-    Fills in this RestApiOperation's parameters and payload with the provided values
-    :param path_params: A dictionary of path parameters
-    :param query_params: A dictionary of query parameters
-    :param headers: A dictionary of headers
-    :param request_body: The payload of the request
-    :return: A PreparedRestApiRequest object
-    """
+    def url_join(self, base_url, path):
+        """Join a base URL and a path, correcting for any missing slashes."""
+        parsed_base = urlparse(base_url)
+        if not parsed_base.path.endswith("/"):
+            base_path = parsed_base.path + "/"
+        else:
+            base_path = parsed_base.path
+        full_path = urljoin(base_path, path.lstrip("/"))
+        return urlunparse(parsed_base._replace(path=full_path))
 
     def prepare_request(
-        self, path_params=None, query_params=None, headers=None, request_body=None
+        self,
+        path_params: dict[str, Any] | None = None,
+        query_params: dict[str, Any] | None = None,
+        headers: dict[str, Any] | None = None,
+        request_body: Any | None = None,
     ) -> PreparedRestApiRequest:
+        """Prepare the request for this operation.
+
+        Args:
+            path_params: A dictionary of path parameters
+            query_params: A dictionary of query parameters
+            headers: A dictionary of headers
+            request_body: The payload of the request
+
+        Returns:
+            A PreparedRestApiRequest object
+        """
+        from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
+
         path = self.path
         if path_params:
             path = path.format(**path_params)
 
-        url = urljoin(self.server_url, path)
+        url = self.url_join(self.server_url, path)
 
-        processed_query_params, processed_headers = {}, headers
+        processed_query_params = {}
+        processed_headers = headers if headers is not None else {}
         for param in self.params:
             param_name = param["name"]
             param_schema = param["schema"]
             param_default = param_schema.get("default", None)
 
             if param["in"] == "query":
                 if query_params and param_name in query_params:
@@ -121,15 +149,15 @@
                 elif param_default is not None:
                     processed_headers[param_name] = param_default
             elif param["in"] == "path":
                 if not path_params or param_name not in path_params:
                     raise ServiceInvalidRequestError(f"Required path parameter {param_name} not provided")
 
         processed_payload = None
-        if self.request_body:
+        if self.request_body and (self.method == "POST" or self.method == "PUT"):
             if request_body is None and "required" in self.request_body and self.request_body["required"]:
                 raise ServiceInvalidRequestError("Payload is required but was not provided")
             content = self.request_body["content"]
             content_type = list(content.keys())[0]
             processed_headers["Content-Type"] = content_type
             processed_payload = request_body
 
@@ -155,150 +183,189 @@
             f"request_body={self.request_body}, "
             f"summary={self.summary}, "
             f"description={self.description})"
         )
 
 
 class OpenApiParser:
-    def __init__(self, **kwargs):
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
-
     """
+    NOTE: SK Python only supports the OpenAPI Spec >=3.0
+
     Import an OpenAPI file.
+
+    Args:
+        openapi_file: The path to the OpenAPI file which can be local or a URL.
+
+    Returns:
+        The parsed OpenAPI file
+
+
     :param openapi_file: The path to the OpenAPI file which can be local or a URL.
     :return: The parsed OpenAPI file
     """
 
-    def parse(self, openapi_document):
+    def parse(self, openapi_document: str) -> Any | dict[str, Any] | None:
+        """Parse the OpenAPI document."""
         parser = ResolvingParser(openapi_document)
         return parser.specification
 
-    """
-    Creates a RestApiOperation object for each path/method combination
-    :param parsed_document: The parsed OpenAPI document
-    :return: A dictionary of RestApiOperation objects keyed by operationId
-    """
-
-    def create_rest_api_operations(self, parsed_document) -> Dict[str, RestApiOperation]:
+    def create_rest_api_operations(
+        self,
+        parsed_document: Any,
+        execution_settings: "OpenAIFunctionExecutionParameters" | "OpenAPIFunctionExecutionParameters" | None = None,
+    ) -> Dict[str, RestApiOperation]:
+        """Create the REST API Operations from the parsed OpenAPI document.
+
+        Args:
+            parsed_document: The parsed OpenAPI document
+            execution_settings: The execution settings
+
+        Returns:
+            A dictionary of RestApiOperation objects keyed by operationId
+        """
         paths = parsed_document.get("paths", {})
         request_objects = {}
+
+        base_url = "/"
+        servers = parsed_document.get("servers", [])
+        base_url = servers[0].get("url") if servers else "/"
+
+        if execution_settings and execution_settings.server_url_override:
+            base_url = execution_settings.server_url_override
+
         for path, methods in paths.items():
             for method, details in methods.items():
-                server_url = parsed_document.get("servers", [])
-                server_url = server_url[0].get("url") if server_url else "/"
-
                 request_method = method.lower()
 
                 parameters = details.get("parameters", [])
                 operationId = details.get("operationId", path + "_" + request_method)
                 summary = details.get("summary", None)
                 description = details.get("description", None)
 
                 rest_api_operation = RestApiOperation(
                     id=operationId,
                     method=request_method,
-                    server_url=server_url,
+                    server_url=base_url,
                     path=path,
                     params=parameters,
                     request_body=details.get("requestBody", None),
                     summary=summary,
                     description=description,
                 )
 
                 request_objects[operationId] = rest_api_operation
         return request_objects
 
 
 class OpenApiRunner:
+    """The OpenApiRunner that runs the operations defined in the OpenAPI manifest"""
+
     def __init__(
         self,
         parsed_openapi_document: Mapping[str, str],
+        auth_callback: Callable[[Dict[str, str]], Dict[str, str]] | None = None,
     ):
         self.spec = Spec.from_dict(parsed_openapi_document)
+        self.auth_callback = auth_callback
 
     async def run_operation(
         self,
         operation: RestApiOperation,
-        path_params: Optional[Dict[str, str]] = None,
-        query_params: Optional[Dict[str, str]] = None,
-        headers: Optional[Dict[str, str]] = None,
-        request_body: Optional[Union[str, Dict[str, str]]] = None,
+        path_params: Dict[str, str] | None = None,
+        query_params: Dict[str, str] | None = None,
+        headers: Dict[str, str] | None = None,
+        request_body: str | Dict[str, str] | None = None,
     ) -> str:
+        """Runs the operation defined in the OpenAPI manifest"""
+        if headers is None:
+            headers = {}
+
+        if self.auth_callback:
+            headers_update = await self.auth_callback(headers=headers)
+            headers.update(headers_update)
+
         prepared_request = operation.prepare_request(
             path_params=path_params,
             query_params=query_params,
             headers=headers,
             request_body=request_body,
         )
-        is_valid = prepared_request.validate_request(spec=self.spec)
-        if not is_valid:
-            return None
+        # TODO - figure out how to validate a request that has a dynamic API
+        # against a spec that has a template path
 
         async with aiohttp.ClientSession(raise_for_status=True) as session:
             async with session.request(
                 prepared_request.method,
                 prepared_request.url,
                 params=prepared_request.params,
                 headers=prepared_request.headers,
                 json=prepared_request.request_body,
             ) as response:
                 return await response.text()
 
 
-"""
-Registers a plugin with the kernel that can run OpenAPI operations.
-:param kernel: The kernel to register the plugin with
-:param plugin_name: The name of the plugin
-:param openapi_document: The OpenAPI document to register. Can be a filename or URL
-:return: A dictionary of KernelFunctions keyed by operationId
-"""
-
-
-def register_openapi_plugin(
-    kernel: Kernel,
-    plugin_name: str,
-    openapi_document: str,
-) -> Dict[str, KernelFunction]:
-    parser = OpenApiParser()
-    parsed_doc = parser.parse(openapi_document)
-    operations = parser.create_rest_api_operations(parsed_doc)
-    openapi_runner = OpenApiRunner(parsed_openapi_document=parsed_doc)
-
-    plugin = {}
-
-    def create_run_operation_function(runner: OpenApiRunner, operation: RestApiOperation):
-        @kernel_function(
-            description=operation.summary if operation.summary else operation.description,
-            name=operation_id,
-        )
-        async def run_openapi_operation(
-            path_params: Annotated[Optional[Union[Dict, str]], "A dictionary of path parameters"] = None,
-            query_params: Annotated[Optional[Union[Dict, str]], "A dictionary of query parameters"] = None,
-            headers: Annotated[Optional[Union[Dict, str]], "A dictionary of headers"] = None,
-            request_body: Annotated[Optional[Union[Dict, str]], "A dictionary of the request body"] = None,
-        ) -> str:
-            response = await runner.run_operation(
-                operation,
-                path_params=(
-                    json.loads(path_params) if isinstance(path_params, str) else path_params if path_params else None
-                ),
-                query_params=(
-                    json.loads(query_params)
-                    if isinstance(query_params, str)
-                    else query_params if query_params else None
-                ),
-                headers=json.loads(headers) if isinstance(headers, str) else headers if headers else None,
-                request_body=(
-                    json.loads(request_body)
-                    if isinstance(request_body, str)
-                    else request_body if request_body else None
-                ),
+class OpenAPIPlugin:
+    @staticmethod
+    def create(
+        plugin_name: str,
+        openapi_document_path: str,
+        execution_settings: "OpenAIFunctionExecutionParameters" | "OpenAPIFunctionExecutionParameters" | None = None,
+    ) -> KernelPlugin:
+        """Creates an OpenAPI plugin
+
+        Args:
+            plugin_name: The name of the plugin
+            openapi_document_path: The OpenAPI document path, it must be a file path to the spec.
+            execution_settings: The execution settings
+
+        Returns:
+            The KernelPlugin
+        """
+        parser = OpenApiParser()
+        parsed_doc = parser.parse(openapi_document_path)
+        operations = parser.create_rest_api_operations(parsed_doc, execution_settings=execution_settings)
+
+        auth_callback = None
+        if execution_settings and execution_settings.auth_callback:
+            auth_callback = execution_settings.auth_callback
+        openapi_runner = OpenApiRunner(parsed_openapi_document=parsed_doc, auth_callback=auth_callback)
+
+        plugin = {}
+
+        def create_run_operation_function(runner: OpenApiRunner, operation: RestApiOperation):
+            @kernel_function(
+                description=operation.summary if operation.summary else operation.description,
+                name=operation.id,
             )
-            return response
+            async def run_openapi_operation(
+                path_params: Annotated[dict | str | None, "A dictionary of path parameters"] = None,
+                query_params: Annotated[dict | str | None, "A dictionary of query parameters"] = None,
+                headers: Annotated[dict | str | None, "A dictionary of headers"] = None,
+                request_body: Annotated[dict | str | None, "A dictionary of the request body"] = None,
+            ) -> str:
+                response = await runner.run_operation(
+                    operation,
+                    path_params=(
+                        json.loads(path_params)
+                        if isinstance(path_params, str)
+                        else path_params if path_params else None
+                    ),
+                    query_params=(
+                        json.loads(query_params)
+                        if isinstance(query_params, str)
+                        else query_params if query_params else None
+                    ),
+                    headers=json.loads(headers) if isinstance(headers, str) else headers if headers else None,
+                    request_body=(
+                        json.loads(request_body)
+                        if isinstance(request_body, str)
+                        else request_body if request_body else None
+                    ),
+                )
+                return response
 
-        return run_openapi_operation
+            return run_openapi_operation
 
-    for operation_id, operation in operations.items():
-        logger.info(f"Registering OpenAPI operation: {plugin_name}.{operation_id}")
-        plugin[operation_id] = create_run_operation_function(openapi_runner, operation)
-    return kernel.import_plugin_from_object(plugin, plugin_name)
+        for operation_id, operation in operations.items():
+            logger.info(f"Registering OpenAPI operation: {plugin_name}.{operation_id}")
+            plugin[operation_id] = create_run_operation_function(openapi_runner, operation)
+        return plugin
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-0.9.5b1/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.kernel_content import KernelContent
 from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
-from semantic_kernel.contents.streaming_kernel_content import StreamingKernelContent
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 
 __all__ = [
     "ChatMessageContent",
     "KernelContent",
     "TextContent",
-    "StreamingKernelContent",
     "StreamingChatMessageContent",
     "StreamingTextContent",
 ]
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/chat_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 # Copyright (c) Microsoft. All rights reserved.
+from __future__ import annotations
 
 import logging
-from typing import Any, Dict, Final, Iterator, List, Optional, Type, Union
-from xml.etree import ElementTree
-from xml.etree.ElementTree import Element
+from typing import Any, Iterator, List
+from xml.etree.ElementTree import Element, tostring
 
-import defusedxml.ElementTree as ET
+from defusedxml.ElementTree import XML, ParseError
 
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
+from semantic_kernel.contents.chat_message_content_base import ChatMessageContentBase
 from semantic_kernel.contents.chat_role import ChatRole
-from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
+from semantic_kernel.contents.const import (
+    CHAT_MESSAGE_CONTENT,
+    ROOT_KEY_HISTORY,
+    ROOT_KEY_MESSAGE,
+    TYPES_CHAT_MESSAGE_CONTENT,
+)
 from semantic_kernel.exceptions import ContentInitializationError, ContentSerializationError
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 logger = logging.getLogger(__name__)
 
-ROOT_KEY_MESSAGE: Final[str] = "message"
-ROOT_KEY_HISTORY: Final[str] = "chat_history"
-
 
 class ChatHistory(KernelBaseModel):
     """
     This class holds the history of chat messages from a chat conversation.
 
     Note: the constructor takes a system_message parameter, which is not part
     of the class definition. This is to allow the system_message to be passed in
     as a keyword argument, but not be part of the class definition.
 
     Attributes:
         messages (List[ChatMessageContent]): The list of chat messages in the history.
     """
 
-    messages: List[ChatMessageContent]
+    messages: list["ChatMessageContent"]
+    message_type: TYPES_CHAT_MESSAGE_CONTENT = CHAT_MESSAGE_CONTENT
 
     def __init__(self, **data: Any):
         """
         Initializes a new instance of the ChatHistory class, optionally incorporating a message and/or
         a system message at the beginning of the chat history.
 
         This constructor allows for flexible initialization with chat messages and an optional messages or a
@@ -52,75 +56,86 @@
                 included at the start of the chat history.
 
         Note: The 'system_message' is not retained as part of the class's attributes; it's used during
         initialization and then discarded. The rest of the keyword arguments are passed to the superclass
         constructor and handled according to the Pydantic model's behavior.
         """
         system_message_content = data.pop("system_message", None)
+        message_type = data.get("message_type", CHAT_MESSAGE_CONTENT)
 
         if system_message_content:
-            system_message = ChatMessageContent(role=ChatRole.SYSTEM, content=system_message_content)
+            system_message = ChatMessageContentBase.from_fields(
+                role=ChatRole.SYSTEM, content=system_message_content, type=message_type
+            )
 
             if "messages" in data:
                 data["messages"] = [system_message] + data["messages"]
             else:
                 data["messages"] = [system_message]
         if "messages" not in data:
             data["messages"] = []
         super().__init__(**data)
 
-    def add_system_message(self, content: str) -> None:
+    def add_system_message(self, content: str, **kwargs: Any) -> None:
         """Add a system message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.SYSTEM, content))
+        self.add_message(message=self._prepare_for_add(ChatRole.SYSTEM, content, **kwargs))
 
-    def add_user_message(self, content: str) -> None:
+    def add_user_message(self, content: str, **kwargs: Any) -> None:
         """Add a user message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.USER, content))
+        self.add_message(message=self._prepare_for_add(ChatRole.USER, content, **kwargs))
 
-    def add_assistant_message(self, content: str) -> None:
+    def add_assistant_message(self, content: str, **kwargs: Any) -> None:
         """Add an assistant message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.ASSISTANT, content))
+        self.add_message(message=self._prepare_for_add(ChatRole.ASSISTANT, content, **kwargs))
 
-    def add_tool_message(self, content: Optional[str] = None, metadata: Optional[Dict[str, Any]] = None) -> None:
+    def add_tool_message(
+        self, content: str | None = None, metadata: dict[str, Any] | None = None, **kwargs: Any
+    ) -> None:
         """Add a tool message to the chat history."""
-        self.add_message(message=self._prepare_for_add(ChatRole.TOOL, content), metadata=metadata)
+        self.add_message(message=self._prepare_for_add(ChatRole.TOOL, content, **kwargs), metadata=metadata)
 
     def add_message(
         self,
-        message: Union[ChatMessageContent, Dict[str, Any]],
-        encoding: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
+        message: "ChatMessageContent" | dict[str, Any],
+        encoding: str | None = None,
+        metadata: dict[str, Any] | None = None,
     ) -> None:
         """Add a message to the history.
 
         This method accepts either a ChatMessageContent instance or a
         dictionary with the necessary information to construct a ChatMessageContent instance.
 
         Args:
             message (Union[ChatMessageContent, dict]): The message to add, either as
                 a pre-constructed ChatMessageContent instance or a dictionary specifying 'role' and 'content'.
             encoding (Optional[str]): The encoding of the message. Required if 'message' is a dict.
             metadata (Optional[dict[str, Any]]): Any metadata to attach to the message. Required if 'message' is a dict.
         """
-        if isinstance(message, ChatMessageContent) or isinstance(message, StreamingChatMessageContent):
+        from semantic_kernel.contents.chat_message_content import ChatMessageContent
+
+        if isinstance(message, ChatMessageContent):
             self.messages.append(message)
             return
         if "role" not in message:
             raise ContentInitializationError(f"Dictionary must contain at least the role. Got: {message}")
         if encoding:
             message["encoding"] = encoding
         if metadata:
             message["metadata"] = metadata
-        self.messages.append(ChatMessageContent(**message))
+        if "type" not in message:
+            message["type"] = self.message_type
+        self.messages.append(ChatMessageContentBase.from_dict(message))
 
-    def _prepare_for_add(self, role: ChatRole, content: str) -> Dict[str, str]:
+    def _prepare_for_add(self, role: ChatRole, content: str | None = None, **kwargs: Any) -> dict[str, str]:
         """Prepare a message to be added to the history."""
-        return {"role": role, "content": content}
+        kwargs["role"] = role
+        kwargs["content"] = content
+        return kwargs
 
-    def remove_message(self, message: ChatMessageContent) -> bool:
+    def remove_message(self, message: "ChatMessageContent") -> bool:
         """Remove a message from the history.
 
         Args:
             message (ChatMessageContent): The message to remove.
 
         Returns:
             bool: True if the message was removed, False if the message was not found.
@@ -131,26 +146,26 @@
         except ValueError:
             return False
 
     def __len__(self) -> int:
         """Return the number of messages in the history."""
         return len(self.messages)
 
-    def __getitem__(self, index: int) -> ChatMessageContent:
+    def __getitem__(self, index: int) -> "ChatMessageContent":
         """Get a message from the history using the [] operator.
 
         Args:
             index (int): The index of the message to get.
 
         Returns:
             ChatMessageContent: The message at the specified index.
         """
         return self.messages[index]
 
-    def __contains__(self, item: ChatMessageContent) -> bool:
+    def __contains__(self, item: "ChatMessageContent") -> bool:
         """Check if a message is in the history.
 
         Args:
             item (ChatMessageContent): The message to check for.
 
         Returns:
             bool: True if the message is in the history, False otherwise.
@@ -158,73 +173,79 @@
         return item in self.messages
 
     def __str__(self) -> str:
         """Return a string representation of the history."""
         chat_history_xml = Element(ROOT_KEY_HISTORY)
         for message in self.messages:
             chat_history_xml.append(message.to_element(root_key=ROOT_KEY_MESSAGE))
-        return ElementTree.tostring(chat_history_xml, encoding="unicode", short_empty_elements=True)
+        return tostring(chat_history_xml, encoding="unicode", short_empty_elements=True)
 
-    def __iter__(self) -> Iterator[ChatMessageContent]:
+    def __iter__(self) -> Iterator["ChatMessageContent"]:
         """Return an iterator over the messages in the history."""
         return iter(self.messages)
 
     def __eq__(self, other: Any) -> bool:
         """Check if two ChatHistory instances are equal."""
         if not isinstance(other, ChatHistory):
             return False
 
         return self.messages == other.messages
 
     @classmethod
-    def from_rendered_prompt(
-        cls, rendered_prompt: str, chat_message_content_type: Type[ChatMessageContent] = ChatMessageContent
-    ) -> "ChatHistory":
+    def from_rendered_prompt(cls, rendered_prompt: str, message_type: str = CHAT_MESSAGE_CONTENT) -> "ChatHistory":
         """
         Create a ChatHistory instance from a rendered prompt.
 
         Args:
             rendered_prompt (str): The rendered prompt to convert to a ChatHistory instance.
 
         Returns:
             ChatHistory: The ChatHistory instance created from the rendered prompt.
         """
-        messages: List[chat_message_content_type] = []
+        messages: List[ChatMessageContent] = []
         prompt = rendered_prompt.strip()
         try:
-            xml_prompt = ET.fromstring(f"<prompt>{prompt}</prompt>")
-        except ET.ParseError as e:
-            logger.error(f"Error parsing XML of prompt: {e}")
-            return cls(messages=[chat_message_content_type(role=ChatRole.USER, content=prompt)])
+            xml_prompt = XML(text=f"<prompt>{prompt}</prompt>")
+        except ParseError:
+            logger.info(f"Could not parse prompt {prompt} as xml, treating as text")
+            return cls(
+                messages=[ChatMessageContentBase.from_fields(role=ChatRole.USER, content=prompt, type=message_type)]
+            )
         if xml_prompt.text and xml_prompt.text.strip():
-            messages.append(chat_message_content_type(role=ChatRole.SYSTEM, content=xml_prompt.text.strip()))
+            messages.append(
+                ChatMessageContentBase.from_fields(
+                    role=ChatRole.SYSTEM, content=xml_prompt.text.strip(), type=message_type
+                )
+            )
         for item in xml_prompt:
             if item.tag == ROOT_KEY_MESSAGE:
-                messages.append(chat_message_content_type.from_element(item))
+                messages.append(ChatMessageContentBase.from_element(item))
             elif item.tag == ROOT_KEY_HISTORY:
                 for message in item:
-                    messages.append(chat_message_content_type.from_element(message))
+                    messages.append(ChatMessageContentBase.from_element(message))
             if item.tail and item.tail.strip():
-                messages.append(chat_message_content_type(role=ChatRole.USER, content=item.tail.strip()))
+                messages.append(
+                    ChatMessageContentBase.from_fields(role=ChatRole.USER, content=item.tail.strip(), type=message_type)
+                )
         if len(messages) == 1 and messages[0].role == ChatRole.SYSTEM:
             messages[0].role = ChatRole.USER
-        return cls(messages=messages)
+        return cls(messages=messages, message_type=message_type)
 
     def serialize(self) -> str:
         """
         Serializes the ChatHistory instance to a JSON string.
 
         Returns:
             str: A JSON string representation of the ChatHistory instance.
 
         Raises:
             ValueError: If the ChatHistory instance cannot be serialized to JSON.
         """
         try:
-            return self.model_dump_json(indent=4)
+            return self.model_dump_json(indent=4, exclude_none=True)
         except Exception as e:
             raise ContentSerializationError(f"Unable to serialize ChatHistory to JSON: {e}") from e
 
     @classmethod
     def restore_chat_history(cls, chat_history_json: str) -> "ChatHistory":
         """
         Restores a ChatHistory instance from a JSON string.
@@ -246,15 +267,14 @@
             raise ContentInitializationError(f"Invalid JSON format: {e}")
 
     def store_chat_history_to_file(self, file_path: str) -> None:
         """
         Stores the serialized ChatHistory to a file.
 
         Args:
-            chat_history (ChatHistory): The ChatHistory instance to serialize and store.
             file_path (str): The path to the file where the serialized data will be stored.
         """
         json_str = self.serialize()
         with open(file_path, "w") as file:
             file.write(json_str)
 
     @classmethod
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/chat_message_content_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,84 @@
 # Copyright (c) Microsoft. All rights reserved.
-import json
-from typing import Optional
+import sys
+from typing import TYPE_CHECKING, Any, Dict, Final
+
+from semantic_kernel.contents.const import ALL_CHAT_MESSAGE_CONTENTS, CHAT_MESSAGE_CONTENT
+
+if sys.version_info >= (3, 9):
+    from typing import Annotated
+else:
+    from typing_extensions import Annotated
+
 from xml.etree.ElementTree import Element
 
-from defusedxml import ElementTree
+from pydantic import Field, RootModel
 
-from semantic_kernel.contents.chat_role import ChatRole
-from semantic_kernel.contents.kernel_content import KernelContent
+if TYPE_CHECKING:
+    from semantic_kernel.contents.chat_message_content import ChatMessageContent
 
+DISCRIMINATOR_FIELD: Final[str] = "type"
 
-class ChatMessageContent(KernelContent):
-    """This is the base class for chat message response content.
 
-    All Chat Completion Services should return a instance of this class as response.
-    Or they can implement their own subclass of this class and return an instance.
-
-    Args:
-        inner_content: Optional[Any] - The inner content of the response,
-            this should hold all the information from the response so even
-            when not creating a subclass a developer can leverage the full thing.
-        ai_model_id: Optional[str] - The id of the AI model that generated this response.
-        metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-        role: ChatRole - The role of the chat message.
-        content: Optional[str] - The text of the response.
-        encoding: Optional[str] - The encoding of the text.
+class ChatMessageContentBase(RootModel):
+    """Base class for all chat message content types.
 
-    Methods:
-        __str__: Returns the content of the response.
-    """
+    This class is used to dynamically create a certain type of ChatMessageContent, based on the type field.
+    Please use this class always through the classmethods, from_dict, from_fields or from_element.
+    If you don't do that, you need to manually rebuild the model with the model_rebuild method,
+    after importing the ChatMessageContent and all it's subclasses. And you then have to use the root field.
 
-    role: ChatRole
-    content: Optional[str] = None
-    encoding: Optional[str] = None
+    The first two use dictionaries, directly or as kwargs to create the ChatMessageContent,
+    the last one uses an XML Element to create the ChatMessageContent.
+    All these methods then return the root field of the ChatMessageContentBase,
+      which is a instance of ChatMessageContent or the requested subclass.
+    """
 
-    def __str__(self) -> str:
-        return self.content or ""
+    root: Annotated[ALL_CHAT_MESSAGE_CONTENTS, Field(discriminator=DISCRIMINATOR_FIELD)]
 
-    def to_element(self, root_key: str) -> Element:
-        """Convert the ChatMessageContent to an XML Element.
+    @classmethod
+    def from_fields(cls, **kwargs: Any) -> "ChatMessageContent":
+        """Create a new instance of ChatMessageContent from fields.
 
         Args:
-            root_key: str - The key to use for the root of the XML Element.
+            kwargs: Any - The keyword arguments to create the ChatMessageContent with.
 
         Returns:
-            Element - The XML Element representing the ChatMessageContent.
+            ChatMessageContent - The new instance of ChatMessageContent or a subclass.
         """
-        root = Element(root_key)
-        root.set("role", self.role.value)
-        root.text = self.content or ""
-        return root
+        from semantic_kernel.connectors.ai.open_ai.contents import (  # noqa: F401, I001, E501
+            AzureChatMessageContent,
+            OpenAIChatMessageContent,
+        )
+        from semantic_kernel.contents.chat_message_content import ChatMessageContent  # noqa: F401, I001, E501
+
+        cls.model_rebuild()
+        if DISCRIMINATOR_FIELD not in kwargs:
+            kwargs[DISCRIMINATOR_FIELD] = CHAT_MESSAGE_CONTENT
+        return cls(**kwargs).root
 
-    def to_prompt(self, root_key: str) -> str:
-        """Convert the ChatMessageContent to a prompt.
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> "ChatMessageContent":
+        """Create a new instance of ChatMessageContent from a dictionary.
+
+        Args:
+            data: Dict[str, Any] - The dictionary to create the ChatMessageContent from.
 
         Returns:
-            str - The prompt from the ChatMessageContent.
+            ChatMessageContent - The new instance of ChatMessageContent or a subclass.
         """
-
-        root = self.to_element(root_key)
-        return ElementTree.tostring(root, encoding=self.encoding or "unicode", short_empty_elements=False)
+        return cls.from_fields(**data)
 
     @classmethod
     def from_element(cls, element: Element) -> "ChatMessageContent":
-        """Create a new instance of ChatMessageContent from a prompt.
+        """Create a new instance of ChatMessageContent from a XML element.
 
         Args:
-            prompt: str - The prompt to create the ChatMessageContent from.
+            element: Element - The XML Element to create the ChatMessageContent from.
 
         Returns:
-            ChatMessageContent - The new instance of ChatMessageContent.
+            ChatMessageContent - The new instance of ChatMessageContent or a subclass.
         """
-        args = {"role": element.get("role", ChatRole.USER.value), "content": element.text}
-        if metadata := element.get("metadata"):
-            args["metadata"] = json.loads(metadata)
-        return cls(**args)
+        kwargs: Dict[str, Any] = {"content": element.text}
+        for key, value in element.items():
+            kwargs[key] = value
+        return cls.from_fields(**kwargs)
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/kernel_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/streaming_kernel_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
+import sys
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional
 
-from pydantic import Field
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+from typing import Any
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
-class StreamingKernelContent(KernelBaseModel, ABC):
-    """Base class for all streaming kernel contents."""
+class StreamingContentMixin(KernelBaseModel, ABC):
+    """Mixin class for all streaming kernel contents."""
 
     choice_index: int
-    inner_content: Optional[Any] = None
-    ai_model_id: Optional[str] = None
-    metadata: Dict[str, Any] = Field(default_factory=dict)
-
-    @abstractmethod
-    def __str__(self) -> str:
-        pass
 
     @abstractmethod
     def __bytes__(self) -> bytes:
         pass
 
     @abstractmethod
-    def __add__(self, other: "StreamingKernelContent") -> "StreamingKernelContent":
+    def __add__(self, other: Any) -> Self:
         pass
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/streaming_text_content.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
-from typing import Optional
 
-from semantic_kernel.contents.streaming_kernel_content import StreamingKernelContent
+from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
+from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import ContentAdditionException
 
 
-class StreamingTextContent(StreamingKernelContent):
+class StreamingTextContent(StreamingContentMixin, TextContent):
     """This is the base class for streaming text response content.
 
     All Text Completion Services should return a instance of this class as streaming response.
     Or they can implement their own subclass of this class and return an instance.
 
     Args:
         choice_index: int - The index of the choice that generated this response.
@@ -23,20 +23,14 @@
 
     Methods:
         __str__: Returns the text of the response.
         __bytes__: Returns the content of the response encoded in the encoding.
         __add__: Combines two StreamingTextContent instances.
     """
 
-    text: Optional[str] = None
-    encoding: Optional[str] = None
-
-    def __str__(self) -> str:
-        return self.text
-
     def __bytes__(self) -> bytes:
         return self.text.encode(self.encoding if self.encoding else "utf-8") if self.text else b""
 
     def __add__(self, other: "StreamingTextContent") -> "StreamingTextContent":
         """When combining two StreamingTextContent instances, the text fields are combined.
 
         The inner_content of the first one is used, choice_index, ai_model_id and encoding should be the same.
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/contents/text_content.py` & `semantic_kernel-0.9.5b1/semantic_kernel/contents/text_content.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         __str__: Returns the text of the response.
     """
 
     text: Optional[str] = None
     encoding: Optional[str] = None
 
     def __str__(self) -> str:
-        return self.text
+        return self.text or ""
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,19 +205,15 @@
         Example:
              KernelContext["input"] = "3"
              {{time.days_ago $input}} => Sunday, 7 May, 2023
         """
         d = datetime.date.today() - datetime.timedelta(days=int(days))
         return d.strftime("%A, %d %B, %Y")
 
-    @kernel_function(
-        description="""Get the date of the last day matching the supplied week day name in English.
-        Example: Che giorno era 'Martedi' scorso -> dateMatchingLastDayName 'Tuesday' => Tuesday,
-        16 May, 2023"""
-    )
+    @kernel_function(description="""Get the date of the last day matching the supplied week day name in English.""")
     def date_matching_last_day_name(self, day_name: str) -> str:
         """
         Get the date of the last day matching the supplied day name
 
         params:
             day_name: The day name to match with.
         returns:
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/events/function_invoked_event_args.py` & `semantic_kernel-0.9.5b1/semantic_kernel/events/function_invoked_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/events/function_invoking_event_args.py` & `semantic_kernel-0.9.5b1/semantic_kernel/events/function_invoking_event_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/events/kernel_events_args.py` & `semantic_kernel-0.9.5b1/semantic_kernel/events/kernel_events_args.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     pass
 
 
 class KernelPluginNotFoundError(KernelException):
     pass
 
 
+class KernelPluginInvalidConfigurationError(KernelException):
+    pass
+
+
 class KernelFunctionNotFoundError(KernelException):
     pass
 
 
 class KernelFunctionAlreadyExistsError(KernelException):
     pass
 
@@ -37,8 +41,9 @@
 __all__ = [
     "KernelException",
     "KernelFunctionAlreadyExistsError",
     "KernelFunctionNotFoundError",
     "KernelInvokeException",
     "KernelPluginNotFoundError",
     "KernelServiceNotFoundError",
+    "KernelPluginInvalidConfigurationError",
 ]
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/function_result.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/function_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_arguments.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, AsyncIterable, Callable, Dict, List, Optional, Union
 
-from semantic_kernel.contents.streaming_kernel_content import StreamingKernelContent
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import (
     HANDLEBARS_TEMPLATE_FORMAT_NAME,
@@ -18,14 +17,15 @@
 )
 from semantic_kernel.prompt_template.handlebars_prompt_template import HandlebarsPromptTemplate
 from semantic_kernel.prompt_template.jinja2_prompt_template import Jinja2PromptTemplate
 from semantic_kernel.prompt_template.kernel_prompt_template import KernelPromptTemplate
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+    from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
     from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
     from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
     from semantic_kernel.kernel import Kernel
     from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
     from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -193,23 +193,23 @@
             )
 
     @abstractmethod
     async def _invoke_internal_stream(
         self,
         kernel: "Kernel",
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[FunctionResult, List[Union[StreamingKernelContent, Any]]]]:
+    ) -> AsyncIterable[Union[FunctionResult, List[Union["StreamingContentMixin", Any]]]]:
         pass
 
     async def invoke_stream(
         self,
         kernel: "Kernel",
         arguments: Optional[KernelArguments] = None,
         **kwargs: Any,
-    ) -> AsyncIterable[Union[FunctionResult, List[Union[StreamingKernelContent, Any]]]]:
+    ) -> AsyncIterable[Union[FunctionResult, List[Union["StreamingContentMixin", Any]]]]:
         """
         Invoke a stream async function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
             kwargs (Any): Additional keyword arguments that will be
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from inspect import isasyncgen, isasyncgenfunction, isawaitable, iscoroutinefunction, isgenerator, isgeneratorfunction
 from typing import TYPE_CHECKING, Any, AsyncIterable, Callable, Dict, List, Optional, Union
 
 from pydantic import ValidationError
 
-from semantic_kernel.contents.streaming_kernel_content import StreamingKernelContent
+from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 
@@ -110,15 +110,15 @@
             metadata={"arguments": arguments, "used_arguments": function_arguments},
         )
 
     async def _invoke_internal_stream(
         self,
         kernel: "Kernel",
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[List[StreamingKernelContent], Any]]:
+    ) -> AsyncIterable[Union[List[StreamingContentMixin], Any]]:
         if self.stream_method is None:
             raise NotImplementedError("Stream method not implemented")
         function_arguments = self.gather_function_parameters(kernel, arguments)
         if isasyncgenfunction(self.stream_method):
             async for partial_result in self.stream_method(**function_arguments):
                 yield partial_result
         elif isgeneratorfunction(self.stream_method):
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
-from semantic_kernel.contents.streaming_kernel_content import StreamingKernelContent
+from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import TEMPLATE_FORMAT_MAP, KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
@@ -169,15 +169,15 @@
         kernel: "Kernel",
         service: ChatCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
         arguments: KernelArguments,
     ) -> FunctionResult:
         """Handles the chat service call."""
-        chat_history = ChatHistory.from_rendered_prompt(prompt, service.get_chat_message_content_class())
+        chat_history = ChatHistory.from_rendered_prompt(prompt, service.get_chat_message_content_type())
 
         # pass the kernel in for auto function calling
         kwargs = {}
         if isinstance(execution_settings, OpenAIChatPromptExecutionSettings) and isinstance(
             service, ChatCompletionClientBase
         ):
             kwargs["kernel"] = kernel
@@ -232,15 +232,15 @@
             metadata=metadata,
         )
 
     async def _invoke_internal_stream(
         self,
         kernel: "Kernel",
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[FunctionResult, List[StreamingKernelContent]]]:
+    ) -> AsyncIterable[Union[FunctionResult, List[StreamingContentMixin]]]:
         """Invokes the function stream with the given arguments."""
         arguments = self.add_default_values(arguments)
         service, execution_settings = kernel.select_ai_service(self, arguments)
         prompt = await self.prompt_template.render(kernel, arguments)
 
         if isinstance(service, ChatCompletionClientBase):
             async for content in self._handle_complete_chat_stream(
@@ -267,26 +267,28 @@
     async def _handle_complete_chat_stream(
         self,
         kernel: "Kernel",
         service: ChatCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
         arguments: KernelArguments,
-    ) -> AsyncIterable[Union[FunctionResult, List[StreamingKernelContent]]]:
+    ) -> AsyncIterable[Union[FunctionResult, List[StreamingContentMixin]]]:
         """Handles the chat service call."""
 
         # pass the kernel in for auto function calling
         kwargs = {}
         if isinstance(execution_settings, OpenAIChatPromptExecutionSettings) and isinstance(
             service, ChatCompletionClientBase
         ):
             kwargs["kernel"] = kernel
             kwargs["arguments"] = arguments
 
-        chat_history = ChatHistory.from_rendered_prompt(prompt, service.get_chat_message_content_class())
+        chat_history = ChatHistory.from_rendered_prompt(
+            prompt,
+        )
         try:
             async for partial_content in service.complete_chat_stream(
                 chat_history=chat_history,
                 settings=execution_settings,
                 **kwargs,
             ):
                 yield partial_content
@@ -297,15 +299,15 @@
             yield FunctionResult(function=self.metadata, value=None, metadata={"exception": e})
 
     async def _handle_complete_text_stream(
         self,
         service: TextCompletionClientBase,
         execution_settings: PromptExecutionSettings,
         prompt: str,
-    ) -> AsyncIterable[Union[FunctionResult, List[StreamingKernelContent]]]:
+    ) -> AsyncIterable[Union[FunctionResult, List[StreamingContentMixin]]]:
         """Handles the text service call."""
         try:
             async for partial_content in service.complete_stream(prompt=prompt, settings=execution_settings):
                 yield partial_content
             return
         except Exception as e:
             logger.error(f"Error occurred while invoking function {self.name}: {e}")
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_parameter_metadata.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/kernel_plugin_collection.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/kernel_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-0.9.5b1/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/kernel.py` & `semantic_kernel-0.9.5b1/semantic_kernel/kernel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import glob
 import importlib
 import inspect
+import json
 import logging
 import os
 from copy import copy
-from typing import Any, AsyncIterable, Callable, Literal, Type, TypeVar
+from types import MethodType
+from typing import TYPE_CHECKING, Any, AsyncIterable, Callable, ItemsView, Literal, Type, TypeVar, Union
 
+import httpx
 import yaml
 from pydantic import Field, field_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
-from semantic_kernel.contents.streaming_kernel_content import StreamingKernelContent
+from semantic_kernel.connectors.openai_plugin.openai_authentication_config import OpenAIAuthenticationConfig
+from semantic_kernel.connectors.openai_plugin.openai_function_execution_parameters import (
+    OpenAIFunctionExecutionParameters,
+)
+from semantic_kernel.connectors.openai_plugin.openai_utils import OpenAIUtils
+from semantic_kernel.connectors.openapi_plugin.openapi_function_execution_parameters import (
+    OpenAPIFunctionExecutionParameters,
+)
+from semantic_kernel.connectors.openapi_plugin.openapi_manager import OpenAPIPlugin
+from semantic_kernel.connectors.utils.document_loader import DocumentLoader
 from semantic_kernel.events import FunctionInvokedEventArgs, FunctionInvokingEventArgs
 from semantic_kernel.exceptions import (
     FunctionInitializationError,
     FunctionNameNotUniqueError,
     KernelFunctionAlreadyExistsError,
     KernelFunctionNotFoundError,
     KernelInvokeException,
+    KernelPluginInvalidConfigurationError,
     KernelPluginNotFoundError,
     KernelServiceNotFoundError,
     PluginInitializationError,
     PluginInvalidNameError,
     ServiceInvalidRequestError,
     ServiceInvalidTypeError,
     TemplateSyntaxError,
@@ -34,29 +47,32 @@
 from semantic_kernel.functions.kernel_function import TEMPLATE_FORMAT_MAP, KernelFunction
 from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_plugin import KernelPlugin
 from semantic_kernel.functions.kernel_plugin_collection import KernelPluginCollection
 from semantic_kernel.kernel_pydantic import KernelBaseModel
-from semantic_kernel.prompt_template.const import (
-    KERNEL_TEMPLATE_FORMAT_NAME,
-    TEMPLATE_FORMAT_TYPES,
-)
+from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME, TEMPLATE_FORMAT_TYPES
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 from semantic_kernel.reliability.pass_through_without_retry import PassThroughWithoutRetry
 from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 from semantic_kernel.services.ai_service_selector import AIServiceSelector
 from semantic_kernel.utils.validation import validate_plugin_name
 
+if TYPE_CHECKING:
+    from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
+    from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
+    from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+    from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
+
 T = TypeVar("T")
 
-ALL_SERVICE_TYPES = "TextCompletionClientBase | ChatCompletionClientBase | EmbeddingGeneratorBase"
+ALL_SERVICE_TYPES = Union["TextCompletionClientBase", "ChatCompletionClientBase", "EmbeddingGeneratorBase"]
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class Kernel(KernelBaseModel):
     """
     The Kernel class is the main entry point for the Semantic Kernel. It provides the ability to run
@@ -138,15 +154,15 @@
         self,
         functions: KernelFunction | list[KernelFunction] | None = None,
         arguments: KernelArguments | None = None,
         function_name: str | None = None,
         plugin_name: str | None = None,
         return_function_results: bool | None = False,
         **kwargs: Any,
-    ) -> AsyncIterable[list["StreamingKernelContent"] | list[FunctionResult]]:
+    ) -> AsyncIterable[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult]]:
         """Execute one or more stream functions.
 
         This will execute the functions in the order they are provided, if a list of functions is provided.
         When multiple functions are provided only the last one is streamed, the rest is executed as a pipeline.
 
         Arguments:
             functions (KernelFunction | list[KernelFunction]): The function or functions to execute,
@@ -156,15 +172,15 @@
             function_name (str | None): The name of the function to execute
             plugin_name (str | None): The name of the plugin to execute
             return_function_results (bool | None): If True, the function results are returned in addition to
                 the streaming content, otherwise only the streaming content is returned.
             kwargs (dict[str, Any]): arguments that can be used instead of supplying KernelArguments
 
         Yields:
-            StreamingKernelContent: The content of the stream of the last function provided.
+            StreamingContentMixin: The content of the stream of the last function provided.
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
         if not functions:
             if not function_name or not plugin_name:
                 raise KernelFunctionNotFoundError("No function(s) or function- and plugin-name provided")
             functions = [self.func(plugin_name, function_name)]
@@ -203,46 +219,54 @@
                 logger.info(
                     f"Execution was skipped on function invoking event of pipeline step "
                     f"{pipeline_step}: {stream_function.plugin_name}.{stream_function.name}."
                 )
                 return
                 # TODO: decide how to put results into kernelarguments,
                 # might need to be done as part of the invoked_handler
-            function_result = []
+            function_result: FunctionResult | list[list["StreamingContentMixin"] | Any] = []
             exception = None
 
             async for stream_message in stream_function.invoke_stream(self, arguments):
                 if isinstance(stream_message, FunctionResult):
-                    exception = stream_message.metadata.get("exception", None)
-                    if exception:
-                        break
+                    function_result = stream_message
+                    break
+                assert isinstance(function_result, list)
                 function_result.append(stream_message)
                 yield stream_message
 
-            output_function_result = []
-            for result in function_result:
-                for choice in result:
-                    if len(output_function_result) <= choice.choice_index:
-                        output_function_result.append(copy(choice))
-                    else:
-                        output_function_result[choice.choice_index] += choice
-            func_result = FunctionResult(function=stream_function.metadata, value=output_function_result)
+            if isinstance(function_result, FunctionResult):
+                func_result = function_result
+                exception = func_result.metadata.get("exception", None)
+            else:
+                output_function_result: list["StreamingContentMixin"] = []
+                assert isinstance(function_result, list)
+                for result in function_result:
+                    assert isinstance(result, list)
+                    for choice in result:
+                        if isinstance(choice, FunctionResult):
+                            continue
+                        if len(output_function_result) <= choice.choice_index:
+                            output_function_result.append(copy(choice))
+                        else:
+                            output_function_result[choice.choice_index] += choice
+                func_result = FunctionResult(function=stream_function.metadata, value=output_function_result)
             function_invoked_args = self.on_function_invoked(
                 stream_function.metadata,
                 arguments,
                 func_result,
                 exception,
             )
             if function_invoked_args.exception:
                 raise ServiceInvalidRequestError(
                     f"Something went wrong in stream function. "
                     f"During function invocation:'{stream_function.plugin_name}.{stream_function.name}'. "
                     f"Error description: '{str(function_invoked_args.exception)}'"
                 ) from function_invoked_args.exception
-            if return_function_results:
+            if return_function_results and function_invoked_args.function_result:
                 results.append(function_invoked_args.function_result)
             if function_invoked_args.is_cancel_requested:
                 logger.info(
                     f"Execution was cancelled on function invoked event of pipeline step "
                     f"{pipeline_step}: {stream_function.plugin_name}.{stream_function.name}."
                 )
                 return
@@ -285,15 +309,15 @@
 
         Returns:
             FunctionResult | list[FunctionResult] | None: The result of the function(s)
 
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
-        results = []
+        results: list[FunctionResult] = []
         pipeline_step = 0
         if not functions:
             if not function_name or not plugin_name:
                 raise KernelFunctionNotFoundError("No function or plugin name provided")
             functions = [self.func(plugin_name, function_name)]
         if not isinstance(functions, list):
             functions = [functions]
@@ -331,26 +355,29 @@
                         "Something went wrong in function invocation. During function invocation:"
                         f" '{func.plugin_name}.{func.name}'. Error description: '{str(exc)}'"
                     )
                     exception = exc
 
                 # this allows a hook to alter the results before adding.
                 function_invoked_args = self.on_function_invoked(func.metadata, arguments, function_result, exception)
-                results.append(function_invoked_args.function_result)
+                if function_invoked_args.function_result:
+                    results.append(function_invoked_args.function_result)
+                else:
+                    results.append(FunctionResult(function=func.metadata, value=None, metadata={}))
 
                 if function_invoked_args.exception:
                     raise KernelInvokeException(
                         f"Error occurred while invoking function: '{func.plugin_name}.{func.name}'"
                     ) from function_invoked_args.exception
                 if function_invoked_args.is_cancel_requested:
                     logger.info(
                         f"Execution was cancelled on function invoked event of pipeline step "
                         f"{pipeline_step}: {func.plugin_name}.{func.name}."
                     )
-                    return results if results else None
+                    return results if results else FunctionResult(function=func.metadata, value=None, metadata={})
                 if function_invoked_args.updated_arguments:
                     logger.info(
                         f"Arguments updated by function_invoked_handler in pipeline step: "
                         f"{pipeline_step}, new arguments: {function_invoked_args.arguments}"
                     )
                     arguments = function_invoked_args.arguments
                 if function_invoked_args.is_repeat_requested:
@@ -490,14 +517,15 @@
             KernelPlugin: The imported plugin of type KernelPlugin.
         """
         if not plugin_name.strip():
             raise PluginInvalidNameError("Plugin name cannot be empty")
         logger.debug(f"Importing plugin {plugin_name}")
 
         functions: dict[str, KernelFunction] = {}
+        candidates: list[tuple[str, MethodType]] | ItemsView[str, Any] = []
 
         if isinstance(plugin_instance, dict):
             candidates = plugin_instance.items()
         else:
             candidates = inspect.getmembers(plugin_instance, inspect.ismethod)
         # Read every method from the plugin instance
         for _, candidate in candidates:
@@ -514,29 +542,34 @@
         logger.debug(f"Methods imported: {len(functions)}")
 
         plugin = KernelPlugin(name=plugin_name, functions=functions)
         self.plugins.add(plugin)
 
         return plugin
 
-    def import_native_plugin_from_directory(self, parent_directory: str, plugin_directory_name: str) -> KernelPlugin:
+    def import_native_plugin_from_directory(
+        self, parent_directory: str, plugin_directory_name: str
+    ) -> KernelPlugin | None:
         MODULE_NAME = "native_function"
 
         validate_plugin_name(plugin_directory_name)
 
         plugin_directory = os.path.abspath(os.path.join(parent_directory, plugin_directory_name))
         native_py_file_path = os.path.join(plugin_directory, f"{MODULE_NAME}.py")
 
         if not os.path.exists(native_py_file_path):
             raise PluginInitializationError(f"Native Plugin Python File does not exist: {native_py_file_path}")
 
         plugin_name = os.path.basename(plugin_directory)
 
         spec = importlib.util.spec_from_file_location(MODULE_NAME, native_py_file_path)
+        if not spec:
+            raise PluginInitializationError(f"Failed to load plugin: {plugin_name}")
         module = importlib.util.module_from_spec(spec)
+        assert spec.loader
         spec.loader.exec_module(module)
 
         class_name = next(
             (name for name, cls in inspect.getmembers(module, inspect.isclass) if cls.__module__ == MODULE_NAME),
             None,
         )
         if class_name:
@@ -615,15 +648,15 @@
                         prompt_template_config = PromptTemplateConfig.from_json(config_file.read())
                     prompt_template_config.name = item
 
                     with open(prompt_path, "r") as prompt_file:
                         prompt = prompt_file.read()
                         prompt_template_config.template = prompt
 
-                    prompt_template = TEMPLATE_FORMAT_MAP[prompt_template_config.template_format](
+                    prompt_template = TEMPLATE_FORMAT_MAP[prompt_template_config.template_format](  # type: ignore
                         prompt_template_config=prompt_template_config
                     )
 
                     functions.append(
                         self.create_function_from_prompt(
                             plugin_name=plugin_directory_name,
                             prompt_template=prompt_template,
@@ -632,14 +665,110 @@
                             function_name=item,
                             description=prompt_template_config.description,
                         )
                     )
 
         return KernelPlugin(name=plugin_directory_name, functions=functions)
 
+    async def import_plugin_from_openai(
+        self,
+        plugin_name: str,
+        plugin_url: str | None = None,
+        plugin_str: str | None = None,
+        execution_parameters: OpenAIFunctionExecutionParameters | None = None,
+    ) -> KernelPlugin:
+        """Create a plugin from the Open AI manifest.
+
+        Args:
+            plugin_name (str): The name of the plugin
+            plugin_url (str | None): The URL of the plugin
+            plugin_str (str | None): The JSON string of the plugin
+            execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
+
+        Returns:
+            KernelPlugin: The imported plugin
+
+        Raises:
+            PluginInitializationError: if the plugin URL or plugin JSON/YAML is not provided
+        """
+
+        if execution_parameters is None:
+            execution_parameters = OpenAIFunctionExecutionParameters()
+
+        validate_plugin_name(plugin_name)
+
+        if plugin_str is not None:
+            # Load plugin from the provided JSON string/YAML string
+            openai_manifest = plugin_str
+        elif plugin_url is not None:
+            # Load plugin from the URL
+            http_client = execution_parameters.http_client if execution_parameters.http_client else httpx.AsyncClient()
+            openai_manifest = await DocumentLoader.from_uri(
+                url=plugin_url, http_client=http_client, auth_callback=None, user_agent=execution_parameters.user_agent
+            )
+        else:
+            raise PluginInitializationError("Either plugin_url or plugin_json must be provided.")
+
+        try:
+            plugin_json = json.loads(openai_manifest)
+            openai_auth_config = OpenAIAuthenticationConfig(**plugin_json["auth"])
+        except json.JSONDecodeError as ex:
+            raise KernelPluginInvalidConfigurationError("Parsing of Open AI manifest for auth config failed.") from ex
+
+        # Modify the auth callback in execution parameters if it's provided
+        if execution_parameters and execution_parameters.auth_callback:
+            initial_auth_callback = execution_parameters.auth_callback
+
+            async def custom_auth_callback(**kwargs):
+                return await initial_auth_callback(plugin_name, openai_auth_config, **kwargs)
+
+            execution_parameters.auth_callback = custom_auth_callback
+
+        try:
+            openapi_spec_url = OpenAIUtils.parse_openai_manifest_for_openapi_spec_url(plugin_json)
+        except PluginInitializationError as ex:
+            raise KernelPluginInvalidConfigurationError(
+                "Parsing of Open AI manifest for OpenAPI spec URL failed."
+            ) from ex
+
+        return self.import_plugin_from_openapi(
+            plugin_name=plugin_name,
+            openapi_document_path=openapi_spec_url,
+            execution_settings=execution_parameters,
+        )
+
+    def import_plugin_from_openapi(
+        self,
+        plugin_name: str,
+        openapi_document_path: str,
+        execution_settings: "OpenAIFunctionExecutionParameters" | "OpenAPIFunctionExecutionParameters" | None = None,
+    ) -> KernelPlugin:
+        """Create a plugin from an OpenAPI manifest.
+
+        Args:
+            plugin_name (str): The name of the plugin
+            openapi_document_path (str): The OpenAPI document path
+            execution_settings (OpenAIFunctionExecutionParameters | OpenAPIFunctionExecutionParameters | None):
+                The execution settings
+
+        Returns:
+            KernelPlugin: The imported plugin
+        """
+        validate_plugin_name(plugin_name)
+
+        if not openapi_document_path:
+            raise PluginInitializationError("OpenAPI document path is required.")
+
+        plugin = OpenAPIPlugin.create(
+            plugin_name=plugin_name,
+            openapi_document_path=openapi_document_path,
+            execution_settings=execution_settings,
+        )
+        return self.import_plugin_from_object(plugin, plugin_name)
+
     def _validate_plugin_directory(self, parent_directory: str, plugin_directory_name: str) -> str:
         """Validate the plugin name and that the plugin directory exists.
 
         Args:
             parent_directory (str): The parent directory
             plugin_directory_name (str): The plugin directory name
 
@@ -805,15 +934,15 @@
         """Uses the AI service selector to select a service for the function."""
         return self.ai_service_selector.select_ai_service(self, function, arguments)
 
     def get_service(
         self,
         service_id: str | None = None,
         type: Type[ALL_SERVICE_TYPES] | None = None,
-    ) -> ALL_SERVICE_TYPES:
+    ) -> "AIServiceClientBase":
         """Get a service by service_id and type.
 
         Type is optional and when not supplied, no checks are done.
         Type should be
             TextCompletionClientBase, ChatCompletionClientBase, EmbeddingGeneratorBase
             or a subclass of one.
             You can also check for multiple types in one go,
@@ -829,14 +958,15 @@
         Returns:
             ALL_SERVICE_TYPES: The service.
 
         Raises:
             ValueError: If no service is found that matches the type.
 
         """
+        service: "AIServiceClientBase | None" = None
         if not service_id or service_id == "default":
             if not type:
                 if default_service := self.services.get("default"):
                     return default_service
                 return list(self.services.values())[0]
             if default_service := self.services.get("default"):
                 if isinstance(default_service, type):
@@ -847,19 +977,19 @@
             raise KernelServiceNotFoundError(f"No service found of type {type}")
         if not (service := self.services.get(service_id)):
             raise KernelServiceNotFoundError(f"Service with service_id '{service_id}' does not exist")
         if type and not isinstance(service, type):
             raise ServiceInvalidTypeError(f"Service with service_id '{service_id}' is not of type {type}")
         return service
 
-    def get_services_by_type(self, type: Type[T]) -> dict[str, T]:
+    def get_services_by_type(self, type: Type[ALL_SERVICE_TYPES]) -> dict[str, "AIServiceClientBase"]:
         return {service.service_id: service for service in self.services.values() if isinstance(service, type)}
 
     def get_prompt_execution_settings_from_service_id(
-        self, service_id: str, type: Type[T] | None = None
+        self, service_id: str, type: Type[ALL_SERVICE_TYPES] | None = None
     ) -> PromptExecutionSettings:
         """Get the specific request settings from the service, instantiated with the service_id and ai_model_id."""
         service = self.get_service(service_id, type=type)
         return service.instantiate_prompt_execution_settings(
             service_id=service_id,
             extension_data={"ai_model_id": service.ai_model_id},
         )
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/kernel_pydantic.py` & `semantic_kernel-0.9.5b1/semantic_kernel/kernel_pydantic.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import List, Optional
 
 from pydantic import PrivateAttr
 
-from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
-    EmbeddingGeneratorBase,
-)
+from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 
 
 class SemanticTextMemory(SemanticTextMemoryBase):
     _storage: MemoryStoreBase = PrivateAttr()
+    # TODO: replace with kernel and service_selector pattern
     _embeddings_generator: EmbeddingGeneratorBase = PrivateAttr()
 
     def __init__(self, storage: MemoryStoreBase, embeddings_generator: EmbeddingGeneratorBase) -> None:
         """Initialize a new instance of SemanticTextMemory.
 
         Arguments:
             storage {MemoryStoreBase} -- The MemoryStoreBase to use for storage.
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.9.5b1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/action_planner/action_planner.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/action_planner/action_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,19 +144,20 @@
             logger.info(
                 f"ActionPlanner has picked {generated_plan['plan']['function']}.       "
                 "              Reference to this function found in context:"
                 f" {function_ref}"
             )
             plan = Plan(description=goal, function=function_ref)
 
-        for key, val in generated_plan["plan"]["parameters"].items():
-            logger.info(f"Parameter {key}: {val}")
-            if val:
-                plan.parameters[key] = str(val)
-                plan.state[key] = str(val)
+        if "parameters" in generated_plan["plan"]:
+            for key, val in generated_plan["plan"]["parameters"].items():
+                logger.info(f"Parameter {key}: {val}")
+                if val:
+                    plan.parameters[key] = str(val)
+                    plan.state[key] = str(val)
 
         return plan
 
     @kernel_function(description="List a few good examples of plans to generate", name="GoodExamples")
     def good_examples(self, goal: Annotated[str, "The current goal processed by the planner"]) -> str:
         return dedent(
             """
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/basic_planner.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from typing import Optional
 
 import yaml
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
+from semantic_kernel.connectors.ai.open_ai.services.azure_chat_completion import AzureChatCompletion
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion import OpenAIChatCompletion
 from semantic_kernel.connectors.ai.open_ai.utils import (
+    get_function_calling_object,
     get_tool_call_object,
 )
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.exceptions.planner_exceptions import PlannerInvalidConfigurationError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
@@ -24,27 +26,26 @@
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner_options import (
     FunctionCallingStepwisePlannerOptions,
 )
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner_result import (
     FunctionCallingStepwisePlannerResult,
     UserInteraction,
 )
-from semantic_kernel.planners.planner_extensions import PlannerKernelExtension
 from semantic_kernel.prompt_template.kernel_prompt_template import KernelPromptTemplate
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
 CUR_DIR = os.path.dirname(os.path.realpath(__file__))
 PLAN_YAML_FILE_PATH = os.path.join(CUR_DIR, "generate_plan.yaml")
 STEP_PROMPT_FILE_PATH = os.path.join(CUR_DIR, "step_prompt.txt")
 
 STEPWISE_PLANNER_PLUGIN_NAME = "StepwisePlanner_Excluded"
 
 STEPWISE_USER_MESSAGE = (
-    "Perform the next step of the plan if there is more work to do."
-    "When you have reached a final answer, use the UserInteraction-SendFinalAnswer"
+    "Perform the next step of the plan if there is more work to do. "
+    "When you have reached a final answer, use the UserInteraction-SendFinalAnswer "
     "function to communicate this back to the user."
 )
 
 USER_INTERACTION_SEND_FINAL_ANSWER = "UserInteraction-SendFinalAnswer"
 
 logger: logging.Logger = logging.getLogger(__name__)
 
@@ -102,25 +103,33 @@
         Raises:
             PlannerInvalidConfigurationError: If the input question is empty
         """
         if not question:
             raise PlannerInvalidConfigurationError("Input question cannot be empty")
 
         try:
-            chat_completion = kernel.get_service(service_id=self.service_id, type=OpenAIChatCompletion)
+            chat_completion = kernel.get_service(service_id=self.service_id)
         except Exception as exc:
             raise PlannerInvalidConfigurationError(
                 f"The OpenAI service `{self.service_id}` is not available. Please configure the AI service."
             ) from exc
 
+        if not isinstance(chat_completion, (OpenAIChatCompletion, AzureChatCompletion)):
+            raise PlannerInvalidConfigurationError(
+                f"The service with id `{self.service_id}` is not an OpenAI based service."
+            )
+
         prompt_execution_settings: (
             OpenAIChatPromptExecutionSettings
         ) = self.options.execution_settings or chat_completion.get_prompt_execution_settings_class()(
             service_id=self.service_id
         )
+        if self.options.max_completion_tokens:
+            prompt_execution_settings.max_tokens = self.options.max_completion_tokens
+        prompt_execution_settings.max_auto_invoke_attempts = self.options.max_iterations
 
         # Clone the kernel so that we can add planner-specific plugins without affecting the original kernel instance
         cloned_kernel = copy(kernel)
         cloned_kernel.import_plugin_from_object(UserInteraction(), "UserInteraction")
 
         # Create and invoke a kernel function to generate the initial plan
         initial_plan = await self._generate_plan(question, cloned_kernel)
@@ -213,15 +222,17 @@
         self,
         question: str,
         kernel: Kernel,
         arguments: KernelArguments = None,
     ) -> str:
         """Generate the plan for the given question using the kernel"""
         generate_plan_function = self._create_config_from_yaml(kernel)
-        functions_manual = await PlannerKernelExtension.get_functions_manual(kernel, arguments)
+        functions_manual = get_function_calling_object(
+            kernel, {"exclude_function": [f"{self.service_id}", "sequential_planner-create_plan"]}
+        )
         generated_plan_args = KernelArguments(
             name_delimiter="-",
             available_functions=functions_manual,
             goal=question,
         )
         generate_plan_result = await kernel.invoke(generate_plan_function, generated_plan_args)
         return str(generate_plan_result)
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Any, Callable, Optional
+from __future__ import annotations
+
+from typing import Any, Callable
 
 from pydantic import model_validator
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIPromptExecutionSettings,
 )
 from semantic_kernel.planners.planner_options import PlannerOptions
 
 
 class FunctionCallingStepwisePlannerOptions(PlannerOptions):
     """The Function Calling Stepwise Planner Options."""
 
-    max_tokens: Optional[int] = None
-    max_tokens_ratio: Optional[float] = 0.1
-    max_completion_tokens: Optional[int] = None
-    max_prompt_tokens: Optional[int] = None
-    get_initial_plan: Optional[Callable[[], str]] = None
-    get_step_prompt: Optional[Callable[[], str]] = None
-    max_iterations: Optional[int] = 15
-    min_iteration_time_ms: Optional[int] = 100
-    execution_settings: Optional[OpenAIPromptExecutionSettings] = None
+    max_tokens: int | None = None
+    max_tokens_ratio: float | None = 0.1
+    max_completion_tokens: int | None = None
+    max_prompt_tokens: int | None = None
+    get_initial_plan: Callable[[], str] | None = None
+    get_step_prompt: Callable[[], str] | None = None
+    max_iterations: int | None = 15
+    min_iteration_time_ms: int | None = 100
+    execution_settings: OpenAIPromptExecutionSettings | None = None
 
     @model_validator(mode="before")
     @classmethod
     def calculate_token_limits(cls, data: Any) -> Any:
         if isinstance(data, dict):
             max_tokens = data.get("max_tokens")
             # Ensure max_tokens_ratio has a default value if not provided
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/plan.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/Plugins/StepwiseStep/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/stepwise_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py` & `semantic_kernel-0.9.5b1/semantic_kernel/planners/stepwise_planner/stepwise_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 PromptExecutionSettingsT = TypeVar("PromptExecutionSettingsT", bound=PromptExecutionSettings)
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class PromptTemplateConfig(KernelBaseModel):
-    name: Optional[str] = ""
+    name: str = ""
     description: Optional[str] = ""
     template: Optional[str] = None
     template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME
     input_variables: List[InputVariable] = Field(default_factory=list)
     execution_settings: Dict[str, PromptExecutionSettings] = Field(default_factory=dict)
 
     @field_validator("execution_settings", mode="before")
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 
 import json
 import logging
 import re
 from enum import Enum
 from typing import Callable, Dict
 
-from semantic_kernel.contents.chat_history import ROOT_KEY_MESSAGE
+from semantic_kernel.contents.chat_history import ROOT_KEY_MESSAGE, ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+def _messages(this, options, *args, **kwargs):
+    if not isinstance(this.context["chat_history"], ChatHistory):
+        return ""
+    return str(this.context["chat_history"])
+
+
 def _message_to_prompt(this, *args, **kwargs):
     if isinstance(this.context, ChatMessageContent):
         return str(this.context.to_prompt(ROOT_KEY_MESSAGE))
     return str(this.context)
 
 
 def _message(this, options, *args, **kwargs):
@@ -159,8 +165,9 @@
     "camel_case": _camel_case,
     "camelCase": _camel_case,
     "snake_case": _snake_case,
     "snakeCase": _snake_case,
     "message": _message,
     "message_to_prompt": _message_to_prompt,
     "messageToPrompt": _message_to_prompt,
+    "messages": _messages,
 }
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-0.9.5b1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.9.5b1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-0.9.5b1/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-0.9.5b1/semantic_kernel/services/ai_service_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,13 +29,15 @@
         If the same service_id is in both, the one in the arguments will be used.
         """
         execution_settings_dict = arguments.execution_settings or {}
         if func_exec_settings := getattr(function, "prompt_execution_settings", None):
             for id, settings in func_exec_settings.items():
                 if id not in execution_settings_dict:
                     execution_settings_dict[id] = settings
+        if not execution_settings_dict:
+            execution_settings_dict = {"default": PromptExecutionSettings()}
         for service_id, settings in execution_settings_dict.items():
             service = kernel.get_service(service_id, type=(TextCompletionClientBase, ChatCompletionClientBase))
             if service:
                 service_settings = service.get_prompt_execution_settings_from_settings(settings)
                 return service, service_settings
         raise KernelServiceNotFoundError("No service found.")
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.9.5b1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.9.5b1/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.9.5b1/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/utils/naming.py` & `semantic_kernel-0.9.5b1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/utils/null_logger.py` & `semantic_kernel-0.9.5b1/semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/utils/settings.py` & `semantic_kernel-0.9.5b1/semantic_kernel/utils/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -292,7 +292,43 @@
     Reads the Azure AI Search environment variables including index name from the .env file.
 
     Returns:
         Dict[str, str]: the Azure AI search environment variables
     """
     api_key, url, index_name = azure_aisearch_settings_from_dot_env(include_index_name=True)
     return {"key": api_key, "endpoint": url, "indexName": index_name}
+
+
+def azure_key_vault_settings_from_dot_env(
+    include_client_id: bool = True, include_client_secret: bool = True
+) -> Tuple[str, Optional[str], Optional[str]]:
+    """
+    Reads the Azure Key Vault environment variables for the .env file.
+
+    Returns:
+        Tuple[str, str, str]: Azure Key Vault endpoint, the Azure Key Vault client ID, the Azure Key Vault client secret
+    """
+    config = dotenv_values(".env")
+    endpoint = config.get("AZURE_KEY_VAULT_ENDPOINT", None)
+    client_id = config.get("AZURE_KEY_VAULT_CLIENT_ID", None)
+    client_secret = config.get("AZURE_KEY_VAULT_CLIENT_SECRET", None)
+
+    assert endpoint is not None, "Azure Key Vault endpoint not found in .env file"
+    if include_client_id:
+        assert client_id is not None, "Azure Key Vault client ID not found in .env file"
+    if include_client_secret:
+        assert client_secret is not None, "Azure Key Vault client secret not found in .env file"
+
+    if include_client_id and include_client_secret:
+        return endpoint, client_id, client_secret
+    return endpoint, client_id
+
+
+def azure_key_vault_settings_from_dot_env_as_dict() -> Dict[str, str]:
+    """
+    Reads the Azure Key Vault environment variables for the .env file.
+
+    Returns:
+        Dict[str, str]: Azure Key Vault environment variables
+    """
+    endpoint, client_id, client_secret = azure_key_vault_settings_from_dot_env()
+    return {"endpoint": endpoint, "client_id": client_id, "client_secret": client_secret}
```

### Comparing `semantic_kernel-0.9.4b1/semantic_kernel/utils/validation.py` & `semantic_kernel-0.9.5b1/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.4b1/PKG-INFO` & `semantic_kernel-0.9.5b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.9.4b1
+Version: 0.9.5b1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,15 +26,15 @@
 Provides-Extra: weaviate
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: azure-core (>=1.28.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-identity (>=1.13.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-search-documents (==11.6.0b1) ; extra == "azure" or extra == "all"
 Requires-Dist: chromadb (>=0.4.13,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: eval_type_backport (>=0.1.3,<0.2.0) ; python_version < "3.9"
+Requires-Dist: eval_type_backport (>=0.1.3,<0.2.0) ; python_version < "3.10"
 Requires-Dist: google-generativeai (>=0.1) ; (python_version >= "3.9") and (extra == "google" or extra == "all")
 Requires-Dist: grpcio (>=1.40.0) ; python_version == "3.8"
 Requires-Dist: grpcio (>=1.50.0) ; python_version >= "3.9"
 Requires-Dist: grpcio (>=1.60.0) ; python_version >= "3.12"
 Requires-Dist: grpcio-status (>=1.53.0,<2.0.0) ; (python_version >= "3.9") and (extra == "google" or extra == "all")
 Requires-Dist: ipykernel (>=6.21.1,<7.0.0) ; extra == "notebooks" or extra == "all"
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
```

