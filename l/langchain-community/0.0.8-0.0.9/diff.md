# Comparing `tmp/langchain_community-0.0.8.tar.gz` & `tmp/langchain_community-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_community-0.0.8.tar", max compression
+gzip compressed data, was "langchain_community-0.0.9.tar", max compression
```

## Comparing `langchain_community-0.0.8.tar` & `langchain_community-0.0.9.tar`

### file list

```diff
@@ -1,892 +1,892 @@
--rw-r--r--   0        0        0     1201 2024-01-03 17:13:53.974334 langchain_community-0.0.8/README.md
--rw-r--r--   0        0        0      307 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/adapters/__init__.py
--rw-r--r--   0        0        0    12143 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/adapters/openai.py
--rw-r--r--   0        0        0     3327 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0     1781 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/amadeus/__init__.py
--rw-r--r--   0        0        0      961 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0     1035 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0      397 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0     3594 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0     1091 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      177 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0     3250 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0    10135 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0     2904 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0     2045 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0     2227 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0     1894 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/json/base.py
--rw-r--r--   0        0        0     1819 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0      595 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0     1190 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0     1931 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0     2038 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0     4228 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0     1812 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0     2870 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0    12987 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0    11686 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0     1743 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0     2557 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0     3317 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0      174 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0     4274 2024-01-03 17:13:53.974334 langchain_community-0.0.8/langchain_community/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0     2507 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0     2649 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0     2773 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0     3771 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0       21 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0     1114 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0       23 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0     2355 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0     1202 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0     1084 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0     3866 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0     1428 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0     2862 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0     1465 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0     1095 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0     1933 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0    58113 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/cache.py
--rw-r--r--   0        0        0     2671 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/__init__.py
--rw-r--r--   0        0        0    14408 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/aim_callback.py
--rw-r--r--   0        0        0    14820 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/argilla_callback.py
--rw-r--r--   0        0        0     7438 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/arize_callback.py
--rw-r--r--   0        0        0    11266 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/arthur_callback.py
--rw-r--r--   0        0        0    18897 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/clearml_callback.py
--rw-r--r--   0        0        0    23193 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0     6340 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/confident_callback.py
--rw-r--r--   0        0        0     6498 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/context_callback.py
--rw-r--r--   0        0        0    13138 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/flyte_callback.py
--rw-r--r--   0        0        0     2587 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/human.py
--rw-r--r--   0        0        0     9224 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/infino_callback.py
--rw-r--r--   0        0        0    13880 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0    20527 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     1891 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/manager.py
--rw-r--r--   0        0        0    24156 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0     7710 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/openai_info.py
--rw-r--r--   0        0        0     5535 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0     8758 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0     3211 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0     5435 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0    15534 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      407 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0     4713 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/tracers/comet.py
--rw-r--r--   0        0        0    19114 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0     4526 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0     8505 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/utils.py
--rw-r--r--   0        0        0    20601 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/wandb_callback.py
--rw-r--r--   0        0        0     8067 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0      452 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/__init__.py
--rw-r--r--   0        0        0      444 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/base.py
--rw-r--r--   0        0        0     2705 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0     4048 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/gmail.py
--rw-r--r--   0        0        0     7910 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/imessage.py
--rw-r--r--   0        0        0     5742 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/langsmith.py
--rw-r--r--   0        0        0     3112 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/slack.py
--rw-r--r--   0        0        0     5390 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/telegram.py
--rw-r--r--   0        0        0     3270 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/utils.py
--rw-r--r--   0        0        0     4280 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     2570 2024-01-03 17:13:53.978334 langchain_community-0.0.8/langchain_community/chat_message_histories/__init__.py
--rw-r--r--   0        0        0     4127 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/astradb.py
--rw-r--r--   0        0        0     2392 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0     6510 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0     5810 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0     6836 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0     1379 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/file.py
--rw-r--r--   0        0        0     3349 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      633 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0     7112 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/momento.py
--rw-r--r--   0        0        0     2734 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0     4288 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0     2659 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/postgres.py
--rw-r--r--   0        0        0     1971 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/redis.py
--rw-r--r--   0        0        0     9515 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0    10331 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0     4717 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/sql.py
--rw-r--r--   0        0        0     1176 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0     2148 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0     4652 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/xata.py
--rw-r--r--   0        0        0     6452 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_message_histories/zep.py
--rw-r--r--   0        0        0     3659 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/__init__.py
--rw-r--r--   0        0        0     7963 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/anthropic.py
--rw-r--r--   0        0        0     7945 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/anyscale.py
--rw-r--r--   0        0        0    11171 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/azure_openai.py
--rw-r--r--   0        0        0     6007 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0    10083 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/baichuan.py
--rw-r--r--   0        0        0    12777 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     4284 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/bedrock.py
--rw-r--r--   0        0        0     7571 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/cohere.py
--rw-r--r--   0        0        0     1250 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/databricks.py
--rw-r--r--   0        0        0     7874 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/ernie.py
--rw-r--r--   0        0        0     5586 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/everlyai.py
--rw-r--r--   0        0        0     3217 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/fake.py
--rw-r--r--   0        0        0    11742 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/fireworks.py
--rw-r--r--   0        0        0     6312 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/gigachat.py
--rw-r--r--   0        0        0    11608 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/google_palm.py
--rw-r--r--   0        0        0    12859 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/gpt_router.py
--rw-r--r--   0        0        0     5549 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/huggingface.py
--rw-r--r--   0        0        0     3698 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/human.py
--rw-r--r--   0        0        0    10549 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/hunyuan.py
--rw-r--r--   0        0        0     7654 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0    15167 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/jinachat.py
--rw-r--r--   0        0        0    10992 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/konko.py
--rw-r--r--   0        0        0    15710 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/litellm.py
--rw-r--r--   0        0        0      967 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/meta.py
--rw-r--r--   0        0        0     3180 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/minimax.py
--rw-r--r--   0        0        0     6908 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/mlflow.py
--rw-r--r--   0        0        0     6737 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0    13160 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/ollama.py
--rw-r--r--   0        0        0    26580 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/openai.py
--rw-r--r--   0        0        0    10376 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0     5261 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0    14261 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/tongyi.py
--rw-r--r--   0        0        0    14385 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/vertexai.py
--rw-r--r--   0        0        0     5119 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0     5054 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/wasm_chat.py
--rw-r--r--   0        0        0     9392 2024-01-03 17:13:53.982334 langchain_community-0.0.8/langchain_community/chat_models/yandex.py
--rw-r--r--   0        0        0    11166 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/chat_models/zhipuai.py
--rw-r--r--   0        0        0      549 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/docstore/__init__.py
--rw-r--r--   0        0        0     1090 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      833 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/docstore/base.py
--rw-r--r--   0        0        0       70 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/docstore/document.py
--rw-r--r--   0        0        0     1610 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/docstore/in_memory.py
--rw-r--r--   0        0        0     1487 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/docstore/wikipedia.py
--rw-r--r--   0        0        0    16095 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/__init__.py
--rw-r--r--   0        0        0     2841 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/acreom.py
--rw-r--r--   0        0        0    10240 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/airbyte.py
--rw-r--r--   0        0        0      815 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0     1281 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/airtable.py
--rw-r--r--   0        0        0     2759 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0     5272 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0      879 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/arxiv.py
--rw-r--r--   0        0        0     4218 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/assemblyai.py
--rw-r--r--   0        0        0     3454 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/astradb.py
--rw-r--r--   0        0        0     8129 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/async_html.py
--rw-r--r--   0        0        0      563 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/azlyrics.py
--rw-r--r--   0        0        0     1545 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0     1582 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0     1644 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0     1857 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0     1931 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0     3175 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/base.py
--rw-r--r--   0        0        0     6992 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/base_o365.py
--rw-r--r--   0        0        0     3922 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/bibtex.py
--rw-r--r--   0        0        0     3673 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/bigquery.py
--rw-r--r--   0        0        0     2736 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/bilibili.py
--rw-r--r--   0        0        0    10302 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/blackboard.py
--rw-r--r--   0        0        0      374 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0     5340 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0     6636 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0     1526 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0     5709 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/blockchain.py
--rw-r--r--   0        0        0     1047 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/brave_search.py
--rw-r--r--   0        0        0     2124 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/browserless.py
--rw-r--r--   0        0        0     1986 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/chatgpt.py
--rw-r--r--   0        0        0     2746 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/chromium.py
--rw-r--r--   0        0        0      527 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/college_confidential.py
--rw-r--r--   0        0        0     3269 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/concurrent.py
--rw-r--r--   0        0        0    27612 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/confluence.py
--rw-r--r--   0        0        0     1052 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/conllu.py
--rw-r--r--   0        0        0     3649 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/couchbase.py
--rw-r--r--   0        0        0     5926 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/csv_loader.py
--rw-r--r--   0        0        0     6617 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0     4937 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0     1923 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/dataframe.py
--rw-r--r--   0        0        0     2054 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/diffbot.py
--rw-r--r--   0        0        0     5942 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/directory.py
--rw-r--r--   0        0        0     1237 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/discord.py
--rw-r--r--   0        0        0     3146 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/doc_intelligence.py
--rw-r--r--   0        0        0    13450 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/docugami.py
--rw-r--r--   0        0        0     1852 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/docusaurus.py
--rw-r--r--   0        0        0     6229 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/dropbox.py
--rw-r--r--   0        0        0     3150 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0     3834 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/email.py
--rw-r--r--   0        0        0     1496 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/epub.py
--rw-r--r--   0        0        0     7798 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/etherscan.py
--rw-r--r--   0        0        0     5757 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/evernote.py
--rw-r--r--   0        0        0     1687 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/excel.py
--rw-r--r--   0        0        0     1270 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0     2254 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/fauna.py
--rw-r--r--   0        0        0     1543 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/figma.py
--rw-r--r--   0        0        0     2118 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0     3138 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/gcs_file.py
--rw-r--r--   0        0        0     6390 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/generic.py
--rw-r--r--   0        0        0     2518 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/geodataframe.py
--rw-r--r--   0        0        0     4116 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/git.py
--rw-r--r--   0        0        0     3453 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/gitbook.py
--rw-r--r--   0        0        0     6973 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/github.py
--rw-r--r--   0        0        0     5096 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0    14225 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/googledrive.py
--rw-r--r--   0        0        0      928 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/gutenberg.py
--rw-r--r--   0        0        0     1557 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/helpers.py
--rw-r--r--   0        0        0     2075 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/hn.py
--rw-r--r--   0        0        0     1158 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/html.py
--rw-r--r--   0        0        0     2045 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/html_bs.py
--rw-r--r--   0        0        0     3208 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0     7642 2024-01-03 17:13:53.986334 langchain_community-0.0.8/langchain_community/document_loaders/ifixit.py
--rw-r--r--   0        0        0     1173 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/image.py
--rw-r--r--   0        0        0     3594 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/image_captions.py
--rw-r--r--   0        0        0      477 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/imsdb.py
--rw-r--r--   0        0        0     1688 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/iugu.py
--rw-r--r--   0        0        0     3705 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/joplin.py
--rw-r--r--   0        0        0     5907 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/json_loader.py
--rw-r--r--   0        0        0     6058 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/lakefs.py
--rw-r--r--   0        0        0     2008 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/larksuite.py
--rw-r--r--   0        0        0     1818 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/markdown.py
--rw-r--r--   0        0        0     3112 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/mastodon.py
--rw-r--r--   0        0        0     3282 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/max_compute.py
--rw-r--r--   0        0        0     3918 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      846 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/merge.py
--rw-r--r--   0        0        0     2540 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/mhtml.py
--rw-r--r--   0        0        0     3074 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0     2522 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/mongodb.py
--rw-r--r--   0        0        0     4296 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/news.py
--rw-r--r--   0        0        0     4301 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/notebook.py
--rw-r--r--   0        0        0      814 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/notion.py
--rw-r--r--   0        0        0     6718 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/notiondb.py
--rw-r--r--   0        0        0     1088 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/nuclia.py
--rw-r--r--   0        0        0     3593 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/obs_directory.py
--rw-r--r--   0        0        0     4768 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/obs_file.py
--rw-r--r--   0        0        0     6150 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/obsidian.py
--rw-r--r--   0        0        0     1770 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/odt.py
--rw-r--r--   0        0        0     3381 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/onedrive.py
--rw-r--r--   0        0        0     1154 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0     8074 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/onenote.py
--rw-r--r--   0        0        0     1331 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/open_city_data.py
--rw-r--r--   0        0        0     1748 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/org_mode.py
--rw-r--r--   0        0        0      947 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0    10716 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0     4534 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/doc_intelligence.py
--rw-r--r--   0        0        0    15283 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0     2502 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0     5767 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      109 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0     1609 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      136 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0     3745 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      495 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0     2103 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0     5114 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0     1679 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0     1664 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0    21036 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0     1214 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0      505 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0    26024 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/pdf.py
--rw-r--r--   0        0        0     1161 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0     2508 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/powerpoint.py
--rw-r--r--   0        0        0     1371 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/psychic.py
--rw-r--r--   0        0        0     1172 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/pubmed.py
--rw-r--r--   0        0        0     3388 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0      527 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/python.py
--rw-r--r--   0        0        0     8426 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/quip.py
--rw-r--r--   0        0        0     6928 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/readthedocs.py
--rw-r--r--   0        0        0    11591 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0     4584 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/reddit.py
--rw-r--r--   0        0        0      705 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/roam.py
--rw-r--r--   0        0        0     4604 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0     4936 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/rspace.py
--rw-r--r--   0        0        0     4895 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/rss.py
--rw-r--r--   0        0        0     1832 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/rst.py
--rw-r--r--   0        0        0     2061 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/rtf.py
--rw-r--r--   0        0        0     5759 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/s3_directory.py
--rw-r--r--   0        0        0     5412 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/s3_file.py
--rw-r--r--   0        0        0     2318 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/sharepoint.py
--rw-r--r--   0        0        0     8530 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/sitemap.py
--rw-r--r--   0        0        0     4131 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/slack_directory.py
--rw-r--r--   0        0        0     4799 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0     2004 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/spreedly.py
--rw-r--r--   0        0        0      851 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/srt.py
--rw-r--r--   0        0        0     1811 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/stripe.py
--rw-r--r--   0        0        0     9008 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/telegram.py
--rw-r--r--   0        0        0     1783 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0     1700 2024-01-03 17:13:53.990334 langchain_community-0.0.8/langchain_community/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0     3024 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0     2010 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/text.py
--rw-r--r--   0        0        0      950 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0     1572 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/toml.py
--rw-r--r--   0        0        0     6561 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/trello.py
--rw-r--r--   0        0        0     1293 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/tsv.py
--rw-r--r--   0        0        0     3438 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/twitter.py
--rw-r--r--   0        0        0    13793 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/unstructured.py
--rw-r--r--   0        0        0     6019 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/url.py
--rw-r--r--   0        0        0     7590 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/url_playwright.py
--rw-r--r--   0        0        0     6640 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/url_selenium.py
--rw-r--r--   0        0        0     1682 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/weather.py
--rw-r--r--   0        0        0    10164 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/web_base.py
--rw-r--r--   0        0        0     1770 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0     2142 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/wikipedia.py
--rw-r--r--   0        0        0     4583 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/word_document.py
--rw-r--r--   0        0        0     1489 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/xml.py
--rw-r--r--   0        0        0     1119 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/xorbits.py
--rw-r--r--   0        0        0    14798 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_loaders/youtube.py
--rw-r--r--   0        0        0     1849 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/__init__.py
--rw-r--r--   0        0        0     5214 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0     3463 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0     2155 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0     2331 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0     7882 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0     4133 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/google_translate.py
--rw-r--r--   0        0        0     1834 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/html2text.py
--rw-r--r--   0        0        0     1410 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0     1475 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0     6243 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     6033 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     6632 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/__init__.py
--rw-r--r--   0        0        0     9614 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0     1865 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/awa.py
--rw-r--r--   0        0        0     7063 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/azure_openai.py
--rw-r--r--   0        0        0     5201 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     6695 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/bedrock.py
--rw-r--r--   0        0        0     2725 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/bookend.py
--rw-r--r--   0        0        0     5454 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/clarifai.py
--rw-r--r--   0        0        0     2869 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0     4660 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/cohere.py
--rw-r--r--   0        0        0     5216 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/dashscope.py
--rw-r--r--   0        0        0     1310 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/databricks.py
--rw-r--r--   0        0        0     4426 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/deepinfra.py
--rw-r--r--   0        0        0     3671 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/edenai.py
--rw-r--r--   0        0        0     8401 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/elasticsearch.py
--rw-r--r--   0        0        0     5500 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/embaas.py
--rw-r--r--   0        0        0     4831 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/ernie.py
--rw-r--r--   0        0        0     1512 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/fake.py
--rw-r--r--   0        0        0     3452 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/fastembed.py
--rw-r--r--   0        0        0     3272 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/google_palm.py
--rw-r--r--   0        0        0     1664 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/gpt4all.py
--rw-r--r--   0        0        0     5274 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/gradient_ai.py
--rw-r--r--   0        0        0    11898 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/huggingface.py
--rw-r--r--   0        0        0     3789 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0    10260 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/infinity.py
--rw-r--r--   0        0        0     3673 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0     2607 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/jina.py
--rw-r--r--   0        0        0     2873 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0     4163 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/llamacpp.py
--rw-r--r--   0        0        0     2293 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/llm_rails.py
--rw-r--r--   0        0        0    12261 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/localai.py
--rw-r--r--   0        0        0     4798 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/minimax.py
--rw-r--r--   0        0        0     2417 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/mlflow.py
--rw-r--r--   0        0        0     2479 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0     2384 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0     5115 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/mosaicml.py
--rw-r--r--   0        0        0     2203 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/nlpcloud.py
--rw-r--r--   0        0        0     3420 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0     7691 2024-01-03 17:13:53.994334 langchain_community-0.0.8/langchain_community/embeddings/ollama.py
--rw-r--r--   0        0        0    29067 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/openai.py
--rw-r--r--   0        0        0     7591 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0     3807 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/self_hosted.py
--rw-r--r--   0        0        0     6589 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      189 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0     3743 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0     2413 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0    13929 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/vertexai.py
--rw-r--r--   0        0        0     4198 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/volcengine.py
--rw-r--r--   0        0        0     6255 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/voyageai.py
--rw-r--r--   0        0        0     3303 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/xinference.py
--rw-r--r--   0        0        0     5934 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/embeddings/yandex.py
--rw-r--r--   0        0        0      930 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/__init__.py
--rw-r--r--   0        0        0     6961 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/arangodb_graph.py
--rw-r--r--   0        0        0     5294 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/falkordb_graph.py
--rw-r--r--   0        0        0     1584 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/graph_document.py
--rw-r--r--   0        0        0     1008 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/graph_store.py
--rw-r--r--   0        0        0     2510 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/hugegraph.py
--rw-r--r--   0        0        0     4227 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/kuzu_graph.py
--rw-r--r--   0        0        0     1644 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/memgraph_graph.py
--rw-r--r--   0        0        0     8112 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/nebula_graph.py
--rw-r--r--   0        0        0     8388 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/neo4j_graph.py
--rw-r--r--   0        0        0     9398 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/neptune_graph.py
--rw-r--r--   0        0        0     6545 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/networkx_graph.py
--rw-r--r--   0        0        0    10118 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/graphs/rdf_graph.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/indexes/__init__.py
--rw-r--r--   0        0        0    20960 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0     5221 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/indexes/base.py
--rw-r--r--   0        0        0    23006 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/__init__.py
--rw-r--r--   0        0        0     5292 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/ai21.py
--rw-r--r--   0        0        0    11493 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/aleph_alpha.py
--rw-r--r--   0        0        0     3061 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0    12356 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/anthropic.py
--rw-r--r--   0        0        0    10630 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/anyscale.py
--rw-r--r--   0        0        0     9619 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/aphrodite.py
--rw-r--r--   0        0        0     4356 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/arcee.py
--rw-r--r--   0        0        0     6007 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/aviary.py
--rw-r--r--   0        0        0    10251 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/azureml_endpoint.py
--rw-r--r--   0        0        0     7603 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     4725 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/bananadev.py
--rw-r--r--   0        0        0     3187 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/baseten.py
--rw-r--r--   0        0        0     9099 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/beam.py
--rw-r--r--   0        0        0    15531 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/bedrock.py
--rw-r--r--   0        0        0     6232 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/bittensor.py
--rw-r--r--   0        0        0     4044 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/cerebriumai.py
--rw-r--r--   0        0        0     3969 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/chatglm.py
--rw-r--r--   0        0        0     7262 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/clarifai.py
--rw-r--r--   0        0        0     4277 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0     7970 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/cohere.py
--rw-r--r--   0        0        0     4227 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/ctransformers.py
--rw-r--r--   0        0        0     4135 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/ctranslate2.py
--rw-r--r--   0        0        0    17597 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/databricks.py
--rw-r--r--   0        0        0     7006 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/deepinfra.py
--rw-r--r--   0        0        0     8615 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/deepsparse.py
--rw-r--r--   0        0        0     9463 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/edenai.py
--rw-r--r--   0        0        0     2444 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/fake.py
--rw-r--r--   0        0        0    11773 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/fireworks.py
--rw-r--r--   0        0        0     3762 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/forefrontai.py
--rw-r--r--   0        0        0     8739 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/gigachat.py
--rw-r--r--   0        0        0     8854 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/google_palm.py
--rw-r--r--   0        0        0     5301 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/gooseai.py
--rw-r--r--   0        0        0     6525 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/gpt4all.py
--rw-r--r--   0        0        0    14199 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/grammars/list.gbnf
--rw-r--r--   0        0        0     5508 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0     4658 2024-01-03 17:13:53.998334 langchain_community-0.0.8/langchain_community/llms/huggingface_hub.py
--rw-r--r--   0        0        0     9215 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0    11403 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0     2582 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/human.py
--rw-r--r--   0        0        0     4723 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0     5087 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/koboldai.py
--rw-r--r--   0        0        0    12537 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/llamacpp.py
--rw-r--r--   0        0        0     1328 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/loading.py
--rw-r--r--   0        0        0     1965 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/manifest.py
--rw-r--r--   0        0        0     5470 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/minimax.py
--rw-r--r--   0        0        0     3466 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/mlflow.py
--rw-r--r--   0        0        0     3279 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0     3288 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/modal.py
--rw-r--r--   0        0        0     6150 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/mosaicml.py
--rw-r--r--   0        0        0     5049 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/nlpcloud.py
--rw-r--r--   0        0        0    12182 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/oci_data_science_model_deployment_endpoint.py
--rw-r--r--   0        0        0     5207 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/octoai_endpoint.py
--rw-r--r--   0        0        0    16101 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/ollama.py
--rw-r--r--   0        0        0     3980 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/opaqueprompts.py
--rw-r--r--   0        0        0    47378 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/openai.py
--rw-r--r--   0        0        0    10743 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/openllm.py
--rw-r--r--   0        0        0      902 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/openlm.py
--rw-r--r--   0        0        0     8059 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0     5402 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/petals.py
--rw-r--r--   0        0        0     4182 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/pipelineai.py
--rw-r--r--   0        0        0     1594 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/predibase.py
--rw-r--r--   0        0        0     4410 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/predictionguard.py
--rw-r--r--   0        0        0     8809 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/promptlayer_openai.py
--rw-r--r--   0        0        0     8024 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/replicate.py
--rw-r--r--   0        0        0     7387 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/rwkv.py
--rw-r--r--   0        0        0    13193 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0     7743 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/self_hosted.py
--rw-r--r--   0        0        0     7743 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0     4720 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/stochasticai.py
--rw-r--r--   0        0        0     7552 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/symblai_nebula.py
--rw-r--r--   0        0        0    14081 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/textgen.py
--rw-r--r--   0        0        0     5243 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/titan_takeoff.py
--rw-r--r--   0        0        0     7349 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/titan_takeoff_pro.py
--rw-r--r--   0        0        0     7526 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/together.py
--rw-r--r--   0        0        0    11318 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/tongyi.py
--rw-r--r--   0        0        0      258 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/utils.py
--rw-r--r--   0        0        0    18948 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/vertexai.py
--rw-r--r--   0        0        0     5592 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/vllm.py
--rw-r--r--   0        0        0     6591 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/volcengine_maas.py
--rw-r--r--   0        0        0    14918 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/watsonxllm.py
--rw-r--r--   0        0        0     4970 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/writer.py
--rw-r--r--   0        0        0     6325 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/xinference.py
--rw-r--r--   0        0        0    10797 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/llms/yandex.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/py.typed
--rw-r--r--   0        0        0     4245 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/__init__.py
--rw-r--r--   0        0        0     4328 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/arcee.py
--rw-r--r--   0        0        0      773 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/arxiv.py
--rw-r--r--   0        0        0     4279 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0     4691 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/bedrock.py
--rw-r--r--   0        0        0     3648 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/bm25.py
--rw-r--r--   0        0        0     2684 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/chaindesk.py
--rw-r--r--   0        0        0     3024 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0     2816 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2338 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/databerry.py
--rw-r--r--   0        0        0     6778 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/docarray.py
--rw-r--r--   0        0        0     4639 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0     2000 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/embedchain.py
--rw-r--r--   0        0        0     4583 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0    17552 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0     1985 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/kay.py
--rw-r--r--   0        0        0    13811 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/kendra.py
--rw-r--r--   0        0        0     2570 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/knn.py
--rw-r--r--   0        0        0     3162 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/llama_index.py
--rw-r--r--   0        0        0     1486 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/metal.py
--rw-r--r--   0        0        0     2435 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/milvus.py
--rw-r--r--   0        0        0      644 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/outline.py
--rw-r--r--   0        0        0     5733 2024-01-03 17:13:54.002334 langchain_community-0.0.8/langchain_community/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0      643 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/pubmed.py
--rw-r--r--   0        0        0      104 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/pupmed.py
--rw-r--r--   0        0        0     7468 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/qdrant_sparse_vector_retriever.py
--rw-r--r--   0        0        0     1935 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/remote_retriever.py
--rw-r--r--   0        0        0     4131 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/svm.py
--rw-r--r--   0        0        0     2855 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0     4079 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/tfidf.py
--rw-r--r--   0        0        0     4555 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0     6195 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0      656 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/wikipedia.py
--rw-r--r--   0        0        0     2356 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/you.py
--rw-r--r--   0        0        0     5904 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/zep.py
--rw-r--r--   0        0        0     2735 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/retrievers/zilliz.py
--rw-r--r--   0        0        0      501 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/storage/__init__.py
--rw-r--r--   0        0        0      179 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/storage/exceptions.py
--rw-r--r--   0        0        0     4788 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/storage/redis.py
--rw-r--r--   0        0        0     5764 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/storage/upstash_redis.py
--rw-r--r--   0        0        0    33542 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/__init__.py
--rw-r--r--   0        0        0     3185 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/app.py
--rw-r--r--   0        0        0     2109 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/base.py
--rw-r--r--   0        0        0     4140 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/owner.py
--rw-r--r--   0        0        0     2746 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/rule.py
--rw-r--r--   0        0        0     1074 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0     2314 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/utils.py
--rw-r--r--   0        0        0     2624 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ainetwork/value.py
--rw-r--r--   0        0        0      257 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/amadeus/__init__.py
--rw-r--r--   0        0        0      435 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/amadeus/base.py
--rw-r--r--   0        0        0     1845 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0     5611 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0     1276 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/amadeus/utils.py
--rw-r--r--   0        0        0       25 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/arxiv/__init__.py
--rw-r--r--   0        0        0     1228 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/arxiv/tool.py
--rw-r--r--   0        0        0      802 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0     5375 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0     5304 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0     4336 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0     3675 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0     3542 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      776 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/utils.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/bearly/__init__.py
--rw-r--r--   0        0        0     5468 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/bearly/tool.py
--rw-r--r--   0        0        0      170 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/bing_search/__init__.py
--rw-r--r--   0        0        0     1463 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/brave_search/__init__.py
--rw-r--r--   0        0        0     1354 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/brave_search/tool.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/clickup/__init__.py
--rw-r--r--   0        0        0     8298 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/clickup/prompt.py
--rw-r--r--   0        0        0     1230 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/clickup/tool.py
--rw-r--r--   0        0        0     1336 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/convert_to_openai.py
--rw-r--r--   0        0        0      268 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0     2214 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      147 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0     2641 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0     8015 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0    20701 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/e2b_data_analysis/unparse.py
--rw-r--r--   0        0        0     1024 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/__init__.py
--rw-r--r--   0        0        0     3465 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0     3885 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0     5386 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0     2249 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0     2476 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0     1966 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0     2187 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0     2407 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      164 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      203 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/eleven_labs/models.py
--rw-r--r--   0        0        0     2709 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0      723 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/__init__.py
--rw-r--r--   0        0        0     1749 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/copy.py
--rw-r--r--   0        0        0     1345 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/delete.py
--rw-r--r--   0        0        0     1965 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/file_search.py
--rw-r--r--   0        0        0     1432 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/list_dir.py
--rw-r--r--   0        0        0     1889 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/move.py
--rw-r--r--   0        0        0     1340 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/read.py
--rw-r--r--   0        0        0     1726 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/utils.py
--rw-r--r--   0        0        0     1614 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/github/__init__.py
--rw-r--r--   0        0        0     6220 2024-01-03 17:13:54.006334 langchain_community-0.0.8/langchain_community/tools/github/prompt.py
--rw-r--r--   0        0        0     1194 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/github/tool.py
--rw-r--r--   0        0        0       20 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gitlab/__init__.py
--rw-r--r--   0        0        0     3438 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gitlab/prompt.py
--rw-r--r--   0        0        0      972 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gitlab/tool.py
--rw-r--r--   0        0        0      601 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/__init__.py
--rw-r--r--   0        0        0     1004 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/base.py
--rw-r--r--   0        0        0     2564 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/create_draft.py
--rw-r--r--   0        0        0     2202 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/get_message.py
--rw-r--r--   0        0        0     1560 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/get_thread.py
--rw-r--r--   0        0        0     4874 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/search.py
--rw-r--r--   0        0        0     2939 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/send_message.py
--rw-r--r--   0        0        0     4528 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/gmail/utils.py
--rw-r--r--   0        0        0      136 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/golden_query/__init__.py
--rw-r--r--   0        0        0     1108 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/golden_query/tool.py
--rw-r--r--   0        0        0      171 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0     3173 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      152 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      854 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_finance/tool.py
--rw-r--r--   0        0        0      140 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      826 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      140 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      822 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_lens/tool.py
--rw-r--r--   0        0        0      140 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_places/__init__.py
--rw-r--r--   0        0        0     1141 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_places/tool.py
--rw-r--r--   0        0        0      152 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      847 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      195 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_search/__init__.py
--rw-r--r--   0        0        0     1489 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_search/tool.py
--rw-r--r--   0        0        0      243 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_serper/__init__.py
--rw-r--r--   0        0        0     2113 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_serper/tool.py
--rw-r--r--   0        0        0      148 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      844 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/graphql/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/graphql/tool.py
--rw-r--r--   0        0        0      132 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/human/__init__.py
--rw-r--r--   0        0        0      983 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/human/tool.py
--rw-r--r--   0        0        0     2286 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/ifttt.py
--rw-r--r--   0        0        0       43 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/interaction/__init__.py
--rw-r--r--   0        0        0      464 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/jira/__init__.py
--rw-r--r--   0        0        0     3170 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/jira/prompt.py
--rw-r--r--   0        0        0     1342 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/json/__init__.py
--rw-r--r--   0        0        0     4139 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/json/tool.py
--rw-r--r--   0        0        0      134 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/memorize/__init__.py
--rw-r--r--   0        0        0     1828 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      853 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      154 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0     2690 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      359 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/multion/__init__.py
--rw-r--r--   0        0        0     1751 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/multion/close_session.py
--rw-r--r--   0        0        0     2199 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/multion/create_session.py
--rw-r--r--   0        0        0     2401 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/nasa/__init__.py
--rw-r--r--   0        0        0     5197 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/nasa/prompt.py
--rw-r--r--   0        0        0      831 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/nasa/tool.py
--rw-r--r--   0        0        0      111 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/nuclia/__init__.py
--rw-r--r--   0        0        0     7915 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/nuclia/tool.py
--rw-r--r--   0        0        0      654 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/__init__.py
--rw-r--r--   0        0        0      508 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/base.py
--rw-r--r--   0        0        0     1858 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0     4833 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/events_search.py
--rw-r--r--   0        0        0     4246 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/messages_search.py
--rw-r--r--   0        0        0     2898 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/send_event.py
--rw-r--r--   0        0        0     1789 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/send_message.py
--rw-r--r--   0        0        0     2212 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/office365/utils.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0    21288 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      191 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      162 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      966 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      763 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/playwright/__init__.py
--rw-r--r--   0        0        0     2135 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/playwright/base.py
--rw-r--r--   0        0        0     3083 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/playwright/click.py
--rw-r--r--   0        0        0     1340 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/playwright/current_page.py
--rw-r--r--   0        0        0     3051 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0     2383 2024-01-03 17:13:54.010334 langchain_community-0.0.8/langchain_community/tools/playwright/extract_text.py
--rw-r--r--   0        0        0     3743 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/playwright/get_elements.py
--rw-r--r--   0        0        0     2878 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/playwright/navigate.py
--rw-r--r--   0        0        0     1926 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0     3049 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/playwright/utils.py
--rw-r--r--   0        0        0     2902 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/plugin.py
--rw-r--r--   0        0        0       52 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/powerbi/__init__.py
--rw-r--r--   0        0        0     7339 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/powerbi/prompt.py
--rw-r--r--   0        0        0    11075 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/pubmed/__init__.py
--rw-r--r--   0        0        0      944 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/pubmed/tool.py
--rw-r--r--   0        0        0     1965 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/reddit_search/tool.py
--rw-r--r--   0        0        0     1586 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/render.py
--rw-r--r--   0        0        0       52 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/requests/__init__.py
--rw-r--r--   0        0        0     6323 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/requests/tool.py
--rw-r--r--   0        0        0       31 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0     1100 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      214 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/searchapi/__init__.py
--rw-r--r--   0        0        0     2114 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/searx_search/__init__.py
--rw-r--r--   0        0        0     2261 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/searx_search/tool.py
--rw-r--r--   0        0        0       36 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/semanticscholar/__init__.py
--rw-r--r--   0        0        0     1190 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/semanticscholar/tool.py
--rw-r--r--   0        0        0      103 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/shell/__init__.py
--rw-r--r--   0        0        0     2266 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/shell/tool.py
--rw-r--r--   0        0        0      502 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/__init__.py
--rw-r--r--   0        0        0      460 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/base.py
--rw-r--r--   0        0        0     1118 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/get_channel.py
--rw-r--r--   0        0        0     1402 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/get_message.py
--rw-r--r--   0        0        0     2071 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/schedule_message.py
--rw-r--r--   0        0        0     1222 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/send_message.py
--rw-r--r--   0        0        0     1135 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/slack/utils.py
--rw-r--r--   0        0        0       18 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/sleep/__init__.py
--rw-r--r--   0        0        0     1229 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      550 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/spark_sql/prompt.py
--rw-r--r--   0        0        0     4376 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      597 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/sql_database/prompt.py
--rw-r--r--   0        0        0     4487 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      868 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/steam/__init__.py
--rw-r--r--   0        0        0     1657 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/steam/prompt.py
--rw-r--r--   0        0        0      842 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/steam/tool.py
--rw-r--r--   0        0        0      186 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0     3377 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0     1395 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/steamship_image_generation/utils.py
--rw-r--r--   0        0        0      189 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0     3375 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0     3302 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      867 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      156 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      887 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0     2473 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0        0 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/youtube/__init__.py
--rw-r--r--   0        0        0     1729 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/youtube/search.py
--rw-r--r--   0        0        0      193 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/zapier/__init__.py
--rw-r--r--   0        0        0     1182 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/zapier/prompt.py
--rw-r--r--   0        0        0     7730 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/tools/zapier/tool.py
--rw-r--r--   0        0        0    10998 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/__init__.py
--rw-r--r--   0        0        0     2192 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      844 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/anthropic.py
--rw-r--r--   0        0        0     8458 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/apify.py
--rw-r--r--   0        0        0     8710 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/arcee.py
--rw-r--r--   0        0        0     9262 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/arxiv.py
--rw-r--r--   0        0        0     2437 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/awslambda.py
--rw-r--r--   0        0        0     2499 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/bibtex.py
--rw-r--r--   0        0        0     3608 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/bing_search.py
--rw-r--r--   0        0        0     2356 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/brave_search.py
--rw-r--r--   0        0        0    19771 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/clickup.py
--rw-r--r--   0        0        0     6377 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0     7854 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0     4310 2024-01-03 17:13:54.014334 langchain_community-0.0.8/langchain_community/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0    32187 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/github.py
--rw-r--r--   0        0        0    11975 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/gitlab.py
--rw-r--r--   0        0        0     1858 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/golden_query.py
--rw-r--r--   0        0        0     3400 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_finance.py
--rw-r--r--   0        0        0     2804 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_jobs.py
--rw-r--r--   0        0        0     2859 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_lens.py
--rw-r--r--   0        0        0     4107 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_places_api.py
--rw-r--r--   0        0        0     5171 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_scholar.py
--rw-r--r--   0        0        0     5048 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_search.py
--rw-r--r--   0        0        0     6503 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_serper.py
--rw-r--r--   0        0        0     4033 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/google_trends.py
--rw-r--r--   0        0        0     1903 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/graphql.py
--rw-r--r--   0        0        0     6195 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/jira.py
--rw-r--r--   0        0        0     2647 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/max_compute.py
--rw-r--r--   0        0        0     3748 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/merriam_webster.py
--rw-r--r--   0        0        0     6809 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/metaphor_search.py
--rw-r--r--   0        0        0     1820 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/nasa.py
--rw-r--r--   0        0        0     3287 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/opaqueprompts.py
--rw-r--r--   0        0        0    11017 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/openapi.py
--rw-r--r--   0        0        0     2462 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/openweathermap.py
--rw-r--r--   0        0        0     3351 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/outline.py
--rw-r--r--   0        0        0     2355 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/portkey.py
--rw-r--r--   0        0        0    11246 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/powerbi.py
--rw-r--r--   0        0        0     6936 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/pubmed.py
--rw-r--r--   0        0        0     2159 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/python.py
--rw-r--r--   0        0        0     4474 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/reddit_search.py
--rw-r--r--   0        0        0     8221 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/redis.py
--rw-r--r--   0        0        0     6992 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/requests.py
--rw-r--r--   0        0        0     2220 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/scenexplain.py
--rw-r--r--   0        0        0     5226 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/searchapi.py
--rw-r--r--   0        0        0    16625 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/searx_search.py
--rw-r--r--   0        0        0     2789 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/semanticscholar.py
--rw-r--r--   0        0        0     8703 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/serpapi.py
--rw-r--r--   0        0        0     7519 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/spark_sql.py
--rw-r--r--   0        0        0    19752 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/sql_database.py
--rw-r--r--   0        0        0     2639 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/stackexchange.py
--rw-r--r--   0        0        0     5857 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/steam.py
--rw-r--r--   0        0        0     6834 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/tavily_search.py
--rw-r--r--   0        0        0     4006 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0     3441 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/twilio.py
--rw-r--r--   0        0        0     4072 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/vertexai.py
--rw-r--r--   0        0        0     4045 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/wikipedia.py
--rw-r--r--   0        0        0     2011 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0    11666 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utilities/zapier.py
--rw-r--r--   0        0        0       45 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utils/__init__.py
--rw-r--r--   0        0        0     1511 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utils/ernie_functions.py
--rw-r--r--   0        0        0     2713 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utils/math.py
--rw-r--r--   0        0        0      264 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utils/openai.py
--rw-r--r--   0        0        0     1518 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/utils/openai_functions.py
--rw-r--r--   0        0        0    16216 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/__init__.py
--rw-r--r--   0        0        0    19780 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0    15738 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/analyticdb.py
--rw-r--r--   0        0        0    16632 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/annoy.py
--rw-r--r--   0        0        0    28449 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/astradb.py
--rw-r--r--   0        0        0    12136 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/atlas.py
--rw-r--r--   0        0        0    21155 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/awadb.py
--rw-r--r--   0        0        0    14522 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0    27218 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/azuresearch.py
--rw-r--r--   0        0        0    15034 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/bageldb.py
--rw-r--r--   0        0        0    16548 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0    33082 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/bigquery_vector_search.py
--rw-r--r--   0        0        0    14809 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/cassandra.py
--rw-r--r--   0        0        0    30537 2024-01-03 17:13:54.018334 langchain_community-0.0.8/langchain_community/vectorstores/chroma.py
--rw-r--r--   0        0        0    10953 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/clarifai.py
--rw-r--r--   0        0        0    17735 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/clickhouse.py
--rw-r--r--   0        0        0    12713 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/dashvector.py
--rw-r--r--   0        0        0    18360 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0    40265 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/deeplake.py
--rw-r--r--   0        0        0    12973 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/dingo.py
--rw-r--r--   0        0        0      236 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0     6945 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/docarray/base.py
--rw-r--r--   0        0        0     4044 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0     2418 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0    28714 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0    46759 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0    14183 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/epsilla.py
--rw-r--r--   0        0        0    42920 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/faiss.py
--rw-r--r--   0        0        0    26837 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/hippo.py
--rw-r--r--   0        0        0    13642 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/hologres.py
--rw-r--r--   0        0        0    14234 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/jaguar.py
--rw-r--r--   0        0        0     4173 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/lancedb.py
--rw-r--r--   0        0        0     7745 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/llm_rails.py
--rw-r--r--   0        0        0    17047 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/marqo.py
--rw-r--r--   0        0        0    21430 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/matching_engine.py
--rw-r--r--   0        0        0    10400 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/meilisearch.py
--rw-r--r--   0        0        0    32968 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/milvus.py
--rw-r--r--   0        0        0    19047 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0    13869 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0    22546 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/myscale.py
--rw-r--r--   0        0        0    35000 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0     5403 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/nucliadb.py
--rw-r--r--   0        0        0    31850 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0    17895 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/pgembedding.py
--rw-r--r--   0        0        0     8891 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0    35925 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/pgvector.py
--rw-r--r--   0        0        0    17517 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/pinecone.py
--rw-r--r--   0        0        0    90569 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/qdrant.py
--rw-r--r--   0        0        0      265 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0    54458 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/redis/base.py
--rw-r--r--   0        0        0      420 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/redis/constants.py
--rw-r--r--   0        0        0    16227 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/redis/filters.py
--rw-r--r--   0        0        0    10419 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/redis/schema.py
--rw-r--r--   0        0        0    12192 2024-01-03 17:13:54.022334 langchain_community-0.0.8/langchain_community/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0    19610 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/scann.py
--rw-r--r--   0        0        0     9707 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/semadb.py
--rw-r--r--   0        0        0    17628 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0    12375 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/sklearn.py
--rw-r--r--   0        0        0     7316 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0    17150 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/starrocks.py
--rw-r--r--   0        0        0    15689 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/supabase.py
--rw-r--r--   0        0        0    14726 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/surrealdb.py
--rw-r--r--   0        0        0     9557 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/tair.py
--rw-r--r--   0        0        0    13927 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0     4927 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/tigris.py
--rw-r--r--   0        0        0    28826 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/tiledb.py
--rw-r--r--   0        0        0    29831 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/timescalevector.py
--rw-r--r--   0        0        0     9712 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/typesense.py
--rw-r--r--   0        0        0     5888 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/usearch.py
--rw-r--r--   0        0        0     2474 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/utils.py
--rw-r--r--   0        0        0    12908 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/vald.py
--rw-r--r--   0        0        0    19844 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/vearch.py
--rw-r--r--   0        0        0    21305 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/vectara.py
--rw-r--r--   0        0        0     9785 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/vespa.py
--rw-r--r--   0        0        0    19226 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/weaviate.py
--rw-r--r--   0        0        0     9032 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/xata.py
--rw-r--r--   0        0        0    10761 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0    23192 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/zep.py
--rw-r--r--   0        0        0     7575 2024-01-03 17:13:54.026334 langchain_community-0.0.8/langchain_community/vectorstores/zilliz.py
--rw-r--r--   0        0        0     9713 2024-01-03 17:13:54.026334 langchain_community-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7333 1970-01-01 00:00:00.000000 langchain_community-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1201 2024-01-06 00:18:17.246393 langchain_community-0.0.9/README.md
+-rw-r--r--   0        0        0      307 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/adapters/__init__.py
+-rw-r--r--   0        0        0    12143 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/adapters/openai.py
+-rw-r--r--   0        0        0     3327 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0     1781 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/amadeus/__init__.py
+-rw-r--r--   0        0        0      961 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0     1035 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0      397 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0     3594 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0     1091 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      177 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0     3250 2024-01-06 00:18:17.246393 langchain_community-0.0.9/langchain_community/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0    10135 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0     2904 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0     2045 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0     2227 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0     1894 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0     1819 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      595 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0     1190 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0     1931 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0     2038 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0     4228 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0     1812 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0     2870 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0    12987 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0    11686 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0     1743 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0     2557 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0     3317 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0      174 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0     4274 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0     2507 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0     2649 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     2773 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0     3771 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0       21 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0     1114 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0       23 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0     2355 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0     1202 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0     1084 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0     3866 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0     1428 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0     2862 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0     1465 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0     1095 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0     1933 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0    58301 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/cache.py
+-rw-r--r--   0        0        0     2671 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/__init__.py
+-rw-r--r--   0        0        0    14408 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/aim_callback.py
+-rw-r--r--   0        0        0    14820 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0     7438 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/arize_callback.py
+-rw-r--r--   0        0        0    11266 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0    18897 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0    23193 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0     6340 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/confident_callback.py
+-rw-r--r--   0        0        0     6498 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/context_callback.py
+-rw-r--r--   0        0        0    13138 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0     2587 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/human.py
+-rw-r--r--   0        0        0     9224 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/infino_callback.py
+-rw-r--r--   0        0        0    13880 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0    20527 2024-01-06 00:18:17.250393 langchain_community-0.0.9/langchain_community/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     1891 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/manager.py
+-rw-r--r--   0        0        0    24156 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0     7710 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/openai_info.py
+-rw-r--r--   0        0        0     5535 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0     8758 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0     3211 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0     5435 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0    15534 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      498 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0     4713 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0    19114 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0     4526 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0     8505 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/utils.py
+-rw-r--r--   0        0        0    20601 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0     8067 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0      452 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/__init__.py
+-rw-r--r--   0        0        0      444 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/base.py
+-rw-r--r--   0        0        0     2705 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0     4048 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/gmail.py
+-rw-r--r--   0        0        0     7910 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/imessage.py
+-rw-r--r--   0        0        0     5823 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0     3112 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/slack.py
+-rw-r--r--   0        0        0     5390 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/telegram.py
+-rw-r--r--   0        0        0     3270 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/utils.py
+-rw-r--r--   0        0        0     4280 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     2570 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0     4127 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0     2392 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0     6510 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0     5810 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0     6836 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0     1379 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/file.py
+-rw-r--r--   0        0        0     3349 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      633 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0     7112 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/momento.py
+-rw-r--r--   0        0        0     2734 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0     4288 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0     2659 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0     1971 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/redis.py
+-rw-r--r--   0        0        0     9515 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0    10331 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0     4717 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/sql.py
+-rw-r--r--   0        0        0     1176 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0     2148 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0     4652 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/xata.py
+-rw-r--r--   0        0        0     6452 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     3659 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/__init__.py
+-rw-r--r--   0        0        0     7963 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/anthropic.py
+-rw-r--r--   0        0        0     7945 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/anyscale.py
+-rw-r--r--   0        0        0    11324 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/azure_openai.py
+-rw-r--r--   0        0        0     6007 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0    10083 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/baichuan.py
+-rw-r--r--   0        0        0    12777 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     4284 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/bedrock.py
+-rw-r--r--   0        0        0     7571 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/cohere.py
+-rw-r--r--   0        0        0     1250 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/databricks.py
+-rw-r--r--   0        0        0     7874 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/ernie.py
+-rw-r--r--   0        0        0     5586 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/everlyai.py
+-rw-r--r--   0        0        0     3217 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/fake.py
+-rw-r--r--   0        0        0    11742 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/fireworks.py
+-rw-r--r--   0        0        0     6312 2024-01-06 00:18:17.254393 langchain_community-0.0.9/langchain_community/chat_models/gigachat.py
+-rw-r--r--   0        0        0    11608 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/google_palm.py
+-rw-r--r--   0        0        0    12859 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/gpt_router.py
+-rw-r--r--   0        0        0     5549 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/huggingface.py
+-rw-r--r--   0        0        0     3698 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/human.py
+-rw-r--r--   0        0        0    10549 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/hunyuan.py
+-rw-r--r--   0        0        0     7654 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0    15167 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/jinachat.py
+-rw-r--r--   0        0        0    10992 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/konko.py
+-rw-r--r--   0        0        0    15710 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/litellm.py
+-rw-r--r--   0        0        0      967 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/meta.py
+-rw-r--r--   0        0        0     3180 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/minimax.py
+-rw-r--r--   0        0        0     6908 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/mlflow.py
+-rw-r--r--   0        0        0     6737 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0    13160 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/ollama.py
+-rw-r--r--   0        0        0    26722 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/openai.py
+-rw-r--r--   0        0        0    10376 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0     5261 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0    14261 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/tongyi.py
+-rw-r--r--   0        0        0    14385 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/vertexai.py
+-rw-r--r--   0        0        0     5119 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0     5054 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/wasm_chat.py
+-rw-r--r--   0        0        0     9392 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/yandex.py
+-rw-r--r--   0        0        0    11166 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/chat_models/zhipuai.py
+-rw-r--r--   0        0        0      549 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/docstore/__init__.py
+-rw-r--r--   0        0        0     1090 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      833 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/docstore/base.py
+-rw-r--r--   0        0        0       70 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/docstore/document.py
+-rw-r--r--   0        0        0     1610 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/docstore/in_memory.py
+-rw-r--r--   0        0        0     1487 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/docstore/wikipedia.py
+-rw-r--r--   0        0        0    16095 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2841 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/acreom.py
+-rw-r--r--   0        0        0    10240 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      815 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0     1281 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/airtable.py
+-rw-r--r--   0        0        0     2759 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0     5272 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0      879 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/arxiv.py
+-rw-r--r--   0        0        0     4218 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0     3454 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/astradb.py
+-rw-r--r--   0        0        0     8129 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/async_html.py
+-rw-r--r--   0        0        0      563 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0     1545 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0     1582 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0     1644 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0     1857 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0     1931 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0     3175 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/base.py
+-rw-r--r--   0        0        0     6992 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/base_o365.py
+-rw-r--r--   0        0        0     3922 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/bibtex.py
+-rw-r--r--   0        0        0     3673 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/bigquery.py
+-rw-r--r--   0        0        0     2736 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/bilibili.py
+-rw-r--r--   0        0        0    10302 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      374 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0     5340 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0     6636 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0     1526 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0     5709 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/blockchain.py
+-rw-r--r--   0        0        0     1047 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/brave_search.py
+-rw-r--r--   0        0        0     2124 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/browserless.py
+-rw-r--r--   0        0        0     1986 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0     2746 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/chromium.py
+-rw-r--r--   0        0        0      527 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0     3269 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/concurrent.py
+-rw-r--r--   0        0        0    27612 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/confluence.py
+-rw-r--r--   0        0        0     1052 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/conllu.py
+-rw-r--r--   0        0        0     3649 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/couchbase.py
+-rw-r--r--   0        0        0     5926 2024-01-06 00:18:17.258393 langchain_community-0.0.9/langchain_community/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0     6617 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0     4937 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0     1923 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/dataframe.py
+-rw-r--r--   0        0        0     2054 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/diffbot.py
+-rw-r--r--   0        0        0     5942 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/directory.py
+-rw-r--r--   0        0        0     1237 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/discord.py
+-rw-r--r--   0        0        0     3146 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/doc_intelligence.py
+-rw-r--r--   0        0        0    13450 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/docugami.py
+-rw-r--r--   0        0        0     1852 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0     6229 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/dropbox.py
+-rw-r--r--   0        0        0     3150 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0     3834 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/email.py
+-rw-r--r--   0        0        0     1496 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/epub.py
+-rw-r--r--   0        0        0     7798 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/etherscan.py
+-rw-r--r--   0        0        0     5757 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/evernote.py
+-rw-r--r--   0        0        0     1687 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/excel.py
+-rw-r--r--   0        0        0     1270 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0     2254 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/fauna.py
+-rw-r--r--   0        0        0     1543 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/figma.py
+-rw-r--r--   0        0        0     2118 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0     3138 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0     6390 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/generic.py
+-rw-r--r--   0        0        0     2518 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0     4116 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/git.py
+-rw-r--r--   0        0        0     3453 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/gitbook.py
+-rw-r--r--   0        0        0     6973 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/github.py
+-rw-r--r--   0        0        0     5096 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0    14225 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      928 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0     1557 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/helpers.py
+-rw-r--r--   0        0        0     2075 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/hn.py
+-rw-r--r--   0        0        0     1158 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/html.py
+-rw-r--r--   0        0        0     2045 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/html_bs.py
+-rw-r--r--   0        0        0     3208 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0     7642 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/ifixit.py
+-rw-r--r--   0        0        0     1173 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/image.py
+-rw-r--r--   0        0        0     3594 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      477 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/imsdb.py
+-rw-r--r--   0        0        0     1688 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/iugu.py
+-rw-r--r--   0        0        0     3705 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/joplin.py
+-rw-r--r--   0        0        0     5907 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/json_loader.py
+-rw-r--r--   0        0        0     6058 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/lakefs.py
+-rw-r--r--   0        0        0     2008 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/larksuite.py
+-rw-r--r--   0        0        0     1818 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/markdown.py
+-rw-r--r--   0        0        0     3112 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/mastodon.py
+-rw-r--r--   0        0        0     3282 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/max_compute.py
+-rw-r--r--   0        0        0     3918 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      846 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/merge.py
+-rw-r--r--   0        0        0     2540 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/mhtml.py
+-rw-r--r--   0        0        0     3074 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0     2522 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/mongodb.py
+-rw-r--r--   0        0        0     4296 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/news.py
+-rw-r--r--   0        0        0     4301 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/notebook.py
+-rw-r--r--   0        0        0      814 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/notion.py
+-rw-r--r--   0        0        0     6718 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/notiondb.py
+-rw-r--r--   0        0        0     1088 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/nuclia.py
+-rw-r--r--   0        0        0     3593 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0     4768 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/obs_file.py
+-rw-r--r--   0        0        0     6150 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/obsidian.py
+-rw-r--r--   0        0        0     1770 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/odt.py
+-rw-r--r--   0        0        0     3381 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/onedrive.py
+-rw-r--r--   0        0        0     1154 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0     8074 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/onenote.py
+-rw-r--r--   0        0        0     1331 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0     1748 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/org_mode.py
+-rw-r--r--   0        0        0      947 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0    10716 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0     4534 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/doc_intelligence.py
+-rw-r--r--   0        0        0    15283 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0     2502 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0     5767 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      109 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0     1609 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      136 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0     3745 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      495 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0     2103 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0     5114 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0     1679 2024-01-06 00:18:17.262393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0     1664 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0    21036 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0     1214 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      505 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0    26024 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/pdf.py
+-rw-r--r--   0        0        0     1161 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0     2508 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0     1371 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/psychic.py
+-rw-r--r--   0        0        0     1172 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/pubmed.py
+-rw-r--r--   0        0        0     3388 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      527 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/python.py
+-rw-r--r--   0        0        0     8426 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/quip.py
+-rw-r--r--   0        0        0     6928 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0    11591 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0     4584 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/reddit.py
+-rw-r--r--   0        0        0      705 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/roam.py
+-rw-r--r--   0        0        0     4604 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0     4936 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/rspace.py
+-rw-r--r--   0        0        0     4895 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/rss.py
+-rw-r--r--   0        0        0     1832 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/rst.py
+-rw-r--r--   0        0        0     2061 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/rtf.py
+-rw-r--r--   0        0        0     5759 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0     5412 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/s3_file.py
+-rw-r--r--   0        0        0     2318 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0     8530 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/sitemap.py
+-rw-r--r--   0        0        0     4131 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0     4799 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0     2004 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/spreedly.py
+-rw-r--r--   0        0        0      851 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/srt.py
+-rw-r--r--   0        0        0     1811 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/stripe.py
+-rw-r--r--   0        0        0     9008 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/telegram.py
+-rw-r--r--   0        0        0     1783 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0     1700 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0     3024 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0     2010 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/text.py
+-rw-r--r--   0        0        0      950 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0     1572 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/toml.py
+-rw-r--r--   0        0        0     6561 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/trello.py
+-rw-r--r--   0        0        0     1293 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/tsv.py
+-rw-r--r--   0        0        0     3438 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/twitter.py
+-rw-r--r--   0        0        0    13793 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/unstructured.py
+-rw-r--r--   0        0        0     6019 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/url.py
+-rw-r--r--   0        0        0     7590 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0     6640 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0     1682 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/weather.py
+-rw-r--r--   0        0        0    10164 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/web_base.py
+-rw-r--r--   0        0        0     1770 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0     2142 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0     4583 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/word_document.py
+-rw-r--r--   0        0        0     1489 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/xml.py
+-rw-r--r--   0        0        0     1119 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/xorbits.py
+-rw-r--r--   0        0        0    14798 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_loaders/youtube.py
+-rw-r--r--   0        0        0     1849 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/__init__.py
+-rw-r--r--   0        0        0     5214 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0     3463 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0     2155 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0     2331 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     7882 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0     4133 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/google_translate.py
+-rw-r--r--   0        0        0     1834 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/html2text.py
+-rw-r--r--   0        0        0     1410 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0     1475 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0     6243 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     6033 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     6632 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/__init__.py
+-rw-r--r--   0        0        0     9614 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0     1865 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/awa.py
+-rw-r--r--   0        0        0     7222 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/azure_openai.py
+-rw-r--r--   0        0        0     5201 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     6695 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/bedrock.py
+-rw-r--r--   0        0        0     2725 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/bookend.py
+-rw-r--r--   0        0        0     5454 2024-01-06 00:18:17.266393 langchain_community-0.0.9/langchain_community/embeddings/clarifai.py
+-rw-r--r--   0        0        0     2869 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0     4660 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/cohere.py
+-rw-r--r--   0        0        0     5216 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/dashscope.py
+-rw-r--r--   0        0        0     1310 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/databricks.py
+-rw-r--r--   0        0        0     4426 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/deepinfra.py
+-rw-r--r--   0        0        0     3671 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/edenai.py
+-rw-r--r--   0        0        0     8401 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0     5500 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/embaas.py
+-rw-r--r--   0        0        0     4831 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/ernie.py
+-rw-r--r--   0        0        0     1512 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/fake.py
+-rw-r--r--   0        0        0     3452 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/fastembed.py
+-rw-r--r--   0        0        0     3272 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/google_palm.py
+-rw-r--r--   0        0        0     1664 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/gpt4all.py
+-rw-r--r--   0        0        0     5274 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0    11898 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/huggingface.py
+-rw-r--r--   0        0        0     3789 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0    10260 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/infinity.py
+-rw-r--r--   0        0        0     3673 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0     2607 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/jina.py
+-rw-r--r--   0        0        0     2873 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0     4163 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/llamacpp.py
+-rw-r--r--   0        0        0     2293 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/llm_rails.py
+-rw-r--r--   0        0        0    12261 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/localai.py
+-rw-r--r--   0        0        0     4798 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/minimax.py
+-rw-r--r--   0        0        0     2417 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/mlflow.py
+-rw-r--r--   0        0        0     2479 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0     2384 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0     5115 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/mosaicml.py
+-rw-r--r--   0        0        0     2203 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0     3420 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0     7691 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/ollama.py
+-rw-r--r--   0        0        0    29230 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/openai.py
+-rw-r--r--   0        0        0     7591 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     3807 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/self_hosted.py
+-rw-r--r--   0        0        0     6589 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      189 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0     3743 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0     2413 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0    13929 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/vertexai.py
+-rw-r--r--   0        0        0     4198 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/volcengine.py
+-rw-r--r--   0        0        0     6255 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/voyageai.py
+-rw-r--r--   0        0        0     3303 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/xinference.py
+-rw-r--r--   0        0        0     5934 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/embeddings/yandex.py
+-rw-r--r--   0        0        0      930 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/__init__.py
+-rw-r--r--   0        0        0     6961 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0     5294 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0     1584 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/graph_document.py
+-rw-r--r--   0        0        0     1008 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/graph_store.py
+-rw-r--r--   0        0        0     2510 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/hugegraph.py
+-rw-r--r--   0        0        0     4227 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0     1644 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0     8112 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/nebula_graph.py
+-rw-r--r--   0        0        0     8388 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0     9398 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/neptune_graph.py
+-rw-r--r--   0        0        0     6545 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/networkx_graph.py
+-rw-r--r--   0        0        0    10118 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/graphs/rdf_graph.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/indexes/__init__.py
+-rw-r--r--   0        0        0    20960 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0     5221 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/indexes/base.py
+-rw-r--r--   0        0        0    23006 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/llms/__init__.py
+-rw-r--r--   0        0        0     5292 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/llms/ai21.py
+-rw-r--r--   0        0        0    11493 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/llms/aleph_alpha.py
+-rw-r--r--   0        0        0     3061 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0    12356 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/llms/anthropic.py
+-rw-r--r--   0        0        0    10630 2024-01-06 00:18:17.270393 langchain_community-0.0.9/langchain_community/llms/anyscale.py
+-rw-r--r--   0        0        0     9619 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/aphrodite.py
+-rw-r--r--   0        0        0     4356 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/arcee.py
+-rw-r--r--   0        0        0     6007 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/aviary.py
+-rw-r--r--   0        0        0    10251 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0     7603 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     4725 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/bananadev.py
+-rw-r--r--   0        0        0     3187 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/baseten.py
+-rw-r--r--   0        0        0     9099 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/beam.py
+-rw-r--r--   0        0        0    15531 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/bedrock.py
+-rw-r--r--   0        0        0     6232 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/bittensor.py
+-rw-r--r--   0        0        0     4044 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/cerebriumai.py
+-rw-r--r--   0        0        0     3969 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/chatglm.py
+-rw-r--r--   0        0        0     7262 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/clarifai.py
+-rw-r--r--   0        0        0     4277 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0     7970 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/cohere.py
+-rw-r--r--   0        0        0     4227 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/ctransformers.py
+-rw-r--r--   0        0        0     4135 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/ctranslate2.py
+-rw-r--r--   0        0        0    17597 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/databricks.py
+-rw-r--r--   0        0        0     7006 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/deepinfra.py
+-rw-r--r--   0        0        0     8615 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/deepsparse.py
+-rw-r--r--   0        0        0     9463 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/edenai.py
+-rw-r--r--   0        0        0     2444 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/fake.py
+-rw-r--r--   0        0        0    11773 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/fireworks.py
+-rw-r--r--   0        0        0     3762 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/forefrontai.py
+-rw-r--r--   0        0        0     8739 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/gigachat.py
+-rw-r--r--   0        0        0     8854 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/google_palm.py
+-rw-r--r--   0        0        0     5301 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/gooseai.py
+-rw-r--r--   0        0        0     6525 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/gpt4all.py
+-rw-r--r--   0        0        0    14199 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0     5508 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0     4658 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/huggingface_hub.py
+-rw-r--r--   0        0        0     9215 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0    11403 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0     2582 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/human.py
+-rw-r--r--   0        0        0     4723 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0     5087 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/koboldai.py
+-rw-r--r--   0        0        0    12537 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/llamacpp.py
+-rw-r--r--   0        0        0     1328 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/loading.py
+-rw-r--r--   0        0        0     1965 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/manifest.py
+-rw-r--r--   0        0        0     5470 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/minimax.py
+-rw-r--r--   0        0        0     3466 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/mlflow.py
+-rw-r--r--   0        0        0     3279 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0     3288 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/modal.py
+-rw-r--r--   0        0        0     6150 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/mosaicml.py
+-rw-r--r--   0        0        0     5049 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/nlpcloud.py
+-rw-r--r--   0        0        0    12182 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/oci_data_science_model_deployment_endpoint.py
+-rw-r--r--   0        0        0     5207 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0    16101 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/ollama.py
+-rw-r--r--   0        0        0     3980 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/opaqueprompts.py
+-rw-r--r--   0        0        0    47691 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/openai.py
+-rw-r--r--   0        0        0    10743 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/openllm.py
+-rw-r--r--   0        0        0      902 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/openlm.py
+-rw-r--r--   0        0        0     8059 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0     5402 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/petals.py
+-rw-r--r--   0        0        0     4182 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/pipelineai.py
+-rw-r--r--   0        0        0     1594 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/predibase.py
+-rw-r--r--   0        0        0     4410 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/predictionguard.py
+-rw-r--r--   0        0        0     8809 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0     8024 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/replicate.py
+-rw-r--r--   0        0        0     7387 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/rwkv.py
+-rw-r--r--   0        0        0    13193 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     7743 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/self_hosted.py
+-rw-r--r--   0        0        0     7743 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0     4720 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/stochasticai.py
+-rw-r--r--   0        0        0     7552 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/symblai_nebula.py
+-rw-r--r--   0        0        0    14081 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/textgen.py
+-rw-r--r--   0        0        0     5243 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/titan_takeoff.py
+-rw-r--r--   0        0        0     7349 2024-01-06 00:18:17.274393 langchain_community-0.0.9/langchain_community/llms/titan_takeoff_pro.py
+-rw-r--r--   0        0        0     7526 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/together.py
+-rw-r--r--   0        0        0    11318 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/tongyi.py
+-rw-r--r--   0        0        0      258 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/utils.py
+-rw-r--r--   0        0        0    18948 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/vertexai.py
+-rw-r--r--   0        0        0     5592 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/vllm.py
+-rw-r--r--   0        0        0     6591 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/volcengine_maas.py
+-rw-r--r--   0        0        0    14918 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/watsonxllm.py
+-rw-r--r--   0        0        0     4970 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/writer.py
+-rw-r--r--   0        0        0     6325 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/xinference.py
+-rw-r--r--   0        0        0    10797 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/llms/yandex.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/py.typed
+-rw-r--r--   0        0        0     4245 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/__init__.py
+-rw-r--r--   0        0        0     4328 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/arcee.py
+-rw-r--r--   0        0        0      773 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/arxiv.py
+-rw-r--r--   0        0        0     4279 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/azure_cognitive_search.py
+-rw-r--r--   0        0        0     4691 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/bedrock.py
+-rw-r--r--   0        0        0     3648 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/bm25.py
+-rw-r--r--   0        0        0     2684 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/chaindesk.py
+-rw-r--r--   0        0        0     3024 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0     2816 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2338 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/databerry.py
+-rw-r--r--   0        0        0     6778 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/docarray.py
+-rw-r--r--   0        0        0     4639 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0     2000 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/embedchain.py
+-rw-r--r--   0        0        0     4583 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0    17552 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0     1985 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/kay.py
+-rw-r--r--   0        0        0    13811 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/kendra.py
+-rw-r--r--   0        0        0     2570 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/knn.py
+-rw-r--r--   0        0        0     3162 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/llama_index.py
+-rw-r--r--   0        0        0     1486 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/metal.py
+-rw-r--r--   0        0        0     2435 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/milvus.py
+-rw-r--r--   0        0        0      644 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/outline.py
+-rw-r--r--   0        0        0     5733 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      643 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/pubmed.py
+-rw-r--r--   0        0        0      104 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/pupmed.py
+-rw-r--r--   0        0        0     7468 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/qdrant_sparse_vector_retriever.py
+-rw-r--r--   0        0        0     1935 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0     4131 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/svm.py
+-rw-r--r--   0        0        0     2855 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0     4079 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/tfidf.py
+-rw-r--r--   0        0        0     4555 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0     6195 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0      656 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/wikipedia.py
+-rw-r--r--   0        0        0     2356 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/you.py
+-rw-r--r--   0        0        0     5904 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/zep.py
+-rw-r--r--   0        0        0     2735 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/retrievers/zilliz.py
+-rw-r--r--   0        0        0      501 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/storage/__init__.py
+-rw-r--r--   0        0        0      179 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/storage/exceptions.py
+-rw-r--r--   0        0        0     4788 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/storage/redis.py
+-rw-r--r--   0        0        0     5764 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/storage/upstash_redis.py
+-rw-r--r--   0        0        0    33542 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/__init__.py
+-rw-r--r--   0        0        0     3185 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/app.py
+-rw-r--r--   0        0        0     2109 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/base.py
+-rw-r--r--   0        0        0     4140 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0     2746 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0     1074 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0     2314 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/utils.py
+-rw-r--r--   0        0        0     2624 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      257 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      435 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/amadeus/base.py
+-rw-r--r--   0        0        0     1845 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0     5611 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0     1276 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/amadeus/utils.py
+-rw-r--r--   0        0        0       25 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0     1228 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      802 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0     5375 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0     5304 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0     4336 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0     3675 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0     3542 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      776 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/utils.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/bearly/__init__.py
+-rw-r--r--   0        0        0     5468 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/bearly/tool.py
+-rw-r--r--   0        0        0      170 2024-01-06 00:18:17.278393 langchain_community-0.0.9/langchain_community/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0     1463 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0     1354 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/brave_search/tool.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/clickup/__init__.py
+-rw-r--r--   0        0        0     8298 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/clickup/prompt.py
+-rw-r--r--   0        0        0     1230 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/clickup/tool.py
+-rw-r--r--   0        0        0     1336 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      268 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0     2214 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      147 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     2641 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0     8015 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0    20701 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/e2b_data_analysis/unparse.py
+-rw-r--r--   0        0        0     1024 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/__init__.py
+-rw-r--r--   0        0        0     3465 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0     3885 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0     5386 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0     2249 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0     2476 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0     1966 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0     2187 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0     2407 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      164 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      203 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0     2709 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0      723 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/__init__.py
+-rw-r--r--   0        0        0     1749 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/copy.py
+-rw-r--r--   0        0        0     1345 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/delete.py
+-rw-r--r--   0        0        0     1965 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/file_search.py
+-rw-r--r--   0        0        0     1432 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0     1889 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/move.py
+-rw-r--r--   0        0        0     1340 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/read.py
+-rw-r--r--   0        0        0     1726 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/utils.py
+-rw-r--r--   0        0        0     1614 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/github/__init__.py
+-rw-r--r--   0        0        0     6220 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/github/prompt.py
+-rw-r--r--   0        0        0     1194 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/github/tool.py
+-rw-r--r--   0        0        0       20 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0     3438 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gitlab/prompt.py
+-rw-r--r--   0        0        0      972 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gitlab/tool.py
+-rw-r--r--   0        0        0      601 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/__init__.py
+-rw-r--r--   0        0        0     1004 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/base.py
+-rw-r--r--   0        0        0     2564 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0     2202 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/get_message.py
+-rw-r--r--   0        0        0     1560 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0     4874 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/search.py
+-rw-r--r--   0        0        0     2939 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/send_message.py
+-rw-r--r--   0        0        0     4528 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/gmail/utils.py
+-rw-r--r--   0        0        0      136 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0     1108 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      171 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0     3173 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      152 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      854 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      140 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      826 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      140 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      822 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      140 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_places/__init__.py
+-rw-r--r--   0        0        0     1141 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_places/tool.py
+-rw-r--r--   0        0        0      152 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      847 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      195 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_search/__init__.py
+-rw-r--r--   0        0        0     1489 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_search/tool.py
+-rw-r--r--   0        0        0      243 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0     2113 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      148 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      844 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/graphql/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/graphql/tool.py
+-rw-r--r--   0        0        0      132 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/human/__init__.py
+-rw-r--r--   0        0        0      983 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/human/tool.py
+-rw-r--r--   0        0        0     2286 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      464 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/jira/__init__.py
+-rw-r--r--   0        0        0     3170 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/jira/prompt.py
+-rw-r--r--   0        0        0     1342 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2024-01-06 00:18:17.282393 langchain_community-0.0.9/langchain_community/tools/json/__init__.py
+-rw-r--r--   0        0        0     4139 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/json/tool.py
+-rw-r--r--   0        0        0      134 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/memorize/__init__.py
+-rw-r--r--   0        0        0     1828 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      853 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      154 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0     2690 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0      359 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/multion/__init__.py
+-rw-r--r--   0        0        0     1751 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/multion/close_session.py
+-rw-r--r--   0        0        0     2199 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/multion/create_session.py
+-rw-r--r--   0        0        0     2401 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/nasa/__init__.py
+-rw-r--r--   0        0        0     5197 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/nasa/prompt.py
+-rw-r--r--   0        0        0      831 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/nasa/tool.py
+-rw-r--r--   0        0        0      111 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0     7915 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      654 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/__init__.py
+-rw-r--r--   0        0        0      508 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/base.py
+-rw-r--r--   0        0        0     1858 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0     4833 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/events_search.py
+-rw-r--r--   0        0        0     4246 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/messages_search.py
+-rw-r--r--   0        0        0     2898 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/send_event.py
+-rw-r--r--   0        0        0     1789 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/send_message.py
+-rw-r--r--   0        0        0     2212 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/office365/utils.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0    21288 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      191 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      162 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      966 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      763 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/__init__.py
+-rw-r--r--   0        0        0     2135 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/base.py
+-rw-r--r--   0        0        0     3083 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/click.py
+-rw-r--r--   0        0        0     1340 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/current_page.py
+-rw-r--r--   0        0        0     3051 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0     2383 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0     3743 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0     2878 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/navigate.py
+-rw-r--r--   0        0        0     1926 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0     3049 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/playwright/utils.py
+-rw-r--r--   0        0        0     2902 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/plugin.py
+-rw-r--r--   0        0        0       52 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0     7339 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/powerbi/prompt.py
+-rw-r--r--   0        0        0    11075 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0      944 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/pubmed/tool.py
+-rw-r--r--   0        0        0     1965 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0     1586 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/render.py
+-rw-r--r--   0        0        0       52 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/requests/__init__.py
+-rw-r--r--   0        0        0     6323 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/requests/tool.py
+-rw-r--r--   0        0        0       31 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0     1100 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      214 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0     2114 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0     2261 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/searx_search/tool.py
+-rw-r--r--   0        0        0       36 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/semanticscholar/__init__.py
+-rw-r--r--   0        0        0     1190 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/semanticscholar/tool.py
+-rw-r--r--   0        0        0      103 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/shell/__init__.py
+-rw-r--r--   0        0        0     2266 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/shell/tool.py
+-rw-r--r--   0        0        0      502 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/__init__.py
+-rw-r--r--   0        0        0      460 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/base.py
+-rw-r--r--   0        0        0     1118 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/get_channel.py
+-rw-r--r--   0        0        0     1402 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/get_message.py
+-rw-r--r--   0        0        0     2071 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0     1222 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/send_message.py
+-rw-r--r--   0        0        0     1135 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/slack/utils.py
+-rw-r--r--   0        0        0       18 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/sleep/__init__.py
+-rw-r--r--   0        0        0     1229 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      550 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/spark_sql/prompt.py
+-rw-r--r--   0        0        0     4376 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      597 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     4487 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      868 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/steam/__init__.py
+-rw-r--r--   0        0        0     1657 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/steam/prompt.py
+-rw-r--r--   0        0        0      842 2024-01-06 00:18:17.286394 langchain_community-0.0.9/langchain_community/tools/steam/tool.py
+-rw-r--r--   0        0        0      186 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0     3377 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0     1395 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/steamship_image_generation/utils.py
+-rw-r--r--   0        0        0      189 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0     3375 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0     3302 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      867 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      156 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      887 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0     2473 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0        0 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/youtube/__init__.py
+-rw-r--r--   0        0        0     1729 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/youtube/search.py
+-rw-r--r--   0        0        0      193 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/zapier/__init__.py
+-rw-r--r--   0        0        0     1182 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/zapier/prompt.py
+-rw-r--r--   0        0        0     7730 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/tools/zapier/tool.py
+-rw-r--r--   0        0        0    10998 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/__init__.py
+-rw-r--r--   0        0        0     2192 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      844 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/anthropic.py
+-rw-r--r--   0        0        0     8458 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/apify.py
+-rw-r--r--   0        0        0     8710 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/arcee.py
+-rw-r--r--   0        0        0     9262 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/arxiv.py
+-rw-r--r--   0        0        0     2437 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/awslambda.py
+-rw-r--r--   0        0        0     2499 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/bibtex.py
+-rw-r--r--   0        0        0     3608 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/bing_search.py
+-rw-r--r--   0        0        0     2356 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/brave_search.py
+-rw-r--r--   0        0        0    19771 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/clickup.py
+-rw-r--r--   0        0        0     6377 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0     7854 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0     4310 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0    32187 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/github.py
+-rw-r--r--   0        0        0    11975 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/gitlab.py
+-rw-r--r--   0        0        0     1858 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/golden_query.py
+-rw-r--r--   0        0        0     3400 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_finance.py
+-rw-r--r--   0        0        0     2804 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_jobs.py
+-rw-r--r--   0        0        0     2859 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_lens.py
+-rw-r--r--   0        0        0     4107 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_places_api.py
+-rw-r--r--   0        0        0     5171 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_scholar.py
+-rw-r--r--   0        0        0     5048 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_search.py
+-rw-r--r--   0        0        0     6503 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_serper.py
+-rw-r--r--   0        0        0     4033 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/google_trends.py
+-rw-r--r--   0        0        0     1903 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/graphql.py
+-rw-r--r--   0        0        0     6195 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/jira.py
+-rw-r--r--   0        0        0     2647 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/max_compute.py
+-rw-r--r--   0        0        0     3748 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/merriam_webster.py
+-rw-r--r--   0        0        0     6809 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/metaphor_search.py
+-rw-r--r--   0        0        0     1820 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/nasa.py
+-rw-r--r--   0        0        0     3287 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0    11017 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/openapi.py
+-rw-r--r--   0        0        0     2462 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/openweathermap.py
+-rw-r--r--   0        0        0     3351 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/outline.py
+-rw-r--r--   0        0        0     2355 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/portkey.py
+-rw-r--r--   0        0        0    11246 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/powerbi.py
+-rw-r--r--   0        0        0     6936 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/pubmed.py
+-rw-r--r--   0        0        0     2159 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/python.py
+-rw-r--r--   0        0        0     4474 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/reddit_search.py
+-rw-r--r--   0        0        0     8221 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/redis.py
+-rw-r--r--   0        0        0     6992 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/requests.py
+-rw-r--r--   0        0        0     2220 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/scenexplain.py
+-rw-r--r--   0        0        0     5226 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/searchapi.py
+-rw-r--r--   0        0        0    16625 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/searx_search.py
+-rw-r--r--   0        0        0     2789 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/semanticscholar.py
+-rw-r--r--   0        0        0     8703 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/serpapi.py
+-rw-r--r--   0        0        0     7519 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/spark_sql.py
+-rw-r--r--   0        0        0    19752 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/sql_database.py
+-rw-r--r--   0        0        0     2639 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/stackexchange.py
+-rw-r--r--   0        0        0     5857 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/steam.py
+-rw-r--r--   0        0        0     6834 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/tavily_search.py
+-rw-r--r--   0        0        0     4006 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0     3441 2024-01-06 00:18:17.290393 langchain_community-0.0.9/langchain_community/utilities/twilio.py
+-rw-r--r--   0        0        0     4072 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utilities/vertexai.py
+-rw-r--r--   0        0        0     4045 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utilities/wikipedia.py
+-rw-r--r--   0        0        0     2011 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0    11666 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utilities/zapier.py
+-rw-r--r--   0        0        0       45 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utils/__init__.py
+-rw-r--r--   0        0        0     1511 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utils/ernie_functions.py
+-rw-r--r--   0        0        0     2713 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utils/math.py
+-rw-r--r--   0        0        0      264 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utils/openai.py
+-rw-r--r--   0        0        0      377 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/utils/openai_functions.py
+-rw-r--r--   0        0        0    16216 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/__init__.py
+-rw-r--r--   0        0        0    19780 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0    15738 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0    16632 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/annoy.py
+-rw-r--r--   0        0        0    28449 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/astradb.py
+-rw-r--r--   0        0        0    12136 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/atlas.py
+-rw-r--r--   0        0        0    21155 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/awadb.py
+-rw-r--r--   0        0        0    14522 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0    27218 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0    15034 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/bageldb.py
+-rw-r--r--   0        0        0    16548 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0    33082 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/bigquery_vector_search.py
+-rw-r--r--   0        0        0    14809 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/cassandra.py
+-rw-r--r--   0        0        0    30537 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/chroma.py
+-rw-r--r--   0        0        0    10953 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/clarifai.py
+-rw-r--r--   0        0        0    17735 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0    12713 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/dashvector.py
+-rw-r--r--   0        0        0    18360 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0    40265 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/deeplake.py
+-rw-r--r--   0        0        0    12973 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/dingo.py
+-rw-r--r--   0        0        0      236 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0     6945 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0     4044 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0     2418 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0    28714 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0    46759 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0    14183 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/epsilla.py
+-rw-r--r--   0        0        0    42920 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/faiss.py
+-rw-r--r--   0        0        0    26837 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/hippo.py
+-rw-r--r--   0        0        0    13642 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/hologres.py
+-rw-r--r--   0        0        0    14234 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/jaguar.py
+-rw-r--r--   0        0        0     4173 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/lancedb.py
+-rw-r--r--   0        0        0     7745 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0    17047 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/marqo.py
+-rw-r--r--   0        0        0    21430 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0    10400 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0    34224 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/milvus.py
+-rw-r--r--   0        0        0    19047 2024-01-06 00:18:17.294394 langchain_community-0.0.9/langchain_community/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0    13869 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0    22546 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/myscale.py
+-rw-r--r--   0        0        0    35000 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0     5403 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0    31850 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0    17895 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0     8891 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0    35925 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    17517 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    90569 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      265 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0    54458 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/redis/base.py
+-rw-r--r--   0        0        0      420 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/redis/constants.py
+-rw-r--r--   0        0        0    16227 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0    10419 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0    12192 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0    19610 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/scann.py
+-rw-r--r--   0        0        0     9707 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/semadb.py
+-rw-r--r--   0        0        0    17628 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0    12375 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/sklearn.py
+-rw-r--r--   0        0        0     7316 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0    17150 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/starrocks.py
+-rw-r--r--   0        0        0    15689 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/supabase.py
+-rw-r--r--   0        0        0    14726 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/surrealdb.py
+-rw-r--r--   0        0        0     9557 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/tair.py
+-rw-r--r--   0        0        0    13927 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0     4927 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/tigris.py
+-rw-r--r--   0        0        0    28826 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/tiledb.py
+-rw-r--r--   0        0        0    29831 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0     9712 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/typesense.py
+-rw-r--r--   0        0        0     5888 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/usearch.py
+-rw-r--r--   0        0        0     2474 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/utils.py
+-rw-r--r--   0        0        0    12908 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/vald.py
+-rw-r--r--   0        0        0    19844 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/vearch.py
+-rw-r--r--   0        0        0    21305 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/vectara.py
+-rw-r--r--   0        0        0     9785 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/vespa.py
+-rw-r--r--   0        0        0    19226 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/weaviate.py
+-rw-r--r--   0        0        0     9032 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/xata.py
+-rw-r--r--   0        0        0    10761 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0    23192 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/zep.py
+-rw-r--r--   0        0        0     7575 2024-01-06 00:18:17.298394 langchain_community-0.0.9/langchain_community/vectorstores/zilliz.py
+-rw-r--r--   0        0        0     9721 2024-01-06 00:18:17.302394 langchain_community-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7333 1970-01-01 00:00:00.000000 langchain_community-0.0.9/PKG-INFO
```

### Comparing `langchain_community-0.0.8/README.md` & `langchain_community-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/adapters/openai.py` & `langchain_community-0.0.9/langchain_community/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/__init__.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/ainetwork/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/ainetwork/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/amadeus/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/amadeus/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/azure_cognitive_services.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/azure_cognitive_services.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/clickup/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/clickup/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/csv/__init__.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/file_management/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/file_management/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/github/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/gitlab/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/gitlab/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/gmail/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/jira/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/jira/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/json/base.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/json/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/json/prompt.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/json/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/json/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/json/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/multion/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/multion/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/nasa/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/nasa/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/nla/tool.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/nla/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/nla/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/nla/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/office365/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/office365/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/base.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/planner.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/planner_prompt.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/prompt.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/spec.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/openapi/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/openapi/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/playwright/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/playwright/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/base.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/chat_base.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/chat_base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/prompt.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/powerbi/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/powerbi/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/slack/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/slack/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/base.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/prompt.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/spark_sql/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/spark_sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/sql/base.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/sql/prompt.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/sql/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/steam/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/steam/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/xorbits/__init__.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/agent_toolkits/zapier/toolkit.py` & `langchain_community-0.0.9/langchain_community/agent_toolkits/zapier/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/cache.py` & `langchain_community-0.0.9/langchain_community/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 except ImportError:
     from sqlalchemy.ext.declarative import declarative_base
 
 from langchain_core.caches import RETURN_VAL_TYPE, BaseCache
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models.llms import LLM, get_prompts
 from langchain_core.load.dump import dumps
