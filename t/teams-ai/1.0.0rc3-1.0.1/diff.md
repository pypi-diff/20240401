# Comparing `tmp/teams_ai-1.0.0rc3.tar.gz` & `tmp/teams_ai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teams_ai-1.0.0rc3.tar", max compression
+gzip compressed data, was "teams_ai-1.0.1.tar", max compression
```

## Comparing `teams_ai-1.0.0rc3.tar` & `teams_ai-1.0.1.tar`

### file list

```diff
@@ -1,168 +1,169 @@
--rw-r--r--   0        0        0     1093 2024-02-28 17:27:33.896122 teams_ai-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0     1735 2024-03-04 22:28:36.337236 teams_ai-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0      913 2024-02-28 17:27:33.903101 teams_ai-1.0.0rc3/README.md
--rw-r--r--   0        0        0      644 2024-02-28 17:27:33.921639 teams_ai-1.0.0rc3/teams/__init__.py
--rw-r--r--   0        0        0      963 2024-02-28 17:27:33.922639 teams_ai-1.0.0rc3/teams/activity_type.py
--rw-r--r--   0        0        0      385 2024-02-28 17:27:33.932364 teams_ai-1.0.0rc3/teams/adaptive_cards/__init__.py
--rw-r--r--   0        0        0    10716 2024-02-28 17:27:33.940894 teams_ai-1.0.0rc3/teams/adaptive_cards/adaptive_cards.py
--rw-r--r--   0        0        0      471 2024-02-28 17:27:33.941901 teams_ai-1.0.0rc3/teams/adaptive_cards/adaptive_cards_options.py
--rw-r--r--   0        0        0      252 2024-02-28 17:27:33.941901 teams_ai-1.0.0rc3/teams/adaptive_cards/adaptive_cards_search_params.py
--rw-r--r--   0        0        0      245 2024-02-28 17:27:33.942826 teams_ai-1.0.0rc3/teams/adaptive_cards/adaptive_cards_search_result.py
--rw-r--r--   0        0        0      183 2024-02-28 17:27:33.942826 teams_ai-1.0.0rc3/teams/ai/__init__.py
--rw-r--r--   0        0        0      321 2024-02-28 17:27:33.943872 teams_ai-1.0.0rc3/teams/ai/actions/__init__.py
--rw-r--r--   0        0        0     1001 2024-02-28 17:27:33.950724 teams_ai-1.0.0rc3/teams/ai/actions/action_entry.py
--rw-r--r--   0        0        0      641 2024-02-28 17:27:33.950724 teams_ai-1.0.0rc3/teams/ai/actions/action_turn_context.py
--rw-r--r--   0        0        0      462 2024-02-28 17:27:33.951724 teams_ai-1.0.0rc3/teams/ai/actions/action_types.py
--rw-r--r--   0        0        0     8703 2024-03-04 19:10:38.237856 teams_ai-1.0.0rc3/teams/ai/ai.py
--rw-r--r--   0        0        0      767 2024-02-28 17:27:33.958725 teams_ai-1.0.0rc3/teams/ai/ai_options.py
--rw-r--r--   0        0        0      425 2024-02-28 17:27:33.959629 teams_ai-1.0.0rc3/teams/ai/augmentations/__init__.py
--rw-r--r--   0        0        0     1635 2024-03-04 19:10:38.243854 teams_ai-1.0.0rc3/teams/ai/augmentations/augmentation.py
--rw-r--r--   0        0        0     2554 2024-03-04 19:10:38.249089 teams_ai-1.0.0rc3/teams/ai/augmentations/default_augmentation.py
--rw-r--r--   0        0        0     9234 2024-03-04 19:10:38.255088 teams_ai-1.0.0rc3/teams/ai/augmentations/monologue_augmentation.py
--rw-r--r--   0        0        0     7071 2024-03-04 19:10:38.262051 teams_ai-1.0.0rc3/teams/ai/augmentations/sequence_augmentation.py
--rw-r--r--   0        0        0      196 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/clients/__init__.py
--rw-r--r--   0        0        0     7230 2024-03-04 19:10:38.267267 teams_ai-1.0.0rc3/teams/ai/clients/llm_client.py
--rw-r--r--   0        0        0      224 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/data_sources/__init__.py
--rw-r--r--   0        0        0     1360 2024-03-04 19:10:38.273303 teams_ai-1.0.0rc3/teams/ai/data_sources/data_source.py
--rw-r--r--   0        0        0     2500 2024-03-04 19:10:38.279346 teams_ai-1.0.0rc3/teams/ai/data_sources/text_data_source.py
--rw-r--r--   0        0        0      624 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/embeddings/__init__.py
--rw-r--r--   0        0        0     4409 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/embeddings/azure_openai_embeddings.py
--rw-r--r--   0        0        0     1048 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/embeddings/azure_openai_embeddings_options.py
--rw-r--r--   0        0        0      894 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/embeddings/embeddings_model.py
--rw-r--r--   0        0        0      802 2024-02-28 17:27:33.962205 teams_ai-1.0.0rc3/teams/ai/embeddings/embeddings_response.py
--rw-r--r--   0        0        0     3803 2024-02-28 17:27:33.968740 teams_ai-1.0.0rc3/teams/ai/embeddings/openai_embeddings.py
--rw-r--r--   0        0        0      991 2024-02-28 17:27:33.968740 teams_ai-1.0.0rc3/teams/ai/embeddings/openai_embeddings_options.py
--rw-r--r--   0        0        0      562 2024-02-28 17:27:33.968740 teams_ai-1.0.0rc3/teams/ai/models/__init__.py
--rw-r--r--   0        0        0      729 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/models/chat_completion_action.py
--rw-r--r--   0        0        0     7123 2024-03-04 19:10:38.285350 teams_ai-1.0.0rc3/teams/ai/models/openai_model.py
--rw-r--r--   0        0        0     1302 2024-03-04 19:10:38.291151 teams_ai-1.0.0rc3/teams/ai/models/prompt_completion_model.py
--rw-r--r--   0        0        0      909 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/models/prompt_response.py
--rw-r--r--   0        0        0      557 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/moderators/__init__.py
--rw-r--r--   0        0        0     1743 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/moderators/azure_content_safety_moderator.py
--rw-r--r--   0        0        0      656 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/moderators/default_moderator.py
--rw-r--r--   0        0        0     1589 2024-03-04 19:10:38.297196 teams_ai-1.0.0rc3/teams/ai/moderators/moderator.py
--rw-r--r--   0        0        0     4332 2024-03-04 19:10:38.303162 teams_ai-1.0.0rc3/teams/ai/moderators/openai_moderator.py
--rw-r--r--   0        0        0      521 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/planners/__init__.py
--rw-r--r--   0        0        0     6057 2024-03-04 19:10:38.309390 teams_ai-1.0.0rc3/teams/ai/planners/action_planner.py
--rw-r--r--   0        0        0     2085 2024-02-29 18:07:09.525392 teams_ai-1.0.0rc3/teams/ai/planners/plan.py
--rw-r--r--   0        0        0      967 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/planners/planner.py
--rw-r--r--   0        0        0     1476 2024-02-28 17:27:33.969778 teams_ai-1.0.0rc3/teams/ai/prompts/__init__.py
--rw-r--r--   0        0        0      846 2024-02-28 17:27:33.975341 teams_ai-1.0.0rc3/teams/ai/prompts/assistant_message.py
--rw-r--r--   0        0        0     1066 2024-02-28 17:27:33.975782 teams_ai-1.0.0rc3/teams/ai/prompts/augmentation_config.py
--rw-r--r--   0        0        0     3285 2024-02-28 17:27:33.976301 teams_ai-1.0.0rc3/teams/ai/prompts/completion_config.py
--rw-r--r--   0        0        0      428 2024-02-28 17:27:33.976301 teams_ai-1.0.0rc3/teams/ai/prompts/function_call.py
--rw-r--r--   0        0        0     2992 2024-03-04 19:10:38.315390 teams_ai-1.0.0rc3/teams/ai/prompts/function_call_message.py
--rw-r--r--   0        0        0     3137 2024-03-04 19:10:38.321390 teams_ai-1.0.0rc3/teams/ai/prompts/function_response_message.py
--rw-r--r--   0        0        0     1511 2024-02-28 17:27:33.977950 teams_ai-1.0.0rc3/teams/ai/prompts/message.py
--rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.978714 teams_ai-1.0.0rc3/teams/ai/prompts/prompt.py
--rw-r--r--   0        0        0     2493 2024-03-04 19:10:38.326426 teams_ai-1.0.0rc3/teams/ai/prompts/prompt_functions.py
--rw-r--r--   0        0        0    14609 2024-03-04 19:10:38.332764 teams_ai-1.0.0rc3/teams/ai/prompts/prompt_manager.py
--rw-r--r--   0        0        0     1571 2024-02-28 17:27:33.986946 teams_ai-1.0.0rc3/teams/ai/prompts/prompt_manager_options.py
--rw-r--r--   0        0        0      478 2024-02-28 17:27:33.986946 teams_ai-1.0.0rc3/teams/ai/prompts/prompt_section_layout.py
--rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.988031 teams_ai-1.0.0rc3/teams/ai/prompts/prompt_template.py
--rw-r--r--   0        0        0     2116 2024-02-28 17:27:33.988538 teams_ai-1.0.0rc3/teams/ai/prompts/prompt_template_config.py
--rw-r--r--   0        0        0      614 2024-02-28 17:27:33.988538 teams_ai-1.0.0rc3/teams/ai/prompts/rendered_prompt_section.py
--rw-r--r--   0        0        0      800 2024-02-28 17:27:33.989546 teams_ai-1.0.0rc3/teams/ai/prompts/sections/__init__.py
--rw-r--r--   0        0        0     4108 2024-03-04 19:10:38.339727 teams_ai-1.0.0rc3/teams/ai/prompts/sections/action_augmentation_section.py
--rw-r--r--   0        0        0     6894 2024-03-04 19:10:38.345727 teams_ai-1.0.0rc3/teams/ai/prompts/sections/conversation_history_section.py
--rw-r--r--   0        0        0     2451 2024-03-04 19:10:38.351007 teams_ai-1.0.0rc3/teams/ai/prompts/sections/data_source_section.py
--rw-r--r--   0        0        0     3361 2024-03-04 19:10:38.357972 teams_ai-1.0.0rc3/teams/ai/prompts/sections/group_section.py
--rw-r--r--   0        0        0     9245 2024-03-04 19:10:38.363971 teams_ai-1.0.0rc3/teams/ai/prompts/sections/layout_engine_section.py
--rw-r--r--   0        0        0     2941 2024-03-04 19:10:38.370157 teams_ai-1.0.0rc3/teams/ai/prompts/sections/prompt_section.py
--rw-r--r--   0        0        0     7305 2024-03-04 19:10:38.376193 teams_ai-1.0.0rc3/teams/ai/prompts/sections/prompt_section_base.py
--rw-r--r--   0        0        0     9006 2024-03-04 19:10:38.382234 teams_ai-1.0.0rc3/teams/ai/prompts/sections/template_section.py
--rw-r--r--   0        0        0     3124 2024-03-04 19:10:38.388234 teams_ai-1.0.0rc3/teams/ai/prompts/sections/text_section.py
--rw-r--r--   0        0        0      635 2024-02-28 17:27:33.994231 teams_ai-1.0.0rc3/teams/ai/prompts/system_message.py
--rw-r--r--   0        0        0     4028 2024-03-04 19:10:38.394784 teams_ai-1.0.0rc3/teams/ai/prompts/user_input_message.py
--rw-r--r--   0        0        0      800 2024-02-28 17:27:33.996243 teams_ai-1.0.0rc3/teams/ai/prompts/user_message.py
--rw-r--r--   0        0        0      213 2024-02-28 17:27:33.997052 teams_ai-1.0.0rc3/teams/ai/tokenizers/__init__.py
--rw-r--r--   0        0        0     1071 2024-02-28 17:27:33.998562 teams_ai-1.0.0rc3/teams/ai/tokenizers/gpt_tokenizer.py
--rw-r--r--   0        0        0      993 2024-02-28 17:27:33.999575 teams_ai-1.0.0rc3/teams/ai/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     1436 2024-03-04 19:10:38.399820 teams_ai-1.0.0rc3/teams/ai/utilities.py
--rw-r--r--   0        0        0      621 2024-02-28 17:27:34.000614 teams_ai-1.0.0rc3/teams/ai/validators/__init__.py
--rw-r--r--   0        0        0     4284 2024-03-04 19:10:38.405822 teams_ai-1.0.0rc3/teams/ai/validators/action_response_validator.py
--rw-r--r--   0        0        0      777 2024-03-04 19:10:38.411023 teams_ai-1.0.0rc3/teams/ai/validators/default_response_validator.py
--rw-r--r--   0        0        0     3045 2024-03-04 19:10:38.417058 teams_ai-1.0.0rc3/teams/ai/validators/json_response_validator.py
--rw-r--r--   0        0        0     1286 2024-03-04 19:10:38.423061 teams_ai-1.0.0rc3/teams/ai/validators/prompt_response_validator.py
--rw-r--r--   0        0        0      648 2024-02-28 17:27:34.002010 teams_ai-1.0.0rc3/teams/ai/validators/validation.py
--rw-r--r--   0        0        0    24013 2024-03-04 19:10:38.429023 teams_ai-1.0.0rc3/teams/app.py
--rw-r--r--   0        0        0      296 2024-02-28 17:27:34.013515 teams_ai-1.0.0rc3/teams/app_error.py
--rw-r--r--   0        0        0     2433 2024-02-28 17:27:34.019518 teams_ai-1.0.0rc3/teams/app_options.py
--rw-r--r--   0        0        0      566 2024-02-28 17:27:34.020527 teams_ai-1.0.0rc3/teams/input_file.py
--rw-r--r--   0        0        0      154 2024-02-28 17:27:34.020845 teams_ai-1.0.0rc3/teams/meetings/__init__.py
--rw-r--r--   0        0        0     3653 2024-02-28 17:27:34.028331 teams_ai-1.0.0rc3/teams/meetings/meetings.py
--rw-r--r--   0        0        0      228 2024-02-28 17:27:34.029400 teams_ai-1.0.0rc3/teams/message_extensions/__init__.py
--rw-r--r--   0        0        0    24283 2024-02-28 17:27:34.039795 teams_ai-1.0.0rc3/teams/message_extensions/message_extensions.py
--rw-r--r--   0        0        0      241 2024-02-28 17:27:34.039795 teams_ai-1.0.0rc3/teams/message_reaction_types.py
--rw-r--r--   0        0        0        0 2024-02-28 17:27:34.039795 teams_ai-1.0.0rc3/teams/py.typed
--rw-r--r--   0        0        0      328 2024-02-28 17:27:34.041095 teams_ai-1.0.0rc3/teams/query.py
--rw-r--r--   0        0        0      762 2024-02-28 17:27:34.049441 teams_ai-1.0.0rc3/teams/route.py
--rw-r--r--   0        0        0      512 2024-03-04 19:10:38.436267 teams_ai-1.0.0rc3/teams/state/__init__.py
--rw-r--r--   0        0        0     1373 2024-03-04 19:10:38.442230 teams_ai-1.0.0rc3/teams/state/conversation_state.py
--rw-r--r--   0        0        0     3481 2024-03-04 19:10:38.447269 teams_ai-1.0.0rc3/teams/state/memory.py
--rw-r--r--   0        0        0     4230 2024-03-04 19:10:38.453524 teams_ai-1.0.0rc3/teams/state/state.py
--rw-r--r--   0        0        0     1118 2024-03-04 19:10:38.458550 teams_ai-1.0.0rc3/teams/state/temp_state.py
--rw-r--r--   0        0        0      732 2024-03-04 19:10:38.463524 teams_ai-1.0.0rc3/teams/state/todict.py
--rw-r--r--   0        0        0     2478 2024-03-04 22:28:06.315751 teams_ai-1.0.0rc3/teams/state/turn_state.py
--rw-r--r--   0        0        0     1314 2024-03-04 19:10:38.469569 teams_ai-1.0.0rc3/teams/state/user_state.py
--rw-r--r--   0        0        0      239 2024-02-28 17:27:34.059743 teams_ai-1.0.0rc3/teams/task_modules/__init__.py
--rw-r--r--   0        0        0     6458 2024-02-28 17:27:34.070570 teams_ai-1.0.0rc3/teams/task_modules/task_modules.py
--rw-r--r--   0        0        0      488 2024-02-28 17:27:34.071531 teams_ai-1.0.0rc3/teams/task_modules/task_modules_options.py
--rw-r--r--   0        0        0     3813 2024-02-28 17:27:34.071531 teams_ai-1.0.0rc3/teams/teams_adapter.py
--rw-r--r--   0        0        0     1190 2024-02-28 17:27:34.072531 teams_ai-1.0.0rc3/teams/typing.py
--rw-r--r--   0        0        0      292 2024-02-28 17:27:34.072531 teams_ai-1.0.0rc3/teams/user_agent.py
--rw-r--r--   0        0        0      200 2024-02-28 17:27:34.073532 teams_ai-1.0.0rc3/teams/utils/json/__init__.py
--rw-r--r--   0        0        0      620 2024-02-28 17:27:34.073532 teams_ai-1.0.0rc3/teams/utils/json/parse.py
--rw-r--r--   0        0        0     1747 2024-02-28 17:27:34.074530 teams_ai-1.0.0rc3/teams/utils/json/parse_object.py
--rw-r--r--   0        0        0     4967 2024-02-28 17:27:34.074530 teams_ai-1.0.0rc3/tests/adaptive_cards/test_adaptive_cards.py
--rw-r--r--   0        0        0     2746 2024-02-28 17:27:34.075531 teams_ai-1.0.0rc3/tests/ai/augmentations/test_default_augmentation.py
--rw-r--r--   0        0        0     6483 2024-02-28 17:27:34.075531 teams_ai-1.0.0rc3/tests/ai/augmentations/test_monologue_augmentation.py
--rw-r--r--   0        0        0     7587 2024-03-04 19:10:38.474809 teams_ai-1.0.0rc3/tests/ai/augmentations/test_sequence_augmentation.py
--rw-r--r--   0        0        0     1502 2024-02-28 17:27:34.077308 teams_ai-1.0.0rc3/tests/ai/data_sources/test_text_data_source.py
--rw-r--r--   0        0        0     6184 2024-02-28 17:27:34.077308 teams_ai-1.0.0rc3/tests/ai/embeddings/test_azure_openai_embeddings.py
--rw-r--r--   0        0        0     5296 2024-02-28 17:27:34.078204 teams_ai-1.0.0rc3/tests/ai/embeddings/test_openai_embeddings.py
--rw-r--r--   0        0        0     5006 2024-02-28 17:27:34.078742 teams_ai-1.0.0rc3/tests/ai/models/test_openai_model.py
--rw-r--r--   0        0        0    10196 2024-03-04 19:10:38.480811 teams_ai-1.0.0rc3/tests/ai/moderators/test_azure_content_safety_moderator.py
--rw-r--r--   0        0        0      828 2024-02-28 17:27:34.079758 teams_ai-1.0.0rc3/tests/ai/moderators/test_default_moderator.py
--rw-r--r--   0        0        0     9480 2024-03-04 19:10:38.486811 teams_ai-1.0.0rc3/tests/ai/moderators/test_openai_moderator.py
--rw-r--r--   0        0        0      692 2024-02-28 17:27:34.081309 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/happy_path/actions.json
--rw-r--r--   0        0        0      587 2024-02-28 17:27:34.081309 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/happy_path/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/happy_path/skprompt.txt
--rw-r--r--   0        0        0      614 2024-02-28 17:27:34.082314 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/include_images/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/include_images/skprompt.txt
--rw-r--r--   0        0        0      366 2024-02-28 17:27:34.083314 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/migrate_old_schema/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.083314 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/migrate_old_schema/skprompt.txt
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.084313 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/no_config/skprompt.txt
--rw-r--r--   0        0        0      582 2024-02-28 17:27:34.084313 teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/no_prompt/config.json
--rw-r--r--   0        0        0     1164 2024-02-28 17:27:34.085314 teams_ai-1.0.0rc3/tests/ai/prompts/test_assistant_message.py
--rw-r--r--   0        0        0     7157 2024-03-04 19:10:38.492599 teams_ai-1.0.0rc3/tests/ai/prompts/test_conversation_history.py
--rw-r--r--   0        0        0     1560 2024-02-28 17:27:34.085423 teams_ai-1.0.0rc3/tests/ai/prompts/test_data_source_section.py
--rw-r--r--   0        0        0     2175 2024-02-28 17:27:34.085423 teams_ai-1.0.0rc3/tests/ai/prompts/test_function_call_message.py
--rw-r--r--   0        0        0     2221 2024-02-28 17:27:34.086488 teams_ai-1.0.0rc3/tests/ai/prompts/test_function_response_message.py
--rw-r--r--   0        0        0     2807 2024-02-28 17:27:34.086488 teams_ai-1.0.0rc3/tests/ai/prompts/test_group_section.py
--rw-r--r--   0        0        0     6968 2024-02-28 17:27:34.086488 teams_ai-1.0.0rc3/tests/ai/prompts/test_layout_engine.py
--rw-r--r--   0        0        0     9570 2024-03-04 19:10:38.498635 teams_ai-1.0.0rc3/tests/ai/prompts/test_prompt_manager_v2.py
--rw-r--r--   0        0        0     8405 2024-02-28 17:27:34.087490 teams_ai-1.0.0rc3/tests/ai/prompts/test_prompt_section_base.py
--rw-r--r--   0        0        0     1056 2024-02-28 17:27:34.087490 teams_ai-1.0.0rc3/tests/ai/prompts/test_system_message.py
--rw-r--r--   0        0        0     9290 2024-03-04 19:10:38.503635 teams_ai-1.0.0rc3/tests/ai/prompts/test_template_section.py
--rw-r--r--   0        0        0     2319 2024-02-28 17:27:34.088994 teams_ai-1.0.0rc3/tests/ai/prompts/test_text_section.py
--rw-r--r--   0        0        0     7349 2024-03-04 19:10:38.509640 teams_ai-1.0.0rc3/tests/ai/prompts/test_user_input_message.py
--rw-r--r--   0        0        0     1048 2024-02-28 17:27:34.089504 teams_ai-1.0.0rc3/tests/ai/prompts/test_user_message.py
--rw-r--r--   0        0        0     1457 2024-02-28 17:27:34.089504 teams_ai-1.0.0rc3/tests/ai/test_utilities.py
--rw-r--r--   0        0        0      853 2024-02-28 17:27:34.089504 teams_ai-1.0.0rc3/tests/ai/tokenizers/test_gpt_tokenizer.py
--rw-r--r--   0        0        0     6169 2024-02-28 17:27:34.090510 teams_ai-1.0.0rc3/tests/ai/validators/test_action_response_validator.py
--rw-r--r--   0        0        0      822 2024-02-28 17:27:34.090510 teams_ai-1.0.0rc3/tests/ai/validators/test_default_response_validator.py
--rw-r--r--   0        0        0     5196 2024-02-28 17:27:34.091510 teams_ai-1.0.0rc3/tests/ai/validators/test_json_response_validator.py
--rw-r--r--   0        0        0     4144 2024-03-04 22:28:06.315751 teams_ai-1.0.0rc3/tests/state/test_conversation_state.py
--rw-r--r--   0        0        0     6119 2024-03-04 19:10:38.514847 teams_ai-1.0.0rc3/tests/state/test_custom_turn_state.py
--rw-r--r--   0        0        0     1797 2024-03-04 22:28:06.330899 teams_ai-1.0.0rc3/tests/state/test_temp_state.py
--rw-r--r--   0        0        0     6510 2024-03-04 22:28:06.338955 teams_ai-1.0.0rc3/tests/state/test_turn_state.py
--rw-r--r--   0        0        0     3692 2024-03-04 22:28:06.344899 teams_ai-1.0.0rc3/tests/state/test_user_state.py
--rw-r--r--   0        0        0     2251 2024-02-28 17:27:34.094112 teams_ai-1.0.0rc3/tests/task_modules/test_task_modules.py
--rw-r--r--   0        0        0    29183 2024-02-28 17:27:34.095113 teams_ai-1.0.0rc3/tests/test_app.py
--rw-r--r--   0        0        0    11702 2024-02-28 17:27:34.096123 teams_ai-1.0.0rc3/tests/test_meetings.py
--rw-r--r--   0        0        0    32052 2024-02-28 17:27:34.106581 teams_ai-1.0.0rc3/tests/test_message_extensions.py
--rw-r--r--   0        0        0      146 2024-02-28 17:27:34.106581 teams_ai-1.0.0rc3/tests/utils/__init__.py
--rw-r--r--   0        0        0      526 2024-02-28 17:27:34.107578 teams_ai-1.0.0rc3/tests/utils/activity.py
--rw-r--r--   0        0        0     1055 2024-02-28 17:27:34.107578 teams_ai-1.0.0rc3/tests/utils/adapter.py
--rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 teams_ai-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-28 17:27:33.896122 teams_ai-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-01 19:58:49.301616 teams_ai-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      913 2024-02-28 17:27:33.903101 teams_ai-1.0.1/README.md
+-rw-r--r--   0        0        0      644 2024-02-28 17:27:33.921639 teams_ai-1.0.1/teams/__init__.py
+-rw-r--r--   0        0        0      963 2024-02-28 17:27:33.922639 teams_ai-1.0.1/teams/activity_type.py
+-rw-r--r--   0        0        0      386 2024-04-01 15:45:21.915342 teams_ai-1.0.1/teams/adaptive_cards/__init__.py
+-rw-r--r--   0        0        0    10814 2024-04-01 15:45:21.926346 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards.py
+-rw-r--r--   0        0        0      471 2024-02-28 17:27:33.941901 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards_options.py
+-rw-r--r--   0        0        0      252 2024-02-28 17:27:33.941901 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards_search_params.py
+-rw-r--r--   0        0        0      344 2024-03-26 18:27:31.042285 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards_search_result.py
+-rw-r--r--   0        0        0      183 2024-02-28 17:27:33.942826 teams_ai-1.0.1/teams/ai/__init__.py
+-rw-r--r--   0        0        0      321 2024-02-28 17:27:33.943872 teams_ai-1.0.1/teams/ai/actions/__init__.py
+-rw-r--r--   0        0        0     1001 2024-02-28 17:27:33.950724 teams_ai-1.0.1/teams/ai/actions/action_entry.py
+-rw-r--r--   0        0        0      641 2024-02-28 17:27:33.950724 teams_ai-1.0.1/teams/ai/actions/action_turn_context.py
+-rw-r--r--   0        0        0      502 2024-04-01 15:45:21.927348 teams_ai-1.0.1/teams/ai/actions/action_types.py
+-rw-r--r--   0        0        0     9105 2024-04-01 15:45:21.935879 teams_ai-1.0.1/teams/ai/ai.py
+-rw-r--r--   0        0        0      903 2024-04-01 15:45:21.942863 teams_ai-1.0.1/teams/ai/ai_options.py
+-rw-r--r--   0        0        0      425 2024-02-28 17:27:33.959629 teams_ai-1.0.1/teams/ai/augmentations/__init__.py
+-rw-r--r--   0        0        0     1635 2024-03-04 19:10:38.243854 teams_ai-1.0.1/teams/ai/augmentations/augmentation.py
+-rw-r--r--   0        0        0     2554 2024-03-04 19:10:38.249089 teams_ai-1.0.1/teams/ai/augmentations/default_augmentation.py
+-rw-r--r--   0        0        0     9793 2024-03-27 21:04:22.729223 teams_ai-1.0.1/teams/ai/augmentations/monologue_augmentation.py
+-rw-r--r--   0        0        0     7071 2024-03-04 19:10:38.262051 teams_ai-1.0.1/teams/ai/augmentations/sequence_augmentation.py
+-rw-r--r--   0        0        0      196 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/clients/__init__.py
+-rw-r--r--   0        0        0     7230 2024-03-04 19:10:38.267267 teams_ai-1.0.1/teams/ai/clients/llm_client.py
+-rw-r--r--   0        0        0      224 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/data_sources/__init__.py
+-rw-r--r--   0        0        0     1360 2024-03-04 19:10:38.273303 teams_ai-1.0.1/teams/ai/data_sources/data_source.py
+-rw-r--r--   0        0        0     2500 2024-03-04 19:10:38.279346 teams_ai-1.0.1/teams/ai/data_sources/text_data_source.py
+-rw-r--r--   0        0        0      625 2024-04-01 15:45:21.948864 teams_ai-1.0.1/teams/ai/embeddings/__init__.py
+-rw-r--r--   0        0        0     4409 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings.py
+-rw-r--r--   0        0        0     1048 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings_options.py
+-rw-r--r--   0        0        0      894 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/embeddings_model.py
+-rw-r--r--   0        0        0      802 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/embeddings_response.py
+-rw-r--r--   0        0        0     3803 2024-02-28 17:27:33.968740 teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings.py
+-rw-r--r--   0        0        0      991 2024-02-28 17:27:33.968740 teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings_options.py
+-rw-r--r--   0        0        0      562 2024-02-28 17:27:33.968740 teams_ai-1.0.1/teams/ai/models/__init__.py
+-rw-r--r--   0        0        0      729 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/models/chat_completion_action.py
+-rw-r--r--   0        0        0     7123 2024-03-04 19:10:38.285350 teams_ai-1.0.1/teams/ai/models/openai_model.py
+-rw-r--r--   0        0        0     1302 2024-03-04 19:10:38.291151 teams_ai-1.0.1/teams/ai/models/prompt_completion_model.py
+-rw-r--r--   0        0        0      909 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/models/prompt_response.py
+-rw-r--r--   0        0        0      557 2024-03-05 21:42:08.164469 teams_ai-1.0.1/teams/ai/moderators/__init__.py
+-rw-r--r--   0        0        0     7695 2024-03-26 18:27:31.059067 teams_ai-1.0.1/teams/ai/moderators/azure_content_safety_moderator.py
+-rw-r--r--   0        0        0      656 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/moderators/default_moderator.py
+-rw-r--r--   0        0        0     1589 2024-03-04 19:10:38.297196 teams_ai-1.0.1/teams/ai/moderators/moderator.py
+-rw-r--r--   0        0        0     4332 2024-03-05 21:41:32.156765 teams_ai-1.0.1/teams/ai/moderators/openai_moderator.py
+-rw-r--r--   0        0        0      654 2024-04-01 15:45:21.950878 teams_ai-1.0.1/teams/ai/planners/__init__.py
+-rw-r--r--   0        0        0     6127 2024-04-01 15:45:21.959862 teams_ai-1.0.1/teams/ai/planners/action_planner.py
+-rw-r--r--   0        0        0    14445 2024-04-01 15:45:21.966864 teams_ai-1.0.1/teams/ai/planners/assistants_planner.py
+-rw-r--r--   0        0        0     2085 2024-02-29 18:07:09.525392 teams_ai-1.0.1/teams/ai/planners/plan.py
+-rw-r--r--   0        0        0     1065 2024-04-01 15:45:21.968867 teams_ai-1.0.1/teams/ai/planners/planner.py
+-rw-r--r--   0        0        0     1476 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/prompts/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-28 17:27:33.975341 teams_ai-1.0.1/teams/ai/prompts/assistant_message.py
+-rw-r--r--   0        0        0     1066 2024-02-28 17:27:33.975782 teams_ai-1.0.1/teams/ai/prompts/augmentation_config.py
+-rw-r--r--   0        0        0     3285 2024-02-28 17:27:33.976301 teams_ai-1.0.1/teams/ai/prompts/completion_config.py
+-rw-r--r--   0        0        0      428 2024-02-28 17:27:33.976301 teams_ai-1.0.1/teams/ai/prompts/function_call.py
+-rw-r--r--   0        0        0     2992 2024-03-04 19:10:38.315390 teams_ai-1.0.1/teams/ai/prompts/function_call_message.py
+-rw-r--r--   0        0        0     3137 2024-03-04 19:10:38.321390 teams_ai-1.0.1/teams/ai/prompts/function_response_message.py
+-rw-r--r--   0        0        0     1511 2024-02-28 17:27:33.977950 teams_ai-1.0.1/teams/ai/prompts/message.py
+-rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.978714 teams_ai-1.0.1/teams/ai/prompts/prompt.py
+-rw-r--r--   0        0        0     2493 2024-03-04 19:10:38.326426 teams_ai-1.0.1/teams/ai/prompts/prompt_functions.py
+-rw-r--r--   0        0        0    14657 2024-03-27 21:04:22.780312 teams_ai-1.0.1/teams/ai/prompts/prompt_manager.py
+-rw-r--r--   0        0        0     1571 2024-02-28 17:27:33.986946 teams_ai-1.0.1/teams/ai/prompts/prompt_manager_options.py
+-rw-r--r--   0        0        0      478 2024-02-28 17:27:33.986946 teams_ai-1.0.1/teams/ai/prompts/prompt_section_layout.py
+-rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.988031 teams_ai-1.0.1/teams/ai/prompts/prompt_template.py
+-rw-r--r--   0        0        0     2116 2024-02-28 17:27:33.988538 teams_ai-1.0.1/teams/ai/prompts/prompt_template_config.py
+-rw-r--r--   0        0        0      614 2024-02-28 17:27:33.988538 teams_ai-1.0.1/teams/ai/prompts/rendered_prompt_section.py
+-rw-r--r--   0        0        0      800 2024-02-28 17:27:33.989546 teams_ai-1.0.1/teams/ai/prompts/sections/__init__.py
+-rw-r--r--   0        0        0     4104 2024-03-27 21:04:22.804466 teams_ai-1.0.1/teams/ai/prompts/sections/action_augmentation_section.py
+-rw-r--r--   0        0        0     6894 2024-03-04 19:10:38.345727 teams_ai-1.0.1/teams/ai/prompts/sections/conversation_history_section.py
+-rw-r--r--   0        0        0     2451 2024-03-04 19:10:38.351007 teams_ai-1.0.1/teams/ai/prompts/sections/data_source_section.py
+-rw-r--r--   0        0        0     3361 2024-03-04 19:10:38.357972 teams_ai-1.0.1/teams/ai/prompts/sections/group_section.py
+-rw-r--r--   0        0        0     9245 2024-03-04 19:10:38.363971 teams_ai-1.0.1/teams/ai/prompts/sections/layout_engine_section.py
+-rw-r--r--   0        0        0     2941 2024-03-04 19:10:38.370157 teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section.py
+-rw-r--r--   0        0        0     7305 2024-03-04 19:10:38.376193 teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section_base.py
+-rw-r--r--   0        0        0     9006 2024-03-04 19:10:38.382234 teams_ai-1.0.1/teams/ai/prompts/sections/template_section.py
+-rw-r--r--   0        0        0     3124 2024-03-04 19:10:38.388234 teams_ai-1.0.1/teams/ai/prompts/sections/text_section.py
+-rw-r--r--   0        0        0      635 2024-02-28 17:27:33.994231 teams_ai-1.0.1/teams/ai/prompts/system_message.py
+-rw-r--r--   0        0        0     4028 2024-03-04 19:10:38.394784 teams_ai-1.0.1/teams/ai/prompts/user_input_message.py
+-rw-r--r--   0        0        0      800 2024-02-28 17:27:33.996243 teams_ai-1.0.1/teams/ai/prompts/user_message.py
+-rw-r--r--   0        0        0      213 2024-02-28 17:27:33.997052 teams_ai-1.0.1/teams/ai/tokenizers/__init__.py
+-rw-r--r--   0        0        0     1071 2024-02-28 17:27:33.998562 teams_ai-1.0.1/teams/ai/tokenizers/gpt_tokenizer.py
+-rw-r--r--   0        0        0      993 2024-02-28 17:27:33.999575 teams_ai-1.0.1/teams/ai/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     1436 2024-03-04 19:10:38.399820 teams_ai-1.0.1/teams/ai/utilities.py
+-rw-r--r--   0        0        0      621 2024-02-28 17:27:34.000614 teams_ai-1.0.1/teams/ai/validators/__init__.py
+-rw-r--r--   0        0        0     4284 2024-03-04 19:10:38.405822 teams_ai-1.0.1/teams/ai/validators/action_response_validator.py
+-rw-r--r--   0        0        0      777 2024-03-04 19:10:38.411023 teams_ai-1.0.1/teams/ai/validators/default_response_validator.py
+-rw-r--r--   0        0        0     3045 2024-03-26 20:05:45.109561 teams_ai-1.0.1/teams/ai/validators/json_response_validator.py
+-rw-r--r--   0        0        0     1286 2024-03-04 19:10:38.423061 teams_ai-1.0.1/teams/ai/validators/prompt_response_validator.py
+-rw-r--r--   0        0        0      648 2024-02-28 17:27:34.002010 teams_ai-1.0.1/teams/ai/validators/validation.py
+-rw-r--r--   0        0        0    24013 2024-03-04 19:10:38.429023 teams_ai-1.0.1/teams/app.py
+-rw-r--r--   0        0        0      296 2024-02-28 17:27:34.013515 teams_ai-1.0.1/teams/app_error.py
+-rw-r--r--   0        0        0     2433 2024-02-28 17:27:34.019518 teams_ai-1.0.1/teams/app_options.py
+-rw-r--r--   0        0        0      566 2024-02-28 17:27:34.020527 teams_ai-1.0.1/teams/input_file.py
+-rw-r--r--   0        0        0      154 2024-02-28 17:27:34.020845 teams_ai-1.0.1/teams/meetings/__init__.py
+-rw-r--r--   0        0        0     3653 2024-02-28 17:27:34.028331 teams_ai-1.0.1/teams/meetings/meetings.py
+-rw-r--r--   0        0        0      228 2024-02-28 17:27:34.029400 teams_ai-1.0.1/teams/message_extensions/__init__.py
+-rw-r--r--   0        0        0    24315 2024-04-01 15:45:21.976862 teams_ai-1.0.1/teams/message_extensions/message_extensions.py
+-rw-r--r--   0        0        0      241 2024-02-28 17:27:34.039795 teams_ai-1.0.1/teams/message_reaction_types.py
+-rw-r--r--   0        0        0        0 2024-02-28 17:27:34.039795 teams_ai-1.0.1/teams/py.typed
+-rw-r--r--   0        0        0      328 2024-02-28 17:27:34.041095 teams_ai-1.0.1/teams/query.py
+-rw-r--r--   0        0        0      762 2024-02-28 17:27:34.049441 teams_ai-1.0.1/teams/route.py
+-rw-r--r--   0        0        0      512 2024-03-04 19:10:38.436267 teams_ai-1.0.1/teams/state/__init__.py
+-rw-r--r--   0        0        0     1373 2024-03-04 19:10:38.442230 teams_ai-1.0.1/teams/state/conversation_state.py
+-rw-r--r--   0        0        0     3481 2024-03-04 19:10:38.447269 teams_ai-1.0.1/teams/state/memory.py
+-rw-r--r--   0        0        0     4222 2024-04-01 15:45:21.983876 teams_ai-1.0.1/teams/state/state.py
+-rw-r--r--   0        0        0     1118 2024-03-04 19:10:38.458550 teams_ai-1.0.1/teams/state/temp_state.py
+-rw-r--r--   0        0        0      732 2024-03-04 19:10:38.463524 teams_ai-1.0.1/teams/state/todict.py
+-rw-r--r--   0        0        0     2478 2024-03-26 18:27:31.059067 teams_ai-1.0.1/teams/state/turn_state.py
+-rw-r--r--   0        0        0     1314 2024-03-04 19:10:38.469569 teams_ai-1.0.1/teams/state/user_state.py
+-rw-r--r--   0        0        0      239 2024-02-28 17:27:34.059743 teams_ai-1.0.1/teams/task_modules/__init__.py
+-rw-r--r--   0        0        0     6430 2024-04-01 15:45:21.991863 teams_ai-1.0.1/teams/task_modules/task_modules.py
+-rw-r--r--   0        0        0      488 2024-02-28 17:27:34.071531 teams_ai-1.0.1/teams/task_modules/task_modules_options.py
+-rw-r--r--   0        0        0     3825 2024-04-01 19:59:26.866077 teams_ai-1.0.1/teams/teams_adapter.py
+-rw-r--r--   0        0        0     1190 2024-02-28 17:27:34.072531 teams_ai-1.0.1/teams/typing.py
+-rw-r--r--   0        0        0      292 2024-02-28 17:27:34.072531 teams_ai-1.0.1/teams/user_agent.py
+-rw-r--r--   0        0        0      200 2024-02-28 17:27:34.073532 teams_ai-1.0.1/teams/utils/json/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-27 21:04:22.850998 teams_ai-1.0.1/teams/utils/json/parse.py
+-rw-r--r--   0        0        0     1747 2024-02-28 17:27:34.074530 teams_ai-1.0.1/teams/utils/json/parse_object.py
+-rw-r--r--   0        0        0     4966 2024-04-01 15:45:22.007862 teams_ai-1.0.1/tests/adaptive_cards/test_adaptive_cards.py
+-rw-r--r--   0        0        0     2746 2024-02-28 17:27:34.075531 teams_ai-1.0.1/tests/ai/augmentations/test_default_augmentation.py
+-rw-r--r--   0        0        0     6562 2024-03-27 21:04:22.882484 teams_ai-1.0.1/tests/ai/augmentations/test_monologue_augmentation.py
+-rw-r--r--   0        0        0     7587 2024-03-04 19:10:38.474809 teams_ai-1.0.1/tests/ai/augmentations/test_sequence_augmentation.py
+-rw-r--r--   0        0        0     1502 2024-02-28 17:27:34.077308 teams_ai-1.0.1/tests/ai/data_sources/test_text_data_source.py
+-rw-r--r--   0        0        0     6111 2024-04-01 15:45:22.009865 teams_ai-1.0.1/tests/ai/embeddings/test_azure_openai_embeddings.py
+-rw-r--r--   0        0        0     5222 2024-04-01 15:45:22.009865 teams_ai-1.0.1/tests/ai/embeddings/test_openai_embeddings.py
+-rw-r--r--   0        0        0     5006 2024-02-28 17:27:34.078742 teams_ai-1.0.1/tests/ai/models/test_openai_model.py
+-rw-r--r--   0        0        0     6927 2024-03-26 18:27:31.075685 teams_ai-1.0.1/tests/ai/moderators/test_azure_content_safety_moderator.py
+-rw-r--r--   0        0        0      828 2024-02-28 17:27:34.079758 teams_ai-1.0.1/tests/ai/moderators/test_default_moderator.py
+-rw-r--r--   0        0        0     9480 2024-03-04 19:10:38.486811 teams_ai-1.0.1/tests/ai/moderators/test_openai_moderator.py
+-rw-r--r--   0        0        0      692 2024-02-28 17:27:34.081309 teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/actions.json
+-rw-r--r--   0        0        0      587 2024-02-28 17:27:34.081309 teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/skprompt.txt
+-rw-r--r--   0        0        0      614 2024-02-28 17:27:34.082314 teams_ai-1.0.1/tests/ai/prompts/test_assets/include_images/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.0.1/tests/ai/prompts/test_assets/include_images/skprompt.txt
+-rw-r--r--   0        0        0      366 2024-02-28 17:27:34.083314 teams_ai-1.0.1/tests/ai/prompts/test_assets/migrate_old_schema/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.083314 teams_ai-1.0.1/tests/ai/prompts/test_assets/migrate_old_schema/skprompt.txt
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.084313 teams_ai-1.0.1/tests/ai/prompts/test_assets/no_config/skprompt.txt
+-rw-r--r--   0        0        0      582 2024-02-28 17:27:34.084313 teams_ai-1.0.1/tests/ai/prompts/test_assets/no_prompt/config.json
+-rw-r--r--   0        0        0     1164 2024-02-28 17:27:34.085314 teams_ai-1.0.1/tests/ai/prompts/test_assistant_message.py
+-rw-r--r--   0        0        0     7157 2024-03-04 19:10:38.492599 teams_ai-1.0.1/tests/ai/prompts/test_conversation_history.py
+-rw-r--r--   0        0        0     1560 2024-02-28 17:27:34.085423 teams_ai-1.0.1/tests/ai/prompts/test_data_source_section.py
+-rw-r--r--   0        0        0     2175 2024-02-28 17:27:34.085423 teams_ai-1.0.1/tests/ai/prompts/test_function_call_message.py
+-rw-r--r--   0        0        0     2221 2024-02-28 17:27:34.086488 teams_ai-1.0.1/tests/ai/prompts/test_function_response_message.py
+-rw-r--r--   0        0        0     2807 2024-02-28 17:27:34.086488 teams_ai-1.0.1/tests/ai/prompts/test_group_section.py
+-rw-r--r--   0        0        0     6968 2024-02-28 17:27:34.086488 teams_ai-1.0.1/tests/ai/prompts/test_layout_engine.py
+-rw-r--r--   0        0        0     9570 2024-03-04 19:10:38.498635 teams_ai-1.0.1/tests/ai/prompts/test_prompt_manager_v2.py
+-rw-r--r--   0        0        0     8405 2024-02-28 17:27:34.087490 teams_ai-1.0.1/tests/ai/prompts/test_prompt_section_base.py
+-rw-r--r--   0        0        0     1056 2024-02-28 17:27:34.087490 teams_ai-1.0.1/tests/ai/prompts/test_system_message.py
+-rw-r--r--   0        0        0     9290 2024-03-04 19:10:38.503635 teams_ai-1.0.1/tests/ai/prompts/test_template_section.py
+-rw-r--r--   0        0        0     2319 2024-02-28 17:27:34.088994 teams_ai-1.0.1/tests/ai/prompts/test_text_section.py
+-rw-r--r--   0        0        0     7349 2024-03-04 19:10:38.509640 teams_ai-1.0.1/tests/ai/prompts/test_user_input_message.py
+-rw-r--r--   0        0        0     1048 2024-02-28 17:27:34.089504 teams_ai-1.0.1/tests/ai/prompts/test_user_message.py
+-rw-r--r--   0        0        0     1457 2024-02-28 17:27:34.089504 teams_ai-1.0.1/tests/ai/test_utilities.py
+-rw-r--r--   0        0        0      853 2024-02-28 17:27:34.089504 teams_ai-1.0.1/tests/ai/tokenizers/test_gpt_tokenizer.py
+-rw-r--r--   0        0        0     6169 2024-02-28 17:27:34.090510 teams_ai-1.0.1/tests/ai/validators/test_action_response_validator.py
+-rw-r--r--   0        0        0      822 2024-02-28 17:27:34.090510 teams_ai-1.0.1/tests/ai/validators/test_default_response_validator.py
+-rw-r--r--   0        0        0     5196 2024-02-28 17:27:34.091510 teams_ai-1.0.1/tests/ai/validators/test_json_response_validator.py
+-rw-r--r--   0        0        0     4144 2024-03-26 18:27:31.075685 teams_ai-1.0.1/tests/state/test_conversation_state.py
+-rw-r--r--   0        0        0     6119 2024-03-04 19:10:38.514847 teams_ai-1.0.1/tests/state/test_custom_turn_state.py
+-rw-r--r--   0        0        0     1797 2024-03-26 18:27:31.075685 teams_ai-1.0.1/tests/state/test_temp_state.py
+-rw-r--r--   0        0        0     6510 2024-03-26 18:27:31.092235 teams_ai-1.0.1/tests/state/test_turn_state.py
+-rw-r--r--   0        0        0     3692 2024-03-26 18:27:31.099741 teams_ai-1.0.1/tests/state/test_user_state.py
+-rw-r--r--   0        0        0     2250 2024-04-01 15:45:22.019885 teams_ai-1.0.1/tests/task_modules/test_task_modules.py
+-rw-r--r--   0        0        0    29183 2024-02-28 17:27:34.095113 teams_ai-1.0.1/tests/test_app.py
+-rw-r--r--   0        0        0    11702 2024-02-28 17:27:34.096123 teams_ai-1.0.1/tests/test_meetings.py
+-rw-r--r--   0        0        0    32052 2024-02-28 17:27:34.106581 teams_ai-1.0.1/tests/test_message_extensions.py
+-rw-r--r--   0        0        0      146 2024-02-28 17:27:34.106581 teams_ai-1.0.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0      526 2024-02-28 17:27:34.107578 teams_ai-1.0.1/tests/utils/activity.py
+-rw-r--r--   0        0        0     1055 2024-02-28 17:27:34.107578 teams_ai-1.0.1/tests/utils/adapter.py
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 teams_ai-1.0.1/PKG-INFO
```

### Comparing `teams_ai-1.0.0rc3/LICENSE` & `teams_ai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/pyproject.toml` & `teams_ai-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teams-ai"
-version = "1.0.0.rc3"
+version = "1.0.1"
 description = "SDK focused on building AI based applications for Microsoft Teams."
 authors = ["Microsoft <teams@microsoft.com>"]
 readme = "README.md"
 repository = "https://github.com/microsoft/teams-ai"
 documentation = "https://learn.microsoft.com/en-us/microsoftteams/platform/bots/how-to/teams%20conversational%20ai/teams-conversation-ai-overview"
 keywords = ["microsoft", "teams", "ai", "bot"]
 packages = [
@@ -20,21 +20,22 @@
 tiktoken = "^0.4.0"
 aiohttp = "^3.8.5"
 jsonschema = "^4.21.1"
 types-pyyaml = "^6.0.12.12"
 pyyaml = "^6.0.1"
 dataclasses-json = "^0.6.4"
 openai = "^1.11.1"
+azure-ai-contentsafety = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pylint = "^2.17.4"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.1"
-black = "^23.7.0"
+black = ">=23.7,<25.0"
 isort = "^5.12.0"
 mypy = "^1.5.0"
 httpx = "^0.26.0"
 
 [tool.poetry.scripts]
 lint = "scripts:lint"
 fmt = "scripts:fmt"
```

### Comparing `teams_ai-1.0.0rc3/README.md` & `teams_ai-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/__init__.py` & `teams_ai-1.0.1/teams/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/activity_type.py` & `teams_ai-1.0.1/teams/activity_type.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/adaptive_cards/adaptive_cards.py` & `teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,17 +169,15 @@
                 return True
 
             self._route_registry.append(Route[StateT](__selector__, __handler__))
             return func
 
         return __call__
 
-    def search(
-        self, dataset: Union[str, Pattern[str], Callable[[TurnContext], bool]]
-    ) -> Callable[
+    def search(self, dataset: Union[str, Pattern[str], Callable[[TurnContext], bool]]) -> Callable[
         [
             Callable[
                 [TurnContext, StateT, Query[AdaptiveCardsSearchParams]],
                 Awaitable[List[AdaptiveCardsSearchResult]],
             ]
         ],
         Callable[
@@ -236,20 +234,24 @@
             [TurnContext, StateT, Query[AdaptiveCardsSearchParams]],
             Awaitable[List[AdaptiveCardsSearchResult]],
         ]:
             async def __handler__(context: TurnContext, state: StateT) -> bool:
                 params = context.activity.value
                 # Flatten search parameters
                 query = Query[AdaptiveCardsSearchParams](
-                    count=params["queryOptions"]["top"]
-                    if params and params["queryOptions"] and params["queryOptions"]["top"]
-                    else 25,
-                    skip=params["queryOptions"]["skip"]
-                    if params and params["queryOptions"] and params["queryOptions"]["skip"]
-                    else 0,
+                    count=(
+                        params["queryOptions"]["top"]
+                        if params and params["queryOptions"] and params["queryOptions"]["top"]
+                        else 25
+                    ),
+                    skip=(
+                        params["queryOptions"]["skip"]
+                        if params and params["queryOptions"] and params["queryOptions"]["skip"]
+                        else 0
+                    ),
                     parameters=AdaptiveCardsSearchParams(
                         query_text=params["queryText"] if params and params["queryText"] else "",
                         dataset=params["dataset"] if params and params["dataset"] else "",
                     ),
                 )
                 result = await func(context, state, query)
                 if context.turn_state.get(ActivityTypes.invoke_response) is None:
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/actions/action_entry.py` & `teams_ai-1.0.1/teams/ai/actions/action_entry.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/actions/action_turn_context.py` & `teams_ai-1.0.1/teams/ai/actions/action_turn_context.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/ai.py` & `teams_ai-1.0.1/teams/ai/ai.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     _actions: Dict[str, ActionEntry[StateT]] = {}
 
     @property
     def options(self) -> AIOptions:
         return self._options
 
     @property
-    def planner(self) -> Planner:
+    def planner(self) -> Planner[StateT]:
         return self._options.planner
 
     @property
     def moderator(self) -> Moderator[StateT]:
         return self._options.moderator
 
     def __init__(self, options: AIOptions, *, logger=Logger("teams.ai")) -> None:
@@ -68,14 +68,17 @@
             ),
             ActionTypes.DO_COMMAND: ActionEntry[StateT](
                 ActionTypes.DO_COMMAND, True, self._on_do_command
             ),
             ActionTypes.SAY_COMMAND: ActionEntry[StateT](
                 ActionTypes.SAY_COMMAND, True, self._on_say_command
             ),
+            ActionTypes.TOO_MANY_STEPS: ActionEntry[StateT](
+                ActionTypes.TOO_MANY_STEPS, True, self._on_too_many_steps
+            ),
         }
 
     def action(
         self, name: Optional[str] = None, *, allow_overrides=False
     ) -> Callable[[ActionHandler[StateT]], ActionHandler[StateT]]:
         """
         Registers a new action event listener. This method can be used as either
@@ -263,7 +266,15 @@
 
         if context.activity.channel_id == Channels.ms_teams:
             await context.send_activity(response.replace("\n", "<br>"))
         else:
             await context.send_activity(response)
 
         return ""
+
+    async def _on_too_many_steps(
+        self,
+        _context: ActionTurnContext,
+        _state: StateT,
+    ) -> str:
+        self._logger.error("The run retrieval for the Assistants Planner has expired.")
+        return ActionTypes.STOP
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/ai_options.py` & `teams_ai-1.0.1/teams/ai/ai_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from typing import Generic, TypeVar
 
+from ..state import TurnState
 from .moderators.default_moderator import DefaultModerator
 from .moderators.moderator import Moderator
 from .planners.planner import Planner
 
+StateT = TypeVar("StateT", bound=TurnState)
+
 
 @dataclass
-class AIOptions:
-    planner: Planner
+class AIOptions(Generic[StateT]):
+    planner: Planner[StateT]
     """
     The planner to use for generating plans.
     """
 
     moderator: Moderator = field(default_factory=DefaultModerator)
     """
     Optional. The moderator to use for moderating input passed to
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/augmentations/augmentation.py` & `teams_ai-1.0.1/teams/ai/augmentations/augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/augmentations/default_augmentation.py` & `teams_ai-1.0.1/teams/ai/augmentations/default_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/augmentations/monologue_augmentation.py` & `teams_ai-1.0.1/teams/ai/augmentations/monologue_augmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,23 +82,32 @@
 
 InnerMonologueSchema: Dict[str, Any] = {
     "type": "object",
     "properties": {
         "thoughts": {
             "type": "object",
             "properties": {
-                "thought": {"type": "string"},
-                "reasoning": {"type": "string"},
-                "plan": {"type": "string"},
+                "thought": {"type": "string", "description": "your current thought"},
+                "reasoning": {
+                    "type": "string",
+                    "description": "self reflect on why you made this decision",
+                },
+                "plan": {
+                    "type": "string",
+                    "description": "a short bulleted list that conveys your long-term plan",
+                },
             },
             "required": ["thought", "reasoning", "plan"],
         },
         "action": {
             "type": "object",
-            "properties": {"name": {"type": "string"}, "parameters": {"type": "object"}},
+            "properties": {
+                "name": {"type": "string", "description": "name of action to execute"},
+                "parameters": {"type": "object", "description": "action parameters"},
+            },
             "required": ["name"],
         },
     },
     "required": ["thoughts", "action"],
 }
 "Json schema for validating an 'InnerMonologue'"
 
@@ -170,14 +179,15 @@
             tokenizer (Tokenizer): Tokenizer to use for encoding/decoding text.
             response (PromptResponse[str]): Response to validate.
             remaining_attempts (int): Number of remaining attempts to validate the response.
 
         Returns:
         Validation: A 'Validation' object.
         """
+
         # Validate that we got a well-formed inner monologue
         validation_result = await self._monologue_validator.validate_response(
             context, memory, tokenizer, response, remaining_attempts
         )
 
         if not validation_result.valid:
             # Catch the case where the action is missing.
@@ -186,14 +196,15 @@
             if validation_result.feedback == _MISSING_ACTION_FEEDBACK:
                 validation_result.feedback = _SAY_REDIRECT_FEEDBACK
             return validation_result
 
         # Validate that the action exists and its parameters are valid
         if validation_result.value:
             monologue = InnerMonologue.from_dict(validation_result.value)
+            validation_result.value = monologue
             parameters = (
                 json.dumps(monologue.action.parameters) if monologue.action.parameters else ""
             )
             message = Message[str](
                 role="assistant",
                 content=None,
                 function_call=FunctionCall(name=monologue.action.name, arguments=parameters),
@@ -227,15 +238,16 @@
 
         Returns:
             Plan: The created plan.
         """
         # Identify the action to perform
         if response.message and response.message.content:
             command: PredictedCommand
-            monologue: InnerMonologue = response.message.content
+            # Double encoding/decoding required for class
+            monologue = InnerMonologue.from_dict(InnerMonologue.to_dict(response.message.content))
 
             if monologue.action.name == "SAY":
                 params = monologue.action.parameters
                 response_val = cast(str, params.get("text")) if params else ""
                 command = PredictedSayCommand(response=response_val)
             else:
                 command = PredictedDoCommand(
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/augmentations/sequence_augmentation.py` & `teams_ai-1.0.1/teams/ai/augmentations/sequence_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/clients/llm_client.py` & `teams_ai-1.0.1/teams/ai/clients/llm_client.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/data_sources/data_source.py` & `teams_ai-1.0.1/teams/ai/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/data_sources/text_data_source.py` & `teams_ai-1.0.1/teams/ai/data_sources/text_data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/__init__.py` & `teams_ai-1.0.1/teams/ai/embeddings/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
+
 from .azure_openai_embeddings import AzureOpenAIEmbeddings
 from .azure_openai_embeddings_options import AzureOpenAIEmbeddingsOptions
 from .embeddings_model import EmbeddingsModel
 from .embeddings_response import EmbeddingsResponse
 from .openai_embeddings import OpenAIEmbeddings
 from .openai_embeddings_options import OpenAIEmbeddingsOptions
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/azure_openai_embeddings.py` & `teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/azure_openai_embeddings_options.py` & `teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/embeddings_model.py` & `teams_ai-1.0.1/teams/ai/embeddings/embeddings_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/embeddings_response.py` & `teams_ai-1.0.1/teams/ai/embeddings/embeddings_response.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/openai_embeddings.py` & `teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/embeddings/openai_embeddings_options.py` & `teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/models/__init__.py` & `teams_ai-1.0.1/teams/ai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/models/chat_completion_action.py` & `teams_ai-1.0.1/teams/ai/models/chat_completion_action.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/models/openai_model.py` & `teams_ai-1.0.1/teams/ai/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/models/prompt_completion_model.py` & `teams_ai-1.0.1/teams/ai/models/prompt_completion_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/models/prompt_response.py` & `teams_ai-1.0.1/teams/ai/models/prompt_response.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/moderators/__init__.py` & `teams_ai-1.0.1/teams/ai/moderators/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/moderators/default_moderator.py` & `teams_ai-1.0.1/teams/ai/moderators/default_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/moderators/moderator.py` & `teams_ai-1.0.1/teams/ai/moderators/moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/moderators/openai_moderator.py` & `teams_ai-1.0.1/teams/ai/moderators/openai_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/planners/__init__.py` & `teams_ai-1.0.1/teams/ai/planners/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 """
 
 from .action_planner import (
     ActionPlanner,
     ActionPlannerOptions,
     ActionPlannerPromptFactory,
 )
+from .assistants_planner import AssistantsPlanner, AssistantsPlannerOptions
 from .plan import Plan, PredictedCommand, PredictedDoCommand, PredictedSayCommand
 from .planner import Planner
 
 __all__ = [
     "ActionPlanner",
     "ActionPlannerOptions",
+    "AssistantsPlanner",
+    "AssistantsPlannerOptions",
     "ActionPlannerPromptFactory",
     "Plan",
     "PredictedCommand",
     "PredictedDoCommand",
     "PredictedSayCommand",
     "Planner",
 ]
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/planners/action_planner.py` & `teams_ai-1.0.1/teams/ai/planners/action_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from logging import Logger
-from typing import Awaitable, Callable, List, Optional, Union
+from typing import Awaitable, Callable, List, Optional, TypeVar, Union
 
 from botbuilder.core import TurnContext
 
 from ...app_error import ApplicationError
 from ...state import MemoryBase, TurnState
 from ..augmentations.default_augmentation import DefaultAugmentation
 from ..clients import LLMClient, LLMClientOptions
@@ -25,14 +25,16 @@
 from .plan import Plan
 from .planner import Planner
 
 ActionPlannerPromptFactory = Callable[
     [TurnContext, TurnState, "ActionPlanner"], Awaitable[PromptTemplate]
 ]
 
+StateT = TypeVar("StateT", bound=TurnState)
+
 
 @dataclass
 class ActionPlannerOptions:
     """
     Options used to configure an `ActionPlanner` instance.
     """
 
@@ -51,15 +53,15 @@
     tokenizer: Tokenizer = field(default_factory=GPTTokenizer)
     "Optional tokenizer to use. Defaults to `GPTTokenizer`"
 
     logger: Optional[Logger] = None
     "Optional. When set the model will log requests"
 
 
-class ActionPlanner(Planner):
+class ActionPlanner(Planner[StateT]):
     """
     A planner that uses a Large Language Model (LLM) to generate plans.
     """
 
     _options: ActionPlannerOptions
     _prompt_factory: ActionPlannerPromptFactory
 
@@ -126,17 +128,17 @@
                 self._options.prompts.add_prompt(prompt)
 
         template = await self._options.prompts.get_prompt(name)
         include_history = template.config.completion.include_history
         client = LLMClient(
             LLMClientOptions(
                 model=self._options.model,
-                history_variable=f"conversation.{name}_history"
-                if include_history
-                else f"temp.{name}_history",
+                history_variable=(
+                    f"conversation.{name}_history" if include_history else f"temp.{name}_history"
+                ),
                 input_variable="temp.input",
                 validator=validator,
                 logger=self._options.logger,
             )
         )
 
         return await client.complete_prompt(
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/planners/plan.py` & `teams_ai-1.0.1/teams/ai/planners/plan.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/planners/planner.py` & `teams_ai-1.0.1/teams/ai/planners/planner.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from typing import Generic, TypeVar
 
 from botbuilder.core import TurnContext
 
 from ...state import TurnState
 from .plan import Plan
 
+StateT = TypeVar("StateT", bound=TurnState)
 
-class Planner(ABC):
+
+class Planner(Generic[StateT], ABC):
     """
     A planner is responsible for generating a plan that the AI system will execute.
     """
 
     @abstractmethod
     async def begin_task(self, context: TurnContext, state: TurnState) -> Plan:
         """
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/__init__.py` & `teams_ai-1.0.1/teams/ai/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/assistant_message.py` & `teams_ai-1.0.1/teams/ai/prompts/assistant_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/augmentation_config.py` & `teams_ai-1.0.1/teams/ai/prompts/augmentation_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/completion_config.py` & `teams_ai-1.0.1/teams/ai/prompts/completion_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/function_call_message.py` & `teams_ai-1.0.1/teams/ai/prompts/function_call_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/function_response_message.py` & `teams_ai-1.0.1/teams/ai/prompts/function_response_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/message.py` & `teams_ai-1.0.1/teams/ai/prompts/message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/prompt.py` & `teams_ai-1.0.1/teams/ai/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/prompt_functions.py` & `teams_ai-1.0.1/teams/ai/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/prompt_manager.py` & `teams_ai-1.0.1/teams/ai/prompts/prompt_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,17 @@
 
             # Include user input
             if template_config.completion.include_images:
                 sections.append(UserInputMessage(self._options.max_input_tokens))
             elif template_config.completion.include_input:
                 sections.append(UserMessage("{{$temp.input}}", self._options.max_input_tokens))
 
-            template = PromptTemplate(template_name, Prompt(sections), template_config)
+            template = PromptTemplate(
+                template_name, Prompt(sections), template_config, template_actions
+            )
 
             if augmentation:
                 template.augmentation = augmentation
 
             # Cache loaded template
             self._prompts[name] = template
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/prompt_manager_options.py` & `teams_ai-1.0.1/teams/ai/prompts/prompt_manager_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/prompt_template.py` & `teams_ai-1.0.1/teams/ai/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/prompt_template_config.py` & `teams_ai-1.0.1/teams/ai/prompts/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/rendered_prompt_section.py` & `teams_ai-1.0.1/teams/ai/prompts/rendered_prompt_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/__init__.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/action_augmentation_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/action_augmentation_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Union
 
-import yaml
 from botbuilder.core import TurnContext
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 
 from ....state import MemoryBase
 from ...models.chat_completion_action import ChatCompletionAction
 from ...tokenizers.tokenizer import Tokenizer
 from ..message import Message
 from ..prompt_functions import PromptFunctions
 from ..rendered_prompt_section import RenderedPromptSection
 from .prompt_section_base import PromptSectionBase
 
 
+@dataclass_json
 @dataclass
-class ActionValue(yaml.YAMLObject):
+class ActionValue(DataClassJsonMixin):
     description: Optional[str] = None
     parameters: Optional[Union[Dict[str, Any], Dict[str, Dict[str, Any]]]] = None
 
 
 @dataclass_json
 @dataclass
 class ActionList(DataClassJsonMixin):
@@ -74,15 +74,15 @@
                     else params
                 )
                 action_list.actions[action.name] = ActionValue(
                     description=action.description, parameters=updated_params
                 )
 
         # Build augmentation text
-        self._text = f"{yaml.dump(action_list.to_dict())}\n\n{call_to_action}"
+        self._text = f"{action_list.to_json()}\n\n{call_to_action}"
 
     async def render_as_messages(
         self,
         context: TurnContext,
         memory: MemoryBase,
         functions: PromptFunctions,
         tokenizer: Tokenizer,
```

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/conversation_history_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/conversation_history_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/data_source_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/data_source_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/group_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/group_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/layout_engine_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/layout_engine_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/prompt_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/prompt_section_base.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section_base.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/template_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/template_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/sections/text_section.py` & `teams_ai-1.0.1/teams/ai/prompts/sections/text_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/system_message.py` & `teams_ai-1.0.1/teams/ai/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/user_input_message.py` & `teams_ai-1.0.1/teams/ai/prompts/user_input_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/prompts/user_message.py` & `teams_ai-1.0.1/teams/ai/prompts/user_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/tokenizers/gpt_tokenizer.py` & `teams_ai-1.0.1/teams/ai/tokenizers/gpt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/tokenizers/tokenizer.py` & `teams_ai-1.0.1/teams/ai/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/utilities.py` & `teams_ai-1.0.1/teams/ai/utilities.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/validators/__init__.py` & `teams_ai-1.0.1/teams/ai/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/validators/action_response_validator.py` & `teams_ai-1.0.1/teams/ai/validators/action_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/validators/default_response_validator.py` & `teams_ai-1.0.1/teams/ai/validators/default_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/validators/json_response_validator.py` & `teams_ai-1.0.1/teams/ai/validators/json_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/validators/prompt_response_validator.py` & `teams_ai-1.0.1/teams/ai/validators/prompt_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/ai/validators/validation.py` & `teams_ai-1.0.1/teams/ai/validators/validation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/app.py` & `teams_ai-1.0.1/teams/app.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/app_options.py` & `teams_ai-1.0.1/teams/app_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/input_file.py` & `teams_ai-1.0.1/teams/input_file.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/meetings/meetings.py` & `teams_ai-1.0.1/teams/meetings/meetings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/message_extensions/message_extensions.py` & `teams_ai-1.0.1/teams/message_extensions/message_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,15 @@
 
 class MessageExtensions(Generic[StateT]):
     _routes: List[Route[StateT]] = []
 
     def __init__(self, routes: List[Route[StateT]]) -> None:
         self._routes = routes
 
-    def query(
-        self, command_id: Union[str, Pattern[str]]
-    ) -> Callable[
+    def query(self, command_id: Union[str, Pattern[str]]) -> Callable[
         [
             Callable[
                 [TurnContext, StateT, MessagingExtensionQuery],
                 Awaitable[MessagingExtensionResult],
             ]
         ],
         Callable[
@@ -111,17 +109,15 @@
                 return True
 
             self._routes.append(Route[StateT](__selector__, __invoke__, True))
             return func
 
         return __call__
 
-    def query_link(
-        self, command_id: Union[str, Pattern[str]]
-    ) -> Callable[
+    def query_link(self, command_id: Union[str, Pattern[str]]) -> Callable[
         [Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]]],
         Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]],
     ]:
         """
         Registers a handler that implements a Link Unfurling based Message Extension.
 
         ```python
@@ -149,15 +145,18 @@
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, str],
                 Awaitable[MessagingExtensionResult],
             ]
