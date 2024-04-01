# Comparing `tmp/parea_ai-0.2.98.tar.gz` & `tmp/parea_ai-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parea_ai-0.2.98.tar", max compression
+gzip compressed data, was "parea_ai-0.2.99.tar", max compression
```

## Comparing `parea_ai-0.2.98.tar` & `parea_ai-0.2.99.tar`

### file list

```diff
@@ -1,110 +1,112 @@
--rw-r--r--   0        0        0    10885 2023-08-20 21:20:28.852856 parea_ai-0.2.98/LICENSE
--rw-r--r--   0        0        0     9235 2024-02-14 14:14:12.122946 parea_ai-0.2.98/README.md
--rw-r--r--   0        0        0     1468 2024-02-22 22:03:59.883162 parea_ai-0.2.98/parea/__init__.py
--rw-r--r--   0        0        0     6946 2024-02-27 00:02:12.059435 parea_ai-0.2.98/parea/api_client.py
--rw-r--r--   0        0        0       67 2023-12-04 15:41:40.745154 parea_ai-0.2.98/parea/cache/__init__.py
--rw-r--r--   0        0        0     2440 2024-01-31 18:19:44.430549 parea_ai-0.2.98/parea/cache/cache.py
--rw-r--r--   0        0        0     1086 2024-02-08 22:51:08.684428 parea_ai-0.2.98/parea/cache/in_memory.py
--rw-r--r--   0        0        0     3413 2024-02-08 22:51:08.684669 parea_ai-0.2.98/parea/cache/redis.py
--rw-r--r--   0        0        0    13125 2024-03-08 21:39:10.307068 parea_ai-0.2.98/parea/client.py
--rw-r--r--   0        0        0    28920 2024-02-13 19:28:34.590078 parea_ai-0.2.98/parea/constants.py
--rw-r--r--   0        0        0        0 2023-12-28 15:31:08.905428 parea_ai-0.2.98/parea/cookbook/__init__.py
--rw-r--r--   0        0        0    32707 2023-12-28 15:31:08.905634 parea_ai-0.2.98/parea/cookbook/data/2022-letter.txt
--rw-r--r--   0        0        0     3266 2024-02-02 23:05:25.496913 parea_ai-0.2.98/parea/cookbook/data/openai_input_examples.py
--rw-r--r--   0        0        0    39028 2023-12-28 15:31:08.906159 parea_ai-0.2.98/parea/cookbook/data/state_of_the_union.txt
--rw-r--r--   0        0        0     1032 2024-02-22 22:03:59.886734 parea_ai-0.2.98/parea/cookbook/enpoints_for_datasets.py
--rw-r--r--   0        0        0   125729 2023-10-20 10:37:54.166453 parea_ai-0.2.98/parea/cookbook/img/dashboard.png
--rw-r--r--   0        0        0   188882 2023-10-20 10:37:54.169788 parea_ai-0.2.98/parea/cookbook/img/dashboard_detailed_view.png
--rw-r--r--   0        0        0   164710 2023-10-20 10:37:54.173123 parea_ai-0.2.98/parea/cookbook/img/deployed_prompts.png
--rw-r--r--   0        0        0   155407 2023-10-20 10:37:54.175947 parea_ai-0.2.98/parea/cookbook/img/feedback.png
--rw-r--r--   0        0        0   108037 2023-10-20 10:37:54.178843 parea_ai-0.2.98/parea/cookbook/img/logs.png
--rw-r--r--   0        0        0    97109 2023-10-20 10:37:54.181383 parea_ai-0.2.98/parea/cookbook/img/meta_data.png
--rw-r--r--   0        0        0   208641 2023-12-11 20:59:22.654215 parea_ai-0.2.98/parea/cookbook/img/trace_log_view.png
--rw-r--r--   0        0        0       33 2024-02-06 23:02:17.644166 parea_ai-0.2.98/parea/cookbook/inputs.csv
--rw-r--r--   0        0        0        0 2023-12-28 15:31:08.906254 parea_ai-0.2.98/parea/cookbook/langchain/__init__.py
--rw-r--r--   0        0        0     8779 2024-03-09 20:10:44.017375 parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_RAG_evals.py
--rw-r--r--   0        0        0     1641 2024-01-26 18:26:54.386918 parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_anthropic_function_calling.py
--rw-r--r--   0        0        0     2754 2024-01-26 18:26:54.370113 parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_bedrock_rag.py
--rw-r--r--   0        0        0     1376 2024-01-26 18:26:54.354773 parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_rag_agents.py
--rw-r--r--   0        0        0     1500 2024-02-01 23:01:58.981813 parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_rag_question_answering.py
--rw-r--r--   0        0        0      990 2024-03-08 21:39:10.307831 parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_simple.py
--rw-r--r--   0        0        0     5005 2024-02-06 23:02:17.644693 parea_ai-0.2.98/parea/cookbook/oai_no_streaming_old_oai.py
--rw-r--r--   0        0        0     4863 2024-02-22 23:35:25.811944 parea_ai-0.2.98/parea/cookbook/oai_streaming_new_oai.py
--rw-r--r--   0        0        0     4824 2024-02-06 23:02:17.645765 parea_ai-0.2.98/parea/cookbook/oai_streaming_old_oai.py
--rw-r--r--   0        0        0     1264 2024-02-06 23:02:17.646226 parea_ai-0.2.98/parea/cookbook/random_number_generator.py
--rw-r--r--   0        0        0     1129 2024-02-22 22:03:55.228218 parea_ai-0.2.98/parea/cookbook/run_experiment.py
--rw-r--r--   0        0        0     1571 2024-03-09 20:10:44.017920 parea_ai-0.2.98/parea/cookbook/run_experiment_balanced_acc.py
--rw-r--r--   0        0        0     1311 2024-02-22 22:03:59.889052 parea_ai-0.2.98/parea/cookbook/run_experiment_using_saved_test_collection.py
--rw-r--r--   0        0        0     1100 2024-02-08 23:35:46.006378 parea_ai-0.2.98/parea/cookbook/run_experiment_with_targets.py
--rw-r--r--   0        0        0    17865 2024-02-06 23:02:17.646953 parea_ai-0.2.98/parea/cookbook/trace_logs-1706294443.csv
--rw-r--r--   0        0        0     4630 2024-02-19 20:43:08.161836 parea_ai-0.2.98/parea/cookbook/tracing_and_evaluating_openai_endpoint.py
--rw-r--r--   0        0        0     1884 2024-02-08 23:34:31.673739 parea_ai-0.2.98/parea/cookbook/tracing_azure_open_ai.py
--rw-r--r--   0        0        0     1128 2024-03-09 20:10:44.018210 parea_ai-0.2.98/parea/cookbook/tracing_open_ai_streams.py
--rw-r--r--   0        0        0      526 2024-02-06 23:02:17.647486 parea_ai-0.2.98/parea/cookbook/tracing_openai_test.py
--rw-r--r--   0        0        0      452 2024-02-06 23:02:17.647870 parea_ai-0.2.98/parea/cookbook/tracing_scores.py
--rw-r--r--   0        0        0     1604 2024-03-09 20:14:17.361770 parea_ai-0.2.98/parea/cookbook/tracing_tool_calling.py
--rw-r--r--   0        0        0    23307 2024-02-08 22:53:13.397873 parea_ai-0.2.98/parea/cookbook/tracing_with_Parea_sdk.ipynb
--rw-r--r--   0        0        0     3807 2024-02-22 22:03:59.889504 parea_ai-0.2.98/parea/cookbook/tracing_with_agent.py
--rw-r--r--   0        0        0     3430 2024-02-08 22:51:08.689759 parea_ai-0.2.98/parea/cookbook/tracing_with_deployed_prompt.py
--rw-r--r--   0        0        0     9599 2024-02-08 22:53:13.370880 parea_ai-0.2.98/parea/cookbook/tracing_with_function_calling_and_chains.ipynb
--rw-r--r--   0        0        0     1419 2024-03-08 21:39:10.307940 parea_ai-0.2.98/parea/cookbook/tracing_with_images_open_ai.py
--rw-r--r--   0        0        0     1782 2024-03-01 23:02:45.003485 parea_ai-0.2.98/parea/cookbook/tracing_with_instructor.py
--rw-r--r--   0        0        0     3325 2024-02-08 22:51:08.691230 parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_directly.py
--rw-r--r--   0        0        0     3067 2024-02-06 23:02:17.648509 parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_directly2.py
--rw-r--r--   0        0        0     3568 2024-02-06 23:02:17.648924 parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_directly_new_openai_version.py
--rw-r--r--   0        0        0      671 2024-02-06 23:02:17.649359 parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_simple.py
--rw-r--r--   0        0        0     2594 2024-02-19 20:43:05.891725 parea_ai-0.2.98/parea/cookbook/tracing_with_openai_requests_api.py
--rw-r--r--   0        0        0     8428 2024-02-08 22:51:08.693759 parea_ai-0.2.98/parea/cookbook/tracing_with_openai_with_functions.py
--rw-r--r--   0        0        0      792 2024-02-13 19:28:34.590829 parea_ai-0.2.98/parea/cookbook/tracing_with_parea_streaming.py
--rw-r--r--   0        0        0     5775 2024-02-13 19:28:34.591183 parea_ai-0.2.98/parea/cookbook/tracing_without_deployed_prompt.py
--rw-r--r--   0        0        0      110 2024-02-08 22:51:08.694538 parea_ai-0.2.98/parea/evals/__init__.py
--rw-r--r--   0        0        0       59 2023-12-11 20:59:22.656375 parea_ai-0.2.98/parea/evals/chat/__init__.py
--rw-r--r--   0        0        0     3502 2024-01-08 19:18:44.325772 parea_ai-0.2.98/parea/evals/chat/goal_success_ratio.py
--rw-r--r--   0        0        0       47 2024-02-27 00:02:12.060624 parea_ai-0.2.98/parea/evals/dataset_level/__init__.py
--rw-r--r--   0        0        0      665 2024-02-27 00:02:12.061117 parea_ai-0.2.98/parea/evals/dataset_level/balanced_acc.py
--rw-r--r--   0        0        0      626 2024-02-15 16:35:22.512942 parea_ai-0.2.98/parea/evals/general/__init__.py
--rw-r--r--   0        0        0     1755 2023-12-11 20:59:22.657405 parea_ai-0.2.98/parea/evals/general/answer_matches_target_llm_grader.py
--rw-r--r--   0        0        0      637 2024-01-26 13:43:59.773760 parea_ai-0.2.98/parea/evals/general/answer_matches_target_recall.py
--rw-r--r--   0        0        0     2691 2024-02-08 23:53:45.691619 parea_ai-0.2.98/parea/evals/general/answer_relevancy.py
--rw-r--r--   0        0        0      453 2024-02-15 16:35:22.513297 parea_ai-0.2.98/parea/evals/general/levenshtein.py
--rw-r--r--   0        0        0     3256 2024-01-31 18:19:44.432522 parea_ai-0.2.98/parea/evals/general/llm_grader.py
--rw-r--r--   0        0        0     4903 2024-02-01 21:55:37.203450 parea_ai-0.2.98/parea/evals/general/lm_vs_lm.py
--rw-r--r--   0        0        0     2903 2024-02-01 21:55:37.203798 parea_ai-0.2.98/parea/evals/general/self_check.py
--rw-r--r--   0        0        0     1077 2024-02-13 19:28:34.592160 parea_ai-0.2.98/parea/evals/general/semantic_similarity.py
--rw-r--r--   0        0        0      662 2024-02-26 20:09:21.220133 parea_ai-0.2.98/parea/evals/rag/__init__.py
--rw-r--r--   0        0        0     2701 2024-01-08 19:18:44.328858 parea_ai-0.2.98/parea/evals/rag/answer_context_faithfulness_binary.py
--rw-r--r--   0        0        0     1778 2024-01-26 13:43:59.773968 parea_ai-0.2.98/parea/evals/rag/answer_context_faithfulness_precision.py
--rw-r--r--   0        0        0     6010 2024-01-31 18:19:44.432780 parea_ai-0.2.98/parea/evals/rag/answer_context_faithfulness_statement_level.py
--rw-r--r--   0        0        0     1882 2024-02-26 20:09:21.220288 parea_ai-0.2.98/parea/evals/rag/context_has_answer.py
--rw-r--r--   0        0        0     2508 2024-01-31 18:19:44.433028 parea_ai-0.2.98/parea/evals/rag/context_query_relevancy.py
--rw-r--r--   0        0        0     4682 2024-01-31 18:19:44.433656 parea_ai-0.2.98/parea/evals/rag/context_ranking_listwise.py
--rw-r--r--   0        0        0     4384 2024-01-31 18:19:44.433873 parea_ai-0.2.98/parea/evals/rag/context_ranking_pointwise.py
--rw-r--r--   0        0        0     4779 2024-01-31 18:19:44.434110 parea_ai-0.2.98/parea/evals/rag/percent_target_supported_by_context.py
--rw-r--r--   0        0        0      203 2023-12-11 20:59:22.661739 parea_ai-0.2.98/parea/evals/summary/__init__.py
--rw-r--r--   0        0        0     2050 2024-01-08 19:18:44.332330 parea_ai-0.2.98/parea/evals/summary/factual_inconsistency_binary.py
--rw-r--r--   0        0        0     2205 2024-01-08 19:18:44.332737 parea_ai-0.2.98/parea/evals/summary/factual_inconsistency_scale.py
--rw-r--r--   0        0        0     3141 2024-01-08 19:18:44.333263 parea_ai-0.2.98/parea/evals/summary/likert_scale.py
--rw-r--r--   0        0        0     4491 2024-02-27 00:02:12.061548 parea_ai-0.2.98/parea/evals/utils.py
--rw-r--r--   0        0        0        0 2024-01-08 15:00:33.228017 parea_ai-0.2.98/parea/experiment/__init__.py
--rw-r--r--   0        0        0     1368 2024-02-07 15:30:38.423848 parea_ai-0.2.98/parea/experiment/cli.py
--rw-r--r--   0        0        0     2844 2024-03-04 13:39:44.040082 parea_ai-0.2.98/parea/experiment/datasets.py
--rw-r--r--   0        0        0     3303 2024-02-08 22:51:08.694801 parea_ai-0.2.98/parea/experiment/dvc.py
--rw-r--r--   0        0        0     9602 2024-02-29 22:19:15.915003 parea_ai-0.2.98/parea/experiment/experiment.py
--rw-r--r--   0        0        0     2577 2024-03-09 20:07:53.904076 parea_ai-0.2.98/parea/helpers.py
--rw-r--r--   0        0        0     3125 2024-02-22 22:03:59.892027 parea_ai-0.2.98/parea/parea_logger.py
--rw-r--r--   0        0        0       41 2024-02-08 22:51:08.695958 parea_ai-0.2.98/parea/schemas/__init__.py
--rw-r--r--   0        0        0     3600 2024-03-06 16:16:29.205192 parea_ai-0.2.98/parea/schemas/log.py
--rw-r--r--   0        0        0     7326 2024-03-08 21:39:10.308748 parea_ai-0.2.98/parea/schemas/models.py
--rw-r--r--   0        0        0     1798 2024-03-04 13:39:44.041450 parea_ai-0.2.98/parea/types.py
--rw-r--r--   0        0        0        0 2023-08-27 01:13:16.987358 parea_ai-0.2.98/parea/utils/__init__.py
--rw-r--r--   0        0        0      971 2024-03-08 21:39:10.308893 parea_ai-0.2.98/parea/utils/trace_integrations/langchain.py
--rw-r--r--   0        0        0    12017 2024-03-08 21:39:10.309648 parea_ai-0.2.98/parea/utils/trace_utils.py
--rw-r--r--   0        0        0     2507 2024-03-04 13:39:44.042963 parea_ai-0.2.98/parea/utils/universal_encoder.py
--rw-r--r--   0        0        0      149 2024-03-01 23:55:10.234333 parea_ai-0.2.98/parea/wrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 23:55:10.235044 parea_ai-0.2.98/parea/wrapper/openai/__init__.py
--rw-r--r--   0        0        0    15483 2024-03-04 13:39:44.043318 parea_ai-0.2.98/parea/wrapper/openai/openai.py
--rw-r--r--   0        0        0     4037 2024-03-04 13:39:44.043541 parea_ai-0.2.98/parea/wrapper/openai_raw_api_tracer.py
--rw-r--r--   0        0        0    13201 2024-03-09 20:20:45.553686 parea_ai-0.2.98/parea/wrapper/utils.py
--rw-r--r--   0        0        0    10257 2024-03-04 13:39:44.044292 parea_ai-0.2.98/parea/wrapper/wrapper.py
--rw-r--r--   0        0        0     3992 2024-03-09 20:22:28.875120 parea_ai-0.2.98/pyproject.toml
--rw-r--r--   0        0        0    10657 1970-01-01 00:00:00.000000 parea_ai-0.2.98/PKG-INFO
+-rw-r--r--   0        0        0    10885 2023-08-20 21:20:28.852856 parea_ai-0.2.99/LICENSE
+-rw-r--r--   0        0        0     9235 2024-02-14 14:14:12.122946 parea_ai-0.2.99/README.md
+-rw-r--r--   0        0        0     1468 2024-02-22 22:03:59.883162 parea_ai-0.2.99/parea/__init__.py
+-rw-r--r--   0        0        0     6946 2024-02-27 00:02:12.059435 parea_ai-0.2.99/parea/api_client.py
+-rw-r--r--   0        0        0       67 2023-12-04 15:41:40.745154 parea_ai-0.2.99/parea/cache/__init__.py
+-rw-r--r--   0        0        0     2440 2024-01-31 18:19:44.430549 parea_ai-0.2.99/parea/cache/cache.py
+-rw-r--r--   0        0        0     1086 2024-02-08 22:51:08.684428 parea_ai-0.2.99/parea/cache/in_memory.py
+-rw-r--r--   0        0        0     3413 2024-02-08 22:51:08.684669 parea_ai-0.2.99/parea/cache/redis.py
+-rw-r--r--   0        0        0    13125 2024-03-12 22:48:50.884472 parea_ai-0.2.99/parea/client.py
+-rw-r--r--   0        0        0    28920 2024-02-13 19:28:34.590078 parea_ai-0.2.99/parea/constants.py
+-rw-r--r--   0        0        0        0 2023-12-28 15:31:08.905428 parea_ai-0.2.99/parea/cookbook/__init__.py
+-rw-r--r--   0        0        0    32707 2023-12-28 15:31:08.905634 parea_ai-0.2.99/parea/cookbook/data/2022-letter.txt
+-rw-r--r--   0        0        0     3266 2024-02-02 23:05:25.496913 parea_ai-0.2.99/parea/cookbook/data/openai_input_examples.py
+-rw-r--r--   0        0        0    75042 2024-03-13 16:26:11.800763 parea_ai-0.2.99/parea/cookbook/data/pg-essay/paul_graham_essay.txt
+-rw-r--r--   0        0        0    39028 2023-12-28 15:31:08.906159 parea_ai-0.2.99/parea/cookbook/data/state_of_the_union.txt
+-rw-r--r--   0        0        0     1032 2024-02-22 22:03:59.886734 parea_ai-0.2.99/parea/cookbook/enpoints_for_datasets.py
+-rw-r--r--   0        0        0   125729 2023-10-20 10:37:54.166453 parea_ai-0.2.99/parea/cookbook/img/dashboard.png
+-rw-r--r--   0        0        0   188882 2023-10-20 10:37:54.169788 parea_ai-0.2.99/parea/cookbook/img/dashboard_detailed_view.png
+-rw-r--r--   0        0        0   164710 2023-10-20 10:37:54.173123 parea_ai-0.2.99/parea/cookbook/img/deployed_prompts.png
+-rw-r--r--   0        0        0   155407 2023-10-20 10:37:54.175947 parea_ai-0.2.99/parea/cookbook/img/feedback.png
+-rw-r--r--   0        0        0   108037 2023-10-20 10:37:54.178843 parea_ai-0.2.99/parea/cookbook/img/logs.png
+-rw-r--r--   0        0        0    97109 2023-10-20 10:37:54.181383 parea_ai-0.2.99/parea/cookbook/img/meta_data.png
+-rw-r--r--   0        0        0   208641 2023-12-11 20:59:22.654215 parea_ai-0.2.99/parea/cookbook/img/trace_log_view.png
+-rw-r--r--   0        0        0       33 2024-02-06 23:02:17.644166 parea_ai-0.2.99/parea/cookbook/inputs.csv
+-rw-r--r--   0        0        0        0 2023-12-28 15:31:08.906254 parea_ai-0.2.99/parea/cookbook/langchain/__init__.py
+-rw-r--r--   0        0        0     8779 2024-03-09 20:10:44.017375 parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_RAG_evals.py
+-rw-r--r--   0        0        0     1641 2024-01-26 18:26:54.386918 parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_anthropic_function_calling.py
+-rw-r--r--   0        0        0     2754 2024-01-26 18:26:54.370113 parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_bedrock_rag.py
+-rw-r--r--   0        0        0     1376 2024-01-26 18:26:54.354773 parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_rag_agents.py
+-rw-r--r--   0        0        0     1500 2024-02-01 23:01:58.981813 parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_rag_question_answering.py
+-rw-r--r--   0        0        0      990 2024-03-08 21:39:10.307831 parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_simple.py
+-rw-r--r--   0        0        0     5005 2024-02-06 23:02:17.644693 parea_ai-0.2.99/parea/cookbook/oai_no_streaming_old_oai.py
+-rw-r--r--   0        0        0     4863 2024-02-22 23:35:25.811944 parea_ai-0.2.99/parea/cookbook/oai_streaming_new_oai.py
+-rw-r--r--   0        0        0     4824 2024-02-06 23:02:17.645765 parea_ai-0.2.99/parea/cookbook/oai_streaming_old_oai.py
+-rw-r--r--   0        0        0     1264 2024-02-06 23:02:17.646226 parea_ai-0.2.99/parea/cookbook/random_number_generator.py
+-rw-r--r--   0        0        0     1129 2024-02-22 22:03:55.228218 parea_ai-0.2.99/parea/cookbook/run_experiment.py
+-rw-r--r--   0        0        0     1571 2024-03-12 22:48:50.885960 parea_ai-0.2.99/parea/cookbook/run_experiment_balanced_acc.py
+-rw-r--r--   0        0        0     1311 2024-02-22 22:03:59.889052 parea_ai-0.2.99/parea/cookbook/run_experiment_using_saved_test_collection.py
+-rw-r--r--   0        0        0     1100 2024-02-08 23:35:46.006378 parea_ai-0.2.99/parea/cookbook/run_experiment_with_targets.py
+-rw-r--r--   0        0        0     1943 2024-03-13 17:00:09.495765 parea_ai-0.2.99/parea/cookbook/run_experimnt_pg.py
+-rw-r--r--   0        0        0    17865 2024-02-06 23:02:17.646953 parea_ai-0.2.99/parea/cookbook/trace_logs-1706294443.csv
+-rw-r--r--   0        0        0     4630 2024-02-19 20:43:08.161836 parea_ai-0.2.99/parea/cookbook/tracing_and_evaluating_openai_endpoint.py
+-rw-r--r--   0        0        0     1884 2024-03-13 16:55:55.165940 parea_ai-0.2.99/parea/cookbook/tracing_azure_open_ai.py
+-rw-r--r--   0        0        0     1128 2024-03-09 20:10:44.018210 parea_ai-0.2.99/parea/cookbook/tracing_open_ai_streams.py
+-rw-r--r--   0        0        0      526 2024-02-06 23:02:17.647486 parea_ai-0.2.99/parea/cookbook/tracing_openai_test.py
+-rw-r--r--   0        0        0      452 2024-02-06 23:02:17.647870 parea_ai-0.2.99/parea/cookbook/tracing_scores.py
+-rw-r--r--   0        0        0     1604 2024-03-12 22:48:50.886426 parea_ai-0.2.99/parea/cookbook/tracing_tool_calling.py
+-rw-r--r--   0        0        0    23307 2024-02-08 22:53:13.397873 parea_ai-0.2.99/parea/cookbook/tracing_with_Parea_sdk.ipynb
+-rw-r--r--   0        0        0     3807 2024-02-22 22:03:59.889504 parea_ai-0.2.99/parea/cookbook/tracing_with_agent.py
+-rw-r--r--   0        0        0     3430 2024-02-08 22:51:08.689759 parea_ai-0.2.99/parea/cookbook/tracing_with_deployed_prompt.py
+-rw-r--r--   0        0        0     9599 2024-02-08 22:53:13.370880 parea_ai-0.2.99/parea/cookbook/tracing_with_function_calling_and_chains.ipynb
+-rw-r--r--   0        0        0     1419 2024-03-13 16:55:45.238431 parea_ai-0.2.99/parea/cookbook/tracing_with_images_open_ai.py
+-rw-r--r--   0        0        0     1833 2024-03-09 22:27:17.573469 parea_ai-0.2.99/parea/cookbook/tracing_with_instructor.py
+-rw-r--r--   0        0        0     3325 2024-02-08 22:51:08.691230 parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_directly.py
+-rw-r--r--   0        0        0     3067 2024-02-06 23:02:17.648509 parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_directly2.py
+-rw-r--r--   0        0        0     3568 2024-02-06 23:02:17.648924 parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_directly_new_openai_version.py
+-rw-r--r--   0        0        0      671 2024-02-06 23:02:17.649359 parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_simple.py
+-rw-r--r--   0        0        0     2594 2024-02-19 20:43:05.891725 parea_ai-0.2.99/parea/cookbook/tracing_with_openai_requests_api.py
+-rw-r--r--   0        0        0     8428 2024-02-08 22:51:08.693759 parea_ai-0.2.99/parea/cookbook/tracing_with_openai_with_functions.py
+-rw-r--r--   0        0        0      792 2024-02-13 19:28:34.590829 parea_ai-0.2.99/parea/cookbook/tracing_with_parea_streaming.py
+-rw-r--r--   0        0        0     5775 2024-02-13 19:28:34.591183 parea_ai-0.2.99/parea/cookbook/tracing_without_deployed_prompt.py
+-rw-r--r--   0        0        0      110 2024-02-08 22:51:08.694538 parea_ai-0.2.99/parea/evals/__init__.py
+-rw-r--r--   0        0        0       59 2023-12-11 20:59:22.656375 parea_ai-0.2.99/parea/evals/chat/__init__.py
+-rw-r--r--   0        0        0     3502 2024-01-08 19:18:44.325772 parea_ai-0.2.99/parea/evals/chat/goal_success_ratio.py
+-rw-r--r--   0        0        0       47 2024-02-27 00:02:12.060624 parea_ai-0.2.99/parea/evals/dataset_level/__init__.py
+-rw-r--r--   0        0        0      665 2024-02-27 00:02:12.061117 parea_ai-0.2.99/parea/evals/dataset_level/balanced_acc.py
+-rw-r--r--   0        0        0      626 2024-02-15 16:35:22.512942 parea_ai-0.2.99/parea/evals/general/__init__.py
+-rw-r--r--   0        0        0     1755 2023-12-11 20:59:22.657405 parea_ai-0.2.99/parea/evals/general/answer_matches_target_llm_grader.py
+-rw-r--r--   0        0        0      637 2024-01-26 13:43:59.773760 parea_ai-0.2.99/parea/evals/general/answer_matches_target_recall.py
+-rw-r--r--   0        0        0     2691 2024-02-08 23:53:45.691619 parea_ai-0.2.99/parea/evals/general/answer_relevancy.py
+-rw-r--r--   0        0        0      453 2024-02-15 16:35:22.513297 parea_ai-0.2.99/parea/evals/general/levenshtein.py
+-rw-r--r--   0        0        0     3256 2024-01-31 18:19:44.432522 parea_ai-0.2.99/parea/evals/general/llm_grader.py
+-rw-r--r--   0        0        0     4903 2024-02-01 21:55:37.203450 parea_ai-0.2.99/parea/evals/general/lm_vs_lm.py
+-rw-r--r--   0        0        0     2903 2024-02-01 21:55:37.203798 parea_ai-0.2.99/parea/evals/general/self_check.py
+-rw-r--r--   0        0        0     1077 2024-02-13 19:28:34.592160 parea_ai-0.2.99/parea/evals/general/semantic_similarity.py
+-rw-r--r--   0        0        0      662 2024-02-26 20:09:21.220133 parea_ai-0.2.99/parea/evals/rag/__init__.py
+-rw-r--r--   0        0        0     2701 2024-01-08 19:18:44.328858 parea_ai-0.2.99/parea/evals/rag/answer_context_faithfulness_binary.py
+-rw-r--r--   0        0        0     1778 2024-01-26 13:43:59.773968 parea_ai-0.2.99/parea/evals/rag/answer_context_faithfulness_precision.py
+-rw-r--r--   0        0        0     6010 2024-01-31 18:19:44.432780 parea_ai-0.2.99/parea/evals/rag/answer_context_faithfulness_statement_level.py
+-rw-r--r--   0        0        0     1882 2024-02-26 20:09:21.220288 parea_ai-0.2.99/parea/evals/rag/context_has_answer.py
+-rw-r--r--   0        0        0     2508 2024-01-31 18:19:44.433028 parea_ai-0.2.99/parea/evals/rag/context_query_relevancy.py
+-rw-r--r--   0        0        0     4682 2024-01-31 18:19:44.433656 parea_ai-0.2.99/parea/evals/rag/context_ranking_listwise.py
+-rw-r--r--   0        0        0     4384 2024-01-31 18:19:44.433873 parea_ai-0.2.99/parea/evals/rag/context_ranking_pointwise.py
+-rw-r--r--   0        0        0     4779 2024-01-31 18:19:44.434110 parea_ai-0.2.99/parea/evals/rag/percent_target_supported_by_context.py
+-rw-r--r--   0        0        0      203 2023-12-11 20:59:22.661739 parea_ai-0.2.99/parea/evals/summary/__init__.py
+-rw-r--r--   0        0        0     2050 2024-01-08 19:18:44.332330 parea_ai-0.2.99/parea/evals/summary/factual_inconsistency_binary.py
+-rw-r--r--   0        0        0     2205 2024-01-08 19:18:44.332737 parea_ai-0.2.99/parea/evals/summary/factual_inconsistency_scale.py
+-rw-r--r--   0        0        0     3141 2024-01-08 19:18:44.333263 parea_ai-0.2.99/parea/evals/summary/likert_scale.py
+-rw-r--r--   0        0        0     4491 2024-02-27 00:02:12.061548 parea_ai-0.2.99/parea/evals/utils.py
+-rw-r--r--   0        0        0        0 2024-01-08 15:00:33.228017 parea_ai-0.2.99/parea/experiment/__init__.py
+-rw-r--r--   0        0        0     1368 2024-02-07 15:30:38.423848 parea_ai-0.2.99/parea/experiment/cli.py
+-rw-r--r--   0        0        0     2844 2024-03-04 13:39:44.040082 parea_ai-0.2.99/parea/experiment/datasets.py
+-rw-r--r--   0        0        0     3303 2024-02-08 22:51:08.694801 parea_ai-0.2.99/parea/experiment/dvc.py
+-rw-r--r--   0        0        0     9602 2024-02-29 22:19:15.915003 parea_ai-0.2.99/parea/experiment/experiment.py
+-rw-r--r--   0        0        0     2781 2024-03-13 17:02:52.572359 parea_ai-0.2.99/parea/helpers.py
+-rw-r--r--   0        0        0     3125 2024-02-22 22:03:59.892027 parea_ai-0.2.99/parea/parea_logger.py
+-rw-r--r--   0        0        0       41 2024-02-08 22:51:08.695958 parea_ai-0.2.99/parea/schemas/__init__.py
+-rw-r--r--   0        0        0     3600 2024-03-06 16:16:29.205192 parea_ai-0.2.99/parea/schemas/log.py
+-rw-r--r--   0        0        0     7326 2024-03-08 21:39:10.308748 parea_ai-0.2.99/parea/schemas/models.py
+-rw-r--r--   0        0        0     1798 2024-03-04 13:39:44.041450 parea_ai-0.2.99/parea/types.py
+-rw-r--r--   0        0        0        0 2023-08-27 01:13:16.987358 parea_ai-0.2.99/parea/utils/__init__.py
+-rw-r--r--   0        0        0      971 2024-03-08 21:39:10.308893 parea_ai-0.2.99/parea/utils/trace_integrations/langchain.py
+-rw-r--r--   0        0        0    12017 2024-03-08 21:39:10.309648 parea_ai-0.2.99/parea/utils/trace_utils.py
+-rw-r--r--   0        0        0     2507 2024-03-04 13:39:44.042963 parea_ai-0.2.99/parea/utils/universal_encoder.py
+-rw-r--r--   0        0        0      149 2024-03-01 23:55:10.234333 parea_ai-0.2.99/parea/wrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 23:55:10.235044 parea_ai-0.2.99/parea/wrapper/openai/__init__.py
+-rw-r--r--   0        0        0    15483 2024-03-12 22:48:50.886750 parea_ai-0.2.99/parea/wrapper/openai/openai.py
+-rw-r--r--   0        0        0     4037 2024-03-04 13:39:44.043541 parea_ai-0.2.99/parea/wrapper/openai_raw_api_tracer.py
+-rw-r--r--   0        0        0    13201 2024-03-09 20:24:19.496957 parea_ai-0.2.99/parea/wrapper/utils.py
+-rw-r--r--   0        0        0    10257 2024-03-12 22:48:50.886992 parea_ai-0.2.99/parea/wrapper/wrapper.py
+-rw-r--r--   0        0        0     3992 2024-03-13 17:03:52.662785 parea_ai-0.2.99/pyproject.toml
+-rw-r--r--   0        0        0    10657 1970-01-01 00:00:00.000000 parea_ai-0.2.99/PKG-INFO
```

### Comparing `parea_ai-0.2.98/LICENSE` & `parea_ai-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/README.md` & `parea_ai-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/__init__.py` & `parea_ai-0.2.99/parea/__init__.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/api_client.py` & `parea_ai-0.2.99/parea/api_client.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cache/cache.py` & `parea_ai-0.2.99/parea/cache/cache.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cache/in_memory.py` & `parea_ai-0.2.99/parea/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cache/redis.py` & `parea_ai-0.2.99/parea/cache/redis.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/client.py` & `parea_ai-0.2.99/parea/client.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/constants.py` & `parea_ai-0.2.99/parea/constants.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/data/2022-letter.txt` & `parea_ai-0.2.99/parea/cookbook/data/2022-letter.txt`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/data/openai_input_examples.py` & `parea_ai-0.2.99/parea/cookbook/data/openai_input_examples.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/data/state_of_the_union.txt` & `parea_ai-0.2.99/parea/cookbook/data/state_of_the_union.txt`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/enpoints_for_datasets.py` & `parea_ai-0.2.99/parea/cookbook/enpoints_for_datasets.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/dashboard.png` & `parea_ai-0.2.99/parea/cookbook/img/dashboard.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/dashboard_detailed_view.png` & `parea_ai-0.2.99/parea/cookbook/img/dashboard_detailed_view.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/deployed_prompts.png` & `parea_ai-0.2.99/parea/cookbook/img/deployed_prompts.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/feedback.png` & `parea_ai-0.2.99/parea/cookbook/img/feedback.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/logs.png` & `parea_ai-0.2.99/parea/cookbook/img/logs.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/meta_data.png` & `parea_ai-0.2.99/parea/cookbook/img/meta_data.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/img/trace_log_view.png` & `parea_ai-0.2.99/parea/cookbook/img/trace_log_view.png`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_RAG_evals.py` & `parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_RAG_evals.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_anthropic_function_calling.py` & `parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_anthropic_function_calling.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_bedrock_rag.py` & `parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_bedrock_rag.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_rag_agents.py` & `parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_rag_agents.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_rag_question_answering.py` & `parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_rag_question_answering.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/langchain/trace_langchain_simple.py` & `parea_ai-0.2.99/parea/cookbook/langchain/trace_langchain_simple.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/oai_no_streaming_old_oai.py` & `parea_ai-0.2.99/parea/cookbook/oai_no_streaming_old_oai.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/oai_streaming_new_oai.py` & `parea_ai-0.2.99/parea/cookbook/oai_streaming_new_oai.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/oai_streaming_old_oai.py` & `parea_ai-0.2.99/parea/cookbook/oai_streaming_old_oai.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/random_number_generator.py` & `parea_ai-0.2.99/parea/cookbook/random_number_generator.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/run_experiment.py` & `parea_ai-0.2.99/parea/cookbook/run_experiment.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/run_experiment_balanced_acc.py` & `parea_ai-0.2.99/parea/cookbook/run_experiment_balanced_acc.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/run_experiment_using_saved_test_collection.py` & `parea_ai-0.2.99/parea/cookbook/run_experiment_using_saved_test_collection.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/run_experiment_with_targets.py` & `parea_ai-0.2.99/parea/cookbook/run_experiment_with_targets.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/trace_logs-1706294443.csv` & `parea_ai-0.2.99/parea/cookbook/trace_logs-1706294443.csv`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_and_evaluating_openai_endpoint.py` & `parea_ai-0.2.99/parea/cookbook/tracing_and_evaluating_openai_endpoint.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_azure_open_ai.py` & `parea_ai-0.2.99/parea/cookbook/tracing_azure_open_ai.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_open_ai_streams.py` & `parea_ai-0.2.99/parea/cookbook/tracing_open_ai_streams.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_openai_test.py` & `parea_ai-0.2.99/parea/cookbook/tracing_openai_test.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_tool_calling.py` & `parea_ai-0.2.99/parea/cookbook/tracing_tool_calling.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_Parea_sdk.ipynb` & `parea_ai-0.2.99/parea/cookbook/tracing_with_Parea_sdk.ipynb`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_agent.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_agent.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_deployed_prompt.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_deployed_prompt.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_function_calling_and_chains.ipynb` & `parea_ai-0.2.99/parea/cookbook/tracing_with_function_calling_and_chains.ipynb`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_images_open_ai.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_images_open_ai.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_instructor.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_instructor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
 
 import asyncio
 import inspect
 import os
 