-from langchain_core.load.load import loads
+from langchain_core.load.load import _loads_suppress_warning
 from langchain_core.outputs import ChatGeneration, Generation
 from langchain_core.utils import get_from_env
 
 from langchain_community.vectorstores.redis import Redis as RedisVectorstore
 
 logger = logging.getLogger(__file__)
 
@@ -145,15 +145,18 @@
     Does not raise exceptions for malformed entries, just logs a warning
     and returns none: the caller should be prepared for such a cache miss.
 
     Returns:
         RETURN_VAL_TYPE: A list of generations.
     """
     try:
-        generations = [loads(_item_str) for _item_str in json.loads(generations_str)]
+        generations = [
+            _loads_suppress_warning(_item_str)
+            for _item_str in json.loads(generations_str)
+        ]
         return generations
     except (json.JSONDecodeError, TypeError):
         # deferring the (soft) handling to after the legacy-format attempt
         pass
 
     try:
         gen_dicts = json.loads(generations_str)
@@ -220,15 +223,15 @@
             .where(self.cache_schema.llm == llm_string)
             .order_by(self.cache_schema.idx)
         )
         with Session(self.engine) as session:
             rows = session.execute(stmt).fetchall()
             if rows:
                 try:
-                    return [loads(row[0]) for row in rows]
+                    return [_loads_suppress_warning(row[0]) for row in rows]
                 except Exception:
                     logger.warning(
                         "Retrieving a cache value that could not be deserialized "
                         "properly. This is likely due to the cache being in an "
                         "older format. Please recreate your cache to avoid this "
                         "error."
                     )
@@ -391,15 +394,15 @@
         """Look up based on prompt and llm_string."""
         generations = []
         # Read from a Redis HASH
         results = self.redis.hgetall(self._key(prompt, llm_string))
         if results:
             for _, text in results.items():
                 try:
-                    generations.append(loads(text))
+                    generations.append(_loads_suppress_warning(text))
                 except Exception:
                     logger.warning(
                         "Retrieving a cache value that could not be deserialized "
                         "properly. This is likely due to the cache being in an "
                         "older format. Please recreate your cache to avoid this "
                         "error."
                     )
@@ -531,15 +534,17 @@
             query=prompt,
             k=1,
             distance_threshold=self.score_threshold,
         )
         if results:
             for document in results:
                 try:
-                    generations.extend(loads(document.metadata["return_val"]))
+                    generations.extend(
+                        _loads_suppress_warning(document.metadata["return_val"])
+                    )
                 except Exception:
                     logger.warning(
                         "Retrieving a cache value that could not be deserialized "
                         "properly. This is likely due to the cache being in an "
                         "older format. Please recreate your cache to avoid this "
                         "error."
                     )
@@ -1181,15 +1186,15 @@
         self.cache_schema = cache_schema
         self.cache_schema.metadata.create_all(self.engine)
 
     def lookup(self, prompt: str, llm_string: str) -> Optional[RETURN_VAL_TYPE]:
         """Look up based on prompt and llm_string."""
         rows = self._search_rows(prompt, llm_string)
         if rows:
-            return [loads(row[0]) for row in rows]
+            return [_loads_suppress_warning(row[0]) for row in rows]
         return None
 
     def update(self, prompt: str, llm_string: str, return_val: RETURN_VAL_TYPE) -> None:
         """Update based on prompt and llm_string."""
         self._delete_previous(prompt, llm_string)
         prompt_md5 = self.get_md5(prompt)
         items = [
```

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/__init__.py` & `langchain_community-0.0.9/langchain_community/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/aim_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/aim_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/argilla_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/argilla_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/arize_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/arize_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/arthur_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/arthur_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/clearml_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/clearml_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/comet_ml_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/comet_ml_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/confident_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/confident_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/context_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/context_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/flyte_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/flyte_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/human.py` & `langchain_community-0.0.9/langchain_community/callbacks/human.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/infino_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/infino_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/labelstudio_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/labelstudio_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/llmonitor_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/llmonitor_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/manager.py` & `langchain_community-0.0.9/langchain_community/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/mlflow_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/mlflow_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/openai_info.py` & `langchain_community-0.0.9/langchain_community/callbacks/openai_info.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/promptlayer_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/promptlayer_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/sagemaker_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/sagemaker_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/streamlit/__init__.py` & `langchain_community-0.0.9/langchain_community/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/streamlit/mutable_expander.py` & `langchain_community-0.0.9/langchain_community/callbacks/streamlit/mutable_expander.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/streamlit/streamlit_callback_handler.py` & `langchain_community-0.0.9/langchain_community/callbacks/streamlit/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/tracers/comet.py` & `langchain_community-0.0.9/langchain_community/callbacks/tracers/comet.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/tracers/wandb.py` & `langchain_community-0.0.9/langchain_community/callbacks/tracers/wandb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/trubrics_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/trubrics_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/utils.py` & `langchain_community-0.0.9/langchain_community/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/wandb_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/callbacks/whylabs_callback.py` & `langchain_community-0.0.9/langchain_community/callbacks/whylabs_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/facebook_messenger.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/facebook_messenger.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/gmail.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/gmail.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/imessage.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/imessage.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/langsmith.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/langsmith.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Dict, Iterable, Iterator, List, Optional, Union, cast
 
 from langchain_core.chat_sessions import ChatSession
-from langchain_core.load import load
+from langchain_core.load.load import _load_suppress_warning
 
 from langchain_community.chat_loaders.base import BaseChatLoader
 
 if TYPE_CHECKING:
     from langsmith.client import Client
     from langsmith.schemas import Run
 
@@ -62,16 +62,18 @@
         """
         if llm_run.run_type != "llm":
             raise ValueError(f"Expected run of type llm. Got: {llm_run.run_type}")
         if "messages" not in llm_run.inputs:
             raise ValueError(f"Run has no 'messages' inputs. Got {llm_run.inputs}")
         if not llm_run.outputs:
             raise ValueError("Cannot convert pending run")