-        ) -> Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult],]:
+        ) -> Callable[
+            [TurnContext, StateT, str],
+            Awaitable[MessagingExtensionResult],
+        ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
 
                 value = cast(
                     AppBasedLinkQuery,
                     deserializer_helper(AppBasedLinkQuery, context.activity.value),
@@ -171,17 +170,15 @@
                 return True
 
             self._routes.append(Route[StateT](__selector__, __invoke__, True))
             return func
 
         return __call__
 
-    def anonymous_query_link(
-        self, command_id: Union[str, Pattern[str]]
-    ) -> Callable[
+    def anonymous_query_link(self, command_id: Union[str, Pattern[str]]) -> Callable[
         [Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]]],
         Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]],
     ]:
         """
         Registers a handler for a command that performs anonymous link unfurling.
 
         ```python
@@ -456,17 +453,15 @@
                 return True
 
             self._routes.append(Route[StateT](__selector__, __invoke__, True))
             return func
 
         return __call__
 
-    def fetch_task(
-        self, command_id: Union[str, Pattern[str]]
-    ) -> Callable[
+    def fetch_task(self, command_id: Union[str, Pattern[str]]) -> Callable[
         [Callable[[TurnContext, StateT], Awaitable[Union[TaskModuleTaskInfo, str]]]],
         Callable[[TurnContext, StateT], Awaitable[Union[TaskModuleTaskInfo, str]]],
     ]:
         """
         Registers a handler to process the initial fetch task for an
         Action based message extension.
 
