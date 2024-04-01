# Comparing `tmp/gigachain-0.1.7.1.tar.gz` & `tmp/gigachain-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain-0.1.7.1.tar", max compression
+gzip compressed data, was "gigachain-0.1.9.tar", max compression
```

## Comparing `gigachain-0.1.7.1.tar` & `gigachain-0.1.9.tar`

### file list

```diff
@@ -1,1338 +1,1338 @@
--rw-r--r--   0        0        0     1067 2023-11-15 10:30:09.324245 gigachain-0.1.7.1/LICENSE
--rw-r--r--   0        0        0     5879 2024-02-19 11:59:44.033252 gigachain-0.1.7.1/README.md
--rw-r--r--   0        0        0    14039 2024-02-19 11:59:44.036677 gigachain-0.1.7.1/langchain/__init__.py
--rw-r--r--   0        0        0      667 2023-10-03 14:24:35.511215 gigachain-0.1.7.1/langchain/_api/__init__.py
--rw-r--r--   0        0        0      471 2023-12-18 12:05:46.810499 gigachain-0.1.7.1/langchain/_api/deprecation.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:46.811728 gigachain-0.1.7.1/langchain/_api/path.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.531593 gigachain-0.1.7.1/langchain/adapters/__init__.py
--rw-r--r--   0        0        0      653 2024-01-10 09:04:40.316153 gigachain-0.1.7.1/langchain/adapters/openai.py
--rw-r--r--   0        0        0     4952 2024-01-30 14:52:09.424324 gigachain-0.1.7.1/langchain/agents/__init__.py
--rw-r--r--   0        0        0    54823 2024-02-19 11:59:44.041252 gigachain-0.1.7.1/langchain/agents/agent.py
--rw-r--r--   0        0        0    15135 2024-01-30 14:52:09.448072 gigachain-0.1.7.1/langchain/agents/agent_iterator.py
--rw-r--r--   0        0        0     3678 2024-02-05 09:38:07.003324 gigachain-0.1.7.1/langchain/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2023-08-24 07:36:02.856871 gigachain-0.1.7.1/langchain/agents/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:46.824912 gigachain-0.1.7.1/langchain/agents/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.825868 gigachain-0.1.7.1/langchain/agents/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:46.826776 gigachain-0.1.7.1/langchain/agents/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:46.827627 gigachain-0.1.7.1/langchain/agents/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2023-10-06 14:43:01.368502 gigachain-0.1.7.1/langchain/agents/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.828657 gigachain-0.1.7.1/langchain/agents/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.534160 gigachain-0.1.7.1/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0     3235 2023-12-18 12:05:46.830026 gigachain-0.1.7.1/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
--rw-r--r--   0        0        0       97 2023-10-30 16:05:53.823759 gigachain-0.1.7.1/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
--rw-r--r--   0        0        0     1091 2023-12-18 12:05:46.831119 gigachain-0.1.7.1/langchain/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      177 2024-01-18 15:16:40.601939 gigachain-0.1.7.1/langchain/agents/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.318190 gigachain-0.1.7.1/langchain/agents/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-21 13:51:28.536932 gigachain-0.1.7.1/langchain/agents/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0      617 2023-12-18 12:05:46.832827 gigachain-0.1.7.1/langchain/agents/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2023-09-19 14:33:02.213182 gigachain-0.1.7.1/langchain/agents/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.833490 gigachain-0.1.7.1/langchain/agents/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2023-08-21 13:51:28.537602 gigachain-0.1.7.1/langchain/agents/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.834225 gigachain-0.1.7.1/langchain/agents/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2023-08-21 13:51:28.538134 gigachain-0.1.7.1/langchain/agents/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.834919 gigachain-0.1.7.1/langchain/agents/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2023-08-21 13:51:28.538568 gigachain-0.1.7.1/langchain/agents/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.835830 gigachain-0.1.7.1/langchain/agents/agent_toolkits/json/base.py
--rw-r--r--   0        0        0      126 2023-12-18 12:05:46.837036 gigachain-0.1.7.1/langchain/agents/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.841473 gigachain-0.1.7.1/langchain/agents/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2023-08-21 13:51:28.539651 gigachain-0.1.7.1/langchain/agents/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.842445 gigachain-0.1.7.1/langchain/agents/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2023-12-18 12:05:46.842756 gigachain-0.1.7.1/langchain/agents/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.843062 gigachain-0.1.7.1/langchain/agents/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.540099 gigachain-0.1.7.1/langchain/agents/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:46.843983 gigachain-0.1.7.1/langchain/agents/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:46.844896 gigachain-0.1.7.1/langchain/agents/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2023-08-21 13:51:28.541150 gigachain-0.1.7.1/langchain/agents/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:46.845738 gigachain-0.1.7.1/langchain/agents/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2023-08-21 13:51:28.541736 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:46.846914 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0      530 2024-01-10 09:04:40.319042 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0     1153 2023-12-18 12:05:46.848467 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0      186 2023-12-18 12:05:46.849502 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:46.850112 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0      157 2023-12-18 12:05:46.850853 gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0     1104 2023-12-18 12:05:46.851835 gigachain-0.1.7.1/langchain/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0      174 2024-01-18 15:16:40.603187 gigachain-0.1.7.1/langchain/agents/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:46.852728 gigachain-0.1.7.1/langchain/agents/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-21 13:51:28.545958 gigachain-0.1.7.1/langchain/agents/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:46.853881 gigachain-0.1.7.1/langchain/agents/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:46.854708 gigachain-0.1.7.1/langchain/agents/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0      269 2023-12-18 12:05:46.855739 gigachain-0.1.7.1/langchain/agents/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.856940 gigachain-0.1.7.1/langchain/agents/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0     1094 2023-12-18 12:05:46.857872 gigachain-0.1.7.1/langchain/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:46.858297 gigachain-0.1.7.1/langchain/agents/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:46.859032 gigachain-0.1.7.1/langchain/agents/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0     1103 2023-12-18 12:05:46.860134 gigachain-0.1.7.1/langchain/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0       23 2023-08-21 13:51:28.548199 gigachain-0.1.7.1/langchain/agents/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0      123 2023-12-18 12:05:46.861223 gigachain-0.1.7.1/langchain/agents/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:46.862436 gigachain-0.1.7.1/langchain/agents/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:46.863534 gigachain-0.1.7.1/langchain/agents/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2023-08-21 13:51:28.549117 gigachain-0.1.7.1/langchain/agents/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.864520 gigachain-0.1.7.1/langchain/agents/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0      184 2023-12-18 12:05:46.865869 gigachain-0.1.7.1/langchain/agents/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:46.866709 gigachain-0.1.7.1/langchain/agents/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:46.867144 gigachain-0.1.7.1/langchain/agents/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:46.867506 gigachain-0.1.7.1/langchain/agents/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0       56 2023-08-21 13:51:28.549949 gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/__init__.py
--rw-r--r--   0        0        0     4211 2023-12-18 12:05:46.868458 gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/base.py
--rw-r--r--   0        0        0     1557 2023-08-31 07:54:47.805977 gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/prompt.py
--rw-r--r--   0        0        0     3001 2024-01-18 15:16:40.604061 gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/toolkit.py
--rw-r--r--   0        0        0     1095 2023-12-18 12:05:46.870552 gigachain-0.1.7.1/langchain/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2023-08-21 13:51:28.551302 gigachain-0.1.7.1/langchain/agents/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.871982 gigachain-0.1.7.1/langchain/agents/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0     1948 2024-01-30 12:21:20.018308 gigachain-0.1.7.1/langchain/agents/agent_types.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.551838 gigachain-0.1.7.1/langchain/agents/chat/__init__.py
--rw-r--r--   0        0        0     5084 2024-01-30 14:52:09.448709 gigachain-0.1.7.1/langchain/agents/chat/base.py
--rw-r--r--   0        0        0     1977 2024-02-19 11:59:44.043936 gigachain-0.1.7.1/langchain/agents/chat/output_parser.py
--rw-r--r--   0        0        0     1776 2023-10-19 12:57:52.688319 gigachain-0.1.7.1/langchain/agents/chat/prompt.py
--rw-r--r--   0        0        0       75 2023-08-21 13:51:28.552791 gigachain-0.1.7.1/langchain/agents/conversational/__init__.py
--rw-r--r--   0        0        0     4957 2024-01-30 14:52:09.450058 gigachain-0.1.7.1/langchain/agents/conversational/base.py
--rw-r--r--   0        0        0     1463 2024-02-19 11:59:44.046857 gigachain-0.1.7.1/langchain/agents/conversational/output_parser.py
--rw-r--r--   0        0        0     1312 2023-10-19 12:57:52.695256 gigachain-0.1.7.1/langchain/agents/conversational/prompt.py
--rw-r--r--   0        0        0       75 2023-08-21 13:51:28.553657 gigachain-0.1.7.1/langchain/agents/conversational_chat/__init__.py
--rw-r--r--   0        0        0     5264 2024-01-30 14:52:09.451543 gigachain-0.1.7.1/langchain/agents/conversational_chat/base.py
--rw-r--r--   0        0        0     2398 2024-02-19 11:59:44.047687 gigachain-0.1.7.1/langchain/agents/conversational_chat/output_parser.py
--rw-r--r--   0        0        0     2934 2023-10-19 12:57:52.702190 gigachain-0.1.7.1/langchain/agents/conversational_chat/prompt.py
--rw-r--r--   0        0        0      847 2023-11-10 13:07:49.983002 gigachain-0.1.7.1/langchain/agents/format_scratchpad/__init__.py
--rw-r--r--   0        0        0     2209 2024-01-30 14:52:09.453369 gigachain-0.1.7.1/langchain/agents/format_scratchpad/gigachat_functions.py
--rw-r--r--   0        0        0     1885 2024-01-30 14:52:09.454023 gigachain-0.1.7.1/langchain/agents/format_scratchpad/gigachat_tools.py
--rw-r--r--   0        0        0      528 2023-12-18 12:05:46.881864 gigachain-0.1.7.1/langchain/agents/format_scratchpad/log.py
--rw-r--r--   0        0        0      721 2023-12-18 12:05:46.882588 gigachain-0.1.7.1/langchain/agents/format_scratchpad/log_to_messages.py
--rw-r--r--   0        0        0     2203 2023-12-18 12:05:46.883234 gigachain-0.1.7.1/langchain/agents/format_scratchpad/openai_functions.py
--rw-r--r--   0        0        0     1885 2024-01-10 09:04:40.320052 gigachain-0.1.7.1/langchain/agents/format_scratchpad/openai_tools.py
--rw-r--r--   0        0        0      578 2023-12-18 12:05:46.884524 gigachain-0.1.7.1/langchain/agents/format_scratchpad/xml.py
--rw-r--r--   0        0        0        0 2024-01-30 14:52:09.454162 gigachain-0.1.7.1/langchain/agents/gigachat_functions_agent/__init__.py
--rw-r--r--   0        0        0     2567 2024-01-30 14:52:09.455188 gigachain-0.1.7.1/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0     4183 2024-02-19 11:59:44.050849 gigachain-0.1.7.1/langchain/agents/gigachat_functions_agent/base.py
--rw-r--r--   0        0        0        0 2024-01-30 14:52:09.456658 gigachain-0.1.7.1/langchain/agents/gigachat_tools/__init__.py
--rw-r--r--   0        0        0     3243 2024-01-30 14:52:09.457940 gigachain-0.1.7.1/langchain/agents/gigachat_tools/base.py
--rw-r--r--   0        0        0     3244 2024-01-30 14:52:09.458914 gigachain-0.1.7.1/langchain/agents/initialize.py
--rw-r--r--   0        0        0        0 2024-01-18 15:16:40.615878 gigachain-0.1.7.1/langchain/agents/json_chat/__init__.py
--rw-r--r--   0        0        0     6832 2024-02-19 11:59:44.052733 gigachain-0.1.7.1/langchain/agents/json_chat/base.py
--rw-r--r--   0        0        0      551 2024-01-18 15:16:40.617394 gigachain-0.1.7.1/langchain/agents/json_chat/prompt.py
--rw-r--r--   0        0        0    23921 2024-02-05 09:38:07.006461 gigachain-0.1.7.1/langchain/agents/load_tools.py
--rw-r--r--   0        0        0     4629 2024-02-05 09:38:07.008317 gigachain-0.1.7.1/langchain/agents/loading.py
--rw-r--r--   0        0        0       86 2023-08-21 13:51:28.555248 gigachain-0.1.7.1/langchain/agents/mrkl/__init__.py
--rw-r--r--   0        0        0     6046 2024-02-05 09:38:07.009352 gigachain-0.1.7.1/langchain/agents/mrkl/base.py
--rw-r--r--   0        0        0     3407 2024-02-19 11:59:44.053832 gigachain-0.1.7.1/langchain/agents/mrkl/output_parser.py
--rw-r--r--   0        0        0     1602 2023-12-18 12:05:46.889787 gigachain-0.1.7.1/langchain/agents/mrkl/prompt.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:46.890436 gigachain-0.1.7.1/langchain/agents/openai_assistant/__init__.py
--rw-r--r--   0        0        0    25732 2024-02-19 11:59:44.057021 gigachain-0.1.7.1/langchain/agents/openai_assistant/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556082 gigachain-0.1.7.1/langchain/agents/openai_functions_agent/__init__.py
--rw-r--r--   0        0        0     2567 2023-12-18 12:05:46.893881 gigachain-0.1.7.1/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0    11522 2024-02-05 09:38:07.013922 gigachain-0.1.7.1/langchain/agents/openai_functions_agent/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556705 gigachain-0.1.7.1/langchain/agents/openai_functions_multi_agent/__init__.py
--rw-r--r--   0        0        0    11944 2024-01-30 14:52:09.469737 gigachain-0.1.7.1/langchain/agents/openai_functions_multi_agent/base.py
--rw-r--r--   0        0        0        0 2024-01-18 15:16:40.628412 gigachain-0.1.7.1/langchain/agents/openai_tools/__init__.py
--rw-r--r--   0        0        0     3388 2024-02-05 09:38:07.015358 gigachain-0.1.7.1/langchain/agents/openai_tools/base.py
--rw-r--r--   0        0        0     1419 2024-01-30 14:52:09.472444 gigachain-0.1.7.1/langchain/agents/output_parsers/__init__.py
--rw-r--r--   0        0        0     3210 2024-02-06 09:21:29.047846 gigachain-0.1.7.1/langchain/agents/output_parsers/gigachat_functions.py
--rw-r--r--   0        0        0     1846 2024-01-30 14:52:09.474836 gigachain-0.1.7.1/langchain/agents/output_parsers/json.py
--rw-r--r--   0        0        0     3467 2024-01-18 15:16:40.630141 gigachain-0.1.7.1/langchain/agents/output_parsers/openai_functions.py
--rw-r--r--   0        0        0     3492 2024-01-18 15:16:40.631038 gigachain-0.1.7.1/langchain/agents/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     2455 2024-02-19 11:59:44.058015 gigachain-0.1.7.1/langchain/agents/output_parsers/react_json_single_input.py
--rw-r--r--   0        0        0     3218 2023-12-18 12:05:46.905924 gigachain-0.1.7.1/langchain/agents/output_parsers/react_single_input.py
--rw-r--r--   0        0        0     1545 2023-12-18 12:05:46.906825 gigachain-0.1.7.1/langchain/agents/output_parsers/self_ask.py
--rw-r--r--   0        0        0     1658 2023-12-18 12:05:46.907986 gigachain-0.1.7.1/langchain/agents/output_parsers/xml.py
--rw-r--r--   0        0        0       76 2023-08-21 13:51:28.557154 gigachain-0.1.7.1/langchain/agents/react/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-05 09:38:07.016302 gigachain-0.1.7.1/langchain/agents/react/agent.py
--rw-r--r--   0        0        0     5714 2024-01-30 14:52:09.476897 gigachain-0.1.7.1/langchain/agents/react/base.py
--rw-r--r--   0        0        0     1231 2023-12-18 12:05:46.909814 gigachain-0.1.7.1/langchain/agents/react/output_parser.py
--rw-r--r--   0        0        0     3005 2023-12-18 12:05:46.910755 gigachain-0.1.7.1/langchain/agents/react/textworld_prompt.py
--rw-r--r--   0        0        0    10562 2023-12-18 12:05:46.911736 gigachain-0.1.7.1/langchain/agents/react/wiki_prompt.py
--rw-r--r--   0        0        0     1175 2023-12-18 12:05:46.912970 gigachain-0.1.7.1/langchain/agents/schema.py
--rw-r--r--   0        0        0      106 2023-08-21 13:51:28.559443 gigachain-0.1.7.1/langchain/agents/self_ask_with_search/__init__.py
--rw-r--r--   0        0        0     8175 2024-02-05 09:38:07.018712 gigachain-0.1.7.1/langchain/agents/self_ask_with_search/base.py
--rw-r--r--   0        0        0      138 2023-09-25 07:40:35.498979 gigachain-0.1.7.1/langchain/agents/self_ask_with_search/output_parser.py
--rw-r--r--   0        0        0     3502 2023-12-18 12:05:46.916766 gigachain-0.1.7.1/langchain/agents/self_ask_with_search/prompt.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.560593 gigachain-0.1.7.1/langchain/agents/structured_chat/__init__.py
--rw-r--r--   0        0        0     9948 2024-02-05 09:38:07.019939 gigachain-0.1.7.1/langchain/agents/structured_chat/base.py
--rw-r--r--   0        0        0     3799 2024-02-19 11:59:44.059328 gigachain-0.1.7.1/langchain/agents/structured_chat/output_parser.py
--rw-r--r--   0        0        0     1663 2023-09-07 06:38:18.010991 gigachain-0.1.7.1/langchain/agents/structured_chat/prompt.py
--rw-r--r--   0        0        0     1409 2024-01-30 14:52:09.480078 gigachain-0.1.7.1/langchain/agents/tools.py
--rw-r--r--   0        0        0     1475 2024-01-29 08:25:46.514870 gigachain-0.1.7.1/langchain/agents/types.py
--rw-r--r--   0        0        0      384 2023-12-18 12:05:46.920460 gigachain-0.1.7.1/langchain/agents/utils.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.562209 gigachain-0.1.7.1/langchain/agents/xml/__init__.py
--rw-r--r--   0        0        0     7258 2024-02-05 09:38:07.021076 gigachain-0.1.7.1/langchain/agents/xml/base.py
--rw-r--r--   0        0        0      767 2024-01-18 15:16:40.638769 gigachain-0.1.7.1/langchain/agents/xml/prompt.py
--rw-r--r--   0        0        0      217 2023-12-18 12:05:46.922138 gigachain-0.1.7.1/langchain/base_language.py
--rw-r--r--   0        0        0      701 2024-01-10 09:04:40.325005 gigachain-0.1.7.1/langchain/cache.py
--rw-r--r--   0        0        0     2509 2024-02-05 09:38:07.023023 gigachain-0.1.7.1/langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      211 2023-12-18 12:05:46.925154 gigachain-0.1.7.1/langchain/callbacks/aim_callback.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.925829 gigachain-0.1.7.1/langchain/callbacks/argilla_callback.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:46.926936 gigachain-0.1.7.1/langchain/callbacks/arize_callback.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.325707 gigachain-0.1.7.1/langchain/callbacks/arthur_callback.py
--rw-r--r--   0        0        0      653 2024-01-30 14:52:09.481536 gigachain-0.1.7.1/langchain/callbacks/base.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.326482 gigachain-0.1.7.1/langchain/callbacks/clearml_callback.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.327283 gigachain-0.1.7.1/langchain/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:46.931986 gigachain-0.1.7.1/langchain/callbacks/confident_callback.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.328061 gigachain-0.1.7.1/langchain/callbacks/context_callback.py
--rw-r--r--   0        0        0     2589 2024-01-30 14:52:09.482134 gigachain-0.1.7.1/langchain/callbacks/file.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.328815 gigachain-0.1.7.1/langchain/callbacks/flyte_callback.py
--rw-r--r--   0        0        0      275 2024-01-10 09:04:40.329559 gigachain-0.1.7.1/langchain/callbacks/human.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.330500 gigachain-0.1.7.1/langchain/callbacks/infino_callback.py
--rw-r--r--   0        0        0      241 2023-12-18 12:05:46.936755 gigachain-0.1.7.1/langchain/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0      142 2024-01-10 09:04:40.331568 gigachain-0.1.7.1/langchain/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     1777 2023-12-18 12:05:46.938871 gigachain-0.1.7.1/langchain/callbacks/manager.py
--rw-r--r--   0        0        0      305 2024-01-10 09:04:40.332484 gigachain-0.1.7.1/langchain/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.333267 gigachain-0.1.7.1/langchain/callbacks/openai_info.py
--rw-r--r--   0        0        0      141 2024-01-10 09:04:40.333971 gigachain-0.1.7.1/langchain/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0      135 2024-01-10 09:04:40.334649 gigachain-0.1.7.1/langchain/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:46.944007 gigachain-0.1.7.1/langchain/callbacks/stdout.py
--rw-r--r--   0        0        0     2399 2024-01-30 14:52:09.482780 gigachain-0.1.7.1/langchain/callbacks/streaming_aiter.py
--rw-r--r--   0        0        0     3371 2023-12-18 12:05:46.945805 gigachain-0.1.7.1/langchain/callbacks/streaming_aiter_final_only.py
--rw-r--r--   0        0        0      173 2024-01-30 14:52:09.483494 gigachain-0.1.7.1/langchain/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     3357 2024-01-30 14:52:09.484144 gigachain-0.1.7.1/langchain/callbacks/streaming_stdout_final_only.py
--rw-r--r--   0        0        0     3190 2023-10-03 07:51:15.793630 gigachain-0.1.7.1/langchain/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0      185 2023-12-18 12:05:46.947518 gigachain-0.1.7.1/langchain/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0      490 2024-01-10 09:04:40.335344 gigachain-0.1.7.1/langchain/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      589 2023-12-18 12:05:46.949215 gigachain-0.1.7.1/langchain/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:46.950003 gigachain-0.1.7.1/langchain/callbacks/tracers/base.py
--rw-r--r--   0        0        0      154 2024-01-10 09:04:40.336248 gigachain-0.1.7.1/langchain/callbacks/tracers/comet.py
--rw-r--r--   0        0        0      233 2023-12-18 12:05:46.951869 gigachain-0.1.7.1/langchain/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      218 2023-12-18 12:05:46.952818 gigachain-0.1.7.1/langchain/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.953574 gigachain-0.1.7.1/langchain/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2023-12-18 12:05:46.954653 gigachain-0.1.7.1/langchain/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0     1384 2023-12-18 12:05:46.955043 gigachain-0.1.7.1/langchain/callbacks/tracers/logging.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.955825 gigachain-0.1.7.1/langchain/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.956667 gigachain-0.1.7.1/langchain/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2023-12-18 12:05:46.957919 gigachain-0.1.7.1/langchain/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      168 2023-12-18 12:05:46.958747 gigachain-0.1.7.1/langchain/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0      229 2024-01-10 09:04:40.336940 gigachain-0.1.7.1/langchain/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0      132 2024-01-10 09:04:40.337840 gigachain-0.1.7.1/langchain/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0      403 2023-12-18 12:05:46.961334 gigachain-0.1.7.1/langchain/callbacks/utils.py
--rw-r--r--   0        0        0      130 2024-01-10 09:04:40.338883 gigachain-0.1.7.1/langchain/callbacks/wandb_callback.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.339806 gigachain-0.1.7.1/langchain/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0     5951 2024-02-19 11:59:44.060249 gigachain-0.1.7.1/langchain/chains/__init__.py
--rw-r--r--   0        0        0       84 2023-08-21 13:51:28.576965 gigachain-0.1.7.1/langchain/chains/api/__init__.py
--rw-r--r--   0        0        0     8919 2024-01-30 14:52:09.484893 gigachain-0.1.7.1/langchain/chains/api/base.py
--rw-r--r--   0        0        0     2452 2024-01-10 09:04:40.341669 gigachain-0.1.7.1/langchain/chains/api/news_docs.py
--rw-r--r--   0        0        0     3399 2023-08-21 13:51:28.578041 gigachain-0.1.7.1/langchain/chains/api/open_meteo_docs.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.578278 gigachain-0.1.7.1/langchain/chains/api/openapi/__init__.py
--rw-r--r--   0        0        0     8786 2024-01-30 14:52:09.485529 gigachain-0.1.7.1/langchain/chains/api/openapi/chain.py
--rw-r--r--   0        0        0     1791 2023-08-21 13:51:28.579000 gigachain-0.1.7.1/langchain/chains/api/openapi/prompts.py
--rw-r--r--   0        0        0     2025 2023-12-18 12:05:46.968380 gigachain-0.1.7.1/langchain/chains/api/openapi/requests_chain.py
--rw-r--r--   0        0        0     1847 2023-12-18 12:05:46.969509 gigachain-0.1.7.1/langchain/chains/api/openapi/response_chain.py
--rw-r--r--   0        0        0     1920 2023-08-21 13:51:28.580702 gigachain-0.1.7.1/langchain/chains/api/podcast_docs.py
--rw-r--r--   0        0        0     1326 2023-12-18 12:05:46.970482 gigachain-0.1.7.1/langchain/chains/api/prompt.py
--rw-r--r--   0        0        0     1537 2023-08-21 13:51:28.581731 gigachain-0.1.7.1/langchain/chains/api/tmdb_docs.py
--rw-r--r--   0        0        0    28483 2024-02-19 11:59:44.064308 gigachain-0.1.7.1/langchain/chains/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.582802 gigachain-0.1.7.1/langchain/chains/chat_vector_db/__init__.py
--rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.972569 gigachain-0.1.7.1/langchain/chains/chat_vector_db/prompts.py
--rw-r--r--   0        0        0      367 2024-01-10 09:04:40.342648 gigachain-0.1.7.1/langchain/chains/combine_documents/__init__.py
--rw-r--r--   0        0        0     8052 2024-02-05 09:38:07.028425 gigachain-0.1.7.1/langchain/chains/combine_documents/base.py
--rw-r--r--   0        0        0     1743 2023-11-15 10:30:09.330835 gigachain-0.1.7.1/langchain/chains/combine_documents/conditional.py
--rw-r--r--   0        0        0    11739 2024-01-30 14:52:09.489218 gigachain-0.1.7.1/langchain/chains/combine_documents/map_reduce.py
--rw-r--r--   0        0        0     8949 2024-01-30 14:52:09.489828 gigachain-0.1.7.1/langchain/chains/combine_documents/map_rerank.py
--rw-r--r--   0        0        0    13894 2024-02-19 11:59:44.065836 gigachain-0.1.7.1/langchain/chains/combine_documents/reduce.py
--rw-r--r--   0        0        0     9113 2024-01-30 14:52:09.491341 gigachain-0.1.7.1/langchain/chains/combine_documents/refine.py
--rw-r--r--   0        0        0    11030 2024-01-30 14:52:09.493101 gigachain-0.1.7.1/langchain/chains/combine_documents/stuff.py
--rw-r--r--   0        0        0      107 2023-08-21 13:51:28.587546 gigachain-0.1.7.1/langchain/chains/constitutional_ai/__init__.py
--rw-r--r--   0        0        0     6341 2024-01-30 14:52:09.494092 gigachain-0.1.7.1/langchain/chains/constitutional_ai/base.py
--rw-r--r--   0        0        0      283 2023-12-18 12:05:46.981590 gigachain-0.1.7.1/langchain/chains/constitutional_ai/models.py
--rw-r--r--   0        0        0    21738 2023-08-21 13:51:28.588681 gigachain-0.1.7.1/langchain/chains/constitutional_ai/principles.py
--rw-r--r--   0        0        0    14534 2023-12-18 12:05:46.982679 gigachain-0.1.7.1/langchain/chains/constitutional_ai/prompts.py
--rw-r--r--   0        0        0       71 2023-08-21 13:51:28.589976 gigachain-0.1.7.1/langchain/chains/conversation/__init__.py
--rw-r--r--   0        0        0     2366 2024-01-18 15:16:40.657291 gigachain-0.1.7.1/langchain/chains/conversation/base.py
--rw-r--r--   0        0        0      856 2023-08-21 13:51:28.590517 gigachain-0.1.7.1/langchain/chains/conversation/memory.py
--rw-r--r--   0        0        0     1063 2023-12-18 12:05:46.984228 gigachain-0.1.7.1/langchain/chains/conversation/prompt.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.591153 gigachain-0.1.7.1/langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0    18065 2024-01-30 14:52:09.495867 gigachain-0.1.7.1/langchain/chains/conversational_retrieval/base.py
--rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.988192 gigachain-0.1.7.1/langchain/chains/conversational_retrieval/prompts.py
--rw-r--r--   0        0        0      126 2023-08-21 13:51:28.592942 gigachain-0.1.7.1/langchain/chains/elasticsearch_database/__init__.py
--rw-r--r--   0        0        0     8287 2024-01-30 14:52:09.496743 gigachain-0.1.7.1/langchain/chains/elasticsearch_database/base.py
--rw-r--r--   0        0        0     2480 2023-12-18 12:05:46.989727 gigachain-0.1.7.1/langchain/chains/elasticsearch_database/prompts.py
--rw-r--r--   0        0        0      669 2023-10-30 16:05:53.857849 gigachain-0.1.7.1/langchain/chains/encoder.py
--rw-r--r--   0        0        0      465 2023-12-18 12:05:46.990078 gigachain-0.1.7.1/langchain/chains/ernie_functions/__init__.py
--rw-r--r--   0        0        0    23289 2024-01-30 14:52:09.497422 gigachain-0.1.7.1/langchain/chains/ernie_functions/base.py
--rw-r--r--   0        0        0      741 2023-12-18 12:05:46.991949 gigachain-0.1.7.1/langchain/chains/example_generator.py
--rw-r--r--   0        0        0       51 2023-08-21 13:51:28.594704 gigachain-0.1.7.1/langchain/chains/flare/__init__.py
--rw-r--r--   0        0        0     9033 2024-01-30 14:52:09.498135 gigachain-0.1.7.1/langchain/chains/flare/base.py
--rw-r--r--   0        0        0     1949 2023-12-18 12:05:46.993539 gigachain-0.1.7.1/langchain/chains/flare/prompts.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.596462 gigachain-0.1.7.1/langchain/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0     8397 2024-01-30 14:52:09.499040 gigachain-0.1.7.1/langchain/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0     3671 2024-01-18 15:16:40.667708 gigachain-0.1.7.1/langchain/chains/graph_qa/base.py
--rw-r--r--   0        0        0    10452 2024-01-30 14:52:09.499619 gigachain-0.1.7.1/langchain/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0     9625 2023-12-18 12:05:46.997918 gigachain-0.1.7.1/langchain/chains/graph_qa/cypher_utils.py
--rw-r--r--   0        0        0     5272 2024-01-30 14:52:09.500412 gigachain-0.1.7.1/langchain/chains/graph_qa/falkordb.py
--rw-r--r--   0        0        0     3717 2024-01-30 14:52:09.501133 gigachain-0.1.7.1/langchain/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0     3698 2024-01-30 14:52:09.501760 gigachain-0.1.7.1/langchain/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0     3692 2024-01-30 14:52:09.502275 gigachain-0.1.7.1/langchain/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     6890 2024-01-30 14:52:09.502956 gigachain-0.1.7.1/langchain/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0     6610 2024-02-19 11:59:44.066669 gigachain-0.1.7.1/langchain/chains/graph_qa/neptune_sparql.py
--rw-r--r--   0        0        0     7226 2024-02-19 11:59:44.067927 gigachain-0.1.7.1/langchain/chains/graph_qa/ontotext_graphdb.py
--rw-r--r--   0        0        0    25955 2024-02-19 11:59:44.071989 gigachain-0.1.7.1/langchain/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0     5440 2024-01-30 14:52:09.503584 gigachain-0.1.7.1/langchain/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0     2662 2024-01-10 09:04:40.353033 gigachain-0.1.7.1/langchain/chains/history_aware_retriever.py
--rw-r--r--   0        0        0       75 2023-08-21 13:51:28.600763 gigachain-0.1.7.1/langchain/chains/hyde/__init__.py
--rw-r--r--   0        0        0     3341 2024-01-30 14:52:09.504159 gigachain-0.1.7.1/langchain/chains/hyde/base.py
--rw-r--r--   0        0        0     2482 2023-12-18 12:05:47.005583 gigachain-0.1.7.1/langchain/chains/hyde/prompts.py
--rw-r--r--   0        0        0    15030 2024-01-30 14:52:09.505741 gigachain-0.1.7.1/langchain/chains/llm.py
--rw-r--r--   0        0        0      450 2024-02-19 11:59:44.074835 gigachain-0.1.7.1/langchain/chains/llm_bash/__init__.py
--rw-r--r--   0        0        0      139 2023-08-21 13:51:28.604012 gigachain-0.1.7.1/langchain/chains/llm_checker/__init__.py
--rw-r--r--   0        0        0     6164 2024-01-30 14:52:09.506477 gigachain-0.1.7.1/langchain/chains/llm_checker/base.py
--rw-r--r--   0        0        0     1341 2023-12-18 12:05:47.009556 gigachain-0.1.7.1/langchain/chains/llm_checker/prompt.py
--rw-r--r--   0        0        0      143 2023-08-21 13:51:28.605454 gigachain-0.1.7.1/langchain/chains/llm_math/__init__.py
--rw-r--r--   0        0        0     6723 2024-01-30 14:52:09.507287 gigachain-0.1.7.1/langchain/chains/llm_math/base.py
--rw-r--r--   0        0        0     1158 2023-12-18 12:05:47.012133 gigachain-0.1.7.1/langchain/chains/llm_math/prompt.py
--rw-r--r--   0        0        0     3193 2024-01-30 14:52:09.507829 gigachain-0.1.7.1/langchain/chains/llm_requests.py
--rw-r--r--   0        0        0      352 2023-08-21 13:51:28.607135 gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/__init__.py
--rw-r--r--   0        0        0     6582 2024-02-19 11:59:44.076343 gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/base.py
--rw-r--r--   0        0        0     1143 2023-08-22 11:25:59.886227 gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
--rw-r--r--   0        0        0      696 2023-08-22 11:25:59.887142 gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
--rw-r--r--   0        0        0      234 2023-08-22 11:25:59.887992 gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
--rw-r--r--   0        0        0      834 2023-08-22 11:25:59.888905 gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
--rw-r--r--   0        0        0      467 2024-02-19 11:59:44.079463 gigachain-0.1.7.1/langchain/chains/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0    25297 2024-02-19 11:59:44.083239 gigachain-0.1.7.1/langchain/chains/loading.py
--rw-r--r--   0        0        0     3732 2024-01-30 14:52:09.509329 gigachain-0.1.7.1/langchain/chains/mapreduce.py
--rw-r--r--   0        0        0     3086 2024-02-19 11:59:44.084467 gigachain-0.1.7.1/langchain/chains/moderation.py
--rw-r--r--   0        0        0       96 2023-08-21 13:51:28.612079 gigachain-0.1.7.1/langchain/chains/natbot/__init__.py
--rw-r--r--   0        0        0     4695 2024-01-30 14:52:09.510954 gigachain-0.1.7.1/langchain/chains/natbot/base.py
--rw-r--r--   0        0        0    16050 2024-02-19 11:59:44.085897 gigachain-0.1.7.1/langchain/chains/natbot/crawler.py
--rw-r--r--   0        0        0     6769 2023-12-18 12:05:47.020892 gigachain-0.1.7.1/langchain/chains/natbot/prompt.py
--rw-r--r--   0        0        0     1357 2024-02-19 11:59:44.086856 gigachain-0.1.7.1/langchain/chains/openai_functions/__init__.py
--rw-r--r--   0        0        0    10075 2024-02-19 11:59:44.088105 gigachain-0.1.7.1/langchain/chains/openai_functions/base.py
--rw-r--r--   0        0        0     3526 2023-12-18 12:05:47.023612 gigachain-0.1.7.1/langchain/chains/openai_functions/citation_fuzzy_match.py
--rw-r--r--   0        0        0     4073 2024-02-13 15:39:43.470656 gigachain-0.1.7.1/langchain/chains/openai_functions/extraction.py
--rw-r--r--   0        0        0    11306 2024-01-30 14:52:09.513026 gigachain-0.1.7.1/langchain/chains/openai_functions/openapi.py
--rw-r--r--   0        0        0     3918 2023-12-18 12:05:47.026792 gigachain-0.1.7.1/langchain/chains/openai_functions/qa_with_structure.py
--rw-r--r--   0        0        0     2660 2023-12-18 12:05:47.027705 gigachain-0.1.7.1/langchain/chains/openai_functions/tagging.py
--rw-r--r--   0        0        0     1257 2023-08-21 13:51:28.616551 gigachain-0.1.7.1/langchain/chains/openai_functions/utils.py
--rw-r--r--   0        0        0      134 2023-11-10 13:07:50.024454 gigachain-0.1.7.1/langchain/chains/openai_tools/__init__.py
--rw-r--r--   0        0        0     1665 2024-01-30 14:52:09.513836 gigachain-0.1.7.1/langchain/chains/openai_tools/extraction.py
--rw-r--r--   0        0        0     2015 2023-12-18 12:05:47.029972 gigachain-0.1.7.1/langchain/chains/prompt_selector.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.617097 gigachain-0.1.7.1/langchain/chains/qa_generation/__init__.py
--rw-r--r--   0        0        0     2464 2024-01-30 14:52:09.514825 gigachain-0.1.7.1/langchain/chains/qa_generation/base.py
--rw-r--r--   0        0        0     2657 2023-12-18 12:05:47.032423 gigachain-0.1.7.1/langchain/chains/qa_generation/prompt.py
--rw-r--r--   0        0        0      173 2023-08-21 13:51:28.619059 gigachain-0.1.7.1/langchain/chains/qa_with_sources/__init__.py
--rw-r--r--   0        0        0     7976 2024-01-30 14:52:09.515775 gigachain-0.1.7.1/langchain/chains/qa_with_sources/base.py
--rw-r--r--   0        0        0     6793 2023-12-18 12:05:47.034152 gigachain-0.1.7.1/langchain/chains/qa_with_sources/loading.py
--rw-r--r--   0        0        0     4144 2023-12-18 12:05:47.035020 gigachain-0.1.7.1/langchain/chains/qa_with_sources/map_reduce_prompt.py
--rw-r--r--   0        0        0     1764 2023-12-18 12:05:47.035786 gigachain-0.1.7.1/langchain/chains/qa_with_sources/refine_prompts.py
--rw-r--r--   0        0        0     2459 2024-01-30 14:52:09.516490 gigachain-0.1.7.1/langchain/chains/qa_with_sources/retrieval.py
--rw-r--r--   0        0        0     3471 2023-12-18 12:05:47.037437 gigachain-0.1.7.1/langchain/chains/qa_with_sources/stuff_prompt.py
--rw-r--r--   0        0        0     2770 2024-01-30 14:52:09.517232 gigachain-0.1.7.1/langchain/chains/qa_with_sources/vector_db.py
--rw-r--r--   0        0        0      131 2024-02-19 11:59:44.089276 gigachain-0.1.7.1/langchain/chains/query_constructor/__init__.py
--rw-r--r--   0        0        0    13721 2024-02-19 11:59:44.092907 gigachain-0.1.7.1/langchain/chains/query_constructor/base.py
--rw-r--r--   0        0        0     3191 2023-12-18 12:05:47.039898 gigachain-0.1.7.1/langchain/chains/query_constructor/ir.py
--rw-r--r--   0        0        0     5707 2023-12-18 12:05:47.040791 gigachain-0.1.7.1/langchain/chains/query_constructor/parser.py
--rw-r--r--   0        0        0    10146 2023-12-18 12:05:47.041579 gigachain-0.1.7.1/langchain/chains/query_constructor/prompt.py
--rw-r--r--   0        0        0      321 2023-12-18 12:05:47.042242 gigachain-0.1.7.1/langchain/chains/query_constructor/schema.py
--rw-r--r--   0        0        0     8503 2024-01-30 14:52:09.520520 gigachain-0.1.7.1/langchain/chains/question_answering/__init__.py
--rw-r--r--   0        0        0     5425 2023-12-18 12:05:47.043620 gigachain-0.1.7.1/langchain/chains/question_answering/map_reduce_prompt.py
--rw-r--r--   0        0        0     2477 2023-12-18 12:05:47.044547 gigachain-0.1.7.1/langchain/chains/question_answering/map_rerank_prompt.py
--rw-r--r--   0        0        0     3133 2023-12-18 12:05:47.045293 gigachain-0.1.7.1/langchain/chains/question_answering/refine_prompts.py
--rw-r--r--   0        0        0     1404 2023-12-18 12:05:47.046327 gigachain-0.1.7.1/langchain/chains/question_answering/stuff_prompt.py
--rw-r--r--   0        0        0     2742 2024-01-18 15:16:40.690412 gigachain-0.1.7.1/langchain/chains/retrieval.py
--rw-r--r--   0        0        0       62 2023-08-21 13:51:28.631121 gigachain-0.1.7.1/langchain/chains/retrieval_qa/__init__.py
--rw-r--r--   0        0        0     9952 2024-01-30 14:52:09.521401 gigachain-0.1.7.1/langchain/chains/retrieval_qa/base.py
--rw-r--r--   0        0        0      527 2023-12-18 12:05:47.048474 gigachain-0.1.7.1/langchain/chains/retrieval_qa/prompt.py
--rw-r--r--   0        0        0      407 2023-08-21 13:51:28.632647 gigachain-0.1.7.1/langchain/chains/router/__init__.py
--rw-r--r--   0        0        0     4571 2024-01-30 14:52:09.522373 gigachain-0.1.7.1/langchain/chains/router/base.py
--rw-r--r--   0        0        0     1982 2024-01-30 14:52:09.523128 gigachain-0.1.7.1/langchain/chains/router/embedding_router.py
--rw-r--r--   0        0        0     4283 2024-01-30 14:52:09.524077 gigachain-0.1.7.1/langchain/chains/router/llm_router.py
--rw-r--r--   0        0        0     2245 2023-12-18 12:05:47.052334 gigachain-0.1.7.1/langchain/chains/router/multi_prompt.py
--rw-r--r--   0        0        0     1849 2023-09-04 05:57:22.503454 gigachain-0.1.7.1/langchain/chains/router/multi_prompt_prompt.py
--rw-r--r--   0        0        0     1904 2023-08-21 14:03:46.158141 gigachain-0.1.7.1/langchain/chains/router/multi_retrieval_prompt.py
--rw-r--r--   0        0        0     3659 2024-01-18 15:16:40.692341 gigachain-0.1.7.1/langchain/chains/router/multi_retrieval_qa.py
--rw-r--r--   0        0        0     7510 2024-01-30 14:52:09.524946 gigachain-0.1.7.1/langchain/chains/sequential.py
--rw-r--r--   0        0        0       47 2023-08-21 13:51:28.636997 gigachain-0.1.7.1/langchain/chains/sql_database/__init__.py
--rw-r--r--   0        0        0    30619 2024-01-30 14:52:09.527171 gigachain-0.1.7.1/langchain/chains/sql_database/prompt.py
--rw-r--r--   0        0        0     5293 2024-02-05 09:38:07.034504 gigachain-0.1.7.1/langchain/chains/sql_database/query.py
--rw-r--r--   0        0        0      204 2024-02-19 11:59:44.093587 gigachain-0.1.7.1/langchain/chains/structured_output/__init__.py
--rw-r--r--   0        0        0    15509 2024-02-19 11:59:44.094244 gigachain-0.1.7.1/langchain/chains/structured_output/base.py
--rw-r--r--   0        0        0     6711 2024-02-19 11:59:44.097491 gigachain-0.1.7.1/langchain/chains/summarize/__init__.py
--rw-r--r--   0        0        0      271 2023-12-18 12:05:47.059118 gigachain-0.1.7.1/langchain/chains/summarize/map_reduce_prompt.py
--rw-r--r--   0        0        0     1138 2023-12-18 12:05:47.060439 gigachain-0.1.7.1/langchain/chains/summarize/refine_prompts.py
--rw-r--r--   0        0        0      271 2023-12-18 12:05:47.061163 gigachain-0.1.7.1/langchain/chains/summarize/stuff_prompt.py
--rw-r--r--   0        0        0     2369 2024-01-30 14:52:09.529553 gigachain-0.1.7.1/langchain/chains/transform.py
--rw-r--r--   0        0        0      452 2023-09-12 10:52:10.662329 gigachain-0.1.7.1/langchain/chat_loaders/__init__.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.064850 gigachain-0.1.7.1/langchain/chat_loaders/base.py
--rw-r--r--   0        0        0      240 2023-12-18 12:05:47.066006 gigachain-0.1.7.1/langchain/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0       99 2024-01-10 09:04:40.356789 gigachain-0.1.7.1/langchain/chat_loaders/gmail.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.067658 gigachain-0.1.7.1/langchain/chat_loaders/imessage.py
--rw-r--r--   0        0        0      187 2023-12-18 12:05:47.068610 gigachain-0.1.7.1/langchain/chat_loaders/langsmith.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.069730 gigachain-0.1.7.1/langchain/chat_loaders/slack.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.070887 gigachain-0.1.7.1/langchain/chat_loaders/telegram.py
--rw-r--r--   0        0        0      290 2023-12-18 12:05:47.071655 gigachain-0.1.7.1/langchain/chat_loaders/utils.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.072872 gigachain-0.1.7.1/langchain/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     1995 2024-01-18 15:16:40.697309 gigachain-0.1.7.1/langchain/chat_models/__init__.py
--rw-r--r--   0        0        0      199 2024-01-10 09:04:40.357806 gigachain-0.1.7.1/langchain/chat_models/anthropic.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.358738 gigachain-0.1.7.1/langchain/chat_models/anyscale.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.078945 gigachain-0.1.7.1/langchain/chat_models/azure_openai.py
--rw-r--r--   0        0        0      189 2023-12-18 12:05:47.080365 gigachain-0.1.7.1/langchain/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.359766 gigachain-0.1.7.1/langchain/chat_models/baichuan.py
--rw-r--r--   0        0        0      131 2024-01-10 09:04:40.360897 gigachain-0.1.7.1/langchain/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      268 2024-01-10 09:04:40.361805 gigachain-0.1.7.1/langchain/chat_models/base.py
--rw-r--r--   0        0        0      131 2023-12-18 12:05:47.084089 gigachain-0.1.7.1/langchain/chat_models/bedrock.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.362621 gigachain-0.1.7.1/langchain/chat_models/cohere.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.085569 gigachain-0.1.7.1/langchain/chat_models/databricks.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.363366 gigachain-0.1.7.1/langchain/chat_models/ernie.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.364542 gigachain-0.1.7.1/langchain/chat_models/everlyai.py
--rw-r--r--   0        0        0      169 2023-12-18 12:05:47.088330 gigachain-0.1.7.1/langchain/chat_models/fake.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.365619 gigachain-0.1.7.1/langchain/chat_models/fireworks.py
--rw-r--r--   0        0        0       95 2024-01-10 09:04:40.366318 gigachain-0.1.7.1/langchain/chat_models/gigachat.py
--rw-r--r--   0        0        0      158 2024-01-10 09:04:40.367091 gigachain-0.1.7.1/langchain/chat_models/google_palm.py
--rw-r--r--   0        0        0      114 2024-01-10 09:04:40.367972 gigachain-0.1.7.1/langchain/chat_models/human.py
--rw-r--r--   0        0        0      107 2024-01-10 09:04:40.368737 gigachain-0.1.7.1/langchain/chat_models/hunyuan.py
--rw-r--r--   0        0        0      159 2024-01-10 09:04:40.369542 gigachain-0.1.7.1/langchain/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0      102 2024-01-10 09:04:40.370300 gigachain-0.1.7.1/langchain/chat_models/jinachat.py
--rw-r--r--   0        0        0       94 2024-01-10 09:04:40.371073 gigachain-0.1.7.1/langchain/chat_models/konko.py
--rw-r--r--   0        0        0      137 2024-01-10 09:04:40.371862 gigachain-0.1.7.1/langchain/chat_models/litellm.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.372837 gigachain-0.1.7.1/langchain/chat_models/meta.py
--rw-r--r--   0        0        0      100 2024-01-10 09:04:40.373952 gigachain-0.1.7.1/langchain/chat_models/minimax.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.098332 gigachain-0.1.7.1/langchain/chat_models/mlflow.py
--rw-r--r--   0        0        0      156 2024-01-10 09:04:40.375069 gigachain-0.1.7.1/langchain/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.375700 gigachain-0.1.7.1/langchain/chat_models/ollama.py
--rw-r--r--   0        0        0      104 2024-01-10 09:04:40.377001 gigachain-0.1.7.1/langchain/chat_models/openai.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.102210 gigachain-0.1.7.1/langchain/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.103242 gigachain-0.1.7.1/langchain/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0      104 2024-01-10 09:04:40.377793 gigachain-0.1.7.1/langchain/chat_models/tongyi.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.378622 gigachain-0.1.7.1/langchain/chat_models/vertexai.py
--rw-r--r--   0        0        0      178 2024-01-10 09:04:40.379547 gigachain-0.1.7.1/langchain/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.380328 gigachain-0.1.7.1/langchain/chat_models/yandex.py
--rw-r--r--   0        0        0     1184 2024-02-05 09:38:07.036821 gigachain-0.1.7.1/langchain/docstore/__init__.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.107159 gigachain-0.1.7.1/langchain/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.107958 gigachain-0.1.7.1/langchain/docstore/base.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:47.108669 gigachain-0.1.7.1/langchain/docstore/document.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.109501 gigachain-0.1.7.1/langchain/docstore/in_memory.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.110273 gigachain-0.1.7.1/langchain/docstore/wikipedia.py
--rw-r--r--   0        0        0     5722 2024-02-05 09:38:07.038977 gigachain-0.1.7.1/langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.112427 gigachain-0.1.7.1/langchain/document_loaders/acreom.py
--rw-r--r--   0        0        0      554 2023-12-18 12:05:47.113265 gigachain-0.1.7.1/langchain/document_loaders/airbyte.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.114177 gigachain-0.1.7.1/langchain/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.115207 gigachain-0.1.7.1/langchain/document_loaders/airtable.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.116053 gigachain-0.1.7.1/langchain/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.381440 gigachain-0.1.7.1/langchain/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.117596 gigachain-0.1.7.1/langchain/document_loaders/arxiv.py
--rw-r--r--   0        0        0      190 2023-12-18 12:05:47.118350 gigachain-0.1.7.1/langchain/document_loaders/assemblyai.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.382547 gigachain-0.1.7.1/langchain/document_loaders/async_html.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.120014 gigachain-0.1.7.1/langchain/document_loaders/azlyrics.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.120412 gigachain-0.1.7.1/langchain/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0      166 2023-12-18 12:05:47.121235 gigachain-0.1.7.1/langchain/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0      151 2023-12-18 12:05:47.122051 gigachain-0.1.7.1/langchain/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0      146 2023-12-18 12:05:47.122866 gigachain-0.1.7.1/langchain/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.123637 gigachain-0.1.7.1/langchain/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.124374 gigachain-0.1.7.1/langchain/document_loaders/base.py
--rw-r--r--   0        0        0      120 2024-01-10 09:04:40.383758 gigachain-0.1.7.1/langchain/document_loaders/base_o365.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.125960 gigachain-0.1.7.1/langchain/document_loaders/bibtex.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.126880 gigachain-0.1.7.1/langchain/document_loaders/bigquery.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.127706 gigachain-0.1.7.1/langchain/document_loaders/bilibili.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.128455 gigachain-0.1.7.1/langchain/document_loaders/blackboard.py
--rw-r--r--   0        0        0      374 2024-01-18 15:16:40.702123 gigachain-0.1.7.1/langchain/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0      140 2024-01-10 09:04:40.384621 gigachain-0.1.7.1/langchain/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.130737 gigachain-0.1.7.1/langchain/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.131488 gigachain-0.1.7.1/langchain/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0      172 2023-12-18 12:05:47.132145 gigachain-0.1.7.1/langchain/document_loaders/blockchain.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.132987 gigachain-0.1.7.1/langchain/document_loaders/brave_search.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.133606 gigachain-0.1.7.1/langchain/document_loaders/browserless.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.134633 gigachain-0.1.7.1/langchain/document_loaders/chatgpt.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.135559 gigachain-0.1.7.1/langchain/document_loaders/chromium.py
--rw-r--r--   0        0        0      146 2023-12-18 12:05:47.137221 gigachain-0.1.7.1/langchain/document_loaders/college_confidential.py
--rw-r--r--   0        0        0      118 2024-01-10 09:04:40.385398 gigachain-0.1.7.1/langchain/document_loaders/concurrent.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:47.139495 gigachain-0.1.7.1/langchain/document_loaders/confluence.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.141295 gigachain-0.1.7.1/langchain/document_loaders/conllu.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.141905 gigachain-0.1.7.1/langchain/document_loaders/couchbase.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:47.142595 gigachain-0.1.7.1/langchain/document_loaders/csv_loader.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.143458 gigachain-0.1.7.1/langchain/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.144613 gigachain-0.1.7.1/langchain/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0      163 2023-12-18 12:05:47.145949 gigachain-0.1.7.1/langchain/document_loaders/dataframe.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.147296 gigachain-0.1.7.1/langchain/document_loaders/diffbot.py
--rw-r--r--   0        0        0      115 2024-01-10 09:04:40.386259 gigachain-0.1.7.1/langchain/document_loaders/directory.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.149307 gigachain-0.1.7.1/langchain/document_loaders/discord.py
--rw-r--r--   0        0        0      119 2024-01-10 09:04:40.387645 gigachain-0.1.7.1/langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.150906 gigachain-0.1.7.1/langchain/document_loaders/docusaurus.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.151662 gigachain-0.1.7.1/langchain/document_loaders/dropbox.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.152424 gigachain-0.1.7.1/langchain/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0      177 2023-12-18 12:05:47.153750 gigachain-0.1.7.1/langchain/document_loaders/email.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.154940 gigachain-0.1.7.1/langchain/document_loaders/epub.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.156146 gigachain-0.1.7.1/langchain/document_loaders/etherscan.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.156948 gigachain-0.1.7.1/langchain/document_loaders/evernote.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.158021 gigachain-0.1.7.1/langchain/document_loaders/excel.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.158818 gigachain-0.1.7.1/langchain/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.160349 gigachain-0.1.7.1/langchain/document_loaders/fauna.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.161384 gigachain-0.1.7.1/langchain/document_loaders/figma.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.163101 gigachain-0.1.7.1/langchain/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.164293 gigachain-0.1.7.1/langchain/document_loaders/gcs_file.py
--rw-r--r--   0        0        0      109 2024-01-10 09:04:40.388322 gigachain-0.1.7.1/langchain/document_loaders/generic.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.166270 gigachain-0.1.7.1/langchain/document_loaders/geodataframe.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.167324 gigachain-0.1.7.1/langchain/document_loaders/git.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.168806 gigachain-0.1.7.1/langchain/document_loaders/gitbook.py
--rw-r--r--   0        0        0      160 2023-12-18 12:05:47.169956 gigachain-0.1.7.1/langchain/document_loaders/github.py
--rw-r--r--   0        0        0      145 2023-12-18 12:05:47.171116 gigachain-0.1.7.1/langchain/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.389172 gigachain-0.1.7.1/langchain/document_loaders/googledrive.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.173144 gigachain-0.1.7.1/langchain/document_loaders/gutenberg.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.174366 gigachain-0.1.7.1/langchain/document_loaders/helpers.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.175285 gigachain-0.1.7.1/langchain/document_loaders/hn.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.176378 gigachain-0.1.7.1/langchain/document_loaders/html.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.177108 gigachain-0.1.7.1/langchain/document_loaders/html_bs.py
--rw-r--r--   0        0        0      144 2023-12-18 12:05:47.178240 gigachain-0.1.7.1/langchain/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.389976 gigachain-0.1.7.1/langchain/document_loaders/ifixit.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.180404 gigachain-0.1.7.1/langchain/document_loaders/image.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.181253 gigachain-0.1.7.1/langchain/document_loaders/image_captions.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.182514 gigachain-0.1.7.1/langchain/document_loaders/imsdb.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.390811 gigachain-0.1.7.1/langchain/document_loaders/iugu.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.391872 gigachain-0.1.7.1/langchain/document_loaders/joplin.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.184945 gigachain-0.1.7.1/langchain/document_loaders/json_loader.py
--rw-r--r--   0        0        0      198 2023-12-18 12:05:47.185665 gigachain-0.1.7.1/langchain/document_loaders/lakefs.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.186694 gigachain-0.1.7.1/langchain/document_loaders/larksuite.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.188009 gigachain-0.1.7.1/langchain/document_loaders/markdown.py
--rw-r--r--   0        0        0      122 2024-01-10 09:04:40.392640 gigachain-0.1.7.1/langchain/document_loaders/mastodon.py
--rw-r--r--   0        0        0      110 2023-12-18 12:05:47.190950 gigachain-0.1.7.1/langchain/document_loaders/max_compute.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.191580 gigachain-0.1.7.1/langchain/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.192413 gigachain-0.1.7.1/langchain/document_loaders/merge.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.193132 gigachain-0.1.7.1/langchain/document_loaders/mhtml.py
--rw-r--r--   0        0        0      131 2024-01-10 09:04:40.393450 gigachain-0.1.7.1/langchain/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.195107 gigachain-0.1.7.1/langchain/document_loaders/mongodb.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.196443 gigachain-0.1.7.1/langchain/document_loaders/news.py
--rw-r--r--   0        0        0      196 2023-12-18 12:05:47.198825 gigachain-0.1.7.1/langchain/document_loaders/notebook.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.199713 gigachain-0.1.7.1/langchain/document_loaders/notion.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.394263 gigachain-0.1.7.1/langchain/document_loaders/notiondb.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.201509 gigachain-0.1.7.1/langchain/document_loaders/nuclia.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.202637 gigachain-0.1.7.1/langchain/document_loaders/obs_directory.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.203432 gigachain-0.1.7.1/langchain/document_loaders/obs_file.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.204584 gigachain-0.1.7.1/langchain/document_loaders/obsidian.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.205631 gigachain-0.1.7.1/langchain/document_loaders/odt.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.206554 gigachain-0.1.7.1/langchain/document_loaders/onedrive.py
--rw-r--r--   0        0        0      125 2024-01-10 09:04:40.395058 gigachain-0.1.7.1/langchain/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0      109 2024-01-10 09:04:40.395856 gigachain-0.1.7.1/langchain/document_loaders/onenote.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.209150 gigachain-0.1.7.1/langchain/document_loaders/open_city_data.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.209977 gigachain-0.1.7.1/langchain/document_loaders/org_mode.py
--rw-r--r--   0        0        0      789 2024-01-18 15:16:40.703524 gigachain-0.1.7.1/langchain/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0      225 2023-12-18 12:05:47.210876 gigachain-0.1.7.1/langchain/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.211715 gigachain-0.1.7.1/langchain/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.212945 gigachain-0.1.7.1/langchain/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0      176 2024-01-10 09:04:40.397095 gigachain-0.1.7.1/langchain/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      109 2024-01-18 15:16:40.704455 gigachain-0.1.7.1/langchain/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.214977 gigachain-0.1.7.1/langchain/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      136 2024-01-18 15:16:40.705628 gigachain-0.1.7.1/langchain/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.216206 gigachain-0.1.7.1/langchain/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.217158 gigachain-0.1.7.1/langchain/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.217871 gigachain-0.1.7.1/langchain/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.218842 gigachain-0.1.7.1/langchain/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.219645 gigachain-0.1.7.1/langchain/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.220840 gigachain-0.1.7.1/langchain/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0      494 2024-01-10 09:04:40.398416 gigachain-0.1.7.1/langchain/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.399315 gigachain-0.1.7.1/langchain/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.223502 gigachain-0.1.7.1/langchain/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0      706 2023-12-18 12:05:47.224305 gigachain-0.1.7.1/langchain/document_loaders/pdf.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.225423 gigachain-0.1.7.1/langchain/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.226416 gigachain-0.1.7.1/langchain/document_loaders/powerpoint.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.227234 gigachain-0.1.7.1/langchain/document_loaders/psychic.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.228478 gigachain-0.1.7.1/langchain/document_loaders/pubmed.py
--rw-r--r--   0        0        0      137 2023-12-18 12:05:47.229728 gigachain-0.1.7.1/langchain/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.230746 gigachain-0.1.7.1/langchain/document_loaders/python.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.400297 gigachain-0.1.7.1/langchain/document_loaders/quip.py
--rw-r--r--   0        0        0      128 2024-01-10 09:04:40.401198 gigachain-0.1.7.1/langchain/document_loaders/readthedocs.py
--rw-r--r--   0        0        0      132 2024-01-10 09:04:40.402205 gigachain-0.1.7.1/langchain/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.403129 gigachain-0.1.7.1/langchain/document_loaders/reddit.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.234795 gigachain-0.1.7.1/langchain/document_loaders/roam.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.403904 gigachain-0.1.7.1/langchain/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.236908 gigachain-0.1.7.1/langchain/document_loaders/rspace.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:47.237697 gigachain-0.1.7.1/langchain/document_loaders/rss.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.238291 gigachain-0.1.7.1/langchain/document_loaders/rst.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.239100 gigachain-0.1.7.1/langchain/document_loaders/rtf.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.239781 gigachain-0.1.7.1/langchain/document_loaders/s3_directory.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.240496 gigachain-0.1.7.1/langchain/document_loaders/s3_file.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.241193 gigachain-0.1.7.1/langchain/document_loaders/sharepoint.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.404728 gigachain-0.1.7.1/langchain/document_loaders/sitemap.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.243092 gigachain-0.1.7.1/langchain/document_loaders/slack_directory.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.243833 gigachain-0.1.7.1/langchain/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.405568 gigachain-0.1.7.1/langchain/document_loaders/spreedly.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.245722 gigachain-0.1.7.1/langchain/document_loaders/srt.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.406422 gigachain-0.1.7.1/langchain/document_loaders/stripe.py
--rw-r--r--   0        0        0      275 2023-12-18 12:05:47.248314 gigachain-0.1.7.1/langchain/document_loaders/telegram.py
--rw-r--r--   0        0        0      147 2023-12-18 12:05:47.249456 gigachain-0.1.7.1/langchain/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0      123 2023-12-18 12:05:47.250244 gigachain-0.1.7.1/langchain/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.250861 gigachain-0.1.7.1/langchain/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.251412 gigachain-0.1.7.1/langchain/document_loaders/text.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.252277 gigachain-0.1.7.1/langchain/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.253561 gigachain-0.1.7.1/langchain/document_loaders/toml.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.254464 gigachain-0.1.7.1/langchain/document_loaders/trello.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.255363 gigachain-0.1.7.1/langchain/document_loaders/tsv.py
--rw-r--r--   0        0        0      119 2024-01-10 09:04:40.407370 gigachain-0.1.7.1/langchain/document_loaders/twitter.py
--rw-r--r--   0        0        0      601 2023-12-18 12:05:47.259283 gigachain-0.1.7.1/langchain/document_loaders/unstructured.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.260397 gigachain-0.1.7.1/langchain/document_loaders/url.py
--rw-r--r--   0        0        0      236 2023-12-18 12:05:47.261334 gigachain-0.1.7.1/langchain/document_loaders/url_playwright.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.262991 gigachain-0.1.7.1/langchain/document_loaders/url_selenium.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.263820 gigachain-0.1.7.1/langchain/document_loaders/weather.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.408467 gigachain-0.1.7.1/langchain/document_loaders/web_base.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.265747 gigachain-0.1.7.1/langchain/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.266913 gigachain-0.1.7.1/langchain/document_loaders/wikipedia.py
--rw-r--r--   0        0        0      187 2023-12-18 12:05:47.268711 gigachain-0.1.7.1/langchain/document_loaders/word_document.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.269613 gigachain-0.1.7.1/langchain/document_loaders/xml.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.270340 gigachain-0.1.7.1/langchain/document_loaders/xorbits.py
--rw-r--r--   0        0        0      218 2024-01-10 09:04:40.409212 gigachain-0.1.7.1/langchain/document_loaders/youtube.py
--rw-r--r--   0        0        0     1616 2024-02-05 09:38:07.040859 gigachain-0.1.7.1/langchain/document_transformers/__init__.py
--rw-r--r--   0        0        0      155 2024-01-10 09:04:40.410215 gigachain-0.1.7.1/langchain/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.274031 gigachain-0.1.7.1/langchain/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.274901 gigachain-0.1.7.1/langchain/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0      145 2023-12-18 12:05:47.275765 gigachain-0.1.7.1/langchain/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0      487 2024-01-10 09:04:40.411019 gigachain-0.1.7.1/langchain/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.277716 gigachain-0.1.7.1/langchain/document_transformers/google_translate.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.278875 gigachain-0.1.7.1/langchain/document_transformers/html2text.py
--rw-r--r--   0        0        0     2042 2023-10-30 16:05:53.900619 gigachain-0.1.7.1/langchain/document_transformers/loading.py
--rw-r--r--   0        0        0      137 2024-01-10 09:04:40.411886 gigachain-0.1.7.1/langchain/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0      144 2023-12-18 12:05:47.280608 gigachain-0.1.7.1/langchain/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0      191 2023-12-18 12:05:47.281371 gigachain-0.1.7.1/langchain/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     2103 2023-10-30 16:05:53.902104 gigachain-0.1.7.1/langchain/document_transformers/serializers.py
--rw-r--r--   0        0        0     6033 2023-10-06 14:43:01.456268 gigachain-0.1.7.1/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     3598 2024-02-05 09:38:07.042664 gigachain-0.1.7.1/langchain/embeddings/__init__.py
--rw-r--r--   0        0        0      248 2023-12-18 12:05:47.283533 gigachain-0.1.7.1/langchain/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0       90 2023-12-18 12:05:47.284257 gigachain-0.1.7.1/langchain/embeddings/awa.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.285011 gigachain-0.1.7.1/langchain/embeddings/azure_openai.py
--rw-r--r--   0        0        0      142 2023-12-18 12:05:47.285672 gigachain-0.1.7.1/langchain/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.286522 gigachain-0.1.7.1/langchain/embeddings/base.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.287374 gigachain-0.1.7.1/langchain/embeddings/bedrock.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.412764 gigachain-0.1.7.1/langchain/embeddings/bookend.py
--rw-r--r--   0        0        0     8260 2024-02-19 11:59:44.100972 gigachain-0.1.7.1/langchain/embeddings/cache.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.292653 gigachain-0.1.7.1/langchain/embeddings/clarifai.py
--rw-r--r--   0        0        0      148 2024-01-10 09:04:40.413596 gigachain-0.1.7.1/langchain/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.293939 gigachain-0.1.7.1/langchain/embeddings/cohere.py
--rw-r--r--   0        0        0      117 2024-01-10 09:04:40.414696 gigachain-0.1.7.1/langchain/embeddings/dashscope.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.415721 gigachain-0.1.7.1/langchain/embeddings/databricks.py
--rw-r--r--   0        0        0      117 2024-01-10 09:04:40.416625 gigachain-0.1.7.1/langchain/embeddings/deepinfra.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.297444 gigachain-0.1.7.1/langchain/embeddings/edenai.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.298257 gigachain-0.1.7.1/langchain/embeddings/elasticsearch.py
--rw-r--r--   0        0        0      115 2024-01-10 09:04:40.417442 gigachain-0.1.7.1/langchain/embeddings/embaas.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:47.299986 gigachain-0.1.7.1/langchain/embeddings/ernie.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:47.300774 gigachain-0.1.7.1/langchain/embeddings/fake.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.301576 gigachain-0.1.7.1/langchain/embeddings/fastembed.py
--rw-r--r--   0        0        0      121 2024-01-10 09:04:40.418811 gigachain-0.1.7.1/langchain/embeddings/google_palm.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.303315 gigachain-0.1.7.1/langchain/embeddings/gpt4all.py
--rw-r--r--   0        0        0      108 2024-01-10 09:04:40.419865 gigachain-0.1.7.1/langchain/embeddings/gradient_ai.py
--rw-r--r--   0        0        0      344 2024-01-10 09:04:40.420673 gigachain-0.1.7.1/langchain/embeddings/huggingface.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.421652 gigachain-0.1.7.1/langchain/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0      200 2023-12-18 12:05:47.305872 gigachain-0.1.7.1/langchain/embeddings/infinity.py
--rw-r--r--   0        0        0      140 2024-01-10 09:04:40.422554 gigachain-0.1.7.1/langchain/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.307827 gigachain-0.1.7.1/langchain/embeddings/jina.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.308610 gigachain-0.1.7.1/langchain/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.309681 gigachain-0.1.7.1/langchain/embeddings/llamacpp.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.310693 gigachain-0.1.7.1/langchain/embeddings/llm_rails.py
--rw-r--r--   0        0        0      118 2024-01-10 09:04:40.423295 gigachain-0.1.7.1/langchain/embeddings/localai.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.424032 gigachain-0.1.7.1/langchain/embeddings/minimax.py
--rw-r--r--   0        0        0       99 2024-01-10 09:04:40.425886 gigachain-0.1.7.1/langchain/embeddings/mlflow.py
--rw-r--r--   0        0        0      134 2024-01-10 09:04:40.427005 gigachain-0.1.7.1/langchain/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.314820 gigachain-0.1.7.1/langchain/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.315663 gigachain-0.1.7.1/langchain/embeddings/mosaicml.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.316642 gigachain-0.1.7.1/langchain/embeddings/nlpcloud.py
--rw-r--r--   0        0        0      119 2024-01-10 09:04:40.427920 gigachain-0.1.7.1/langchain/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.318757 gigachain-0.1.7.1/langchain/embeddings/ollama.py
--rw-r--r--   0        0        0      115 2024-01-10 09:04:40.429049 gigachain-0.1.7.1/langchain/embeddings/openai.py
--rw-r--r--   0        0        0      200 2023-12-18 12:05:47.321173 gigachain-0.1.7.1/langchain/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0      121 2024-01-10 09:04:40.429895 gigachain-0.1.7.1/langchain/embeddings/self_hosted.py
--rw-r--r--   0        0        0      255 2024-01-10 09:04:40.430809 gigachain-0.1.7.1/langchain/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:47.324200 gigachain-0.1.7.1/langchain/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.325329 gigachain-0.1.7.1/langchain/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0      130 2024-01-10 09:04:40.432025 gigachain-0.1.7.1/langchain/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.327137 gigachain-0.1.7.1/langchain/embeddings/vertexai.py
--rw-r--r--   0        0        0      117 2024-01-10 09:04:40.433066 gigachain-0.1.7.1/langchain/embeddings/voyageai.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.328934 gigachain-0.1.7.1/langchain/embeddings/xinference.py
--rw-r--r--   0        0        0      476 2023-08-21 13:51:28.799282 gigachain-0.1.7.1/langchain/env.py
--rw-r--r--   0        0        0     5803 2023-10-30 16:05:53.905619 gigachain-0.1.7.1/langchain/evaluation/__init__.py
--rw-r--r--   0        0        0      165 2023-08-21 13:51:28.800913 gigachain-0.1.7.1/langchain/evaluation/agents/__init__.py
--rw-r--r--   0        0        0    13884 2024-02-19 11:59:44.102083 gigachain-0.1.7.1/langchain/evaluation/agents/trajectory_eval_chain.py
--rw-r--r--   0        0        0     9688 2023-12-18 12:05:47.331055 gigachain-0.1.7.1/langchain/evaluation/agents/trajectory_eval_prompt.py
--rw-r--r--   0        0        0     1400 2024-01-18 15:16:40.713791 gigachain-0.1.7.1/langchain/evaluation/comparison/__init__.py
--rw-r--r--   0        0        0    16056 2024-01-18 15:16:40.715217 gigachain-0.1.7.1/langchain/evaluation/comparison/eval_chain.py
--rw-r--r--   0        0        0     2358 2023-12-18 12:05:47.333888 gigachain-0.1.7.1/langchain/evaluation/comparison/prompt.py
--rw-r--r--   0        0        0     1647 2024-01-18 15:16:40.716003 gigachain-0.1.7.1/langchain/evaluation/criteria/__init__.py
--rw-r--r--   0        0        0    21358 2024-01-18 15:16:40.717295 gigachain-0.1.7.1/langchain/evaluation/criteria/eval_chain.py
--rw-r--r--   0        0        0     2723 2023-12-18 12:05:47.336070 gigachain-0.1.7.1/langchain/evaluation/criteria/prompt.py
--rw-r--r--   0        0        0      323 2023-08-21 13:51:28.806871 gigachain-0.1.7.1/langchain/evaluation/embedding_distance/__init__.py
--rw-r--r--   0        0        0    15503 2024-01-18 15:16:40.719400 gigachain-0.1.7.1/langchain/evaluation/embedding_distance/base.py
--rw-r--r--   0        0        0        0 2023-10-03 07:51:15.890624 gigachain-0.1.7.1/langchain/evaluation/exact_match/__init__.py
--rw-r--r--   0        0        0     2751 2023-10-03 07:51:15.891318 gigachain-0.1.7.1/langchain/evaluation/exact_match/base.py
--rw-r--r--   0        0        0     6693 2024-01-18 15:16:40.720469 gigachain-0.1.7.1/langchain/evaluation/loading.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.807950 gigachain-0.1.7.1/langchain/evaluation/parsing/__init__.py
--rw-r--r--   0        0        0     5246 2024-01-18 15:16:40.721461 gigachain-0.1.7.1/langchain/evaluation/parsing/base.py
--rw-r--r--   0        0        0     3679 2023-10-30 16:05:53.907474 gigachain-0.1.7.1/langchain/evaluation/parsing/json_distance.py
--rw-r--r--   0        0        0     3197 2023-10-30 16:05:53.907950 gigachain-0.1.7.1/langchain/evaluation/parsing/json_schema.py
--rw-r--r--   0        0        0      344 2023-08-21 13:51:28.808592 gigachain-0.1.7.1/langchain/evaluation/qa/__init__.py
--rw-r--r--   0        0        0    10886 2023-12-18 12:05:47.339833 gigachain-0.1.7.1/langchain/evaluation/qa/eval_chain.py
--rw-r--r--   0        0        0     6525 2023-12-18 12:05:47.340520 gigachain-0.1.7.1/langchain/evaluation/qa/eval_prompt.py
--rw-r--r--   0        0        0     1052 2023-12-18 12:05:47.341163 gigachain-0.1.7.1/langchain/evaluation/qa/generate_chain.py
--rw-r--r--   0        0        0      917 2023-12-18 12:05:47.341977 gigachain-0.1.7.1/langchain/evaluation/qa/generate_prompt.py
--rw-r--r--   0        0        0        0 2023-10-03 07:51:15.892405 gigachain-0.1.7.1/langchain/evaluation/regex_match/__init__.py
--rw-r--r--   0        0        0     2407 2023-10-03 07:51:15.893632 gigachain-0.1.7.1/langchain/evaluation/regex_match/base.py
--rw-r--r--   0        0        0    18197 2024-01-18 15:16:40.722881 gigachain-0.1.7.1/langchain/evaluation/schema.py
--rw-r--r--   0        0        0     1112 2024-01-18 15:16:40.723972 gigachain-0.1.7.1/langchain/evaluation/scoring/__init__.py
--rw-r--r--   0        0        0    15656 2024-01-18 15:16:40.725217 gigachain-0.1.7.1/langchain/evaluation/scoring/eval_chain.py
--rw-r--r--   0        0        0     2129 2023-12-18 12:05:47.344553 gigachain-0.1.7.1/langchain/evaluation/scoring/prompt.py
--rw-r--r--   0        0        0      285 2023-08-21 13:51:28.811472 gigachain-0.1.7.1/langchain/evaluation/string_distance/__init__.py
--rw-r--r--   0        0        0    14014 2023-12-18 12:05:47.346023 gigachain-0.1.7.1/langchain/evaluation/string_distance/base.py
--rw-r--r--   0        0        0      141 2023-08-21 13:51:28.812128 gigachain-0.1.7.1/langchain/example_generator.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.347238 gigachain-0.1.7.1/langchain/formatting.py
--rw-r--r--   0        0        0     7435 2023-12-18 12:05:47.348391 gigachain-0.1.7.1/langchain/globals/__init__.py
--rw-r--r--   0        0        0     1104 2024-02-05 09:38:07.044315 gigachain-0.1.7.1/langchain/graphs/__init__.py
--rw-r--r--   0        0        0      148 2024-01-10 09:04:40.437971 gigachain-0.1.7.1/langchain/graphs/arangodb_graph.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.438954 gigachain-0.1.7.1/langchain/graphs/falkordb_graph.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.350721 gigachain-0.1.7.1/langchain/graphs/graph_document.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.351490 gigachain-0.1.7.1/langchain/graphs/graph_store.py
--rw-r--r--   0        0        0       84 2023-12-18 12:05:47.352513 gigachain-0.1.7.1/langchain/graphs/hugegraph.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.353474 gigachain-0.1.7.1/langchain/graphs/kuzu_graph.py
--rw-r--r--   0        0        0      106 2024-01-10 09:04:40.439872 gigachain-0.1.7.1/langchain/graphs/memgraph_graph.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.440630 gigachain-0.1.7.1/langchain/graphs/nebula_graph.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.441708 gigachain-0.1.7.1/langchain/graphs/neo4j_graph.py
--rw-r--r--   0        0        0       94 2024-01-10 09:04:40.442566 gigachain-0.1.7.1/langchain/graphs/neptune_graph.py
--rw-r--r--   0        0        0      299 2023-12-18 12:05:47.358092 gigachain-0.1.7.1/langchain/graphs/networkx_graph.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.443339 gigachain-0.1.7.1/langchain/graphs/rdf_graph.py
--rw-r--r--   0        0        0     2874 2023-12-18 12:05:47.360240 gigachain-0.1.7.1/langchain/hub.py
--rw-r--r--   0        0        0      973 2023-10-19 12:57:52.913246 gigachain-0.1.7.1/langchain/indexes/__init__.py
--rw-r--r--   0        0        0    22479 2024-02-19 11:59:44.103064 gigachain-0.1.7.1/langchain/indexes/_api.py
--rw-r--r--   0        0        0    20556 2024-02-19 11:59:44.105332 gigachain-0.1.7.1/langchain/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0     5221 2023-10-19 12:57:52.916879 gigachain-0.1.7.1/langchain/indexes/base.py
--rw-r--r--   0        0        0     1752 2024-01-18 15:16:40.727874 gigachain-0.1.7.1/langchain/indexes/graph.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.816990 gigachain-0.1.7.1/langchain/indexes/prompts/__init__.py
--rw-r--r--   0        0        0     3241 2023-12-18 12:05:47.364265 gigachain-0.1.7.1/langchain/indexes/prompts/entity_extraction.py
--rw-r--r--   0        0        0     1797 2023-12-18 12:05:47.365149 gigachain-0.1.7.1/langchain/indexes/prompts/entity_summarization.py
--rw-r--r--   0        0        0     2276 2024-01-18 15:16:40.730868 gigachain-0.1.7.1/langchain/indexes/prompts/knowledge_triplet_extraction.py
--rw-r--r--   0        0        0     3423 2024-01-18 15:16:40.731835 gigachain-0.1.7.1/langchain/indexes/vectorstore.py
--rw-r--r--   0        0        0      282 2023-12-18 12:05:47.367912 gigachain-0.1.7.1/langchain/input.py
--rw-r--r--   0        0        0    17126 2024-02-05 09:38:07.045985 gigachain-0.1.7.1/langchain/llms/__init__.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.373059 gigachain-0.1.7.1/langchain/llms/ai21.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.375795 gigachain-0.1.7.1/langchain/llms/aleph_alpha.py
--rw-r--r--   0        0        0      114 2024-01-10 09:04:40.445264 gigachain-0.1.7.1/langchain/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0       82 2024-01-10 09:04:40.446089 gigachain-0.1.7.1/langchain/llms/anthropic.py
--rw-r--r--   0        0        0       88 2024-01-10 09:04:40.446963 gigachain-0.1.7.1/langchain/llms/anyscale.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:47.380664 gigachain-0.1.7.1/langchain/llms/arcee.py
--rw-r--r--   0        0        0       82 2024-01-10 09:04:40.448322 gigachain-0.1.7.1/langchain/llms/aviary.py
--rw-r--r--   0        0        0      507 2023-12-18 12:05:47.382858 gigachain-0.1.7.1/langchain/llms/azureml_endpoint.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.383805 gigachain-0.1.7.1/langchain/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.384682 gigachain-0.1.7.1/langchain/llms/bananadev.py
--rw-r--r--   0        0        0      228 2024-01-10 09:04:40.449816 gigachain-0.1.7.1/langchain/llms/base.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.386653 gigachain-0.1.7.1/langchain/llms/baseten.py
--rw-r--r--   0        0        0       67 2024-01-10 09:04:40.450756 gigachain-0.1.7.1/langchain/llms/beam.py
--rw-r--r--   0        0        0      128 2024-01-10 09:04:40.451692 gigachain-0.1.7.1/langchain/llms/bedrock.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.389069 gigachain-0.1.7.1/langchain/llms/bittensor.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.389772 gigachain-0.1.7.1/langchain/llms/cerebriumai.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.390471 gigachain-0.1.7.1/langchain/llms/chatglm.py
--rw-r--r--   0        0        0       79 2024-01-10 09:04:40.452477 gigachain-0.1.7.1/langchain/llms/clarifai.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.391687 gigachain-0.1.7.1/langchain/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0       89 2024-01-10 09:04:40.453363 gigachain-0.1.7.1/langchain/llms/cohere.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.393292 gigachain-0.1.7.1/langchain/llms/ctransformers.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.394040 gigachain-0.1.7.1/langchain/llms/ctranslate2.py
--rw-r--r--   0        0        0      101 2024-01-10 09:04:40.454645 gigachain-0.1.7.1/langchain/llms/databricks.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.455573 gigachain-0.1.7.1/langchain/llms/deepinfra.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.397072 gigachain-0.1.7.1/langchain/llms/deepsparse.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.397873 gigachain-0.1.7.1/langchain/llms/edenai.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.399013 gigachain-0.1.7.1/langchain/llms/fake.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.456495 gigachain-0.1.7.1/langchain/llms/fireworks.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.400669 gigachain-0.1.7.1/langchain/llms/forefrontai.py
--rw-r--r--   0        0        0       79 2024-01-10 09:04:40.457511 gigachain-0.1.7.1/langchain/llms/gigachat.py
--rw-r--r--   0        0        0       86 2024-01-10 09:04:40.459648 gigachain-0.1.7.1/langchain/llms/google_palm.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.403054 gigachain-0.1.7.1/langchain/llms/gooseai.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.403988 gigachain-0.1.7.1/langchain/llms/gpt4all.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.404853 gigachain-0.1.7.1/langchain/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2023-08-29 13:18:02.701979 gigachain-0.1.7.1/langchain/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2023-08-29 13:18:02.702167 gigachain-0.1.7.1/langchain/llms/grammars/list.gbnf
--rw-r--r--   0        0        0      122 2024-01-10 09:04:40.460567 gigachain-0.1.7.1/langchain/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0      107 2024-01-10 09:04:40.461738 gigachain-0.1.7.1/langchain/llms/huggingface_hub.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.462973 gigachain-0.1.7.1/langchain/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:47.408597 gigachain-0.1.7.1/langchain/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0       95 2024-01-10 09:04:40.464144 gigachain-0.1.7.1/langchain/llms/human.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.465399 gigachain-0.1.7.1/langchain/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.466206 gigachain-0.1.7.1/langchain/llms/koboldai.py
--rw-r--r--   0        0        0       79 2023-12-18 12:05:47.413304 gigachain-0.1.7.1/langchain/llms/llamacpp.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.414682 gigachain-0.1.7.1/langchain/llms/loading.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.415424 gigachain-0.1.7.1/langchain/llms/manifest.py
--rw-r--r--   0        0        0       85 2024-01-10 09:04:40.467239 gigachain-0.1.7.1/langchain/llms/minimax.py
--rw-r--r--   0        0        0       73 2024-01-10 09:04:40.468921 gigachain-0.1.7.1/langchain/llms/mlflow.py
--rw-r--r--   0        0        0      102 2024-01-10 09:04:40.469899 gigachain-0.1.7.1/langchain/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:47.418198 gigachain-0.1.7.1/langchain/llms/modal.py
--rw-r--r--   0        0        0       95 2024-01-10 09:04:40.470830 gigachain-0.1.7.1/langchain/llms/mosaicml.py
--rw-r--r--   0        0        0       79 2023-12-18 12:05:47.419808 gigachain-0.1.7.1/langchain/llms/nlpcloud.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.420848 gigachain-0.1.7.1/langchain/llms/octoai_endpoint.py
--rw-r--r--   0        0        0       82 2024-01-10 09:04:40.471699 gigachain-0.1.7.1/langchain/llms/ollama.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.422749 gigachain-0.1.7.1/langchain/llms/opaqueprompts.py
--rw-r--r--   0        0        0      193 2024-01-10 09:04:40.472465 gigachain-0.1.7.1/langchain/llms/openai.py
--rw-r--r--   0        0        0       76 2024-01-10 09:04:40.473297 gigachain-0.1.7.1/langchain/llms/openllm.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.425514 gigachain-0.1.7.1/langchain/llms/openlm.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.426494 gigachain-0.1.7.1/langchain/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.427233 gigachain-0.1.7.1/langchain/llms/petals.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.427965 gigachain-0.1.7.1/langchain/llms/pipelineai.py
--rw-r--r--   0        0        0       82 2023-12-18 12:05:47.428665 gigachain-0.1.7.1/langchain/llms/predibase.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.429339 gigachain-0.1.7.1/langchain/llms/predictionguard.py
--rw-r--r--   0        0        0      168 2023-12-18 12:05:47.430258 gigachain-0.1.7.1/langchain/llms/promptlayer_openai.py
--rw-r--r--   0        0        0       82 2023-12-18 12:05:47.431189 gigachain-0.1.7.1/langchain/llms/replicate.py
--rw-r--r--   0        0        0       67 2023-12-18 12:05:47.431973 gigachain-0.1.7.1/langchain/llms/rwkv.py
--rw-r--r--   0        0        0      160 2024-01-10 09:04:40.479050 gigachain-0.1.7.1/langchain/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.479967 gigachain-0.1.7.1/langchain/llms/self_hosted.py
--rw-r--r--   0        0        0      143 2024-01-10 09:04:40.480961 gigachain-0.1.7.1/langchain/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.435028 gigachain-0.1.7.1/langchain/llms/stochasticai.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.481881 gigachain-0.1.7.1/langchain/llms/symblai_nebula.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.436528 gigachain-0.1.7.1/langchain/llms/textgen.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.437384 gigachain-0.1.7.1/langchain/llms/titan_takeoff.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.438099 gigachain-0.1.7.1/langchain/llms/titan_takeoff_pro.py
--rw-r--r--   0        0        0       79 2023-12-18 12:05:47.438940 gigachain-0.1.7.1/langchain/llms/together.py
--rw-r--r--   0        0        0       89 2024-01-10 09:04:40.482832 gigachain-0.1.7.1/langchain/llms/tongyi.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.440079 gigachain-0.1.7.1/langchain/llms/utils.py
--rw-r--r--   0        0        0      147 2024-01-10 09:04:40.483851 gigachain-0.1.7.1/langchain/llms/vertexai.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.441569 gigachain-0.1.7.1/langchain/llms/vllm.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.441823 gigachain-0.1.7.1/langchain/llms/volcengine_maas.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.442050 gigachain-0.1.7.1/langchain/llms/watsonxllm.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.442855 gigachain-0.1.7.1/langchain/llms/writer.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.443467 gigachain-0.1.7.1/langchain/llms/xinference.py
--rw-r--r--   0        0        0       79 2024-01-10 09:04:40.484703 gigachain-0.1.7.1/langchain/llms/yandex.py
--rw-r--r--   0        0        0      206 2023-12-18 12:05:47.445806 gigachain-0.1.7.1/langchain/load/__init__.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.446683 gigachain-0.1.7.1/langchain/load/dump.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.447484 gigachain-0.1.7.1/langchain/load/load.py
--rw-r--r--   0        0        0      412 2023-12-18 12:05:47.448066 gigachain-0.1.7.1/langchain/load/serializable.py
--rw-r--r--   0        0        0     3256 2024-01-18 15:16:40.735874 gigachain-0.1.7.1/langchain/memory/__init__.py
--rw-r--r--   0        0        0     4861 2024-02-19 11:59:44.106523 gigachain-0.1.7.1/langchain/memory/buffer.py
--rw-r--r--   0        0        0     1616 2023-12-18 12:05:47.450214 gigachain-0.1.7.1/langchain/memory/buffer_window.py
--rw-r--r--   0        0        0     2245 2024-02-19 11:59:44.107383 gigachain-0.1.7.1/langchain/memory/chat_memory.py
--rw-r--r--   0        0        0     1560 2024-02-05 09:38:07.048026 gigachain-0.1.7.1/langchain/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.485550 gigachain-0.1.7.1/langchain/memory/chat_message_histories/astradb.py
--rw-r--r--   0        0        0      145 2024-01-10 09:04:40.486385 gigachain-0.1.7.1/langchain/memory/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0      143 2023-12-18 12:05:47.453355 gigachain-0.1.7.1/langchain/memory/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0      142 2023-12-18 12:05:47.454333 gigachain-0.1.7.1/langchain/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0      157 2023-12-18 12:05:47.455260 gigachain-0.1.7.1/langchain/memory/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.456262 gigachain-0.1.7.1/langchain/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0      145 2024-01-10 09:04:40.487202 gigachain-0.1.7.1/langchain/memory/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.458129 gigachain-0.1.7.1/langchain/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.488531 gigachain-0.1.7.1/langchain/memory/chat_message_histories/momento.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.489333 gigachain-0.1.7.1/langchain/memory/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.461292 gigachain-0.1.7.1/langchain/memory/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0      142 2024-01-10 09:04:40.490216 gigachain-0.1.7.1/langchain/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.469349 gigachain-0.1.7.1/langchain/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.470277 gigachain-0.1.7.1/langchain/memory/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0      157 2023-12-18 12:05:47.474949 gigachain-0.1.7.1/langchain/memory/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0      248 2024-01-10 09:04:40.492289 gigachain-0.1.7.1/langchain/memory/chat_message_histories/sql.py
--rw-r--r--   0        0        0      145 2023-12-18 12:05:47.476873 gigachain-0.1.7.1/langchain/memory/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0      155 2023-12-18 12:05:47.477734 gigachain-0.1.7.1/langchain/memory/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.478747 gigachain-0.1.7.1/langchain/memory/chat_message_histories/xata.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.479566 gigachain-0.1.7.1/langchain/memory/chat_message_histories/zep.py
--rw-r--r--   0        0        0     2912 2023-12-18 12:05:47.480430 gigachain-0.1.7.1/langchain/memory/combined.py
--rw-r--r--   0        0        0    15677 2024-02-05 09:38:07.049258 gigachain-0.1.7.1/langchain/memory/entity.py
--rw-r--r--   0        0        0     5075 2024-01-18 15:16:40.739203 gigachain-0.1.7.1/langchain/memory/kg.py
--rw-r--r--   0        0        0     3106 2023-12-18 12:05:47.483008 gigachain-0.1.7.1/langchain/memory/motorhead_memory.py
--rw-r--r--   0        0        0    13128 2023-12-18 12:05:47.483791 gigachain-0.1.7.1/langchain/memory/prompt.py
--rw-r--r--   0        0        0      794 2023-12-18 12:05:47.484537 gigachain-0.1.7.1/langchain/memory/readonly.py
--rw-r--r--   0        0        0      761 2023-12-18 12:05:47.485293 gigachain-0.1.7.1/langchain/memory/simple.py
--rw-r--r--   0        0        0     3389 2023-12-18 12:05:47.485998 gigachain-0.1.7.1/langchain/memory/summary.py
--rw-r--r--   0        0        0     2949 2023-12-18 12:05:47.486936 gigachain-0.1.7.1/langchain/memory/summary_buffer.py
--rw-r--r--   0        0        0     2144 2023-12-18 12:05:47.487927 gigachain-0.1.7.1/langchain/memory/token_buffer.py
--rw-r--r--   0        0        0      617 2023-08-29 13:18:02.706587 gigachain-0.1.7.1/langchain/memory/utils.py
--rw-r--r--   0        0        0     3002 2023-12-18 12:05:47.489028 gigachain-0.1.7.1/langchain/memory/vectorstore.py
--rw-r--r--   0        0        0     5090 2024-01-18 15:16:40.740045 gigachain-0.1.7.1/langchain/memory/zep_memory.py
--rw-r--r--   0        0        0     3278 2024-02-19 11:59:44.108300 gigachain-0.1.7.1/langchain/model_laboratory.py
--rw-r--r--   0        0        0     2216 2023-12-18 12:05:47.491014 gigachain-0.1.7.1/langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1084 2023-12-18 12:05:47.491916 gigachain-0.1.7.1/langchain/output_parsers/boolean.py
--rw-r--r--   0        0        0     1799 2023-12-18 12:05:47.492673 gigachain-0.1.7.1/langchain/output_parsers/combining.py
--rw-r--r--   0        0        0     1924 2024-01-30 14:52:09.530941 gigachain-0.1.7.1/langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1205 2023-12-18 12:05:47.494416 gigachain-0.1.7.1/langchain/output_parsers/enum.py
--rw-r--r--   0        0        0      424 2024-01-30 14:52:09.531645 gigachain-0.1.7.1/langchain/output_parsers/ernie_functions.py
--rw-r--r--   0        0        0     3153 2023-12-18 12:05:47.496827 gigachain-0.1.7.1/langchain/output_parsers/fix.py
--rw-r--r--   0        0        0     3958 2024-01-18 15:16:40.741558 gigachain-0.1.7.1/langchain/output_parsers/format_instructions.py
--rw-r--r--   0        0        0      298 2024-01-10 09:04:40.495028 gigachain-0.1.7.1/langchain/output_parsers/json.py
--rw-r--r--   0        0        0      310 2023-12-18 12:05:47.500021 gigachain-0.1.7.1/langchain/output_parsers/list.py
--rw-r--r--   0        0        0      702 2023-08-21 13:51:28.860635 gigachain-0.1.7.1/langchain/output_parsers/loading.py
--rw-r--r--   0        0        0     8214 2024-02-19 14:58:30.900628 gigachain-0.1.7.1/langchain/output_parsers/openai_functions.py
--rw-r--r--   0        0        0     3781 2024-02-19 11:59:44.109135 gigachain-0.1.7.1/langchain/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     6548 2024-01-30 14:52:09.533731 gigachain-0.1.7.1/langchain/output_parsers/pandas_dataframe.py
--rw-r--r--   0        0        0      699 2023-12-18 12:05:47.503286 gigachain-0.1.7.1/langchain/output_parsers/prompts.py
--rw-r--r--   0        0        0     1975 2024-02-19 11:59:44.112663 gigachain-0.1.7.1/langchain/output_parsers/pydantic.py
--rw-r--r--   0        0        0      129 2024-01-30 14:52:09.534282 gigachain-0.1.7.1/langchain/output_parsers/rail_parser.py
--rw-r--r--   0        0        0     1214 2023-12-18 12:05:47.506059 gigachain-0.1.7.1/langchain/output_parsers/regex.py
--rw-r--r--   0        0        0     1709 2023-12-18 12:05:47.506885 gigachain-0.1.7.1/langchain/output_parsers/regex_dict.py
--rw-r--r--   0        0        0     7792 2024-01-18 15:16:40.746608 gigachain-0.1.7.1/langchain/output_parsers/retry.py
--rw-r--r--   0        0        0     3134 2024-02-19 11:59:44.113701 gigachain-0.1.7.1/langchain/output_parsers/structured.py
--rw-r--r--   0        0        0       93 2024-01-10 09:04:40.496050 gigachain-0.1.7.1/langchain/output_parsers/xml.py
--rw-r--r--   0        0        0     2181 2024-02-19 11:59:44.114743 gigachain-0.1.7.1/langchain/output_parsers/yaml.py
--rw-r--r--   0        0        0     2560 2023-12-18 12:05:47.510676 gigachain-0.1.7.1/langchain/prompts/__init__.py
--rw-r--r--   0        0        0      565 2023-12-18 12:05:47.511466 gigachain-0.1.7.1/langchain/prompts/base.py
--rw-r--r--   0        0        0     1045 2023-12-18 12:05:47.512665 gigachain-0.1.7.1/langchain/prompts/chat.py
--rw-r--r--   0        0        0      568 2023-12-18 12:05:47.513679 gigachain-0.1.7.1/langchain/prompts/example_selector/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.514537 gigachain-0.1.7.1/langchain/prompts/example_selector/base.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.515578 gigachain-0.1.7.1/langchain/prompts/example_selector/length_based.py
--rw-r--r--   0        0        0      203 2024-02-19 11:59:44.116103 gigachain-0.1.7.1/langchain/prompts/example_selector/ngram_overlap.py
--rw-r--r--   0        0        0      288 2023-12-18 12:05:47.517451 gigachain-0.1.7.1/langchain/prompts/example_selector/semantic_similarity.py
--rw-r--r--   0        0        0      265 2023-12-18 12:05:47.518312 gigachain-0.1.7.1/langchain/prompts/few_shot.py
--rw-r--r--   0        0        0      128 2023-12-18 12:05:47.519153 gigachain-0.1.7.1/langchain/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0      530 2023-12-18 12:05:47.519896 gigachain-0.1.7.1/langchain/prompts/loading.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.520643 gigachain-0.1.7.1/langchain/prompts/pipeline.py
--rw-r--r--   0        0        0      153 2023-12-18 12:05:47.521708 gigachain-0.1.7.1/langchain/prompts/prompt.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.868214 gigachain-0.1.7.1/langchain/py.typed
--rw-r--r--   0        0        0      897 2023-08-21 13:51:28.868582 gigachain-0.1.7.1/langchain/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2023-08-21 13:51:28.868846 gigachain-0.1.7.1/langchain/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2023-08-21 13:51:28.869090 gigachain-0.1.7.1/langchain/pydantic_v1/main.py
--rw-r--r--   0        0        0      121 2024-01-18 15:16:40.748012 gigachain-0.1.7.1/langchain/python.py
--rw-r--r--   0        0        0      222 2024-01-18 15:16:40.748946 gigachain-0.1.7.1/langchain/requests.py
--rw-r--r--   0        0        0     3488 2024-02-05 09:38:07.052123 gigachain-0.1.7.1/langchain/retrievers/__init__.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.523253 gigachain-0.1.7.1/langchain/retrievers/arcee.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.524007 gigachain-0.1.7.1/langchain/retrievers/arxiv.py
--rw-r--r--   0        0        0      150 2024-01-10 09:04:40.496942 gigachain-0.1.7.1/langchain/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0      221 2023-12-18 12:05:47.525596 gigachain-0.1.7.1/langchain/retrievers/bedrock.py
--rw-r--r--   0        0        0      162 2023-12-18 12:05:47.526294 gigachain-0.1.7.1/langchain/retrievers/bm25.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.527002 gigachain-0.1.7.1/langchain/retrievers/chaindesk.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.527627 gigachain-0.1.7.1/langchain/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0      126 2024-01-10 09:04:40.497936 gigachain-0.1.7.1/langchain/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2298 2024-01-30 14:52:09.535664 gigachain-0.1.7.1/langchain/retrievers/contextual_compression.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.530630 gigachain-0.1.7.1/langchain/retrievers/databerry.py
--rw-r--r--   0        0        0      129 2023-12-18 12:05:47.531715 gigachain-0.1.7.1/langchain/retrievers/docarray.py
--rw-r--r--   0        0        0      701 2024-02-19 11:59:44.117225 gigachain-0.1.7.1/langchain/retrievers/document_compressors/__init__.py
--rw-r--r--   0        0        0     3775 2024-01-18 15:16:40.751239 gigachain-0.1.7.1/langchain/retrievers/document_compressors/base.py
--rw-r--r--   0        0        0     3955 2024-02-19 11:59:44.118211 gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_extract.py
--rw-r--r--   0        0        0      621 2023-08-21 13:51:28.874260 gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_extract_prompt.py
--rw-r--r--   0        0        0     2757 2023-12-18 12:05:47.535586 gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_filter.py
--rw-r--r--   0        0        0      336 2023-09-04 15:41:37.267607 gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_filter_prompt.py
--rw-r--r--   0        0        0     4213 2024-02-19 11:59:44.119219 gigachain-0.1.7.1/langchain/retrievers/document_compressors/cohere_rerank.py
--rw-r--r--   0        0        0     3031 2024-01-18 15:16:40.752303 gigachain-0.1.7.1/langchain/retrievers/document_compressors/embeddings_filter.py
--rw-r--r--   0        0        0     2415 2024-02-19 11:59:44.119578 gigachain-0.1.7.1/langchain/retrievers/document_compressors/flashrank_rerank.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.538561 gigachain-0.1.7.1/langchain/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.539048 gigachain-0.1.7.1/langchain/retrievers/embedchain.py
--rw-r--r--   0        0        0     9668 2024-02-19 11:59:44.121380 gigachain-0.1.7.1/langchain/retrievers/ensemble.py
--rw-r--r--   0        0        0      171 2023-12-18 12:05:47.540495 gigachain-0.1.7.1/langchain/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0      334 2024-01-10 09:04:40.499089 gigachain-0.1.7.1/langchain/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.542055 gigachain-0.1.7.1/langchain/retrievers/kay.py
--rw-r--r--   0        0        0      803 2023-12-18 12:05:47.542775 gigachain-0.1.7.1/langchain/retrievers/kendra.py
--rw-r--r--   0        0        0       88 2024-01-10 09:04:40.499990 gigachain-0.1.7.1/langchain/retrievers/knn.py
--rw-r--r--   0        0        0      177 2023-12-18 12:05:47.544144 gigachain-0.1.7.1/langchain/retrievers/llama_index.py
--rw-r--r--   0        0        0     3489 2024-01-30 14:52:09.537598 gigachain-0.1.7.1/langchain/retrievers/merger_retriever.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.546337 gigachain-0.1.7.1/langchain/retrievers/metal.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.547245 gigachain-0.1.7.1/langchain/retrievers/milvus.py
--rw-r--r--   0        0        0     7120 2024-02-19 11:59:44.124377 gigachain-0.1.7.1/langchain/retrievers/multi_query.py
--rw-r--r--   0        0        0     3920 2024-02-19 11:59:44.125450 gigachain-0.1.7.1/langchain/retrievers/multi_vector.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.549986 gigachain-0.1.7.1/langchain/retrievers/outline.py
--rw-r--r--   0        0        0     5196 2024-02-19 11:59:44.127086 gigachain-0.1.7.1/langchain/retrievers/parent_document_retriever.py
--rw-r--r--   0        0        0      150 2024-01-10 09:04:40.501259 gigachain-0.1.7.1/langchain/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.552477 gigachain-0.1.7.1/langchain/retrievers/pubmed.py
--rw-r--r--   0        0        0       94 2023-08-21 13:51:28.881470 gigachain-0.1.7.1/langchain/retrievers/pupmed.py
--rw-r--r--   0        0        0     2930 2024-01-30 14:52:09.541854 gigachain-0.1.7.1/langchain/retrievers/re_phraser.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.554463 gigachain-0.1.7.1/langchain/retrievers/remote_retriever.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.882217 gigachain-0.1.7.1/langchain/retrievers/self_query/__init__.py
--rw-r--r--   0        0        0     2194 2024-01-30 14:52:09.542270 gigachain-0.1.7.1/langchain/retrievers/self_query/astradb.py
--rw-r--r--   0        0        0     9664 2024-02-19 11:59:44.128307 gigachain-0.1.7.1/langchain/retrievers/self_query/base.py
--rw-r--r--   0        0        0     1474 2023-09-12 10:52:10.683073 gigachain-0.1.7.1/langchain/retrievers/self_query/chroma.py
--rw-r--r--   0        0        0     1918 2024-01-18 15:16:40.762739 gigachain-0.1.7.1/langchain/retrievers/self_query/dashvector.py
--rw-r--r--   0        0        0     2592 2023-09-04 05:57:22.522888 gigachain-0.1.7.1/langchain/retrievers/self_query/deeplake.py
--rw-r--r--   0        0        0     3273 2024-02-19 11:59:44.129505 gigachain-0.1.7.1/langchain/retrievers/self_query/elasticsearch.py
--rw-r--r--   0        0        0     3352 2024-01-30 14:52:09.544010 gigachain-0.1.7.1/langchain/retrievers/self_query/milvus.py
--rw-r--r--   0        0        0     2303 2023-12-18 12:05:47.558690 gigachain-0.1.7.1/langchain/retrievers/self_query/mongodb_atlas.py
--rw-r--r--   0        0        0     3636 2024-02-19 11:59:44.130638 gigachain-0.1.7.1/langchain/retrievers/self_query/myscale.py
--rw-r--r--   0        0        0     3271 2024-02-05 09:38:07.053042 gigachain-0.1.7.1/langchain/retrievers/self_query/opensearch.py
--rw-r--r--   0        0        0     1529 2024-02-19 11:59:44.131270 gigachain-0.1.7.1/langchain/retrievers/self_query/pgvector.py
--rw-r--r--   0        0        0     1687 2023-10-06 14:43:01.539605 gigachain-0.1.7.1/langchain/retrievers/self_query/pinecone.py
--rw-r--r--   0        0        0     3168 2024-02-19 11:59:44.132385 gigachain-0.1.7.1/langchain/retrievers/self_query/qdrant.py
--rw-r--r--   0        0        0     3376 2024-01-18 15:16:40.763805 gigachain-0.1.7.1/langchain/retrievers/self_query/redis.py
--rw-r--r--   0        0        0     2974 2023-09-12 10:52:10.683619 gigachain-0.1.7.1/langchain/retrievers/self_query/supabase.py
--rw-r--r--   0        0        0     2633 2023-09-25 07:40:35.527447 gigachain-0.1.7.1/langchain/retrievers/self_query/timescalevector.py
--rw-r--r--   0        0        0     2164 2023-10-19 12:57:53.001031 gigachain-0.1.7.1/langchain/retrievers/self_query/vectara.py
--rw-r--r--   0        0        0     2619 2023-11-15 10:30:09.358178 gigachain-0.1.7.1/langchain/retrievers/self_query/weaviate.py
--rw-r--r--   0        0        0       88 2024-01-10 09:04:40.503132 gigachain-0.1.7.1/langchain/retrievers/svm.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.560135 gigachain-0.1.7.1/langchain/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.560807 gigachain-0.1.7.1/langchain/retrievers/tfidf.py
--rw-r--r--   0        0        0     6279 2024-01-30 14:52:09.545577 gigachain-0.1.7.1/langchain/retrievers/time_weighted_retriever.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.564083 gigachain-0.1.7.1/langchain/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0      150 2023-12-18 12:05:47.566297 gigachain-0.1.7.1/langchain/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0     8702 2024-02-19 11:59:44.135613 gigachain-0.1.7.1/langchain/retrievers/web_research.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.567950 gigachain-0.1.7.1/langchain/retrievers/wikipedia.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.569099 gigachain-0.1.7.1/langchain/retrievers/you.py
--rw-r--r--   0        0        0      142 2023-12-18 12:05:47.569898 gigachain-0.1.7.1/langchain/retrievers/zep.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.570757 gigachain-0.1.7.1/langchain/retrievers/zilliz.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.887732 gigachain-0.1.7.1/langchain/runnables/__init__.py
--rw-r--r--   0        0        0      809 2023-12-18 12:05:47.571530 gigachain-0.1.7.1/langchain/runnables/hub.py
--rw-r--r--   0        0        0     1521 2023-12-18 12:05:47.572385 gigachain-0.1.7.1/langchain/runnables/openai_functions.py
--rw-r--r--   0        0        0     2065 2023-12-18 12:05:47.575459 gigachain-0.1.7.1/langchain/schema/__init__.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.576297 gigachain-0.1.7.1/langchain/schema/agent.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.576979 gigachain-0.1.7.1/langchain/schema/cache.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:47.577169 gigachain-0.1.7.1/langchain/schema/callbacks/__init__.py
--rw-r--r--   0        0        0      511 2023-12-18 12:05:47.577786 gigachain-0.1.7.1/langchain/schema/callbacks/base.py
--rw-r--r--   0        0        0     1511 2023-12-18 12:05:47.578611 gigachain-0.1.7.1/langchain/schema/callbacks/manager.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.579043 gigachain-0.1.7.1/langchain/schema/callbacks/stdout.py
--rw-r--r--   0        0        0      131 2023-12-18 12:05:47.579408 gigachain-0.1.7.1/langchain/schema/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:47.579637 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.580043 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/base.py
--rw-r--r--   0        0        0      176 2023-12-18 12:05:47.580505 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      219 2023-12-18 12:05:47.580868 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.581282 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2023-12-18 12:05:47.581685 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.582039 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.582518 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2023-12-18 12:05:47.582779 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      257 2023-12-18 12:05:47.583106 gigachain-0.1.7.1/langchain/schema/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0       80 2023-12-18 12:05:47.583799 gigachain-0.1.7.1/langchain/schema/chat.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.584843 gigachain-0.1.7.1/langchain/schema/chat_history.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.585605 gigachain-0.1.7.1/langchain/schema/document.py
--rw-r--r--   0        0        0       75 2023-12-18 12:05:47.586431 gigachain-0.1.7.1/langchain/schema/embeddings.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.587468 gigachain-0.1.7.1/langchain/schema/exceptions.py
--rw-r--r--   0        0        0      367 2023-12-18 12:05:47.588176 gigachain-0.1.7.1/langchain/schema/language_model.py
--rw-r--r--   0        0        0       71 2023-12-18 12:05:47.588957 gigachain-0.1.7.1/langchain/schema/memory.py
--rw-r--r--   0        0        0     1048 2023-12-18 12:05:47.589743 gigachain-0.1.7.1/langchain/schema/messages.py
--rw-r--r--   0        0        0      320 2023-12-18 12:05:47.590462 gigachain-0.1.7.1/langchain/schema/output.py
--rw-r--r--   0        0        0      651 2023-12-18 12:05:47.591291 gigachain-0.1.7.1/langchain/schema/output_parser.py
--rw-r--r--   0        0        0       80 2023-12-18 12:05:47.592095 gigachain-0.1.7.1/langchain/schema/prompt.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.592918 gigachain-0.1.7.1/langchain/schema/prompt_template.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.593622 gigachain-0.1.7.1/langchain/schema/retriever.py
--rw-r--r--   0        0        0     1796 2023-12-18 12:05:47.594714 gigachain-0.1.7.1/langchain/schema/runnable/__init__.py
--rw-r--r--   0        0        0      781 2023-12-18 12:05:47.595763 gigachain-0.1.7.1/langchain/schema/runnable/base.py
--rw-r--r--   0        0        0       89 2023-12-18 12:05:47.596655 gigachain-0.1.7.1/langchain/schema/runnable/branch.py
--rw-r--r--   0        0        0      665 2023-12-18 12:05:47.597563 gigachain-0.1.7.1/langchain/schema/runnable/config.py
--rw-r--r--   0        0        0      333 2023-12-18 12:05:47.598462 gigachain-0.1.7.1/langchain/schema/runnable/configurable.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.599358 gigachain-0.1.7.1/langchain/schema/runnable/fallbacks.py
--rw-r--r--   0        0        0      260 2023-12-18 12:05:47.600021 gigachain-0.1.7.1/langchain/schema/runnable/history.py
--rw-r--r--   0        0        0      205 2023-12-18 12:05:47.600672 gigachain-0.1.7.1/langchain/schema/runnable/passthrough.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.601412 gigachain-0.1.7.1/langchain/schema/runnable/retry.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.602442 gigachain-0.1.7.1/langchain/schema/runnable/router.py
--rw-r--r--   0        0        0     1118 2023-12-18 12:05:47.603240 gigachain-0.1.7.1/langchain/schema/runnable/utils.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.604392 gigachain-0.1.7.1/langchain/schema/storage.py
--rw-r--r--   0        0        0      137 2023-12-18 12:05:47.605680 gigachain-0.1.7.1/langchain/schema/vectorstore.py
--rw-r--r--   0        0        0      130 2024-01-18 15:16:40.768493 gigachain-0.1.7.1/langchain/serpapi.py
--rw-r--r--   0        0        0     3544 2024-01-18 15:16:40.769415 gigachain-0.1.7.1/langchain/smith/__init__.py
--rw-r--r--   0        0        0     2199 2024-01-18 15:16:40.770441 gigachain-0.1.7.1/langchain/smith/evaluation/__init__.py
--rw-r--r--   0        0        0    12480 2024-01-10 09:04:40.504756 gigachain-0.1.7.1/langchain/smith/evaluation/config.py
--rw-r--r--   0        0        0     9936 2023-12-18 12:05:47.609341 gigachain-0.1.7.1/langchain/smith/evaluation/name_generation.py
--rw-r--r--   0        0        0     3306 2024-02-19 11:59:44.136955 gigachain-0.1.7.1/langchain/smith/evaluation/progress.py
--rw-r--r--   0        0        0    50978 2024-02-19 11:59:44.138253 gigachain-0.1.7.1/langchain/smith/evaluation/runner_utils.py
--rw-r--r--   0        0        0    17107 2023-12-18 12:05:47.613221 gigachain-0.1.7.1/langchain/smith/evaluation/string_run_evaluator.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.895985 gigachain-0.1.7.1/langchain/smith/evaluation/utils.py
--rw-r--r--   0        0        0      139 2024-01-18 15:16:40.773265 gigachain-0.1.7.1/langchain/sql_database.py
--rw-r--r--   0        0        0     1571 2024-02-05 09:38:07.054993 gigachain-0.1.7.1/langchain/storage/__init__.py
--rw-r--r--   0        0        0     2517 2023-12-18 12:05:47.615861 gigachain-0.1.7.1/langchain/storage/_lc_store.py
--rw-r--r--   0        0        0     2970 2023-12-18 12:05:47.616837 gigachain-0.1.7.1/langchain/storage/encoder_backed.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.617809 gigachain-0.1.7.1/langchain/storage/exceptions.py
--rw-r--r--   0        0        0     4307 2024-02-19 11:59:44.139633 gigachain-0.1.7.1/langchain/storage/file_system.py
--rw-r--r--   0        0        0     4448 2024-02-19 11:59:44.141288 gigachain-0.1.7.1/langchain/storage/in_memory.py
--rw-r--r--   0        0        0       83 2023-12-18 12:05:47.621280 gigachain-0.1.7.1/langchain/storage/redis.py
--rw-r--r--   0        0        0      166 2024-01-10 09:04:40.510757 gigachain-0.1.7.1/langchain/storage/upstash_redis.py
--rw-r--r--   0        0        0    55865 2024-02-19 11:59:44.142960 gigachain-0.1.7.1/langchain/text_splitter.py
--rw-r--r--   0        0        0     5663 2024-01-18 15:16:40.776804 gigachain-0.1.7.1/langchain/tools/__init__.py
--rw-r--r--   0        0        0      166 2023-12-18 12:05:47.625523 gigachain-0.1.7.1/langchain/tools/ainetwork/app.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.626232 gigachain-0.1.7.1/langchain/tools/ainetwork/base.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.626998 gigachain-0.1.7.1/langchain/tools/ainetwork/owner.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.627720 gigachain-0.1.7.1/langchain/tools/ainetwork/rule.py
--rw-r--r--   0        0        0      130 2023-12-18 12:05:47.628416 gigachain-0.1.7.1/langchain/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.630133 gigachain-0.1.7.1/langchain/tools/ainetwork/value.py
--rw-r--r--   0        0        0      257 2024-01-18 15:16:40.778408 gigachain-0.1.7.1/langchain/tools/amadeus/__init__.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.630970 gigachain-0.1.7.1/langchain/tools/amadeus/base.py
--rw-r--r--   0        0        0      180 2023-12-18 12:05:47.632104 gigachain-0.1.7.1/langchain/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:47.632931 gigachain-0.1.7.1/langchain/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0       25 2023-08-21 13:51:28.901095 gigachain-0.1.7.1/langchain/tools/arxiv/__init__.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.634560 gigachain-0.1.7.1/langchain/tools/arxiv/tool.py
--rw-r--r--   0        0        0      802 2024-01-18 15:16:40.780425 gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.636784 gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:47.638067 gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.638948 gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.639702 gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.640091 gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      332 2024-01-10 09:04:40.515503 gigachain-0.1.7.1/langchain/tools/base.py
--rw-r--r--   0        0        0        0 2023-10-19 12:57:53.049903 gigachain-0.1.7.1/langchain/tools/bearly/__init__.py
--rw-r--r--   0        0        0      229 2024-01-10 09:04:40.518070 gigachain-0.1.7.1/langchain/tools/bearly/tool.py
--rw-r--r--   0        0        0      170 2024-01-18 15:16:40.781740 gigachain-0.1.7.1/langchain/tools/bing_search/__init__.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.643848 gigachain-0.1.7.1/langchain/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.906784 gigachain-0.1.7.1/langchain/tools/brave_search/__init__.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.644621 gigachain-0.1.7.1/langchain/tools/brave_search/tool.py
--rw-r--r--   0        0        0        0 2023-10-06 14:43:01.562867 gigachain-0.1.7.1/langchain/tools/clickup/__init__.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.646160 gigachain-0.1.7.1/langchain/tools/clickup/tool.py
--rw-r--r--   0        0        0      157 2024-02-05 09:38:07.057285 gigachain-0.1.7.1/langchain/tools/convert_to_openai.py
--rw-r--r--   0        0        0      268 2024-01-18 15:16:40.785078 gigachain-0.1.7.1/langchain/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0      197 2023-12-18 12:05:47.647471 gigachain-0.1.7.1/langchain/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      147 2024-01-18 15:16:40.786394 gigachain-0.1.7.1/langchain/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0      269 2023-12-18 12:05:47.648366 gigachain-0.1.7.1/langchain/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2023-10-30 16:05:53.968119 gigachain-0.1.7.1/langchain/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0      240 2024-01-10 09:04:40.519149 gigachain-0.1.7.1/langchain/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0     1024 2024-01-18 15:16:40.788076 gigachain-0.1.7.1/langchain/tools/edenai/__init__.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.651357 gigachain-0.1.7.1/langchain/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.652284 gigachain-0.1.7.1/langchain/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.653108 gigachain-0.1.7.1/langchain/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0      139 2023-12-18 12:05:47.654289 gigachain-0.1.7.1/langchain/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0      143 2023-12-18 12:05:47.667832 gigachain-0.1.7.1/langchain/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.673367 gigachain-0.1.7.1/langchain/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0      128 2023-12-18 12:05:47.678230 gigachain-0.1.7.1/langchain/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0      126 2023-12-18 12:05:47.680238 gigachain-0.1.7.1/langchain/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      164 2024-01-18 15:16:40.789002 gigachain-0.1.7.1/langchain/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.681114 gigachain-0.1.7.1/langchain/tools/eleven_labs/models.py
--rw-r--r--   0        0        0      138 2024-01-10 09:04:40.520141 gigachain-0.1.7.1/langchain/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0      723 2024-01-18 15:16:40.790286 gigachain-0.1.7.1/langchain/tools/file_management/__init__.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.683048 gigachain-0.1.7.1/langchain/tools/file_management/copy.py
--rw-r--r--   0        0        0      155 2023-12-18 12:05:47.684055 gigachain-0.1.7.1/langchain/tools/file_management/delete.py
--rw-r--r--   0        0        0      160 2023-12-18 12:05:47.684795 gigachain-0.1.7.1/langchain/tools/file_management/file_search.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.685876 gigachain-0.1.7.1/langchain/tools/file_management/list_dir.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.687226 gigachain-0.1.7.1/langchain/tools/file_management/move.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.688294 gigachain-0.1.7.1/langchain/tools/file_management/read.py
--rw-r--r--   0        0        0      150 2023-12-18 12:05:47.690230 gigachain-0.1.7.1/langchain/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2023-08-21 13:51:28.913036 gigachain-0.1.7.1/langchain/tools/github/__init__.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.692510 gigachain-0.1.7.1/langchain/tools/github/tool.py
--rw-r--r--   0        0        0       20 2023-09-19 14:33:02.316769 gigachain-0.1.7.1/langchain/tools/gitlab/__init__.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.694012 gigachain-0.1.7.1/langchain/tools/gitlab/tool.py
--rw-r--r--   0        0        0      500 2024-01-18 15:16:40.791834 gigachain-0.1.7.1/langchain/tools/gmail/__init__.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.695102 gigachain-0.1.7.1/langchain/tools/gmail/base.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.696034 gigachain-0.1.7.1/langchain/tools/gmail/create_draft.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:47.696879 gigachain-0.1.7.1/langchain/tools/gmail/get_message.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.697691 gigachain-0.1.7.1/langchain/tools/gmail/get_thread.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.698533 gigachain-0.1.7.1/langchain/tools/gmail/search.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.699261 gigachain-0.1.7.1/langchain/tools/gmail/send_message.py
--rw-r--r--   0        0        0      136 2024-01-18 15:16:40.794195 gigachain-0.1.7.1/langchain/tools/golden_query/__init__.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.701139 gigachain-0.1.7.1/langchain/tools/golden_query/tool.py
--rw-r--r--   0        0        0      171 2024-01-18 15:16:40.795771 gigachain-0.1.7.1/langchain/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0      151 2024-01-10 09:04:40.524958 gigachain-0.1.7.1/langchain/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      152 2024-01-18 15:16:40.798988 gigachain-0.1.7.1/langchain/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.703299 gigachain-0.1.7.1/langchain/tools/google_finance/tool.py
--rw-r--r--   0        0        0      140 2024-01-18 15:16:40.802247 gigachain-0.1.7.1/langchain/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.703936 gigachain-0.1.7.1/langchain/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      140 2024-01-18 15:16:40.804061 gigachain-0.1.7.1/langchain/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.704750 gigachain-0.1.7.1/langchain/tools/google_lens/tool.py
--rw-r--r--   0        0        0      140 2024-01-18 15:16:40.808715 gigachain-0.1.7.1/langchain/tools/google_places/__init__.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.706017 gigachain-0.1.7.1/langchain/tools/google_places/tool.py
--rw-r--r--   0        0        0      152 2024-01-18 15:16:40.810765 gigachain-0.1.7.1/langchain/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.707012 gigachain-0.1.7.1/langchain/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      195 2024-01-18 15:16:40.814439 gigachain-0.1.7.1/langchain/tools/google_search/__init__.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.708241 gigachain-0.1.7.1/langchain/tools/google_search/tool.py
--rw-r--r--   0        0        0      243 2024-01-18 15:16:40.816966 gigachain-0.1.7.1/langchain/tools/google_serper/__init__.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.709262 gigachain-0.1.7.1/langchain/tools/google_serper/tool.py
--rw-r--r--   0        0        0      148 2024-01-18 15:16:40.824180 gigachain-0.1.7.1/langchain/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.709982 gigachain-0.1.7.1/langchain/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2023-08-21 13:51:28.921484 gigachain-0.1.7.1/langchain/tools/graphql/__init__.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.710894 gigachain-0.1.7.1/langchain/tools/graphql/tool.py
--rw-r--r--   0        0        0      132 2024-01-18 15:16:40.829390 gigachain-0.1.7.1/langchain/tools/human/__init__.py
--rw-r--r--   0        0        0       92 2024-01-10 09:04:40.530860 gigachain-0.1.7.1/langchain/tools/human/tool.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.713440 gigachain-0.1.7.1/langchain/tools/ifttt.py
--rw-r--r--   0        0        0       43 2023-08-21 13:51:28.923495 gigachain-0.1.7.1/langchain/tools/interaction/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.714893 gigachain-0.1.7.1/langchain/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2023-08-21 13:51:28.924161 gigachain-0.1.7.1/langchain/tools/jira/__init__.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.717607 gigachain-0.1.7.1/langchain/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2023-08-21 13:51:28.925352 gigachain-0.1.7.1/langchain/tools/json/__init__.py
--rw-r--r--   0        0        0      174 2024-01-10 09:04:40.535392 gigachain-0.1.7.1/langchain/tools/json/tool.py
--rw-r--r--   0        0        0      134 2024-01-18 15:16:40.836631 gigachain-0.1.7.1/langchain/tools/memorize/__init__.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.719498 gigachain-0.1.7.1/langchain/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2023-12-18 12:05:47.720059 gigachain-0.1.7.1/langchain/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.720682 gigachain-0.1.7.1/langchain/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      154 2024-01-18 15:16:40.840932 gigachain-0.1.7.1/langchain/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.721767 gigachain-0.1.7.1/langchain/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      359 2024-01-18 15:16:40.842423 gigachain-0.1.7.1/langchain/tools/multion/__init__.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:47.722885 gigachain-0.1.7.1/langchain/tools/multion/close_session.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.723750 gigachain-0.1.7.1/langchain/tools/multion/create_session.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.724545 gigachain-0.1.7.1/langchain/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:47.724833 gigachain-0.1.7.1/langchain/tools/nasa/__init__.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.725566 gigachain-0.1.7.1/langchain/tools/nasa/tool.py
--rw-r--r--   0        0        0      111 2024-01-18 15:16:40.844691 gigachain-0.1.7.1/langchain/tools/nuclia/__init__.py
--rw-r--r--   0        0        0      135 2023-12-18 12:05:47.726427 gigachain-0.1.7.1/langchain/tools/nuclia/tool.py
--rw-r--r--   0        0        0      567 2024-01-18 15:16:40.847490 gigachain-0.1.7.1/langchain/tools/office365/__init__.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.727311 gigachain-0.1.7.1/langchain/tools/office365/base.py
--rw-r--r--   0        0        0      197 2023-12-18 12:05:47.728682 gigachain-0.1.7.1/langchain/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:47.730216 gigachain-0.1.7.1/langchain/tools/office365/events_search.py
--rw-r--r--   0        0        0      166 2023-12-18 12:05:47.731158 gigachain-0.1.7.1/langchain/tools/office365/messages_search.py
--rw-r--r--   0        0        0      151 2023-12-18 12:05:47.732031 gigachain-0.1.7.1/langchain/tools/office365/send_event.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.732938 gigachain-0.1.7.1/langchain/tools/office365/send_message.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933159 gigachain-0.1.7.1/langchain/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933535 gigachain-0.1.7.1/langchain/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0      542 2024-01-10 09:04:40.537910 gigachain-0.1.7.1/langchain/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      191 2024-01-18 15:16:40.849295 gigachain-0.1.7.1/langchain/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      162 2024-01-18 15:16:40.852577 gigachain-0.1.7.1/langchain/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.735667 gigachain-0.1.7.1/langchain/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      763 2024-01-18 15:16:40.855894 gigachain-0.1.7.1/langchain/tools/playwright/__init__.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.538998 gigachain-0.1.7.1/langchain/tools/playwright/base.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.737713 gigachain-0.1.7.1/langchain/tools/playwright/click.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.738636 gigachain-0.1.7.1/langchain/tools/playwright/current_page.py
--rw-r--r--   0        0        0      198 2023-12-18 12:05:47.739546 gigachain-0.1.7.1/langchain/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.740370 gigachain-0.1.7.1/langchain/tools/playwright/extract_text.py
--rw-r--r--   0        0        0      168 2024-01-10 09:04:40.540758 gigachain-0.1.7.1/langchain/tools/playwright/get_elements.py
--rw-r--r--   0        0        0      152 2023-12-18 12:05:47.741776 gigachain-0.1.7.1/langchain/tools/playwright/navigate.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.742595 gigachain-0.1.7.1/langchain/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0      214 2024-01-10 09:04:40.541624 gigachain-0.1.7.1/langchain/tools/plugin.py
--rw-r--r--   0        0        0       52 2023-08-21 13:51:28.940033 gigachain-0.1.7.1/langchain/tools/powerbi/__init__.py
--rw-r--r--   0        0        0      189 2023-12-18 12:05:47.747546 gigachain-0.1.7.1/langchain/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2023-08-21 13:51:28.941121 gigachain-0.1.7.1/langchain/tools/pubmed/__init__.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.748986 gigachain-0.1.7.1/langchain/tools/pubmed/tool.py
--rw-r--r--   0        0        0      512 2023-12-18 12:05:47.750576 gigachain-0.1.7.1/langchain/tools/python/__init__.py
--rw-r--r--   0        0        0        0 2024-01-10 09:04:40.541802 gigachain-0.1.7.1/langchain/tools/reddit_search/__init__.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.750982 gigachain-0.1.7.1/langchain/tools/reddit_search/tool.py
--rw-r--r--   0        0        0     1581 2024-02-05 09:38:07.058119 gigachain-0.1.7.1/langchain/tools/render.py
--rw-r--r--   0        0        0       52 2023-08-21 13:51:28.942395 gigachain-0.1.7.1/langchain/tools/requests/__init__.py
--rw-r--r--   0        0        0      349 2024-01-10 09:04:40.543130 gigachain-0.1.7.1/langchain/tools/requests/tool.py
--rw-r--r--   0        0        0     2494 2024-02-19 11:59:44.144021 gigachain-0.1.7.1/langchain/tools/retriever.py
--rw-r--r--   0        0        0       31 2023-08-21 13:51:28.943010 gigachain-0.1.7.1/langchain/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:47.754166 gigachain-0.1.7.1/langchain/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      214 2024-01-18 15:16:40.857082 gigachain-0.1.7.1/langchain/tools/searchapi/__init__.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.754976 gigachain-0.1.7.1/langchain/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.943553 gigachain-0.1.7.1/langchain/tools/searx_search/__init__.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:47.756022 gigachain-0.1.7.1/langchain/tools/searx_search/tool.py
--rw-r--r--   0        0        0      103 2024-01-18 15:16:40.858323 gigachain-0.1.7.1/langchain/tools/shell/__init__.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.545873 gigachain-0.1.7.1/langchain/tools/shell/tool.py
--rw-r--r--   0        0        0      433 2024-01-18 15:16:40.859291 gigachain-0.1.7.1/langchain/tools/slack/__init__.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.757949 gigachain-0.1.7.1/langchain/tools/slack/base.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.758288 gigachain-0.1.7.1/langchain/tools/slack/get_channel.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:47.758614 gigachain-0.1.7.1/langchain/tools/slack/get_message.py
--rw-r--r--   0        0        0      179 2023-12-18 12:05:47.758964 gigachain-0.1.7.1/langchain/tools/slack/schedule_message.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.759577 gigachain-0.1.7.1/langchain/tools/slack/send_message.py
--rw-r--r--   0        0        0       18 2023-08-21 13:51:28.944873 gigachain-0.1.7.1/langchain/tools/sleep/__init__.py
--rw-r--r--   0        0        0      110 2023-12-18 12:05:47.760887 gigachain-0.1.7.1/langchain/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2023-08-21 13:51:28.945531 gigachain-0.1.7.1/langchain/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      304 2023-12-18 12:05:47.762602 gigachain-0.1.7.1/langchain/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.946602 gigachain-0.1.7.1/langchain/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.763764 gigachain-0.1.7.1/langchain/tools/sql_database/prompt.py
--rw-r--r--   0        0        0      337 2023-12-18 12:05:47.764601 gigachain-0.1.7.1/langchain/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2023-12-18 12:05:47.764989 gigachain-0.1.7.1/langchain/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.765358 gigachain-0.1.7.1/langchain/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2023-12-18 12:05:47.765850 gigachain-0.1.7.1/langchain/tools/steam/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.766652 gigachain-0.1.7.1/langchain/tools/steam/tool.py
--rw-r--r--   0        0        0      186 2024-01-18 15:16:40.861528 gigachain-0.1.7.1/langchain/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0      180 2024-01-10 09:04:40.549946 gigachain-0.1.7.1/langchain/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0      189 2024-01-18 15:16:40.863373 gigachain-0.1.7.1/langchain/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0      187 2023-12-18 12:05:47.769298 gigachain-0.1.7.1/langchain/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2023-08-21 13:51:28.948611 gigachain-0.1.7.1/langchain/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0      192 2024-01-10 09:04:40.550932 gigachain-0.1.7.1/langchain/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2023-08-21 13:51:28.949334 gigachain-0.1.7.1/langchain/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.770933 gigachain-0.1.7.1/langchain/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      156 2024-01-18 15:16:40.865406 gigachain-0.1.7.1/langchain/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.772046 gigachain-0.1.7.1/langchain/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.772808 gigachain-0.1.7.1/langchain/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.950523 gigachain-0.1.7.1/langchain/tools/youtube/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.773642 gigachain-0.1.7.1/langchain/tools/youtube/search.py
--rw-r--r--   0        0        0      193 2024-01-18 15:16:40.866803 gigachain-0.1.7.1/langchain/tools/zapier/__init__.py
--rw-r--r--   0        0        0      162 2023-12-18 12:05:47.775875 gigachain-0.1.7.1/langchain/tools/zapier/tool.py
--rw-r--r--   0        0        0     2327 2024-02-05 09:38:07.060904 gigachain-0.1.7.1/langchain/utilities/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.777546 gigachain-0.1.7.1/langchain/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      193 2024-01-10 09:04:40.553326 gigachain-0.1.7.1/langchain/utilities/anthropic.py
--rw-r--r--   0        0        0       89 2023-12-18 12:05:47.779550 gigachain-0.1.7.1/langchain/utilities/apify.py
--rw-r--r--   0        0        0      361 2023-12-18 12:05:47.780643 gigachain-0.1.7.1/langchain/utilities/arcee.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.781484 gigachain-0.1.7.1/langchain/utilities/arxiv.py
--rw-r--r--   0        0        0      274 2023-08-21 13:51:28.954857 gigachain-0.1.7.1/langchain/utilities/asyncio.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.782588 gigachain-0.1.7.1/langchain/utilities/awslambda.py
--rw-r--r--   0        0        0      104 2024-01-10 09:04:40.554292 gigachain-0.1.7.1/langchain/utilities/bibtex.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.784354 gigachain-0.1.7.1/langchain/utilities/bing_search.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.785090 gigachain-0.1.7.1/langchain/utilities/brave_search.py
--rw-r--r--   0        0        0      269 2024-01-10 09:04:40.555397 gigachain-0.1.7.1/langchain/utilities/clickup.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.786400 gigachain-0.1.7.1/langchain/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.787554 gigachain-0.1.7.1/langchain/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0      129 2023-12-18 12:05:47.788355 gigachain-0.1.7.1/langchain/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.556303 gigachain-0.1.7.1/langchain/utilities/github.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.789907 gigachain-0.1.7.1/langchain/utilities/gitlab.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.557288 gigachain-0.1.7.1/langchain/utilities/golden_query.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.790928 gigachain-0.1.7.1/langchain/utilities/google_finance.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.791487 gigachain-0.1.7.1/langchain/utilities/google_jobs.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.791854 gigachain-0.1.7.1/langchain/utilities/google_lens.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.792836 gigachain-0.1.7.1/langchain/utilities/google_places_api.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.793660 gigachain-0.1.7.1/langchain/utilities/google_scholar.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.794263 gigachain-0.1.7.1/langchain/utilities/google_search.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.794850 gigachain-0.1.7.1/langchain/utilities/google_serper.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.795198 gigachain-0.1.7.1/langchain/utilities/google_trends.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.796297 gigachain-0.1.7.1/langchain/utilities/graphql.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.797166 gigachain-0.1.7.1/langchain/utilities/jira.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.798009 gigachain-0.1.7.1/langchain/utilities/loading.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.798917 gigachain-0.1.7.1/langchain/utilities/max_compute.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.558668 gigachain-0.1.7.1/langchain/utilities/merriam_webster.py
--rw-r--r--   0        0        0      132 2024-01-10 09:04:40.559696 gigachain-0.1.7.1/langchain/utilities/metaphor_search.py
--rw-r--r--   0        0        0      101 2024-01-10 09:04:40.560501 gigachain-0.1.7.1/langchain/utilities/nasa.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.801862 gigachain-0.1.7.1/langchain/utilities/opaqueprompts.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.803267 gigachain-0.1.7.1/langchain/utilities/openapi.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.804229 gigachain-0.1.7.1/langchain/utilities/openweathermap.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.562773 gigachain-0.1.7.1/langchain/utilities/outline.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.805758 gigachain-0.1.7.1/langchain/utilities/portkey.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.563881 gigachain-0.1.7.1/langchain/utilities/powerbi.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.807428 gigachain-0.1.7.1/langchain/utilities/pubmed.py
--rw-r--r--   0        0        0       86 2024-01-10 09:04:40.566650 gigachain-0.1.7.1/langchain/utilities/python.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.808570 gigachain-0.1.7.1/langchain/utilities/reddit_search.py
--rw-r--r--   0        0        0      201 2024-01-10 09:04:40.567678 gigachain-0.1.7.1/langchain/utilities/redis.py
--rw-r--r--   0        0        0      181 2023-12-18 12:05:47.810729 gigachain-0.1.7.1/langchain/utilities/requests.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.811895 gigachain-0.1.7.1/langchain/utilities/scenexplain.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.812573 gigachain-0.1.7.1/langchain/utilities/searchapi.py
--rw-r--r--   0        0        0      151 2024-01-10 09:04:40.568799 gigachain-0.1.7.1/langchain/utilities/searx_search.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.814336 gigachain-0.1.7.1/langchain/utilities/serpapi.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.815076 gigachain-0.1.7.1/langchain/utilities/spark_sql.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.570370 gigachain-0.1.7.1/langchain/utilities/sql_database.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.816263 gigachain-0.1.7.1/langchain/utilities/stackexchange.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.816643 gigachain-0.1.7.1/langchain/utilities/steam.py
--rw-r--r--   0        0        0      126 2024-01-10 09:04:40.571469 gigachain-0.1.7.1/langchain/utilities/tavily_search.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.818236 gigachain-0.1.7.1/langchain/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.819464 gigachain-0.1.7.1/langchain/utilities/twilio.py
--rw-r--r--   0        0        0      276 2023-12-18 12:05:47.820326 gigachain-0.1.7.1/langchain/utilities/vertexai.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.572515 gigachain-0.1.7.1/langchain/utilities/wikipedia.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.822016 gigachain-0.1.7.1/langchain/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.823234 gigachain-0.1.7.1/langchain/utilities/zapier.py
--rw-r--r--   0        0        0     1221 2023-12-18 12:05:47.824245 gigachain-0.1.7.1/langchain/utils/__init__.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.825271 gigachain-0.1.7.1/langchain/utils/aiter.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.826109 gigachain-0.1.7.1/langchain/utils/env.py
--rw-r--r--   0        0        0      325 2024-01-18 15:16:40.869253 gigachain-0.1.7.1/langchain/utils/ernie_functions.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.827383 gigachain-0.1.7.1/langchain/utils/formatting.py
--rw-r--r--   0        0        0      421 2023-12-18 12:05:47.828299 gigachain-0.1.7.1/langchain/utils/html.py
--rw-r--r--   0        0        0      211 2023-12-18 12:05:47.829085 gigachain-0.1.7.1/langchain/utils/input.py
--rw-r--r--   0        0        0      139 2024-01-18 15:16:40.869655 gigachain-0.1.7.1/langchain/utils/interactive_env.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.829865 gigachain-0.1.7.1/langchain/utils/iter.py
--rw-r--r--   0        0        0      258 2023-12-18 12:05:47.830615 gigachain-0.1.7.1/langchain/utils/json_schema.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.831372 gigachain-0.1.7.1/langchain/utils/loading.py
--rw-r--r--   0        0        0      181 2023-12-18 12:05:47.832276 gigachain-0.1.7.1/langchain/utils/math.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.833389 gigachain-0.1.7.1/langchain/utils/openai.py
--rw-r--r--   0        0        0      330 2023-12-18 12:05:47.834161 gigachain-0.1.7.1/langchain/utils/openai_functions.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.835107 gigachain-0.1.7.1/langchain/utils/pydantic.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:47.835836 gigachain-0.1.7.1/langchain/utils/strings.py
--rw-r--r--   0        0        0      446 2023-12-18 12:05:47.836793 gigachain-0.1.7.1/langchain/utils/utils.py
--rw-r--r--   0        0        0     2768 2024-02-05 09:38:07.062918 gigachain-0.1.7.1/langchain/vectorstores/__init__.py
--rw-r--r--   0        0        0      220 2024-01-10 09:04:40.575258 gigachain-0.1.7.1/langchain/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0      109 2024-01-10 09:04:40.576760 gigachain-0.1.7.1/langchain/vectorstores/analyticdb.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.580566 gigachain-0.1.7.1/langchain/vectorstores/annoy.py
--rw-r--r--   0        0        0      100 2024-01-10 09:04:40.583665 gigachain-0.1.7.1/langchain/vectorstores/astradb.py
--rw-r--r--   0        0        0       82 2023-12-18 12:05:47.842405 gigachain-0.1.7.1/langchain/vectorstores/atlas.py
--rw-r--r--   0        0        0       78 2024-01-10 09:04:40.584957 gigachain-0.1.7.1/langchain/vectorstores/awadb.py
--rw-r--r--   0        0        0      256 2024-01-10 09:04:40.586040 gigachain-0.1.7.1/langchain/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0      188 2024-01-10 09:04:40.587676 gigachain-0.1.7.1/langchain/vectorstores/azuresearch.py
--rw-r--r--   0        0        0       89 2024-01-10 09:04:40.589288 gigachain-0.1.7.1/langchain/vectorstores/bageldb.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.846640 gigachain-0.1.7.1/langchain/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.847689 gigachain-0.1.7.1/langchain/vectorstores/base.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.848672 gigachain-0.1.7.1/langchain/vectorstores/cassandra.py
--rw-r--r--   0        0        0       90 2024-01-10 09:04:40.590074 gigachain-0.1.7.1/langchain/vectorstores/chroma.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:47.850266 gigachain-0.1.7.1/langchain/vectorstores/clarifai.py
--rw-r--r--   0        0        0      148 2024-01-10 09:04:40.590843 gigachain-0.1.7.1/langchain/vectorstores/clickhouse.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.852012 gigachain-0.1.7.1/langchain/vectorstores/dashvector.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:47.852481 gigachain-0.1.7.1/langchain/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:47.853219 gigachain-0.1.7.1/langchain/vectorstores/deeplake.py
--rw-r--r--   0        0        0       78 2023-12-18 12:05:47.854024 gigachain-0.1.7.1/langchain/vectorstores/dingo.py
--rw-r--r--   0        0        0      236 2024-01-18 15:16:40.872866 gigachain-0.1.7.1/langchain/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.591768 gigachain-0.1.7.1/langchain/vectorstores/docarray/base.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.859528 gigachain-0.1.7.1/langchain/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.860361 gigachain-0.1.7.1/langchain/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0      184 2024-01-10 09:04:40.593248 gigachain-0.1.7.1/langchain/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0      362 2023-12-18 12:05:47.862557 gigachain-0.1.7.1/langchain/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0       84 2023-12-18 12:05:47.863374 gigachain-0.1.7.1/langchain/vectorstores/epsilla.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.594436 gigachain-0.1.7.1/langchain/vectorstores/faiss.py
--rw-r--r--   0        0        0       78 2024-01-10 09:04:40.595403 gigachain-0.1.7.1/langchain/vectorstores/hippo.py
--rw-r--r--   0        0        0       96 2024-01-10 09:04:40.596341 gigachain-0.1.7.1/langchain/vectorstores/hologres.py
--rw-r--r--   0        0        0       84 2023-12-18 12:05:47.867322 gigachain-0.1.7.1/langchain/vectorstores/lancedb.py
--rw-r--r--   0        0        0      128 2023-12-18 12:05:47.868167 gigachain-0.1.7.1/langchain/vectorstores/llm_rails.py
--rw-r--r--   0        0        0       78 2023-12-18 12:05:47.869093 gigachain-0.1.7.1/langchain/vectorstores/marqo.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.870058 gigachain-0.1.7.1/langchain/vectorstores/matching_engine.py
--rw-r--r--   0        0        0       96 2024-01-10 09:04:40.597226 gigachain-0.1.7.1/langchain/vectorstores/meilisearch.py
--rw-r--r--   0        0        0       81 2024-01-10 09:04:40.599173 gigachain-0.1.7.1/langchain/vectorstores/milvus.py
--rw-r--r--   0        0        0      128 2024-01-10 09:04:40.600394 gigachain-0.1.7.1/langchain/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0      192 2024-01-10 09:04:40.601389 gigachain-0.1.7.1/langchain/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0      179 2024-01-10 09:04:40.602397 gigachain-0.1.7.1/langchain/vectorstores/myscale.py
--rw-r--r--   0        0        0      147 2024-01-10 09:04:40.603441 gigachain-0.1.7.1/langchain/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.604618 gigachain-0.1.7.1/langchain/vectorstores/nucliadb.py
--rw-r--r--   0        0        0      147 2024-01-10 09:04:40.605556 gigachain-0.1.7.1/langchain/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0      234 2024-01-10 09:04:40.607685 gigachain-0.1.7.1/langchain/vectorstores/pgembedding.py
--rw-r--r--   0        0        0       93 2024-01-10 09:04:40.608761 gigachain-0.1.7.1/langchain/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0      149 2024-01-10 09:04:40.609389 gigachain-0.1.7.1/langchain/vectorstores/pgvector.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:47.880186 gigachain-0.1.7.1/langchain/vectorstores/pinecone.py
--rw-r--r--   0        0        0      130 2024-01-10 09:04:40.610308 gigachain-0.1.7.1/langchain/vectorstores/qdrant.py
--rw-r--r--   0        0        0      265 2023-09-12 10:52:10.695398 gigachain-0.1.7.1/langchain/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0      213 2024-01-10 09:04:40.611387 gigachain-0.1.7.1/langchain/vectorstores/redis/base.py
--rw-r--r--   0        0        0      416 2023-12-18 12:05:47.884194 gigachain-0.1.7.1/langchain/vectorstores/redis/filters.py
--rw-r--r--   0        0        0      503 2023-12-18 12:05:47.885024 gigachain-0.1.7.1/langchain/vectorstores/redis/schema.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.885729 gigachain-0.1.7.1/langchain/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.612428 gigachain-0.1.7.1/langchain/vectorstores/scann.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.887513 gigachain-0.1.7.1/langchain/vectorstores/semadb.py
--rw-r--r--   0        0        0      165 2024-01-10 09:04:40.613481 gigachain-0.1.7.1/langchain/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0      364 2024-01-10 09:04:40.614368 gigachain-0.1.7.1/langchain/vectorstores/sklearn.py
--rw-r--r--   0        0        0       90 2023-12-18 12:05:47.889663 gigachain-0.1.7.1/langchain/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0      154 2024-01-10 09:04:40.617741 gigachain-0.1.7.1/langchain/vectorstores/starrocks.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.891235 gigachain-0.1.7.1/langchain/vectorstores/supabase.py
--rw-r--r--   0        0        0       75 2024-01-10 09:04:40.620407 gigachain-0.1.7.1/langchain/vectorstores/tair.py
--rw-r--r--   0        0        0      191 2023-12-18 12:05:47.893009 gigachain-0.1.7.1/langchain/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.893937 gigachain-0.1.7.1/langchain/vectorstores/tigris.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.621429 gigachain-0.1.7.1/langchain/vectorstores/tiledb.py
--rw-r--r--   0        0        0      124 2024-01-10 09:04:40.622500 gigachain-0.1.7.1/langchain/vectorstores/timescalevector.py
--rw-r--r--   0        0        0       90 2023-12-18 12:05:47.896743 gigachain-0.1.7.1/langchain/vectorstores/typesense.py
--rw-r--r--   0        0        0       84 2024-01-10 09:04:40.623762 gigachain-0.1.7.1/langchain/vectorstores/usearch.py
--rw-r--r--   0        0        0      227 2023-12-18 12:05:47.898744 gigachain-0.1.7.1/langchain/vectorstores/utils.py
--rw-r--r--   0        0        0       75 2023-12-18 12:05:47.899754 gigachain-0.1.7.1/langchain/vectorstores/vald.py
--rw-r--r--   0        0        0       81 2024-01-10 09:04:40.624717 gigachain-0.1.7.1/langchain/vectorstores/vearch.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.901403 gigachain-0.1.7.1/langchain/vectorstores/vectara.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.902340 gigachain-0.1.7.1/langchain/vectorstores/vespa.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.625644 gigachain-0.1.7.1/langchain/vectorstores/weaviate.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.904061 gigachain-0.1.7.1/langchain/vectorstores/xata.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:47.904403 gigachain-0.1.7.1/langchain/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.905433 gigachain-0.1.7.1/langchain/vectorstores/zep.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.906395 gigachain-0.1.7.1/langchain/vectorstores/zilliz.py
--rw-r--r--   0        0        0    11760 2024-02-19 14:59:12.876975 gigachain-0.1.7.1/pyproject.toml
--rw-r--r--   0        0        0    13973 1970-01-01 00:00:00.000000 gigachain-0.1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-11-15 10:30:09.324245 gigachain-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5879 2024-02-22 08:54:03.058827 gigachain-0.1.9/README.md
+-rw-r--r--   0        0        0    14039 2024-02-22 08:54:03.062847 gigachain-0.1.9/langchain/__init__.py
+-rw-r--r--   0        0        0      667 2023-10-03 14:24:35.511215 gigachain-0.1.9/langchain/_api/__init__.py
+-rw-r--r--   0        0        0      471 2023-12-18 12:05:46.810499 gigachain-0.1.9/langchain/_api/deprecation.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:46.811728 gigachain-0.1.9/langchain/_api/path.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.531593 gigachain-0.1.9/langchain/adapters/__init__.py
+-rw-r--r--   0        0        0      653 2024-01-10 09:04:40.316153 gigachain-0.1.9/langchain/adapters/openai.py
+-rw-r--r--   0        0        0     4952 2024-02-22 08:54:03.066384 gigachain-0.1.9/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    54823 2024-02-22 08:54:03.070466 gigachain-0.1.9/langchain/agents/agent.py
+-rw-r--r--   0        0        0    15135 2024-02-22 08:54:03.072200 gigachain-0.1.9/langchain/agents/agent_iterator.py
+-rw-r--r--   0        0        0     3678 2024-02-22 08:54:03.075025 gigachain-0.1.9/langchain/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2023-08-24 07:36:02.856871 gigachain-0.1.9/langchain/agents/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:46.824912 gigachain-0.1.9/langchain/agents/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:46.825868 gigachain-0.1.9/langchain/agents/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      156 2023-12-18 12:05:46.826776 gigachain-0.1.9/langchain/agents/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:46.827627 gigachain-0.1.9/langchain/agents/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-10-06 14:43:01.368502 gigachain-0.1.9/langchain/agents/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:46.828657 gigachain-0.1.9/langchain/agents/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.534160 gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0     3235 2023-12-18 12:05:46.830026 gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
+-rw-r--r--   0        0        0       97 2023-10-30 16:05:53.823759 gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
+-rw-r--r--   0        0        0     1091 2023-12-18 12:05:46.831119 gigachain-0.1.9/langchain/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      177 2024-01-18 15:16:40.601939 gigachain-0.1.9/langchain/agents/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.318190 gigachain-0.1.9/langchain/agents/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-21 13:51:28.536932 gigachain-0.1.9/langchain/agents/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0      617 2023-12-18 12:05:46.832827 gigachain-0.1.9/langchain/agents/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2023-09-19 14:33:02.213182 gigachain-0.1.9/langchain/agents/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:46.833490 gigachain-0.1.9/langchain/agents/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2023-08-21 13:51:28.537602 gigachain-0.1.9/langchain/agents/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:46.834225 gigachain-0.1.9/langchain/agents/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2023-08-21 13:51:28.538134 gigachain-0.1.9/langchain/agents/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:46.834919 gigachain-0.1.9/langchain/agents/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2023-08-21 13:51:28.538568 gigachain-0.1.9/langchain/agents/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:46.835830 gigachain-0.1.9/langchain/agents/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0      126 2023-12-18 12:05:46.837036 gigachain-0.1.9/langchain/agents/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:46.841473 gigachain-0.1.9/langchain/agents/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2023-08-21 13:51:28.539651 gigachain-0.1.9/langchain/agents/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:46.842445 gigachain-0.1.9/langchain/agents/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2023-12-18 12:05:46.842756 gigachain-0.1.9/langchain/agents/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:46.843062 gigachain-0.1.9/langchain/agents/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.540099 gigachain-0.1.9/langchain/agents/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0       87 2023-12-18 12:05:46.843983 gigachain-0.1.9/langchain/agents/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0       96 2023-12-18 12:05:46.844896 gigachain-0.1.9/langchain/agents/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2023-08-21 13:51:28.541150 gigachain-0.1.9/langchain/agents/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:46.845738 gigachain-0.1.9/langchain/agents/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2023-08-21 13:51:28.541736 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:46.846914 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0      530 2024-01-10 09:04:40.319042 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0     1153 2023-12-18 12:05:46.848467 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0      186 2023-12-18 12:05:46.849502 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0      170 2023-12-18 12:05:46.850112 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0      157 2023-12-18 12:05:46.850853 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0     1104 2023-12-18 12:05:46.851835 gigachain-0.1.9/langchain/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0      174 2024-01-18 15:16:40.603187 gigachain-0.1.9/langchain/agents/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0      140 2023-12-18 12:05:46.852728 gigachain-0.1.9/langchain/agents/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-21 13:51:28.545958 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:46.853881 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:46.854708 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0      269 2023-12-18 12:05:46.855739 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:46.856940 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0     1094 2023-12-18 12:05:46.857872 gigachain-0.1.9/langchain/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:46.858297 gigachain-0.1.9/langchain/agents/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:46.859032 gigachain-0.1.9/langchain/agents/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0     1103 2023-12-18 12:05:46.860134 gigachain-0.1.9/langchain/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-21 13:51:28.548199 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0      123 2023-12-18 12:05:46.861223 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:46.862436 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:46.863534 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2023-08-21 13:51:28.549117 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:46.864520 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0      184 2023-12-18 12:05:46.865869 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:46.866709 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:46.867144 gigachain-0.1.9/langchain/agents/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:46.867506 gigachain-0.1.9/langchain/agents/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0       56 2023-08-21 13:51:28.549949 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/__init__.py
+-rw-r--r--   0        0        0     4211 2023-12-18 12:05:46.868458 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/base.py
+-rw-r--r--   0        0        0     1557 2023-08-31 07:54:47.805977 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/prompt.py
+-rw-r--r--   0        0        0     3001 2024-01-18 15:16:40.604061 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/toolkit.py
+-rw-r--r--   0        0        0     1095 2023-12-18 12:05:46.870552 gigachain-0.1.9/langchain/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-21 13:51:28.551302 gigachain-0.1.9/langchain/agents/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:46.871982 gigachain-0.1.9/langchain/agents/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0     1948 2024-01-30 12:21:20.018308 gigachain-0.1.9/langchain/agents/agent_types.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.551838 gigachain-0.1.9/langchain/agents/chat/__init__.py
+-rw-r--r--   0        0        0     5084 2024-02-22 08:54:03.075995 gigachain-0.1.9/langchain/agents/chat/base.py
+-rw-r--r--   0        0        0     1977 2024-02-22 08:54:03.079601 gigachain-0.1.9/langchain/agents/chat/output_parser.py
+-rw-r--r--   0        0        0     1776 2023-10-19 12:57:52.688319 gigachain-0.1.9/langchain/agents/chat/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-21 13:51:28.552791 gigachain-0.1.9/langchain/agents/conversational/__init__.py
+-rw-r--r--   0        0        0     4957 2024-02-22 08:54:03.081376 gigachain-0.1.9/langchain/agents/conversational/base.py
+-rw-r--r--   0        0        0     1463 2024-02-22 08:54:03.084332 gigachain-0.1.9/langchain/agents/conversational/output_parser.py
+-rw-r--r--   0        0        0     1312 2023-10-19 12:57:52.695256 gigachain-0.1.9/langchain/agents/conversational/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-21 13:51:28.553657 gigachain-0.1.9/langchain/agents/conversational_chat/__init__.py
+-rw-r--r--   0        0        0     5264 2024-02-22 08:54:03.087665 gigachain-0.1.9/langchain/agents/conversational_chat/base.py
+-rw-r--r--   0        0        0     2398 2024-02-22 08:54:03.088654 gigachain-0.1.9/langchain/agents/conversational_chat/output_parser.py
+-rw-r--r--   0        0        0     2934 2023-10-19 12:57:52.702190 gigachain-0.1.9/langchain/agents/conversational_chat/prompt.py
+-rw-r--r--   0        0        0      847 2023-11-10 13:07:49.983002 gigachain-0.1.9/langchain/agents/format_scratchpad/__init__.py
+-rw-r--r--   0        0        0     2209 2024-02-22 08:54:03.092203 gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_functions.py
+-rw-r--r--   0        0        0     1885 2024-02-22 08:54:03.093583 gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_tools.py
+-rw-r--r--   0        0        0      528 2023-12-18 12:05:46.881864 gigachain-0.1.9/langchain/agents/format_scratchpad/log.py
+-rw-r--r--   0        0        0      721 2023-12-18 12:05:46.882588 gigachain-0.1.9/langchain/agents/format_scratchpad/log_to_messages.py
+-rw-r--r--   0        0        0     2203 2023-12-18 12:05:46.883234 gigachain-0.1.9/langchain/agents/format_scratchpad/openai_functions.py
+-rw-r--r--   0        0        0     1885 2024-01-10 09:04:40.320052 gigachain-0.1.9/langchain/agents/format_scratchpad/openai_tools.py
+-rw-r--r--   0        0        0      578 2023-12-18 12:05:46.884524 gigachain-0.1.9/langchain/agents/format_scratchpad/xml.py
+-rw-r--r--   0        0        0        0 2024-02-22 08:54:03.093863 gigachain-0.1.9/langchain/agents/gigachat_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2567 2024-02-22 08:54:03.094866 gigachain-0.1.9/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0     4183 2024-02-22 08:54:03.097385 gigachain-0.1.9/langchain/agents/gigachat_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2024-02-22 08:54:03.097626 gigachain-0.1.9/langchain/agents/gigachat_tools/__init__.py
+-rw-r--r--   0        0        0     3243 2024-02-22 08:54:03.099768 gigachain-0.1.9/langchain/agents/gigachat_tools/base.py
+-rw-r--r--   0        0        0     3244 2024-02-22 08:54:03.100651 gigachain-0.1.9/langchain/agents/initialize.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:16:40.615878 gigachain-0.1.9/langchain/agents/json_chat/__init__.py
+-rw-r--r--   0        0        0     6832 2024-02-22 08:54:03.101790 gigachain-0.1.9/langchain/agents/json_chat/base.py
+-rw-r--r--   0        0        0      551 2024-01-18 15:16:40.617394 gigachain-0.1.9/langchain/agents/json_chat/prompt.py
+-rw-r--r--   0        0        0    23975 2024-03-01 11:50:11.615565 gigachain-0.1.9/langchain/agents/load_tools.py
+-rw-r--r--   0        0        0     4629 2024-02-22 08:54:03.106160 gigachain-0.1.9/langchain/agents/loading.py
+-rw-r--r--   0        0        0       86 2023-08-21 13:51:28.555248 gigachain-0.1.9/langchain/agents/mrkl/__init__.py
+-rw-r--r--   0        0        0     6046 2024-02-22 08:54:03.107273 gigachain-0.1.9/langchain/agents/mrkl/base.py
+-rw-r--r--   0        0        0     3407 2024-02-22 08:54:03.108171 gigachain-0.1.9/langchain/agents/mrkl/output_parser.py
+-rw-r--r--   0        0        0     1602 2023-12-18 12:05:46.889787 gigachain-0.1.9/langchain/agents/mrkl/prompt.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:46.890436 gigachain-0.1.9/langchain/agents/openai_assistant/__init__.py
+-rw-r--r--   0        0        0    25732 2024-02-22 08:54:03.113714 gigachain-0.1.9/langchain/agents/openai_assistant/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556082 gigachain-0.1.9/langchain/agents/openai_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2567 2023-12-18 12:05:46.893881 gigachain-0.1.9/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0    11522 2024-02-22 08:54:03.115573 gigachain-0.1.9/langchain/agents/openai_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556705 gigachain-0.1.9/langchain/agents/openai_functions_multi_agent/__init__.py
+-rw-r--r--   0        0        0    11944 2024-02-22 08:54:03.117313 gigachain-0.1.9/langchain/agents/openai_functions_multi_agent/base.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:16:40.628412 gigachain-0.1.9/langchain/agents/openai_tools/__init__.py
+-rw-r--r--   0        0        0     3388 2024-02-22 08:54:03.118744 gigachain-0.1.9/langchain/agents/openai_tools/base.py
+-rw-r--r--   0        0        0     1419 2024-02-22 08:54:03.121605 gigachain-0.1.9/langchain/agents/output_parsers/__init__.py
+-rw-r--r--   0        0        0     3210 2024-02-22 08:54:03.124433 gigachain-0.1.9/langchain/agents/output_parsers/gigachat_functions.py
+-rw-r--r--   0        0        0     1846 2024-02-22 08:54:03.125684 gigachain-0.1.9/langchain/agents/output_parsers/json.py
+-rw-r--r--   0        0        0     3467 2024-01-18 15:16:40.630141 gigachain-0.1.9/langchain/agents/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0     3492 2024-01-18 15:16:40.631038 gigachain-0.1.9/langchain/agents/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     2455 2024-02-22 08:54:03.126947 gigachain-0.1.9/langchain/agents/output_parsers/react_json_single_input.py
+-rw-r--r--   0        0        0     3218 2023-12-18 12:05:46.905924 gigachain-0.1.9/langchain/agents/output_parsers/react_single_input.py
+-rw-r--r--   0        0        0     1545 2023-12-18 12:05:46.906825 gigachain-0.1.9/langchain/agents/output_parsers/self_ask.py
+-rw-r--r--   0        0        0     1658 2023-12-18 12:05:46.907986 gigachain-0.1.9/langchain/agents/output_parsers/xml.py
+-rw-r--r--   0        0        0       76 2023-08-21 13:51:28.557154 gigachain-0.1.9/langchain/agents/react/__init__.py
+-rw-r--r--   0        0        0     3903 2024-02-22 08:54:03.128763 gigachain-0.1.9/langchain/agents/react/agent.py
+-rw-r--r--   0        0        0     5714 2024-02-22 08:54:03.130890 gigachain-0.1.9/langchain/agents/react/base.py
+-rw-r--r--   0        0        0     1231 2023-12-18 12:05:46.909814 gigachain-0.1.9/langchain/agents/react/output_parser.py
+-rw-r--r--   0        0        0     3005 2023-12-18 12:05:46.910755 gigachain-0.1.9/langchain/agents/react/textworld_prompt.py
+-rw-r--r--   0        0        0    10562 2023-12-18 12:05:46.911736 gigachain-0.1.9/langchain/agents/react/wiki_prompt.py
+-rw-r--r--   0        0        0     1175 2023-12-18 12:05:46.912970 gigachain-0.1.9/langchain/agents/schema.py
+-rw-r--r--   0        0        0      106 2023-08-21 13:51:28.559443 gigachain-0.1.9/langchain/agents/self_ask_with_search/__init__.py
+-rw-r--r--   0        0        0     8175 2024-02-22 08:54:03.134843 gigachain-0.1.9/langchain/agents/self_ask_with_search/base.py
+-rw-r--r--   0        0        0      138 2023-09-25 07:40:35.498979 gigachain-0.1.9/langchain/agents/self_ask_with_search/output_parser.py
+-rw-r--r--   0        0        0     3502 2023-12-18 12:05:46.916766 gigachain-0.1.9/langchain/agents/self_ask_with_search/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.560593 gigachain-0.1.9/langchain/agents/structured_chat/__init__.py
+-rw-r--r--   0        0        0     9948 2024-02-22 08:54:03.135995 gigachain-0.1.9/langchain/agents/structured_chat/base.py
+-rw-r--r--   0        0        0     3799 2024-02-22 08:54:03.137224 gigachain-0.1.9/langchain/agents/structured_chat/output_parser.py
+-rw-r--r--   0        0        0     1663 2023-09-07 06:38:18.010991 gigachain-0.1.9/langchain/agents/structured_chat/prompt.py
+-rw-r--r--   0        0        0     1409 2024-02-22 08:54:03.138801 gigachain-0.1.9/langchain/agents/tools.py
+-rw-r--r--   0        0        0     1475 2024-01-29 08:25:46.514870 gigachain-0.1.9/langchain/agents/types.py
+-rw-r--r--   0        0        0      384 2023-12-18 12:05:46.920460 gigachain-0.1.9/langchain/agents/utils.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.562209 gigachain-0.1.9/langchain/agents/xml/__init__.py
+-rw-r--r--   0        0        0     7258 2024-02-22 08:54:03.140006 gigachain-0.1.9/langchain/agents/xml/base.py
+-rw-r--r--   0        0        0      767 2024-01-18 15:16:40.638769 gigachain-0.1.9/langchain/agents/xml/prompt.py
+-rw-r--r--   0        0        0      217 2023-12-18 12:05:46.922138 gigachain-0.1.9/langchain/base_language.py
+-rw-r--r--   0        0        0      701 2024-01-10 09:04:40.325005 gigachain-0.1.9/langchain/cache.py
+-rw-r--r--   0        0        0     2509 2024-02-22 08:54:03.143127 gigachain-0.1.9/langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      211 2023-12-18 12:05:46.925154 gigachain-0.1.9/langchain/callbacks/aim_callback.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:46.925829 gigachain-0.1.9/langchain/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:46.926936 gigachain-0.1.9/langchain/callbacks/arize_callback.py
+-rw-r--r--   0        0        0      133 2024-01-10 09:04:40.325707 gigachain-0.1.9/langchain/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0      653 2024-02-22 08:54:03.144267 gigachain-0.1.9/langchain/callbacks/base.py
+-rw-r--r--   0        0        0      129 2024-01-10 09:04:40.326482 gigachain-0.1.9/langchain/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0      133 2024-01-10 09:04:40.327283 gigachain-0.1.9/langchain/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:46.931986 gigachain-0.1.9/langchain/callbacks/confident_callback.py
+-rw-r--r--   0        0        0      129 2024-01-10 09:04:40.328061 gigachain-0.1.9/langchain/callbacks/context_callback.py
+-rw-r--r--   0        0        0     2589 2024-02-22 08:54:03.145615 gigachain-0.1.9/langchain/callbacks/file.py
+-rw-r--r--   0        0        0      123 2024-01-10 09:04:40.328815 gigachain-0.1.9/langchain/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0      275 2024-01-10 09:04:40.329559 gigachain-0.1.9/langchain/callbacks/human.py
+-rw-r--r--   0        0        0      133 2024-01-10 09:04:40.330500 gigachain-0.1.9/langchain/callbacks/infino_callback.py
+-rw-r--r--   0        0        0      241 2023-12-18 12:05:46.936755 gigachain-0.1.9/langchain/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0      142 2024-01-10 09:04:40.331568 gigachain-0.1.9/langchain/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     1777 2023-12-18 12:05:46.938871 gigachain-0.1.9/langchain/callbacks/manager.py
+-rw-r--r--   0        0        0      305 2024-01-10 09:04:40.332484 gigachain-0.1.9/langchain/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0      113 2024-01-10 09:04:40.333267 gigachain-0.1.9/langchain/callbacks/openai_info.py
+-rw-r--r--   0        0        0      141 2024-01-10 09:04:40.333971 gigachain-0.1.9/langchain/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0      135 2024-01-10 09:04:40.334649 gigachain-0.1.9/langchain/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:46.944007 gigachain-0.1.9/langchain/callbacks/stdout.py
+-rw-r--r--   0        0        0     2399 2024-02-22 08:54:03.146818 gigachain-0.1.9/langchain/callbacks/streaming_aiter.py
+-rw-r--r--   0        0        0     3371 2023-12-18 12:05:46.945805 gigachain-0.1.9/langchain/callbacks/streaming_aiter_final_only.py
+-rw-r--r--   0        0        0      173 2024-02-22 08:54:03.147647 gigachain-0.1.9/langchain/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     3357 2024-02-22 08:54:03.148511 gigachain-0.1.9/langchain/callbacks/streaming_stdout_final_only.py
+-rw-r--r--   0        0        0     3190 2023-10-03 07:51:15.793630 gigachain-0.1.9/langchain/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0      185 2023-12-18 12:05:46.947518 gigachain-0.1.9/langchain/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0      490 2024-01-10 09:04:40.335344 gigachain-0.1.9/langchain/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      589 2023-12-18 12:05:46.949215 gigachain-0.1.9/langchain/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      154 2023-12-18 12:05:46.950003 gigachain-0.1.9/langchain/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      154 2024-01-10 09:04:40.336248 gigachain-0.1.9/langchain/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0      233 2023-12-18 12:05:46.951869 gigachain-0.1.9/langchain/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      218 2023-12-18 12:05:46.952818 gigachain-0.1.9/langchain/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:46.953574 gigachain-0.1.9/langchain/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2023-12-18 12:05:46.954653 gigachain-0.1.9/langchain/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0     1384 2023-12-18 12:05:46.955043 gigachain-0.1.9/langchain/callbacks/tracers/logging.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:46.955825 gigachain-0.1.9/langchain/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:46.956667 gigachain-0.1.9/langchain/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2023-12-18 12:05:46.957919 gigachain-0.1.9/langchain/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      168 2023-12-18 12:05:46.958747 gigachain-0.1.9/langchain/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0      229 2024-01-10 09:04:40.336940 gigachain-0.1.9/langchain/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0      132 2024-01-10 09:04:40.337840 gigachain-0.1.9/langchain/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0      403 2023-12-18 12:05:46.961334 gigachain-0.1.9/langchain/callbacks/utils.py
+-rw-r--r--   0        0        0      130 2024-01-10 09:04:40.338883 gigachain-0.1.9/langchain/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0      129 2024-01-10 09:04:40.339806 gigachain-0.1.9/langchain/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0     5951 2024-02-22 08:54:03.149844 gigachain-0.1.9/langchain/chains/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-21 13:51:28.576965 gigachain-0.1.9/langchain/chains/api/__init__.py
+-rw-r--r--   0        0        0     8919 2024-02-22 08:54:03.151385 gigachain-0.1.9/langchain/chains/api/base.py
+-rw-r--r--   0        0        0     2452 2024-01-10 09:04:40.341669 gigachain-0.1.9/langchain/chains/api/news_docs.py
+-rw-r--r--   0        0        0     3399 2023-08-21 13:51:28.578041 gigachain-0.1.9/langchain/chains/api/open_meteo_docs.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.578278 gigachain-0.1.9/langchain/chains/api/openapi/__init__.py
+-rw-r--r--   0        0        0     8786 2024-02-22 08:54:03.152480 gigachain-0.1.9/langchain/chains/api/openapi/chain.py
+-rw-r--r--   0        0        0     1791 2023-08-21 13:51:28.579000 gigachain-0.1.9/langchain/chains/api/openapi/prompts.py
+-rw-r--r--   0        0        0     2025 2023-12-18 12:05:46.968380 gigachain-0.1.9/langchain/chains/api/openapi/requests_chain.py
+-rw-r--r--   0        0        0     1847 2023-12-18 12:05:46.969509 gigachain-0.1.9/langchain/chains/api/openapi/response_chain.py
+-rw-r--r--   0        0        0     1920 2023-08-21 13:51:28.580702 gigachain-0.1.9/langchain/chains/api/podcast_docs.py
+-rw-r--r--   0        0        0     1326 2023-12-18 12:05:46.970482 gigachain-0.1.9/langchain/chains/api/prompt.py
+-rw-r--r--   0        0        0     1537 2023-08-21 13:51:28.581731 gigachain-0.1.9/langchain/chains/api/tmdb_docs.py
+-rw-r--r--   0        0        0    28487 2024-03-01 11:50:11.617337 gigachain-0.1.9/langchain/chains/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.582802 gigachain-0.1.9/langchain/chains/chat_vector_db/__init__.py
+-rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.972569 gigachain-0.1.9/langchain/chains/chat_vector_db/prompts.py
+-rw-r--r--   0        0        0      367 2024-01-10 09:04:40.342648 gigachain-0.1.9/langchain/chains/combine_documents/__init__.py
+-rw-r--r--   0        0        0     8094 2024-03-01 11:50:11.618347 gigachain-0.1.9/langchain/chains/combine_documents/base.py
+-rw-r--r--   0        0        0     1743 2023-11-15 10:30:09.330835 gigachain-0.1.9/langchain/chains/combine_documents/conditional.py
+-rw-r--r--   0        0        0    11781 2024-03-01 11:50:11.619466 gigachain-0.1.9/langchain/chains/combine_documents/map_reduce.py
+-rw-r--r--   0        0        0     8991 2024-03-01 11:50:11.620114 gigachain-0.1.9/langchain/chains/combine_documents/map_rerank.py
+-rw-r--r--   0        0        0    13894 2024-02-22 08:54:03.165440 gigachain-0.1.9/langchain/chains/combine_documents/reduce.py
+-rw-r--r--   0        0        0     9113 2024-02-22 08:54:03.166781 gigachain-0.1.9/langchain/chains/combine_documents/refine.py
+-rw-r--r--   0        0        0    11030 2024-02-22 08:54:03.169663 gigachain-0.1.9/langchain/chains/combine_documents/stuff.py
+-rw-r--r--   0        0        0      107 2023-08-21 13:51:28.587546 gigachain-0.1.9/langchain/chains/constitutional_ai/__init__.py
+-rw-r--r--   0        0        0     6341 2024-02-22 08:54:03.170812 gigachain-0.1.9/langchain/chains/constitutional_ai/base.py
+-rw-r--r--   0        0        0      283 2023-12-18 12:05:46.981590 gigachain-0.1.9/langchain/chains/constitutional_ai/models.py
+-rw-r--r--   0        0        0    21738 2023-08-21 13:51:28.588681 gigachain-0.1.9/langchain/chains/constitutional_ai/principles.py
+-rw-r--r--   0        0        0    14534 2023-12-18 12:05:46.982679 gigachain-0.1.9/langchain/chains/constitutional_ai/prompts.py
+-rw-r--r--   0        0        0       71 2023-08-21 13:51:28.589976 gigachain-0.1.9/langchain/chains/conversation/__init__.py
+-rw-r--r--   0        0        0     2366 2024-01-18 15:16:40.657291 gigachain-0.1.9/langchain/chains/conversation/base.py
+-rw-r--r--   0        0        0      856 2023-08-21 13:51:28.590517 gigachain-0.1.9/langchain/chains/conversation/memory.py
+-rw-r--r--   0        0        0     1063 2023-12-18 12:05:46.984228 gigachain-0.1.9/langchain/chains/conversation/prompt.py
+-rw-r--r--   0        0        0       49 2023-08-21 13:51:28.591153 gigachain-0.1.9/langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0    18065 2024-02-22 08:54:03.173623 gigachain-0.1.9/langchain/chains/conversational_retrieval/base.py
+-rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.988192 gigachain-0.1.9/langchain/chains/conversational_retrieval/prompts.py
+-rw-r--r--   0        0        0      126 2023-08-21 13:51:28.592942 gigachain-0.1.9/langchain/chains/elasticsearch_database/__init__.py
+-rw-r--r--   0        0        0     8287 2024-02-22 08:54:03.175145 gigachain-0.1.9/langchain/chains/elasticsearch_database/base.py
+-rw-r--r--   0        0        0     2480 2023-12-18 12:05:46.989727 gigachain-0.1.9/langchain/chains/elasticsearch_database/prompts.py
+-rw-r--r--   0        0        0      669 2023-10-30 16:05:53.857849 gigachain-0.1.9/langchain/chains/encoder.py
+-rw-r--r--   0        0        0      465 2023-12-18 12:05:46.990078 gigachain-0.1.9/langchain/chains/ernie_functions/__init__.py
+-rw-r--r--   0        0        0    23205 2024-03-01 11:50:11.621045 gigachain-0.1.9/langchain/chains/ernie_functions/base.py
+-rw-r--r--   0        0        0      741 2023-12-18 12:05:46.991949 gigachain-0.1.9/langchain/chains/example_generator.py
+-rw-r--r--   0        0        0       51 2023-08-21 13:51:28.594704 gigachain-0.1.9/langchain/chains/flare/__init__.py
+-rw-r--r--   0        0        0     9033 2024-02-22 08:54:03.177642 gigachain-0.1.9/langchain/chains/flare/base.py
+-rw-r--r--   0        0        0     1949 2023-12-18 12:05:46.993539 gigachain-0.1.9/langchain/chains/flare/prompts.py
+-rw-r--r--   0        0        0       49 2023-08-21 13:51:28.596462 gigachain-0.1.9/langchain/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0     8397 2024-02-22 08:54:03.178971 gigachain-0.1.9/langchain/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0     3671 2024-01-18 15:16:40.667708 gigachain-0.1.9/langchain/chains/graph_qa/base.py
+-rw-r--r--   0        0        0    10452 2024-02-22 08:54:03.179960 gigachain-0.1.9/langchain/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0     9625 2023-12-18 12:05:46.997918 gigachain-0.1.9/langchain/chains/graph_qa/cypher_utils.py
+-rw-r--r--   0        0        0     5272 2024-02-22 08:54:03.180901 gigachain-0.1.9/langchain/chains/graph_qa/falkordb.py
+-rw-r--r--   0        0        0     3717 2024-02-22 08:54:03.182056 gigachain-0.1.9/langchain/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0     3698 2024-02-22 08:54:03.182898 gigachain-0.1.9/langchain/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0     3692 2024-02-22 08:54:03.183710 gigachain-0.1.9/langchain/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     6890 2024-02-22 08:54:03.184676 gigachain-0.1.9/langchain/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0     6610 2024-02-22 08:54:03.185246 gigachain-0.1.9/langchain/chains/graph_qa/neptune_sparql.py
+-rw-r--r--   0        0        0     7226 2024-02-22 08:54:03.185912 gigachain-0.1.9/langchain/chains/graph_qa/ontotext_graphdb.py
+-rw-r--r--   0        0        0    25955 2024-02-22 08:54:03.189550 gigachain-0.1.9/langchain/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0     5838 2024-03-01 11:50:11.621545 gigachain-0.1.9/langchain/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0     2662 2024-01-10 09:04:40.353033 gigachain-0.1.9/langchain/chains/history_aware_retriever.py
+-rw-r--r--   0        0        0       75 2023-08-21 13:51:28.600763 gigachain-0.1.9/langchain/chains/hyde/__init__.py
+-rw-r--r--   0        0        0     3341 2024-02-22 08:54:03.191623 gigachain-0.1.9/langchain/chains/hyde/base.py
+-rw-r--r--   0        0        0     2482 2023-12-18 12:05:47.005583 gigachain-0.1.9/langchain/chains/hyde/prompts.py
+-rw-r--r--   0        0        0    15030 2024-02-22 08:54:03.195047 gigachain-0.1.9/langchain/chains/llm.py
+-rw-r--r--   0        0        0      450 2024-02-22 08:54:03.198689 gigachain-0.1.9/langchain/chains/llm_bash/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-21 13:51:28.604012 gigachain-0.1.9/langchain/chains/llm_checker/__init__.py
+-rw-r--r--   0        0        0     6164 2024-02-22 08:54:03.200128 gigachain-0.1.9/langchain/chains/llm_checker/base.py
+-rw-r--r--   0        0        0     1341 2023-12-18 12:05:47.009556 gigachain-0.1.9/langchain/chains/llm_checker/prompt.py
+-rw-r--r--   0        0        0      143 2023-08-21 13:51:28.605454 gigachain-0.1.9/langchain/chains/llm_math/__init__.py
+-rw-r--r--   0        0        0     6723 2024-02-22 08:54:03.201078 gigachain-0.1.9/langchain/chains/llm_math/base.py
+-rw-r--r--   0        0        0     1158 2023-12-18 12:05:47.012133 gigachain-0.1.9/langchain/chains/llm_math/prompt.py
+-rw-r--r--   0        0        0     3193 2024-02-22 08:54:03.201902 gigachain-0.1.9/langchain/chains/llm_requests.py
+-rw-r--r--   0        0        0      352 2023-08-21 13:51:28.607135 gigachain-0.1.9/langchain/chains/llm_summarization_checker/__init__.py
+-rw-r--r--   0        0        0     6582 2024-02-22 08:54:03.202882 gigachain-0.1.9/langchain/chains/llm_summarization_checker/base.py
+-rw-r--r--   0        0        0     1143 2023-08-22 11:25:59.886227 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
+-rw-r--r--   0        0        0      696 2023-08-22 11:25:59.887142 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
+-rw-r--r--   0        0        0      234 2023-08-22 11:25:59.887992 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
+-rw-r--r--   0        0        0      834 2023-08-22 11:25:59.888905 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
+-rw-r--r--   0        0        0      467 2024-02-22 08:54:03.205485 gigachain-0.1.9/langchain/chains/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0    25297 2024-02-22 08:54:03.209215 gigachain-0.1.9/langchain/chains/loading.py
+-rw-r--r--   0        0        0     3732 2024-02-22 08:54:03.210816 gigachain-0.1.9/langchain/chains/mapreduce.py
+-rw-r--r--   0        0        0     3086 2024-02-22 08:54:03.212255 gigachain-0.1.9/langchain/chains/moderation.py
+-rw-r--r--   0        0        0       96 2023-08-21 13:51:28.612079 gigachain-0.1.9/langchain/chains/natbot/__init__.py
+-rw-r--r--   0        0        0     4695 2024-02-22 08:54:03.213323 gigachain-0.1.9/langchain/chains/natbot/base.py
+-rw-r--r--   0        0        0    16050 2024-02-22 08:54:03.214508 gigachain-0.1.9/langchain/chains/natbot/crawler.py
+-rw-r--r--   0        0        0     6769 2023-12-18 12:05:47.020892 gigachain-0.1.9/langchain/chains/natbot/prompt.py
+-rw-r--r--   0        0        0     1357 2024-02-22 08:54:03.215313 gigachain-0.1.9/langchain/chains/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10080 2024-03-01 11:50:11.622695 gigachain-0.1.9/langchain/chains/openai_functions/base.py
+-rw-r--r--   0        0        0     3522 2024-03-01 11:50:11.624093 gigachain-0.1.9/langchain/chains/openai_functions/citation_fuzzy_match.py
+-rw-r--r--   0        0        0     4298 2024-03-01 11:50:11.625958 gigachain-0.1.9/langchain/chains/openai_functions/extraction.py
+-rw-r--r--   0        0        0    11311 2024-03-01 11:50:11.627637 gigachain-0.1.9/langchain/chains/openai_functions/openapi.py
+-rw-r--r--   0        0        0     3923 2024-03-01 11:50:11.628248 gigachain-0.1.9/langchain/chains/openai_functions/qa_with_structure.py
+-rw-r--r--   0        0        0     2665 2024-03-01 11:50:11.628741 gigachain-0.1.9/langchain/chains/openai_functions/tagging.py
+-rw-r--r--   0        0        0     1257 2023-08-21 13:51:28.616551 gigachain-0.1.9/langchain/chains/openai_functions/utils.py
+-rw-r--r--   0        0        0      134 2023-11-10 13:07:50.024454 gigachain-0.1.9/langchain/chains/openai_tools/__init__.py
+-rw-r--r--   0        0        0     1665 2024-02-22 08:54:03.220719 gigachain-0.1.9/langchain/chains/openai_tools/extraction.py
+-rw-r--r--   0        0        0     2015 2023-12-18 12:05:47.029972 gigachain-0.1.9/langchain/chains/prompt_selector.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.617097 gigachain-0.1.9/langchain/chains/qa_generation/__init__.py
+-rw-r--r--   0        0        0     2464 2024-02-22 08:54:03.221867 gigachain-0.1.9/langchain/chains/qa_generation/base.py
+-rw-r--r--   0        0        0     2657 2023-12-18 12:05:47.032423 gigachain-0.1.9/langchain/chains/qa_generation/prompt.py
+-rw-r--r--   0        0        0      173 2023-08-21 13:51:28.619059 gigachain-0.1.9/langchain/chains/qa_with_sources/__init__.py
+-rw-r--r--   0        0        0     7976 2024-02-22 08:54:03.223422 gigachain-0.1.9/langchain/chains/qa_with_sources/base.py
+-rw-r--r--   0        0        0     6793 2023-12-18 12:05:47.034152 gigachain-0.1.9/langchain/chains/qa_with_sources/loading.py
+-rw-r--r--   0        0        0     4144 2023-12-18 12:05:47.035020 gigachain-0.1.9/langchain/chains/qa_with_sources/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1764 2023-12-18 12:05:47.035786 gigachain-0.1.9/langchain/chains/qa_with_sources/refine_prompts.py
+-rw-r--r--   0        0        0     2459 2024-02-22 08:54:03.224282 gigachain-0.1.9/langchain/chains/qa_with_sources/retrieval.py
+-rw-r--r--   0        0        0     3471 2023-12-18 12:05:47.037437 gigachain-0.1.9/langchain/chains/qa_with_sources/stuff_prompt.py
+-rw-r--r--   0        0        0     2770 2024-02-22 08:54:03.225130 gigachain-0.1.9/langchain/chains/qa_with_sources/vector_db.py
+-rw-r--r--   0        0        0      131 2024-02-22 08:54:03.225931 gigachain-0.1.9/langchain/chains/query_constructor/__init__.py
+-rw-r--r--   0        0        0    13721 2024-02-22 08:54:03.230318 gigachain-0.1.9/langchain/chains/query_constructor/base.py
+-rw-r--r--   0        0        0     3191 2023-12-18 12:05:47.039898 gigachain-0.1.9/langchain/chains/query_constructor/ir.py
+-rw-r--r--   0        0        0     5707 2023-12-18 12:05:47.040791 gigachain-0.1.9/langchain/chains/query_constructor/parser.py
+-rw-r--r--   0        0        0    10146 2023-12-18 12:05:47.041579 gigachain-0.1.9/langchain/chains/query_constructor/prompt.py
+-rw-r--r--   0        0        0      321 2023-12-18 12:05:47.042242 gigachain-0.1.9/langchain/chains/query_constructor/schema.py
+-rw-r--r--   0        0        0     8503 2024-02-22 08:54:03.231561 gigachain-0.1.9/langchain/chains/question_answering/__init__.py
+-rw-r--r--   0        0        0     5425 2023-12-18 12:05:47.043620 gigachain-0.1.9/langchain/chains/question_answering/map_reduce_prompt.py
+-rw-r--r--   0        0        0     2477 2023-12-18 12:05:47.044547 gigachain-0.1.9/langchain/chains/question_answering/map_rerank_prompt.py
+-rw-r--r--   0        0        0     3133 2023-12-18 12:05:47.045293 gigachain-0.1.9/langchain/chains/question_answering/refine_prompts.py
+-rw-r--r--   0        0        0     1404 2023-12-18 12:05:47.046327 gigachain-0.1.9/langchain/chains/question_answering/stuff_prompt.py
+-rw-r--r--   0        0        0     2742 2024-01-18 15:16:40.690412 gigachain-0.1.9/langchain/chains/retrieval.py
+-rw-r--r--   0        0        0       62 2023-08-21 13:51:28.631121 gigachain-0.1.9/langchain/chains/retrieval_qa/__init__.py
+-rw-r--r--   0        0        0     9952 2024-02-22 08:54:03.232560 gigachain-0.1.9/langchain/chains/retrieval_qa/base.py
+-rw-r--r--   0        0        0      527 2023-12-18 12:05:47.048474 gigachain-0.1.9/langchain/chains/retrieval_qa/prompt.py
+-rw-r--r--   0        0        0      407 2023-08-21 13:51:28.632647 gigachain-0.1.9/langchain/chains/router/__init__.py
+-rw-r--r--   0        0        0     4571 2024-02-22 08:54:03.234029 gigachain-0.1.9/langchain/chains/router/base.py
+-rw-r--r--   0        0        0     1982 2024-02-22 08:54:03.234826 gigachain-0.1.9/langchain/chains/router/embedding_router.py
+-rw-r--r--   0        0        0     4283 2024-02-22 08:54:03.235785 gigachain-0.1.9/langchain/chains/router/llm_router.py
+-rw-r--r--   0        0        0     2245 2023-12-18 12:05:47.052334 gigachain-0.1.9/langchain/chains/router/multi_prompt.py
+-rw-r--r--   0        0        0     1849 2023-09-04 05:57:22.503454 gigachain-0.1.9/langchain/chains/router/multi_prompt_prompt.py
+-rw-r--r--   0        0        0     1904 2023-08-21 14:03:46.158141 gigachain-0.1.9/langchain/chains/router/multi_retrieval_prompt.py
+-rw-r--r--   0        0        0     3659 2024-01-18 15:16:40.692341 gigachain-0.1.9/langchain/chains/router/multi_retrieval_qa.py
+-rw-r--r--   0        0        0     7510 2024-02-22 08:54:03.236797 gigachain-0.1.9/langchain/chains/sequential.py
+-rw-r--r--   0        0        0       47 2023-08-21 13:51:28.636997 gigachain-0.1.9/langchain/chains/sql_database/__init__.py
+-rw-r--r--   0        0        0    30619 2024-02-22 08:54:03.240301 gigachain-0.1.9/langchain/chains/sql_database/prompt.py
+-rw-r--r--   0        0        0     5293 2024-02-22 08:54:03.241443 gigachain-0.1.9/langchain/chains/sql_database/query.py
+-rw-r--r--   0        0        0      204 2024-02-22 08:54:03.242140 gigachain-0.1.9/langchain/chains/structured_output/__init__.py
+-rw-r--r--   0        0        0    22268 2024-03-01 11:50:11.629251 gigachain-0.1.9/langchain/chains/structured_output/base.py
+-rw-r--r--   0        0        0     6711 2024-02-22 08:54:03.246577 gigachain-0.1.9/langchain/chains/summarize/__init__.py
+-rw-r--r--   0        0        0      271 2023-12-18 12:05:47.059118 gigachain-0.1.9/langchain/chains/summarize/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1138 2023-12-18 12:05:47.060439 gigachain-0.1.9/langchain/chains/summarize/refine_prompts.py
+-rw-r--r--   0        0        0      271 2023-12-18 12:05:47.061163 gigachain-0.1.9/langchain/chains/summarize/stuff_prompt.py
+-rw-r--r--   0        0        0     2369 2024-02-22 08:54:03.247840 gigachain-0.1.9/langchain/chains/transform.py
+-rw-r--r--   0        0        0      452 2023-09-12 10:52:10.662329 gigachain-0.1.9/langchain/chat_loaders/__init__.py
+-rw-r--r--   0        0        0       95 2023-12-18 12:05:47.064850 gigachain-0.1.9/langchain/chat_loaders/base.py
+-rw-r--r--   0        0        0      240 2023-12-18 12:05:47.066006 gigachain-0.1.9/langchain/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0       99 2024-01-10 09:04:40.356789 gigachain-0.1.9/langchain/chat_loaders/gmail.py
+-rw-r--r--   0        0        0      107 2023-12-18 12:05:47.067658 gigachain-0.1.9/langchain/chat_loaders/imessage.py
+-rw-r--r--   0        0        0      187 2023-12-18 12:05:47.068610 gigachain-0.1.9/langchain/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.069730 gigachain-0.1.9/langchain/chat_loaders/slack.py
+-rw-r--r--   0        0        0      107 2023-12-18 12:05:47.070887 gigachain-0.1.9/langchain/chat_loaders/telegram.py
+-rw-r--r--   0        0        0      290 2023-12-18 12:05:47.071655 gigachain-0.1.9/langchain/chat_loaders/utils.py
+-rw-r--r--   0        0        0      107 2023-12-18 12:05:47.072872 gigachain-0.1.9/langchain/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     1995 2024-01-18 15:16:40.697309 gigachain-0.1.9/langchain/chat_models/__init__.py
+-rw-r--r--   0        0        0      199 2024-01-10 09:04:40.357806 gigachain-0.1.9/langchain/chat_models/anthropic.py
+-rw-r--r--   0        0        0      103 2024-01-10 09:04:40.358738 gigachain-0.1.9/langchain/chat_models/anyscale.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.078945 gigachain-0.1.9/langchain/chat_models/azure_openai.py
+-rw-r--r--   0        0        0      189 2023-12-18 12:05:47.080365 gigachain-0.1.9/langchain/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0      110 2024-01-10 09:04:40.359766 gigachain-0.1.9/langchain/chat_models/baichuan.py
+-rw-r--r--   0        0        0      131 2024-01-10 09:04:40.360897 gigachain-0.1.9/langchain/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      268 2024-01-10 09:04:40.361805 gigachain-0.1.9/langchain/chat_models/base.py
+-rw-r--r--   0        0        0      131 2023-12-18 12:05:47.084089 gigachain-0.1.9/langchain/chat_models/bedrock.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.362621 gigachain-0.1.9/langchain/chat_models/cohere.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.085569 gigachain-0.1.9/langchain/chat_models/databricks.py
+-rw-r--r--   0        0        0       91 2024-01-10 09:04:40.363366 gigachain-0.1.9/langchain/chat_models/ernie.py
+-rw-r--r--   0        0        0      103 2024-01-10 09:04:40.364542 gigachain-0.1.9/langchain/chat_models/everlyai.py
+-rw-r--r--   0        0        0      169 2023-12-18 12:05:47.088330 gigachain-0.1.9/langchain/chat_models/fake.py
+-rw-r--r--   0        0        0      113 2024-01-10 09:04:40.365619 gigachain-0.1.9/langchain/chat_models/fireworks.py
+-rw-r--r--   0        0        0       95 2024-01-10 09:04:40.366318 gigachain-0.1.9/langchain/chat_models/gigachat.py
+-rw-r--r--   0        0        0      158 2024-01-10 09:04:40.367091 gigachain-0.1.9/langchain/chat_models/google_palm.py
+-rw-r--r--   0        0        0      114 2024-01-10 09:04:40.367972 gigachain-0.1.9/langchain/chat_models/human.py
+-rw-r--r--   0        0        0      107 2024-01-10 09:04:40.368737 gigachain-0.1.9/langchain/chat_models/hunyuan.py
+-rw-r--r--   0        0        0      159 2024-01-10 09:04:40.369542 gigachain-0.1.9/langchain/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      102 2024-01-10 09:04:40.370300 gigachain-0.1.9/langchain/chat_models/jinachat.py
+-rw-r--r--   0        0        0       94 2024-01-10 09:04:40.371073 gigachain-0.1.9/langchain/chat_models/konko.py
+-rw-r--r--   0        0        0      137 2024-01-10 09:04:40.371862 gigachain-0.1.9/langchain/chat_models/litellm.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.372837 gigachain-0.1.9/langchain/chat_models/meta.py
+-rw-r--r--   0        0        0      100 2024-01-10 09:04:40.373952 gigachain-0.1.9/langchain/chat_models/minimax.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.098332 gigachain-0.1.9/langchain/chat_models/mlflow.py
+-rw-r--r--   0        0        0      156 2024-01-10 09:04:40.375069 gigachain-0.1.9/langchain/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.375700 gigachain-0.1.9/langchain/chat_models/ollama.py
+-rw-r--r--   0        0        0      104 2024-01-10 09:04:40.377001 gigachain-0.1.9/langchain/chat_models/openai.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:47.102210 gigachain-0.1.9/langchain/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.103242 gigachain-0.1.9/langchain/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0      104 2024-01-10 09:04:40.377793 gigachain-0.1.9/langchain/chat_models/tongyi.py
+-rw-r--r--   0        0        0      110 2024-01-10 09:04:40.378622 gigachain-0.1.9/langchain/chat_models/vertexai.py
+-rw-r--r--   0        0        0      178 2024-01-10 09:04:40.379547 gigachain-0.1.9/langchain/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0      103 2024-01-10 09:04:40.380328 gigachain-0.1.9/langchain/chat_models/yandex.py
+-rw-r--r--   0        0        0     1184 2024-02-22 08:54:03.251031 gigachain-0.1.9/langchain/docstore/__init__.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.107159 gigachain-0.1.9/langchain/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.107958 gigachain-0.1.9/langchain/docstore/base.py
+-rw-r--r--   0        0        0       70 2023-12-18 12:05:47.108669 gigachain-0.1.9/langchain/docstore/document.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.109501 gigachain-0.1.9/langchain/docstore/in_memory.py
+-rw-r--r--   0        0        0       86 2023-12-18 12:05:47.110273 gigachain-0.1.9/langchain/docstore/wikipedia.py
+-rw-r--r--   0        0        0     5722 2024-02-22 08:54:03.254344 gigachain-0.1.9/langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.112427 gigachain-0.1.9/langchain/document_loaders/acreom.py
+-rw-r--r--   0        0        0      554 2023-12-18 12:05:47.113265 gigachain-0.1.9/langchain/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.114177 gigachain-0.1.9/langchain/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.115207 gigachain-0.1.9/langchain/document_loaders/airtable.py
+-rw-r--r--   0        0        0      116 2023-12-18 12:05:47.116053 gigachain-0.1.9/langchain/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0      113 2024-01-10 09:04:40.381440 gigachain-0.1.9/langchain/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.117596 gigachain-0.1.9/langchain/document_loaders/arxiv.py
+-rw-r--r--   0        0        0      190 2023-12-18 12:05:47.118350 gigachain-0.1.9/langchain/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0      116 2024-01-10 09:04:40.382547 gigachain-0.1.9/langchain/document_loaders/async_html.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.120014 gigachain-0.1.9/langchain/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:47.120412 gigachain-0.1.9/langchain/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0      166 2023-12-18 12:05:47.121235 gigachain-0.1.9/langchain/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0      151 2023-12-18 12:05:47.122051 gigachain-0.1.9/langchain/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0      146 2023-12-18 12:05:47.122866 gigachain-0.1.9/langchain/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.123637 gigachain-0.1.9/langchain/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.124374 gigachain-0.1.9/langchain/document_loaders/base.py
+-rw-r--r--   0        0        0      120 2024-01-10 09:04:40.383758 gigachain-0.1.9/langchain/document_loaders/base_o365.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.125960 gigachain-0.1.9/langchain/document_loaders/bibtex.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.126880 gigachain-0.1.9/langchain/document_loaders/bigquery.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.127706 gigachain-0.1.9/langchain/document_loaders/bilibili.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.128455 gigachain-0.1.9/langchain/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      374 2024-01-18 15:16:40.702123 gigachain-0.1.9/langchain/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0      140 2024-01-10 09:04:40.384621 gigachain-0.1.9/langchain/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.130737 gigachain-0.1.9/langchain/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0      138 2023-12-18 12:05:47.131488 gigachain-0.1.9/langchain/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0      172 2023-12-18 12:05:47.132145 gigachain-0.1.9/langchain/document_loaders/blockchain.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.132987 gigachain-0.1.9/langchain/document_loaders/brave_search.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.133606 gigachain-0.1.9/langchain/document_loaders/browserless.py
+-rw-r--r--   0        0        0      138 2023-12-18 12:05:47.134633 gigachain-0.1.9/langchain/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.135559 gigachain-0.1.9/langchain/document_loaders/chromium.py
+-rw-r--r--   0        0        0      146 2023-12-18 12:05:47.137221 gigachain-0.1.9/langchain/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0      118 2024-01-10 09:04:40.385398 gigachain-0.1.9/langchain/document_loaders/concurrent.py
+-rw-r--r--   0        0        0      154 2023-12-18 12:05:47.139495 gigachain-0.1.9/langchain/document_loaders/confluence.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.141295 gigachain-0.1.9/langchain/document_loaders/conllu.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.141905 gigachain-0.1.9/langchain/document_loaders/couchbase.py
+-rw-r--r--   0        0        0      156 2023-12-18 12:05:47.142595 gigachain-0.1.9/langchain/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0      116 2023-12-18 12:05:47.143458 gigachain-0.1.9/langchain/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.144613 gigachain-0.1.9/langchain/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0      163 2023-12-18 12:05:47.145949 gigachain-0.1.9/langchain/document_loaders/dataframe.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.147296 gigachain-0.1.9/langchain/document_loaders/diffbot.py
+-rw-r--r--   0        0        0      115 2024-01-10 09:04:40.386259 gigachain-0.1.9/langchain/document_loaders/directory.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.149307 gigachain-0.1.9/langchain/document_loaders/discord.py
+-rw-r--r--   0        0        0      119 2024-01-10 09:04:40.387645 gigachain-0.1.9/langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.150906 gigachain-0.1.9/langchain/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.151662 gigachain-0.1.9/langchain/document_loaders/dropbox.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.152424 gigachain-0.1.9/langchain/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0      177 2023-12-18 12:05:47.153750 gigachain-0.1.9/langchain/document_loaders/email.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.154940 gigachain-0.1.9/langchain/document_loaders/epub.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.156146 gigachain-0.1.9/langchain/document_loaders/etherscan.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.156948 gigachain-0.1.9/langchain/document_loaders/evernote.py
+-rw-r--r--   0        0        0      118 2023-12-18 12:05:47.158021 gigachain-0.1.9/langchain/document_loaders/excel.py
+-rw-r--r--   0        0        0      167 2023-12-18 12:05:47.158818 gigachain-0.1.9/langchain/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.160349 gigachain-0.1.9/langchain/document_loaders/fauna.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:47.161384 gigachain-0.1.9/langchain/document_loaders/figma.py
+-rw-r--r--   0        0        0      116 2023-12-18 12:05:47.163101 gigachain-0.1.9/langchain/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.164293 gigachain-0.1.9/langchain/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0      109 2024-01-10 09:04:40.388322 gigachain-0.1.9/langchain/document_loaders/generic.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.166270 gigachain-0.1.9/langchain/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.167324 gigachain-0.1.9/langchain/document_loaders/git.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.168806 gigachain-0.1.9/langchain/document_loaders/gitbook.py
+-rw-r--r--   0        0        0      160 2023-12-18 12:05:47.169956 gigachain-0.1.9/langchain/document_loaders/github.py
+-rw-r--r--   0        0        0      145 2023-12-18 12:05:47.171116 gigachain-0.1.9/langchain/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0      112 2024-01-10 09:04:40.389172 gigachain-0.1.9/langchain/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.173144 gigachain-0.1.9/langchain/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.174366 gigachain-0.1.9/langchain/document_loaders/helpers.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.175285 gigachain-0.1.9/langchain/document_loaders/hn.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.176378 gigachain-0.1.9/langchain/document_loaders/html.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.177108 gigachain-0.1.9/langchain/document_loaders/html_bs.py
+-rw-r--r--   0        0        0      144 2023-12-18 12:05:47.178240 gigachain-0.1.9/langchain/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.389976 gigachain-0.1.9/langchain/document_loaders/ifixit.py
+-rw-r--r--   0        0        0      118 2023-12-18 12:05:47.180404 gigachain-0.1.9/langchain/document_loaders/image.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.181253 gigachain-0.1.9/langchain/document_loaders/image_captions.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.182514 gigachain-0.1.9/langchain/document_loaders/imsdb.py
+-rw-r--r--   0        0        0       91 2024-01-10 09:04:40.390811 gigachain-0.1.9/langchain/document_loaders/iugu.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.391872 gigachain-0.1.9/langchain/document_loaders/joplin.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.184945 gigachain-0.1.9/langchain/document_loaders/json_loader.py
+-rw-r--r--   0        0        0      198 2023-12-18 12:05:47.185665 gigachain-0.1.9/langchain/document_loaders/lakefs.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.186694 gigachain-0.1.9/langchain/document_loaders/larksuite.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:47.188009 gigachain-0.1.9/langchain/document_loaders/markdown.py
+-rw-r--r--   0        0        0      122 2024-01-10 09:04:40.392640 gigachain-0.1.9/langchain/document_loaders/mastodon.py
+-rw-r--r--   0        0        0      110 2023-12-18 12:05:47.190950 gigachain-0.1.9/langchain/document_loaders/max_compute.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.191580 gigachain-0.1.9/langchain/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.192413 gigachain-0.1.9/langchain/document_loaders/merge.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.193132 gigachain-0.1.9/langchain/document_loaders/mhtml.py
+-rw-r--r--   0        0        0      131 2024-01-10 09:04:40.393450 gigachain-0.1.9/langchain/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.195107 gigachain-0.1.9/langchain/document_loaders/mongodb.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.196443 gigachain-0.1.9/langchain/document_loaders/news.py
+-rw-r--r--   0        0        0      196 2023-12-18 12:05:47.198825 gigachain-0.1.9/langchain/document_loaders/notebook.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.199713 gigachain-0.1.9/langchain/document_loaders/notion.py
+-rw-r--r--   0        0        0      112 2024-01-10 09:04:40.394263 gigachain-0.1.9/langchain/document_loaders/notiondb.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.201509 gigachain-0.1.9/langchain/document_loaders/nuclia.py
+-rw-r--r--   0        0        0      116 2023-12-18 12:05:47.202637 gigachain-0.1.9/langchain/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.203432 gigachain-0.1.9/langchain/document_loaders/obs_file.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.204584 gigachain-0.1.9/langchain/document_loaders/obsidian.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.205631 gigachain-0.1.9/langchain/document_loaders/odt.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.206554 gigachain-0.1.9/langchain/document_loaders/onedrive.py
+-rw-r--r--   0        0        0      125 2024-01-10 09:04:40.395058 gigachain-0.1.9/langchain/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0      109 2024-01-10 09:04:40.395856 gigachain-0.1.9/langchain/document_loaders/onenote.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.209150 gigachain-0.1.9/langchain/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.209977 gigachain-0.1.9/langchain/document_loaders/org_mode.py
+-rw-r--r--   0        0        0      789 2024-01-18 15:16:40.703524 gigachain-0.1.9/langchain/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0      225 2023-12-18 12:05:47.210876 gigachain-0.1.9/langchain/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.211715 gigachain-0.1.9/langchain/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.212945 gigachain-0.1.9/langchain/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0      176 2024-01-10 09:04:40.397095 gigachain-0.1.9/langchain/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      109 2024-01-18 15:16:40.704455 gigachain-0.1.9/langchain/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.214977 gigachain-0.1.9/langchain/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      136 2024-01-18 15:16:40.705628 gigachain-0.1.9/langchain/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.216206 gigachain-0.1.9/langchain/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.217158 gigachain-0.1.9/langchain/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0      141 2023-12-18 12:05:47.217871 gigachain-0.1.9/langchain/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:47.218842 gigachain-0.1.9/langchain/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.219645 gigachain-0.1.9/langchain/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.220840 gigachain-0.1.9/langchain/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0      494 2024-01-10 09:04:40.398416 gigachain-0.1.9/langchain/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0      112 2024-01-10 09:04:40.399315 gigachain-0.1.9/langchain/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.223502 gigachain-0.1.9/langchain/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0      706 2023-12-18 12:05:47.224305 gigachain-0.1.9/langchain/document_loaders/pdf.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.225423 gigachain-0.1.9/langchain/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.226416 gigachain-0.1.9/langchain/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.227234 gigachain-0.1.9/langchain/document_loaders/psychic.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.228478 gigachain-0.1.9/langchain/document_loaders/pubmed.py
+-rw-r--r--   0        0        0      137 2023-12-18 12:05:47.229728 gigachain-0.1.9/langchain/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.230746 gigachain-0.1.9/langchain/document_loaders/python.py
+-rw-r--r--   0        0        0       91 2024-01-10 09:04:40.400297 gigachain-0.1.9/langchain/document_loaders/quip.py
+-rw-r--r--   0        0        0      128 2024-01-10 09:04:40.401198 gigachain-0.1.9/langchain/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0      132 2024-01-10 09:04:40.402205 gigachain-0.1.9/langchain/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0      116 2024-01-10 09:04:40.403129 gigachain-0.1.9/langchain/document_loaders/reddit.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.234795 gigachain-0.1.9/langchain/document_loaders/roam.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.403904 gigachain-0.1.9/langchain/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.236908 gigachain-0.1.9/langchain/document_loaders/rspace.py
+-rw-r--r--   0        0        0       96 2023-12-18 12:05:47.237697 gigachain-0.1.9/langchain/document_loaders/rss.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.238291 gigachain-0.1.9/langchain/document_loaders/rst.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.239100 gigachain-0.1.9/langchain/document_loaders/rtf.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.239781 gigachain-0.1.9/langchain/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.240496 gigachain-0.1.9/langchain/document_loaders/s3_file.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.241193 gigachain-0.1.9/langchain/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0      116 2024-01-10 09:04:40.404728 gigachain-0.1.9/langchain/document_loaders/sitemap.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.243092 gigachain-0.1.9/langchain/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.243833 gigachain-0.1.9/langchain/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0      112 2024-01-10 09:04:40.405568 gigachain-0.1.9/langchain/document_loaders/spreedly.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.245722 gigachain-0.1.9/langchain/document_loaders/srt.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.406422 gigachain-0.1.9/langchain/document_loaders/stripe.py
+-rw-r--r--   0        0        0      275 2023-12-18 12:05:47.248314 gigachain-0.1.9/langchain/document_loaders/telegram.py
+-rw-r--r--   0        0        0      147 2023-12-18 12:05:47.249456 gigachain-0.1.9/langchain/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0      123 2023-12-18 12:05:47.250244 gigachain-0.1.9/langchain/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0      141 2023-12-18 12:05:47.250861 gigachain-0.1.9/langchain/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.251412 gigachain-0.1.9/langchain/document_loaders/text.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.252277 gigachain-0.1.9/langchain/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.253561 gigachain-0.1.9/langchain/document_loaders/toml.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.254464 gigachain-0.1.9/langchain/document_loaders/trello.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.255363 gigachain-0.1.9/langchain/document_loaders/tsv.py
+-rw-r--r--   0        0        0      119 2024-01-10 09:04:40.407370 gigachain-0.1.9/langchain/document_loaders/twitter.py
+-rw-r--r--   0        0        0      601 2023-12-18 12:05:47.259283 gigachain-0.1.9/langchain/document_loaders/unstructured.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.260397 gigachain-0.1.9/langchain/document_loaders/url.py
+-rw-r--r--   0        0        0      236 2023-12-18 12:05:47.261334 gigachain-0.1.9/langchain/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.262991 gigachain-0.1.9/langchain/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.263820 gigachain-0.1.9/langchain/document_loaders/weather.py
+-rw-r--r--   0        0        0      110 2024-01-10 09:04:40.408467 gigachain-0.1.9/langchain/document_loaders/web_base.py
+-rw-r--r--   0        0        0      167 2023-12-18 12:05:47.265747 gigachain-0.1.9/langchain/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.266913 gigachain-0.1.9/langchain/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0      187 2023-12-18 12:05:47.268711 gigachain-0.1.9/langchain/document_loaders/word_document.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.269613 gigachain-0.1.9/langchain/document_loaders/xml.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.270340 gigachain-0.1.9/langchain/document_loaders/xorbits.py
+-rw-r--r--   0        0        0      218 2024-01-10 09:04:40.409212 gigachain-0.1.9/langchain/document_loaders/youtube.py
+-rw-r--r--   0        0        0     1616 2024-02-22 08:54:03.257298 gigachain-0.1.9/langchain/document_transformers/__init__.py
+-rw-r--r--   0        0        0      155 2024-01-10 09:04:40.410215 gigachain-0.1.9/langchain/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0      149 2023-12-18 12:05:47.274031 gigachain-0.1.9/langchain/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:47.274901 gigachain-0.1.9/langchain/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0      145 2023-12-18 12:05:47.275765 gigachain-0.1.9/langchain/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0      487 2024-01-10 09:04:40.411019 gigachain-0.1.9/langchain/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0      149 2023-12-18 12:05:47.277716 gigachain-0.1.9/langchain/document_transformers/google_translate.py
+-rw-r--r--   0        0        0      121 2023-12-18 12:05:47.278875 gigachain-0.1.9/langchain/document_transformers/html2text.py
+-rw-r--r--   0        0        0     2042 2023-10-30 16:05:53.900619 gigachain-0.1.9/langchain/document_transformers/loading.py
+-rw-r--r--   0        0        0      137 2024-01-10 09:04:40.411886 gigachain-0.1.9/langchain/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0      144 2023-12-18 12:05:47.280608 gigachain-0.1.9/langchain/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0      191 2023-12-18 12:05:47.281371 gigachain-0.1.9/langchain/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     2103 2023-10-30 16:05:53.902104 gigachain-0.1.9/langchain/document_transformers/serializers.py
+-rw-r--r--   0        0        0     6033 2023-10-06 14:43:01.456268 gigachain-0.1.9/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     3598 2024-02-22 08:54:03.259977 gigachain-0.1.9/langchain/embeddings/__init__.py
+-rw-r--r--   0        0        0      248 2023-12-18 12:05:47.283533 gigachain-0.1.9/langchain/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0       90 2023-12-18 12:05:47.284257 gigachain-0.1.9/langchain/embeddings/awa.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.285011 gigachain-0.1.9/langchain/embeddings/azure_openai.py
+-rw-r--r--   0        0        0      142 2023-12-18 12:05:47.285672 gigachain-0.1.9/langchain/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.286522 gigachain-0.1.9/langchain/embeddings/base.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:47.287374 gigachain-0.1.9/langchain/embeddings/bedrock.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.412764 gigachain-0.1.9/langchain/embeddings/bookend.py
+-rw-r--r--   0        0        0     8260 2024-02-22 08:54:03.263810 gigachain-0.1.9/langchain/embeddings/cache.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.292653 gigachain-0.1.9/langchain/embeddings/clarifai.py
+-rw-r--r--   0        0        0      148 2024-01-10 09:04:40.413596 gigachain-0.1.9/langchain/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:47.293939 gigachain-0.1.9/langchain/embeddings/cohere.py
+-rw-r--r--   0        0        0      117 2024-01-10 09:04:40.414696 gigachain-0.1.9/langchain/embeddings/dashscope.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.415721 gigachain-0.1.9/langchain/embeddings/databricks.py
+-rw-r--r--   0        0        0      117 2024-01-10 09:04:40.416625 gigachain-0.1.9/langchain/embeddings/deepinfra.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:47.297444 gigachain-0.1.9/langchain/embeddings/edenai.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.298257 gigachain-0.1.9/langchain/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0      115 2024-01-10 09:04:40.417442 gigachain-0.1.9/langchain/embeddings/embaas.py
+-rw-r--r--   0        0        0       96 2023-12-18 12:05:47.299986 gigachain-0.1.9/langchain/embeddings/ernie.py
+-rw-r--r--   0        0        0      164 2023-12-18 12:05:47.300774 gigachain-0.1.9/langchain/embeddings/fake.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.301576 gigachain-0.1.9/langchain/embeddings/fastembed.py
+-rw-r--r--   0        0        0      121 2024-01-10 09:04:40.418811 gigachain-0.1.9/langchain/embeddings/google_palm.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:47.303315 gigachain-0.1.9/langchain/embeddings/gpt4all.py
+-rw-r--r--   0        0        0      108 2024-01-10 09:04:40.419865 gigachain-0.1.9/langchain/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0      344 2024-01-10 09:04:40.420673 gigachain-0.1.9/langchain/embeddings/huggingface.py
+-rw-r--r--   0        0        0      133 2024-01-10 09:04:40.421652 gigachain-0.1.9/langchain/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0      200 2023-12-18 12:05:47.305872 gigachain-0.1.9/langchain/embeddings/infinity.py
+-rw-r--r--   0        0        0      140 2024-01-10 09:04:40.422554 gigachain-0.1.9/langchain/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0       93 2023-12-18 12:05:47.307827 gigachain-0.1.9/langchain/embeddings/jina.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.308610 gigachain-0.1.9/langchain/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.309681 gigachain-0.1.9/langchain/embeddings/llamacpp.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.310693 gigachain-0.1.9/langchain/embeddings/llm_rails.py
+-rw-r--r--   0        0        0      118 2024-01-10 09:04:40.423295 gigachain-0.1.9/langchain/embeddings/localai.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.424032 gigachain-0.1.9/langchain/embeddings/minimax.py
+-rw-r--r--   0        0        0       99 2024-01-10 09:04:40.425886 gigachain-0.1.9/langchain/embeddings/mlflow.py
+-rw-r--r--   0        0        0      134 2024-01-10 09:04:40.427005 gigachain-0.1.9/langchain/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.314820 gigachain-0.1.9/langchain/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.315663 gigachain-0.1.9/langchain/embeddings/mosaicml.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.316642 gigachain-0.1.9/langchain/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0      119 2024-01-10 09:04:40.427920 gigachain-0.1.9/langchain/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:47.318757 gigachain-0.1.9/langchain/embeddings/ollama.py
+-rw-r--r--   0        0        0      115 2024-01-10 09:04:40.429049 gigachain-0.1.9/langchain/embeddings/openai.py
+-rw-r--r--   0        0        0      200 2023-12-18 12:05:47.321173 gigachain-0.1.9/langchain/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      121 2024-01-10 09:04:40.429895 gigachain-0.1.9/langchain/embeddings/self_hosted.py
+-rw-r--r--   0        0        0      255 2024-01-10 09:04:40.430809 gigachain-0.1.9/langchain/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      148 2023-12-18 12:05:47.324200 gigachain-0.1.9/langchain/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0      107 2023-12-18 12:05:47.325329 gigachain-0.1.9/langchain/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0      130 2024-01-10 09:04:40.432025 gigachain-0.1.9/langchain/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.327137 gigachain-0.1.9/langchain/embeddings/vertexai.py
+-rw-r--r--   0        0        0      117 2024-01-10 09:04:40.433066 gigachain-0.1.9/langchain/embeddings/voyageai.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.328934 gigachain-0.1.9/langchain/embeddings/xinference.py
+-rw-r--r--   0        0        0      476 2023-08-21 13:51:28.799282 gigachain-0.1.9/langchain/env.py
+-rw-r--r--   0        0        0     5803 2023-10-30 16:05:53.905619 gigachain-0.1.9/langchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-21 13:51:28.800913 gigachain-0.1.9/langchain/evaluation/agents/__init__.py
+-rw-r--r--   0        0        0    13884 2024-02-22 08:54:03.265154 gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_chain.py
+-rw-r--r--   0        0        0     9688 2023-12-18 12:05:47.331055 gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_prompt.py
+-rw-r--r--   0        0        0     1400 2024-01-18 15:16:40.713791 gigachain-0.1.9/langchain/evaluation/comparison/__init__.py
+-rw-r--r--   0        0        0    16056 2024-01-18 15:16:40.715217 gigachain-0.1.9/langchain/evaluation/comparison/eval_chain.py
+-rw-r--r--   0        0        0     2358 2023-12-18 12:05:47.333888 gigachain-0.1.9/langchain/evaluation/comparison/prompt.py
+-rw-r--r--   0        0        0     1647 2024-01-18 15:16:40.716003 gigachain-0.1.9/langchain/evaluation/criteria/__init__.py
+-rw-r--r--   0        0        0    21358 2024-01-18 15:16:40.717295 gigachain-0.1.9/langchain/evaluation/criteria/eval_chain.py
+-rw-r--r--   0        0        0     2723 2023-12-18 12:05:47.336070 gigachain-0.1.9/langchain/evaluation/criteria/prompt.py
+-rw-r--r--   0        0        0      323 2023-08-21 13:51:28.806871 gigachain-0.1.9/langchain/evaluation/embedding_distance/__init__.py
+-rw-r--r--   0        0        0    15503 2024-01-18 15:16:40.719400 gigachain-0.1.9/langchain/evaluation/embedding_distance/base.py
+-rw-r--r--   0        0        0        0 2023-10-03 07:51:15.890624 gigachain-0.1.9/langchain/evaluation/exact_match/__init__.py
+-rw-r--r--   0        0        0     2751 2023-10-03 07:51:15.891318 gigachain-0.1.9/langchain/evaluation/exact_match/base.py
+-rw-r--r--   0        0        0     6693 2024-01-18 15:16:40.720469 gigachain-0.1.9/langchain/evaluation/loading.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.807950 gigachain-0.1.9/langchain/evaluation/parsing/__init__.py
+-rw-r--r--   0        0        0     5246 2024-01-18 15:16:40.721461 gigachain-0.1.9/langchain/evaluation/parsing/base.py
+-rw-r--r--   0        0        0     3679 2023-10-30 16:05:53.907474 gigachain-0.1.9/langchain/evaluation/parsing/json_distance.py
+-rw-r--r--   0        0        0     3197 2023-10-30 16:05:53.907950 gigachain-0.1.9/langchain/evaluation/parsing/json_schema.py
+-rw-r--r--   0        0        0      344 2023-08-21 13:51:28.808592 gigachain-0.1.9/langchain/evaluation/qa/__init__.py
+-rw-r--r--   0        0        0    10886 2023-12-18 12:05:47.339833 gigachain-0.1.9/langchain/evaluation/qa/eval_chain.py
+-rw-r--r--   0        0        0     6525 2023-12-18 12:05:47.340520 gigachain-0.1.9/langchain/evaluation/qa/eval_prompt.py
+-rw-r--r--   0        0        0     1052 2023-12-18 12:05:47.341163 gigachain-0.1.9/langchain/evaluation/qa/generate_chain.py
+-rw-r--r--   0        0        0      917 2023-12-18 12:05:47.341977 gigachain-0.1.9/langchain/evaluation/qa/generate_prompt.py
+-rw-r--r--   0        0        0        0 2023-10-03 07:51:15.892405 gigachain-0.1.9/langchain/evaluation/regex_match/__init__.py
+-rw-r--r--   0        0        0     2407 2023-10-03 07:51:15.893632 gigachain-0.1.9/langchain/evaluation/regex_match/base.py
+-rw-r--r--   0        0        0    18197 2024-01-18 15:16:40.722881 gigachain-0.1.9/langchain/evaluation/schema.py
+-rw-r--r--   0        0        0     1112 2024-01-18 15:16:40.723972 gigachain-0.1.9/langchain/evaluation/scoring/__init__.py
+-rw-r--r--   0        0        0    15656 2024-01-18 15:16:40.725217 gigachain-0.1.9/langchain/evaluation/scoring/eval_chain.py
+-rw-r--r--   0        0        0     2129 2023-12-18 12:05:47.344553 gigachain-0.1.9/langchain/evaluation/scoring/prompt.py
+-rw-r--r--   0        0        0      285 2023-08-21 13:51:28.811472 gigachain-0.1.9/langchain/evaluation/string_distance/__init__.py
+-rw-r--r--   0        0        0    14014 2023-12-18 12:05:47.346023 gigachain-0.1.9/langchain/evaluation/string_distance/base.py
+-rw-r--r--   0        0        0      141 2023-08-21 13:51:28.812128 gigachain-0.1.9/langchain/example_generator.py
+-rw-r--r--   0        0        0      167 2023-12-18 12:05:47.347238 gigachain-0.1.9/langchain/formatting.py
+-rw-r--r--   0        0        0     7435 2023-12-18 12:05:47.348391 gigachain-0.1.9/langchain/globals/__init__.py
+-rw-r--r--   0        0        0     1104 2024-02-22 08:54:03.267822 gigachain-0.1.9/langchain/graphs/__init__.py
+-rw-r--r--   0        0        0      148 2024-01-10 09:04:40.437971 gigachain-0.1.9/langchain/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0      113 2024-01-10 09:04:40.438954 gigachain-0.1.9/langchain/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0      141 2023-12-18 12:05:47.350721 gigachain-0.1.9/langchain/graphs/graph_document.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.351490 gigachain-0.1.9/langchain/graphs/graph_store.py
+-rw-r--r--   0        0        0       84 2023-12-18 12:05:47.352513 gigachain-0.1.9/langchain/graphs/hugegraph.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.353474 gigachain-0.1.9/langchain/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0      106 2024-01-10 09:04:40.439872 gigachain-0.1.9/langchain/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0       91 2024-01-10 09:04:40.440630 gigachain-0.1.9/langchain/graphs/nebula_graph.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.441708 gigachain-0.1.9/langchain/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0       94 2024-01-10 09:04:40.442566 gigachain-0.1.9/langchain/graphs/neptune_graph.py
+-rw-r--r--   0        0        0      299 2023-12-18 12:05:47.358092 gigachain-0.1.9/langchain/graphs/networkx_graph.py
+-rw-r--r--   0        0        0       98 2024-01-10 09:04:40.443339 gigachain-0.1.9/langchain/graphs/rdf_graph.py
+-rw-r--r--   0        0        0     2874 2023-12-18 12:05:47.360240 gigachain-0.1.9/langchain/hub.py
+-rw-r--r--   0        0        0      902 2024-03-01 11:50:11.630290 gigachain-0.1.9/langchain/indexes/__init__.py
+-rw-r--r--   0        0        0    22479 2024-02-22 08:54:03.268766 gigachain-0.1.9/langchain/indexes/_api.py
+-rw-r--r--   0        0        0    20556 2024-02-22 08:54:03.269921 gigachain-0.1.9/langchain/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0     5221 2023-10-19 12:57:52.916879 gigachain-0.1.9/langchain/indexes/base.py
+-rw-r--r--   0        0        0     1752 2024-01-18 15:16:40.727874 gigachain-0.1.9/langchain/indexes/graph.py
+-rw-r--r--   0        0        0       49 2023-08-21 13:51:28.816990 gigachain-0.1.9/langchain/indexes/prompts/__init__.py
+-rw-r--r--   0        0        0     3241 2023-12-18 12:05:47.364265 gigachain-0.1.9/langchain/indexes/prompts/entity_extraction.py
+-rw-r--r--   0        0        0     1797 2023-12-18 12:05:47.365149 gigachain-0.1.9/langchain/indexes/prompts/entity_summarization.py
+-rw-r--r--   0        0        0     2276 2024-01-18 15:16:40.730868 gigachain-0.1.9/langchain/indexes/prompts/knowledge_triplet_extraction.py
+-rw-r--r--   0        0        0     3423 2024-01-18 15:16:40.731835 gigachain-0.1.9/langchain/indexes/vectorstore.py
+-rw-r--r--   0        0        0      282 2023-12-18 12:05:47.367912 gigachain-0.1.9/langchain/input.py
+-rw-r--r--   0        0        0    17126 2024-02-22 08:54:03.273345 gigachain-0.1.9/langchain/llms/__init__.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.373059 gigachain-0.1.9/langchain/llms/ai21.py
+-rw-r--r--   0        0        0       86 2023-12-18 12:05:47.375795 gigachain-0.1.9/langchain/llms/aleph_alpha.py
+-rw-r--r--   0        0        0      114 2024-01-10 09:04:40.445264 gigachain-0.1.9/langchain/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0       82 2024-01-10 09:04:40.446089 gigachain-0.1.9/langchain/llms/anthropic.py
+-rw-r--r--   0        0        0       88 2024-01-10 09:04:40.446963 gigachain-0.1.9/langchain/llms/anyscale.py
+-rw-r--r--   0        0        0       70 2023-12-18 12:05:47.380664 gigachain-0.1.9/langchain/llms/arcee.py
+-rw-r--r--   0        0        0       82 2024-01-10 09:04:40.448322 gigachain-0.1.9/langchain/llms/aviary.py
+-rw-r--r--   0        0        0      507 2023-12-18 12:05:47.382858 gigachain-0.1.9/langchain/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.383805 gigachain-0.1.9/langchain/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0       76 2023-12-18 12:05:47.384682 gigachain-0.1.9/langchain/llms/bananadev.py
+-rw-r--r--   0        0        0      228 2024-01-10 09:04:40.449816 gigachain-0.1.9/langchain/llms/base.py
+-rw-r--r--   0        0        0       76 2023-12-18 12:05:47.386653 gigachain-0.1.9/langchain/llms/baseten.py
+-rw-r--r--   0        0        0       67 2024-01-10 09:04:40.450756 gigachain-0.1.9/langchain/llms/beam.py
+-rw-r--r--   0        0        0      128 2024-01-10 09:04:40.451692 gigachain-0.1.9/langchain/llms/bedrock.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.389069 gigachain-0.1.9/langchain/llms/bittensor.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.389772 gigachain-0.1.9/langchain/llms/cerebriumai.py
+-rw-r--r--   0        0        0       76 2023-12-18 12:05:47.390471 gigachain-0.1.9/langchain/llms/chatglm.py
+-rw-r--r--   0        0        0       79 2024-01-10 09:04:40.452477 gigachain-0.1.9/langchain/llms/clarifai.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.391687 gigachain-0.1.9/langchain/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0       89 2024-01-10 09:04:40.453363 gigachain-0.1.9/langchain/llms/cohere.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.393292 gigachain-0.1.9/langchain/llms/ctransformers.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.394040 gigachain-0.1.9/langchain/llms/ctranslate2.py
+-rw-r--r--   0        0        0      101 2024-01-10 09:04:40.454645 gigachain-0.1.9/langchain/llms/databricks.py
+-rw-r--r--   0        0        0       98 2024-01-10 09:04:40.455573 gigachain-0.1.9/langchain/llms/deepinfra.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.397072 gigachain-0.1.9/langchain/llms/deepsparse.py
+-rw-r--r--   0        0        0       73 2023-12-18 12:05:47.397873 gigachain-0.1.9/langchain/llms/edenai.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:47.399013 gigachain-0.1.9/langchain/llms/fake.py
+-rw-r--r--   0        0        0       98 2024-01-10 09:04:40.456495 gigachain-0.1.9/langchain/llms/fireworks.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.400669 gigachain-0.1.9/langchain/llms/forefrontai.py
+-rw-r--r--   0        0        0       79 2024-01-10 09:04:40.457511 gigachain-0.1.9/langchain/llms/gigachat.py
+-rw-r--r--   0        0        0       86 2024-01-10 09:04:40.459648 gigachain-0.1.9/langchain/llms/google_palm.py
+-rw-r--r--   0        0        0       76 2023-12-18 12:05:47.403054 gigachain-0.1.9/langchain/llms/gooseai.py
+-rw-r--r--   0        0        0       76 2023-12-18 12:05:47.403988 gigachain-0.1.9/langchain/llms/gpt4all.py
+-rw-r--r--   0        0        0      116 2023-12-18 12:05:47.404853 gigachain-0.1.9/langchain/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2023-08-29 13:18:02.701979 gigachain-0.1.9/langchain/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2023-08-29 13:18:02.702167 gigachain-0.1.9/langchain/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0      122 2024-01-10 09:04:40.460567 gigachain-0.1.9/langchain/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0      107 2024-01-10 09:04:40.461738 gigachain-0.1.9/langchain/llms/huggingface_hub.py
+-rw-r--r--   0        0        0      129 2024-01-10 09:04:40.462973 gigachain-0.1.9/langchain/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0      148 2023-12-18 12:05:47.408597 gigachain-0.1.9/langchain/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0       95 2024-01-10 09:04:40.464144 gigachain-0.1.9/langchain/llms/human.py
+-rw-r--r--   0        0        0      123 2024-01-10 09:04:40.465399 gigachain-0.1.9/langchain/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0       87 2024-01-10 09:04:40.466206 gigachain-0.1.9/langchain/llms/koboldai.py
+-rw-r--r--   0        0        0       79 2023-12-18 12:05:47.413304 gigachain-0.1.9/langchain/llms/llamacpp.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.414682 gigachain-0.1.9/langchain/llms/loading.py
+-rw-r--r--   0        0        0       93 2023-12-18 12:05:47.415424 gigachain-0.1.9/langchain/llms/manifest.py
+-rw-r--r--   0        0        0       85 2024-01-10 09:04:40.467239 gigachain-0.1.9/langchain/llms/minimax.py
+-rw-r--r--   0        0        0       73 2024-01-10 09:04:40.468921 gigachain-0.1.9/langchain/llms/mlflow.py
+-rw-r--r--   0        0        0      102 2024-01-10 09:04:40.469899 gigachain-0.1.9/langchain/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0       70 2023-12-18 12:05:47.418198 gigachain-0.1.9/langchain/llms/modal.py
+-rw-r--r--   0        0        0       95 2024-01-10 09:04:40.470830 gigachain-0.1.9/langchain/llms/mosaicml.py
+-rw-r--r--   0        0        0       79 2023-12-18 12:05:47.419808 gigachain-0.1.9/langchain/llms/nlpcloud.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.420848 gigachain-0.1.9/langchain/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0       82 2024-01-10 09:04:40.471699 gigachain-0.1.9/langchain/llms/ollama.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.422749 gigachain-0.1.9/langchain/llms/opaqueprompts.py
+-rw-r--r--   0        0        0      193 2024-01-10 09:04:40.472465 gigachain-0.1.9/langchain/llms/openai.py
+-rw-r--r--   0        0        0       76 2024-01-10 09:04:40.473297 gigachain-0.1.9/langchain/llms/openllm.py
+-rw-r--r--   0        0        0       73 2023-12-18 12:05:47.425514 gigachain-0.1.9/langchain/llms/openlm.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:47.426494 gigachain-0.1.9/langchain/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0       73 2023-12-18 12:05:47.427233 gigachain-0.1.9/langchain/llms/petals.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.427965 gigachain-0.1.9/langchain/llms/pipelineai.py
+-rw-r--r--   0        0        0       82 2023-12-18 12:05:47.428665 gigachain-0.1.9/langchain/llms/predibase.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.429339 gigachain-0.1.9/langchain/llms/predictionguard.py
+-rw-r--r--   0        0        0      168 2023-12-18 12:05:47.430258 gigachain-0.1.9/langchain/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0       82 2023-12-18 12:05:47.431189 gigachain-0.1.9/langchain/llms/replicate.py
+-rw-r--r--   0        0        0       67 2023-12-18 12:05:47.431973 gigachain-0.1.9/langchain/llms/rwkv.py
+-rw-r--r--   0        0        0      160 2024-01-10 09:04:40.479050 gigachain-0.1.9/langchain/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.479967 gigachain-0.1.9/langchain/llms/self_hosted.py
+-rw-r--r--   0        0        0      143 2024-01-10 09:04:40.480961 gigachain-0.1.9/langchain/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.435028 gigachain-0.1.9/langchain/llms/stochasticai.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.481881 gigachain-0.1.9/langchain/llms/symblai_nebula.py
+-rw-r--r--   0        0        0       76 2023-12-18 12:05:47.436528 gigachain-0.1.9/langchain/llms/textgen.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.437384 gigachain-0.1.9/langchain/llms/titan_takeoff.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:47.438099 gigachain-0.1.9/langchain/llms/titan_takeoff_pro.py
+-rw-r--r--   0        0        0       79 2023-12-18 12:05:47.438940 gigachain-0.1.9/langchain/llms/together.py
+-rw-r--r--   0        0        0       89 2024-01-10 09:04:40.482832 gigachain-0.1.9/langchain/llms/tongyi.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.440079 gigachain-0.1.9/langchain/llms/utils.py
+-rw-r--r--   0        0        0      147 2024-01-10 09:04:40.483851 gigachain-0.1.9/langchain/llms/vertexai.py
+-rw-r--r--   0        0        0       93 2023-12-18 12:05:47.441569 gigachain-0.1.9/langchain/llms/vllm.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.441823 gigachain-0.1.9/langchain/llms/volcengine_maas.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.442050 gigachain-0.1.9/langchain/llms/watsonxllm.py
+-rw-r--r--   0        0        0       73 2023-12-18 12:05:47.442855 gigachain-0.1.9/langchain/llms/writer.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.443467 gigachain-0.1.9/langchain/llms/xinference.py
+-rw-r--r--   0        0        0       79 2024-01-10 09:04:40.484703 gigachain-0.1.9/langchain/llms/yandex.py
+-rw-r--r--   0        0        0      206 2023-12-18 12:05:47.445806 gigachain-0.1.9/langchain/load/__init__.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.446683 gigachain-0.1.9/langchain/load/dump.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.447484 gigachain-0.1.9/langchain/load/load.py
+-rw-r--r--   0        0        0      412 2023-12-18 12:05:47.448066 gigachain-0.1.9/langchain/load/serializable.py
+-rw-r--r--   0        0        0     3256 2024-01-18 15:16:40.735874 gigachain-0.1.9/langchain/memory/__init__.py
+-rw-r--r--   0        0        0     4861 2024-02-22 08:54:03.274556 gigachain-0.1.9/langchain/memory/buffer.py
+-rw-r--r--   0        0        0     1616 2024-03-01 11:50:11.631255 gigachain-0.1.9/langchain/memory/buffer_window.py
+-rw-r--r--   0        0        0     2245 2024-02-22 08:54:03.275441 gigachain-0.1.9/langchain/memory/chat_memory.py
+-rw-r--r--   0        0        0     1560 2024-02-22 08:54:03.277945 gigachain-0.1.9/langchain/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.485550 gigachain-0.1.9/langchain/memory/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0      145 2024-01-10 09:04:40.486385 gigachain-0.1.9/langchain/memory/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0      143 2023-12-18 12:05:47.453355 gigachain-0.1.9/langchain/memory/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0      142 2023-12-18 12:05:47.454333 gigachain-0.1.9/langchain/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0      157 2023-12-18 12:05:47.455260 gigachain-0.1.9/langchain/memory/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0      121 2023-12-18 12:05:47.456262 gigachain-0.1.9/langchain/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0      145 2024-01-10 09:04:40.487202 gigachain-0.1.9/langchain/memory/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      118 2023-12-18 12:05:47.458129 gigachain-0.1.9/langchain/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.488531 gigachain-0.1.9/langchain/memory/chat_message_histories/momento.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.489333 gigachain-0.1.9/langchain/memory/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.461292 gigachain-0.1.9/langchain/memory/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0      142 2024-01-10 09:04:40.490216 gigachain-0.1.9/langchain/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.469349 gigachain-0.1.9/langchain/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0      141 2023-12-18 12:05:47.470277 gigachain-0.1.9/langchain/memory/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0      157 2023-12-18 12:05:47.474949 gigachain-0.1.9/langchain/memory/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0      248 2024-01-10 09:04:40.492289 gigachain-0.1.9/langchain/memory/chat_message_histories/sql.py
+-rw-r--r--   0        0        0      145 2023-12-18 12:05:47.476873 gigachain-0.1.9/langchain/memory/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0      155 2023-12-18 12:05:47.477734 gigachain-0.1.9/langchain/memory/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0      121 2023-12-18 12:05:47.478747 gigachain-0.1.9/langchain/memory/chat_message_histories/xata.py
+-rw-r--r--   0        0        0      118 2023-12-18 12:05:47.479566 gigachain-0.1.9/langchain/memory/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     2912 2023-12-18 12:05:47.480430 gigachain-0.1.9/langchain/memory/combined.py
+-rw-r--r--   0        0        0    15677 2024-02-22 08:54:03.279615 gigachain-0.1.9/langchain/memory/entity.py
+-rw-r--r--   0        0        0     5075 2024-01-18 15:16:40.739203 gigachain-0.1.9/langchain/memory/kg.py
+-rw-r--r--   0        0        0     3106 2023-12-18 12:05:47.483008 gigachain-0.1.9/langchain/memory/motorhead_memory.py
+-rw-r--r--   0        0        0    13128 2023-12-18 12:05:47.483791 gigachain-0.1.9/langchain/memory/prompt.py
+-rw-r--r--   0        0        0      794 2023-12-18 12:05:47.484537 gigachain-0.1.9/langchain/memory/readonly.py
+-rw-r--r--   0        0        0      761 2023-12-18 12:05:47.485293 gigachain-0.1.9/langchain/memory/simple.py
+-rw-r--r--   0        0        0     3389 2023-12-18 12:05:47.485998 gigachain-0.1.9/langchain/memory/summary.py
+-rw-r--r--   0        0        0     2949 2023-12-18 12:05:47.486936 gigachain-0.1.9/langchain/memory/summary_buffer.py
+-rw-r--r--   0        0        0     2144 2023-12-18 12:05:47.487927 gigachain-0.1.9/langchain/memory/token_buffer.py
+-rw-r--r--   0        0        0      617 2023-08-29 13:18:02.706587 gigachain-0.1.9/langchain/memory/utils.py
+-rw-r--r--   0        0        0     3002 2023-12-18 12:05:47.489028 gigachain-0.1.9/langchain/memory/vectorstore.py
+-rw-r--r--   0        0        0     5090 2024-01-18 15:16:40.740045 gigachain-0.1.9/langchain/memory/zep_memory.py
+-rw-r--r--   0        0        0     3278 2024-02-22 08:54:03.280782 gigachain-0.1.9/langchain/model_laboratory.py
+-rw-r--r--   0        0        0     2216 2023-12-18 12:05:47.491014 gigachain-0.1.9/langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1433 2024-03-01 11:50:11.632242 gigachain-0.1.9/langchain/output_parsers/boolean.py
+-rw-r--r--   0        0        0     1799 2023-12-18 12:05:47.492673 gigachain-0.1.9/langchain/output_parsers/combining.py
+-rw-r--r--   0        0        0     1924 2024-02-22 08:54:03.283314 gigachain-0.1.9/langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1205 2023-12-18 12:05:47.494416 gigachain-0.1.9/langchain/output_parsers/enum.py
+-rw-r--r--   0        0        0      424 2024-02-22 08:54:03.284260 gigachain-0.1.9/langchain/output_parsers/ernie_functions.py
+-rw-r--r--   0        0        0     3153 2023-12-18 12:05:47.496827 gigachain-0.1.9/langchain/output_parsers/fix.py
+-rw-r--r--   0        0        0     3958 2024-01-18 15:16:40.741558 gigachain-0.1.9/langchain/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0      298 2024-01-10 09:04:40.495028 gigachain-0.1.9/langchain/output_parsers/json.py
+-rw-r--r--   0        0        0      310 2023-12-18 12:05:47.500021 gigachain-0.1.9/langchain/output_parsers/list.py
+-rw-r--r--   0        0        0      702 2023-08-21 13:51:28.860635 gigachain-0.1.9/langchain/output_parsers/loading.py
+-rw-r--r--   0        0        0      364 2024-03-01 11:50:11.633028 gigachain-0.1.9/langchain/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0      229 2024-03-01 11:50:11.633712 gigachain-0.1.9/langchain/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     6548 2024-02-22 08:54:03.288456 gigachain-0.1.9/langchain/output_parsers/pandas_dataframe.py
+-rw-r--r--   0        0        0      699 2023-12-18 12:05:47.503286 gigachain-0.1.9/langchain/output_parsers/prompts.py
+-rw-r--r--   0        0        0       99 2024-03-01 11:50:11.634691 gigachain-0.1.9/langchain/output_parsers/pydantic.py
+-rw-r--r--   0        0        0      129 2024-02-22 08:54:03.292714 gigachain-0.1.9/langchain/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0     1214 2023-12-18 12:05:47.506059 gigachain-0.1.9/langchain/output_parsers/regex.py
+-rw-r--r--   0        0        0     1709 2023-12-18 12:05:47.506885 gigachain-0.1.9/langchain/output_parsers/regex_dict.py
+-rw-r--r--   0        0        0     7792 2024-01-18 15:16:40.746608 gigachain-0.1.9/langchain/output_parsers/retry.py
+-rw-r--r--   0        0        0     3134 2024-02-22 08:54:03.293969 gigachain-0.1.9/langchain/output_parsers/structured.py
+-rw-r--r--   0        0        0       93 2024-01-10 09:04:40.496050 gigachain-0.1.9/langchain/output_parsers/xml.py
+-rw-r--r--   0        0        0     2181 2024-02-22 08:54:03.295025 gigachain-0.1.9/langchain/output_parsers/yaml.py
+-rw-r--r--   0        0        0     2560 2023-12-18 12:05:47.510676 gigachain-0.1.9/langchain/prompts/__init__.py
+-rw-r--r--   0        0        0      565 2023-12-18 12:05:47.511466 gigachain-0.1.9/langchain/prompts/base.py
+-rw-r--r--   0        0        0     1045 2023-12-18 12:05:47.512665 gigachain-0.1.9/langchain/prompts/chat.py
+-rw-r--r--   0        0        0      568 2023-12-18 12:05:47.513679 gigachain-0.1.9/langchain/prompts/example_selector/__init__.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.514537 gigachain-0.1.9/langchain/prompts/example_selector/base.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:47.515578 gigachain-0.1.9/langchain/prompts/example_selector/length_based.py
+-rw-r--r--   0        0        0      203 2024-02-22 08:54:03.296005 gigachain-0.1.9/langchain/prompts/example_selector/ngram_overlap.py
+-rw-r--r--   0        0        0      288 2023-12-18 12:05:47.517451 gigachain-0.1.9/langchain/prompts/example_selector/semantic_similarity.py
+-rw-r--r--   0        0        0      265 2023-12-18 12:05:47.518312 gigachain-0.1.9/langchain/prompts/few_shot.py
+-rw-r--r--   0        0        0      128 2023-12-18 12:05:47.519153 gigachain-0.1.9/langchain/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0      530 2023-12-18 12:05:47.519896 gigachain-0.1.9/langchain/prompts/loading.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.520643 gigachain-0.1.9/langchain/prompts/pipeline.py
+-rw-r--r--   0        0        0      153 2023-12-18 12:05:47.521708 gigachain-0.1.9/langchain/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.868214 gigachain-0.1.9/langchain/py.typed
+-rw-r--r--   0        0        0      897 2023-08-21 13:51:28.868582 gigachain-0.1.9/langchain/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2023-08-21 13:51:28.868846 gigachain-0.1.9/langchain/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2023-08-21 13:51:28.869090 gigachain-0.1.9/langchain/pydantic_v1/main.py
+-rw-r--r--   0        0        0      121 2024-01-18 15:16:40.748012 gigachain-0.1.9/langchain/python.py
+-rw-r--r--   0        0        0      222 2024-01-18 15:16:40.748946 gigachain-0.1.9/langchain/requests.py
+-rw-r--r--   0        0        0     3488 2024-02-22 08:54:03.298877 gigachain-0.1.9/langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.523253 gigachain-0.1.9/langchain/retrievers/arcee.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.524007 gigachain-0.1.9/langchain/retrievers/arxiv.py
+-rw-r--r--   0        0        0      150 2024-01-10 09:04:40.496942 gigachain-0.1.9/langchain/retrievers/azure_cognitive_search.py
+-rw-r--r--   0        0        0      221 2023-12-18 12:05:47.525596 gigachain-0.1.9/langchain/retrievers/bedrock.py
+-rw-r--r--   0        0        0      162 2023-12-18 12:05:47.526294 gigachain-0.1.9/langchain/retrievers/bm25.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.527002 gigachain-0.1.9/langchain/retrievers/chaindesk.py
+-rw-r--r--   0        0        0      138 2023-12-18 12:05:47.527627 gigachain-0.1.9/langchain/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0      126 2024-01-10 09:04:40.497936 gigachain-0.1.9/langchain/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2298 2024-02-22 08:54:03.299860 gigachain-0.1.9/langchain/retrievers/contextual_compression.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.530630 gigachain-0.1.9/langchain/retrievers/databerry.py
+-rw-r--r--   0        0        0      129 2023-12-18 12:05:47.531715 gigachain-0.1.9/langchain/retrievers/docarray.py
+-rw-r--r--   0        0        0      701 2024-02-22 08:54:03.300629 gigachain-0.1.9/langchain/retrievers/document_compressors/__init__.py
+-rw-r--r--   0        0        0     2938 2024-03-01 11:50:11.635714 gigachain-0.1.9/langchain/retrievers/document_compressors/base.py
+-rw-r--r--   0        0        0     3955 2024-02-22 08:54:03.301513 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract.py
+-rw-r--r--   0        0        0      621 2023-08-21 13:51:28.874260 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract_prompt.py
+-rw-r--r--   0        0        0     2757 2023-12-18 12:05:47.535586 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_filter.py
+-rw-r--r--   0        0        0      336 2023-09-04 15:41:37.267607 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_filter_prompt.py
+-rw-r--r--   0        0        0     4213 2024-02-22 08:54:03.302441 gigachain-0.1.9/langchain/retrievers/document_compressors/cohere_rerank.py
+-rw-r--r--   0        0        0     3031 2024-01-18 15:16:40.752303 gigachain-0.1.9/langchain/retrievers/document_compressors/embeddings_filter.py
+-rw-r--r--   0        0        0     2415 2024-02-22 08:54:03.302873 gigachain-0.1.9/langchain/retrievers/document_compressors/flashrank_rerank.py
+-rw-r--r--   0        0        0      141 2023-12-18 12:05:47.538561 gigachain-0.1.9/langchain/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.539048 gigachain-0.1.9/langchain/retrievers/embedchain.py
+-rw-r--r--   0        0        0     9668 2024-02-22 08:54:03.304010 gigachain-0.1.9/langchain/retrievers/ensemble.py
+-rw-r--r--   0        0        0      171 2023-12-18 12:05:47.540495 gigachain-0.1.9/langchain/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0      334 2024-01-10 09:04:40.499089 gigachain-0.1.9/langchain/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.542055 gigachain-0.1.9/langchain/retrievers/kay.py
+-rw-r--r--   0        0        0      803 2023-12-18 12:05:47.542775 gigachain-0.1.9/langchain/retrievers/kendra.py
+-rw-r--r--   0        0        0       88 2024-01-10 09:04:40.499990 gigachain-0.1.9/langchain/retrievers/knn.py
+-rw-r--r--   0        0        0      177 2023-12-18 12:05:47.544144 gigachain-0.1.9/langchain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     3489 2024-02-22 08:54:03.304848 gigachain-0.1.9/langchain/retrievers/merger_retriever.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.546337 gigachain-0.1.9/langchain/retrievers/metal.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.547245 gigachain-0.1.9/langchain/retrievers/milvus.py
+-rw-r--r--   0        0        0     7120 2024-02-22 08:54:03.308226 gigachain-0.1.9/langchain/retrievers/multi_query.py
+-rw-r--r--   0        0        0     3920 2024-02-22 08:54:03.309148 gigachain-0.1.9/langchain/retrievers/multi_vector.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.549986 gigachain-0.1.9/langchain/retrievers/outline.py
+-rw-r--r--   0        0        0     5196 2024-02-22 08:54:03.310174 gigachain-0.1.9/langchain/retrievers/parent_document_retriever.py
+-rw-r--r--   0        0        0      150 2024-01-10 09:04:40.501259 gigachain-0.1.9/langchain/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.552477 gigachain-0.1.9/langchain/retrievers/pubmed.py
+-rw-r--r--   0        0        0       94 2023-08-21 13:51:28.881470 gigachain-0.1.9/langchain/retrievers/pupmed.py
+-rw-r--r--   0        0        0     2930 2024-02-22 08:54:03.313542 gigachain-0.1.9/langchain/retrievers/re_phraser.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.554463 gigachain-0.1.9/langchain/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.882217 gigachain-0.1.9/langchain/retrievers/self_query/__init__.py
+-rw-r--r--   0        0        0     2194 2024-02-22 08:54:03.314677 gigachain-0.1.9/langchain/retrievers/self_query/astradb.py
+-rw-r--r--   0        0        0    10068 2024-03-01 11:50:11.636759 gigachain-0.1.9/langchain/retrievers/self_query/base.py
+-rw-r--r--   0        0        0     1474 2023-09-12 10:52:10.683073 gigachain-0.1.9/langchain/retrievers/self_query/chroma.py
+-rw-r--r--   0        0        0     1918 2024-01-18 15:16:40.762739 gigachain-0.1.9/langchain/retrievers/self_query/dashvector.py
+-rw-r--r--   0        0        0     2592 2023-09-04 05:57:22.522888 gigachain-0.1.9/langchain/retrievers/self_query/deeplake.py
+-rw-r--r--   0        0        0     3273 2024-02-22 08:54:03.317536 gigachain-0.1.9/langchain/retrievers/self_query/elasticsearch.py
+-rw-r--r--   0        0        0     3352 2024-02-22 08:54:03.318497 gigachain-0.1.9/langchain/retrievers/self_query/milvus.py
+-rw-r--r--   0        0        0     2303 2023-12-18 12:05:47.558690 gigachain-0.1.9/langchain/retrievers/self_query/mongodb_atlas.py
+-rw-r--r--   0        0        0     3636 2024-02-22 08:54:03.319483 gigachain-0.1.9/langchain/retrievers/self_query/myscale.py
+-rw-r--r--   0        0        0     3271 2024-02-22 08:54:03.320355 gigachain-0.1.9/langchain/retrievers/self_query/opensearch.py
+-rw-r--r--   0        0        0     1529 2024-02-22 08:54:03.320824 gigachain-0.1.9/langchain/retrievers/self_query/pgvector.py
+-rw-r--r--   0        0        0     1687 2023-10-06 14:43:01.539605 gigachain-0.1.9/langchain/retrievers/self_query/pinecone.py
+-rw-r--r--   0        0        0     3168 2024-02-22 08:54:03.321769 gigachain-0.1.9/langchain/retrievers/self_query/qdrant.py
+-rw-r--r--   0        0        0     3376 2024-01-18 15:16:40.763805 gigachain-0.1.9/langchain/retrievers/self_query/redis.py
+-rw-r--r--   0        0        0     2974 2023-09-12 10:52:10.683619 gigachain-0.1.9/langchain/retrievers/self_query/supabase.py
+-rw-r--r--   0        0        0     2633 2023-09-25 07:40:35.527447 gigachain-0.1.9/langchain/retrievers/self_query/timescalevector.py
+-rw-r--r--   0        0        0     2164 2023-10-19 12:57:53.001031 gigachain-0.1.9/langchain/retrievers/self_query/vectara.py
+-rw-r--r--   0        0        0     2619 2023-11-15 10:30:09.358178 gigachain-0.1.9/langchain/retrievers/self_query/weaviate.py
+-rw-r--r--   0        0        0       88 2024-01-10 09:04:40.503132 gigachain-0.1.9/langchain/retrievers/svm.py
+-rw-r--r--   0        0        0      167 2023-12-18 12:05:47.560135 gigachain-0.1.9/langchain/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.560807 gigachain-0.1.9/langchain/retrievers/tfidf.py
+-rw-r--r--   0        0        0     6279 2024-02-22 08:54:03.324848 gigachain-0.1.9/langchain/retrievers/time_weighted_retriever.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.564083 gigachain-0.1.9/langchain/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0      150 2023-12-18 12:05:47.566297 gigachain-0.1.9/langchain/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0     9014 2024-03-01 11:50:11.638549 gigachain-0.1.9/langchain/retrievers/web_research.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.567950 gigachain-0.1.9/langchain/retrievers/wikipedia.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.569099 gigachain-0.1.9/langchain/retrievers/you.py
+-rw-r--r--   0        0        0      142 2023-12-18 12:05:47.569898 gigachain-0.1.9/langchain/retrievers/zep.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.570757 gigachain-0.1.9/langchain/retrievers/zilliz.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.887732 gigachain-0.1.9/langchain/runnables/__init__.py
+-rw-r--r--   0        0        0      809 2023-12-18 12:05:47.571530 gigachain-0.1.9/langchain/runnables/hub.py
+-rw-r--r--   0        0        0     1525 2024-03-01 11:50:11.639231 gigachain-0.1.9/langchain/runnables/openai_functions.py
+-rw-r--r--   0        0        0     2065 2023-12-18 12:05:47.575459 gigachain-0.1.9/langchain/schema/__init__.py
+-rw-r--r--   0        0        0      149 2023-12-18 12:05:47.576297 gigachain-0.1.9/langchain/schema/agent.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.576979 gigachain-0.1.9/langchain/schema/cache.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:47.577169 gigachain-0.1.9/langchain/schema/callbacks/__init__.py
+-rw-r--r--   0        0        0      511 2023-12-18 12:05:47.577786 gigachain-0.1.9/langchain/schema/callbacks/base.py
+-rw-r--r--   0        0        0     1511 2023-12-18 12:05:47.578611 gigachain-0.1.9/langchain/schema/callbacks/manager.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.579043 gigachain-0.1.9/langchain/schema/callbacks/stdout.py
+-rw-r--r--   0        0        0      131 2023-12-18 12:05:47.579408 gigachain-0.1.9/langchain/schema/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:47.579637 gigachain-0.1.9/langchain/schema/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.580043 gigachain-0.1.9/langchain/schema/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      176 2023-12-18 12:05:47.580505 gigachain-0.1.9/langchain/schema/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      219 2023-12-18 12:05:47.580868 gigachain-0.1.9/langchain/schema/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:47.581282 gigachain-0.1.9/langchain/schema/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2023-12-18 12:05:47.581685 gigachain-0.1.9/langchain/schema/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.582039 gigachain-0.1.9/langchain/schema/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.582518 gigachain-0.1.9/langchain/schema/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2023-12-18 12:05:47.582779 gigachain-0.1.9/langchain/schema/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      257 2023-12-18 12:05:47.583106 gigachain-0.1.9/langchain/schema/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0       80 2023-12-18 12:05:47.583799 gigachain-0.1.9/langchain/schema/chat.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.584843 gigachain-0.1.9/langchain/schema/chat_history.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.585605 gigachain-0.1.9/langchain/schema/document.py
+-rw-r--r--   0        0        0       75 2023-12-18 12:05:47.586431 gigachain-0.1.9/langchain/schema/embeddings.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.587468 gigachain-0.1.9/langchain/schema/exceptions.py
+-rw-r--r--   0        0        0      367 2023-12-18 12:05:47.588176 gigachain-0.1.9/langchain/schema/language_model.py
+-rw-r--r--   0        0        0       71 2023-12-18 12:05:47.588957 gigachain-0.1.9/langchain/schema/memory.py
+-rw-r--r--   0        0        0     1048 2023-12-18 12:05:47.589743 gigachain-0.1.9/langchain/schema/messages.py
+-rw-r--r--   0        0        0      320 2023-12-18 12:05:47.590462 gigachain-0.1.9/langchain/schema/output.py
+-rw-r--r--   0        0        0      651 2023-12-18 12:05:47.591291 gigachain-0.1.9/langchain/schema/output_parser.py
+-rw-r--r--   0        0        0       80 2023-12-18 12:05:47.592095 gigachain-0.1.9/langchain/schema/prompt.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.592918 gigachain-0.1.9/langchain/schema/prompt_template.py
+-rw-r--r--   0        0        0       81 2023-12-18 12:05:47.593622 gigachain-0.1.9/langchain/schema/retriever.py
+-rw-r--r--   0        0        0     1796 2023-12-18 12:05:47.594714 gigachain-0.1.9/langchain/schema/runnable/__init__.py
+-rw-r--r--   0        0        0      781 2023-12-18 12:05:47.595763 gigachain-0.1.9/langchain/schema/runnable/base.py
+-rw-r--r--   0        0        0       89 2023-12-18 12:05:47.596655 gigachain-0.1.9/langchain/schema/runnable/branch.py
+-rw-r--r--   0        0        0      665 2023-12-18 12:05:47.597563 gigachain-0.1.9/langchain/schema/runnable/config.py
+-rw-r--r--   0        0        0      333 2023-12-18 12:05:47.598462 gigachain-0.1.9/langchain/schema/runnable/configurable.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.599358 gigachain-0.1.9/langchain/schema/runnable/fallbacks.py
+-rw-r--r--   0        0        0      260 2023-12-18 12:05:47.600021 gigachain-0.1.9/langchain/schema/runnable/history.py
+-rw-r--r--   0        0        0      205 2023-12-18 12:05:47.600672 gigachain-0.1.9/langchain/schema/runnable/passthrough.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.601412 gigachain-0.1.9/langchain/schema/runnable/retry.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.602442 gigachain-0.1.9/langchain/schema/runnable/router.py
+-rw-r--r--   0        0        0     1118 2023-12-18 12:05:47.603240 gigachain-0.1.9/langchain/schema/runnable/utils.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.604392 gigachain-0.1.9/langchain/schema/storage.py
+-rw-r--r--   0        0        0      137 2023-12-18 12:05:47.605680 gigachain-0.1.9/langchain/schema/vectorstore.py
+-rw-r--r--   0        0        0      130 2024-01-18 15:16:40.768493 gigachain-0.1.9/langchain/serpapi.py
+-rw-r--r--   0        0        0     3544 2024-01-18 15:16:40.769415 gigachain-0.1.9/langchain/smith/__init__.py
+-rw-r--r--   0        0        0     2199 2024-01-18 15:16:40.770441 gigachain-0.1.9/langchain/smith/evaluation/__init__.py
+-rw-r--r--   0        0        0    12480 2024-01-10 09:04:40.504756 gigachain-0.1.9/langchain/smith/evaluation/config.py
+-rw-r--r--   0        0        0     9936 2023-12-18 12:05:47.609341 gigachain-0.1.9/langchain/smith/evaluation/name_generation.py
+-rw-r--r--   0        0        0     3310 2024-03-01 11:50:11.639824 gigachain-0.1.9/langchain/smith/evaluation/progress.py
+-rw-r--r--   0        0        0    50978 2024-02-22 08:54:03.330642 gigachain-0.1.9/langchain/smith/evaluation/runner_utils.py
+-rw-r--r--   0        0        0    17107 2023-12-18 12:05:47.613221 gigachain-0.1.9/langchain/smith/evaluation/string_run_evaluator.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.895985 gigachain-0.1.9/langchain/smith/evaluation/utils.py
+-rw-r--r--   0        0        0      139 2024-01-18 15:16:40.773265 gigachain-0.1.9/langchain/sql_database.py
+-rw-r--r--   0        0        0     1571 2024-02-22 08:54:03.333134 gigachain-0.1.9/langchain/storage/__init__.py
+-rw-r--r--   0        0        0     2517 2023-12-18 12:05:47.615861 gigachain-0.1.9/langchain/storage/_lc_store.py
+-rw-r--r--   0        0        0     2970 2023-12-18 12:05:47.616837 gigachain-0.1.9/langchain/storage/encoder_backed.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.617809 gigachain-0.1.9/langchain/storage/exceptions.py
+-rw-r--r--   0        0        0     4307 2024-02-22 08:54:03.334261 gigachain-0.1.9/langchain/storage/file_system.py
+-rw-r--r--   0        0        0     4448 2024-02-22 08:54:03.335210 gigachain-0.1.9/langchain/storage/in_memory.py
+-rw-r--r--   0        0        0       83 2023-12-18 12:05:47.621280 gigachain-0.1.9/langchain/storage/redis.py
+-rw-r--r--   0        0        0      166 2024-01-10 09:04:40.510757 gigachain-0.1.9/langchain/storage/upstash_redis.py
+-rw-r--r--   0        0        0    55865 2024-02-22 08:54:03.336949 gigachain-0.1.9/langchain/text_splitter.py
+-rw-r--r--   0        0        0     5663 2024-01-18 15:16:40.776804 gigachain-0.1.9/langchain/tools/__init__.py
+-rw-r--r--   0        0        0      166 2023-12-18 12:05:47.625523 gigachain-0.1.9/langchain/tools/ainetwork/app.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.626232 gigachain-0.1.9/langchain/tools/ainetwork/base.py
+-rw-r--r--   0        0        0      119 2023-12-18 12:05:47.626998 gigachain-0.1.9/langchain/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0      116 2023-12-18 12:05:47.627720 gigachain-0.1.9/langchain/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0      130 2023-12-18 12:05:47.628416 gigachain-0.1.9/langchain/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0      121 2023-12-18 12:05:47.630133 gigachain-0.1.9/langchain/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      257 2024-01-18 15:16:40.778408 gigachain-0.1.9/langchain/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.630970 gigachain-0.1.9/langchain/tools/amadeus/base.py
+-rw-r--r--   0        0        0      180 2023-12-18 12:05:47.632104 gigachain-0.1.9/langchain/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0      170 2023-12-18 12:05:47.632931 gigachain-0.1.9/langchain/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0       25 2023-08-21 13:51:28.901095 gigachain-0.1.9/langchain/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0      118 2023-12-18 12:05:47.634560 gigachain-0.1.9/langchain/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      802 2024-01-18 15:16:40.780425 gigachain-0.1.9/langchain/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.636784 gigachain-0.1.9/langchain/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0      156 2023-12-18 12:05:47.638067 gigachain-0.1.9/langchain/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0      149 2023-12-18 12:05:47.638948 gigachain-0.1.9/langchain/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0      149 2023-12-18 12:05:47.639702 gigachain-0.1.9/langchain/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0      175 2023-12-18 12:05:47.640091 gigachain-0.1.9/langchain/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      332 2024-01-10 09:04:40.515503 gigachain-0.1.9/langchain/tools/base.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:53.049903 gigachain-0.1.9/langchain/tools/bearly/__init__.py
+-rw-r--r--   0        0        0      229 2024-01-10 09:04:40.518070 gigachain-0.1.9/langchain/tools/bearly/tool.py
+-rw-r--r--   0        0        0      170 2024-01-18 15:16:40.781740 gigachain-0.1.9/langchain/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0      138 2023-12-18 12:05:47.643848 gigachain-0.1.9/langchain/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.906784 gigachain-0.1.9/langchain/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0       95 2023-12-18 12:05:47.644621 gigachain-0.1.9/langchain/tools/brave_search/tool.py
+-rw-r--r--   0        0        0        0 2023-10-06 14:43:01.562867 gigachain-0.1.9/langchain/tools/clickup/__init__.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.646160 gigachain-0.1.9/langchain/tools/clickup/tool.py
+-rw-r--r--   0        0        0      157 2024-02-22 08:54:03.337885 gigachain-0.1.9/langchain/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      268 2024-01-18 15:16:40.785078 gigachain-0.1.9/langchain/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0      197 2023-12-18 12:05:47.647471 gigachain-0.1.9/langchain/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      147 2024-01-18 15:16:40.786394 gigachain-0.1.9/langchain/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0      269 2023-12-18 12:05:47.648366 gigachain-0.1.9/langchain/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2023-10-30 16:05:53.968119 gigachain-0.1.9/langchain/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0      240 2024-01-10 09:04:40.519149 gigachain-0.1.9/langchain/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0     1024 2024-01-18 15:16:40.788076 gigachain-0.1.9/langchain/tools/edenai/__init__.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:47.651357 gigachain-0.1.9/langchain/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:47.652284 gigachain-0.1.9/langchain/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:47.653108 gigachain-0.1.9/langchain/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0      139 2023-12-18 12:05:47.654289 gigachain-0.1.9/langchain/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0      143 2023-12-18 12:05:47.667832 gigachain-0.1.9/langchain/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0      119 2023-12-18 12:05:47.673367 gigachain-0.1.9/langchain/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0      128 2023-12-18 12:05:47.678230 gigachain-0.1.9/langchain/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0      126 2023-12-18 12:05:47.680238 gigachain-0.1.9/langchain/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      164 2024-01-18 15:16:40.789002 gigachain-0.1.9/langchain/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.681114 gigachain-0.1.9/langchain/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0      138 2024-01-10 09:04:40.520141 gigachain-0.1.9/langchain/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0      723 2024-01-18 15:16:40.790286 gigachain-0.1.9/langchain/tools/file_management/__init__.py
+-rw-r--r--   0        0        0      132 2023-12-18 12:05:47.683048 gigachain-0.1.9/langchain/tools/file_management/copy.py
+-rw-r--r--   0        0        0      155 2023-12-18 12:05:47.684055 gigachain-0.1.9/langchain/tools/file_management/delete.py
+-rw-r--r--   0        0        0      160 2023-12-18 12:05:47.684795 gigachain-0.1.9/langchain/tools/file_management/file_search.py
+-rw-r--r--   0        0        0      175 2023-12-18 12:05:47.685876 gigachain-0.1.9/langchain/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0      132 2023-12-18 12:05:47.687226 gigachain-0.1.9/langchain/tools/file_management/move.py
+-rw-r--r--   0        0        0      132 2023-12-18 12:05:47.688294 gigachain-0.1.9/langchain/tools/file_management/read.py
+-rw-r--r--   0        0        0      150 2023-12-18 12:05:47.690230 gigachain-0.1.9/langchain/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2023-08-21 13:51:28.913036 gigachain-0.1.9/langchain/tools/github/__init__.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.692510 gigachain-0.1.9/langchain/tools/github/tool.py
+-rw-r--r--   0        0        0       20 2023-09-19 14:33:02.316769 gigachain-0.1.9/langchain/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.694012 gigachain-0.1.9/langchain/tools/gitlab/tool.py
+-rw-r--r--   0        0        0      500 2024-01-18 15:16:40.791834 gigachain-0.1.9/langchain/tools/gmail/__init__.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.695102 gigachain-0.1.9/langchain/tools/gmail/base.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.696034 gigachain-0.1.9/langchain/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0      154 2023-12-18 12:05:47.696879 gigachain-0.1.9/langchain/tools/gmail/get_message.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:47.697691 gigachain-0.1.9/langchain/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0      167 2023-12-18 12:05:47.698533 gigachain-0.1.9/langchain/tools/gmail/search.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.699261 gigachain-0.1.9/langchain/tools/gmail/send_message.py
+-rw-r--r--   0        0        0      136 2024-01-18 15:16:40.794195 gigachain-0.1.9/langchain/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.701139 gigachain-0.1.9/langchain/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      171 2024-01-18 15:16:40.795771 gigachain-0.1.9/langchain/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0      151 2024-01-10 09:04:40.524958 gigachain-0.1.9/langchain/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      152 2024-01-18 15:16:40.798988 gigachain-0.1.9/langchain/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.703299 gigachain-0.1.9/langchain/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      140 2024-01-18 15:16:40.802247 gigachain-0.1.9/langchain/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.703936 gigachain-0.1.9/langchain/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      140 2024-01-18 15:16:40.804061 gigachain-0.1.9/langchain/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.704750 gigachain-0.1.9/langchain/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      140 2024-01-18 15:16:40.808715 gigachain-0.1.9/langchain/tools/google_places/__init__.py
+-rw-r--r--   0        0        0      161 2023-12-18 12:05:47.706017 gigachain-0.1.9/langchain/tools/google_places/tool.py
+-rw-r--r--   0        0        0      152 2024-01-18 15:16:40.810765 gigachain-0.1.9/langchain/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.707012 gigachain-0.1.9/langchain/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      195 2024-01-18 15:16:40.814439 gigachain-0.1.9/langchain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      161 2023-12-18 12:05:47.708241 gigachain-0.1.9/langchain/tools/google_search/tool.py
+-rw-r--r--   0        0        0      243 2024-01-18 15:16:40.816966 gigachain-0.1.9/langchain/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0      161 2023-12-18 12:05:47.709262 gigachain-0.1.9/langchain/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      148 2024-01-18 15:16:40.824180 gigachain-0.1.9/langchain/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:47.709982 gigachain-0.1.9/langchain/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2023-08-21 13:51:28.921484 gigachain-0.1.9/langchain/tools/graphql/__init__.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.710894 gigachain-0.1.9/langchain/tools/graphql/tool.py
+-rw-r--r--   0        0        0      132 2024-01-18 15:16:40.829390 gigachain-0.1.9/langchain/tools/human/__init__.py
+-rw-r--r--   0        0        0       92 2024-01-10 09:04:40.530860 gigachain-0.1.9/langchain/tools/human/tool.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.713440 gigachain-0.1.9/langchain/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2023-08-21 13:51:28.923495 gigachain-0.1.9/langchain/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.714893 gigachain-0.1.9/langchain/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2023-08-21 13:51:28.924161 gigachain-0.1.9/langchain/tools/jira/__init__.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.717607 gigachain-0.1.9/langchain/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2023-08-21 13:51:28.925352 gigachain-0.1.9/langchain/tools/json/__init__.py
+-rw-r--r--   0        0        0      174 2024-01-10 09:04:40.535392 gigachain-0.1.9/langchain/tools/json/tool.py
+-rw-r--r--   0        0        0      134 2024-01-18 15:16:40.836631 gigachain-0.1.9/langchain/tools/memorize/__init__.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.719498 gigachain-0.1.9/langchain/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2023-12-18 12:05:47.720059 gigachain-0.1.9/langchain/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.720682 gigachain-0.1.9/langchain/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      154 2024-01-18 15:16:40.840932 gigachain-0.1.9/langchain/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0      118 2023-12-18 12:05:47.721767 gigachain-0.1.9/langchain/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0      359 2024-01-18 15:16:40.842423 gigachain-0.1.9/langchain/tools/multion/__init__.py
+-rw-r--r--   0        0        0      170 2023-12-18 12:05:47.722885 gigachain-0.1.9/langchain/tools/multion/close_session.py
+-rw-r--r--   0        0        0      175 2023-12-18 12:05:47.723750 gigachain-0.1.9/langchain/tools/multion/create_session.py
+-rw-r--r--   0        0        0      175 2023-12-18 12:05:47.724545 gigachain-0.1.9/langchain/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:47.724833 gigachain-0.1.9/langchain/tools/nasa/__init__.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.725566 gigachain-0.1.9/langchain/tools/nasa/tool.py
+-rw-r--r--   0        0        0      111 2024-01-18 15:16:40.844691 gigachain-0.1.9/langchain/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0      135 2023-12-18 12:05:47.726427 gigachain-0.1.9/langchain/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      567 2024-01-18 15:16:40.847490 gigachain-0.1.9/langchain/tools/office365/__init__.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.727311 gigachain-0.1.9/langchain/tools/office365/base.py
+-rw-r--r--   0        0        0      197 2023-12-18 12:05:47.728682 gigachain-0.1.9/langchain/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0      164 2023-12-18 12:05:47.730216 gigachain-0.1.9/langchain/tools/office365/events_search.py
+-rw-r--r--   0        0        0      166 2023-12-18 12:05:47.731158 gigachain-0.1.9/langchain/tools/office365/messages_search.py
+-rw-r--r--   0        0        0      151 2023-12-18 12:05:47.732031 gigachain-0.1.9/langchain/tools/office365/send_event.py
+-rw-r--r--   0        0        0      161 2023-12-18 12:05:47.732938 gigachain-0.1.9/langchain/tools/office365/send_message.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933159 gigachain-0.1.9/langchain/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933535 gigachain-0.1.9/langchain/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0      542 2024-01-10 09:04:40.537910 gigachain-0.1.9/langchain/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      191 2024-01-18 15:16:40.849295 gigachain-0.1.9/langchain/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      162 2024-01-18 15:16:40.852577 gigachain-0.1.9/langchain/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      119 2023-12-18 12:05:47.735667 gigachain-0.1.9/langchain/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      763 2024-01-18 15:16:40.855894 gigachain-0.1.9/langchain/tools/playwright/__init__.py
+-rw-r--r--   0        0        0      110 2024-01-10 09:04:40.538998 gigachain-0.1.9/langchain/tools/playwright/base.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.737713 gigachain-0.1.9/langchain/tools/playwright/click.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.738636 gigachain-0.1.9/langchain/tools/playwright/current_page.py
+-rw-r--r--   0        0        0      198 2023-12-18 12:05:47.739546 gigachain-0.1.9/langchain/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.740370 gigachain-0.1.9/langchain/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0      168 2024-01-10 09:04:40.540758 gigachain-0.1.9/langchain/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0      152 2023-12-18 12:05:47.741776 gigachain-0.1.9/langchain/tools/playwright/navigate.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.742595 gigachain-0.1.9/langchain/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0      214 2024-01-10 09:04:40.541624 gigachain-0.1.9/langchain/tools/plugin.py
+-rw-r--r--   0        0        0       52 2023-08-21 13:51:28.940033 gigachain-0.1.9/langchain/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0      189 2023-12-18 12:05:47.747546 gigachain-0.1.9/langchain/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2023-08-21 13:51:28.941121 gigachain-0.1.9/langchain/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0       95 2023-12-18 12:05:47.748986 gigachain-0.1.9/langchain/tools/pubmed/tool.py
+-rw-r--r--   0        0        0      512 2023-12-18 12:05:47.750576 gigachain-0.1.9/langchain/tools/python/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 09:04:40.541802 gigachain-0.1.9/langchain/tools/reddit_search/__init__.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.750982 gigachain-0.1.9/langchain/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0     1581 2024-02-22 08:54:03.338610 gigachain-0.1.9/langchain/tools/render.py
+-rw-r--r--   0        0        0       52 2023-08-21 13:51:28.942395 gigachain-0.1.9/langchain/tools/requests/__init__.py
+-rw-r--r--   0        0        0      349 2024-01-10 09:04:40.543130 gigachain-0.1.9/langchain/tools/requests/tool.py
+-rw-r--r--   0        0        0     2494 2024-02-22 08:54:03.339522 gigachain-0.1.9/langchain/tools/retriever.py
+-rw-r--r--   0        0        0       31 2023-08-21 13:51:28.943010 gigachain-0.1.9/langchain/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0      140 2023-12-18 12:05:47.754166 gigachain-0.1.9/langchain/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      214 2024-01-18 15:16:40.857082 gigachain-0.1.9/langchain/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0      132 2023-12-18 12:05:47.754976 gigachain-0.1.9/langchain/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.943553 gigachain-0.1.9/langchain/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0      156 2023-12-18 12:05:47.756022 gigachain-0.1.9/langchain/tools/searx_search/tool.py
+-rw-r--r--   0        0        0      103 2024-01-18 15:16:40.858323 gigachain-0.1.9/langchain/tools/shell/__init__.py
+-rw-r--r--   0        0        0      123 2024-01-10 09:04:40.545873 gigachain-0.1.9/langchain/tools/shell/tool.py
+-rw-r--r--   0        0        0      433 2024-01-18 15:16:40.859291 gigachain-0.1.9/langchain/tools/slack/__init__.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.757949 gigachain-0.1.9/langchain/tools/slack/base.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.758288 gigachain-0.1.9/langchain/tools/slack/get_channel.py
+-rw-r--r--   0        0        0      164 2023-12-18 12:05:47.758614 gigachain-0.1.9/langchain/tools/slack/get_message.py
+-rw-r--r--   0        0        0      179 2023-12-18 12:05:47.758964 gigachain-0.1.9/langchain/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0      159 2023-12-18 12:05:47.759577 gigachain-0.1.9/langchain/tools/slack/send_message.py
+-rw-r--r--   0        0        0       18 2023-08-21 13:51:28.944873 gigachain-0.1.9/langchain/tools/sleep/__init__.py
+-rw-r--r--   0        0        0      110 2023-12-18 12:05:47.760887 gigachain-0.1.9/langchain/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2023-08-21 13:51:28.945531 gigachain-0.1.9/langchain/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      304 2023-12-18 12:05:47.762602 gigachain-0.1.9/langchain/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2023-08-21 13:51:28.946602 gigachain-0.1.9/langchain/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.763764 gigachain-0.1.9/langchain/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0      337 2023-12-18 12:05:47.764601 gigachain-0.1.9/langchain/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2023-12-18 12:05:47.764989 gigachain-0.1.9/langchain/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.765358 gigachain-0.1.9/langchain/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2023-12-18 12:05:47.765850 gigachain-0.1.9/langchain/tools/steam/__init__.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.766652 gigachain-0.1.9/langchain/tools/steam/tool.py
+-rw-r--r--   0        0        0      186 2024-01-18 15:16:40.861528 gigachain-0.1.9/langchain/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0      180 2024-01-10 09:04:40.549946 gigachain-0.1.9/langchain/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0      189 2024-01-18 15:16:40.863373 gigachain-0.1.9/langchain/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0      187 2023-12-18 12:05:47.769298 gigachain-0.1.9/langchain/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2023-08-21 13:51:28.948611 gigachain-0.1.9/langchain/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0      192 2024-01-10 09:04:40.550932 gigachain-0.1.9/langchain/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2023-08-21 13:51:28.949334 gigachain-0.1.9/langchain/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.770933 gigachain-0.1.9/langchain/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      156 2024-01-18 15:16:40.865406 gigachain-0.1.9/langchain/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:47.772046 gigachain-0.1.9/langchain/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:47.772808 gigachain-0.1.9/langchain/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.950523 gigachain-0.1.9/langchain/tools/youtube/__init__.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.773642 gigachain-0.1.9/langchain/tools/youtube/search.py
+-rw-r--r--   0        0        0      193 2024-01-18 15:16:40.866803 gigachain-0.1.9/langchain/tools/zapier/__init__.py
+-rw-r--r--   0        0        0      162 2023-12-18 12:05:47.775875 gigachain-0.1.9/langchain/tools/zapier/tool.py
+-rw-r--r--   0        0        0     2327 2024-02-22 08:54:03.342679 gigachain-0.1.9/langchain/utilities/__init__.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.777546 gigachain-0.1.9/langchain/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      193 2024-01-10 09:04:40.553326 gigachain-0.1.9/langchain/utilities/anthropic.py
+-rw-r--r--   0        0        0       89 2023-12-18 12:05:47.779550 gigachain-0.1.9/langchain/utilities/apify.py
+-rw-r--r--   0        0        0      361 2023-12-18 12:05:47.780643 gigachain-0.1.9/langchain/utilities/arcee.py
+-rw-r--r--   0        0        0       95 2023-12-18 12:05:47.781484 gigachain-0.1.9/langchain/utilities/arxiv.py
+-rw-r--r--   0        0        0      274 2023-08-21 13:51:28.954857 gigachain-0.1.9/langchain/utilities/asyncio.py
+-rw-r--r--   0        0        0       95 2023-12-18 12:05:47.782588 gigachain-0.1.9/langchain/utilities/awslambda.py
+-rw-r--r--   0        0        0      104 2024-01-10 09:04:40.554292 gigachain-0.1.9/langchain/utilities/bibtex.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.784354 gigachain-0.1.9/langchain/utilities/bing_search.py
+-rw-r--r--   0        0        0      108 2023-12-18 12:05:47.785090 gigachain-0.1.9/langchain/utilities/brave_search.py
+-rw-r--r--   0        0        0      269 2024-01-10 09:04:40.555397 gigachain-0.1.9/langchain/utilities/clickup.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.786400 gigachain-0.1.9/langchain/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0      121 2023-12-18 12:05:47.787554 gigachain-0.1.9/langchain/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0      129 2023-12-18 12:05:47.788355 gigachain-0.1.9/langchain/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0       98 2024-01-10 09:04:40.556303 gigachain-0.1.9/langchain/utilities/github.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.789907 gigachain-0.1.9/langchain/utilities/gitlab.py
+-rw-r--r--   0        0        0      123 2024-01-10 09:04:40.557288 gigachain-0.1.9/langchain/utilities/golden_query.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.790928 gigachain-0.1.9/langchain/utilities/google_finance.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.791487 gigachain-0.1.9/langchain/utilities/google_jobs.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.791854 gigachain-0.1.9/langchain/utilities/google_lens.py
+-rw-r--r--   0        0        0      121 2023-12-18 12:05:47.792836 gigachain-0.1.9/langchain/utilities/google_places_api.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.793660 gigachain-0.1.9/langchain/utilities/google_scholar.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.794263 gigachain-0.1.9/langchain/utilities/google_search.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.794850 gigachain-0.1.9/langchain/utilities/google_serper.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.795198 gigachain-0.1.9/langchain/utilities/google_trends.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.796297 gigachain-0.1.9/langchain/utilities/graphql.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.797166 gigachain-0.1.9/langchain/utilities/jira.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.798009 gigachain-0.1.9/langchain/utilities/loading.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.798917 gigachain-0.1.9/langchain/utilities/max_compute.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.558668 gigachain-0.1.9/langchain/utilities/merriam_webster.py
+-rw-r--r--   0        0        0      132 2024-01-10 09:04:40.559696 gigachain-0.1.9/langchain/utilities/metaphor_search.py
+-rw-r--r--   0        0        0      101 2024-01-10 09:04:40.560501 gigachain-0.1.9/langchain/utilities/nasa.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.801862 gigachain-0.1.9/langchain/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.803267 gigachain-0.1.9/langchain/utilities/openapi.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.804229 gigachain-0.1.9/langchain/utilities/openweathermap.py
+-rw-r--r--   0        0        0      110 2024-01-10 09:04:40.562773 gigachain-0.1.9/langchain/utilities/outline.py
+-rw-r--r--   0        0        0       81 2023-12-18 12:05:47.805758 gigachain-0.1.9/langchain/utilities/portkey.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.563881 gigachain-0.1.9/langchain/utilities/powerbi.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.807428 gigachain-0.1.9/langchain/utilities/pubmed.py
+-rw-r--r--   0        0        0       86 2024-01-10 09:04:40.566650 gigachain-0.1.9/langchain/utilities/python.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.808570 gigachain-0.1.9/langchain/utilities/reddit_search.py
+-rw-r--r--   0        0        0      201 2024-01-10 09:04:40.567678 gigachain-0.1.9/langchain/utilities/redis.py
+-rw-r--r--   0        0        0      181 2023-12-18 12:05:47.810729 gigachain-0.1.9/langchain/utilities/requests.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.811895 gigachain-0.1.9/langchain/utilities/scenexplain.py
+-rw-r--r--   0        0        0      107 2023-12-18 12:05:47.812573 gigachain-0.1.9/langchain/utilities/searchapi.py
+-rw-r--r--   0        0        0      151 2024-01-10 09:04:40.568799 gigachain-0.1.9/langchain/utilities/searx_search.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.814336 gigachain-0.1.9/langchain/utilities/serpapi.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.815076 gigachain-0.1.9/langchain/utilities/spark_sql.py
+-rw-r--r--   0        0        0      139 2024-01-10 09:04:40.570370 gigachain-0.1.9/langchain/utilities/sql_database.py
+-rw-r--r--   0        0        0      119 2023-12-18 12:05:47.816263 gigachain-0.1.9/langchain/utilities/stackexchange.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.816643 gigachain-0.1.9/langchain/utilities/steam.py
+-rw-r--r--   0        0        0      126 2024-01-10 09:04:40.571469 gigachain-0.1.9/langchain/utilities/tavily_search.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.818236 gigachain-0.1.9/langchain/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.819464 gigachain-0.1.9/langchain/utilities/twilio.py
+-rw-r--r--   0        0        0      276 2023-12-18 12:05:47.820326 gigachain-0.1.9/langchain/utilities/vertexai.py
+-rw-r--r--   0        0        0      116 2024-01-10 09:04:40.572515 gigachain-0.1.9/langchain/utilities/wikipedia.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.822016 gigachain-0.1.9/langchain/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.823234 gigachain-0.1.9/langchain/utilities/zapier.py
+-rw-r--r--   0        0        0     1221 2023-12-18 12:05:47.824245 gigachain-0.1.9/langchain/utils/__init__.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:47.825271 gigachain-0.1.9/langchain/utils/aiter.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.826109 gigachain-0.1.9/langchain/utils/env.py
+-rw-r--r--   0        0        0      325 2024-01-18 15:16:40.869253 gigachain-0.1.9/langchain/utils/ernie_functions.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.827383 gigachain-0.1.9/langchain/utils/formatting.py
+-rw-r--r--   0        0        0      421 2023-12-18 12:05:47.828299 gigachain-0.1.9/langchain/utils/html.py
+-rw-r--r--   0        0        0      211 2023-12-18 12:05:47.829085 gigachain-0.1.9/langchain/utils/input.py
+-rw-r--r--   0        0        0      139 2024-01-18 15:16:40.869655 gigachain-0.1.9/langchain/utils/interactive_env.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.829865 gigachain-0.1.9/langchain/utils/iter.py
+-rw-r--r--   0        0        0      258 2023-12-18 12:05:47.830615 gigachain-0.1.9/langchain/utils/json_schema.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.831372 gigachain-0.1.9/langchain/utils/loading.py
+-rw-r--r--   0        0        0      181 2023-12-18 12:05:47.832276 gigachain-0.1.9/langchain/utils/math.py
+-rw-r--r--   0        0        0       86 2023-12-18 12:05:47.833389 gigachain-0.1.9/langchain/utils/openai.py
+-rw-r--r--   0        0        0      330 2023-12-18 12:05:47.834161 gigachain-0.1.9/langchain/utils/openai_functions.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.835107 gigachain-0.1.9/langchain/utils/pydantic.py
+-rw-r--r--   0        0        0      148 2023-12-18 12:05:47.835836 gigachain-0.1.9/langchain/utils/strings.py
+-rw-r--r--   0        0        0      446 2023-12-18 12:05:47.836793 gigachain-0.1.9/langchain/utils/utils.py
+-rw-r--r--   0        0        0     2768 2024-02-22 08:54:03.345759 gigachain-0.1.9/langchain/vectorstores/__init__.py
+-rw-r--r--   0        0        0      220 2024-01-10 09:04:40.575258 gigachain-0.1.9/langchain/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0      109 2024-01-10 09:04:40.576760 gigachain-0.1.9/langchain/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0       87 2024-01-10 09:04:40.580566 gigachain-0.1.9/langchain/vectorstores/annoy.py
+-rw-r--r--   0        0        0      100 2024-01-10 09:04:40.583665 gigachain-0.1.9/langchain/vectorstores/astradb.py
+-rw-r--r--   0        0        0       82 2023-12-18 12:05:47.842405 gigachain-0.1.9/langchain/vectorstores/atlas.py
+-rw-r--r--   0        0        0       78 2024-01-10 09:04:40.584957 gigachain-0.1.9/langchain/vectorstores/awadb.py
+-rw-r--r--   0        0        0      256 2024-01-10 09:04:40.586040 gigachain-0.1.9/langchain/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0      188 2024-01-10 09:04:40.587676 gigachain-0.1.9/langchain/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0       89 2024-01-10 09:04:40.589288 gigachain-0.1.9/langchain/vectorstores/bageldb.py
+-rw-r--r--   0        0        0      115 2023-12-18 12:05:47.846640 gigachain-0.1.9/langchain/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.847689 gigachain-0.1.9/langchain/vectorstores/base.py
+-rw-r--r--   0        0        0      104 2023-12-18 12:05:47.848672 gigachain-0.1.9/langchain/vectorstores/cassandra.py
+-rw-r--r--   0        0        0       90 2024-01-10 09:04:40.590074 gigachain-0.1.9/langchain/vectorstores/chroma.py
+-rw-r--r--   0        0        0       87 2023-12-18 12:05:47.850266 gigachain-0.1.9/langchain/vectorstores/clarifai.py
+-rw-r--r--   0        0        0      148 2024-01-10 09:04:40.590843 gigachain-0.1.9/langchain/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0       93 2023-12-18 12:05:47.852012 gigachain-0.1.9/langchain/vectorstores/dashvector.py
+-rw-r--r--   0        0        0      140 2023-12-18 12:05:47.852481 gigachain-0.1.9/langchain/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0       87 2023-12-18 12:05:47.853219 gigachain-0.1.9/langchain/vectorstores/deeplake.py
+-rw-r--r--   0        0        0       78 2023-12-18 12:05:47.854024 gigachain-0.1.9/langchain/vectorstores/dingo.py
+-rw-r--r--   0        0        0      236 2024-01-18 15:16:40.872866 gigachain-0.1.9/langchain/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0      111 2024-01-10 09:04:40.591768 gigachain-0.1.9/langchain/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0      112 2023-12-18 12:05:47.859528 gigachain-0.1.9/langchain/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.860361 gigachain-0.1.9/langchain/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0      184 2024-01-10 09:04:40.593248 gigachain-0.1.9/langchain/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0      362 2023-12-18 12:05:47.862557 gigachain-0.1.9/langchain/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0       84 2023-12-18 12:05:47.863374 gigachain-0.1.9/langchain/vectorstores/epsilla.py
+-rw-r--r--   0        0        0       87 2024-01-10 09:04:40.594436 gigachain-0.1.9/langchain/vectorstores/faiss.py
+-rw-r--r--   0        0        0       78 2024-01-10 09:04:40.595403 gigachain-0.1.9/langchain/vectorstores/hippo.py
+-rw-r--r--   0        0        0       96 2024-01-10 09:04:40.596341 gigachain-0.1.9/langchain/vectorstores/hologres.py
+-rw-r--r--   0        0        0       84 2023-12-18 12:05:47.867322 gigachain-0.1.9/langchain/vectorstores/lancedb.py
+-rw-r--r--   0        0        0      128 2023-12-18 12:05:47.868167 gigachain-0.1.9/langchain/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0       78 2023-12-18 12:05:47.869093 gigachain-0.1.9/langchain/vectorstores/marqo.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.870058 gigachain-0.1.9/langchain/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0       96 2024-01-10 09:04:40.597226 gigachain-0.1.9/langchain/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0       81 2024-01-10 09:04:40.599173 gigachain-0.1.9/langchain/vectorstores/milvus.py
+-rw-r--r--   0        0        0      128 2024-01-10 09:04:40.600394 gigachain-0.1.9/langchain/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0      192 2024-01-10 09:04:40.601389 gigachain-0.1.9/langchain/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0      179 2024-01-10 09:04:40.602397 gigachain-0.1.9/langchain/vectorstores/myscale.py
+-rw-r--r--   0        0        0      147 2024-01-10 09:04:40.603441 gigachain-0.1.9/langchain/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0       87 2024-01-10 09:04:40.604618 gigachain-0.1.9/langchain/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0      147 2024-01-10 09:04:40.605556 gigachain-0.1.9/langchain/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0      234 2024-01-10 09:04:40.607685 gigachain-0.1.9/langchain/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0       93 2024-01-10 09:04:40.608761 gigachain-0.1.9/langchain/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0      149 2024-01-10 09:04:40.609389 gigachain-0.1.9/langchain/vectorstores/pgvector.py
+-rw-r--r--   0        0        0       87 2023-12-18 12:05:47.880186 gigachain-0.1.9/langchain/vectorstores/pinecone.py
+-rw-r--r--   0        0        0      130 2024-01-10 09:04:40.610308 gigachain-0.1.9/langchain/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      265 2023-09-12 10:52:10.695398 gigachain-0.1.9/langchain/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0      213 2024-01-10 09:04:40.611387 gigachain-0.1.9/langchain/vectorstores/redis/base.py
+-rw-r--r--   0        0        0      416 2023-12-18 12:05:47.884194 gigachain-0.1.9/langchain/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0      503 2023-12-18 12:05:47.885024 gigachain-0.1.9/langchain/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0       86 2023-12-18 12:05:47.885729 gigachain-0.1.9/langchain/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0       87 2024-01-10 09:04:40.612428 gigachain-0.1.9/langchain/vectorstores/scann.py
+-rw-r--r--   0        0        0       81 2023-12-18 12:05:47.887513 gigachain-0.1.9/langchain/vectorstores/semadb.py
+-rw-r--r--   0        0        0      165 2024-01-10 09:04:40.613481 gigachain-0.1.9/langchain/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0      364 2024-01-10 09:04:40.614368 gigachain-0.1.9/langchain/vectorstores/sklearn.py
+-rw-r--r--   0        0        0       90 2023-12-18 12:05:47.889663 gigachain-0.1.9/langchain/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0      154 2024-01-10 09:04:40.617741 gigachain-0.1.9/langchain/vectorstores/starrocks.py
+-rw-r--r--   0        0        0      109 2023-12-18 12:05:47.891235 gigachain-0.1.9/langchain/vectorstores/supabase.py
+-rw-r--r--   0        0        0       75 2024-01-10 09:04:40.620407 gigachain-0.1.9/langchain/vectorstores/tair.py
+-rw-r--r--   0        0        0      191 2023-12-18 12:05:47.893009 gigachain-0.1.9/langchain/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0       81 2023-12-18 12:05:47.893937 gigachain-0.1.9/langchain/vectorstores/tigris.py
+-rw-r--r--   0        0        0       97 2024-01-10 09:04:40.621429 gigachain-0.1.9/langchain/vectorstores/tiledb.py
+-rw-r--r--   0        0        0      124 2024-01-10 09:04:40.622500 gigachain-0.1.9/langchain/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0       90 2023-12-18 12:05:47.896743 gigachain-0.1.9/langchain/vectorstores/typesense.py
+-rw-r--r--   0        0        0       84 2024-01-10 09:04:40.623762 gigachain-0.1.9/langchain/vectorstores/usearch.py
+-rw-r--r--   0        0        0      227 2023-12-18 12:05:47.898744 gigachain-0.1.9/langchain/vectorstores/utils.py
+-rw-r--r--   0        0        0       75 2023-12-18 12:05:47.899754 gigachain-0.1.9/langchain/vectorstores/vald.py
+-rw-r--r--   0        0        0       81 2024-01-10 09:04:40.624717 gigachain-0.1.9/langchain/vectorstores/vearch.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.901403 gigachain-0.1.9/langchain/vectorstores/vectara.py
+-rw-r--r--   0        0        0       88 2023-12-18 12:05:47.902340 gigachain-0.1.9/langchain/vectorstores/vespa.py
+-rw-r--r--   0        0        0      103 2024-01-10 09:04:40.625644 gigachain-0.1.9/langchain/vectorstores/weaviate.py
+-rw-r--r--   0        0        0       97 2023-12-18 12:05:47.904061 gigachain-0.1.9/langchain/vectorstores/xata.py
+-rw-r--r--   0        0        0       96 2023-12-18 12:05:47.904403 gigachain-0.1.9/langchain/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0      132 2023-12-18 12:05:47.905433 gigachain-0.1.9/langchain/vectorstores/zep.py
+-rw-r--r--   0        0        0       81 2023-12-18 12:05:47.906395 gigachain-0.1.9/langchain/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    11751 2024-03-01 11:50:11.652206 gigachain-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 gigachain-0.1.9/PKG-INFO
```

### Comparing `gigachain-0.1.7.1/LICENSE` & `gigachain-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/README.md` & `gigachain-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/__init__.py` & `gigachain-0.1.9/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/_api/__init__.py` & `gigachain-0.1.9/langchain/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/adapters/openai.py` & `gigachain-0.1.9/langchain/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/__init__.py` & `gigachain-0.1.9/langchain/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent.py` & `gigachain-0.1.9/langchain/agents/agent.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_iterator.py` & `gigachain-0.1.9/langchain/agents/agent_iterator.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/__init__.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/csv/__init__.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/github/toolkit.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/planner.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/openapi/planner_prompt.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/pandas/__init__.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/python/__init__.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/python/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/spark/__init__.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/base.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/prompt.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/vectorstore/toolkit.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/toolkit.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_toolkits/xorbits/__init__.py` & `gigachain-0.1.9/langchain/agents/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/agent_types.py` & `gigachain-0.1.9/langchain/agents/agent_types.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/chat/base.py` & `gigachain-0.1.9/langchain/agents/chat/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/chat/output_parser.py` & `gigachain-0.1.9/langchain/agents/chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/chat/prompt.py` & `gigachain-0.1.9/langchain/agents/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/conversational/base.py` & `gigachain-0.1.9/langchain/agents/conversational/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/conversational/output_parser.py` & `gigachain-0.1.9/langchain/agents/conversational/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/conversational/prompt.py` & `gigachain-0.1.9/langchain/agents/conversational/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/conversational_chat/base.py` & `gigachain-0.1.9/langchain/agents/conversational_chat/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/conversational_chat/output_parser.py` & `gigachain-0.1.9/langchain/agents/conversational_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/conversational_chat/prompt.py` & `gigachain-0.1.9/langchain/agents/conversational_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/__init__.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/gigachat_functions.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/gigachat_tools.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_tools.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/log.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/log.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/log_to_messages.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/log_to_messages.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/openai_functions.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/openai_tools.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/openai_tools.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/format_scratchpad/xml.py` & `gigachain-0.1.9/langchain/agents/format_scratchpad/xml.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py` & `gigachain-0.1.9/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/gigachat_functions_agent/base.py` & `gigachain-0.1.9/langchain/agents/gigachat_functions_agent/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/gigachat_tools/base.py` & `gigachain-0.1.9/langchain/agents/gigachat_tools/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/initialize.py` & `gigachain-0.1.9/langchain/agents/initialize.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/json_chat/base.py` & `gigachain-0.1.9/langchain/agents/json_chat/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/json_chat/prompt.py` & `gigachain-0.1.9/langchain/agents/json_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/load_tools.py` & `gigachain-0.1.9/langchain/agents/load_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,18 @@
     "human": (_get_human_tool, ["prompt_func", "input_func"]),
     "awslambda": (
         _get_lambda_api,
         ["awslambda_tool_name", "awslambda_tool_description", "function_name"],
     ),
     "stackexchange": (_get_stackexchange, []),
     "sceneXplain": (_get_scenexplain, []),
-    "graphql": (_get_graphql_tool, ["graphql_endpoint", "custom_headers"]),
+    "graphql": (
+        _get_graphql_tool,
+        ["graphql_endpoint", "custom_headers", "fetch_schema_from_transport"],
+    ),
     "openweathermap-api": (_get_openweathermap, ["openweathermap_api_key"]),
     "dataforseo-api-search": (
         _get_dataforseo_api_search,
         ["api_login", "api_password", "aiosession"],
     ),
     "dataforseo-api-search-json": (
         _get_dataforseo_api_search_json,
```

### Comparing `gigachain-0.1.7.1/langchain/agents/loading.py` & `gigachain-0.1.9/langchain/agents/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/mrkl/base.py` & `gigachain-0.1.9/langchain/agents/mrkl/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/mrkl/output_parser.py` & `gigachain-0.1.9/langchain/agents/mrkl/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/mrkl/prompt.py` & `gigachain-0.1.9/langchain/agents/mrkl/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/openai_assistant/base.py` & `gigachain-0.1.9/langchain/agents/openai_assistant/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py` & `gigachain-0.1.9/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/openai_functions_agent/base.py` & `gigachain-0.1.9/langchain/agents/openai_functions_agent/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/openai_functions_multi_agent/base.py` & `gigachain-0.1.9/langchain/agents/openai_functions_multi_agent/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/openai_tools/base.py` & `gigachain-0.1.9/langchain/agents/openai_tools/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/__init__.py` & `gigachain-0.1.9/langchain/agents/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/gigachat_functions.py` & `gigachain-0.1.9/langchain/agents/output_parsers/gigachat_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/json.py` & `gigachain-0.1.9/langchain/agents/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/openai_functions.py` & `gigachain-0.1.9/langchain/agents/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/openai_tools.py` & `gigachain-0.1.9/langchain/agents/output_parsers/openai_tools.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/react_json_single_input.py` & `gigachain-0.1.9/langchain/agents/output_parsers/react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/react_single_input.py` & `gigachain-0.1.9/langchain/agents/output_parsers/react_single_input.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/self_ask.py` & `gigachain-0.1.9/langchain/agents/output_parsers/self_ask.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/output_parsers/xml.py` & `gigachain-0.1.9/langchain/agents/output_parsers/xml.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/react/agent.py` & `gigachain-0.1.9/langchain/agents/react/agent.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/react/base.py` & `gigachain-0.1.9/langchain/agents/react/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/react/output_parser.py` & `gigachain-0.1.9/langchain/agents/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/react/textworld_prompt.py` & `gigachain-0.1.9/langchain/agents/react/textworld_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/react/wiki_prompt.py` & `gigachain-0.1.9/langchain/agents/react/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/schema.py` & `gigachain-0.1.9/langchain/agents/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/self_ask_with_search/base.py` & `gigachain-0.1.9/langchain/agents/self_ask_with_search/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/self_ask_with_search/prompt.py` & `gigachain-0.1.9/langchain/agents/self_ask_with_search/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/structured_chat/base.py` & `gigachain-0.1.9/langchain/agents/structured_chat/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/structured_chat/output_parser.py` & `gigachain-0.1.9/langchain/agents/structured_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/structured_chat/prompt.py` & `gigachain-0.1.9/langchain/agents/structured_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/tools.py` & `gigachain-0.1.9/langchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/types.py` & `gigachain-0.1.9/langchain/agents/types.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/xml/base.py` & `gigachain-0.1.9/langchain/agents/xml/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/agents/xml/prompt.py` & `gigachain-0.1.9/langchain/agents/xml/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/cache.py` & `gigachain-0.1.9/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/__init__.py` & `gigachain-0.1.9/langchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/base.py` & `gigachain-0.1.9/langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/file.py` & `gigachain-0.1.9/langchain/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/manager.py` & `gigachain-0.1.9/langchain/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/streaming_aiter.py` & `gigachain-0.1.9/langchain/callbacks/streaming_aiter.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/streaming_aiter_final_only.py` & `gigachain-0.1.9/langchain/callbacks/streaming_aiter_final_only.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/streaming_stdout_final_only.py` & `gigachain-0.1.9/langchain/callbacks/streaming_stdout_final_only.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/streamlit/__init__.py` & `gigachain-0.1.9/langchain/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/tracers/__init__.py` & `gigachain-0.1.9/langchain/callbacks/tracers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/callbacks/tracers/logging.py` & `gigachain-0.1.9/langchain/callbacks/tracers/logging.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/__init__.py` & `gigachain-0.1.9/langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/base.py` & `gigachain-0.1.9/langchain/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/news_docs.py` & `gigachain-0.1.9/langchain/chains/api/news_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/open_meteo_docs.py` & `gigachain-0.1.9/langchain/chains/api/open_meteo_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/openapi/chain.py` & `gigachain-0.1.9/langchain/chains/api/openapi/chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/openapi/prompts.py` & `gigachain-0.1.9/langchain/chains/api/openapi/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/openapi/requests_chain.py` & `gigachain-0.1.9/langchain/chains/api/openapi/requests_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/openapi/response_chain.py` & `gigachain-0.1.9/langchain/chains/api/openapi/response_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/podcast_docs.py` & `gigachain-0.1.9/langchain/chains/api/podcast_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/prompt.py` & `gigachain-0.1.9/langchain/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/api/tmdb_docs.py` & `gigachain-0.1.9/langchain/chains/api/tmdb_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/base.py` & `gigachain-0.1.9/langchain/chains/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,22 @@
     CallbackManager,
     CallbackManagerForChainRun,
     Callbacks,
 )
 from langchain_core.load.dump import dumpd
 from langchain_core.memory import BaseMemory
 from langchain_core.outputs import RunInfo
-from langchain_core.pydantic_v1 import (
-    BaseModel,
-    Field,
-    create_model,
-    root_validator,
-    validator,
-)
+from langchain_core.pydantic_v1 import BaseModel, Field, root_validator, validator
 from langchain_core.runnables import (
     RunnableConfig,
     RunnableSerializable,
     ensure_config,
     run_in_executor,
 )
+from langchain_core.runnables.utils import create_model
 
 from langchain.schema import RUN_KEY
 
 logger = logging.getLogger(__name__)
 
 
 def _get_verbosity() -> bool:
@@ -460,15 +455,15 @@
             self.memory.save_context(inputs, outputs)
         if return_only_outputs:
             return outputs
         else:
             return {**inputs, **outputs}
 
     def prep_inputs(self, inputs: Union[Dict[str, Any], Any]) -> Dict[str, str]:
-        """Validate and prepare chain inputs, including adding inputs from memory.
+        """Prepare chain inputs, including adding inputs from memory.
 
         Args:
             inputs: Dictionary of raw inputs, or single input if chain expects
                 only one param. Should contain all inputs specified in
                 `Chain.input_keys` except for inputs that will be set by the chain's
                 memory.
```

### Comparing `gigachain-0.1.7.1/langchain/chains/chat_vector_db/prompts.py` & `gigachain-0.1.9/langchain/chains/chat_vector_db/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/base.py` & `gigachain-0.1.9/langchain/chains/combine_documents/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain_core.documents import Document
 from langchain_core.prompts import BasePromptTemplate, PromptTemplate
-from langchain_core.pydantic_v1 import BaseModel, Field, create_model
+from langchain_core.pydantic_v1 import BaseModel, Field
 from langchain_core.runnables.config import RunnableConfig
+from langchain_core.runnables.utils import create_model
 
 from langchain.chains.base import Chain
 from langchain.text_splitter import RecursiveCharacterTextSplitter, TextSplitter
 
 DEFAULT_DOCUMENT_SEPARATOR = "\n\n"
 DOCUMENTS_KEY = "context"
 DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template("{page_content}")
```

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/conditional.py` & `gigachain-0.1.9/langchain/chains/combine_documents/conditional.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/map_reduce.py` & `gigachain-0.1.9/langchain/chains/combine_documents/map_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Tuple, Type
 
 from langchain_core.callbacks import Callbacks
 from langchain_core.documents import Document
-from langchain_core.pydantic_v1 import BaseModel, Extra, create_model, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Extra, root_validator
 from langchain_core.runnables.config import RunnableConfig
+from langchain_core.runnables.utils import create_model
 
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.combine_documents.reduce import ReduceDocumentsChain
 from langchain.chains.llm import LLMChain
 
 
 class MapReduceDocumentsChain(BaseCombineDocumentsChain):
```

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/map_rerank.py` & `gigachain-0.1.9/langchain/chains/combine_documents/map_rerank.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union, cast
 
 from langchain_core.callbacks import Callbacks
 from langchain_core.documents import Document
-from langchain_core.pydantic_v1 import BaseModel, Extra, create_model, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Extra, root_validator
 from langchain_core.runnables.config import RunnableConfig
+from langchain_core.runnables.utils import create_model
 
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.llm import LLMChain
 from langchain.output_parsers.regex import RegexParser
 
 
 class MapRerankDocumentsChain(BaseCombineDocumentsChain):
```

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/reduce.py` & `gigachain-0.1.9/langchain/chains/combine_documents/reduce.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/refine.py` & `gigachain-0.1.9/langchain/chains/combine_documents/refine.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/combine_documents/stuff.py` & `gigachain-0.1.9/langchain/chains/combine_documents/stuff.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/constitutional_ai/base.py` & `gigachain-0.1.9/langchain/chains/constitutional_ai/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/constitutional_ai/principles.py` & `gigachain-0.1.9/langchain/chains/constitutional_ai/principles.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/constitutional_ai/prompts.py` & `gigachain-0.1.9/langchain/chains/constitutional_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/conversation/base.py` & `gigachain-0.1.9/langchain/chains/conversation/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/conversation/memory.py` & `gigachain-0.1.9/langchain/chains/conversation/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/conversation/prompt.py` & `gigachain-0.1.9/langchain/chains/conversation/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/conversational_retrieval/base.py` & `gigachain-0.1.9/langchain/chains/conversational_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/conversational_retrieval/prompts.py` & `gigachain-0.1.9/langchain/chains/conversational_retrieval/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/elasticsearch_database/base.py` & `gigachain-0.1.9/langchain/chains/elasticsearch_database/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/elasticsearch_database/prompts.py` & `gigachain-0.1.9/langchain/chains/elasticsearch_database/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/encoder.py` & `gigachain-0.1.9/langchain/chains/encoder.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/ernie_functions/base.py` & `gigachain-0.1.9/langchain/chains/ernie_functions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,39 +306,39 @@
 
     Returns:
         A runnable sequence that will pass the given function to the model when run.
 
     Example:
         .. code-block:: python
 
-                from typing import Optional
+            from typing import Optional
 
-                from langchain.chains.ernie_functions import create_structured_output_chain
-                from langchain_community.chat_models import ErnieBotChat
-                from langchain.prompts import ChatPromptTemplate
-                from langchain.pydantic_v1 import BaseModel, Field
-
-                class Dog(BaseModel):
-                    \"\"\"Identifying information about a dog.\"\"\"
-
-                    name: str = Field(..., description="The dog's name")
-                    color: str = Field(..., description="The dog's color")
-                    fav_food: Optional[str] = Field(None, description="The dog's favorite food")
-
-                llm = ErnieBotChat(model_name="ERNIE-Bot-4")
-                prompt = ChatPromptTemplate.from_messages(
-                    [
-                        ("user", "Use the given format to extract information from the following input: {input}"),
-                        ("assistant", "OK!"),
-                        ("user", "Tip: Make sure to answer in the correct format"),
-                    ]
-                )
-                chain = create_structured_output_chain(Dog, llm, prompt)
-                chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
-                # -> Dog(name="Harry", color="brown", fav_food="chicken")
+            from langchain.chains.ernie_functions import create_structured_output_chain
+            from langchain_community.chat_models import ErnieBotChat
+            from langchain.prompts import ChatPromptTemplate
+            from langchain.pydantic_v1 import BaseModel, Field
+
+            class Dog(BaseModel):
+                \"\"\"Identifying information about a dog.\"\"\"
+
+                name: str = Field(..., description="The dog's name")
+                color: str = Field(..., description="The dog's color")
+                fav_food: Optional[str] = Field(None, description="The dog's favorite food")
+
+            llm = ErnieBotChat(model_name="ERNIE-Bot-4")
+            prompt = ChatPromptTemplate.from_messages(
+                [
+                    ("user", "Use the given format to extract information from the following input: {input}"),
+                    ("assistant", "OK!"),
+                    ("user", "Tip: Make sure to answer in the correct format"),
+                ]
+            )
+            chain = create_structured_output_chain(Dog, llm, prompt)
+            chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
+            # -> Dog(name="Harry", color="brown", fav_food="chicken")
     """  # noqa: E501
     if isinstance(output_schema, dict):
         function: Any = {
             "name": "output_formatter",
             "description": (
                 "Output formatter. Should always be used to format your response to the"
                 " user."
```

### Comparing `gigachain-0.1.7.1/langchain/chains/example_generator.py` & `gigachain-0.1.9/langchain/chains/example_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/flare/base.py` & `gigachain-0.1.9/langchain/chains/flare/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/flare/prompts.py` & `gigachain-0.1.9/langchain/chains/flare/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/arangodb.py` & `gigachain-0.1.9/langchain/chains/graph_qa/arangodb.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/base.py` & `gigachain-0.1.9/langchain/chains/graph_qa/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/cypher.py` & `gigachain-0.1.9/langchain/chains/graph_qa/cypher.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/cypher_utils.py` & `gigachain-0.1.9/langchain/chains/graph_qa/cypher_utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/falkordb.py` & `gigachain-0.1.9/langchain/chains/graph_qa/falkordb.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/hugegraph.py` & `gigachain-0.1.9/langchain/chains/graph_qa/hugegraph.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/kuzu.py` & `gigachain-0.1.9/langchain/chains/graph_qa/kuzu.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/nebulagraph.py` & `gigachain-0.1.9/langchain/chains/graph_qa/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/neptune_cypher.py` & `gigachain-0.1.9/langchain/chains/graph_qa/neptune_cypher.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/neptune_sparql.py` & `gigachain-0.1.9/langchain/chains/graph_qa/neptune_sparql.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/ontotext_graphdb.py` & `gigachain-0.1.9/langchain/chains/graph_qa/ontotext_graphdb.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/prompts.py` & `gigachain-0.1.9/langchain/chains/graph_qa/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/graph_qa/sparql.py` & `gigachain-0.1.9/langchain/chains/graph_qa/sparql.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,23 +37,33 @@
     """
 
     graph: RdfGraph = Field(exclude=True)
     sparql_generation_select_chain: LLMChain
     sparql_generation_update_chain: LLMChain
     sparql_intent_chain: LLMChain
     qa_chain: LLMChain
+    return_sparql_query: bool = False
     input_key: str = "query"  #: :meta private:
     output_key: str = "result"  #: :meta private:
+    sparql_query_key: str = "sparql_query"  #: :meta private:
 
     @property
     def input_keys(self) -> List[str]:
+        """Return the input keys.
+
+        :meta private:
+        """
         return [self.input_key]
 
     @property
     def output_keys(self) -> List[str]:
+        """Return the output keys.
+
+        :meta private:
+        """
         _output_keys = [self.output_key]
         return _output_keys
 
     @classmethod
     def from_llm(
         cls,
         llm: BaseLanguageModel,
@@ -131,8 +141,12 @@
             )
             res = result[self.qa_chain.output_key]
         elif intent == "UPDATE":
             self.graph.update(generated_sparql)
             res = "Successfully inserted triples into the graph."
         else:
             raise ValueError("Unsupported SPARQL query type.")
-        return {self.output_key: res}
+
+        chain_result: Dict[str, Any] = {self.output_key: res}
+        if self.return_sparql_query:
+            chain_result[self.sparql_query_key] = generated_sparql
+        return chain_result
```

### Comparing `gigachain-0.1.7.1/langchain/chains/history_aware_retriever.py` & `gigachain-0.1.9/langchain/chains/history_aware_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/hyde/base.py` & `gigachain-0.1.9/langchain/chains/hyde/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/hyde/prompts.py` & `gigachain-0.1.9/langchain/chains/hyde/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm.py` & `gigachain-0.1.9/langchain/chains/llm.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_checker/base.py` & `gigachain-0.1.9/langchain/chains/llm_checker/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_checker/prompt.py` & `gigachain-0.1.9/langchain/chains/llm_checker/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_math/base.py` & `gigachain-0.1.9/langchain/chains/llm_math/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_math/prompt.py` & `gigachain-0.1.9/langchain/chains/llm_math/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_requests.py` & `gigachain-0.1.9/langchain/chains/llm_requests.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/base.py` & `gigachain-0.1.9/langchain/chains/llm_summarization_checker/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt` & `gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/check_facts.txt` & `gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/check_facts.txt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt` & `gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/loading.py` & `gigachain-0.1.9/langchain/chains/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/mapreduce.py` & `gigachain-0.1.9/langchain/chains/mapreduce.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/moderation.py` & `gigachain-0.1.9/langchain/chains/moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/natbot/base.py` & `gigachain-0.1.9/langchain/chains/natbot/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/natbot/crawler.py` & `gigachain-0.1.9/langchain/chains/natbot/crawler.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/natbot/prompt.py` & `gigachain-0.1.9/langchain/chains/natbot/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/__init__.py` & `gigachain-0.1.9/langchain/chains/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/base.py` & `gigachain-0.1.9/langchain/chains/openai_functions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 )
 
 from langchain_core._api import deprecated
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import (
     BaseLLMOutputParser,
 )
+from langchain_core.output_parsers.openai_functions import (
+    PydanticAttrOutputFunctionsParser,
+)
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.utils.function_calling import (
     PYTHON_TO_JSON_TYPES,
     convert_to_openai_function,
 )
 
 from langchain.chains import LLMChain
 from langchain.chains.structured_output.base import (
     create_openai_fn_runnable,
     create_structured_output_runnable,
     get_openai_output_parser,
 )
-from langchain.output_parsers.openai_functions import (
-    PydanticAttrOutputFunctionsParser,
-)
 
 __all__ = [
     "get_openai_output_parser",
     "create_openai_fn_runnable",
     "create_structured_output_runnable",
     "create_openai_fn_chain",  # deprecated
     "create_structured_output_chain",  # deprecated
```

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/citation_fuzzy_match.py` & `gigachain-0.1.9/langchain/chains/openai_functions/citation_fuzzy_match.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Iterator, List
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import HumanMessage, SystemMessage
+from langchain_core.output_parsers.openai_functions import PydanticOutputFunctionsParser
 from langchain_core.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel, Field
 
 from langchain.chains.llm import LLMChain
 from langchain.chains.openai_functions.utils import get_llm_kwargs
-from langchain.output_parsers.openai_functions import (
-    PydanticOutputFunctionsParser,
-)
 
 
 class FactWithEvidence(BaseModel):
     """Class representing a single statement.
 
     Each fact has a body and a list of sources.
     If there are multiple facts make sure to break them apart
```

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/extraction.py` & `gigachain-0.1.9/langchain/chains/openai_functions/tagging.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,90 @@
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 from langchain_core.language_models import BaseLanguageModel
-from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
-from langchain_core.pydantic_v1 import BaseModel
+from langchain_core.output_parsers.openai_functions import (
+    JsonOutputFunctionsParser,
+    PydanticOutputFunctionsParser,
+)
+from langchain_core.prompts import ChatPromptTemplate
 
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.chains.openai_functions.utils import (
-    _convert_schema,
-    _resolve_schema_references,
-    get_llm_kwargs,
-)
-from langchain.output_parsers.openai_functions import (
-    JsonKeyOutputFunctionsParser,
-    PydanticAttrOutputFunctionsParser,
-)
+from langchain.chains.openai_functions.utils import _convert_schema, get_llm_kwargs
 
 
-def _get_extraction_function(entity_schema: dict) -> dict:
+def _get_tagging_function(schema: dict) -> dict:
     return {
         "name": "information_extraction",
         "description": "Extracts the relevant information from the passage.",
-        "parameters": {
-            "type": "object",
-            "properties": {
-                "info": {"type": "array", "items": _convert_schema(entity_schema)}
-            },
-            "required": ["info"],
-        },
+        "parameters": _convert_schema(schema),
     }
 
 
-_EXTRACTION_TEMPLATE = """Extract and save the relevant entities mentioned \
-in the following passage together with their properties.
+_TAGGING_TEMPLATE = """Extract the desired information from the following passage.
 
 Only extract the properties mentioned in the 'information_extraction' function.
 
-If a property is not present and is not required in the function parameters, do not include it in the output.
-
 Passage:
 {input}
-"""  # noqa: E501
+"""
 
 
-def create_extraction_chain(
+def create_tagging_chain(
     schema: dict,
     llm: BaseLanguageModel,
-    prompt: Optional[BasePromptTemplate] = None,
-    tags: Optional[List[str]] = None,
-    verbose: bool = False,
+    prompt: Optional[ChatPromptTemplate] = None,
+    **kwargs: Any,
 ) -> Chain:
-    """Creates a chain that extracts information from a passage.
+    """Creates a chain that extracts information from a passage
+     based on a schema.
 
     Args:
         schema: The schema of the entities to extract.
         llm: The language model to use.
-        prompt: The prompt to use for extraction.
-        verbose: Whether to run in verbose mode. In verbose mode, some intermediate
-            logs will be printed to the console. Defaults to the global `verbose` value,
-            accessible via `langchain.globals.get_verbose()`.
 
     Returns:
-        Chain that can be used to extract information from a passage.
+        Chain (LLMChain) that can be used to extract information from a passage.
     """
-    function = _get_extraction_function(schema)
-    extraction_prompt = prompt or ChatPromptTemplate.from_template(_EXTRACTION_TEMPLATE)
-    output_parser = JsonKeyOutputFunctionsParser(key_name="info")
+    function = _get_tagging_function(schema)
+    prompt = prompt or ChatPromptTemplate.from_template(_TAGGING_TEMPLATE)
+    output_parser = JsonOutputFunctionsParser()
     llm_kwargs = get_llm_kwargs(function)
     chain = LLMChain(
         llm=llm,
-        prompt=extraction_prompt,
+        prompt=prompt,
         llm_kwargs=llm_kwargs,
         output_parser=output_parser,
-        tags=tags,
-        verbose=verbose,
+        **kwargs,
     )
     return chain
 
 
-def create_extraction_chain_pydantic(
+def create_tagging_chain_pydantic(
     pydantic_schema: Any,
     llm: BaseLanguageModel,
-    prompt: Optional[BasePromptTemplate] = None,
-    verbose: bool = False,
+    prompt: Optional[ChatPromptTemplate] = None,
+    **kwargs: Any,
 ) -> Chain:
-    """Creates a chain that extracts information from a passage using pydantic schema.
+    """Creates a chain that extracts information from a passage
+     based on a pydantic schema.
 
     Args:
         pydantic_schema: The pydantic schema of the entities to extract.
         llm: The language model to use.
-        prompt: The prompt to use for extraction.
-        verbose: Whether to run in verbose mode. In verbose mode, some intermediate
-            logs will be printed to the console. Defaults to the global `verbose` value,
-            accessible via `langchain.globals.get_verbose()`
 
     Returns:
-        Chain that can be used to extract information from a passage.
+        Chain (LLMChain) that can be used to extract information from a passage.
     """
-
-    class PydanticSchema(BaseModel):
-        info: List[pydantic_schema]  # type: ignore
-
     openai_schema = pydantic_schema.schema()
-    openai_schema = _resolve_schema_references(
-        openai_schema, openai_schema.get("definitions", {})
-    )
-
-    function = _get_extraction_function(openai_schema)
-    extraction_prompt = prompt or ChatPromptTemplate.from_template(_EXTRACTION_TEMPLATE)
-    output_parser = PydanticAttrOutputFunctionsParser(
-        pydantic_schema=PydanticSchema, attr_name="info"
-    )
+    function = _get_tagging_function(openai_schema)
+    prompt = prompt or ChatPromptTemplate.from_template(_TAGGING_TEMPLATE)
+    output_parser = PydanticOutputFunctionsParser(pydantic_schema=pydantic_schema)
     llm_kwargs = get_llm_kwargs(function)
     chain = LLMChain(
         llm=llm,
-        prompt=extraction_prompt,
+        prompt=prompt,
         llm_kwargs=llm_kwargs,
         output_parser=output_parser,
-        verbose=verbose,
+        **kwargs,
     )
     return chain
```

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/openapi.py` & `gigachain-0.1.9/langchain/chains/openai_functions/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 from langchain_community.chat_models import ChatOpenAI
 from langchain_community.utilities.openapi import OpenAPISpec
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
+from langchain_core.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
 from langchain_core.utils.input import get_colored_text
 from requests import Response
 
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.chains.sequential import SequentialChain
-from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain.tools import APIOperation
 
 if TYPE_CHECKING:
     from openapi_pydantic import Parameter
 
 
 def _get_description(o: Any, prefer_short: bool) -> Optional[str]:
```

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/qa_with_structure.py` & `gigachain-0.1.9/langchain/chains/openai_functions/qa_with_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, List, Optional, Type, Union
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import HumanMessage, SystemMessage
 from langchain_core.output_parsers import BaseLLMOutputParser
+from langchain_core.output_parsers.openai_functions import (
+    OutputFunctionsParser,
+    PydanticOutputFunctionsParser,
+)
 from langchain_core.prompts import PromptTemplate
 from langchain_core.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel, Field
 
 from langchain.chains.llm import LLMChain
 from langchain.chains.openai_functions.utils import get_llm_kwargs
-from langchain.output_parsers.openai_functions import (
-    OutputFunctionsParser,
-    PydanticOutputFunctionsParser,
-)
 
 
 class AnswerWithSources(BaseModel):
     """An answer to the question, with sources."""
 
     answer: str = Field(..., description="Answer to the question that was asked")
     sources: List[str] = Field(
```

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_functions/utils.py` & `gigachain-0.1.9/langchain/chains/openai_functions/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/openai_tools/extraction.py` & `gigachain-0.1.9/langchain/chains/openai_tools/extraction.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/prompt_selector.py` & `gigachain-0.1.9/langchain/chains/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_generation/base.py` & `gigachain-0.1.9/langchain/chains/qa_generation/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_generation/prompt.py` & `gigachain-0.1.9/langchain/chains/qa_generation/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/base.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/loading.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/map_reduce_prompt.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/refine_prompts.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/retrieval.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/retrieval.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/stuff_prompt.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/qa_with_sources/vector_db.py` & `gigachain-0.1.9/langchain/chains/qa_with_sources/vector_db.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/query_constructor/base.py` & `gigachain-0.1.9/langchain/chains/query_constructor/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/query_constructor/ir.py` & `gigachain-0.1.9/langchain/chains/query_constructor/ir.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/query_constructor/parser.py` & `gigachain-0.1.9/langchain/chains/query_constructor/parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/query_constructor/prompt.py` & `gigachain-0.1.9/langchain/chains/query_constructor/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/question_answering/__init__.py` & `gigachain-0.1.9/langchain/chains/question_answering/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/question_answering/map_reduce_prompt.py` & `gigachain-0.1.9/langchain/chains/question_answering/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/question_answering/map_rerank_prompt.py` & `gigachain-0.1.9/langchain/chains/question_answering/map_rerank_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/question_answering/refine_prompts.py` & `gigachain-0.1.9/langchain/chains/question_answering/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/question_answering/stuff_prompt.py` & `gigachain-0.1.9/langchain/chains/question_answering/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/retrieval.py` & `gigachain-0.1.9/langchain/chains/retrieval.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/retrieval_qa/base.py` & `gigachain-0.1.9/langchain/chains/retrieval_qa/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/retrieval_qa/prompt.py` & `gigachain-0.1.9/langchain/chains/retrieval_qa/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/base.py` & `gigachain-0.1.9/langchain/chains/router/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/embedding_router.py` & `gigachain-0.1.9/langchain/chains/router/embedding_router.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/llm_router.py` & `gigachain-0.1.9/langchain/chains/router/llm_router.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/multi_prompt.py` & `gigachain-0.1.9/langchain/chains/router/multi_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/multi_prompt_prompt.py` & `gigachain-0.1.9/langchain/chains/router/multi_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/multi_retrieval_prompt.py` & `gigachain-0.1.9/langchain/chains/router/multi_retrieval_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/router/multi_retrieval_qa.py` & `gigachain-0.1.9/langchain/chains/router/multi_retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/sequential.py` & `gigachain-0.1.9/langchain/chains/sequential.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/sql_database/prompt.py` & `gigachain-0.1.9/langchain/chains/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/sql_database/query.py` & `gigachain-0.1.9/langchain/chains/sql_database/query.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/structured_output/base.py` & `gigachain-0.1.9/langchain/chains/structured_output/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,35 +2,42 @@
 from typing import Any, Callable, Dict, Literal, Optional, Sequence, Type, Union
 
 from langchain_core.output_parsers import (
     BaseGenerationOutputParser,
     BaseOutputParser,
     JsonOutputParser,
 )
+from langchain_core.output_parsers.openai_functions import (
+    JsonOutputFunctionsParser,
+    PydanticAttrOutputFunctionsParser,
+    PydanticOutputFunctionsParser,
+)
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable
-from langchain_core.utils.function_calling import convert_to_openai_function
+from langchain_core.utils.function_calling import (
+    convert_to_openai_function,
+    convert_to_openai_tool,
+)
 
-from langchain.output_parsers import PydanticOutputParser
-from langchain.output_parsers.openai_functions import (
-    JsonOutputFunctionsParser,
-    PydanticAttrOutputFunctionsParser,
-    PydanticOutputFunctionsParser,
+from langchain.output_parsers import (
+    JsonOutputKeyToolsParser,
+    PydanticOutputParser,
+    PydanticToolsParser,
 )
 
 
 def create_openai_fn_runnable(
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     enforce_single_function_usage: bool = True,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
-    **kwargs: Any,
+    **llm_kwargs: Any,
 ) -> Runnable:
     """Create a runnable sequence that uses OpenAI functions.
 
     Args:
         functions: A sequence of either dictionaries, pydantic.BaseModels classes, or
             Python functions. If dictionaries are passed in, they are assumed to
             already be a valid OpenAI functions. If only a single
@@ -49,14 +56,15 @@
         output_parser: BaseLLMOutputParser to use for parsing model outputs. By default
             will be inferred from the function types. If pydantic.BaseModels are passed
             in, then the OutputParser will try to parse outputs using those. Otherwise
             model outputs will simply be parsed as JSON. If multiple functions are
             passed in and they are not pydantic.BaseModels, the chain output will
             include both the name of the function that was returned and the arguments
             to pass to the function.
+        **llm_kwargs: Additional named arguments to pass to the language model.
 
     Returns:
         A runnable sequence that will pass in the given functions to the model when run.
 
     Example:
         .. code-block:: python
 
@@ -87,33 +95,35 @@
                 structured_llm = create_openai_fn_runnable([RecordPerson, RecordDog], llm)
                 structured_llm.invoke("Harry was a chubby brown beagle who loved chicken)
                 # -> RecordDog(name="Harry", color="brown", fav_food="chicken")
     """  # noqa: E501
     if not functions:
         raise ValueError("Need to pass in at least one function. Received zero.")
     openai_functions = [convert_to_openai_function(f) for f in functions]
-    llm_kwargs: Dict[str, Any] = {"functions": openai_functions, **kwargs}
+    llm_kwargs_: Dict[str, Any] = {"functions": openai_functions, **llm_kwargs}
     if len(openai_functions) == 1 and enforce_single_function_usage:
-        llm_kwargs["function_call"] = {"name": openai_functions[0]["name"]}
+        llm_kwargs_["function_call"] = {"name": openai_functions[0]["name"]}
     output_parser = output_parser or get_openai_output_parser(functions)
     if prompt:
-        return prompt | llm.bind(**llm_kwargs) | output_parser
+        return prompt | llm.bind(**llm_kwargs_) | output_parser
     else:
-        return llm.bind(**llm_kwargs) | output_parser
+        return llm.bind(**llm_kwargs_) | output_parser
 
 
-# TODO: implement mode='openai-tools'.
 def create_structured_output_runnable(
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
-    mode: Literal["openai-functions", "openai-json"] = "openai-functions",
-    enforce_single_function_usage: bool = True,
+    enforce_function_usage: bool = True,
+    return_single: bool = True,
+    mode: Literal[
+        "openai-functions", "openai-tools", "openai-json"
+    ] = "openai-functions",
     **kwargs: Any,
 ) -> Runnable:
     """Create a runnable for extracting structured outputs.
 
     Args:
         output_schema: Either a dictionary or pydantic.BaseModel class. If a dictionary
             is passed in, it's assumed to already be a valid JsonSchema.
@@ -126,27 +136,115 @@
             prompt has input variable 'output_schema' then the given output_schema 
             will be converted to a JsonSchema and inserted in the prompt.
         output_parser: Output parser to use for parsing model outputs. By default
             will be inferred from the function types. If pydantic.BaseModel is passed
             in, then the OutputParser will try to parse outputs using the pydantic 
             class. Otherwise model outputs will be parsed as JSON.
         mode: How structured outputs are extracted from the model. If 'openai-functions' 
-            then OpenAI function calling is used. If 'openai-json' then OpenAI model 
+            then OpenAI function calling is used with the deprecated 'functions', 
+            'function_call' schema. If 'openai-tools' then OpenAI function 
+            calling with the latest 'tools', 'tool_choice' schema is used. This is 
+            recommended over 'openai-functions'. If 'openai-json' then OpenAI model 
             with response_format set to JSON is used.
-        enforce_single_function_usage: Only used if mode is 'openai-functions'. Only 
-            used if a single function is passed in. If
-            True, then the model will be forced to use the given function. If False,
-            then the model will be given the option to use the given function or not.
+        enforce_function_usage: Only applies when mode is 'openai-tools' or 
+            'openai-functions'. If True, then the model will be forced to use the given 
+            output schema. If False, then the model can elect whether to use the output 
+            schema.
+        return_single: Only applies when mode is 'openai-tools'. Whether to a list of 
+            structured outputs or a single one. If True and model does not return any 
+            structured outputs then chain output is None. If False and model does not 
+            return any structured outputs then chain output is an empty list.
         **kwargs: Additional named arguments.
 
     Returns:
-        A runnable sequence that will return a structured output matching the given 
+        A runnable sequence that will return a structured output(s) matching the given 
             output_schema.
+    
+    OpenAI tools example with Pydantic schema (mode='openai-tools'):
+        .. code-block:: python
+        
+                from typing import Optional
+
+                from langchain.chains import create_structured_output_runnable
+                from langchain_openai import ChatOpenAI
+                from langchain_core.pydantic_v1 import BaseModel, Field
+
+
+                class RecordDog(BaseModel):
+                    '''Record some identifying information about a dog.'''
+
+                    name: str = Field(..., description="The dog's name")
+                    color: str = Field(..., description="The dog's color")
+                    fav_food: Optional[str] = Field(None, description="The dog's favorite food")
+
+                llm = ChatOpenAI(model="gpt-3.5-turbo-0125", temperature=0)
+                prompt = ChatPromptTemplate.from_messages(
+                    [
+                        ("system", "You are an extraction algorithm. Please extract every possible instance"), 
+                        ('human', '{input}')
+                    ]
+                )
+                structured_llm = create_structured_output_runnable(
+                    RecordDog, 
+                    llm, 
+                    mode="openai-tools", 
+                    enforce_function_usage=True, 
+                    return_single=True
+                )
+                structured_llm.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
+                # -> RecordDog(name="Harry", color="brown", fav_food="chicken")
+                
+    OpenAI tools example with dict schema (mode="openai-tools"):
+        .. code-block:: python
+        
+                from typing import Optional
 
-    OpenAI functions example:
+                from langchain.chains import create_structured_output_runnable
+                from langchain_openai import ChatOpenAI
+
+
+                dog_schema = {
+                    "type": "function",
+                    "function": {
+                        "name": "record_dog",
+                        "description": "Record some identifying information about a dog.",
+                        "parameters": {
+                            "type": "object",
+                            "properties": {
+                                "name": {
+                                    "description": "The dog's name",
+                                    "type": "string"
+                                },
+                                "color": {
+                                    "description": "The dog's color",
+                                    "type": "string"
+                                },
+                                "fav_food": {
+                                    "description": "The dog's favorite food",
+                                    "type": "string"
+                                }
+                            },
+                            "required": ["name", "color"]
+                        }
+                    }
+                }
+
+
+                llm = ChatOpenAI(model="gpt-3.5-turbo-0125", temperature=0)
+                structured_llm = create_structured_output_runnable(
+                    doc_schema, 
+                    llm, 
+                    mode="openai-tools", 
+                    enforce_function_usage=True, 
+                    return_single=True
+                )
+                structured_llm.invoke("Harry was a chubby brown beagle who loved chicken")
+                # -> {'name': 'Harry', 'color': 'brown', 'fav_food': 'chicken'}
+    
+    OpenAI functions example (mode="openai-functions"):
         .. code-block:: python
 
                 from typing import Optional
 
                 from langchain.chains import create_structured_output_runnable
                 from langchain_openai import ChatOpenAI
                 from langchain_core.pydantic_v1 import BaseModel, Field
@@ -185,15 +283,15 @@
                 system = '''Extract information about any dogs mentioned in the user input.'''
                 prompt = ChatPromptTemplate.from_messages(
                     [("system", system), ("human", "{input}"),]
                 )
                 chain = prompt | structured_llm
                 chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
                 # -> Dog(name="Harry", color="brown", fav_food="chicken")
-    OpenAI json response format example:
+    OpenAI json response format example (mode="openai-json"):
         .. code-block:: python
         
                 from typing import Optional
 
                 from langchain.chains import create_structured_output_runnable
                 from langchain_openai import ChatOpenAI
                 from langchain_core.prompts import ChatPromptTemplate
@@ -215,34 +313,104 @@
                 {output_schema}'''
                 prompt = ChatPromptTemplate.from_messages(
                     [("system", system), ("human", "{input}"),]
                 )
                 chain = prompt | structured_llm
                 chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
     """  # noqa: E501
-    if mode == "openai-functions":
+    # for backwards compatibility
+    force_function_usage = kwargs.get(
+        "enforce_single_function_usage", enforce_function_usage
+    )
+
+    if mode == "openai-tools":
+        # Protect against typos in kwargs
+        keys_in_kwargs = set(kwargs.keys())
+        # Backwards compatibility keys
+        unrecognized_keys = keys_in_kwargs - {"enforce_single_function_usage"}
+        if unrecognized_keys:
+            raise TypeError(
+                f"Got an unexpected keyword argument(s): {unrecognized_keys}."
+            )
+
+        return _create_openai_tools_runnable(
+            output_schema,
+            llm,
+            prompt=prompt,
+            output_parser=output_parser,
+            enforce_tool_usage=force_function_usage,
+            first_tool_only=return_single,
+        )
+
+    elif mode == "openai-functions":
         return _create_openai_functions_structured_output_runnable(
             output_schema,
             llm,
             prompt=prompt,
             output_parser=output_parser,
-            enforce_single_function_usage=enforce_single_function_usage,
-            **kwargs,
+            enforce_single_function_usage=force_function_usage,
+            **kwargs,  # llm-specific kwargs
         )
     elif mode == "openai-json":
+        if force_function_usage:
+            raise ValueError(
+                "enforce_single_function_usage is not supported for mode='openai-json'."
+            )
         return _create_openai_json_runnable(
             output_schema, llm, prompt=prompt, output_parser=output_parser, **kwargs
         )
     else:
         raise ValueError(
-            f"Invalid mode {mode}. Expected one of 'openai-functions', "
+            f"Invalid mode {mode}. Expected one of 'openai-tools', 'openai-functions', "
             f"'openai-json'."
         )
 
 
+def _create_openai_tools_runnable(
+    tool: Union[Dict[str, Any], Type[BaseModel], Callable],
+    llm: Runnable,
+    *,
+    prompt: Optional[BasePromptTemplate],
+    output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]],
+    enforce_tool_usage: bool,
+    first_tool_only: bool,
+) -> Runnable:
+    oai_tool = convert_to_openai_tool(tool)
+    llm_kwargs: Dict[str, Any] = {"tools": [oai_tool]}
+    if enforce_tool_usage:
+        llm_kwargs["tool_choice"] = {
+            "type": "function",
+            "function": {"name": oai_tool["function"]["name"]},
+        }
+    output_parser = output_parser or _get_openai_tool_output_parser(
+        tool, first_tool_only=first_tool_only
+    )
+    if prompt:
+        return prompt | llm.bind(**llm_kwargs) | output_parser
+    else:
+        return llm.bind(**llm_kwargs) | output_parser
+
+
+def _get_openai_tool_output_parser(
+    tool: Union[Dict[str, Any], Type[BaseModel], Callable],
+    *,
+    first_tool_only: bool = False,
+) -> Union[BaseOutputParser, BaseGenerationOutputParser]:
+    if isinstance(tool, type) and issubclass(tool, BaseModel):
+        output_parser: Union[
+            BaseOutputParser, BaseGenerationOutputParser
+        ] = PydanticToolsParser(tools=[tool], first_tool_only=first_tool_only)
+    else:
+        key_name = convert_to_openai_tool(tool)["function"]["name"]
+        output_parser = JsonOutputKeyToolsParser(
+            first_tool_only=first_tool_only, key_name=key_name
+        )
+    return output_parser
+
+
 def get_openai_output_parser(
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
 ) -> Union[BaseOutputParser, BaseGenerationOutputParser]:
     """Get the appropriate function output parser given the user functions.
 
     Args:
         functions: Sequence where element is a dictionary, a pydantic.BaseModel class,
@@ -251,19 +419,18 @@
 
     Returns:
         A PydanticOutputFunctionsParser if functions are Pydantic classes, otherwise
             a JsonOutputFunctionsParser. If there's only one function and it is
             not a Pydantic class, then the output parser will automatically extract
             only the function arguments and not the function name.
     """
-    function_names = [convert_to_openai_function(f)["name"] for f in functions]
     if isinstance(functions[0], type) and issubclass(functions[0], BaseModel):
         if len(functions) > 1:
             pydantic_schema: Union[Dict, Type[BaseModel]] = {
-                name: fn for name, fn in zip(function_names, functions)
+                convert_to_openai_function(fn)["name"]: fn for fn in functions
             }
         else:
             pydantic_schema = functions[0]
         output_parser: Union[
             BaseOutputParser, BaseGenerationOutputParser
         ] = PydanticOutputFunctionsParser(pydantic_schema=pydantic_schema)
     else:
@@ -300,15 +467,15 @@
 
 def _create_openai_functions_structured_output_runnable(
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
-    **kwargs: Any,
+    **llm_kwargs: Any,
 ) -> Runnable:
     if isinstance(output_schema, dict):
         function: Any = {
             "name": "output_formatter",
             "description": (
                 "Output formatter. Should always be used to format your response to the"
                 " user."
@@ -327,9 +494,9 @@
             pydantic_schema=_OutputFormatter, attr_name="output"
         )
     return create_openai_fn_runnable(
         [function],
         llm,
         prompt=prompt,
         output_parser=output_parser,
-        **kwargs,
+        **llm_kwargs,
     )
```

### Comparing `gigachain-0.1.7.1/langchain/chains/summarize/__init__.py` & `gigachain-0.1.9/langchain/chains/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/summarize/refine_prompts.py` & `gigachain-0.1.9/langchain/chains/summarize/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chains/transform.py` & `gigachain-0.1.9/langchain/chains/transform.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/chat_models/__init__.py` & `gigachain-0.1.9/langchain/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/docstore/__init__.py` & `gigachain-0.1.9/langchain/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_loaders/__init__.py` & `gigachain-0.1.9/langchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_loaders/airbyte.py` & `gigachain-0.1.9/langchain/document_loaders/airbyte.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_loaders/parsers/__init__.py` & `gigachain-0.1.9/langchain/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_loaders/pdf.py` & `gigachain-0.1.9/langchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_loaders/unstructured.py` & `gigachain-0.1.9/langchain/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_transformers/__init__.py` & `gigachain-0.1.9/langchain/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_transformers/loading.py` & `gigachain-0.1.9/langchain/document_transformers/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_transformers/serializers.py` & `gigachain-0.1.9/langchain/document_transformers/serializers.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/document_transformers/xsl/html_chunks_with_headers.xslt` & `gigachain-0.1.9/langchain/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/embeddings/__init__.py` & `gigachain-0.1.9/langchain/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/embeddings/cache.py` & `gigachain-0.1.9/langchain/embeddings/cache.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/__init__.py` & `gigachain-0.1.9/langchain/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/agents/trajectory_eval_chain.py` & `gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/agents/trajectory_eval_prompt.py` & `gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/comparison/__init__.py` & `gigachain-0.1.9/langchain/evaluation/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/comparison/eval_chain.py` & `gigachain-0.1.9/langchain/evaluation/comparison/eval_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/comparison/prompt.py` & `gigachain-0.1.9/langchain/evaluation/comparison/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/criteria/__init__.py` & `gigachain-0.1.9/langchain/evaluation/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/criteria/eval_chain.py` & `gigachain-0.1.9/langchain/evaluation/criteria/eval_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/criteria/prompt.py` & `gigachain-0.1.9/langchain/evaluation/criteria/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/embedding_distance/base.py` & `gigachain-0.1.9/langchain/evaluation/embedding_distance/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/exact_match/base.py` & `gigachain-0.1.9/langchain/evaluation/exact_match/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/loading.py` & `gigachain-0.1.9/langchain/evaluation/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/parsing/base.py` & `gigachain-0.1.9/langchain/evaluation/parsing/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/parsing/json_distance.py` & `gigachain-0.1.9/langchain/evaluation/parsing/json_distance.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/parsing/json_schema.py` & `gigachain-0.1.9/langchain/evaluation/parsing/json_schema.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/qa/eval_chain.py` & `gigachain-0.1.9/langchain/evaluation/qa/eval_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/qa/eval_prompt.py` & `gigachain-0.1.9/langchain/evaluation/qa/eval_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/qa/generate_chain.py` & `gigachain-0.1.9/langchain/evaluation/qa/generate_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/qa/generate_prompt.py` & `gigachain-0.1.9/langchain/evaluation/qa/generate_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/regex_match/base.py` & `gigachain-0.1.9/langchain/evaluation/regex_match/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/schema.py` & `gigachain-0.1.9/langchain/evaluation/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/scoring/__init__.py` & `gigachain-0.1.9/langchain/evaluation/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/scoring/eval_chain.py` & `gigachain-0.1.9/langchain/evaluation/scoring/eval_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/scoring/prompt.py` & `gigachain-0.1.9/langchain/evaluation/scoring/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/evaluation/string_distance/base.py` & `gigachain-0.1.9/langchain/evaluation/string_distance/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/globals/__init__.py` & `gigachain-0.1.9/langchain/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/graphs/__init__.py` & `gigachain-0.1.9/langchain/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/hub.py` & `gigachain-0.1.9/langchain/hub.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/__init__.py` & `gigachain-0.1.9/langchain/indexes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""Code to support various indexing workflows.
+"""**Index** is used to avoid writing duplicated content
+into the vectostore and to avoid over-writing content if it's unchanged.
 
-Provides code to:
+Indexes also :
 
 * Create knowledge graphs from data.
 
 * Support indexing workflows from LangChain data loaders to vectorstores.
 
-For indexing workflows, this code is used to avoid writing duplicated content
-into the vectostore and to avoid over-writing content if it's unchanged.
-
-Importantly, this keeps on working even if the content being written is derived
+Importantly, Index keeps on working even if the content being written is derived
 via a set of transformations from some source content (e.g., indexing children
 documents that were derived from parent documents by chunking.)
 """
 from langchain.indexes._api import IndexingResult, aindex, index
 from langchain.indexes._sql_record_manager import SQLRecordManager
 from langchain.indexes.graph import GraphIndexCreator
 from langchain.indexes.vectorstore import VectorstoreIndexCreator
```

### Comparing `gigachain-0.1.7.1/langchain/indexes/_api.py` & `gigachain-0.1.9/langchain/indexes/_api.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/_sql_record_manager.py` & `gigachain-0.1.9/langchain/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/base.py` & `gigachain-0.1.9/langchain/indexes/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/graph.py` & `gigachain-0.1.9/langchain/indexes/graph.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/prompts/entity_extraction.py` & `gigachain-0.1.9/langchain/indexes/prompts/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/prompts/entity_summarization.py` & `gigachain-0.1.9/langchain/indexes/prompts/entity_summarization.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/prompts/knowledge_triplet_extraction.py` & `gigachain-0.1.9/langchain/indexes/prompts/knowledge_triplet_extraction.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/indexes/vectorstore.py` & `gigachain-0.1.9/langchain/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/llms/__init__.py` & `gigachain-0.1.9/langchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/llms/grammars/json.gbnf` & `gigachain-0.1.9/langchain/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/__init__.py` & `gigachain-0.1.9/langchain/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/buffer.py` & `gigachain-0.1.9/langchain/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/buffer_window.py` & `gigachain-0.1.9/langchain/memory/buffer_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     @property
     def buffer(self) -> Union[str, List[BaseMessage]]:
         """String buffer of memory."""
         return self.buffer_as_messages if self.return_messages else self.buffer_as_str
 
     @property
     def buffer_as_str(self) -> str:
-        """Exposes the buffer as a string in case return_messages is True."""
+        """Exposes the buffer as a string in case return_messages is False."""
         messages = self.chat_memory.messages[-self.k * 2 :] if self.k > 0 else []
         return get_buffer_string(
             messages,
             human_prefix=self.human_prefix,
             ai_prefix=self.ai_prefix,
         )
 
     @property
     def buffer_as_messages(self) -> List[BaseMessage]:
-        """Exposes the buffer as a list of messages in case return_messages is False."""
+        """Exposes the buffer as a list of messages in case return_messages is True."""
         return self.chat_memory.messages[-self.k * 2 :] if self.k > 0 else []
 
     @property
     def memory_variables(self) -> List[str]:
         """Will always return list of memory variables.
 
         :meta private:
```

### Comparing `gigachain-0.1.7.1/langchain/memory/chat_memory.py` & `gigachain-0.1.9/langchain/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/chat_message_histories/__init__.py` & `gigachain-0.1.9/langchain/memory/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/combined.py` & `gigachain-0.1.9/langchain/memory/combined.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/entity.py` & `gigachain-0.1.9/langchain/memory/entity.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/kg.py` & `gigachain-0.1.9/langchain/memory/kg.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/motorhead_memory.py` & `gigachain-0.1.9/langchain/memory/motorhead_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/prompt.py` & `gigachain-0.1.9/langchain/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/readonly.py` & `gigachain-0.1.9/langchain/memory/readonly.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/simple.py` & `gigachain-0.1.9/langchain/memory/simple.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/summary.py` & `gigachain-0.1.9/langchain/memory/summary.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/summary_buffer.py` & `gigachain-0.1.9/langchain/memory/summary_buffer.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/token_buffer.py` & `gigachain-0.1.9/langchain/memory/token_buffer.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/utils.py` & `gigachain-0.1.9/langchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/vectorstore.py` & `gigachain-0.1.9/langchain/memory/vectorstore.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/memory/zep_memory.py` & `gigachain-0.1.9/langchain/memory/zep_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/model_laboratory.py` & `gigachain-0.1.9/langchain/model_laboratory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/__init__.py` & `gigachain-0.1.9/langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/boolean.py` & `gigachain-0.1.9/langchain/output_parsers/boolean.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,19 +15,30 @@
         Args:
             text: output of a language model
 
         Returns:
             boolean
 
         """
-        cleaned_text = text.strip()
-        if cleaned_text.upper() not in (self.true_val.upper(), self.false_val.upper()):
+        cleaned_upper_text = text.strip().upper()
+        if (
+            self.true_val.upper() in cleaned_upper_text
+            and self.false_val.upper() in cleaned_upper_text
+        ):
             raise ValueError(
-                f"BooleanOutputParser expected output value to either be "
-                f"{self.true_val} or {self.false_val}. Received {cleaned_text}."
+                f"Ambiguous response. Both {self.true_val} and {self.false_val} in "
+                f"received: {text}."
+            )
+        elif self.true_val.upper() in cleaned_upper_text:
+            return True
+        elif self.false_val.upper() in cleaned_upper_text:
+            return False
+        else:
+            raise ValueError(
+                f"BooleanOutputParser expected output value to include either "
+                f"{self.true_val} or {self.false_val}. Received {text}."
             )
-        return cleaned_text.upper() == self.true_val.upper()
 
     @property
     def _type(self) -> str:
         """Snake-case string identifier for an output parser type."""
         return "boolean_output_parser"
```

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/combining.py` & `gigachain-0.1.9/langchain/output_parsers/combining.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/datetime.py` & `gigachain-0.1.9/langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/enum.py` & `gigachain-0.1.9/langchain/output_parsers/enum.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/fix.py` & `gigachain-0.1.9/langchain/output_parsers/fix.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/format_instructions.py` & `gigachain-0.1.9/langchain/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/loading.py` & `gigachain-0.1.9/langchain/output_parsers/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/pandas_dataframe.py` & `gigachain-0.1.9/langchain/output_parsers/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/prompts.py` & `gigachain-0.1.9/langchain/output_parsers/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/pydantic.py` & `gigachain-0.1.9/langchain/output_parsers/yaml.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 import json
-from typing import Any, List, Type
+import re
+from typing import Type, TypeVar
 
+import yaml
 from langchain_core.exceptions import OutputParserException
-from langchain_core.output_parsers import JsonOutputParser
-from langchain_core.outputs import Generation
+from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.pydantic_v1 import BaseModel, ValidationError
 
-from langchain.output_parsers.format_instructions import PYDANTIC_FORMAT_INSTRUCTIONS
+from langchain.output_parsers.format_instructions import YAML_FORMAT_INSTRUCTIONS
 
+T = TypeVar("T", bound=BaseModel)
 
-class PydanticOutputParser(JsonOutputParser):
-    """Parse an output using a pydantic model."""
 
-    pydantic_object: Type[BaseModel]
-    """The pydantic model to parse.
-    
-    Attention: To avoid potential compatibility issues, it's recommended to use
-        pydantic <2 or leverage the v1 namespace in pydantic >= 2.
-    """
+class YamlOutputParser(BaseOutputParser[T]):
+    """Parse YAML output using a pydantic model."""
 
-    def parse_result(self, result: List[Generation], *, partial: bool = False) -> Any:
-        json_object = super().parse_result(result)
+    pydantic_object: Type[T]
+    """The pydantic model to parse."""
+    pattern: re.Pattern = re.compile(
+        r"^```(?:ya?ml)?(?P<yaml>[^`]*)", re.MULTILINE | re.DOTALL
+    )
+    """Regex pattern to match yaml code blocks 
+    within triple backticks with optional yaml or yml prefix."""
+
+    def parse(self, text: str) -> T:
         try:
+            # Greedy search for 1st yaml candidate.
+            match = re.search(self.pattern, text.strip())
+            yaml_str = ""
+            if match:
+                yaml_str = match.group("yaml")
+            else:
+                # If no backticks were present, try to parse the entire output as yaml.
+                yaml_str = text
+
+            json_object = yaml.safe_load(yaml_str)
             return self.pydantic_object.parse_obj(json_object)
-        except ValidationError as e:
+
+        except (yaml.YAMLError, ValidationError) as e:
             name = self.pydantic_object.__name__
-            msg = f"Failed to parse {name} from completion {json_object}. Got: {e}"
-            raise OutputParserException(msg, llm_output=json_object)
+            msg = f"Failed to parse {name} from completion {text}. Got: {e}"
+            raise OutputParserException(msg, llm_output=text) from e
 
     def get_format_instructions(self) -> str:
         # Copy schema to avoid altering original Pydantic schema.
         schema = {k: v for k, v in self.pydantic_object.schema().items()}
 
         # Remove extraneous fields.
         reduced_schema = schema
         if "title" in reduced_schema:
             del reduced_schema["title"]
         if "type" in reduced_schema:
             del reduced_schema["type"]
-        # Ensure json in context is well-formed with double quotes.
-        schema_str = json.dumps(reduced_schema, ensure_ascii=False)
+        # Ensure yaml in context is well-formed with double quotes.
+        schema_str = json.dumps(reduced_schema)
 
-        return PYDANTIC_FORMAT_INSTRUCTIONS.format(schema=schema_str)
+        return YAML_FORMAT_INSTRUCTIONS.format(schema=schema_str)
 
     @property
     def _type(self) -> str:
-        return "pydantic"
-
-    @property
-    def OutputType(self) -> Type[BaseModel]:
-        """Return the pydantic model."""
-        return self.pydantic_object
+        return "yaml"
```

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/regex.py` & `gigachain-0.1.9/langchain/output_parsers/regex.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/regex_dict.py` & `gigachain-0.1.9/langchain/output_parsers/regex_dict.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/retry.py` & `gigachain-0.1.9/langchain/output_parsers/retry.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/output_parsers/structured.py` & `gigachain-0.1.9/langchain/output_parsers/structured.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/prompts/__init__.py` & `gigachain-0.1.9/langchain/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/prompts/base.py` & `gigachain-0.1.9/langchain/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/prompts/chat.py` & `gigachain-0.1.9/langchain/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/prompts/example_selector/__init__.py` & `gigachain-0.1.9/langchain/prompts/example_selector/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/prompts/loading.py` & `gigachain-0.1.9/langchain/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/pydantic_v1/__init__.py` & `gigachain-0.1.9/langchain/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/__init__.py` & `gigachain-0.1.9/langchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/contextual_compression.py` & `gigachain-0.1.9/langchain/retrievers/contextual_compression.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/__init__.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/base.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,19 @@
-from abc import ABC, abstractmethod
 from inspect import signature
 from typing import List, Optional, Sequence, Union
 
-from langchain_core.documents import BaseDocumentTransformer, Document
-from langchain_core.pydantic_v1 import BaseModel
-from langchain_core.runnables.config import run_in_executor
+from langchain_core.documents import (
+    BaseDocumentCompressor,
+    BaseDocumentTransformer,
+    Document,
+)
 
 from langchain.callbacks.manager import Callbacks
 
 
-class BaseDocumentCompressor(BaseModel, ABC):
-    """Base class for document compressors."""
-
-    @abstractmethod
-    def compress_documents(
-        self,
-        documents: Sequence[Document],
-        query: str,
-        callbacks: Optional[Callbacks] = None,
-    ) -> Sequence[Document]:
-        """Compress retrieved documents given the query context."""
-
-    async def acompress_documents(
-        self,
-        documents: Sequence[Document],
-        query: str,
-        callbacks: Optional[Callbacks] = None,
-    ) -> Sequence[Document]:
-        """Compress retrieved documents given the query context."""
-        return await run_in_executor(
-            None, self.compress_documents, documents, query, callbacks
-        )
-
-
 class DocumentCompressorPipeline(BaseDocumentCompressor):
     """Document compressor that uses a pipeline of Transformers."""
 
     transformers: List[Union[BaseDocumentTransformer, BaseDocumentCompressor]]
     """List of document filters that are chained together and run in sequence."""
 
     class Config:
```

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_extract.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_extract_prompt.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/chain_filter.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/chain_filter.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/cohere_rerank.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/embeddings_filter.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/embeddings_filter.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/document_compressors/flashrank_rerank.py` & `gigachain-0.1.9/langchain/retrievers/document_compressors/flashrank_rerank.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/ensemble.py` & `gigachain-0.1.9/langchain/retrievers/ensemble.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/kendra.py` & `gigachain-0.1.9/langchain/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/merger_retriever.py` & `gigachain-0.1.9/langchain/retrievers/merger_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/multi_query.py` & `gigachain-0.1.9/langchain/retrievers/multi_query.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/multi_vector.py` & `gigachain-0.1.9/langchain/retrievers/multi_vector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/parent_document_retriever.py` & `gigachain-0.1.9/langchain/retrievers/parent_document_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/re_phraser.py` & `gigachain-0.1.9/langchain/retrievers/re_phraser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/astradb.py` & `gigachain-0.1.9/langchain/retrievers/self_query/astradb.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/base.py` & `gigachain-0.1.9/langchain/retrievers/self_query/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from langchain.retrievers.self_query.redis import RedisTranslator
 from langchain.retrievers.self_query.supabase import SupabaseVectorTranslator
 from langchain.retrievers.self_query.timescalevector import TimescaleVectorTranslator
 from langchain.retrievers.self_query.vectara import VectaraTranslator
 from langchain.retrievers.self_query.weaviate import WeaviateTranslator
 
 logger = logging.getLogger(__name__)
+QUERY_CONSTRUCTOR_RUN_NAME = "query_constructor"
 
 
 def _get_builtin_translator(vectorstore: VectorStore) -> Visitor:
     """Get the translator class corresponding to the vector store class."""
     BUILTIN_TRANSLATORS: Dict[Type[VectorStore], Type[Visitor]] = {
         AstraDB: AstraDBTranslator,
         PGVector: PGVectorTranslator,
@@ -72,23 +73,32 @@
         ElasticsearchStore: ElasticsearchTranslator,
         Milvus: MilvusTranslator,
         SupabaseVectorStore: SupabaseVectorTranslator,
         TimescaleVector: TimescaleVectorTranslator,
         OpenSearchVectorSearch: OpenSearchTranslator,
         MongoDBAtlasVectorSearch: MongoDBAtlasTranslator,
     }
+
     if isinstance(vectorstore, Qdrant):
         return QdrantTranslator(metadata_key=vectorstore.metadata_payload_key)
     elif isinstance(vectorstore, MyScale):
         return MyScaleTranslator(metadata_key=vectorstore.metadata_column)
     elif isinstance(vectorstore, Redis):
         return RedisTranslator.from_vectorstore(vectorstore)
     elif vectorstore.__class__ in BUILTIN_TRANSLATORS:
         return BUILTIN_TRANSLATORS[vectorstore.__class__]()
     else:
+        try:
+            from langchain_astradb.vectorstores import AstraDBVectorStore
+
+            if isinstance(vectorstore, AstraDBVectorStore):
+                return AstraDBTranslator()
+        except ImportError:
+            pass
+
         raise ValueError(
             f"Self query retriever with Vector Store type {vectorstore.__class__}"
             f" not supported."
         )
 
 
 class SelfQueryRetriever(BaseRetriever):
@@ -231,14 +241,17 @@
         query_constructor = load_query_constructor_runnable(
             llm,
             document_contents,
             metadata_field_info,
             enable_limit=enable_limit,
             **chain_kwargs,
         )
+        query_constructor = query_constructor.with_config(
+            run_name=QUERY_CONSTRUCTOR_RUN_NAME
+        )
         return cls(
             query_constructor=query_constructor,
             vectorstore=vectorstore,
             use_original_query=use_original_query,
             structured_query_translator=structured_query_translator,
             **kwargs,
         )
```

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/chroma.py` & `gigachain-0.1.9/langchain/retrievers/self_query/chroma.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/dashvector.py` & `gigachain-0.1.9/langchain/retrievers/self_query/dashvector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/deeplake.py` & `gigachain-0.1.9/langchain/retrievers/self_query/deeplake.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/elasticsearch.py` & `gigachain-0.1.9/langchain/retrievers/self_query/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/milvus.py` & `gigachain-0.1.9/langchain/retrievers/self_query/milvus.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/mongodb_atlas.py` & `gigachain-0.1.9/langchain/retrievers/self_query/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/myscale.py` & `gigachain-0.1.9/langchain/retrievers/self_query/myscale.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/opensearch.py` & `gigachain-0.1.9/langchain/retrievers/self_query/opensearch.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/pgvector.py` & `gigachain-0.1.9/langchain/retrievers/self_query/pgvector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/pinecone.py` & `gigachain-0.1.9/langchain/retrievers/self_query/pinecone.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/qdrant.py` & `gigachain-0.1.9/langchain/retrievers/self_query/qdrant.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/redis.py` & `gigachain-0.1.9/langchain/retrievers/self_query/redis.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/supabase.py` & `gigachain-0.1.9/langchain/retrievers/self_query/supabase.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/timescalevector.py` & `gigachain-0.1.9/langchain/retrievers/self_query/timescalevector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/vectara.py` & `gigachain-0.1.9/langchain/retrievers/self_query/vectara.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/self_query/weaviate.py` & `gigachain-0.1.9/langchain/retrievers/self_query/weaviate.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/time_weighted_retriever.py` & `gigachain-0.1.9/langchain/retrievers/time_weighted_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/retrievers/web_research.py` & `gigachain-0.1.9/langchain/retrievers/web_research.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,26 +74,28 @@
     text_splitter: TextSplitter = Field(
         RecursiveCharacterTextSplitter(chunk_size=1500, chunk_overlap=50),
         description="Text splitter for splitting web pages into chunks",
     )
     url_database: List[str] = Field(
         default_factory=list, description="List of processed URLs"
     )
+    verify_ssl: bool = Field(True, description="Verify SSL certificate")
 
     @classmethod
     def from_llm(
         cls,
         vectorstore: VectorStore,
         llm: BaseLLM,
         search: GoogleSearchAPIWrapper,
         prompt: Optional[BasePromptTemplate] = None,
         num_search_results: int = 1,
         text_splitter: RecursiveCharacterTextSplitter = RecursiveCharacterTextSplitter(
             chunk_size=1500, chunk_overlap=150
         ),
+        verify_ssl: bool = True,
     ) -> "WebResearchRetriever":
         """Initialize from llm using default template.
 
         Args:
             vectorstore: Vector store for storing web pages
             llm: llm for search question generation
             search: GoogleSearchAPIWrapper
@@ -123,14 +125,15 @@
 
         return cls(
             vectorstore=vectorstore,
             llm_chain=llm_chain,
             search=search,
             num_search_results=num_search_results,
             text_splitter=text_splitter,
+            verify_ssl=verify_ssl,
         )
 
     def clean_search_query(self, query: str) -> str:
         # Some search tools (e.g., Google) will
         # fail to return results if query has a
         # leading digit: 1. "LangCh..."
         # Check if the first character is a digit
@@ -190,22 +193,27 @@
 
         # Check for any new urls that we have not processed
         new_urls = list(urls.difference(self.url_database))
 
         logger.info(f"New URLs to load: {new_urls}")
         # Load, split, and add new urls to vectorstore
         if new_urls:
-            loader = AsyncHtmlLoader(new_urls, ignore_load_errors=True)
+            loader = AsyncHtmlLoader(
+                new_urls, ignore_load_errors=True, verify_ssl=self.verify_ssl
+            )
             html2text = Html2TextTransformer()
             logger.info("Indexing new urls...")
             docs = loader.load()
             docs = list(html2text.transform_documents(docs))
             docs = self.text_splitter.split_documents(docs)
             self.vectorstore.add_documents(docs)
-            self.url_database.extend(new_urls)
+            if len(docs) > 0:
+                self.url_database.extend(new_urls)
+            else:
+                raise ValueError("No documents were loaded")
 
         # Search for relevant splits
         # TODO: make this async
         logger.info("Grabbing most relevant splits from urls...")
         docs = []
         for query in questions:
             docs.extend(self.vectorstore.similarity_search(query))
```

### Comparing `gigachain-0.1.7.1/langchain/runnables/hub.py` & `gigachain-0.1.9/langchain/runnables/hub.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/runnables/openai_functions.py` & `gigachain-0.1.9/langchain/runnables/openai_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from operator import itemgetter
 from typing import Any, Callable, List, Mapping, Optional, Union
 
 from langchain_core.messages import BaseMessage
+from langchain_core.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain_core.runnables import RouterRunnable, Runnable
 from langchain_core.runnables.base import RunnableBindingBase
 from typing_extensions import TypedDict
 
-from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
-
 
 class OpenAIFunction(TypedDict):
     """A function description for ChatOpenAI"""
 
     name: str
     """The name of the function."""
     description: str
```

### Comparing `gigachain-0.1.7.1/langchain/schema/__init__.py` & `gigachain-0.1.9/langchain/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/callbacks/manager.py` & `gigachain-0.1.9/langchain/schema/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/messages.py` & `gigachain-0.1.9/langchain/schema/messages.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/output_parser.py` & `gigachain-0.1.9/langchain/schema/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/runnable/__init__.py` & `gigachain-0.1.9/langchain/schema/runnable/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/runnable/base.py` & `gigachain-0.1.9/langchain/schema/runnable/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/runnable/config.py` & `gigachain-0.1.9/langchain/schema/runnable/config.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/schema/runnable/utils.py` & `gigachain-0.1.9/langchain/schema/runnable/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/smith/__init__.py` & `gigachain-0.1.9/langchain/smith/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/smith/evaluation/__init__.py` & `gigachain-0.1.9/langchain/smith/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/smith/evaluation/config.py` & `gigachain-0.1.9/langchain/smith/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/smith/evaluation/name_generation.py` & `gigachain-0.1.9/langchain/smith/evaluation/name_generation.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/smith/evaluation/progress.py` & `gigachain-0.1.9/langchain/smith/evaluation/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """A simple progress bar for the console."""
 
 import threading
 from typing import Any, Dict, Optional, Sequence
 from uuid import UUID
 
+from langchain_core.callbacks import base as base_callbacks
 from langchain_core.documents import Document
 from langchain_core.outputs import LLMResult
 
-from langchain.callbacks import base as base_callbacks
-
 
 class ProgressBarCallback(base_callbacks.BaseCallbackHandler):
     """A simple progress bar for the console."""
 
     def __init__(self, total: int, ncols: int = 50, **kwargs: Any):
         """Initialize the progress bar.
```

### Comparing `gigachain-0.1.7.1/langchain/smith/evaluation/runner_utils.py` & `gigachain-0.1.9/langchain/smith/evaluation/runner_utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/smith/evaluation/string_run_evaluator.py` & `gigachain-0.1.9/langchain/smith/evaluation/string_run_evaluator.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/storage/__init__.py` & `gigachain-0.1.9/langchain/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/storage/_lc_store.py` & `gigachain-0.1.9/langchain/storage/_lc_store.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/storage/encoder_backed.py` & `gigachain-0.1.9/langchain/storage/encoder_backed.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/storage/file_system.py` & `gigachain-0.1.9/langchain/storage/file_system.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/storage/in_memory.py` & `gigachain-0.1.9/langchain/storage/in_memory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/text_splitter.py` & `gigachain-0.1.9/langchain/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/__init__.py` & `gigachain-0.1.9/langchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/azure_cognitive_services/__init__.py` & `gigachain-0.1.9/langchain/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/edenai/__init__.py` & `gigachain-0.1.9/langchain/tools/edenai/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/file_management/__init__.py` & `gigachain-0.1.9/langchain/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/office365/__init__.py` & `gigachain-0.1.9/langchain/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/openapi/utils/api_models.py` & `gigachain-0.1.9/langchain/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/playwright/__init__.py` & `gigachain-0.1.9/langchain/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/python/__init__.py` & `gigachain-0.1.9/langchain/tools/python/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/render.py` & `gigachain-0.1.9/langchain/tools/render.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/tools/retriever.py` & `gigachain-0.1.9/langchain/tools/retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/utilities/__init__.py` & `gigachain-0.1.9/langchain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/utils/__init__.py` & `gigachain-0.1.9/langchain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/langchain/vectorstores/__init__.py` & `gigachain-0.1.9/langchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.7.1/pyproject.toml` & `gigachain-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "gigachain"
-version = "0.1.7.1"
+version = "0.1.9"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain"}
 ]
 
 [tool.poetry.scripts]
 langchain-server = "langchain.server:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = ">=0.1.22,<0.2"
-gigachain-community = ">=0.0.20,<0.1"
-langsmith = ">=0.0.83,<0.1"
-gigachat = ">=0.1.16"
+gigachain-core = ">=0.1.26,<0.2"
+gigachain-community = ">=0.0.21,<0.1"
+langsmith = "^0.1.0"
+gigachat = ">=0.1.17"
 pydantic = ">=1,<3"
 SQLAlchemy = ">=1.4,<3"
 requests = "^2"
 PyYAML = ">=5.3"
 numpy = "^1"
 aiohttp = "^3.8.3"
 tenacity = "^8.1.0"
```

### Comparing `gigachain-0.1.7.1/PKG-INFO` & `gigachain-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain
-Version: 0.1.7.1
+Version: 0.1.9
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -56,30 +56,30 @@
 Requires-Dist: dgml-utils (>=0.3.0,<0.4.0) ; extra == "extended-testing"
 Requires-Dist: docarray[hnswlib] (>=0.32.0,<0.33.0) ; extra == "docarray"
 Requires-Dist: esprima (>=4.0.1,<5.0.0) ; extra == "javascript" or extra == "extended-testing"
 Requires-Dist: faiss-cpu (>=1,<2) ; extra == "extended-testing"
 Requires-Dist: feedparser (>=6.0.10,<7.0.0) ; extra == "extended-testing"
 Requires-Dist: fireworks-ai (>=0.9.0,<0.10.0) ; extra == "extended-testing"
 Requires-Dist: geopandas (>=0.13.1,<0.14.0) ; extra == "extended-testing"
-Requires-Dist: gigachain-community (>=0.0.20,<0.1)
-Requires-Dist: gigachain-core (>=0.1.22,<0.2)
+Requires-Dist: gigachain-community (>=0.0.21,<0.1)
+Requires-Dist: gigachain-core (>=0.1.26,<0.2)
 Requires-Dist: gigachain-openai (>=0.0.2,<0.1) ; extra == "extended-testing"
-Requires-Dist: gigachat (>=0.1.16)
+Requires-Dist: gigachat (>=0.1.17)
 Requires-Dist: gitpython (>=3.1.32,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: google-cloud-documentai (>=2.20.1,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: gql (>=3.4.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: hologres-vector (>=0.0.6,<0.0.7) ; extra == "extended-testing"
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0) ; extra == "extended-testing"
 Requires-Dist: huggingface_hub (>=0,<1) ; extra == "llms"
 Requires-Dist: javelin-sdk (>=0.1.8,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: jq (>=1.4.1,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: jsonpatch (>=1.33,<2.0)
 Requires-Dist: jsonschema (>1) ; extra == "extended-testing"
-Requires-Dist: langsmith (>=0.0.83,<0.1)
+Requires-Dist: langsmith (>=0.1.0,<0.2.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0) ; extra == "extended-testing"
 Requires-Dist: manifest-ml (>=0.0.1,<0.0.2) ; extra == "llms"
 Requires-Dist: markdownify (>=0.11.6,<0.12.0) ; extra == "extended-testing"
 Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: msal (>=1.25.0,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: mwparserfromhell (>=0.6.4,<0.7.0) ; extra == "extended-testing"
 Requires-Dist: mwxml (>=0.3.3,<0.4.0) ; extra == "extended-testing"
```