-        messages = load(llm_run.inputs)["messages"]
-        message_chunk = load(llm_run.outputs)["generations"][0]["message"]
+        messages = _load_suppress_warning(llm_run.inputs)["messages"]
+        message_chunk = _load_suppress_warning(llm_run.outputs)["generations"][0][
+            "message"
+        ]
         return ChatSession(messages=messages + [message_chunk])
 
     @staticmethod
     def _get_functions_from_llm_run(llm_run: "Run") -> Optional[List[Dict]]:
         """
         Extract functions from a LangSmith LLM run if they exist.
```

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/slack.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/slack.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/telegram.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/utils.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_loaders/whatsapp.py` & `langchain_community-0.0.9/langchain_community/chat_loaders/whatsapp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/__init__.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/astradb.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/cassandra.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/cassandra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/cosmos_db.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/dynamodb.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/elasticsearch.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/file.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/firestore.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/firestore.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/in_memory.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/momento.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/momento.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/mongodb.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/neo4j.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/neo4j.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/postgres.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/postgres.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/redis.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/rocksetdb.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/singlestoredb.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/sql.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/sql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/streamlit.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/streamlit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/upstash_redis.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/xata.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/xata.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_message_histories/zep.py` & `langchain_community-0.0.9/langchain_community/chat_message_histories/zep.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/__init__.py` & `langchain_community-0.0.9/langchain_community/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/anthropic.py` & `langchain_community-0.0.9/langchain_community/chat_models/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/anyscale.py` & `langchain_community-0.0.9/langchain_community/chat_models/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/azure_openai.py` & `langchain_community-0.0.9/langchain_community/chat_models/azure_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 from __future__ import annotations
 
 import logging
 import os
 import warnings
 from typing import Any, Callable, Dict, List, Union
 
+from langchain_core._api.deprecation import deprecated
 from langchain_core.outputs import ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
 from langchain_community.chat_models.openai import ChatOpenAI
 from langchain_community.utils.openai import is_openai_v1
 
 logger = logging.getLogger(__name__)
 
 
+@deprecated(
+    since="0.1.0", removal="0.2.0", alternative="langchain_openai.AzureChatOpenAI"
+)
 class AzureChatOpenAI(ChatOpenAI):
     """`Azure OpenAI` Chat Completion API.
 
     To use this class you
     must have a deployed model on Azure OpenAI. Use `deployment_name` in the
     constructor to refer to the "Model deployment name" in the Azure portal.