+from dotenv import load_dotenv
 from openai import AsyncOpenAI
 
 # import openai
 from pydantic import BaseModel
 
 
 def print_levels(func):
@@ -21,22 +22,26 @@
 
 client = AsyncOpenAI()
 print('Before patching')
 print_levels(client.chat.completions.create)
 
 from parea import Parea
 
+# load_dotenv()
+
 p = Parea(api_key=os.getenv("PAREA_API_KEY"), project_name='testing')
 p.wrap_openai_client(client)
 print('patched with parea')
 print_levels(client.chat.completions.create)
 
+
 import instructor
 
-client = instructor.patch(client, mode=instructor.Mode.TOOLS)
+
+client2 = instructor.patch(client, mode=instructor.Mode.TOOLS)
 # print(inspect.iscoroutine(client.chat.completions.create))
 print('patched with instructor')
 print_levels(client.chat.completions.create)
 
 
 class UserExtract(BaseModel):
     name: str
```

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_directly.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_directly.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_directly2.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_directly2.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_directly_new_openai_version.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_directly_new_openai_version.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_open_ai_endpoint_simple.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_open_ai_endpoint_simple.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_openai_requests_api.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_openai_requests_api.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_openai_with_functions.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_openai_with_functions.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_with_parea_streaming.py` & `parea_ai-0.2.99/parea/cookbook/tracing_with_parea_streaming.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/cookbook/tracing_without_deployed_prompt.py` & `parea_ai-0.2.99/parea/cookbook/tracing_without_deployed_prompt.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/chat/goal_success_ratio.py` & `parea_ai-0.2.99/parea/evals/chat/goal_success_ratio.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/dataset_level/balanced_acc.py` & `parea_ai-0.2.99/parea/evals/dataset_level/balanced_acc.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/__init__.py` & `parea_ai-0.2.99/parea/evals/general/__init__.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/answer_matches_target_llm_grader.py` & `parea_ai-0.2.99/parea/evals/general/answer_matches_target_llm_grader.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/answer_matches_target_recall.py` & `parea_ai-0.2.99/parea/evals/general/answer_matches_target_recall.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/answer_relevancy.py` & `parea_ai-0.2.99/parea/evals/general/answer_relevancy.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/llm_grader.py` & `parea_ai-0.2.99/parea/evals/general/llm_grader.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/lm_vs_lm.py` & `parea_ai-0.2.99/parea/evals/general/lm_vs_lm.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/self_check.py` & `parea_ai-0.2.99/parea/evals/general/self_check.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/general/semantic_similarity.py` & `parea_ai-0.2.99/parea/evals/general/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/__init__.py` & `parea_ai-0.2.99/parea/evals/rag/__init__.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/answer_context_faithfulness_binary.py` & `parea_ai-0.2.99/parea/evals/rag/answer_context_faithfulness_binary.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/answer_context_faithfulness_precision.py` & `parea_ai-0.2.99/parea/evals/rag/answer_context_faithfulness_precision.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/answer_context_faithfulness_statement_level.py` & `parea_ai-0.2.99/parea/evals/rag/answer_context_faithfulness_statement_level.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/context_has_answer.py` & `parea_ai-0.2.99/parea/evals/rag/context_has_answer.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/context_query_relevancy.py` & `parea_ai-0.2.99/parea/evals/rag/context_query_relevancy.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/context_ranking_listwise.py` & `parea_ai-0.2.99/parea/evals/rag/context_ranking_listwise.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/context_ranking_pointwise.py` & `parea_ai-0.2.99/parea/evals/rag/context_ranking_pointwise.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/rag/percent_target_supported_by_context.py` & `parea_ai-0.2.99/parea/evals/rag/percent_target_supported_by_context.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/summary/factual_inconsistency_binary.py` & `parea_ai-0.2.99/parea/evals/summary/factual_inconsistency_binary.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/summary/factual_inconsistency_scale.py` & `parea_ai-0.2.99/parea/evals/summary/factual_inconsistency_scale.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/summary/likert_scale.py` & `parea_ai-0.2.99/parea/evals/summary/likert_scale.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/evals/utils.py` & `parea_ai-0.2.99/parea/evals/utils.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/experiment/cli.py` & `parea_ai-0.2.99/parea/experiment/cli.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/experiment/datasets.py` & `parea_ai-0.2.99/parea/experiment/datasets.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/experiment/dvc.py` & `parea_ai-0.2.99/parea/experiment/dvc.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/experiment/experiment.py` & `parea_ai-0.2.99/parea/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/helpers.py` & `parea_ai-0.2.99/parea/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,17 +61,21 @@
         return log_data
 
     if log_data.metadata:
         serialized_values = serialize_values(log_data.metadata)
         log_data.metadata = serialized_values
 
     # Support openai vision content format
-    if log_data.configuration:
-        for message in log_data.configuration.messages or []:
-            if isinstance(message, dict) and "content" in message and not isinstance(message["content"], str):
-                message["content"] = json_dumps(message["content"])
+    messages = []
+    if isinstance(log_data, TraceLog) and log_data.configuration:
+        messages = log_data.configuration.messages or []
+    elif isinstance(log_data, Completion) and log_data.llm_configuration:
+        messages = log_data.llm_configuration.messages or []
+    for message in messages:
+        if isinstance(message, dict) and "content" in message and not isinstance(message["content"], str):
+            message["content"] = json_dumps(message["content"])
 
     return log_data
 
 
 def timezone_aware_now() -> datetime:
     return datetime.now(pytz.utc)
```

