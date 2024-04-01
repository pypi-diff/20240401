# Comparing `tmp/langtrace_python_sdk-1.2.8.tar.gz` & `tmp/langtrace_python_sdk-1.2.9.tar.gz`

## Comparing `langtrace_python_sdk-1.2.8.tar` & `langtrace_python_sdk-1.2.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/openai/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/openai/chat_completion.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/openai/embeddings_create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/openai/function_calling.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/openai/images_generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/tests/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/tests/utils.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/LICENSE
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/README.md
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/chat_completion.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/embeddings_create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/function_calling.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/openai/images_generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/utils.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/LICENSE
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/README.md
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 langtrace_python_sdk-1.2.9/PKG-INFO
```

### Comparing `langtrace_python_sdk-1.2.8/src/run_example.py` & `langtrace_python_sdk-1.2.9/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-1.2.9/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-1.2.9/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-1.2.9/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-1.2.9/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-1.2.9/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/openai/chat_completion.py` & `langtrace_python_sdk-1.2.9/src/examples/openai/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/openai/embeddings_create.py` & `langtrace_python_sdk-1.2.9/src/examples/openai/embeddings_create.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/openai/function_calling.py` & `langtrace_python_sdk-1.2.9/src/examples/openai/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-1.2.9/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/langtrace.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-1.2.9/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/tests/utils.py` & `langtrace_python_sdk-1.2.9/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-1.2.9/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-1.2.9/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-1.2.9/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-1.2.9/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/.gitignore` & `langtrace_python_sdk-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/LICENSE` & `langtrace_python_sdk-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/README.md` & `langtrace_python_sdk-1.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 ## Getting Started
 
 To begin utilizing Langtrace, follow these straightforward steps:
 
 1. Install the package using `pip install langtrace-python-sdk`.
 2. Incorporate Langtrace into your project with `from langtrace_python_sdk import langtrace`.
    - This import should precede any other LLM module imports (such as OpenAI, LlamaIndex, etc.) to ensure proper functionality.
-3. Initialize Langtrace by adding `langtrace.init({ write_to_remote_url: false})` to your code.
+3. Initialize Langtrace by adding `langtrace.init(write_to_langtrace_cloud=false)` to your code.
 4. Congratulations, you've completed the basic setup! You will now begin to see traces from your LLM modules logged directly to the console.
 
 
 ## Exporting Traces to Langtrace
 
 To configure trace exporting, you have two options:
 
 You'll need a Langtrace `api_key`, which can be acquired by logging into your Langtrace account.
 
-1. Direct Initialization: Utilize `langtrace.init({ api_key: <YOUR_API_KEY>})`.
+1. Direct Initialization: Utilize `langtrace.init(api_key=<YOUR_API_KEY>)`.
 2. Environment Variables: Set `LANGTRACE_API_KEY`, then add `langtrace.init()` at the beginning of your file.
 
 ### Additional Customization
 
 - `@with_langtrace_root_span` - this decorator is designed to organize and relate different spans, in a hierarchical manner. When you're performing multiple operations that you want to monitor together as a unit, this function helps by establishing a "parent" (`LangtraceRootSpan` or whatever is passed to `name`) span. Then, any calls to the LLM APIs made within the given function (fn) will be considered "children" of this parent span. This setup is especially useful for tracking the performance or behavior of a group of operations collectively, rather than individually.
 
 ```python
```

### Comparing `langtrace_python_sdk-1.2.8/pyproject.toml` & `langtrace_python_sdk-1.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-1.2.8/PKG-INFO` & `langtrace_python_sdk-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -56,25 +56,25 @@
 ## Getting Started
 
 To begin utilizing Langtrace, follow these straightforward steps:
 
 1. Install the package using `pip install langtrace-python-sdk`.
 2. Incorporate Langtrace into your project with `from langtrace_python_sdk import langtrace`.
    - This import should precede any other LLM module imports (such as OpenAI, LlamaIndex, etc.) to ensure proper functionality.
-3. Initialize Langtrace by adding `langtrace.init({ write_to_remote_url: false})` to your code.
+3. Initialize Langtrace by adding `langtrace.init(write_to_langtrace_cloud=false)` to your code.
 4. Congratulations, you've completed the basic setup! You will now begin to see traces from your LLM modules logged directly to the console.
 
 
 ## Exporting Traces to Langtrace
 
 To configure trace exporting, you have two options:
 
 You'll need a Langtrace `api_key`, which can be acquired by logging into your Langtrace account.
 
-1. Direct Initialization: Utilize `langtrace.init({ api_key: <YOUR_API_KEY>})`.
+1. Direct Initialization: Utilize `langtrace.init(api_key=<YOUR_API_KEY>)`.
 2. Environment Variables: Set `LANGTRACE_API_KEY`, then add `langtrace.init()` at the beginning of your file.
 
 ### Additional Customization
 
 - `@with_langtrace_root_span` - this decorator is designed to organize and relate different spans, in a hierarchical manner. When you're performing multiple operations that you want to monitor together as a unit, this function helps by establishing a "parent" (`LangtraceRootSpan` or whatever is passed to `name`) span. Then, any calls to the LLM APIs made within the given function (fn) will be considered "children" of this parent span. This setup is especially useful for tracking the performance or behavior of a group of operations collectively, rather than individually.
 
 ```python
```