```

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/azureml_endpoint.py` & `langchain_community-0.0.9/langchain_community/chat_models/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/baichuan.py` & `langchain_community-0.0.9/langchain_community/chat_models/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/baidu_qianfan_endpoint.py` & `langchain_community-0.0.9/langchain_community/chat_models/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/bedrock.py` & `langchain_community-0.0.9/langchain_community/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/cohere.py` & `langchain_community-0.0.9/langchain_community/chat_models/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/databricks.py` & `langchain_community-0.0.9/langchain_community/chat_models/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/ernie.py` & `langchain_community-0.0.9/langchain_community/chat_models/ernie.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/everlyai.py` & `langchain_community-0.0.9/langchain_community/chat_models/everlyai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/fake.py` & `langchain_community-0.0.9/langchain_community/chat_models/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/fireworks.py` & `langchain_community-0.0.9/langchain_community/chat_models/fireworks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/gigachat.py` & `langchain_community-0.0.9/langchain_community/chat_models/gigachat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/google_palm.py` & `langchain_community-0.0.9/langchain_community/chat_models/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/gpt_router.py` & `langchain_community-0.0.9/langchain_community/chat_models/gpt_router.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/huggingface.py` & `langchain_community-0.0.9/langchain_community/chat_models/huggingface.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/human.py` & `langchain_community-0.0.9/langchain_community/chat_models/human.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/hunyuan.py` & `langchain_community-0.0.9/langchain_community/chat_models/hunyuan.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/javelin_ai_gateway.py` & `langchain_community-0.0.9/langchain_community/chat_models/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/jinachat.py` & `langchain_community-0.0.9/langchain_community/chat_models/jinachat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/konko.py` & `langchain_community-0.0.9/langchain_community/chat_models/konko.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/litellm.py` & `langchain_community-0.0.9/langchain_community/chat_models/litellm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/meta.py` & `langchain_community-0.0.9/langchain_community/chat_models/meta.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/minimax.py` & `langchain_community-0.0.9/langchain_community/chat_models/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/mlflow.py` & `langchain_community-0.0.9/langchain_community/chat_models/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/mlflow_ai_gateway.py` & `langchain_community-0.0.9/langchain_community/chat_models/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/ollama.py` & `langchain_community-0.0.9/langchain_community/chat_models/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/openai.py` & `langchain_community-0.0.9/langchain_community/chat_models/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
+from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
@@ -139,14 +140,15 @@
         return ToolMessageChunk(content=content, tool_call_id=_dict["tool_call_id"])
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role)
     else:
         return default_class(content=content)
 
 
+@deprecated(since="0.1.0", removal="0.2.0", alternative="langchain_openai.ChatOpenAI")
 class ChatOpenAI(BaseChatModel):
     """`OpenAI` Chat large language models API.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
 
     Any parameters that are valid to be passed to the openai.create call can be passed
```

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/pai_eas_endpoint.py` & `langchain_community-0.0.9/langchain_community/chat_models/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/promptlayer_openai.py` & `langchain_community-0.0.9/langchain_community/chat_models/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/tongyi.py` & `langchain_community-0.0.9/langchain_community/chat_models/tongyi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/vertexai.py` & `langchain_community-0.0.9/langchain_community/chat_models/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/volcengine_maas.py` & `langchain_community-0.0.9/langchain_community/chat_models/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/wasm_chat.py` & `langchain_community-0.0.9/langchain_community/chat_models/wasm_chat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/yandex.py` & `langchain_community-0.0.9/langchain_community/chat_models/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/chat_models/zhipuai.py` & `langchain_community-0.0.9/langchain_community/chat_models/zhipuai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/docstore/__init__.py` & `langchain_community-0.0.9/langchain_community/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/docstore/arbitrary_fn.py` & `langchain_community-0.0.9/langchain_community/docstore/arbitrary_fn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/docstore/base.py` & `langchain_community-0.0.9/langchain_community/docstore/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/docstore/in_memory.py` & `langchain_community-0.0.9/langchain_community/docstore/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/docstore/wikipedia.py` & `langchain_community-0.0.9/langchain_community/docstore/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/__init__.py` & `langchain_community-0.0.9/langchain_community/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/acreom.py` & `langchain_community-0.0.9/langchain_community/document_loaders/acreom.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/airbyte.py` & `langchain_community-0.0.9/langchain_community/document_loaders/airbyte.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/airbyte_json.py` & `langchain_community-0.0.9/langchain_community/document_loaders/airbyte_json.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/airtable.py` & `langchain_community-0.0.9/langchain_community/document_loaders/airtable.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/apify_dataset.py` & `langchain_community-0.0.9/langchain_community/document_loaders/apify_dataset.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/arcgis_loader.py` & `langchain_community-0.0.9/langchain_community/document_loaders/arcgis_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/arxiv.py` & `langchain_community-0.0.9/langchain_community/document_loaders/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/assemblyai.py` & `langchain_community-0.0.9/langchain_community/document_loaders/assemblyai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/astradb.py` & `langchain_community-0.0.9/langchain_community/document_loaders/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/async_html.py` & `langchain_community-0.0.9/langchain_community/document_loaders/async_html.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/azlyrics.py` & `langchain_community-0.0.9/langchain_community/document_loaders/azlyrics.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/azure_ai_data.py` & `langchain_community-0.0.9/langchain_community/document_loaders/azure_ai_data.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/azure_blob_storage_container.py` & `langchain_community-0.0.9/langchain_community/document_loaders/azure_blob_storage_container.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/azure_blob_storage_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/azure_blob_storage_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/baiducloud_bos_directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/baiducloud_bos_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/baiducloud_bos_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/baiducloud_bos_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/base.py` & `langchain_community-0.0.9/langchain_community/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/base_o365.py` & `langchain_community-0.0.9/langchain_community/document_loaders/base_o365.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/bibtex.py` & `langchain_community-0.0.9/langchain_community/document_loaders/bibtex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/bigquery.py` & `langchain_community-0.0.9/langchain_community/document_loaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/bilibili.py` & `langchain_community-0.0.9/langchain_community/document_loaders/bilibili.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/blackboard.py` & `langchain_community-0.0.9/langchain_community/document_loaders/blackboard.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/file_system.py` & `langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/file_system.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/schema.py` & `langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/blob_loaders/youtube_audio.py` & `langchain_community-0.0.9/langchain_community/document_loaders/blob_loaders/youtube_audio.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/blockchain.py` & `langchain_community-0.0.9/langchain_community/document_loaders/blockchain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/brave_search.py` & `langchain_community-0.0.9/langchain_community/document_loaders/brave_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/browserless.py` & `langchain_community-0.0.9/langchain_community/document_loaders/browserless.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/chatgpt.py` & `langchain_community-0.0.9/langchain_community/document_loaders/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/chromium.py` & `langchain_community-0.0.9/langchain_community/document_loaders/chromium.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/college_confidential.py` & `langchain_community-0.0.9/langchain_community/document_loaders/college_confidential.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/concurrent.py` & `langchain_community-0.0.9/langchain_community/document_loaders/concurrent.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/confluence.py` & `langchain_community-0.0.9/langchain_community/document_loaders/confluence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/conllu.py` & `langchain_community-0.0.9/langchain_community/document_loaders/conllu.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/couchbase.py` & `langchain_community-0.0.9/langchain_community/document_loaders/couchbase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/csv_loader.py` & `langchain_community-0.0.9/langchain_community/document_loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/cube_semantic.py` & `langchain_community-0.0.9/langchain_community/document_loaders/cube_semantic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/datadog_logs.py` & `langchain_community-0.0.9/langchain_community/document_loaders/datadog_logs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/dataframe.py` & `langchain_community-0.0.9/langchain_community/document_loaders/dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/diffbot.py` & `langchain_community-0.0.9/langchain_community/document_loaders/diffbot.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/discord.py` & `langchain_community-0.0.9/langchain_community/document_loaders/discord.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/doc_intelligence.py` & `langchain_community-0.0.9/langchain_community/document_loaders/doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/docugami.py` & `langchain_community-0.0.9/langchain_community/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/docusaurus.py` & `langchain_community-0.0.9/langchain_community/document_loaders/docusaurus.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/dropbox.py` & `langchain_community-0.0.9/langchain_community/document_loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/duckdb_loader.py` & `langchain_community-0.0.9/langchain_community/document_loaders/duckdb_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/email.py` & `langchain_community-0.0.9/langchain_community/document_loaders/email.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/epub.py` & `langchain_community-0.0.9/langchain_community/document_loaders/epub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/etherscan.py` & `langchain_community-0.0.9/langchain_community/document_loaders/etherscan.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/evernote.py` & `langchain_community-0.0.9/langchain_community/document_loaders/evernote.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/excel.py` & `langchain_community-0.0.9/langchain_community/document_loaders/excel.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/facebook_chat.py` & `langchain_community-0.0.9/langchain_community/document_loaders/facebook_chat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/fauna.py` & `langchain_community-0.0.9/langchain_community/document_loaders/fauna.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/figma.py` & `langchain_community-0.0.9/langchain_community/document_loaders/figma.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/gcs_directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/gcs_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/gcs_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/generic.py` & `langchain_community-0.0.9/langchain_community/document_loaders/generic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/geodataframe.py` & `langchain_community-0.0.9/langchain_community/document_loaders/geodataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/git.py` & `langchain_community-0.0.9/langchain_community/document_loaders/git.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/gitbook.py` & `langchain_community-0.0.9/langchain_community/document_loaders/gitbook.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/github.py` & `langchain_community-0.0.9/langchain_community/document_loaders/github.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/google_speech_to_text.py` & `langchain_community-0.0.9/langchain_community/document_loaders/google_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/googledrive.py` & `langchain_community-0.0.9/langchain_community/document_loaders/googledrive.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/gutenberg.py` & `langchain_community-0.0.9/langchain_community/document_loaders/gutenberg.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/helpers.py` & `langchain_community-0.0.9/langchain_community/document_loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/hn.py` & `langchain_community-0.0.9/langchain_community/document_loaders/hn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/html.py` & `langchain_community-0.0.9/langchain_community/document_loaders/html.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/html_bs.py` & `langchain_community-0.0.9/langchain_community/document_loaders/html_bs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/hugging_face_dataset.py` & `langchain_community-0.0.9/langchain_community/document_loaders/hugging_face_dataset.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/ifixit.py` & `langchain_community-0.0.9/langchain_community/document_loaders/ifixit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/image.py` & `langchain_community-0.0.9/langchain_community/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/image_captions.py` & `langchain_community-0.0.9/langchain_community/document_loaders/image_captions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/iugu.py` & `langchain_community-0.0.9/langchain_community/document_loaders/iugu.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/joplin.py` & `langchain_community-0.0.9/langchain_community/document_loaders/joplin.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/json_loader.py` & `langchain_community-0.0.9/langchain_community/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/lakefs.py` & `langchain_community-0.0.9/langchain_community/document_loaders/lakefs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/larksuite.py` & `langchain_community-0.0.9/langchain_community/document_loaders/larksuite.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/markdown.py` & `langchain_community-0.0.9/langchain_community/document_loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/mastodon.py` & `langchain_community-0.0.9/langchain_community/document_loaders/mastodon.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/max_compute.py` & `langchain_community-0.0.9/langchain_community/document_loaders/max_compute.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/mediawikidump.py` & `langchain_community-0.0.9/langchain_community/document_loaders/mediawikidump.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/merge.py` & `langchain_community-0.0.9/langchain_community/document_loaders/merge.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/mhtml.py` & `langchain_community-0.0.9/langchain_community/document_loaders/mhtml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/modern_treasury.py` & `langchain_community-0.0.9/langchain_community/document_loaders/modern_treasury.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/mongodb.py` & `langchain_community-0.0.9/langchain_community/document_loaders/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/news.py` & `langchain_community-0.0.9/langchain_community/document_loaders/news.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/notebook.py` & `langchain_community-0.0.9/langchain_community/document_loaders/notebook.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/notion.py` & `langchain_community-0.0.9/langchain_community/document_loaders/notion.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/notiondb.py` & `langchain_community-0.0.9/langchain_community/document_loaders/notiondb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/nuclia.py` & `langchain_community-0.0.9/langchain_community/document_loaders/nuclia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/obs_directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/obs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/obs_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/obs_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/obsidian.py` & `langchain_community-0.0.9/langchain_community/document_loaders/obsidian.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/odt.py` & `langchain_community-0.0.9/langchain_community/document_loaders/odt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/onedrive.py` & `langchain_community-0.0.9/langchain_community/document_loaders/onedrive.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/onedrive_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/onedrive_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/onenote.py` & `langchain_community-0.0.9/langchain_community/document_loaders/onenote.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/open_city_data.py` & `langchain_community-0.0.9/langchain_community/document_loaders/open_city_data.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/org_mode.py` & `langchain_community-0.0.9/langchain_community/document_loaders/org_mode.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/__init__.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/audio.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/doc_intelligence.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/docai.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/docai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/generic.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/grobid.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/grobid.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/html/bs4.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/html/bs4.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/cobol.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/cobol.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/javascript.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/javascript.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/language_parser.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/language_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/language/python.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/language/python.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/msword.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/msword.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/pdf.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/parsers/registry.py` & `langchain_community-0.0.9/langchain_community/document_loaders/parsers/registry.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/pdf.py` & `langchain_community-0.0.9/langchain_community/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/polars_dataframe.py` & `langchain_community-0.0.9/langchain_community/document_loaders/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/powerpoint.py` & `langchain_community-0.0.9/langchain_community/document_loaders/powerpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/psychic.py` & `langchain_community-0.0.9/langchain_community/document_loaders/psychic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/pubmed.py` & `langchain_community-0.0.9/langchain_community/document_loaders/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/pyspark_dataframe.py` & `langchain_community-0.0.9/langchain_community/document_loaders/pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/python.py` & `langchain_community-0.0.9/langchain_community/document_loaders/python.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/quip.py` & `langchain_community-0.0.9/langchain_community/document_loaders/quip.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/readthedocs.py` & `langchain_community-0.0.9/langchain_community/document_loaders/readthedocs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/recursive_url_loader.py` & `langchain_community-0.0.9/langchain_community/document_loaders/recursive_url_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/reddit.py` & `langchain_community-0.0.9/langchain_community/document_loaders/reddit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/roam.py` & `langchain_community-0.0.9/langchain_community/document_loaders/roam.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/rocksetdb.py` & `langchain_community-0.0.9/langchain_community/document_loaders/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/rspace.py` & `langchain_community-0.0.9/langchain_community/document_loaders/rspace.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/rss.py` & `langchain_community-0.0.9/langchain_community/document_loaders/rss.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/rst.py` & `langchain_community-0.0.9/langchain_community/document_loaders/rst.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/rtf.py` & `langchain_community-0.0.9/langchain_community/document_loaders/rtf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/s3_directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/s3_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/s3_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/s3_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/sharepoint.py` & `langchain_community-0.0.9/langchain_community/document_loaders/sharepoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/sitemap.py` & `langchain_community-0.0.9/langchain_community/document_loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/slack_directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/slack_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/snowflake_loader.py` & `langchain_community-0.0.9/langchain_community/document_loaders/snowflake_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/spreedly.py` & `langchain_community-0.0.9/langchain_community/document_loaders/spreedly.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/srt.py` & `langchain_community-0.0.9/langchain_community/document_loaders/srt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/stripe.py` & `langchain_community-0.0.9/langchain_community/document_loaders/stripe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/telegram.py` & `langchain_community-0.0.9/langchain_community/document_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/tencent_cos_directory.py` & `langchain_community-0.0.9/langchain_community/document_loaders/tencent_cos_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/tencent_cos_file.py` & `langchain_community-0.0.9/langchain_community/document_loaders/tencent_cos_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/tensorflow_datasets.py` & `langchain_community-0.0.9/langchain_community/document_loaders/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/text.py` & `langchain_community-0.0.9/langchain_community/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/tomarkdown.py` & `langchain_community-0.0.9/langchain_community/document_loaders/tomarkdown.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/toml.py` & `langchain_community-0.0.9/langchain_community/document_loaders/toml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/trello.py` & `langchain_community-0.0.9/langchain_community/document_loaders/trello.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/tsv.py` & `langchain_community-0.0.9/langchain_community/document_loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/twitter.py` & `langchain_community-0.0.9/langchain_community/document_loaders/twitter.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/unstructured.py` & `langchain_community-0.0.9/langchain_community/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/url.py` & `langchain_community-0.0.9/langchain_community/document_loaders/url.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/url_playwright.py` & `langchain_community-0.0.9/langchain_community/document_loaders/url_playwright.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/url_selenium.py` & `langchain_community-0.0.9/langchain_community/document_loaders/url_selenium.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/weather.py` & `langchain_community-0.0.9/langchain_community/document_loaders/weather.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/web_base.py` & `langchain_community-0.0.9/langchain_community/document_loaders/web_base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/whatsapp_chat.py` & `langchain_community-0.0.9/langchain_community/document_loaders/whatsapp_chat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/wikipedia.py` & `langchain_community-0.0.9/langchain_community/document_loaders/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/word_document.py` & `langchain_community-0.0.9/langchain_community/document_loaders/word_document.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/xml.py` & `langchain_community-0.0.9/langchain_community/document_loaders/xml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/xorbits.py` & `langchain_community-0.0.9/langchain_community/document_loaders/xorbits.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_loaders/youtube.py` & `langchain_community-0.0.9/langchain_community/document_loaders/youtube.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/__init__.py` & `langchain_community-0.0.9/langchain_community/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/beautiful_soup_transformer.py` & `langchain_community-0.0.9/langchain_community/document_transformers/beautiful_soup_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/doctran_text_extract.py` & `langchain_community-0.0.9/langchain_community/document_transformers/doctran_text_extract.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/doctran_text_qa.py` & `langchain_community-0.0.9/langchain_community/document_transformers/doctran_text_qa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/doctran_text_translate.py` & `langchain_community-0.0.9/langchain_community/document_transformers/doctran_text_translate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/embeddings_redundant_filter.py` & `langchain_community-0.0.9/langchain_community/document_transformers/embeddings_redundant_filter.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/google_translate.py` & `langchain_community-0.0.9/langchain_community/document_transformers/google_translate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/html2text.py` & `langchain_community-0.0.9/langchain_community/document_transformers/html2text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/long_context_reorder.py` & `langchain_community-0.0.9/langchain_community/document_transformers/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/nuclia_text_transform.py` & `langchain_community-0.0.9/langchain_community/document_transformers/nuclia_text_transform.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/openai_functions.py` & `langchain_community-0.0.9/langchain_community/document_transformers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt` & `langchain_community-0.0.9/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/__init__.py` & `langchain_community-0.0.9/langchain_community/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/aleph_alpha.py` & `langchain_community-0.0.9/langchain_community/embeddings/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/awa.py` & `langchain_community-0.0.9/langchain_community/embeddings/awa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/azure_openai.py` & `langchain_community-0.0.9/langchain_community/embeddings/azure_openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Azure OpenAI embeddings wrapper."""
 from __future__ import annotations
 
 import os
 import warnings
 from typing import Callable, Dict, Optional, Union
 
+from langchain_core._api.deprecation import deprecated
 from langchain_core.pydantic_v1 import Field, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
 from langchain_community.embeddings.openai import OpenAIEmbeddings
 from langchain_community.utils.openai import is_openai_v1
 
 
+@deprecated(
+    since="0.1.0", removal="0.2.0", alternative="langchain_openai.AzureOpenAIEmbeddings"
+)
 class AzureOpenAIEmbeddings(OpenAIEmbeddings):
     """`Azure OpenAI` Embeddings API."""
 
     azure_endpoint: Union[str, None] = None
     """Your Azure endpoint, including the resource.
 
         Automatically inferred from env var `AZURE_OPENAI_ENDPOINT` if not provided.