### Comparing `parea_ai-0.2.98/parea/parea_logger.py` & `parea_ai-0.2.99/parea/parea_logger.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/schemas/log.py` & `parea_ai-0.2.99/parea/schemas/log.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/schemas/models.py` & `parea_ai-0.2.99/parea/schemas/models.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/types.py` & `parea_ai-0.2.99/parea/types.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/utils/trace_integrations/langchain.py` & `parea_ai-0.2.99/parea/utils/trace_integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/utils/trace_utils.py` & `parea_ai-0.2.99/parea/utils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/utils/universal_encoder.py` & `parea_ai-0.2.99/parea/utils/universal_encoder.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/wrapper/openai/openai.py` & `parea_ai-0.2.99/parea/wrapper/openai/openai.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/wrapper/openai_raw_api_tracer.py` & `parea_ai-0.2.99/parea/wrapper/openai_raw_api_tracer.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/wrapper/utils.py` & `parea_ai-0.2.99/parea/wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/parea/wrapper/wrapper.py` & `parea_ai-0.2.99/parea/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.2.98/pyproject.toml` & `parea_ai-0.2.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "parea-ai"
 packages = [{ include = "parea" }]
-version = "0.2.98"
+version = "0.2.99"
 description = "Parea python sdk"
 readme = "README.md"
 authors = ["joel-parea-ai <joel@parea.ai>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/parea-ai/parea-sdk"
 homepage = "https://github.com/parea-ai/parea-sdk"
```

### Comparing `parea_ai-0.2.98/PKG-INFO` & `parea_ai-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parea-ai
-Version: 0.2.98
+Version: 0.2.99
 Summary: Parea python sdk
 Home-page: https://github.com/parea-ai/parea-sdk
 License: Apache Software License 2.0
 Author: joel-parea-ai
 Author-email: joel@parea.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

