# Comparing `tmp/gpt_all_star-0.0.7.tar.gz` & `tmp/gpt_all_star-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_all_star-0.0.7.tar", max compression
+gzip compressed data, was "gpt_all_star-0.0.9.tar", max compression
```

## Comparing `gpt_all_star-0.0.7.tar` & `gpt_all_star-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0     1067 2024-03-07 14:59:22.669755 gpt_all_star-0.0.7/LICENSE
--rw-r--r--   0        0        0     6745 2024-03-07 14:59:22.669755 gpt_all_star-0.0.7/README.md
--rw-r--r--   0        0        0      408 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/__init__.py
--rw-r--r--   0        0        0     2195 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/agents.yml
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/cli/__init__.py
--rw-r--r--   0        0        0     2669 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/cli/console_terminal.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/__init__.py
--rw-r--r--   0        0        0    10388 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/agent.py
--rw-r--r--   0        0        0      226 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/agent_state.py
--rw-r--r--   0        0        0      951 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/agents.py
--rw-r--r--   0        0        0      394 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/architect.py
--rw-r--r--   0        0        0    14971 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/chain.py
--rw-r--r--   0        0        0     5581 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/copilot.py
--rw-r--r--   0        0        0      392 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/designer.py
--rw-r--r--   0        0        0      428 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/engineer.py
--rw-r--r--   0        0        0      437 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/product_owner.py
--rw-r--r--   0        0        0      441 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/project_manager.py
--rw-r--r--   0        0        0      433 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/agents/qa_engineer.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/deployment/__init__.py
--rw-r--r--   0        0        0     2098 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/deployment/deployment.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/execution/__init__.py
--rw-r--r--   0        0        0     1820 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/execution/execution.py
--rw-r--r--   0        0        0      340 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/gpt_all_star.py
--rw-r--r--   0        0        0      608 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/implement_prompt.py
--rw-r--r--   0        0        0      561 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/message.py
--rw-r--r--   0        0        0     8724 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/project.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/development/__init__.py
--rw-r--r--   0        0        0     2766 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/development/additional_tasks.py
--rw-r--r--   0        0        0     1143 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/development/development.py
--rw-r--r--   0        0        0     2421 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/development/nodejs_tasks.py
--rw-r--r--   0        0        0      708 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/development/planning_prompt.py
--rw-r--r--   0        0        0      867 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/development/replanning_prompt.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/entrypoint/__init__.py
--rw-r--r--   0        0        0      861 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/entrypoint/entrypoint.py
--rw-r--r--   0        0        0      688 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/entrypoint/planning_prompt.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/healing/__init__.py
--rw-r--r--   0        0        0      970 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/healing/healing.py
--rw-r--r--   0        0        0      381 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/healing/planning_prompt.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/improvement/__init__.py
--rw-r--r--   0        0        0     1046 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/improvement/improvement.py
--rw-r--r--   0        0        0      386 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/improvement/planning_prompt.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/specification/__init__.py
--rw-r--r--   0        0        0     1677 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/specification/additional_tasks.py
--rw-r--r--   0        0        0     1385 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/specification/specification.py
--rw-r--r--   0        0        0      767 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/step.py
--rw-r--r--   0        0        0     1364 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/steps.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/system_design/__init__.py
--rw-r--r--   0        0        0     2088 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/system_design/additional_tasks.py
--rw-r--r--   0        0        0      825 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/system_design/system_design.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/ui_design/__init__.py
--rw-r--r--   0        0        0      718 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/ui_design/planning_prompt.py
--rw-r--r--   0        0        0      976 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/steps/ui_design/ui_design.py
--rw-r--r--   0        0        0     3528 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/storage.py
--rw-r--r--   0        0        0    11078 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/team.py
--rw-r--r--   0        0        0      692 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/token.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/tools/__init__.py
--rw-r--r--   0        0        0     4640 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/tools/document_chunker.py
--rw-r--r--   0        0        0     2375 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/tools/file_tool.py
--rw-r--r--   0        0        0     1442 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/tools/llama_index_tool.py
--rw-r--r--   0        0        0     4681 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/core/tools/shell_tool.py
--rw-r--r--   0        0        0        0 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/helper/__init__.py
--rw-r--r--   0        0        0      204 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/helper/config_loader.py
--rw-r--r--   0        0        0     4221 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/helper/git.py
--rw-r--r--   0        0        0     1873 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/helper/multi_agent_collaboration_graph.py
--rw-r--r--   0        0        0      327 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/helper/text_parser.py
--rw-r--r--   0        0        0     1610 2024-03-07 14:59:22.673755 gpt_all_star-0.0.7/gpt_all_star/main.py
--rw-r--r--   0        0        0     1887 2024-03-07 14:59:22.677755 gpt_all_star-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8318 1970-01-01 00:00:00.000000 gpt_all_star-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6745 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/README.md
+-rw-r--r--   0        0        0      408 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/__init__.py
+-rw-r--r--   0        0        0     2195 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/agents.yml
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/cli/__init__.py
+-rw-r--r--   0        0        0     2669 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/cli/console_terminal.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/__init__.py
+-rw-r--r--   0        0        0    10701 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/agent.py
+-rw-r--r--   0        0        0      226 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/agent_state.py
+-rw-r--r--   0        0        0      951 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/agents.py
+-rw-r--r--   0        0        0      394 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/architect.py
+-rw-r--r--   0        0        0    14971 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/chain.py
+-rw-r--r--   0        0        0     5931 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/copilot.py
+-rw-r--r--   0        0        0      392 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/designer.py
+-rw-r--r--   0        0        0      428 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/engineer.py
+-rw-r--r--   0        0        0      437 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/product_owner.py
+-rw-r--r--   0        0        0      441 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/project_manager.py
+-rw-r--r--   0        0        0      433 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/agents/qa_engineer.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/deployment/__init__.py
+-rw-r--r--   0        0        0     2408 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/deployment/deployment.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/execution/__init__.py
+-rw-r--r--   0        0        0     1953 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/execution/execution.py
+-rw-r--r--   0        0        0      340 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/gpt_all_star.py
+-rw-r--r--   0        0        0      608 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/implement_prompt.py
+-rw-r--r--   0        0        0      561 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/message.py
+-rw-r--r--   0        0        0     9280 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/project.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/development/__init__.py
+-rw-r--r--   0        0        0     2766 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/development/additional_tasks.py
+-rw-r--r--   0        0        0     1170 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/development/development.py
+-rw-r--r--   0        0        0     2421 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/development/nodejs_tasks.py
+-rw-r--r--   0        0        0      708 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/development/planning_prompt.py
+-rw-r--r--   0        0        0      867 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/development/replanning_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/entrypoint/__init__.py
+-rw-r--r--   0        0        0      919 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/entrypoint/entrypoint.py
+-rw-r--r--   0        0        0      688 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/entrypoint/planning_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/healing/__init__.py
+-rw-r--r--   0        0        0     1047 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/healing/healing.py
+-rw-r--r--   0        0        0      381 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/healing/planning_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/improvement/__init__.py
+-rw-r--r--   0        0        0     1081 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/improvement/improvement.py
+-rw-r--r--   0        0        0      386 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/improvement/planning_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/specification/__init__.py
+-rw-r--r--   0        0        0     1677 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/specification/additional_tasks.py
+-rw-r--r--   0        0        0     1523 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/specification/specification.py
+-rw-r--r--   0        0        0      909 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/step.py
+-rw-r--r--   0        0        0     1364 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/steps.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/system_design/__init__.py
+-rw-r--r--   0        0        0     2088 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/system_design/additional_tasks.py
+-rw-r--r--   0        0        0      852 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/system_design/system_design.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/ui_design/__init__.py
+-rw-r--r--   0        0        0      718 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/ui_design/planning_prompt.py
+-rw-r--r--   0        0        0     1003 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/steps/ui_design/ui_design.py
+-rw-r--r--   0        0        0     3528 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/storage.py
+-rw-r--r--   0        0        0    11383 2024-03-16 02:57:02.235835 gpt_all_star-0.0.9/gpt_all_star/core/team.py
+-rw-r--r--   0        0        0      692 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/core/token.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/core/tools/__init__.py
+-rw-r--r--   0        0        0     4640 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/core/tools/document_chunker.py
+-rw-r--r--   0        0        0     2375 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/core/tools/file_tool.py
+-rw-r--r--   0        0        0     1442 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/core/tools/llama_index_tool.py
+-rw-r--r--   0        0        0     4681 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/core/tools/shell_tool.py
+-rw-r--r--   0        0        0        0 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/helper/__init__.py
+-rw-r--r--   0        0        0      204 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/helper/config_loader.py
+-rw-r--r--   0        0        0     4221 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/helper/git.py
+-rw-r--r--   0        0        0     1873 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/helper/multi_agent_collaboration_graph.py
+-rw-r--r--   0        0        0      327 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/helper/text_parser.py
+-rw-r--r--   0        0        0      750 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/helper/translator.py
+-rw-r--r--   0        0        0     4443 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/locales/ja_JP/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     6110 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/locales/ja_JP/ja.po
+-rw-r--r--   0        0        0     1610 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/gpt_all_star/main.py
+-rw-r--r--   0        0        0     1887 2024-03-16 02:57:02.239835 gpt_all_star-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8318 1970-01-01 00:00:00.000000 gpt_all_star-0.0.9/PKG-INFO
```

### Comparing `gpt_all_star-0.0.7/LICENSE` & `gpt_all_star-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/README.md` & `gpt_all_star-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/agents.yml` & `gpt_all_star-0.0.9/gpt_all_star/agents.yml`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/cli/console_terminal.py` & `gpt_all_star-0.0.9/gpt_all_star/cli/console_terminal.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/agents/agent.py` & `gpt_all_star-0.0.9/gpt_all_star/core/agents/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from rich.panel import Panel
 from rich.table import Table
 
 from gpt_all_star.cli.console_terminal import ConsoleTerminal
 from gpt_all_star.core.message import Message
 from gpt_all_star.core.storage import Storages
 from gpt_all_star.core.tools.shell_tool import ShellTool
+from gpt_all_star.helper.translator import create_translator
 
 # from gpt_all_star.core.tools.llama_index_tool import llama_index_tool
 
 NEXT_COMMAND = "next"
 
 
 class Agent(ABC):
@@ -39,14 +40,15 @@
         role: AgentRole,
         storages: Storages | None,
         debug_mode: bool = False,
         name: str | None = None,
         profile: str | None = None,
         color: str | None = None,
         tools: list = [],
+        language: str | None = None,
     ) -> None:
         self.console = ConsoleTerminal()
         self._llm = _create_llm(os.getenv("OPENAI_API_MODEL_NAME"), 0.1)
 
         self.role: AgentRole = role
         self.name: str = name or self._get_default_profile().name
         self.profile: str = profile or self._get_default_profile().prompt.format()
@@ -58,14 +60,20 @@
         self.additional_tools = tools
         self.set_executor(
             working_directory=(
                 self.storages.root.path.absolute() if self.storages else os.getcwd()
             )
         )
 
+        self._set_language(language)
+        self._ = create_translator(self.language)
+
+    def _set_language(self, language: str | None) -> None:
+        self.language = language if language is not None else "en"
+
     def set_executor(self, working_directory: str) -> None:
         file_tools = FileManagementToolkit(
             root_dir=str(working_directory),
             selected_tools=["read_file", "write_file", "list_directory", "file_delete"],
         ).get_tools()
         self.tools = (
             self.additional_tools
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/agents/agents.py` & `gpt_all_star-0.0.9/gpt_all_star/core/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/agents/chain.py` & `gpt_all_star-0.0.9/gpt_all_star/core/agents/chain.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/agents/copilot.py` & `gpt_all_star-0.0.9/gpt_all_star/core/agents/copilot.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,47 +7,52 @@
 import requests
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 
 from gpt_all_star.core.agents.agent import Agent, AgentRole
 from gpt_all_star.core.storage import Storages
 from gpt_all_star.helper.config_loader import load_configuration
+from gpt_all_star.helper.translator import create_translator
 
 APP_TYPES = ["Client-Side Web Application", "Full-Stack Web Application"]
 
 
 class Copilot(Agent):
     def __init__(
         self,
         storages: Storages | None = None,
         debug_mode: bool = False,
         name: str | None = None,
         profile: str | None = None,
+        language: str | None = None,
     ) -> None:
-        super().__init__(AgentRole.COPILOT, storages, debug_mode, name, profile)
+        super().__init__(
+            AgentRole.COPILOT, storages, debug_mode, name, profile, language=language
+        )
+        self._ = create_translator(language)
 
     def start(self, project_name: str) -> None:
-        self.state(f"Let's start the project! ({project_name})")
+        self.state(self._("Let's start the project! (%s)") % project_name)
 
     def finish(self, project_name: str) -> None:
-        self.state(f"Completed the project! ({project_name})")
+        self.state(self._("Completed the project! (%s)") % project_name)
 
     def ask_project_name(self) -> str:
         default_project_name = "".join(
             random.choice(string.ascii_letters + string.digits) for i in range(15)
         )
         project_name = self.ask(
-            "What is the name of the project?",
+            self._("What is the name of the project?"),
             is_required=False,
             default=default_project_name,
         )
         return project_name
 
     def confirm(self, confirmation: str) -> bool:
-        CONFIRM_CHOICES = ["yes", "no"]
+        CONFIRM_CHOICES = [self._("yes"), self._("no")]
         choice = self.present_choices(
             confirmation,
             CONFIRM_CHOICES,
             default=1,
         )
         return choice == CONFIRM_CHOICES[0]
 
@@ -58,36 +63,40 @@
 
     def get_instructions(self) -> str:
         instructions = self.load_instructions()
         instruction = instructions.get("instruction")
         if instruction:
             return instruction
         return self.ask(
-            "What application do you want to build? Please describe it in as much detail as possible."
+            self._(
+                "What application do you want to build? Please describe it in as much detail as possible."
+            )
         )
 
     def get_app_type(self) -> str:
         instructions = self.load_instructions()
         app_type = instructions.get("app_type")
         if app_type:
             return app_type
         return self.present_choices(
-            "What type of application do you want to build?",
+            self._("What type of application do you want to build?"),
             APP_TYPES,
             default=1,
         )
 
     def caution(self, command: str) -> None:
-        self.state(f"Executing command: {command}")
+        self.state(self._("Executing command: %s") % command)
         self.state(
-            "If it does not work as expected, please consider running the code"
-            + " in another way than above."
+            self._(
+                "If it does not work as expected, please consider running the code"
+                + " in another way than above."
+            )
         )
         self.console.print(
-            "You can press ctrl+c *once* to stop the execution.", style="red"
+            self._("You can press ctrl+c *once* to stop the execution."), style="red"
         )
 
     def run_command(self, command: str) -> None:
         try:
             process = subprocess.Popen(
                 command,
                 shell=True,
@@ -141,15 +150,15 @@
             try:
                 response = requests.get("http://localhost:3000")
                 if response.status_code == 200:
                     return True
             except requests.ConnectionError:
                 pass
             time.sleep(1)
-        self.state("Unable to confirm server startup")
+        self.state(self._("Unable to confirm server startup"))
         return False
 
     def _check_browser_errors(self):
         """Access the site with a headless browser and catch console errors"""
         chrome_options = Options()
         chrome_options.add_argument("--headless")
         driver = webdriver.Chrome(options=chrome_options)
@@ -161,8 +170,8 @@
                 self.console.print(f"Error: {entry['message']}", style="red")
                 errors += f"{entry['message']}\n"
         driver.quit()
         if errors:
             raise Exception({"browser errors": errors})
 
     def _handle_keyboard_interrupt(self) -> None:
-        self.state("Execution stopped.")
+        self.state(self._("Execution stopped."))
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/deployment/deployment.py` & `gpt_all_star-0.0.9/gpt_all_star/core/deployment/deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from rich.syntax import Syntax
 
 from gpt_all_star.core.agents.chain import Chain
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.message import Message
 from gpt_all_star.helper.git import Git
+from gpt_all_star.helper.translator import create_translator
 
 
 class Deployment:
-    def __init__(
-        self,
-        copilot: Copilot,
-    ) -> None:
+    def __init__(self, copilot: Copilot, japanese_mode: bool) -> None:
         self.copilot = copilot
+        self._ = create_translator("ja" if japanese_mode else "en")
+
+    def _set_language(self, language: str | None) -> None:
+        self.language = language if language is not None else "en"
 
     def run(self) -> None:
         git = Git(self.copilot.storages.root.path)
         files_to_add = git.files()
         if not files_to_add:
-            self.copilot.state("No files to add to the repository.")
+            self.copilot.state(self._("No files to add to the repository."))
             return
 
-        self.copilot.state("The following diff will be pushed to the repository")
+        self.copilot.state(
+            self._("The following diff will be pushed to the repository")
+        )
         syntax = Syntax(git.diffs(), "diff", theme="monokai", line_numbers=True)
         self.copilot.console.print(syntax)
 
         commit_info = (
             Chain()
             .create_git_commit_message_chain()
             .invoke(
@@ -48,15 +52,15 @@
                         )
                     ],
                 }
             )
         )
 
         self.copilot.console.new_lines()
-        self.copilot.state("Pushing to the repository...")
+        self.copilot.state(self._("Pushing to the repository..."))
         try:
             branch_name = (
                 commit_info["branch"]
                 if git.check_local_main_branch_exists()
                 else "main"
             )
             is_main_branch = branch_name == "main"
@@ -68,9 +72,9 @@
             git.commit(commit_info["message"])
             git.push()
 
             if not is_main_branch:
                 git.create_pull_request(branch_name)
         except Exception as e:
             self.copilot.state(
-                f"An error occurred while pushing to the repository: {str(e)}"
+                self._("An error occurred while pushing to the repository: %s") % str(e)
             )
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/execution/execution.py` & `gpt_all_star-0.0.9/gpt_all_star/core/execution/execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from gpt_all_star.core.agents.chain import Chain
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.message import Message
 from gpt_all_star.core.steps.healing.healing import Healing
 from gpt_all_star.core.team import Team
+from gpt_all_star.helper.translator import create_translator
 
 
 class Execution:
-    def __init__(
-        self,
-        team: Team,
-        copilot: Copilot,
-    ) -> None:
+    def __init__(self, team: Team, copilot: Copilot, japanese_mode: bool) -> None:
         self.team = team
         self.copilot = copilot
         self.working_directory = self.copilot.storages.app.path.absolute()
+        self._ = create_translator("ja" if japanese_mode else "en")
 
     def run(self) -> None:
         command = (
             Chain()
             .create_command_to_execute_application_chain()
             .invoke(
                 {
@@ -41,15 +39,15 @@
                     ],
                 }
             )
         )
         self.copilot.caution(command["command"])
         MAX_ATTEMPTS = 5
         for attempt in range(MAX_ATTEMPTS):
-            self.copilot.state(f"Attempt {attempt + 1}/{MAX_ATTEMPTS}")
+            self.copilot.state(self._("Attempt %d/%d") % (attempt + 1, MAX_ATTEMPTS))
             try:
                 self.copilot.run_command(command["command"])
             except KeyboardInterrupt:
                 break
             except Exception as e:
                 healing = Healing(copilot=self.copilot, error_message=e)
                 self.team.run(healing)
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/implement_prompt.py` & `gpt_all_star-0.0.9/gpt_all_star/core/implement_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/message.py` & `gpt_all_star-0.0.9/gpt_all_star/core/message.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/project.py` & `gpt_all_star-0.0.9/gpt_all_star/core/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,36 +20,39 @@
 from gpt_all_star.core.steps.specification.specification import Specification
 from gpt_all_star.core.steps.steps import STEPS, StepType
 from gpt_all_star.core.storage import Storage, Storages
 from gpt_all_star.core.team import Team
 from gpt_all_star.helper.multi_agent_collaboration_graph import (
     MultiAgentCollaborationGraph,
 )
+from gpt_all_star.helper.translator import create_translator
 
 
 class Project:
     def __init__(
         self,
         step: StepType = StepType.DEFAULT,
         project_name: str = None,
         japanese_mode: bool = False,
         review_mode: bool = False,
         debug_mode: bool = False,
         plan_and_solve: bool = False,
     ) -> None:
-        self.copilot = Copilot()
+        self.copilot = Copilot(language="ja" if japanese_mode else "en")
         self.start_time = None
         self.plan_and_solve = plan_and_solve
         self._set_modes(japanese_mode, review_mode, debug_mode)
         self._set_project_name(project_name)
         self._set_storages()
         self._set_copilot()
         self._set_agents()
         self._set_step_type(step)
 
+        self._ = create_translator("ja" if japanese_mode else "en")
+
     def _set_modes(
         self, japanese_mode: bool, review_mode: bool, debug_mode: bool
     ) -> None:
         self.japanese_mode = japanese_mode
         self.review_mode = review_mode
         self.debug_mode = debug_mode
 
@@ -83,76 +86,82 @@
             ),
         )
 
     def _set_step_type(self, step: StepType) -> None:
         self.step_type = step or StepType.DEFAULT
         if self.step_type is StepType.DEFAULT:
             if self.debug_mode:
-                self.copilot.state("Archiving previous results...")
+                self.copilot.state(self._("Archiving previous results..."))
             self.storages.archive_storage()
 
     def _execute_steps(self) -> None:
         try:
             for step in STEPS[self.step_type]:
                 self._execute_step(step)
         except KeyboardInterrupt:
-            self.copilot.state("Interrupt received! Stopping...")
+            self.copilot.state(self._("Interrupt received! Stopping..."))
 
     def _execute_step(self, step) -> None:
         MAX_RETRIES = 5
         retries = 0
         success = False
         while retries < MAX_RETRIES and not success:
             try:
-                result = self.team.run(step(self.copilot))
+                result = self.team.run(
+                    step(self.copilot, japanese_mode=self.japanese_mode)
+                )
                 if result:
                     success = True
                 else:
                     self.copilot.state(
-                        f"Retrying step {step} (Attempt {retries + 1}/{MAX_RETRIES})"
+                        self._("Retrying step %d (Attempt %d/%d)")
+                        % (step, retries + 1, MAX_RETRIES)
                     )
                     retries += 1
             except Exception as e:
-                self.copilot.state(f"Failed to execute step {step}. Reason: {str(e)}")
+                self.copilot.state(
+                    self._("Failed to execute step %d. Reason: %s") % (step, str(e))
+                )
                 raise e
 
         if not success:
+            failed_message = "Failed to successfully complete step %(step)d after %(max_retries)d attempts."
             self.copilot.state(
-                f"Failed to successfully complete step {step} after {MAX_RETRIES} attempts."
+                self._(failed_message) % {"step": step, "max_retries": MAX_RETRIES}
             )
             raise Exception(f"Operation failed after {MAX_RETRIES} retries.")
 
     def start(self) -> None:
         self.start_time = time.time()
         self.copilot.start(self.project_name)
         self.team = Team(
             copilot=self.copilot,
             members=self.agents,
             japanese_mode=self.japanese_mode,
             plan_and_solve=self.plan_and_solve,
         )
         self._execute_steps()
         if bool(os.listdir(self.storages.app.path.absolute())):
-            if self.copilot.confirm("Do you want to execute this application?"):
-                Execution(self.team, self.copilot).run()
+            if self.copilot.confirm(self._("Do you want to execute this application?")):
+                Execution(self.team, self.copilot, self.japanese_mode).run()
         if (
             os.environ.get("GITHUB_ORG")
             and os.environ.get("GITHUB_TOKEN")
             and self.copilot.confirm(
-                "Do you want to manage this application code with GitHub?"
+                self._("Do you want to manage this application code with GitHub?")
             )
         ):
-            Deployment(self.copilot).run()
+            Deployment(self.copilot, self.japanese_mode).run()
 
     def chat(self, message: str) -> None:
         for step in STEPS[self.step_type]:
-            step = step(self.copilot, display=False)
+            step = step(self.copilot, display=False, japanese_mode=self.japanese_mode)
             if step.__class__ is Specification:
                 step.instructions = message
-                step.app_type = "Client-Side Web Application"
+                step.app_type = self._("Client-Side Web Application")
             supervisor_name = (
                 Chain()
                 .create_assign_supervisor_chain(members=self.agents.to_array())
                 .invoke(
                     {"messages": [Message.create_human_message(step.planning_prompt())]}
                 )
                 .get("assign")
@@ -211,10 +220,10 @@
                 tasks["plan"].pop(0)
 
     def finish(self) -> None:
         if self.start_time:
             end_time = time.time()
             elapsed_time = end_time - self.start_time
             self.copilot.state(
-                f"Project finished. Elapsed time: {elapsed_time:.2f} seconds."
+                self._("Project finished. Elapsed time: %.2f seconds.") % elapsed_time
             )
         self.copilot.finish(self.project_name)
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/development/additional_tasks.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/development/additional_tasks.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/development/development.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/development/development.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from gpt_all_star.core.steps.development.nodejs_tasks import nodejs_tasks
 from gpt_all_star.core.steps.development.planning_prompt import planning_prompt_template
 from gpt_all_star.core.steps.step import Step
 
 
 class Development(Step):
     def __init__(
-        self,
-        copilot: Copilot,
-        display: bool = True,
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
     ) -> None:
-        super().__init__(copilot, display)
+        super().__init__(copilot, display, japanese_mode)
         self.working_directory = self.copilot.storages.app.path.absolute()
         self.plan_and_solve = True
 
     def planning_prompt(self) -> str:
         planning_prompt = planning_prompt_template.format(
             specifications=self.copilot.storages.docs.get("specifications.md", "N/A"),
             technologies=self.copilot.storages.docs.get("technologies.md", "N/A"),
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/development/nodejs_tasks.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/development/nodejs_tasks.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/development/planning_prompt.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/development/planning_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/development/replanning_prompt.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/development/replanning_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/entrypoint/entrypoint.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/entrypoint/entrypoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.steps.entrypoint.planning_prompt import planning_prompt_template
 from gpt_all_star.core.steps.step import Step
 
 
 class Entrypoint(Step):
-    def __init__(self, copilot: Copilot, display: bool = True) -> None:
-        super().__init__(copilot, display)
+    def __init__(
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
+    ) -> None:
+        super().__init__(copilot, display, japanese_mode)
         self.working_directory = self.copilot.storages.app.path.absolute()
 
     def planning_prompt(self) -> str:
         planning_prompt = planning_prompt_template.format(
             current_source_code=self.copilot.storages.current_source_code(
                 debug_mode=self.copilot.debug_mode
             ),
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/entrypoint/planning_prompt.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/entrypoint/planning_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/healing/healing.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/healing/healing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.steps.healing.planning_prompt import planning_prompt_template
 from gpt_all_star.core.steps.step import Step
 
 
 class Healing(Step):
     def __init__(
-        self, copilot: Copilot, error_message: str, display: bool = True
+        self,
+        copilot: Copilot,
+        error_message: str,
+        display: bool = True,
+        japanese_mode: bool = False,
     ) -> None:
-        super().__init__(copilot, display)
+        super().__init__(copilot, display, japanese_mode)
         self.error_message = error_message
         self.working_directory = self.copilot.storages.app.path.absolute()
 
     def planning_prompt(self) -> str:
         planning_prompt = planning_prompt_template.format(
             error=self.error_message,
             current_source_code=self.copilot.storages.current_source_code(
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/improvement/improvement.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/improvement/improvement.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.steps.improvement.planning_prompt import planning_prompt_template
 from gpt_all_star.core.steps.step import Step
 
 
 class Improvement(Step):
     def __init__(
-        self,
-        copilot: Copilot,
-        display: bool = True,
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
     ) -> None:
-        super().__init__(copilot, display)
+        super().__init__(copilot, display, japanese_mode)
         self.working_directory = self.copilot.storages.app.path.absolute()
 
     def planning_prompt(self) -> str:
         request = self.copilot.ask(
-            "What would you like to update?", is_required=True, default=None
+            self._("What would you like to update?"), is_required=True, default=None
         )
         planning_prompt = planning_prompt_template.format(
             request=request,
             current_source_code=self.copilot.storages.current_source_code(
                 debug_mode=self.copilot.debug_mode
             ),
         )
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/specification/additional_tasks.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/specification/additional_tasks.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/specification/specification.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/specification/specification.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,44 +3,46 @@
     create_additional_tasks,
 )
 from gpt_all_star.core.steps.step import Step
 
 
 class Specification(Step):
     def __init__(
-        self,
-        copilot: Copilot,
-        display: bool = True,
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
     ) -> None:
-        super().__init__(copilot, display)
+        super().__init__(copilot, display, japanese_mode)
         self.working_directory = self.copilot.storages.docs.path.absolute()
         self.instructions = ""
         self.app_type = ""
+        self.japanese_mode = japanese_mode
 
     def planning_prompt(self) -> str:
         return ""
 
     def additional_tasks(self) -> list:
         instructions = (
             self.copilot.get_instructions()
             if self.instructions == ""
             else self.instructions
         )
         app_type = self.copilot.get_app_type() if self.app_type == "" else self.app_type
         if self.display:
             self.copilot.state(
-                f"""
+                self._(
+                    """
 Ok, we have a instruction and app type now!
 ---
 instruction:
-{instructions}
+%s
 app_type:
-{app_type}
+%s
 ---
 """,
+                )
+                % (instructions, app_type)
             )
         return create_additional_tasks(app_type, instructions)
 
     def callback(self) -> bool:
         specifications = self.copilot.storages.docs.get("specifications.md")
         has_specifications = bool(specifications)
         if has_specifications:
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/step.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from abc import ABC, abstractmethod
 
 from gpt_all_star.core.agents.copilot import Copilot
+from gpt_all_star.helper.translator import create_translator
 
 
 class Step(ABC):
     def __init__(
-        self,
-        copilot: Copilot,
-        display: bool = True,
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
     ) -> None:
         self.copilot = copilot
         self.working_directory = self.copilot.storages.root.path.absolute()
         self.plan_and_solve = False
         self.exclude_dirs = [".archive", "node_modules", "build"]
         self.display = display
 
         if self.display:
             self.copilot.console.section(f"STEP: {self.__class__.__name__}")
 
+        self._ = create_translator("ja" if japanese_mode else "en")
+
     @abstractmethod
     def planning_prompt(self) -> str:
         pass
 
     @abstractmethod
     def additional_tasks(self) -> list:
         pass
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/steps.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/steps.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/system_design/additional_tasks.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/system_design/additional_tasks.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/system_design/system_design.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/system_design/system_design.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.steps.step import Step
 from gpt_all_star.core.steps.system_design.additional_tasks import additional_tasks
 
 
 class SystemDesign(Step):
     def __init__(
-        self,
-        copilot: Copilot,
-        display: bool = True,
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
     ) -> None:
-        super().__init__(copilot, display)
+        super().__init__(copilot, display, japanese_mode)
         self.working_directory = self.copilot.storages.docs.path.absolute()
 
     def planning_prompt(self) -> str:
         return ""
 
     def additional_tasks(self) -> list:
         return additional_tasks
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/ui_design/planning_prompt.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/ui_design/planning_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/steps/ui_design/ui_design.py` & `gpt_all_star-0.0.9/gpt_all_star/core/steps/ui_design/ui_design.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from gpt_all_star.core.agents.copilot import Copilot
 from gpt_all_star.core.steps.step import Step
 from gpt_all_star.core.steps.ui_design.planning_prompt import planning_prompt_template
 
 
 class UIDesign(Step):
     def __init__(
-        self,
-        copilot: Copilot,
-        display: bool = True,
+        self, copilot: Copilot, display: bool = True, japanese_mode: bool = False
     ) -> None:
-        super().__init__(copilot, display)
+        super().__init__(copilot, display, japanese_mode)
         self.working_directory = self.copilot.storages.app.path.absolute()
 
     def planning_prompt(self) -> str:
         planning_prompt = planning_prompt_template.format(
             current_source_code=self.copilot.storages.current_source_code(
                 debug_mode=self.copilot.debug_mode
             ),
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/storage.py` & `gpt_all_star-0.0.9/gpt_all_star/core/storage.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/team.py` & `gpt_all_star-0.0.9/gpt_all_star/core/team.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from gpt_all_star.core.steps.step import Step
 from gpt_all_star.helper.config_loader import load_configuration
 from gpt_all_star.helper.multi_agent_collaboration_graph import (
     SUPERVISOR_NAME,
     MultiAgentCollaborationGraph,
 )
 from gpt_all_star.helper.text_parser import TextParser
+from gpt_all_star.helper.translator import create_translator
 
 
 class Team:
     def __init__(
         self,
         copilot: Copilot,
         members: Agents,
@@ -33,30 +34,31 @@
         self.japanese_mode = japanese_mode
         self.plan_and_solve = plan_and_solve
         self.agents = members
         self.copilot = copilot
         self.console = self.copilot.console.console
         self._graph: Optional[MultiAgentCollaborationGraph] = None
         self.supervisor = None
+        self._ = create_translator("ja" if japanese_mode else "en")
         self._initialize_team()
 
     def _initialize_team(self):
-        self.copilot.state("Let's start by building a team!")
+        self.copilot.state(self._("Let's start by building a team!"))
         self._introduce_agents()
-        self.copilot.state("Ok, we have a team now!")
+        self.copilot.state(self._("Ok, we have a team now!"))
         self._display_team_members()
 
     def _assign_supervisor(self, planning_prompt: str | None):
         supervisor_name = (
             Chain()
             .create_assign_supervisor_chain(members=self.agents.to_array())
             .invoke({"messages": [Message.create_human_message(planning_prompt)]})
             .get("assign")
         )
-        self.copilot.state(f"Supervisor assignment: {supervisor_name}.")
+        self.copilot.state(self._("Supervisor assignment: %s.") % supervisor_name)
         supervisor = self.agents.get_agent_by_name(supervisor_name)
         self._graph = MultiAgentCollaborationGraph(supervisor, self.agents.to_array())
         self.supervisor = supervisor
 
     def _execute(self, messages: list[Message]):
         try:
             for output in self._graph.workflow.stream(
@@ -65,15 +67,15 @@
             ):
                 for key, value in output.items():
                     if key == SUPERVISOR_NAME or key == "__end__":
                         if self.supervisor.debug_mode:
                             self.supervisor.state(value)
                     else:
                         self.agents.get_agent_by_name(key).state(
-                            "  ┗ I am in charge of it."
+                            self._("  ┗ I am in charge of it.")
                         )
                         if self.supervisor.debug_mode:
                             latest_message = value.get("messages")[-1].content.strip()
                             self.supervisor.console.print(
                                 f"""
 {key}:
 ---
@@ -96,15 +98,15 @@
             console=self.console,
             spinner="runner",
             speed=0.5,
         ):
             if not self._graph:
                 self._assign_supervisor(planning_prompt)
 
-            self.supervisor.state("Planning tasks.")
+            self.supervisor.state(self._("Planning tasks."))
             tasks = (
                 Chain()
                 .create_planning_chain(self.supervisor.profile)
                 .invoke(
                     {
                         "messages": [Message.create_human_message(planning_prompt)],
                     }
@@ -130,21 +132,24 @@
                 if task["action"] == ACTIONS[0]:
                     todo = f"{task['action']}: {task['command']} in the directory({task.get('working_directory', '')})"
                 else:
                     todo = f"{task['action']}: {task.get('working_directory', '')}/{task.get('filename', '')}"
 
                 if self.supervisor.debug_mode:
                     self.supervisor.state(
-                        f"""\n
-Task: {todo}
-Context: {task['context']}
-Objective: {task['objective']}
-Reason: {task['reason']}
+                        self._(
+                            """\n
+Task: %s
+Context: %s
+Objective: %s
+Reason: %s
 ---
 """
+                        )
+                        % (todo, task["context"], task["objective"], task["reason"])
                     )
                 else:
                     self.supervisor.state(f"({count}/{original_tasks_count}) {todo}")
 
                 message = Message.create_human_message(
                     implement_template.format(
                         task=todo,
@@ -212,15 +217,15 @@
         self._run(planning_prompt, additional_tasks, step.plan_and_solve)
 
         return step.callback()
 
     def _introduce_agents(self) -> None:
         agents_list = load_configuration("./gpt_all_star/agents.yml")
         if agents_list:
-            self.copilot.state("Loading members from `agent.yml`...")
+            self.copilot.state(self._("Loading members from `agent.yml`..."))
             for agent_info in agents_list:
                 self._set_agent_attributes(agent_info)
         else:
             self._introduce_agents_manually()
 
     def _set_agent_attributes(self, agent_info: dict) -> None:
         agent = getattr(self.agents, agent_info["role"])
@@ -236,30 +241,30 @@
 
     def _introduce_agents_manually(self) -> None:
         for role in AgentRole:
             if role is not AgentRole.COPILOT:
                 self._introduce_agent(getattr(self.agents, role.value), role)
 
     def _introduce_agent(self, agent: Agent, role: AgentRole) -> None:
-        self.copilot.state(f"Please introduce the {role.name}.")
+        self.copilot.state(self._("Please introduce the %s.") % role.name)
         self._ask_agent_name(agent, role)
         self._ask_agent_profile(agent, role)
         self._add_instructions_to_profile(agent)
         agent.messages = [Message.create_system_message(agent.profile)]
 
     def _ask_agent_name(self, agent: Agent, role: AgentRole) -> None:
         agent.name = self.copilot.ask(
-            f"What is the name of the {role.name}?",
+            self._("What is the name of the %s?") % role.name,
             is_required=False,
             default=agent.name,
         )
 
     def _ask_agent_profile(self, agent: Agent, role: AgentRole) -> None:
         agent.profile = self.copilot.ask(
-            f"What is the profile of the {role.name}?",
+            self._("What is the profile of the %s?") % role.name,
             is_required=False,
             default=agent.profile,
         )
 
     def _display_team_members(self) -> None:
         table = Table(
             show_header=True, header_style=f"{MAIN_COLOR}", title="Team Members"
```

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/token.py` & `gpt_all_star-0.0.9/gpt_all_star/core/token.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/tools/document_chunker.py` & `gpt_all_star-0.0.9/gpt_all_star/core/tools/document_chunker.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/tools/file_tool.py` & `gpt_all_star-0.0.9/gpt_all_star/core/tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/tools/llama_index_tool.py` & `gpt_all_star-0.0.9/gpt_all_star/core/tools/llama_index_tool.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/core/tools/shell_tool.py` & `gpt_all_star-0.0.9/gpt_all_star/core/tools/shell_tool.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/helper/git.py` & `gpt_all_star-0.0.9/gpt_all_star/helper/git.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/helper/multi_agent_collaboration_graph.py` & `gpt_all_star-0.0.9/gpt_all_star/helper/multi_agent_collaboration_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/gpt_all_star/main.py` & `gpt_all_star-0.0.9/gpt_all_star/main.py`

 * *Files identical despite different names*

### Comparing `gpt_all_star-0.0.7/pyproject.toml` & `gpt_all_star-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-all-star"
-version = "0.0.7"
+version = "0.0.9"
 description = "AI-powered code generation tool for scratch development of web applications with a team collaboration of autonomous AI agents. This is a research-project, and its primary value is to explore the possibility of autonomous AI agents."
 authors = ["Yuya Kakui <y.kakui@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 Repository = "https://github.com/kyaukyuai/gpt-all-star"
@@ -21,20 +21,20 @@
 termcolor = "^2.4.0"
 gitpython = "^3.1.41"
 requests = "^2.31.0"
 typer = "^0.9.0"
 pyfiglet = "^1.0.2"
 langchain-openai = "^0.0.8"
 selenium = "^4.17.2"
-langgraph = "^0.0.26"
-langchain-experimental = "^0.0.53"
+langgraph = "^0.0.28"
+langchain-experimental = "^0.0.54"
 llama-index = "^0.10.0"
 tree-sitter-languages = "^1.10.2"
 pygithub = "^2.2.0"
-uvicorn = "^0.27.1"
+uvicorn = "^0.28.0"
 fastapi = "^0.110.0"
 
 [tool.poetry.scripts]
 gpt-all-star = 'gpt_all_star.main:app'
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.1.1"
```

### Comparing `gpt_all_star-0.0.7/PKG-INFO` & `gpt_all_star-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: gpt-all-star
-Version: 0.0.7
+Version: 0.0.9
 Summary: AI-powered code generation tool for scratch development of web applications with a team collaboration of autonomous AI agents. This is a research-project, and its primary value is to explore the possibility of autonomous AI agents.
 License: MIT
 Author: Yuya Kakui
 Author-email: y.kakui@gmail.com
 Requires-Python: >=3.10.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: gitpython (>=3.1.41,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: langchain (>=0.1.0,<0.2.0)
-Requires-Dist: langchain-experimental (>=0.0.53,<0.0.54)
+Requires-Dist: langchain-experimental (>=0.0.54,<0.0.55)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
-Requires-Dist: langgraph (>=0.0.26,<0.0.27)
+Requires-Dist: langgraph (>=0.0.28,<0.0.29)
 Requires-Dist: llama-index (>=0.10.0,<0.11.0)
 Requires-Dist: openai (>=1.6.1,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: pyfiglet (>=1.0.2,<2.0.0)
 Requires-Dist: pygithub (>=2.2.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: selenium (>=4.17.2,<5.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Requires-Dist: tree-sitter-languages (>=1.10.2,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: uvicorn (>=0.27.1,<0.28.0)
+Requires-Dist: uvicorn (>=0.28.0,<0.29.0)
 Project-URL: Repository, https://github.com/kyaukyuai/gpt-all-star
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img width="628" alt="gpt-all-star" src="https://github.com/kyaukyuai/gpt-all-star/assets/1140707/dc46fbf4-16f9-4989-801d-7df65af0c696">
 
 [![PyPI](https://img.shields.io/pypi/v/gpt-all-star.svg)](https://pypi.org/project/gpt-all-star/) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
```