```

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/baidu_qianfan_endpoint.py` & `langchain_community-0.0.9/langchain_community/embeddings/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/bedrock.py` & `langchain_community-0.0.9/langchain_community/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/bookend.py` & `langchain_community-0.0.9/langchain_community/embeddings/bookend.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/clarifai.py` & `langchain_community-0.0.9/langchain_community/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/cloudflare_workersai.py` & `langchain_community-0.0.9/langchain_community/embeddings/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/cohere.py` & `langchain_community-0.0.9/langchain_community/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/dashscope.py` & `langchain_community-0.0.9/langchain_community/embeddings/dashscope.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/databricks.py` & `langchain_community-0.0.9/langchain_community/embeddings/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/deepinfra.py` & `langchain_community-0.0.9/langchain_community/embeddings/deepinfra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/edenai.py` & `langchain_community-0.0.9/langchain_community/embeddings/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/elasticsearch.py` & `langchain_community-0.0.9/langchain_community/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/embaas.py` & `langchain_community-0.0.9/langchain_community/embeddings/embaas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/ernie.py` & `langchain_community-0.0.9/langchain_community/embeddings/ernie.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/fake.py` & `langchain_community-0.0.9/langchain_community/embeddings/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/fastembed.py` & `langchain_community-0.0.9/langchain_community/embeddings/fastembed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/google_palm.py` & `langchain_community-0.0.9/langchain_community/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/gpt4all.py` & `langchain_community-0.0.9/langchain_community/embeddings/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/gradient_ai.py` & `langchain_community-0.0.9/langchain_community/embeddings/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/huggingface.py` & `langchain_community-0.0.9/langchain_community/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/huggingface_hub.py` & `langchain_community-0.0.9/langchain_community/embeddings/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/infinity.py` & `langchain_community-0.0.9/langchain_community/embeddings/infinity.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/javelin_ai_gateway.py` & `langchain_community-0.0.9/langchain_community/embeddings/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/jina.py` & `langchain_community-0.0.9/langchain_community/embeddings/jina.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/johnsnowlabs.py` & `langchain_community-0.0.9/langchain_community/embeddings/johnsnowlabs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/llamacpp.py` & `langchain_community-0.0.9/langchain_community/embeddings/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/llm_rails.py` & `langchain_community-0.0.9/langchain_community/embeddings/llm_rails.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/localai.py` & `langchain_community-0.0.9/langchain_community/embeddings/localai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/minimax.py` & `langchain_community-0.0.9/langchain_community/embeddings/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/mlflow.py` & `langchain_community-0.0.9/langchain_community/embeddings/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/mlflow_gateway.py` & `langchain_community-0.0.9/langchain_community/embeddings/mlflow_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/modelscope_hub.py` & `langchain_community-0.0.9/langchain_community/embeddings/modelscope_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/mosaicml.py` & `langchain_community-0.0.9/langchain_community/embeddings/mosaicml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/nlpcloud.py` & `langchain_community-0.0.9/langchain_community/embeddings/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/octoai_embeddings.py` & `langchain_community-0.0.9/langchain_community/embeddings/octoai_embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/ollama.py` & `langchain_community-0.0.9/langchain_community/embeddings/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/openai.py` & `langchain_community-0.0.9/langchain_community/embeddings/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Set,
     Tuple,
     Union,
     cast,
 )
 
 import numpy as np
+from langchain_core._api.deprecation import deprecated
 from langchain_core.embeddings import Embeddings
 from langchain_core.pydantic_v1 import BaseModel, Extra, Field, root_validator
 from langchain_core.utils import get_from_dict_or_env, get_pydantic_field_names
 from tenacity import (
     AsyncRetrying,
     before_sleep_log,
     retry,
@@ -133,14 +134,19 @@
     async def _async_embed_with_retry(**kwargs: Any) -> Any:
         response = await embeddings.client.acreate(**kwargs)
         return _check_response(response, skip_empty=embeddings.skip_empty)
 
     return await _async_embed_with_retry(**kwargs)
 
 
+@deprecated(
+    since="0.1.0",
+    removal="0.2.0",
+    alternative="langchain_openai.OpenAIEmbeddings",
+)
 class OpenAIEmbeddings(BaseModel, Embeddings):
     """OpenAI embedding models.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key or pass it
     as a named parameter to the constructor.
```

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/sagemaker_endpoint.py` & `langchain_community-0.0.9/langchain_community/embeddings/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/self_hosted.py` & `langchain_community-0.0.9/langchain_community/embeddings/self_hosted.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/self_hosted_hugging_face.py` & `langchain_community-0.0.9/langchain_community/embeddings/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/spacy_embeddings.py` & `langchain_community-0.0.9/langchain_community/embeddings/spacy_embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/tensorflow_hub.py` & `langchain_community-0.0.9/langchain_community/embeddings/tensorflow_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/vertexai.py` & `langchain_community-0.0.9/langchain_community/embeddings/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/volcengine.py` & `langchain_community-0.0.9/langchain_community/embeddings/volcengine.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/voyageai.py` & `langchain_community-0.0.9/langchain_community/embeddings/voyageai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/xinference.py` & `langchain_community-0.0.9/langchain_community/embeddings/xinference.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/embeddings/yandex.py` & `langchain_community-0.0.9/langchain_community/embeddings/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/__init__.py` & `langchain_community-0.0.9/langchain_community/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/arangodb_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/arangodb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/falkordb_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/falkordb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/graph_document.py` & `langchain_community-0.0.9/langchain_community/graphs/graph_document.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/graph_store.py` & `langchain_community-0.0.9/langchain_community/graphs/graph_store.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/hugegraph.py` & `langchain_community-0.0.9/langchain_community/graphs/hugegraph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/kuzu_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/kuzu_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/memgraph_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/memgraph_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/nebula_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/nebula_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/neo4j_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/neptune_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/networkx_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/graphs/rdf_graph.py` & `langchain_community-0.0.9/langchain_community/graphs/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/indexes/_sql_record_manager.py` & `langchain_community-0.0.9/langchain_community/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/indexes/base.py` & `langchain_community-0.0.9/langchain_community/indexes/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/__init__.py` & `langchain_community-0.0.9/langchain_community/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/ai21.py` & `langchain_community-0.0.9/langchain_community/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/aleph_alpha.py` & `langchain_community-0.0.9/langchain_community/llms/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/amazon_api_gateway.py` & `langchain_community-0.0.9/langchain_community/llms/amazon_api_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/anthropic.py` & `langchain_community-0.0.9/langchain_community/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/anyscale.py` & `langchain_community-0.0.9/langchain_community/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/aphrodite.py` & `langchain_community-0.0.9/langchain_community/llms/aphrodite.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/arcee.py` & `langchain_community-0.0.9/langchain_community/llms/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/aviary.py` & `langchain_community-0.0.9/langchain_community/llms/aviary.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/azureml_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/baidu_qianfan_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/bananadev.py` & `langchain_community-0.0.9/langchain_community/llms/bananadev.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/baseten.py` & `langchain_community-0.0.9/langchain_community/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/beam.py` & `langchain_community-0.0.9/langchain_community/llms/beam.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/bedrock.py` & `langchain_community-0.0.9/langchain_community/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/bittensor.py` & `langchain_community-0.0.9/langchain_community/llms/bittensor.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/cerebriumai.py` & `langchain_community-0.0.9/langchain_community/llms/cerebriumai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/chatglm.py` & `langchain_community-0.0.9/langchain_community/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/clarifai.py` & `langchain_community-0.0.9/langchain_community/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/cloudflare_workersai.py` & `langchain_community-0.0.9/langchain_community/llms/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/cohere.py` & `langchain_community-0.0.9/langchain_community/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/ctransformers.py` & `langchain_community-0.0.9/langchain_community/llms/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/ctranslate2.py` & `langchain_community-0.0.9/langchain_community/llms/ctranslate2.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/databricks.py` & `langchain_community-0.0.9/langchain_community/llms/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/deepinfra.py` & `langchain_community-0.0.9/langchain_community/llms/deepinfra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/deepsparse.py` & `langchain_community-0.0.9/langchain_community/llms/deepsparse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/edenai.py` & `langchain_community-0.0.9/langchain_community/llms/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/fake.py` & `langchain_community-0.0.9/langchain_community/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/fireworks.py` & `langchain_community-0.0.9/langchain_community/llms/fireworks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/forefrontai.py` & `langchain_community-0.0.9/langchain_community/llms/forefrontai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/gigachat.py` & `langchain_community-0.0.9/langchain_community/llms/gigachat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/google_palm.py` & `langchain_community-0.0.9/langchain_community/llms/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/gooseai.py` & `langchain_community-0.0.9/langchain_community/llms/gooseai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/gpt4all.py` & `langchain_community-0.0.9/langchain_community/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/gradient_ai.py` & `langchain_community-0.0.9/langchain_community/llms/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/grammars/json.gbnf` & `langchain_community-0.0.9/langchain_community/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/huggingface_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/huggingface_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/huggingface_hub.py` & `langchain_community-0.0.9/langchain_community/llms/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/huggingface_pipeline.py` & `langchain_community-0.0.9/langchain_community/llms/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/huggingface_text_gen_inference.py` & `langchain_community-0.0.9/langchain_community/llms/huggingface_text_gen_inference.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/human.py` & `langchain_community-0.0.9/langchain_community/llms/human.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/javelin_ai_gateway.py` & `langchain_community-0.0.9/langchain_community/llms/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/koboldai.py` & `langchain_community-0.0.9/langchain_community/llms/koboldai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/llamacpp.py` & `langchain_community-0.0.9/langchain_community/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/loading.py` & `langchain_community-0.0.9/langchain_community/llms/loading.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/manifest.py` & `langchain_community-0.0.9/langchain_community/llms/manifest.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/minimax.py` & `langchain_community-0.0.9/langchain_community/llms/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/mlflow.py` & `langchain_community-0.0.9/langchain_community/llms/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/mlflow_ai_gateway.py` & `langchain_community-0.0.9/langchain_community/llms/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/modal.py` & `langchain_community-0.0.9/langchain_community/llms/modal.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/mosaicml.py` & `langchain_community-0.0.9/langchain_community/llms/mosaicml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/nlpcloud.py` & `langchain_community-0.0.9/langchain_community/llms/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/oci_data_science_model_deployment_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/oci_data_science_model_deployment_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/octoai_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/octoai_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/ollama.py` & `langchain_community-0.0.9/langchain_community/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/opaqueprompts.py` & `langchain_community-0.0.9/langchain_community/llms/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/openai.py` & `langchain_community-0.0.9/langchain_community/llms/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Mapping,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
+from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models.llms import BaseLLM, create_base_retry_decorator
 from langchain_core.outputs import Generation, GenerationChunk, LLMResult
 from langchain_core.pydantic_v1 import Field, root_validator