@@ -495,15 +490,18 @@
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT],
                 Awaitable[Union[TaskModuleTaskInfo, str]],
             ]
-        ) -> Callable[[TurnContext, StateT], Awaitable[Union[TaskModuleTaskInfo, str]],]:
+        ) -> Callable[
+            [TurnContext, StateT],
+            Awaitable[Union[TaskModuleTaskInfo, str]],
+        ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 res = await func(context, state)
                 await self._invoke_task_response(context, res)
                 return True
 
             self._routes.append(Route[StateT](__selector__, __invoke__, True))
             return func
@@ -541,28 +539,29 @@
             return True
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, Any],
                 Awaitable[MessagingExtensionResult],
             ]
-        ) -> Callable[[TurnContext, StateT, Any], Awaitable[MessagingExtensionResult],]:
+        ) -> Callable[
+            [TurnContext, StateT, Any],
+            Awaitable[MessagingExtensionResult],
+        ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 res = await func(context, state, context.activity.value)
                 await self._invoke_action_response(context, res)
                 return True
 
             self._routes.append(Route[StateT](__selector__, __invoke__, True))
             return func
 
         return __call__
 
-    def submit_action(
-        self, command_id: Union[str, Pattern[str]]
-    ) -> Callable[
+    def submit_action(self, command_id: Union[str, Pattern[str]]) -> Callable[
         [
             Callable[
                 [TurnContext, StateT, Any],
                 Awaitable[Union[MessagingExtensionResult, TaskModuleTaskInfo, str, None]],
             ]
         ],
         Callable[
```

### Comparing `teams_ai-1.0.0rc3/teams/route.py` & `teams_ai-1.0.1/teams/route.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/__init__.py` & `teams_ai-1.0.1/teams/state/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/conversation_state.py` & `teams_ai-1.0.1/teams/state/conversation_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/memory.py` & `teams_ai-1.0.1/teams/state/memory.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/state.py` & `teams_ai-1.0.1/teams/state/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 
 from .todict import todict
 
 T = TypeVar("T")
 
 
 @overload
-def state(_cls: None = ...) -> Callable[[Type[T]], Type[T]]:
-    ...
+def state(_cls: None = ...) -> Callable[[Type[T]], Type[T]]: ...
 
 
 @overload
-def state(_cls: Type[T]) -> Type[T]:
-    ...
+def state(_cls: Type[T]) -> Type[T]: ...
 
 
 def state(_cls: Optional[Type[T]] = None) -> Union[Callable[[Type[T]], Type[T]], Type[T]]:
     """
     @state\n
     class Example(State):
         ...
```

### Comparing `teams_ai-1.0.0rc3/teams/state/temp_state.py` & `teams_ai-1.0.1/teams/state/temp_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/todict.py` & `teams_ai-1.0.1/teams/state/todict.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/turn_state.py` & `teams_ai-1.0.1/teams/state/turn_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/state/user_state.py` & `teams_ai-1.0.1/teams/state/user_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/task_modules/task_modules.py` & `teams_ai-1.0.1/teams/task_modules/task_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,15 @@
     _route_registry: List[Route[StateT]]
     _task_data_filter: str
 
     def __init__(self, route_registry: List[Route[StateT]], task_data_filter: str) -> None:
         self._route_registry = route_registry
         self._task_data_filter = task_data_filter
 
-    def fetch(
-        self, verb: Union[str, Pattern[str], Callable[[TurnContext], bool]]
-    ) -> Callable[
+    def fetch(self, verb: Union[str, Pattern[str], Callable[[TurnContext], bool]]) -> Callable[
         [Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str]]]],
         Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str]]],
     ]:
         """
         Adds a route for handling the initial fetch of the task module.
         This method can be used as either a decorator or a method.
 
@@ -77,17 +75,15 @@
 
             self._route_registry.append(Route[StateT](__selector__, __handler__, True))
             return func
 
         return __call__
 
     # TODO: Ported the code first. Need more discussion on the functionality.
-    def submit(
-        self, verb: Union[str, Pattern[str], Callable[[TurnContext], bool]]
-    ) -> Callable[
+    def submit(self, verb: Union[str, Pattern[str], Callable[[TurnContext], bool]]) -> Callable[
         [Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str, None]]]],
         Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str, None]]],
     ]:
         """
         Adds a route for handling the submission of a task module.
         This method can be used as either a decorator or a method.
```

### Comparing `teams_ai-1.0.0rc3/teams/teams_adapter.py` & `teams_ai-1.0.1/teams/teams_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ) -> Optional[Response]:
         res = await super().process(
             request,
             bot,
             cast(WebSocketResponse, ws_response),
         )
 
-        if res:
+        if res is not None:
             res.headers.add("User-Agent", self.user_agent)
 
         return res
 
 
 class _TeamsHttpClientFactory(HttpClientFactory):
     _parent: Optional[HttpClientFactory]
```

### Comparing `teams_ai-1.0.0rc3/teams/typing.py` & `teams_ai-1.0.1/teams/typing.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/teams/utils/json/parse.py` & `teams_ai-1.0.1/teams/utils/json/parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     objects: List[Any] = []
     lines = text.split("\n")
 
     for line in lines:
         obj = parse_object(line)
 
-        if obj is not None:
+        if obj is not None and len(obj) > 0:
             objects.append(obj)
 
     if len(objects) == 0:
         obj = parse_object(text)
 
         if obj is not None:
             objects.append(obj)
```

### Comparing `teams_ai-1.0.0rc3/teams/utils/json/parse_object.py` & `teams_ai-1.0.1/teams/utils/json/parse_object.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/adaptive_cards/test_adaptive_cards.py` & `teams_ai-1.0.1/tests/adaptive_cards/test_adaptive_cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
-
 from unittest import IsolatedAsyncioTestCase, mock
 
 import pytest
 from botbuilder.core import TurnContext
 from botbuilder.schema import Activity, ChannelAccount, ConversationAccount
 
 from teams import Application
```

### Comparing `teams_ai-1.0.0rc3/tests/ai/augmentations/test_default_augmentation.py` & `teams_ai-1.0.1/tests/ai/augmentations/test_default_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/augmentations/test_monologue_augmentation.py` & `teams_ai-1.0.1/tests/ai/augmentations/test_monologue_augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,22 @@
                     + '"parameters": { "foo": "bar" }}}}',
                 )
             ),
             3,
         )
         self.assertEqual(response.valid, True)
         self.assertEqual(response.feedback, None)
-        self.assertEqual(
-            response.value,
-            {
-                "thoughts": {"thought": "test", "reasoning": "test", "plan": "test"},
-                "action": {"name": "test1", "parameters": {"foo": "bar"}},
-            },
-        )
+        if response.value:
+            self.assertEqual(
+                InnerMonologue.to_dict(response.value),
+                {
+                    "thoughts": {"thought": "test", "reasoning": "test", "plan": "test"},
+                    "action": {"name": "test1", "parameters": {"foo": "bar"}},
+                },
+            )
 
     async def test_missing_thought_monologue(self):
         state = TurnState()
         monologue = {
             "thoughts": {"reasoning": "test", "plan": "test"},
             "action": {"name": "test", "parameters": {"foo": "bar"}},
         }
```

### Comparing `teams_ai-1.0.0rc3/tests/ai/augmentations/test_sequence_augmentation.py` & `teams_ai-1.0.1/tests/ai/augmentations/test_sequence_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/data_sources/test_text_data_source.py` & `teams_ai-1.0.1/tests/ai/data_sources/test_text_data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/embeddings/test_azure_openai_embeddings.py` & `teams_ai-1.0.1/tests/ai/embeddings/test_azure_openai_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         return openai.types.CreateEmbeddingResponse(
             data=[
                 openai.types.Embedding(embedding=embedding_1, index=1, object="embedding"),
                 openai.types.Embedding(embedding=embedding_2, index=0, object="embedding"),
             ],
             model="text-embedding-ada-002",
             object="list",
-            usage={"prompt_tokens": 5, "total_tokens": 5}  # type: ignore[arg-type]
-            # need to ignore as "Usage" class is not yet an exported type from openai
+            usage=openai.types.create_embedding_response.Usage(prompt_tokens=5, total_tokens=5),
         )
 
 
 class MockAsyncAzureOpenAI:
     embeddings = MockAsyncEmbeddings()
```

### Comparing `teams_ai-1.0.0rc3/tests/ai/embeddings/test_openai_embeddings.py` & `teams_ai-1.0.1/tests/ai/embeddings/test_openai_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         return openai.types.CreateEmbeddingResponse(
             data=[
                 openai.types.Embedding(embedding=embedding_1, index=1, object="embedding"),
                 openai.types.Embedding(embedding=embedding_2, index=0, object="embedding"),
             ],
             model="text-embedding-ada-002",
             object="list",
-            usage={"prompt_tokens": 5, "total_tokens": 5},  # type: ignore[arg-type]
-            # need to ignore as "Usage" class is not yet an exported type from openai
+            usage=openai.types.create_embedding_response.Usage(prompt_tokens=5, total_tokens=5),
         )
 
 
 class MockAsyncOpenAI:
     embeddings = MockAsyncEmbeddings()
```

### Comparing `teams_ai-1.0.0rc3/tests/ai/models/test_openai_model.py` & `teams_ai-1.0.1/tests/ai/models/test_openai_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/moderators/test_azure_content_safety_moderator.py` & `teams_ai-1.0.1/tests/ai/moderators/test_openai_moderator.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,20 +6,16 @@
 from typing import List, Literal, Optional, Union, cast
 from unittest import IsolatedAsyncioTestCase, mock
 
 import httpx
 import openai
 from botbuilder.core import TurnContext
 
-from teams import ApplicationError
 from teams.ai.actions import ActionTypes
-from teams.ai.moderators import (
-    AzureContentSafetyModerator,
-    AzureContentSafetyModeratorOptions,
-)
+from teams.ai.moderators import OpenAIModerator, OpenAIModeratorOptions
 from teams.ai.planners import Plan, PredictedDoCommand, PredictedSayCommand
 from teams.state import ConversationState, TempState, TurnState, UserState
 
 
 class MockAsyncModerations:
     async def create(
         self,
@@ -131,103 +127,85 @@
     moderations = MockAsyncModerationsWithResults()
 
 
 class MockAsyncOpenAIRateLimited:
     moderations = MockAsyncModerationsRateLimited()
 
 
-class TestAzureContentSafetyModerator(IsolatedAsyncioTestCase):
+class TestOpenAIModerator(IsolatedAsyncioTestCase):
     def create_mock_context(
         self, channel_id="channel1", bot_id="bot1", conversation_id="conversation1", user_id="user1"
     ):
         context = mock.MagicMock()
         context.activity.channel_id = channel_id
         context.activity.recipient.id = bot_id
         context.activity.conversation.id = conversation_id
         context.activity.from_property.id = user_id
         return context
 
-    def test_should_raise_error_no_endpoint(self):
-        with self.assertRaises(ApplicationError):
-            AzureContentSafetyModerator(
-                options=AzureContentSafetyModeratorOptions(api_key="", moderate="output")
-            )
-
-    @mock.patch("openai.AsyncAzureOpenAI", return_value=MockAsyncOpenAI)
+    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAI)
     async def test_should_not_review_input(self, mock_async_openai):
-        moderator = AzureContentSafetyModerator(
-            options=AzureContentSafetyModeratorOptions(api_key="", moderate="output", endpoint=""),
-        )
+        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="output"))
         plan = await moderator.review_input(context=cast(TurnContext, {}), state=TurnState())
         self.assertTrue(mock_async_openai.called)
         self.assertIsNone(plan)
 
-    @mock.patch("openai.AsyncAzureOpenAI", return_value=MockAsyncOpenAIWithResults)
+    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIWithResults)
     async def test_should_review_input_and_flag(self, mock_async_openai):
-        moderator = AzureContentSafetyModerator(
-            options=AzureContentSafetyModeratorOptions(api_key="", moderate="input", endpoint="")
-        )
+        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="input"))
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
         plan = await moderator.review_input(context=context, state=state)
         self.assertTrue(mock_async_openai.called)
         assert plan is not None
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "DO")
         assert isinstance(plan.commands[0], PredictedDoCommand)
         self.assertEqual(plan.commands[0].action, ActionTypes.FLAGGED_INPUT)
 
-    @mock.patch("openai.AsyncAzureOpenAI", return_value=MockAsyncOpenAIRateLimited)
+    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIRateLimited)
     async def test_should_review_input_and_error(self, mock_async_openai):
-        moderator = AzureContentSafetyModerator(
-            options=AzureContentSafetyModeratorOptions(api_key="", moderate="both", endpoint="")
-        )
+        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="both"))
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
         plan = await moderator.review_input(context=context, state=state)
         self.assertTrue(mock_async_openai.called)
         assert plan is not None
         self.assertEqual(len(plan.commands), 1)
         self.assertEqual(plan.commands[0].type, "DO")
         assert isinstance(plan.commands[0], PredictedDoCommand)
         self.assertEqual(plan.commands[0].action, ActionTypes.HTTP_ERROR)
 
-    @mock.patch("openai.AsyncAzureOpenAI", return_value=MockAsyncOpenAI)
+    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAI)
     async def test_should_not_review_output(self, mock_async_openai):
-        moderator = AzureContentSafetyModerator(
-            options=AzureContentSafetyModeratorOptions(api_key="", moderate="input", endpoint="")
-        )
+        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="input"))
         plan = Plan(commands=[PredictedSayCommand(response="test")])
         output = await moderator.review_output(
             context=cast(TurnContext, {}), state=TurnState(), plan=plan
         )
         self.assertTrue(mock_async_openai.called)
         self.assertEqual(plan, output)
 
-    @mock.patch("openai.AsyncAzureOpenAI", return_value=MockAsyncOpenAIWithResults)
+    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIWithResults)
     async def test_should_review_output_and_flag(self, mock_async_openai):
-        moderator = AzureContentSafetyModerator(
-            options=AzureContentSafetyModeratorOptions(api_key="", moderate="output", endpoint="")
-        )
+        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="output"))
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
         plan = Plan(commands=[PredictedSayCommand(response="test")])
         output = await moderator.review_output(context=context, state=state, plan=plan)
         self.assertTrue(mock_async_openai.called)
         assert output is not None
         self.assertEqual(len(output.commands), 1)
         self.assertEqual(output.commands[0].type, "DO")
         assert isinstance(output.commands[0], PredictedDoCommand)
         self.assertEqual(output.commands[0].action, ActionTypes.FLAGGED_OUTPUT)
 
-    @mock.patch("openai.AsyncAzureOpenAI", return_value=MockAsyncOpenAIRateLimited)
+    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIRateLimited)
     async def test_should_review_output_and_error(self, mock_async_openai):
-        moderator = AzureContentSafetyModerator(
-            options=AzureContentSafetyModeratorOptions(api_key="", moderate="both", endpoint="")
-        )
+        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="both"))
         context = self.create_mock_context()
         state = await TurnState[ConversationState, UserState, TempState].load(context)
         plan = Plan(commands=[PredictedSayCommand(response="test")])
         output = await moderator.review_output(context=context, state=state, plan=plan)
         self.assertTrue(mock_async_openai.called)
         assert output is not None
         self.assertEqual(len(output.commands), 1)
```

### Comparing `teams_ai-1.0.0rc3/tests/ai/moderators/test_default_moderator.py` & `teams_ai-1.0.1/tests/ai/moderators/test_default_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/moderators/test_openai_moderator.py` & `teams_ai-1.0.1/tests/ai/prompts/test_prompt_manager_v2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,214 +1,195 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
-from typing import List, Literal, Optional, Union, cast
-from unittest import IsolatedAsyncioTestCase, mock
-
-import httpx
-import openai
-from botbuilder.core import TurnContext
-
-from teams.ai.actions import ActionTypes
-from teams.ai.moderators import OpenAIModerator, OpenAIModeratorOptions
-from teams.ai.planners import Plan, PredictedDoCommand, PredictedSayCommand
-from teams.state import ConversationState, TempState, TurnState, UserState
-
-
-class MockAsyncModerations:
-    async def create(
-        self,
-        *,
-        input: Union[str, List[str]],
-        model: Union[
-            str, Literal["text-moderation-latest", "text-moderation-stable"]
-        ] = "text-moderation-latest",
-        extra_headers: Optional[openai._types.Headers] = None,
-        extra_query: Optional[openai._types.Query] = None,
-        extra_body: Optional[openai._types.Body] = None,
-        timeout: Union[
-            float, httpx.Timeout, None, openai._types.NotGiven
-        ] = openai._types.NOT_GIVEN,
-    ) -> openai.types.ModerationCreateResponse:
-        # pylint: disable=unused-argument
-        return openai.types.ModerationCreateResponse(id="", model=model, results=[])
-
-
-class MockAsyncModerationsWithResults:
-    async def create(
-        self,
-        *,
-        input: Union[str, List[str]],
-        model: Union[
-            str, Literal["text-moderation-latest", "text-moderation-stable"]
-        ] = "text-moderation-latest",
-        extra_headers: Optional[openai._types.Headers] = None,
-        extra_query: Optional[openai._types.Query] = None,
-        extra_body: Optional[openai._types.Body] = None,
-        timeout: Union[
-            float, httpx.Timeout, None, openai._types.NotGiven
-        ] = openai._types.NOT_GIVEN,
-    ) -> openai.types.ModerationCreateResponse:
-        # pylint: disable=unused-argument
-        return openai.types.ModerationCreateResponse(
-            id="",
-            model=model,
-            results=[
-                openai.types.Moderation(
-                    categories=cast(
-                        openai.types.moderation.Categories,
-                        {
-                            "harassment": True,
-                            "harassment/threatening": False,
-                            "hate": False,
-                            "hate/threatening": False,
-                            "self-harm": False,
-                            "self-harm/instructions": False,
-                            "self-harm/intent": False,
-                            "sexual": False,
-                            "sexual/minors": False,
-                            "violence": False,
-                            "violence/graphic": False,
-                        },
-                    ),
-                    category_scores=cast(
-                        openai.types.moderation.CategoryScores,
-                        {
-                            "harassment": 0,
-                            "harassment/threatening": 0,
-                            "hate": 0,
-                            "hate/threatening": 0,
-                            "self-harm": 0,
-                            "self-harm/instructions": 0,
-                            "self-harm/intent": 0,
-                            "sexual": 0,
-                            "sexual/minors": 0,
-                            "violence": 0,
-                            "violence/graphic": 0,
-                        },
-                    ),
-                    flagged=True,
-                )
-            ],
-        )
-
-
-class MockAsyncModerationsRateLimited:
-    async def create(
-        self,
-        *,
-        input: Union[str, List[str]],
-        model: Union[
-            str, Literal["text-moderation-latest", "text-moderation-stable"]
-        ] = "text-moderation-latest",
-        extra_headers: Optional[openai._types.Headers] = None,
-        extra_query: Optional[openai._types.Query] = None,
-        extra_body: Optional[openai._types.Body] = None,
-        timeout: Union[
-            float, httpx.Timeout, None, openai._types.NotGiven
-        ] = openai._types.NOT_GIVEN,
-    ) -> openai.types.ModerationCreateResponse:
-        # pylint: disable=unused-argument
-        raise openai.RateLimitError(
-            message="This is a rate limited error",
-            response=httpx.Response(
-                status_code=429, request=httpx.Request(method="method", url="url")
+import os
+from unittest import IsolatedAsyncioTestCase
+from unittest.mock import MagicMock
+
+from teams.ai.data_sources import TextDataSource
+from teams.ai.prompts import (
+    ConversationHistorySection,
+    GroupSection,
+    Prompt,
+    PromptFunction,
+    PromptManager,
+    PromptManagerOptions,
+    PromptTemplate,
+    TemplateSection,
+    UserInputMessage,
+    UserMessage,
+)
+from teams.ai.prompts.sections import ActionAugmentationSection
+from teams.ai.prompts.sections.data_source_section import DataSourceSection
+from teams.app_error import ApplicationError
+
+TEST_ASSERTS_FOLDER: str = os.path.join("tests", "ai", "prompts", "test_assets")
+
+
+class TestPromptManager(IsolatedAsyncioTestCase):
+    def setUp(self):
+        self.options = PromptManagerOptions(TEST_ASSERTS_FOLDER)
+        self.prompt_manager = PromptManager(self.options)
+
+    def test_add_and_get_data_source(self):
+        data_source = TextDataSource("test_name", "test_text")
+        self.prompt_manager.add_data_source(data_source)
+        self.assertTrue(self.prompt_manager.has_data_source("test_name"))
+        self.assertEqual(self.prompt_manager.get_data_source("test_name"), data_source)
+
+    def test_add_data_source_duplicate(self):
+        data_source = TextDataSource("test_name", "test_text")
+        self.prompt_manager.add_data_source(data_source)
+        with self.assertRaises(ApplicationError) as context:
+            self.prompt_manager.add_data_source(data_source)
+        self.assertEqual(str(context.exception), "DataSource 'test_name' already exists.")
+
+    def test_get_data_source_not_found(self):
+        with self.assertRaises(ApplicationError) as context:
+            self.prompt_manager.get_data_source("not_exist")
+        self.assertEqual(str(context.exception), "DataSource 'not_exist' not found.")
+
+    def test_add_and_get_function(self):
+        function = MagicMock(spec=PromptFunction)
+        self.prompt_manager.add_function("test_name", function)
+        self.assertTrue(self.prompt_manager.has_function("test_name"))
+        self.assertEqual(self.prompt_manager.get_function("test_name"), function)
+
+    def test_add_function_duplicate(self):
+        function = MagicMock(spec=PromptFunction)
+        self.prompt_manager.add_function("test_name", function)
+        with self.assertRaises(ApplicationError) as context:
+            self.prompt_manager.add_function("test_name", function)
+        self.assertEqual(str(context.exception), "Function 'test_name' already exists.")
+
+    def test_get_function_not_found(self):
+        with self.assertRaises(ApplicationError) as context:
+            self.prompt_manager.get_function("not_exist")
+        self.assertEqual(str(context.exception), "Function 'not_exist' not found.")
+
+    async def test_add_and_get_prompt(self):
+        prompt = MagicMock(spec=PromptTemplate)
+        prompt.name = "test"
+        self.prompt_manager.add_prompt(prompt)
+        self.assertTrue(self.prompt_manager.has_prompt("test"))
+
+    def test_add_prompt_duplicate(self):
+        prompt = MagicMock(spec=PromptTemplate)
+        prompt.name = "test"
+        self.prompt_manager.add_prompt(prompt)
+        with self.assertRaises(ApplicationError) as context:
+            self.prompt_manager.add_prompt(prompt)
+        self.assertEqual(
+            str(context.exception),
+            (
+                "The PromptManager.add_prompt() method was called with a "
+                "previously registered prompt named 'test'."
             ),
-            body=None,
         )
 
+    def test_has_prompt_from_file(self):
+        self.assertTrue(self.prompt_manager.has_prompt("happy_path"))
+
+    def test_has_prompt_not_found(self):
+        self.assertFalse(self.prompt_manager.has_prompt("not_found"))
+
+    async def test_get_prompt_from_file_no_config(self):
+        with self.assertRaises(ApplicationError) as context:
+            await self.prompt_manager.get_prompt("no_config")
+        self.assertEqual(
+            str(context.exception),
+            "PromptManager.get_prompt(): an error occurred while loading '"
+            + os.path.join(TEST_ASSERTS_FOLDER, "no_config", "config.json")
+            + "'. The file is either invalid or missing.",
+        )
+
+    async def test_get_prompt_from_file_no_prompt(self):
+        with self.assertRaises(ApplicationError) as context:
+            await self.prompt_manager.get_prompt("no_prompt")
+        self.assertEqual(
+            str(context.exception),
+            "PromptManager.get_prompt(): an error occurred while loading '"
+            + os.path.join(TEST_ASSERTS_FOLDER, "no_prompt", "skprompt.txt")
+            + "'. The file is either invalid or missing.",
+        )
+
+    async def test_get_prompt_from_file(self):
+        self.prompt_manager.add_data_source(TextDataSource("teams-ai", "test_text"))
+        prompt = await self.prompt_manager.get_prompt("happy_path")
+
+        self.assertEqual(prompt.name, "happy_path")
+        assert isinstance(prompt.prompt, Prompt)
+        self.assertEqual(len(prompt.prompt.sections), 3)
+        assert isinstance(prompt.prompt.sections[0], GroupSection)
+        self.assertEqual(len(prompt.prompt.sections[0].sections), 3)
+        assert isinstance(prompt.prompt.sections[0].sections[0], TemplateSection)
+        self.assertEqual(prompt.prompt.sections[0].sections[0].template, "test prompt")
+        assert isinstance(prompt.prompt.sections[0].sections[1], DataSourceSection)
+        assert isinstance(prompt.prompt.sections[0].sections[2], ActionAugmentationSection)
+        self.assertEqual(len(prompt.prompt.sections[0].sections[2].actions.keys()), 3)
+        actions = prompt.prompt.sections[0].sections[2].actions
+        self.assertEqual(actions.get("createList").name, "createList")  # type: ignore[union-attr]
+        self.assertEqual(
+            actions.get("createList").description,  # type: ignore[union-attr]
+            "Creates a new list with an optional set of initial items",
+        )
+        assert isinstance(prompt.prompt.sections[1], ConversationHistorySection)
+        self.assertEqual(prompt.prompt.sections[1].variable, "conversation.happy_path_history")
+        self.assertEqual(
+            prompt.prompt.sections[1].tokens, self.options.max_conversation_history_tokens
+        )
+        assert isinstance(prompt.prompt.sections[2], UserMessage)
+        self.assertEqual(prompt.prompt.sections[2].template, "{{$temp.input}}")
+        self.assertEqual(prompt.prompt.sections[2].tokens, self.options.max_input_tokens)
+
+        self.assertEqual(prompt.config.schema, 1.1)
+        self.assertEqual(prompt.config.description, "test config")
+        self.assertEqual(prompt.config.type, "completion")
+        self.assertEqual(prompt.config.completion.model, "gpt-3.5-turbo")
+        self.assertEqual(prompt.config.completion.completion_type, "chat")
+        self.assertEqual(prompt.config.completion.include_history, True)
+        self.assertEqual(prompt.config.completion.include_input, True)
+        self.assertEqual(prompt.config.completion.max_input_tokens, 2800)
+        self.assertEqual(prompt.config.completion.max_tokens, 1000)
+        self.assertEqual(prompt.config.completion.temperature, 0.9)
+        self.assertEqual(prompt.config.completion.top_p, 0.0)
+        self.assertEqual(prompt.config.completion.presence_penalty, 0.6)
+        self.assertEqual(prompt.config.completion.frequency_penalty, 0.0)
+        self.assertEqual(prompt.config.completion.stop_sequences, [])
+        augmentation = prompt.config.augmentation
+        self.assertEqual(augmentation.augmentation_type, "monologue")  # type: ignore[union-attr]
+        self.assertEqual(
+            augmentation.data_sources.get("teams-ai"), 1200  # type: ignore[union-attr]
+        )
 
-class MockAsyncOpenAI:
-    moderations = MockAsyncModerations()
+    async def test_get_prompt_from_file_include_images(self):
+        self.prompt_manager.add_data_source(TextDataSource("teams-ai", "test_text"))
+        prompt = await self.prompt_manager.get_prompt("include_images")
+
+        self.assertEqual(prompt.name, "include_images")
+        assert isinstance(prompt.prompt, Prompt)
+        self.assertEqual(len(prompt.prompt.sections), 3)
+        assert isinstance(prompt.prompt.sections[0], GroupSection)
+        self.assertEqual(len(prompt.prompt.sections[0].sections), 2)
+        assert isinstance(prompt.prompt.sections[0].sections[0], TemplateSection)
+        self.assertEqual(prompt.prompt.sections[0].sections[0].template, "test prompt")
+        assert isinstance(prompt.prompt.sections[0].sections[1], DataSourceSection)
+        assert isinstance(prompt.prompt.sections[1], ConversationHistorySection)
+        self.assertEqual(prompt.prompt.sections[1].variable, "conversation.include_images_history")
+        self.assertEqual(
+            prompt.prompt.sections[1].tokens, self.options.max_conversation_history_tokens
+        )
+        assert isinstance(prompt.prompt.sections[2], UserInputMessage)
+        self.assertEqual(prompt.prompt.sections[2].tokens, self.options.max_input_tokens)
+        augmentation = prompt.config.augmentation
+        self.assertEqual(augmentation.augmentation_type, "none")  # type: ignore[union-attr]
+        self.assertEqual(
+            augmentation.data_sources.get("teams-ai"), 1200  # type: ignore[union-attr]
+        )
 
+    async def test_get_prompt_from_file_migrate_old_schema(self):
+        prompt = await self.prompt_manager.get_prompt("migrate_old_schema")
 
-class MockAsyncOpenAIWithResults:
-    moderations = MockAsyncModerationsWithResults()
-
-
-class MockAsyncOpenAIRateLimited:
-    moderations = MockAsyncModerationsRateLimited()
-
-
-class TestOpenAIModerator(IsolatedAsyncioTestCase):
-    def create_mock_context(
-        self, channel_id="channel1", bot_id="bot1", conversation_id="conversation1", user_id="user1"
-    ):
-        context = mock.MagicMock()
-        context.activity.channel_id = channel_id
-        context.activity.recipient.id = bot_id
-        context.activity.conversation.id = conversation_id
-        context.activity.from_property.id = user_id
-        return context
-
-    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAI)
-    async def test_should_not_review_input(self, mock_async_openai):
-        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="output"))
-        plan = await moderator.review_input(context=cast(TurnContext, {}), state=TurnState())
-        self.assertTrue(mock_async_openai.called)
-        self.assertIsNone(plan)
-
-    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIWithResults)
-    async def test_should_review_input_and_flag(self, mock_async_openai):
-        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="input"))
-        context = self.create_mock_context()
-        state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = await moderator.review_input(context=context, state=state)
-        self.assertTrue(mock_async_openai.called)
-        assert plan is not None
-        self.assertEqual(len(plan.commands), 1)
-        self.assertEqual(plan.commands[0].type, "DO")
-        assert isinstance(plan.commands[0], PredictedDoCommand)
-        self.assertEqual(plan.commands[0].action, ActionTypes.FLAGGED_INPUT)
-
-    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIRateLimited)
-    async def test_should_review_input_and_error(self, mock_async_openai):
-        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="both"))
-        context = self.create_mock_context()
-        state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = await moderator.review_input(context=context, state=state)
-        self.assertTrue(mock_async_openai.called)
-        assert plan is not None
-        self.assertEqual(len(plan.commands), 1)
-        self.assertEqual(plan.commands[0].type, "DO")
-        assert isinstance(plan.commands[0], PredictedDoCommand)
-        self.assertEqual(plan.commands[0].action, ActionTypes.HTTP_ERROR)
-
-    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAI)
-    async def test_should_not_review_output(self, mock_async_openai):
-        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="input"))
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
-        output = await moderator.review_output(
-            context=cast(TurnContext, {}), state=TurnState(), plan=plan
-        )
-        self.assertTrue(mock_async_openai.called)
-        self.assertEqual(plan, output)
-
-    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIWithResults)
-    async def test_should_review_output_and_flag(self, mock_async_openai):
-        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="output"))
-        context = self.create_mock_context()
-        state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
-        output = await moderator.review_output(context=context, state=state, plan=plan)
-        self.assertTrue(mock_async_openai.called)
-        assert output is not None
-        self.assertEqual(len(output.commands), 1)
-        self.assertEqual(output.commands[0].type, "DO")
-        assert isinstance(output.commands[0], PredictedDoCommand)
-        self.assertEqual(output.commands[0].action, ActionTypes.FLAGGED_OUTPUT)
-
-    @mock.patch("openai.AsyncOpenAI", return_value=MockAsyncOpenAIRateLimited)
-    async def test_should_review_output_and_error(self, mock_async_openai):
-        moderator = OpenAIModerator(options=OpenAIModeratorOptions(api_key="", moderate="both"))
-        context = self.create_mock_context()
-        state = await TurnState[ConversationState, UserState, TempState].load(context)
-        plan = Plan(commands=[PredictedSayCommand(response="test")])
-        output = await moderator.review_output(context=context, state=state, plan=plan)
-        self.assertTrue(mock_async_openai.called)
-        assert output is not None
-        self.assertEqual(len(output.commands), 1)
-        self.assertEqual(output.commands[0].type, "DO")
-        assert isinstance(output.commands[0], PredictedDoCommand)
-        self.assertEqual(output.commands[0].action, ActionTypes.HTTP_ERROR)
+        self.assertEqual(prompt.config.schema, 1.1)
+        self.assertEqual(prompt.config.completion.model, "gpt-3.5-turbo")
```

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/happy_path/actions.json` & `teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/actions.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/happy_path/config.json` & `teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/include_images/config.json` & `teams_ai-1.0.1/tests/ai/prompts/test_assets/include_images/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_assets/no_prompt/config.json` & `teams_ai-1.0.1/tests/ai/prompts/test_assets/no_prompt/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_assistant_message.py` & `teams_ai-1.0.1/tests/ai/prompts/test_assistant_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_conversation_history.py` & `teams_ai-1.0.1/tests/ai/prompts/test_conversation_history.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_data_source_section.py` & `teams_ai-1.0.1/tests/ai/prompts/test_data_source_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_function_call_message.py` & `teams_ai-1.0.1/tests/ai/prompts/test_function_call_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_function_response_message.py` & `teams_ai-1.0.1/tests/ai/prompts/test_function_response_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_group_section.py` & `teams_ai-1.0.1/tests/ai/prompts/test_group_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_layout_engine.py` & `teams_ai-1.0.1/tests/ai/prompts/test_layout_engine.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_prompt_section_base.py` & `teams_ai-1.0.1/tests/ai/prompts/test_prompt_section_base.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_system_message.py` & `teams_ai-1.0.1/tests/ai/prompts/test_system_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_template_section.py` & `teams_ai-1.0.1/tests/ai/prompts/test_template_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_text_section.py` & `teams_ai-1.0.1/tests/ai/prompts/test_text_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_user_input_message.py` & `teams_ai-1.0.1/tests/ai/prompts/test_user_input_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/prompts/test_user_message.py` & `teams_ai-1.0.1/tests/ai/prompts/test_user_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/test_utilities.py` & `teams_ai-1.0.1/tests/ai/test_utilities.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/tokenizers/test_gpt_tokenizer.py` & `teams_ai-1.0.1/tests/ai/tokenizers/test_gpt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/validators/test_action_response_validator.py` & `teams_ai-1.0.1/tests/ai/validators/test_action_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/validators/test_default_response_validator.py` & `teams_ai-1.0.1/tests/ai/validators/test_default_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/ai/validators/test_json_response_validator.py` & `teams_ai-1.0.1/tests/ai/validators/test_json_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/state/test_conversation_state.py` & `teams_ai-1.0.1/tests/state/test_conversation_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/state/test_custom_turn_state.py` & `teams_ai-1.0.1/tests/state/test_custom_turn_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/state/test_temp_state.py` & `teams_ai-1.0.1/tests/state/test_temp_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/state/test_turn_state.py` & `teams_ai-1.0.1/tests/state/test_turn_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/state/test_user_state.py` & `teams_ai-1.0.1/tests/state/test_user_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/task_modules/test_task_modules.py` & `teams_ai-1.0.1/tests/task_modules/test_task_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
-
 from unittest import IsolatedAsyncioTestCase, mock
 
 import pytest
 from botbuilder.core import TurnContext
 from botbuilder.schema import Activity, ChannelAccount, ConversationAccount
 
 from teams import Application
```

### Comparing `teams_ai-1.0.0rc3/tests/test_app.py` & `teams_ai-1.0.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/test_meetings.py` & `teams_ai-1.0.1/tests/test_meetings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/test_message_extensions.py` & `teams_ai-1.0.1/tests/test_message_extensions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/utils/activity.py` & `teams_ai-1.0.1/tests/utils/activity.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/tests/utils/adapter.py` & `teams_ai-1.0.1/tests/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.0rc3/PKG-INFO` & `teams_ai-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: teams-ai
-Version: 1.0.0rc3
+Version: 1.0.1
 Summary: SDK focused on building AI based applications for Microsoft Teams.
 Home-page: https://github.com/microsoft/teams-ai
 Keywords: microsoft,teams,ai,bot
 Author: Microsoft
 Author-email: teams@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: azure-ai-contentsafety (>=1.0.0,<2.0.0)
 Requires-Dist: botbuilder-core (>=4.14.8,<5.0.0)
 Requires-Dist: botbuilder-integration-aiohttp (>=4.14.8,<5.0.0)
 Requires-Dist: botframework-connector (>=4.14.8,<5.0.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
```