@@ -720,14 +721,15 @@
 
                 max_tokens = openai.max_token_for_prompt("Tell me a joke.")
         """
         num_tokens = self.get_num_tokens(prompt)
         return self.max_context_size - num_tokens
 
 
+@deprecated(since="0.1.0", removal="0.2.0", alternative="langchain_openai.OpenAI")
 class OpenAI(BaseOpenAI):
     """OpenAI large language models.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
 
     Any parameters that are valid to be passed to the openai.create call can be passed
@@ -746,14 +748,15 @@
         return ["langchain", "llms", "openai"]
 
     @property
     def _invocation_params(self) -> Dict[str, Any]:
         return {**{"model": self.model_name}, **super()._invocation_params}
 
 
+@deprecated(since="0.1.0", removal="0.2.0", alternative="langchain_openai.AzureOpenAI")
 class AzureOpenAI(BaseOpenAI):
     """Azure-specific OpenAI large language models.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
 
     Any parameters that are valid to be passed to the openai.create call can be passed
@@ -949,14 +952,15 @@
     def lc_attributes(self) -> Dict[str, Any]:
         return {
             "openai_api_type": self.openai_api_type,
             "openai_api_version": self.openai_api_version,
         }
 
 
+@deprecated(since="0.1.0", removal="0.2.0", alternative="langchain_openai.ChatOpenAI")
 class OpenAIChat(BaseLLM):
     """OpenAI Chat large language models.
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
 
     Any parameters that are valid to be passed to the openai.create call can be passed
```

### Comparing `langchain_community-0.0.8/langchain_community/llms/openllm.py` & `langchain_community-0.0.9/langchain_community/llms/openllm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/openlm.py` & `langchain_community-0.0.9/langchain_community/llms/openlm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/pai_eas_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/petals.py` & `langchain_community-0.0.9/langchain_community/llms/petals.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/pipelineai.py` & `langchain_community-0.0.9/langchain_community/llms/pipelineai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/predibase.py` & `langchain_community-0.0.9/langchain_community/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/predictionguard.py` & `langchain_community-0.0.9/langchain_community/llms/predictionguard.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/promptlayer_openai.py` & `langchain_community-0.0.9/langchain_community/llms/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/replicate.py` & `langchain_community-0.0.9/langchain_community/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/rwkv.py` & `langchain_community-0.0.9/langchain_community/llms/rwkv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/sagemaker_endpoint.py` & `langchain_community-0.0.9/langchain_community/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/self_hosted.py` & `langchain_community-0.0.9/langchain_community/llms/self_hosted.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/self_hosted_hugging_face.py` & `langchain_community-0.0.9/langchain_community/llms/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/stochasticai.py` & `langchain_community-0.0.9/langchain_community/llms/stochasticai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/symblai_nebula.py` & `langchain_community-0.0.9/langchain_community/llms/symblai_nebula.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/textgen.py` & `langchain_community-0.0.9/langchain_community/llms/textgen.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/titan_takeoff.py` & `langchain_community-0.0.9/langchain_community/llms/titan_takeoff.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/titan_takeoff_pro.py` & `langchain_community-0.0.9/langchain_community/llms/titan_takeoff_pro.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/together.py` & `langchain_community-0.0.9/langchain_community/llms/together.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/tongyi.py` & `langchain_community-0.0.9/langchain_community/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/vertexai.py` & `langchain_community-0.0.9/langchain_community/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/vllm.py` & `langchain_community-0.0.9/langchain_community/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/volcengine_maas.py` & `langchain_community-0.0.9/langchain_community/llms/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/watsonxllm.py` & `langchain_community-0.0.9/langchain_community/llms/watsonxllm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/writer.py` & `langchain_community-0.0.9/langchain_community/llms/writer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/xinference.py` & `langchain_community-0.0.9/langchain_community/llms/xinference.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/llms/yandex.py` & `langchain_community-0.0.9/langchain_community/llms/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/__init__.py` & `langchain_community-0.0.9/langchain_community/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/arcee.py` & `langchain_community-0.0.9/langchain_community/retrievers/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/arxiv.py` & `langchain_community-0.0.9/langchain_community/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/azure_cognitive_search.py` & `langchain_community-0.0.9/langchain_community/retrievers/azure_cognitive_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/bedrock.py` & `langchain_community-0.0.9/langchain_community/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/bm25.py` & `langchain_community-0.0.9/langchain_community/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/chaindesk.py` & `langchain_community-0.0.9/langchain_community/retrievers/chaindesk.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/chatgpt_plugin_retriever.py` & `langchain_community-0.0.9/langchain_community/retrievers/chatgpt_plugin_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/cohere_rag_retriever.py` & `langchain_community-0.0.9/langchain_community/retrievers/cohere_rag_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/databerry.py` & `langchain_community-0.0.9/langchain_community/retrievers/databerry.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/docarray.py` & `langchain_community-0.0.9/langchain_community/retrievers/docarray.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/elastic_search_bm25.py` & `langchain_community-0.0.9/langchain_community/retrievers/elastic_search_bm25.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/embedchain.py` & `langchain_community-0.0.9/langchain_community/retrievers/embedchain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/google_cloud_documentai_warehouse.py` & `langchain_community-0.0.9/langchain_community/retrievers/google_cloud_documentai_warehouse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/google_vertex_ai_search.py` & `langchain_community-0.0.9/langchain_community/retrievers/google_vertex_ai_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/kay.py` & `langchain_community-0.0.9/langchain_community/retrievers/kay.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/kendra.py` & `langchain_community-0.0.9/langchain_community/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/knn.py` & `langchain_community-0.0.9/langchain_community/retrievers/knn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/llama_index.py` & `langchain_community-0.0.9/langchain_community/retrievers/llama_index.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/metal.py` & `langchain_community-0.0.9/langchain_community/retrievers/metal.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/milvus.py` & `langchain_community-0.0.9/langchain_community/retrievers/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/outline.py` & `langchain_community-0.0.9/langchain_community/retrievers/outline.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/pinecone_hybrid_search.py` & `langchain_community-0.0.9/langchain_community/retrievers/pinecone_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/pubmed.py` & `langchain_community-0.0.9/langchain_community/retrievers/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/qdrant_sparse_vector_retriever.py` & `langchain_community-0.0.9/langchain_community/retrievers/qdrant_sparse_vector_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/remote_retriever.py` & `langchain_community-0.0.9/langchain_community/retrievers/remote_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/svm.py` & `langchain_community-0.0.9/langchain_community/retrievers/svm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/tavily_search_api.py` & `langchain_community-0.0.9/langchain_community/retrievers/tavily_search_api.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/tfidf.py` & `langchain_community-0.0.9/langchain_community/retrievers/tfidf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/vespa_retriever.py` & `langchain_community-0.0.9/langchain_community/retrievers/vespa_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/weaviate_hybrid_search.py` & `langchain_community-0.0.9/langchain_community/retrievers/weaviate_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/wikipedia.py` & `langchain_community-0.0.9/langchain_community/retrievers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/you.py` & `langchain_community-0.0.9/langchain_community/retrievers/you.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/zep.py` & `langchain_community-0.0.9/langchain_community/retrievers/zep.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/retrievers/zilliz.py` & `langchain_community-0.0.9/langchain_community/retrievers/zilliz.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/storage/redis.py` & `langchain_community-0.0.9/langchain_community/storage/redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/storage/upstash_redis.py` & `langchain_community-0.0.9/langchain_community/storage/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/app.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/app.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/base.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/owner.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/owner.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/rule.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/rule.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/transfer.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/transfer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/utils.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ainetwork/value.py` & `langchain_community-0.0.9/langchain_community/tools/ainetwork/value.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/amadeus/closest_airport.py` & `langchain_community-0.0.9/langchain_community/tools/amadeus/closest_airport.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/amadeus/flight_search.py` & `langchain_community-0.0.9/langchain_community/tools/amadeus/flight_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/amadeus/utils.py` & `langchain_community-0.0.9/langchain_community/tools/amadeus/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/arxiv/tool.py` & `langchain_community-0.0.9/langchain_community/tools/arxiv/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/form_recognizer.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/image_analysis.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/speech2text.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/speech2text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/text2speech.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/text2speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/text_analytics_health.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/text_analytics_health.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/azure_cognitive_services/utils.py` & `langchain_community-0.0.9/langchain_community/tools/azure_cognitive_services/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/bearly/tool.py` & `langchain_community-0.0.9/langchain_community/tools/bearly/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/bing_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/brave_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/brave_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/clickup/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/clickup/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/clickup/tool.py` & `langchain_community-0.0.9/langchain_community/tools/clickup/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/convert_to_openai.py` & `langchain_community-0.0.9/langchain_community/tools/convert_to_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/dataforseo_api_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/dataforseo_api_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ddg_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/ddg_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/e2b_data_analysis/tool.py` & `langchain_community-0.0.9/langchain_community/tools/e2b_data_analysis/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/e2b_data_analysis/unparse.py` & `langchain_community-0.0.9/langchain_community/tools/e2b_data_analysis/unparse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/audio_speech_to_text.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/audio_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/audio_text_to_speech.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/audio_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/edenai_base_tool.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/edenai_base_tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/image_explicitcontent.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/image_explicitcontent.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/image_objectdetection.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/image_objectdetection.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/ocr_identityparser.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/ocr_identityparser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/ocr_invoiceparser.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/ocr_invoiceparser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/edenai/text_moderation.py` & `langchain_community-0.0.9/langchain_community/tools/edenai/text_moderation.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/eleven_labs/text2speech.py` & `langchain_community-0.0.9/langchain_community/tools/eleven_labs/text2speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/copy.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/copy.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/delete.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/delete.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/file_search.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/file_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/list_dir.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/list_dir.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/move.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/move.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/read.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/read.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/utils.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/file_management/write.py` & `langchain_community-0.0.9/langchain_community/tools/file_management/write.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/github/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/github/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/github/tool.py` & `langchain_community-0.0.9/langchain_community/tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gitlab/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/gitlab/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gitlab/tool.py` & `langchain_community-0.0.9/langchain_community/tools/gitlab/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/base.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/create_draft.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/get_message.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/get_thread.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/search.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/send_message.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/gmail/utils.py` & `langchain_community-0.0.9/langchain_community/tools/gmail/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/golden_query/tool.py` & `langchain_community-0.0.9/langchain_community/tools/golden_query/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_cloud/texttospeech.py` & `langchain_community-0.0.9/langchain_community/tools/google_cloud/texttospeech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_finance/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_finance/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_jobs/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_jobs/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_lens/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_lens/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_places/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_places/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_scholar/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_scholar/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_serper/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_serper/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/google_trends/tool.py` & `langchain_community-0.0.9/langchain_community/tools/google_trends/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/graphql/tool.py` & `langchain_community-0.0.9/langchain_community/tools/graphql/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/human/tool.py` & `langchain_community-0.0.9/langchain_community/tools/human/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/ifttt.py` & `langchain_community-0.0.9/langchain_community/tools/ifttt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/jira/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/jira/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/jira/tool.py` & `langchain_community-0.0.9/langchain_community/tools/jira/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/json/tool.py` & `langchain_community-0.0.9/langchain_community/tools/json/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/memorize/tool.py` & `langchain_community-0.0.9/langchain_community/tools/memorize/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/merriam_webster/tool.py` & `langchain_community-0.0.9/langchain_community/tools/merriam_webster/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/metaphor_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/metaphor_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/multion/close_session.py` & `langchain_community-0.0.9/langchain_community/tools/multion/close_session.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/multion/create_session.py` & `langchain_community-0.0.9/langchain_community/tools/multion/create_session.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/multion/update_session.py` & `langchain_community-0.0.9/langchain_community/tools/multion/update_session.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/nasa/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/nasa/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/nasa/tool.py` & `langchain_community-0.0.9/langchain_community/tools/nasa/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/nuclia/tool.py` & `langchain_community-0.0.9/langchain_community/tools/nuclia/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/create_draft_message.py` & `langchain_community-0.0.9/langchain_community/tools/office365/create_draft_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/events_search.py` & `langchain_community-0.0.9/langchain_community/tools/office365/events_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/messages_search.py` & `langchain_community-0.0.9/langchain_community/tools/office365/messages_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/send_event.py` & `langchain_community-0.0.9/langchain_community/tools/office365/send_event.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/send_message.py` & `langchain_community-0.0.9/langchain_community/tools/office365/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/office365/utils.py` & `langchain_community-0.0.9/langchain_community/tools/office365/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/openapi/utils/api_models.py` & `langchain_community-0.0.9/langchain_community/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/openweathermap/tool.py` & `langchain_community-0.0.9/langchain_community/tools/openweathermap/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/__init__.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/base.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/click.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/click.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/current_page.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/current_page.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/extract_hyperlinks.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/extract_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/extract_text.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/extract_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/get_elements.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/get_elements.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/navigate.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/navigate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/navigate_back.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/navigate_back.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/playwright/utils.py` & `langchain_community-0.0.9/langchain_community/tools/playwright/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/plugin.py` & `langchain_community-0.0.9/langchain_community/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/powerbi/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/powerbi/tool.py` & `langchain_community-0.0.9/langchain_community/tools/powerbi/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/pubmed/tool.py` & `langchain_community-0.0.9/langchain_community/tools/pubmed/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/reddit_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/reddit_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/render.py` & `langchain_community-0.0.9/langchain_community/tools/render.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/requests/tool.py` & `langchain_community-0.0.9/langchain_community/tools/requests/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/scenexplain/tool.py` & `langchain_community-0.0.9/langchain_community/tools/scenexplain/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/searchapi/tool.py` & `langchain_community-0.0.9/langchain_community/tools/searchapi/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/searx_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/searx_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/semanticscholar/tool.py` & `langchain_community-0.0.9/langchain_community/tools/semanticscholar/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/shell/tool.py` & `langchain_community-0.0.9/langchain_community/tools/shell/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/slack/get_channel.py` & `langchain_community-0.0.9/langchain_community/tools/slack/get_channel.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/slack/get_message.py` & `langchain_community-0.0.9/langchain_community/tools/slack/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/slack/schedule_message.py` & `langchain_community-0.0.9/langchain_community/tools/slack/schedule_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/slack/send_message.py` & `langchain_community-0.0.9/langchain_community/tools/slack/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/slack/utils.py` & `langchain_community-0.0.9/langchain_community/tools/slack/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/sleep/tool.py` & `langchain_community-0.0.9/langchain_community/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/spark_sql/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/spark_sql/tool.py` & `langchain_community-0.0.9/langchain_community/tools/spark_sql/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/sql_database/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/sql_database/tool.py` & `langchain_community-0.0.9/langchain_community/tools/sql_database/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/stackexchange/tool.py` & `langchain_community-0.0.9/langchain_community/tools/stackexchange/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/steam/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/steam/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/steam/tool.py` & `langchain_community-0.0.9/langchain_community/tools/steam/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/steamship_image_generation/tool.py` & `langchain_community-0.0.9/langchain_community/tools/steamship_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/steamship_image_generation/utils.py` & `langchain_community-0.0.9/langchain_community/tools/steamship_image_generation/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/tavily_search/tool.py` & `langchain_community-0.0.9/langchain_community/tools/tavily_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/vectorstore/tool.py` & `langchain_community-0.0.9/langchain_community/tools/vectorstore/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/wikipedia/tool.py` & `langchain_community-0.0.9/langchain_community/tools/wikipedia/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/wolfram_alpha/tool.py` & `langchain_community-0.0.9/langchain_community/tools/wolfram_alpha/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/yahoo_finance_news.py` & `langchain_community-0.0.9/langchain_community/tools/yahoo_finance_news.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/youtube/search.py` & `langchain_community-0.0.9/langchain_community/tools/youtube/search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/zapier/prompt.py` & `langchain_community-0.0.9/langchain_community/tools/zapier/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/tools/zapier/tool.py` & `langchain_community-0.0.9/langchain_community/tools/zapier/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/__init__.py` & `langchain_community-0.0.9/langchain_community/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/alpha_vantage.py` & `langchain_community-0.0.9/langchain_community/utilities/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/anthropic.py` & `langchain_community-0.0.9/langchain_community/utilities/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/apify.py` & `langchain_community-0.0.9/langchain_community/utilities/apify.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/arcee.py` & `langchain_community-0.0.9/langchain_community/utilities/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/arxiv.py` & `langchain_community-0.0.9/langchain_community/utilities/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/awslambda.py` & `langchain_community-0.0.9/langchain_community/utilities/awslambda.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/bibtex.py` & `langchain_community-0.0.9/langchain_community/utilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/bing_search.py` & `langchain_community-0.0.9/langchain_community/utilities/bing_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/brave_search.py` & `langchain_community-0.0.9/langchain_community/utilities/brave_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/clickup.py` & `langchain_community-0.0.9/langchain_community/utilities/clickup.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/dalle_image_generator.py` & `langchain_community-0.0.9/langchain_community/utilities/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/dataforseo_api_search.py` & `langchain_community-0.0.9/langchain_community/utilities/dataforseo_api_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/duckduckgo_search.py` & `langchain_community-0.0.9/langchain_community/utilities/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/github.py` & `langchain_community-0.0.9/langchain_community/utilities/github.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/gitlab.py` & `langchain_community-0.0.9/langchain_community/utilities/gitlab.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/golden_query.py` & `langchain_community-0.0.9/langchain_community/utilities/golden_query.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_finance.py` & `langchain_community-0.0.9/langchain_community/utilities/google_finance.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_jobs.py` & `langchain_community-0.0.9/langchain_community/utilities/google_jobs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_lens.py` & `langchain_community-0.0.9/langchain_community/utilities/google_lens.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_places_api.py` & `langchain_community-0.0.9/langchain_community/utilities/google_places_api.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_scholar.py` & `langchain_community-0.0.9/langchain_community/utilities/google_scholar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_search.py` & `langchain_community-0.0.9/langchain_community/utilities/google_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_serper.py` & `langchain_community-0.0.9/langchain_community/utilities/google_serper.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/google_trends.py` & `langchain_community-0.0.9/langchain_community/utilities/google_trends.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/graphql.py` & `langchain_community-0.0.9/langchain_community/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/jira.py` & `langchain_community-0.0.9/langchain_community/utilities/jira.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/max_compute.py` & `langchain_community-0.0.9/langchain_community/utilities/max_compute.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/merriam_webster.py` & `langchain_community-0.0.9/langchain_community/utilities/merriam_webster.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/metaphor_search.py` & `langchain_community-0.0.9/langchain_community/utilities/metaphor_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/nasa.py` & `langchain_community-0.0.9/langchain_community/utilities/nasa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/opaqueprompts.py` & `langchain_community-0.0.9/langchain_community/utilities/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/openapi.py` & `langchain_community-0.0.9/langchain_community/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/openweathermap.py` & `langchain_community-0.0.9/langchain_community/utilities/openweathermap.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/outline.py` & `langchain_community-0.0.9/langchain_community/utilities/outline.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/portkey.py` & `langchain_community-0.0.9/langchain_community/utilities/portkey.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/powerbi.py` & `langchain_community-0.0.9/langchain_community/utilities/powerbi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/pubmed.py` & `langchain_community-0.0.9/langchain_community/utilities/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/python.py` & `langchain_community-0.0.9/langchain_community/utilities/python.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/reddit_search.py` & `langchain_community-0.0.9/langchain_community/utilities/reddit_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/redis.py` & `langchain_community-0.0.9/langchain_community/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/requests.py` & `langchain_community-0.0.9/langchain_community/utilities/requests.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/scenexplain.py` & `langchain_community-0.0.9/langchain_community/utilities/scenexplain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/searchapi.py` & `langchain_community-0.0.9/langchain_community/utilities/searchapi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/searx_search.py` & `langchain_community-0.0.9/langchain_community/utilities/searx_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/semanticscholar.py` & `langchain_community-0.0.9/langchain_community/utilities/semanticscholar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/serpapi.py` & `langchain_community-0.0.9/langchain_community/utilities/serpapi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/spark_sql.py` & `langchain_community-0.0.9/langchain_community/utilities/spark_sql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/sql_database.py` & `langchain_community-0.0.9/langchain_community/utilities/sql_database.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/stackexchange.py` & `langchain_community-0.0.9/langchain_community/utilities/stackexchange.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/steam.py` & `langchain_community-0.0.9/langchain_community/utilities/steam.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/tavily_search.py` & `langchain_community-0.0.9/langchain_community/utilities/tavily_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/tensorflow_datasets.py` & `langchain_community-0.0.9/langchain_community/utilities/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/twilio.py` & `langchain_community-0.0.9/langchain_community/utilities/twilio.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/vertexai.py` & `langchain_community-0.0.9/langchain_community/utilities/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/wikipedia.py` & `langchain_community-0.0.9/langchain_community/utilities/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/wolfram_alpha.py` & `langchain_community-0.0.9/langchain_community/utilities/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utilities/zapier.py` & `langchain_community-0.0.9/langchain_community/utilities/zapier.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utils/ernie_functions.py` & `langchain_community-0.0.9/langchain_community/utils/ernie_functions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/utils/math.py` & `langchain_community-0.0.9/langchain_community/utils/math.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/__init__.py` & `langchain_community-0.0.9/langchain_community/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/alibabacloud_opensearch.py` & `langchain_community-0.0.9/langchain_community/vectorstores/alibabacloud_opensearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/analyticdb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/analyticdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/annoy.py` & `langchain_community-0.0.9/langchain_community/vectorstores/annoy.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/astradb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/atlas.py` & `langchain_community-0.0.9/langchain_community/vectorstores/atlas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/awadb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/awadb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/azure_cosmos_db.py` & `langchain_community-0.0.9/langchain_community/vectorstores/azure_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/azuresearch.py` & `langchain_community-0.0.9/langchain_community/vectorstores/azuresearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/bageldb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/bageldb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/baiducloud_vector_search.py` & `langchain_community-0.0.9/langchain_community/vectorstores/baiducloud_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/bigquery_vector_search.py` & `langchain_community-0.0.9/langchain_community/vectorstores/bigquery_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/cassandra.py` & `langchain_community-0.0.9/langchain_community/vectorstores/cassandra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/chroma.py` & `langchain_community-0.0.9/langchain_community/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/clarifai.py` & `langchain_community-0.0.9/langchain_community/vectorstores/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/clickhouse.py` & `langchain_community-0.0.9/langchain_community/vectorstores/clickhouse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/dashvector.py` & `langchain_community-0.0.9/langchain_community/vectorstores/dashvector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/databricks_vector_search.py` & `langchain_community-0.0.9/langchain_community/vectorstores/databricks_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/deeplake.py` & `langchain_community-0.0.9/langchain_community/vectorstores/deeplake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/dingo.py` & `langchain_community-0.0.9/langchain_community/vectorstores/dingo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/docarray/base.py` & `langchain_community-0.0.9/langchain_community/vectorstores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/docarray/hnsw.py` & `langchain_community-0.0.9/langchain_community/vectorstores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/docarray/in_memory.py` & `langchain_community-0.0.9/langchain_community/vectorstores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/elastic_vector_search.py` & `langchain_community-0.0.9/langchain_community/vectorstores/elastic_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/elasticsearch.py` & `langchain_community-0.0.9/langchain_community/vectorstores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/epsilla.py` & `langchain_community-0.0.9/langchain_community/vectorstores/epsilla.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/faiss.py` & `langchain_community-0.0.9/langchain_community/vectorstores/faiss.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/hippo.py` & `langchain_community-0.0.9/langchain_community/vectorstores/hippo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/hologres.py` & `langchain_community-0.0.9/langchain_community/vectorstores/hologres.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/jaguar.py` & `langchain_community-0.0.9/langchain_community/vectorstores/jaguar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/lancedb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/lancedb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/llm_rails.py` & `langchain_community-0.0.9/langchain_community/vectorstores/llm_rails.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/marqo.py` & `langchain_community-0.0.9/langchain_community/vectorstores/marqo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/matching_engine.py` & `langchain_community-0.0.9/langchain_community/vectorstores/matching_engine.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/meilisearch.py` & `langchain_community-0.0.9/langchain_community/vectorstores/meilisearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/milvus.py` & `langchain_community-0.0.9/langchain_community/vectorstores/milvus.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,17 @@
         search_params: Optional[dict] = None,
         drop_old: Optional[bool] = False,
         *,
         primary_field: str = "pk",
         text_field: str = "text",
         vector_field: str = "vector",
         metadata_field: Optional[str] = None,
+        partition_names: Optional[list] = None,
+        replica_number: int = 1,
+        timeout: Optional[float] = None,
     ):
         """Initialize the Milvus vector store."""
         try:
             from pymilvus import Collection, utility
         except ImportError:
             raise ValueError(
                 "Could not import pymilvus python package. "
@@ -154,14 +157,18 @@
         self._primary_field = primary_field
         # In order for compatibility, the text field will need to be called "text"
         self._text_field = text_field
         # In order for compatibility, the vector field needs to be called "vector"
         self._vector_field = vector_field
         self._metadata_field = metadata_field
         self.fields: list[str] = []
+        self.partition_names = partition_names
+        self.replica_number = replica_number
+        self.timeout = timeout
+
         # Create the connection to the server
         if connection_args is None:
             connection_args = DEFAULT_MILVUS_CONNECTION
         self.alias = self._create_connection_alias(connection_args)
         self.col: Optional[Collection] = None
 
         # Grab the existing collection if it exists
@@ -172,15 +179,19 @@
             )
         # If need to drop old, drop it
         if drop_old and isinstance(self.col, Collection):
             self.col.drop()
             self.col = None
 
         # Initialize the vector store
-        self._init()
+        self._init(
+            partition_names=partition_names,
+            replica_number=replica_number,
+            timeout=timeout,
+        )
 
     @property
     def embeddings(self) -> Embeddings:
         return self.embedding_func
 
     def _create_connection_alias(self, connection_args: dict) -> str:
         """Create the connection to the Milvus server."""
@@ -231,22 +242,31 @@
             logger.debug("Created new connection using: %s", alias)
             return alias
         except MilvusException as e:
             logger.error("Failed to create new connection using: %s", alias)
             raise e
 
     def _init(
-        self, embeddings: Optional[list] = None, metadatas: Optional[list[dict]] = None
+        self,
+        embeddings: Optional[list] = None,
+        metadatas: Optional[list[dict]] = None,
+        partition_names: Optional[list] = None,
+        replica_number: int = 1,
+        timeout: Optional[float] = None,
     ) -> None:
         if embeddings is not None:
             self._create_collection(embeddings, metadatas)
         self._extract_fields()
         self._create_index()
         self._create_search_params()
-        self._load()
+        self._load(
+            partition_names=partition_names,
+            replica_number=replica_number,
+            timeout=timeout,
+        )
 
     def _create_collection(
         self, embeddings: list, metadatas: Optional[list[dict]] = None
     ) -> None:
         from pymilvus import (
             Collection,
             CollectionSchema,
@@ -392,20 +412,29 @@
             index = self._get_index()
             if index is not None:
                 index_type: str = index["index_param"]["index_type"]
                 metric_type: str = index["index_param"]["metric_type"]
                 self.search_params = self.default_search_params[index_type]
                 self.search_params["metric_type"] = metric_type
 
-    def _load(self) -> None:
+    def _load(
+        self,
+        partition_names: Optional[list] = None,
+        replica_number: int = 1,
+        timeout: Optional[float] = None,
+    ) -> None:
         """Load the collection if available."""
         from pymilvus import Collection
 
         if isinstance(self.col, Collection) and self._get_index() is not None:
-            self.col.load()
+            self.col.load(
+                partition_names=partition_names,
+                replica_number=replica_number,
+                timeout=timeout,
+            )
 
     def add_texts(
         self,
         texts: Iterable[str],
         metadatas: Optional[List[dict]] = None,
         timeout: Optional[int] = None,
         batch_size: int = 1000,
@@ -413,15 +442,15 @@
     ) -> List[str]:
         """Insert text data into Milvus.
 
         Inserting data when the collection has not be made yet will result
         in creating a new Collection. The data of the first entity decides
         the schema of the new collection, the dim is extracted from the first
         embedding and the columns are decided by the first metadata dict.
-        Metada keys will need to be present for all inserted values. At
+        Metadata keys will need to be present for all inserted values. At
         the moment there is no None equivalent in Milvus.
 
         Args:
             texts (Iterable[str]): The texts to embed, it is assumed
                 that they all fit in memory.
             metadatas (Optional[List[dict]]): Metadata dicts attached to each of
                 the texts. Defaults to None.
@@ -447,15 +476,22 @@
 
         if len(embeddings) == 0:
             logger.debug("Nothing to insert, skipping.")
             return []
 
         # If the collection hasn't been initialized yet, perform all steps to do so
         if not isinstance(self.col, Collection):
-            self._init(embeddings, metadatas)
+            kwargs = {"embeddings": embeddings, "metadatas": metadatas}
+            if self.partition_names:
+                kwargs["partition_names"] = self.partition_names
+            if self.replica_number:
+                kwargs["replica_number"] = self.replica_number
+            if self.timeout:
+                kwargs["timeout"] = self.timeout
+            self._init(**kwargs)
 
         # Dict to hold all insert columns
         insert_dict: dict[str, list] = {
             self._text_field: texts,
             self._vector_field: embeddings,
         }
```

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/momento_vector_index.py` & `langchain_community-0.0.9/langchain_community/vectorstores/momento_vector_index.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/mongodb_atlas.py` & `langchain_community-0.0.9/langchain_community/vectorstores/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/myscale.py` & `langchain_community-0.0.9/langchain_community/vectorstores/myscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/neo4j_vector.py` & `langchain_community-0.0.9/langchain_community/vectorstores/neo4j_vector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/nucliadb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/nucliadb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/opensearch_vector_search.py` & `langchain_community-0.0.9/langchain_community/vectorstores/opensearch_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/pgembedding.py` & `langchain_community-0.0.9/langchain_community/vectorstores/pgembedding.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/pgvecto_rs.py` & `langchain_community-0.0.9/langchain_community/vectorstores/pgvecto_rs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/pgvector.py` & `langchain_community-0.0.9/langchain_community/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/pinecone.py` & `langchain_community-0.0.9/langchain_community/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/qdrant.py` & `langchain_community-0.0.9/langchain_community/vectorstores/qdrant.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/redis/base.py` & `langchain_community-0.0.9/langchain_community/vectorstores/redis/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/redis/filters.py` & `langchain_community-0.0.9/langchain_community/vectorstores/redis/filters.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/redis/schema.py` & `langchain_community-0.0.9/langchain_community/vectorstores/redis/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/rocksetdb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/scann.py` & `langchain_community-0.0.9/langchain_community/vectorstores/scann.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/semadb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/semadb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/singlestoredb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/sklearn.py` & `langchain_community-0.0.9/langchain_community/vectorstores/sklearn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/sqlitevss.py` & `langchain_community-0.0.9/langchain_community/vectorstores/sqlitevss.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/starrocks.py` & `langchain_community-0.0.9/langchain_community/vectorstores/starrocks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/supabase.py` & `langchain_community-0.0.9/langchain_community/vectorstores/supabase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/surrealdb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/surrealdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/tair.py` & `langchain_community-0.0.9/langchain_community/vectorstores/tair.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/tencentvectordb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/tigris.py` & `langchain_community-0.0.9/langchain_community/vectorstores/tigris.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/tiledb.py` & `langchain_community-0.0.9/langchain_community/vectorstores/tiledb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/timescalevector.py` & `langchain_community-0.0.9/langchain_community/vectorstores/timescalevector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/typesense.py` & `langchain_community-0.0.9/langchain_community/vectorstores/typesense.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/usearch.py` & `langchain_community-0.0.9/langchain_community/vectorstores/usearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/utils.py` & `langchain_community-0.0.9/langchain_community/vectorstores/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/vald.py` & `langchain_community-0.0.9/langchain_community/vectorstores/vald.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/vearch.py` & `langchain_community-0.0.9/langchain_community/vectorstores/vearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/vectara.py` & `langchain_community-0.0.9/langchain_community/vectorstores/vectara.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/vespa.py` & `langchain_community-0.0.9/langchain_community/vectorstores/vespa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/weaviate.py` & `langchain_community-0.0.9/langchain_community/vectorstores/weaviate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/xata.py` & `langchain_community-0.0.9/langchain_community/vectorstores/xata.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/yellowbrick.py` & `langchain_community-0.0.9/langchain_community/vectorstores/yellowbrick.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/zep.py` & `langchain_community-0.0.9/langchain_community/vectorstores/zep.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/langchain_community/vectorstores/zilliz.py` & `langchain_community-0.0.9/langchain_community/vectorstores/zilliz.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.0.8/pyproject.toml` & `langchain_community-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "langchain-community"
-version = "0.0.8"
+version = "0.0.9"
 description = "Community contributed LangChain integrations."
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.1.5,<0.2"
+langchain-core = ">=0.1.7,<0.2"
 SQLAlchemy = ">=1.4,<3"
 requests = "^2"
 PyYAML = ">=5.3"
 numpy = "^1"
 aiohttp = "^3.8.3"
 tenacity = "^8.1.0"
 dataclasses-json = ">= 0.5.7, < 0.7"
@@ -137,15 +137,15 @@
 # See Contributing Guide for more instructions on working with optional dependencies.
 # https://python.langchain.com/docs/contributing/code#working-with-optional-dependencies
 pytest-vcr = "^1.0.2"
 wrapt = "^1.15.0"
 openai = "^1"
 python-dotenv = "^1.0.0"
 cassio = "^0.1.0"
-tiktoken = "^0.3.2"
+tiktoken = ">=0.3.2,<0.6.0"
 anthropic = "^0.3.11"
 langchain-core = { path = "../core", develop = true }
 fireworks-ai = "^0.9.0"
 boto3 = ">=1.28.57,<2"
 google-cloud-aiplatform = ">=1.37.0,<2"
 
 [tool.poetry.group.lint]
```

### Comparing `langchain_community-0.0.8/PKG-INFO` & `langchain_community-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-community
-Version: 0.0.8
+Version: 0.0.9
 Summary: Community contributed LangChain integrations.
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -43,15 +43,15 @@
 Requires-Dist: gradientai (>=1.4.0,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: hologres-vector (>=0.0.6,<0.0.7) ; extra == "extended-testing"
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0) ; extra == "extended-testing"
 Requires-Dist: javelin-sdk (>=0.1.8,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: jq (>=1.4.1,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: jsonschema (>1) ; extra == "extended-testing"
-Requires-Dist: langchain-core (>=0.1.5,<0.2)
+Requires-Dist: langchain-core (>=0.1.7,<0.2)
 Requires-Dist: langsmith (>=0.0.63,<0.1.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0) ; extra == "extended-testing"
 Requires-Dist: markdownify (>=0.11.6,<0.12.0) ; extra == "extended-testing"
 Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: msal (>=1.25.0,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: mwparserfromhell (>=0.6.4,<0.7.0) ; extra == "extended-testing"
 Requires-Dist: mwxml (>=0.3.3,<0.4.0) ; extra == "extended-testing"
```

