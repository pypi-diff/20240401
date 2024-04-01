# Comparing `tmp/flatfile-0.0.8.tar.gz` & `tmp/flatfile-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatfile-0.0.8.tar", max compression
+gzip compressed data, was "flatfile-0.0.9.tar", max compression
```

## Comparing `flatfile-0.0.8.tar` & `flatfile-0.0.9.tar`

### file list

```diff
@@ -1,325 +1,330 @@
--rw-r--r--   0        0        0     3099 2023-10-31 21:51:42.586477 flatfile-0.0.8/README.md
--rw-r--r--   0        0        0      398 2023-10-31 21:51:42.586477 flatfile-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    13393 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/__init__.py
--rw-r--r--   0        0        0     6059 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/client.py
--rw-r--r--   0        0        0      519 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/core/__init__.py
--rw-r--r--   0        0        0      426 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/core/api_error.py
--rw-r--r--   0        0        0     1865 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      166 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/environment.py
--rw-r--r--   0        0        0        0 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/py.typed
--rw-r--r--   0        0        0    13694 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/resources/__init__.py
--rw-r--r--   0        0        0      639 2023-10-31 21:51:42.586477 flatfile-0.0.8/src/flatfile/resources/agents/__init__.py
--rw-r--r--   0        0        0    26215 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/client.py
--rw-r--r--   0        0        0      928 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/__init__.py
--rw-r--r--   0        0        0     1146 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/agent.py
--rw-r--r--   0        0        0     1577 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/agent_config.py
--rw-r--r--   0        0        0     1600 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/agent_log.py
--rw-r--r--   0        0        0     1256 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/agent_response.py
--rw-r--r--   0        0        0      409 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/compiler.py
--rw-r--r--   0        0        0     2138 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/detailed_agent_log.py
--rw-r--r--   0        0        0     1869 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/execution.py
--rw-r--r--   0        0        0     1572 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/get_agent_logs_response.py
--rw-r--r--   0        0        0      948 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/get_detailed_agent_log_response.py
--rw-r--r--   0        0        0     1898 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/get_detailed_agent_logs_response.py
--rw-r--r--   0        0        0     1781 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/get_executions_response.py
--rw-r--r--   0        0        0     1328 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/agents/types/list_agents_response.py
--rw-r--r--   0        0        0      211 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/__init__.py
--rw-r--r--   0        0        0     8597 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/client.py
--rw-r--r--   0        0        0      298 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/types/__init__.py
--rw-r--r--   0        0        0     1733 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/types/api_key.py
--rw-r--r--   0        0        0      890 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/types/api_key_operation.py
--rw-r--r--   0        0        0      479 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/types/api_key_type.py
--rw-r--r--   0        0        0      918 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/auth/types/api_keys_response.py
--rw-r--r--   0        0        0      211 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/cells/__init__.py
--rw-r--r--   0        0        0     6877 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/cells/client.py
--rw-r--r--   0        0        0      287 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/cells/types/__init__.py
--rw-r--r--   0        0        0      936 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/cells/types/cell_value_with_counts.py
--rw-r--r--   0        0        0      937 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/cells/types/cells_response.py
--rw-r--r--   0        0        0      208 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/cells/types/cells_response_data.py
--rw-r--r--   0        0        0      191 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commits/__init__.py
--rw-r--r--   0        0        0     8175 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commits/client.py
--rw-r--r--   0        0        0      254 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commits/types/__init__.py
--rw-r--r--   0        0        0     1646 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commits/types/commit.py
--rw-r--r--   0        0        0      903 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commits/types/commit_response.py
--rw-r--r--   0        0        0      921 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commits/types/list_commits_response.py
--rw-r--r--   0        0        0     1506 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/__init__.py
--rw-r--r--   0        0        0      203 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      265 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      263 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/errors/not_found_error.py
--rw-r--r--   0        0        0     2158 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      107 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/account_id.py
--rw-r--r--   0        0        0     1635 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/action.py
--rw-r--r--   0        0        0      709 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/action_mode.py
--rw-r--r--   0        0        0      631 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/action_schedule.py
--rw-r--r--   0        0        0      104 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/agent_id.py
--rw-r--r--   0        0        0      107 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/document_id.py
--rw-r--r--   0        0        0      111 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/environment_id.py
--rw-r--r--   0        0        0      897 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/error.py
--rw-r--r--   0        0        0      907 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/errors.py
--rw-r--r--   0        0        0      113 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/event_id.py
--rw-r--r--   0        0        0      103 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/file_id.py
--rw-r--r--   0        0        0      747 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/filter.py
--rw-r--r--   0        0        0       83 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/filter_field.py
--rw-r--r--   0        0        0      103 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/guest_id.py
--rw-r--r--   0        0        0      970 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_config.py
--rw-r--r--   0        0        0      945 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_constraint.py
--rw-r--r--   0        0        0      355 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_constraint_type.py
--rw-r--r--   0        0        0     1704 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_enum_property_option.py
--rw-r--r--   0        0        0     1123 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_field.py
--rw-r--r--   0        0        0      993 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_form.py
--rw-r--r--   0        0        0      333 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/input_form_type.py
--rw-r--r--   0        0        0      102 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/job_id.py
--rw-r--r--   0        0        0      114 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/mapping_id.py
--rw-r--r--   0        0        0     1377 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/pagination.py
--rw-r--r--   0        0        0      113 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/record_id.py
--rw-r--r--   0        0        0       83 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/search_field.py
--rw-r--r--   0        0        0       83 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/search_value.py
--rw-r--r--   0        0        0      114 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/secret_id.py
--rw-r--r--   0        0        0      104 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/sheet_id.py
--rw-r--r--   0        0        0      107 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/snapshot_id.py
--rw-r--r--   0        0        0      583 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/sort_direction.py
--rw-r--r--   0        0        0       81 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/sort_field.py
--rw-r--r--   0        0        0      110 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/space_config_id.py
--rw-r--r--   0        0        0      104 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/space_id.py
--rw-r--r--   0        0        0     1135 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/success.py
--rw-r--r--   0        0        0      874 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/success_data.py
--rw-r--r--   0        0        0      104 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/user_id.py
--rw-r--r--   0        0        0      106 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/version_id.py
--rw-r--r--   0        0        0      107 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/commons/types/workbook_id.py
--rw-r--r--   0        0        0      237 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/__init__.py
--rw-r--r--   0        0        0    14126 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/client.py
--rw-r--r--   0        0        0      334 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/types/__init__.py
--rw-r--r--   0        0        0     1573 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/types/document.py
--rw-r--r--   0        0        0     1031 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/types/document_config.py
--rw-r--r--   0        0        0      911 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/types/document_response.py
--rw-r--r--   0        0        0      929 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/documents/types/list_documents_response.py
--rw-r--r--   0        0        0      433 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/__init__.py
--rw-r--r--   0        0        0    18621 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/client.py
--rw-r--r--   0        0        0      596 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/__init__.py
--rw-r--r--   0        0        0     2144 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/environment.py
--rw-r--r--   0        0        0     1974 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/environment_config_create.py
--rw-r--r--   0        0        0     2005 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/environment_config_update.py
--rw-r--r--   0        0        0      923 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/environment_response.py
--rw-r--r--   0        0        0      604 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/guest_authentication_enum.py
--rw-r--r--   0        0        0     1036 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/environments/types/list_environments_response.py
--rw-r--r--   0        0        0     2395 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/__init__.py
--rw-r--r--   0        0        0    14746 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/client.py
--rw-r--r--   0        0        0     2695 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/__init__.py
--rw-r--r--   0        0        0       82 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/action_name.py
--rw-r--r--   0        0        0     1711 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/base_event.py
--rw-r--r--   0        0        0     2940 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/context.py
--rw-r--r--   0        0        0     1229 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/create_event_config.py
--rw-r--r--   0        0        0     1083 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/domain.py
--rw-r--r--   0        0        0     8243 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/event.py
--rw-r--r--   0        0        0     1301 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/event_attributes.py
--rw-r--r--   0        0        0     1126 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/event_context_slugs.py
--rw-r--r--   0        0        0      899 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/event_response.py
--rw-r--r--   0        0        0     6247 2023-10-31 21:51:42.590477 flatfile-0.0.8/src/flatfile/resources/events/types/event_topic.py
--rw-r--r--   0        0        0     1593 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/events/types/generic_event.py
--rw-r--r--   0        0        0      920 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/events/types/list_all_events_response.py
--rw-r--r--   0        0        0      965 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/events/types/origin.py
--rw-r--r--   0        0        0     1250 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/events/types/progress.py
--rw-r--r--   0        0        0       81 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/events/types/sheet_slug.py
--rw-r--r--   0        0        0      237 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/__init__.py
--rw-r--r--   0        0        0    18630 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/client.py
--rw-r--r--   0        0        0      346 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/types/__init__.py
--rw-r--r--   0        0        0     2446 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/types/file.py
--rw-r--r--   0        0        0      895 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/types/file_response.py
--rw-r--r--   0        0        0     1008 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/types/list_files_response.py
--rw-r--r--   0        0        0      438 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/types/mode.py
--rw-r--r--   0        0        0      969 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/files/types/model_file_status_enum.py
--rw-r--r--   0        0        0      453 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/__init__.py
--rw-r--r--   0        0        0    12759 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/client.py
--rw-r--r--   0        0        0      633 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/__init__.py
--rw-r--r--   0        0        0      918 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/create_guest_response.py
--rw-r--r--   0        0        0     1220 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/guest.py
--rw-r--r--   0        0        0     1186 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/guest_config.py
--rw-r--r--   0        0        0     1274 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/guest_config_update.py
--rw-r--r--   0        0        0      899 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/guest_response.py
--rw-r--r--   0        0        0     1151 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/guest_space.py
--rw-r--r--   0        0        0      929 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/guest_workbook.py
--rw-r--r--   0        0        0     1356 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/invite.py
--rw-r--r--   0        0        0      917 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/guests/types/list_guests_response.py
--rw-r--r--   0        0        0     2355 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/__init__.py
--rw-r--r--   0        0        0    29853 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/client.py
--rw-r--r--   0        0        0     3469 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/__init__.py
--rw-r--r--   0        0        0     1116 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/category_mapping.py
--rw-r--r--   0        0        0      760 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/certainty.py
--rw-r--r--   0        0        0      998 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/collection_job_subject.py
--rw-r--r--   0        0        0     1812 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/delete_records_job_config.py
--rw-r--r--   0        0        0     1077 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/destination_field.py
--rw-r--r--   0        0        0      377 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/driver.py
--rw-r--r--   0        0        0     1462 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/edge.py
--rw-r--r--   0        0        0      855 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/empty_object.py
--rw-r--r--   0        0        0     1394 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/enum_details.py
--rw-r--r--   0        0        0      121 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/enum_value.py
--rw-r--r--   0        0        0      929 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/export_job_config.py
--rw-r--r--   0        0        0     2607 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/export_options.py
--rw-r--r--   0        0        0     1146 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/file_job_config.py
--rw-r--r--   0        0        0     2676 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/find_and_replace_job_config.py
--rw-r--r--   0        0        0     1754 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job.py
--rw-r--r--   0        0        0     1145 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_ack_details.py
--rw-r--r--   0        0        0      956 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_cancel_details.py
--rw-r--r--   0        0        0     1017 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_complete_details.py
--rw-r--r--   0        0        0     2693 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_config.py
--rw-r--r--   0        0        0      146 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_destination.py
--rw-r--r--   0        0        0     1466 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan.py
--rw-r--r--   0        0        0     1537 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan_config.py
--rw-r--r--   0        0        0     1175 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan_config_request.py
--rw-r--r--   0        0        0     1150 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan_request.py
--rw-r--r--   0        0        0      738 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_mode.py
--rw-r--r--   0        0        0     1216 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome.py
--rw-r--r--   0        0        0     1308 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next.py
--rw-r--r--   0        0        0     1029 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_download.py
--rw-r--r--   0        0        0      905 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_id.py
--rw-r--r--   0        0        0      907 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_url.py
--rw-r--r--   0        0        0      931 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_wait.py
--rw-r--r--   0        0        0     1050 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_plan.py
--rw-r--r--   0        0        0      908 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_plan_response.py
--rw-r--r--   0        0        0      891 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_response.py
--rw-r--r--   0        0        0       81 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_source.py
--rw-r--r--   0        0        0      957 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_status.py
--rw-r--r--   0        0        0      752 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_subject.py
--rw-r--r--   0        0        0      640 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_type.py
--rw-r--r--   0        0        0     1476 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_update.py
--rw-r--r--   0        0        0      626 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/job_update_config.py
--rw-r--r--   0        0        0     1004 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/list_jobs_response.py
--rw-r--r--   0        0        0     1000 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/metadata.py
--rw-r--r--   0        0        0     2724 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/mutate_job_config.py
--rw-r--r--   0        0        0     1102 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/pipeline_job_config.py
--rw-r--r--   0        0        0      875 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/resource_job_subject.py
--rw-r--r--   0        0        0     1062 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/source_field.py
--rw-r--r--   0        0        0      521 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/jobs/types/trigger.py
--rw-r--r--   0        0        0      433 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/__init__.py
--rw-r--r--   0        0        0     8023 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/client.py
--rw-r--r--   0        0        0      604 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/__init__.py
--rw-r--r--   0        0        0      186 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule.py
--rw-r--r--   0        0        0     1602 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_base.py
--rw-r--r--   0        0        0     1046 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_config.py
--rw-r--r--   0        0        0     1153 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_one_to_one.py
--rw-r--r--   0        0        0      924 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_response.py
--rw-r--r--   0        0        0      337 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_type.py
--rw-r--r--   0        0        0      938 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rules_response.py
--rw-r--r--   0        0        0     1441 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/__init__.py
--rw-r--r--   0        0        0     1941 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/__init__.py
--rw-r--r--   0        0        0      979 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/arrayable_property.py
--rw-r--r--   0        0        0     1348 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/base_property.py
--rw-r--r--   0        0        0     1126 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/boolean_property.py
--rw-r--r--   0        0        0      987 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/boolean_property_config.py
--rw-r--r--   0        0        0      927 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/constraint.py
--rw-r--r--   0        0        0     1070 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/date_property.py
--rw-r--r--   0        0        0     1580 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/enum_property.py
--rw-r--r--   0        0        0     1110 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/enum_property_config.py
--rw-r--r--   0        0        0     1699 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/enum_property_option.py
--rw-r--r--   0        0        0     1061 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/number_config.py
--rw-r--r--   0        0        0     1180 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/number_property.py
--rw-r--r--   0        0        0     2450 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/property.py
--rw-r--r--   0        0        0     1198 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/reference_property.py
--rw-r--r--   0        0        0     1293 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/reference_property_config.py
--rw-r--r--   0        0        0      526 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/reference_property_relationship.py
--rw-r--r--   0        0        0      942 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/string_config.py
--rw-r--r--   0        0        0      977 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/string_config_options.py
--rw-r--r--   0        0        0     1109 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/string_property.py
--rw-r--r--   0        0        0      974 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/unique_constraint.py
--rw-r--r--   0        0        0     1093 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/property/types/unique_constraint_config.py
--rw-r--r--   0        0        0     1053 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/__init__.py
--rw-r--r--   0        0        0    32141 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/client.py
--rw-r--r--   0        0        0     1584 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/__init__.py
--rw-r--r--   0        0        0     1246 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/cell_value.py
--rw-r--r--   0        0        0      182 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/cell_value_union.py
--rw-r--r--   0        0        0      886 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/cell_value_with_links.py
--rw-r--r--   0        0        0      154 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/diff_data.py
--rw-r--r--   0        0        0      869 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/diff_record.py
--rw-r--r--   0        0        0      155 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/diff_records.py
--rw-r--r--   0        0        0      924 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/diff_records_response.py
--rw-r--r--   0        0        0     1062 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/diff_value.py
--rw-r--r--   0        0        0      958 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/get_records_response.py
--rw-r--r--   0        0        0     1317 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/get_records_response_data.py
--rw-r--r--   0        0        0      924 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/record.py
--rw-r--r--   0        0        0     1300 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/record_base.py
--rw-r--r--   0        0        0     1048 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/record_counts.py
--rw-r--r--   0        0        0      156 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/record_data.py
--rw-r--r--   0        0        0      194 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/record_data_with_links.py
--rw-r--r--   0        0        0     1304 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/record_with_links.py
--rw-r--r--   0        0        0      138 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/records.py
--rw-r--r--   0        0        0      945 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/records_response.py
--rw-r--r--   0        0        0     1264 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/records_response_data.py
--rw-r--r--   0        0        0      176 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/records_with_links.py
--rw-r--r--   0        0        0     1129 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/validation_message.py
--rw-r--r--   0        0        0     1292 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/validation_source.py
--rw-r--r--   0        0        0      611 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/records/types/validation_type.py
--rw-r--r--   0        0        0      231 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/secrets/__init__.py
--rw-r--r--   0        0        0     8774 2023-10-31 21:51:42.594477 flatfile-0.0.8/src/flatfile/resources/secrets/client.py
--rw-r--r--   0        0        0      335 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/secrets/types/__init__.py
--rw-r--r--   0        0        0      923 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/secrets/types/secret.py
--rw-r--r--   0        0        0      111 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/secrets/types/secret_name.py
--rw-r--r--   0        0        0      112 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/secrets/types/secret_value.py
--rw-r--r--   0        0        0      917 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/secrets/types/secrets_response.py
--rw-r--r--   0        0        0     1447 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/secrets/types/write_secret.py
--rw-r--r--   0        0        0      593 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/__init__.py
--rw-r--r--   0        0        0    26335 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/client.py
--rw-r--r--   0        0        0      855 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/__init__.py
--rw-r--r--   0        0        0      931 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/field_config_response.py
--rw-r--r--   0        0        0      917 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/list_sheets_response.py
--rw-r--r--   0        0        0      966 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/record_counts_response.py
--rw-r--r--   0        0        0      917 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/record_counts_response_data.py
--rw-r--r--   0        0        0     1749 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet.py
--rw-r--r--   0        0        0      856 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_access.py
--rw-r--r--   0        0        0     1452 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_config.py
--rw-r--r--   0        0        0      897 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_config_or_update.py
--rw-r--r--   0        0        0     1492 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_config_update.py
--rw-r--r--   0        0        0      899 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_response.py
--rw-r--r--   0        0        0     1711 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_update.py
--rw-r--r--   0        0        0      389 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/__init__.py
--rw-r--r--   0        0        0    17979 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/client.py
--rw-r--r--   0        0        0      529 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/__init__.py
--rw-r--r--   0        0        0      783 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/change_type.py
--rw-r--r--   0        0        0      913 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/restore_options.py
--rw-r--r--   0        0        0     1363 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshot.py
--rw-r--r--   0        0        0      911 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshot_response.py
--rw-r--r--   0        0        0     1169 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshot_summary.py
--rw-r--r--   0        0        0      925 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshots_response.py
--rw-r--r--   0        0        0     1007 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/snapshots/types/summary_section.py
--rw-r--r--   0        0        0      515 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/__init__.py
--rw-r--r--   0        0        0    17971 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/client.py
--rw-r--r--   0        0        0      733 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/__init__.py
--rw-r--r--   0        0        0     1378 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/event_token.py
--rw-r--r--   0        0        0      920 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/event_token_response.py
--rw-r--r--   0        0        0     1264 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/get_spaces_sort_field.py
--rw-r--r--   0        0        0     2124 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/internal_space_config_base.py
--rw-r--r--   0        0        0     1055 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/list_spaces_response.py
--rw-r--r--   0        0        0     2642 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/space.py
--rw-r--r--   0        0        0      440 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/space_access.py
--rw-r--r--   0        0        0     1451 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/space_config.py
--rw-r--r--   0        0        0      899 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/space_response.py
--rw-r--r--   0        0        0     1088 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/spaces/types/space_size.py
--rw-r--r--   0        0        0      481 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/__init__.py
--rw-r--r--   0        0        0    14523 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/client.py
--rw-r--r--   0        0        0      679 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/__init__.py
--rw-r--r--   0        0        0     1189 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/api_token.py
--rw-r--r--   0        0        0      958 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/api_token_response.py
--rw-r--r--   0        0        0     1301 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/exchange_token_data.py
--rw-r--r--   0        0        0      945 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/exchange_token_response.py
--rw-r--r--   0        0        0     1081 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/list_api_tokens_response.py
--rw-r--r--   0        0        0      913 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/list_users_response.py
--rw-r--r--   0        0        0      918 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/user.py
--rw-r--r--   0        0        0     1100 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/user_config.py
--rw-r--r--   0        0        0      895 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/users/types/user_response.py
--rw-r--r--   0        0        0      151 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/versions/__init__.py
--rw-r--r--   0        0        0     3583 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/versions/client.py
--rw-r--r--   0        0        0      182 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/versions/types/__init__.py
--rw-r--r--   0        0        0     1010 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/versions/types/version.py
--rw-r--r--   0        0        0      907 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/versions/types/version_response.py
--rw-r--r--   0        0        0      389 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/__init__.py
--rw-r--r--   0        0        0    44432 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/client.py
--rw-r--r--   0        0        0      529 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/__init__.py
--rw-r--r--   0        0        0     1752 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/create_workbook_config.py
--rw-r--r--   0        0        0      929 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/list_workbooks_response.py
--rw-r--r--   0        0        0     1992 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook.py
--rw-r--r--   0        0        0     1334 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook_config_settings.py
--rw-r--r--   0        0        0      911 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook_response.py
--rw-r--r--   0        0        0     1680 2023-10-31 21:51:42.598477 flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook_update.py
--rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 flatfile-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3099 2023-11-06 17:30:43.324272 flatfile-0.0.9/README.md
+-rw-r--r--   0        0        0      398 2023-11-06 17:30:43.324272 flatfile-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    13613 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/__init__.py
+-rw-r--r--   0        0        0     6059 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/client.py
+-rw-r--r--   0        0        0      519 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/core/api_error.py
+-rw-r--r--   0        0        0     1865 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      166 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/environment.py
+-rw-r--r--   0        0        0        0 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/py.typed
+-rw-r--r--   0        0        0    13914 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/__init__.py
+-rw-r--r--   0        0        0      639 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/__init__.py
+-rw-r--r--   0        0        0    29537 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/client.py
+-rw-r--r--   0        0        0      928 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/__init__.py
+-rw-r--r--   0        0        0     1156 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/agent.py
+-rw-r--r--   0        0        0     1577 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/agent_config.py
+-rw-r--r--   0        0        0     1591 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/agent_log.py
+-rw-r--r--   0        0        0     1266 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/agent_response.py
+-rw-r--r--   0        0        0      409 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/compiler.py
+-rw-r--r--   0        0        0     2129 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/detailed_agent_log.py
+-rw-r--r--   0        0        0     1860 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/execution.py
+-rw-r--r--   0        0        0     1563 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/get_agent_logs_response.py
+-rw-r--r--   0        0        0     1564 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/get_detailed_agent_log_response.py
+-rw-r--r--   0        0        0     1889 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/get_detailed_agent_logs_response.py
+-rw-r--r--   0        0        0     1772 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/get_executions_response.py
+-rw-r--r--   0        0        0     1338 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/agents/types/list_agents_response.py
+-rw-r--r--   0        0        0      211 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/__init__.py
+-rw-r--r--   0        0        0     8597 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/client.py
+-rw-r--r--   0        0        0      298 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/types/__init__.py
+-rw-r--r--   0        0        0     1733 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/types/api_key.py
+-rw-r--r--   0        0        0      890 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/types/api_key_operation.py
+-rw-r--r--   0        0        0      479 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/types/api_key_type.py
+-rw-r--r--   0        0        0      918 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/auth/types/api_keys_response.py
+-rw-r--r--   0        0        0      211 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/cells/__init__.py
+-rw-r--r--   0        0        0     6877 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/cells/client.py
+-rw-r--r--   0        0        0      287 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/cells/types/__init__.py
+-rw-r--r--   0        0        0      936 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/cells/types/cell_value_with_counts.py
+-rw-r--r--   0        0        0      937 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/cells/types/cells_response.py
+-rw-r--r--   0        0        0      208 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/cells/types/cells_response_data.py
+-rw-r--r--   0        0        0      191 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/commits/__init__.py
+-rw-r--r--   0        0        0     8175 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/commits/client.py
+-rw-r--r--   0        0        0      254 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/commits/types/__init__.py
+-rw-r--r--   0        0        0     1646 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/commits/types/commit.py
+-rw-r--r--   0        0        0      903 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/commits/types/commit_response.py
+-rw-r--r--   0        0        0      921 2023-11-06 17:30:43.324272 flatfile-0.0.9/src/flatfile/resources/commits/types/list_commits_response.py
+-rw-r--r--   0        0        0     1726 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/__init__.py
+-rw-r--r--   0        0        0      203 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      265 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      263 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0     2505 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      106 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/account_id.py
+-rw-r--r--   0        0        0     1747 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/action.py
+-rw-r--r--   0        0        0      949 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/action_constraint.py
+-rw-r--r--   0        0        0      565 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/action_constraint_type.py
+-rw-r--r--   0        0        0      709 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/action_mode.py
+-rw-r--r--   0        0        0      631 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/action_schedule.py
+-rw-r--r--   0        0        0      103 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/agent_id.py
+-rw-r--r--   0        0        0      106 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/document_id.py
+-rw-r--r--   0        0        0      110 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/environment_id.py
+-rw-r--r--   0        0        0      897 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/error.py
+-rw-r--r--   0        0        0      907 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/errors.py
+-rw-r--r--   0        0        0      104 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/event_id.py
+-rw-r--r--   0        0        0      102 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/file_id.py
+-rw-r--r--   0        0        0      747 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/filter.py
+-rw-r--r--   0        0        0       83 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/filter_field.py
+-rw-r--r--   0        0        0      102 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/guest_id.py
+-rw-r--r--   0        0        0      970 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_config.py
+-rw-r--r--   0        0        0      945 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_constraint.py
+-rw-r--r--   0        0        0      355 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_constraint_type.py
+-rw-r--r--   0        0        0     1704 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_enum_property_option.py
+-rw-r--r--   0        0        0     1123 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_field.py
+-rw-r--r--   0        0        0      993 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_form.py
+-rw-r--r--   0        0        0      333 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/input_form_type.py
+-rw-r--r--   0        0        0      101 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/job_id.py
+-rw-r--r--   0        0        0      105 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/mapping_id.py
+-rw-r--r--   0        0        0       92 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/page_number.py
+-rw-r--r--   0        0        0       91 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/page_size.py
+-rw-r--r--   0        0        0     1377 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/pagination.py
+-rw-r--r--   0        0        0      104 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/record_id.py
+-rw-r--r--   0        0        0       83 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/search_field.py
+-rw-r--r--   0        0        0       83 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/search_value.py
+-rw-r--r--   0        0        0      105 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/secret_id.py
+-rw-r--r--   0        0        0      103 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/sheet_id.py
+-rw-r--r--   0        0        0      106 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/snapshot_id.py
+-rw-r--r--   0        0        0      583 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/sort_direction.py
+-rw-r--r--   0        0        0       81 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/sort_field.py
+-rw-r--r--   0        0        0      109 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/space_config_id.py
+-rw-r--r--   0        0        0      103 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/space_id.py
+-rw-r--r--   0        0        0     1135 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/success.py
+-rw-r--r--   0        0        0      874 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/success_data.py
+-rw-r--r--   0        0        0      107 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/success_query_parameter.py
+-rw-r--r--   0        0        0      103 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/user_id.py
+-rw-r--r--   0        0        0      105 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/version_id.py
+-rw-r--r--   0        0        0      106 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/commons/types/workbook_id.py
+-rw-r--r--   0        0        0      237 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/__init__.py
+-rw-r--r--   0        0        0    14126 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/client.py
+-rw-r--r--   0        0        0      334 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/types/__init__.py
+-rw-r--r--   0        0        0     1573 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/types/document.py
+-rw-r--r--   0        0        0     1031 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/types/document_config.py
+-rw-r--r--   0        0        0      911 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/types/document_response.py
+-rw-r--r--   0        0        0      929 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/documents/types/list_documents_response.py
+-rw-r--r--   0        0        0      433 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/__init__.py
+-rw-r--r--   0        0        0    18617 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/client.py
+-rw-r--r--   0        0        0      596 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/__init__.py
+-rw-r--r--   0        0        0     2142 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/environment.py
+-rw-r--r--   0        0        0     1974 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/environment_config_create.py
+-rw-r--r--   0        0        0     2005 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/environment_config_update.py
+-rw-r--r--   0        0        0      923 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/environment_response.py
+-rw-r--r--   0        0        0      604 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/guest_authentication_enum.py
+-rw-r--r--   0        0        0     1036 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/environments/types/list_environments_response.py
+-rw-r--r--   0        0        0     2395 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/__init__.py
+-rw-r--r--   0        0        0    14746 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/client.py
+-rw-r--r--   0        0        0     2695 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/__init__.py
+-rw-r--r--   0        0        0       82 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/action_name.py
+-rw-r--r--   0        0        0     1711 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/base_event.py
+-rw-r--r--   0        0        0     3017 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/context.py
+-rw-r--r--   0        0        0     1229 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/create_event_config.py
+-rw-r--r--   0        0        0     1083 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/domain.py
+-rw-r--r--   0        0        0     8243 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/event.py
+-rw-r--r--   0        0        0     1301 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/event_attributes.py
+-rw-r--r--   0        0        0     1126 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/event_context_slugs.py
+-rw-r--r--   0        0        0      899 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/event_response.py
+-rw-r--r--   0        0        0     6247 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/event_topic.py
+-rw-r--r--   0        0        0     1593 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/generic_event.py
+-rw-r--r--   0        0        0      920 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/list_all_events_response.py
+-rw-r--r--   0        0        0      965 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/origin.py
+-rw-r--r--   0        0        0     1250 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/progress.py
+-rw-r--r--   0        0        0       81 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/events/types/sheet_slug.py
+-rw-r--r--   0        0        0      237 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/__init__.py
+-rw-r--r--   0        0        0    18630 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/client.py
+-rw-r--r--   0        0        0      346 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/types/__init__.py
+-rw-r--r--   0        0        0     2446 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/types/file.py
+-rw-r--r--   0        0        0      895 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/types/file_response.py
+-rw-r--r--   0        0        0     1008 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/types/list_files_response.py
+-rw-r--r--   0        0        0      438 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/types/mode.py
+-rw-r--r--   0        0        0      969 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/files/types/model_file_status_enum.py
+-rw-r--r--   0        0        0      453 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/__init__.py
+-rw-r--r--   0        0        0    12759 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/client.py
+-rw-r--r--   0        0        0      633 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/__init__.py
+-rw-r--r--   0        0        0      918 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/create_guest_response.py
+-rw-r--r--   0        0        0     1220 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/guest.py
+-rw-r--r--   0        0        0     1186 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/guest_config.py
+-rw-r--r--   0        0        0     1274 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/guest_config_update.py
+-rw-r--r--   0        0        0      899 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/guest_response.py
+-rw-r--r--   0        0        0     1151 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/guest_space.py
+-rw-r--r--   0        0        0      929 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/guest_workbook.py
+-rw-r--r--   0        0        0     1356 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/invite.py
+-rw-r--r--   0        0        0      917 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/guests/types/list_guests_response.py
+-rw-r--r--   0        0        0     2355 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/__init__.py
+-rw-r--r--   0        0        0    29853 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/client.py
+-rw-r--r--   0        0        0     3469 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/__init__.py
+-rw-r--r--   0        0        0     1116 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/category_mapping.py
+-rw-r--r--   0        0        0      760 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/certainty.py
+-rw-r--r--   0        0        0      998 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/collection_job_subject.py
+-rw-r--r--   0        0        0     1812 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/delete_records_job_config.py
+-rw-r--r--   0        0        0     1077 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/destination_field.py
+-rw-r--r--   0        0        0      377 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/driver.py
+-rw-r--r--   0        0        0     1462 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/edge.py
+-rw-r--r--   0        0        0      855 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/empty_object.py
+-rw-r--r--   0        0        0     1394 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/enum_details.py
+-rw-r--r--   0        0        0      121 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/enum_value.py
+-rw-r--r--   0        0        0      929 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/export_job_config.py
+-rw-r--r--   0        0        0     2607 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/export_options.py
+-rw-r--r--   0        0        0     1146 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/file_job_config.py
+-rw-r--r--   0        0        0     2676 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/find_and_replace_job_config.py
+-rw-r--r--   0        0        0     1754 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job.py
+-rw-r--r--   0        0        0     1145 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_ack_details.py
+-rw-r--r--   0        0        0      956 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_cancel_details.py
+-rw-r--r--   0        0        0     1017 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_complete_details.py
+-rw-r--r--   0        0        0     2693 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_config.py
+-rw-r--r--   0        0        0      146 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_destination.py
+-rw-r--r--   0        0        0     1466 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan.py
+-rw-r--r--   0        0        0     1537 2023-11-06 17:30:43.328271 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan_config.py
+-rw-r--r--   0        0        0     1175 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan_config_request.py
+-rw-r--r--   0        0        0     1150 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan_request.py
+-rw-r--r--   0        0        0      738 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_mode.py
+-rw-r--r--   0        0        0     1216 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome.py
+-rw-r--r--   0        0        0     1308 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next.py
+-rw-r--r--   0        0        0     1029 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_download.py
+-rw-r--r--   0        0        0      905 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_id.py
+-rw-r--r--   0        0        0      907 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_url.py
+-rw-r--r--   0        0        0      931 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_wait.py
+-rw-r--r--   0        0        0     1050 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_plan.py
+-rw-r--r--   0        0        0      908 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_plan_response.py
+-rw-r--r--   0        0        0      891 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_response.py
+-rw-r--r--   0        0        0       81 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_source.py
+-rw-r--r--   0        0        0      957 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_status.py
+-rw-r--r--   0        0        0      752 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_subject.py
+-rw-r--r--   0        0        0      640 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_type.py
+-rw-r--r--   0        0        0     1476 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_update.py
+-rw-r--r--   0        0        0      626 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/job_update_config.py
+-rw-r--r--   0        0        0     1004 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/list_jobs_response.py
+-rw-r--r--   0        0        0     1000 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/metadata.py
+-rw-r--r--   0        0        0     2724 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/mutate_job_config.py
+-rw-r--r--   0        0        0     1102 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/pipeline_job_config.py
+-rw-r--r--   0        0        0      875 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/resource_job_subject.py
+-rw-r--r--   0        0        0     1062 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/source_field.py
+-rw-r--r--   0        0        0      521 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/jobs/types/trigger.py
+-rw-r--r--   0        0        0      433 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/__init__.py
+-rw-r--r--   0        0        0     8023 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/client.py
+-rw-r--r--   0        0        0      604 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/__init__.py
+-rw-r--r--   0        0        0      186 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule.py
+-rw-r--r--   0        0        0     1602 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_base.py
+-rw-r--r--   0        0        0     1046 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_config.py
+-rw-r--r--   0        0        0     1153 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_one_to_one.py
+-rw-r--r--   0        0        0      924 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_response.py
+-rw-r--r--   0        0        0      337 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_type.py
+-rw-r--r--   0        0        0      938 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rules_response.py
+-rw-r--r--   0        0        0     1441 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/__init__.py
+-rw-r--r--   0        0        0     1941 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/__init__.py
+-rw-r--r--   0        0        0      979 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/arrayable_property.py
+-rw-r--r--   0        0        0     1348 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/base_property.py
+-rw-r--r--   0        0        0     1126 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/boolean_property.py
+-rw-r--r--   0        0        0      987 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/boolean_property_config.py
+-rw-r--r--   0        0        0      927 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/constraint.py
+-rw-r--r--   0        0        0     1070 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/date_property.py
+-rw-r--r--   0        0        0     1580 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/enum_property.py
+-rw-r--r--   0        0        0     1110 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/enum_property_config.py
+-rw-r--r--   0        0        0     1699 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/enum_property_option.py
+-rw-r--r--   0        0        0     1061 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/number_config.py
+-rw-r--r--   0        0        0     1180 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/number_property.py
+-rw-r--r--   0        0        0     2450 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/property.py
+-rw-r--r--   0        0        0     1198 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/reference_property.py
+-rw-r--r--   0        0        0     1293 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/reference_property_config.py
+-rw-r--r--   0        0        0      526 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/reference_property_relationship.py
+-rw-r--r--   0        0        0      942 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/string_config.py
+-rw-r--r--   0        0        0      977 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/string_config_options.py
+-rw-r--r--   0        0        0     1109 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/string_property.py
+-rw-r--r--   0        0        0      974 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/unique_constraint.py
+-rw-r--r--   0        0        0     1093 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/property/types/unique_constraint_config.py
+-rw-r--r--   0        0        0     1053 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/__init__.py
+-rw-r--r--   0        0        0    32141 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/client.py
+-rw-r--r--   0        0        0     1584 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/__init__.py
+-rw-r--r--   0        0        0     1246 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/cell_value.py
+-rw-r--r--   0        0        0      182 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/cell_value_union.py
+-rw-r--r--   0        0        0      886 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/cell_value_with_links.py
+-rw-r--r--   0        0        0      154 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/diff_data.py
+-rw-r--r--   0        0        0      869 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/diff_record.py
+-rw-r--r--   0        0        0      155 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/diff_records.py
+-rw-r--r--   0        0        0      924 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/diff_records_response.py
+-rw-r--r--   0        0        0     1062 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/diff_value.py
+-rw-r--r--   0        0        0      958 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/get_records_response.py
+-rw-r--r--   0        0        0     1317 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/get_records_response_data.py
+-rw-r--r--   0        0        0      924 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/record.py
+-rw-r--r--   0        0        0     1300 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/record_base.py
+-rw-r--r--   0        0        0     1048 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/record_counts.py
+-rw-r--r--   0        0        0      156 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/record_data.py
+-rw-r--r--   0        0        0      194 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/record_data_with_links.py
+-rw-r--r--   0        0        0     1304 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/record_with_links.py
+-rw-r--r--   0        0        0      138 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/records.py
+-rw-r--r--   0        0        0      945 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/records_response.py
+-rw-r--r--   0        0        0     1264 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/records_response_data.py
+-rw-r--r--   0        0        0      176 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/records_with_links.py
+-rw-r--r--   0        0        0     1129 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/validation_message.py
+-rw-r--r--   0        0        0     1292 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/validation_source.py
+-rw-r--r--   0        0        0      611 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/records/types/validation_type.py
+-rw-r--r--   0        0        0      231 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/__init__.py
+-rw-r--r--   0        0        0     8774 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/client.py
+-rw-r--r--   0        0        0      335 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/types/__init__.py
+-rw-r--r--   0        0        0      923 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/types/secret.py
+-rw-r--r--   0        0        0      111 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/types/secret_name.py
+-rw-r--r--   0        0        0      112 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/types/secret_value.py
+-rw-r--r--   0        0        0      917 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/types/secrets_response.py
+-rw-r--r--   0        0        0     1447 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/secrets/types/write_secret.py
+-rw-r--r--   0        0        0      593 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/__init__.py
+-rw-r--r--   0        0        0    26335 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/client.py
+-rw-r--r--   0        0        0      855 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/__init__.py
+-rw-r--r--   0        0        0      931 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/field_config_response.py
+-rw-r--r--   0        0        0      917 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/list_sheets_response.py
+-rw-r--r--   0        0        0      966 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/record_counts_response.py
+-rw-r--r--   0        0        0      917 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/record_counts_response_data.py
+-rw-r--r--   0        0        0     1749 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet.py
+-rw-r--r--   0        0        0      856 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_access.py
+-rw-r--r--   0        0        0     1562 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_config.py
+-rw-r--r--   0        0        0      897 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_config_or_update.py
+-rw-r--r--   0        0        0     1602 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_config_update.py
+-rw-r--r--   0        0        0      899 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_response.py
+-rw-r--r--   0        0        0     1711 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_update.py
+-rw-r--r--   0        0        0      389 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/__init__.py
+-rw-r--r--   0        0        0    17979 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/client.py
+-rw-r--r--   0        0        0      529 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/__init__.py
+-rw-r--r--   0        0        0      783 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/change_type.py
+-rw-r--r--   0        0        0      913 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/restore_options.py
+-rw-r--r--   0        0        0     1363 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshot.py
+-rw-r--r--   0        0        0      911 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshot_response.py
+-rw-r--r--   0        0        0     1169 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshot_summary.py
+-rw-r--r--   0        0        0      925 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshots_response.py
+-rw-r--r--   0        0        0     1007 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/snapshots/types/summary_section.py
+-rw-r--r--   0        0        0      515 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/__init__.py
+-rw-r--r--   0        0        0    17971 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/client.py
+-rw-r--r--   0        0        0      733 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/__init__.py
+-rw-r--r--   0        0        0     1378 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/event_token.py
+-rw-r--r--   0        0        0      920 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/event_token_response.py
+-rw-r--r--   0        0        0     1264 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/get_spaces_sort_field.py
+-rw-r--r--   0        0        0     2124 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/internal_space_config_base.py
+-rw-r--r--   0        0        0     1055 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/list_spaces_response.py
+-rw-r--r--   0        0        0     2642 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/space.py
+-rw-r--r--   0        0        0      440 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/space_access.py
+-rw-r--r--   0        0        0     1451 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/space_config.py
+-rw-r--r--   0        0        0      899 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/space_response.py
+-rw-r--r--   0        0        0     1088 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/spaces/types/space_size.py
+-rw-r--r--   0        0        0      481 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/__init__.py
+-rw-r--r--   0        0        0    14523 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/client.py
+-rw-r--r--   0        0        0      679 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/__init__.py
+-rw-r--r--   0        0        0     1189 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/api_token.py
+-rw-r--r--   0        0        0      958 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/api_token_response.py
+-rw-r--r--   0        0        0     1301 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/exchange_token_data.py
+-rw-r--r--   0        0        0      945 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/exchange_token_response.py
+-rw-r--r--   0        0        0     1081 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/list_api_tokens_response.py
+-rw-r--r--   0        0        0      913 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/list_users_response.py
+-rw-r--r--   0        0        0      918 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/user.py
+-rw-r--r--   0        0        0     1100 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/user_config.py
+-rw-r--r--   0        0        0      895 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/users/types/user_response.py
+-rw-r--r--   0        0        0      151 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/versions/__init__.py
+-rw-r--r--   0        0        0     3583 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/versions/client.py
+-rw-r--r--   0        0        0      182 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/versions/types/__init__.py
+-rw-r--r--   0        0        0     1010 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/versions/types/version.py
+-rw-r--r--   0        0        0      907 2023-11-06 17:30:43.332272 flatfile-0.0.9/src/flatfile/resources/versions/types/version_response.py
+-rw-r--r--   0        0        0      389 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/__init__.py
+-rw-r--r--   0        0        0    44432 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/client.py
+-rw-r--r--   0        0        0      529 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/__init__.py
+-rw-r--r--   0        0        0     1752 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/create_workbook_config.py
+-rw-r--r--   0        0        0      929 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/list_workbooks_response.py
+-rw-r--r--   0        0        0     1992 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook.py
+-rw-r--r--   0        0        0     1334 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook_config_settings.py
+-rw-r--r--   0        0        0      911 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook_response.py
+-rw-r--r--   0        0        0     1680 2023-11-06 17:30:43.336272 flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook_update.py
+-rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 flatfile-0.0.9/PKG-INFO
```

### Comparing `flatfile-0.0.8/README.md` & `flatfile-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/__init__.py` & `flatfile-0.0.9/src/flatfile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .resources import (
     AccountId,
     Action,
+    ActionConstraint,
+    ActionConstraintType,
     ActionMode,
     ActionName,
     ActionSchedule,
     Agent,
     AgentConfig,
     AgentId,
     AgentLog,
@@ -211,14 +213,16 @@
     Mode,
     ModelFileStatusEnum,
     MutateJobConfig,
     NotFoundError,
     NumberConfig,
     NumberProperty,
     Origin,
+    PageNumber,
+    PageSize,
     Pagination,
     PipelineJobConfig,
     Progress,
     Property,
     Property_Boolean,
     Property_Date,
     Property_Enum,
@@ -275,14 +279,15 @@
     SpaceResponse,
     SpaceSize,
     StringConfig,
     StringConfigOptions,
     StringProperty,
     Success,
     SuccessData,
+    SuccessQueryParameter,
     SummarySection,
     Trigger,
     UniqueConstraint,
     UniqueConstraintConfig,
     User,
     UserConfig,
     UserId,
@@ -322,14 +327,16 @@
     workbooks,
 )
 from .environment import FlatfileEnvironment
 
 __all__ = [
     "AccountId",
     "Action",
+    "ActionConstraint",
+    "ActionConstraintType",
     "ActionMode",
     "ActionName",
     "ActionSchedule",
     "Agent",
     "AgentConfig",
     "AgentId",
     "AgentLog",
@@ -535,14 +542,16 @@
     "Mode",
     "ModelFileStatusEnum",
     "MutateJobConfig",
     "NotFoundError",
     "NumberConfig",
     "NumberProperty",
     "Origin",
+    "PageNumber",
+    "PageSize",
     "Pagination",
     "PipelineJobConfig",
     "Progress",
     "Property",
     "Property_Boolean",
     "Property_Date",
     "Property_Enum",
@@ -599,14 +608,15 @@
     "SpaceResponse",
     "SpaceSize",
     "StringConfig",
     "StringConfigOptions",
     "StringProperty",
     "Success",
     "SuccessData",
+    "SuccessQueryParameter",
     "SummarySection",
     "Trigger",
     "UniqueConstraint",
     "UniqueConstraintConfig",
     "User",
     "UserConfig",
     "UserId",
```

### Comparing `flatfile-0.0.8/src/flatfile/client.py` & `flatfile-0.0.9/src/flatfile/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/core/__init__.py` & `flatfile-0.0.9/src/flatfile/core/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/core/client_wrapper.py` & `flatfile-0.0.9/src/flatfile/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "flatfile",
-            "X-Fern-SDK-Version": "0.0.8",
+            "X-Fern-SDK-Version": "0.0.9",
         }
         headers["X-Disable-Hooks"] = self._x_disable_hooks
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
```

### Comparing `flatfile-0.0.8/src/flatfile/core/datetime_utils.py` & `flatfile-0.0.9/src/flatfile/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/core/jsonable_encoder.py` & `flatfile-0.0.9/src/flatfile/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 )
 from .auth import ApiKey, ApiKeyOperation, ApiKeyType, ApiKeysResponse
 from .cells import CellValueWithCounts, CellsResponse, CellsResponseData
 from .commits import Commit, CommitResponse, ListCommitsResponse
 from .commons import (
     AccountId,
     Action,
+    ActionConstraint,
+    ActionConstraintType,
     ActionMode,
     ActionSchedule,
     AgentId,
     BadRequestError,
     DocumentId,
     EnvironmentId,
     Error,
@@ -62,27 +64,30 @@
     InputEnumPropertyOption,
     InputField,
     InputForm,
     InputFormType,
     JobId,
     MappingId,
     NotFoundError,
+    PageNumber,
+    PageSize,
     Pagination,
     RecordId,
     SearchField,
     SearchValue,
     SecretId,
     SheetId,
     SnapshotId,
     SortDirection,
     SortField,
     SpaceConfigId,
     SpaceId,
     Success,
     SuccessData,
+    SuccessQueryParameter,
     UserId,
     VersionId,
     WorkbookId,
 )
 from .documents import Document, DocumentConfig, DocumentResponse, ListDocumentsResponse
 from .environments import (
     Environment,
@@ -330,14 +335,16 @@
     WorkbookResponse,
     WorkbookUpdate,
 )
 
 __all__ = [
     "AccountId",
     "Action",
+    "ActionConstraint",
+    "ActionConstraintType",
     "ActionMode",
     "ActionName",
     "ActionSchedule",
     "Agent",
     "AgentConfig",
     "AgentId",
     "AgentLog",
@@ -542,14 +549,16 @@
     "Mode",
     "ModelFileStatusEnum",
     "MutateJobConfig",
     "NotFoundError",
     "NumberConfig",
     "NumberProperty",
     "Origin",
+    "PageNumber",
+    "PageSize",
     "Pagination",
     "PipelineJobConfig",
     "Progress",
     "Property",
     "Property_Boolean",
     "Property_Date",
     "Property_Enum",
@@ -606,14 +615,15 @@
     "SpaceResponse",
     "SpaceSize",
     "StringConfig",
     "StringConfigOptions",
     "StringProperty",
     "Success",
     "SuccessData",
+    "SuccessQueryParameter",
     "SummarySection",
     "Trigger",
     "UniqueConstraint",
     "UniqueConstraintConfig",
     "User",
     "UserConfig",
     "UserId",
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/client.py` & `flatfile-0.0.9/src/flatfile/resources/agents/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.errors.not_found_error import NotFoundError
 from ..commons.types.agent_id import AgentId
 from ..commons.types.environment_id import EnvironmentId
 from ..commons.types.errors import Errors
 from ..commons.types.event_id import EventId
+from ..commons.types.page_number import PageNumber
+from ..commons.types.page_size import PageSize
 from ..commons.types.space_id import SpaceId
 from ..commons.types.success import Success
+from ..commons.types.success_query_parameter import SuccessQueryParameter
 from .types.agent_config import AgentConfig
 from .types.agent_response import AgentResponse
 from .types.get_agent_logs_response import GetAgentLogsResponse
 from .types.get_detailed_agent_log_response import GetDetailedAgentLogResponse
 from .types.get_detailed_agent_logs_response import GetDetailedAgentLogsResponse
 from .types.get_executions_response import GetExecutionsResponse
 from .types.list_agents_response import ListAgentsResponse
@@ -45,15 +48,15 @@
         from flatfile.client import Flatfile
 
         client = Flatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         client.list(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
@@ -78,15 +81,15 @@
         from flatfile.client import Flatfile
 
         client = Flatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         client.create(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
             request=AgentConfig(
                 topics=[EventTopic.FILE_CREATED],
                 compiler=Compiler.JS,
                 source="module.exports = { routeEvent: async (...args) => { console.log(args) } }",
             ),
         )
         """
@@ -118,16 +121,16 @@
         from flatfile.client import Flatfile
 
         client = Flatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         client.get(
-            agent_id="us_ag_qGZbKwDW",
-            environment_id="us_env_hVXkXs0b",
+            agent_id="us_ag_YOUR_ID",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
@@ -155,16 +158,16 @@
         from flatfile.client import Flatfile
 
         client = Flatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         client.get_agent_logs(
-            agent_id="us_ag_qGZbKwDW",
-            environment_id="us_env_hVXkXs0b",
+            agent_id="us_ag_YOUR_ID",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}/logs"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
@@ -184,18 +187,29 @@
 
     def get_agent_log(self, event_id: EventId, *, environment_id: EnvironmentId) -> GetDetailedAgentLogResponse:
         """
         Parameters:
             - event_id: EventId.
 
             - environment_id: EnvironmentId.
+        ---
+        from flatfile.client import Flatfile
+
+        client = Flatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        client.get_agent_log(
+            event_id="commons.EventId",
+            environment_id="us_env_YOUR_ID",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/logs/{event_id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/log/{event_id}"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetDetailedAgentLogResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -208,30 +222,44 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_environment_agent_logs(
         self,
         *,
         environment_id: EnvironmentId,
-        space_id: SpaceId,
-        success: typing.Optional[bool] = None,
-        page_size: typing.Optional[int] = None,
-        page_number: typing.Optional[int] = None,
+        space_id: typing.Optional[SpaceId] = None,
+        success: typing.Optional[SuccessQueryParameter] = None,
+        page_size: typing.Optional[PageSize] = None,
+        page_number: typing.Optional[PageNumber] = None,
     ) -> GetDetailedAgentLogsResponse:
         """
         Parameters:
             - environment_id: EnvironmentId.
 
-            - space_id: SpaceId.
+            - space_id: typing.Optional[SpaceId].
+
+            - success: typing.Optional[SuccessQueryParameter].
 
-            - success: typing.Optional[bool].
+            - page_size: typing.Optional[PageSize].
 
-            - page_size: typing.Optional[int]. Number of logs to return in a page (default 20)
+            - page_number: typing.Optional[PageNumber].
+        ---
+        from flatfile.client import Flatfile
 
-            - page_number: typing.Optional[int]. Based on pageSize, which page of records to return
+        client = Flatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        client.get_environment_agent_logs(
+            environment_id="us_env_YOUR_ID",
+            space_id="us_sp_YOUR_ID",
+            success=True,
+            page_size=20,
+            page_number=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents/logs"),
             params=remove_none_from_dict(
                 {
                     "environmentId": environment_id,
@@ -256,30 +284,44 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_environment_agent_executions(
         self,
         *,
         environment_id: EnvironmentId,
-        space_id: SpaceId,
-        success: typing.Optional[bool] = None,
-        page_size: typing.Optional[int] = None,
-        page_number: typing.Optional[int] = None,
+        space_id: typing.Optional[SpaceId] = None,
+        success: typing.Optional[SuccessQueryParameter] = None,
+        page_size: typing.Optional[PageSize] = None,
+        page_number: typing.Optional[PageNumber] = None,
     ) -> GetExecutionsResponse:
         """
         Parameters:
             - environment_id: EnvironmentId.
 
-            - space_id: SpaceId.
+            - space_id: typing.Optional[SpaceId].
 
-            - success: typing.Optional[bool].
+            - success: typing.Optional[SuccessQueryParameter].
 
-            - page_size: typing.Optional[int]. Number of logs to return in a page (default 20)
+            - page_size: typing.Optional[PageSize].
 
-            - page_number: typing.Optional[int]. Based on pageSize, which page of records to return
+            - page_number: typing.Optional[PageNumber].
+        ---
+        from flatfile.client import Flatfile
+
+        client = Flatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        client.get_environment_agent_executions(
+            environment_id="us_env_YOUR_ID",
+            space_id="us_sp_YOUR_ID",
+            success=True,
+            page_size=20,
+            page_number=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents/executions"),
             params=remove_none_from_dict(
                 {
                     "environmentId": environment_id,
@@ -300,24 +342,38 @@
             raise NotFoundError(pydantic.parse_obj_as(Errors, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, agent_id: AgentId) -> Success:
+    def delete(self, agent_id: AgentId, *, environment_id: EnvironmentId) -> Success:
         """
         Deletes a single agent
 
         Parameters:
             - agent_id: AgentId.
+
+            - environment_id: EnvironmentId.
+        ---
+        from flatfile.client import Flatfile
+
+        client = Flatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        client.delete(
+            agent_id="us_ag_YOUR_ID",
+            environment_id="us_env_YOUR_ID",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"),
+            params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Success, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(Errors, _response.json()))  # type: ignore
@@ -342,15 +398,15 @@
         from flatfile.client import AsyncFlatfile
 
         client = AsyncFlatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         await client.list(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
@@ -375,15 +431,15 @@
         from flatfile.client import AsyncFlatfile
 
         client = AsyncFlatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         await client.create(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
             request=AgentConfig(
                 topics=[EventTopic.FILE_CREATED],
                 compiler=Compiler.JS,
                 source="module.exports = { routeEvent: async (...args) => { console.log(args) } }",
             ),
         )
         """
@@ -415,16 +471,16 @@
         from flatfile.client import AsyncFlatfile
 
         client = AsyncFlatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         await client.get(
-            agent_id="us_ag_qGZbKwDW",
-            environment_id="us_env_hVXkXs0b",
+            agent_id="us_ag_YOUR_ID",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
@@ -452,16 +508,16 @@
         from flatfile.client import AsyncFlatfile
 
         client = AsyncFlatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         await client.get_agent_logs(
-            agent_id="us_ag_qGZbKwDW",
-            environment_id="us_env_hVXkXs0b",
+            agent_id="us_ag_YOUR_ID",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}/logs"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
@@ -481,18 +537,29 @@
 
     async def get_agent_log(self, event_id: EventId, *, environment_id: EnvironmentId) -> GetDetailedAgentLogResponse:
         """
         Parameters:
             - event_id: EventId.
 
             - environment_id: EnvironmentId.
+        ---
+        from flatfile.client import AsyncFlatfile
+
+        client = AsyncFlatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        await client.get_agent_log(
+            event_id="commons.EventId",
+            environment_id="us_env_YOUR_ID",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/logs/{event_id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/log/{event_id}"),
             params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetDetailedAgentLogResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -505,30 +572,44 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_environment_agent_logs(
         self,
         *,
         environment_id: EnvironmentId,
-        space_id: SpaceId,
-        success: typing.Optional[bool] = None,
-        page_size: typing.Optional[int] = None,
-        page_number: typing.Optional[int] = None,
+        space_id: typing.Optional[SpaceId] = None,
+        success: typing.Optional[SuccessQueryParameter] = None,
+        page_size: typing.Optional[PageSize] = None,
+        page_number: typing.Optional[PageNumber] = None,
     ) -> GetDetailedAgentLogsResponse:
         """
         Parameters:
             - environment_id: EnvironmentId.
 
-            - space_id: SpaceId.
+            - space_id: typing.Optional[SpaceId].
+
+            - success: typing.Optional[SuccessQueryParameter].
 
-            - success: typing.Optional[bool].
+            - page_size: typing.Optional[PageSize].
 
-            - page_size: typing.Optional[int]. Number of logs to return in a page (default 20)
+            - page_number: typing.Optional[PageNumber].
+        ---
+        from flatfile.client import AsyncFlatfile
 
-            - page_number: typing.Optional[int]. Based on pageSize, which page of records to return
+        client = AsyncFlatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        await client.get_environment_agent_logs(
+            environment_id="us_env_YOUR_ID",
+            space_id="us_sp_YOUR_ID",
+            success=True,
+            page_size=20,
+            page_number=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents/logs"),
             params=remove_none_from_dict(
                 {
                     "environmentId": environment_id,
@@ -553,30 +634,44 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_environment_agent_executions(
         self,
         *,
         environment_id: EnvironmentId,
-        space_id: SpaceId,
-        success: typing.Optional[bool] = None,
-        page_size: typing.Optional[int] = None,
-        page_number: typing.Optional[int] = None,
+        space_id: typing.Optional[SpaceId] = None,
+        success: typing.Optional[SuccessQueryParameter] = None,
+        page_size: typing.Optional[PageSize] = None,
+        page_number: typing.Optional[PageNumber] = None,
     ) -> GetExecutionsResponse:
         """
         Parameters:
             - environment_id: EnvironmentId.
 
-            - space_id: SpaceId.
+            - space_id: typing.Optional[SpaceId].
 
-            - success: typing.Optional[bool].
+            - success: typing.Optional[SuccessQueryParameter].
 
-            - page_size: typing.Optional[int]. Number of logs to return in a page (default 20)
+            - page_size: typing.Optional[PageSize].
 
-            - page_number: typing.Optional[int]. Based on pageSize, which page of records to return
+            - page_number: typing.Optional[PageNumber].
+        ---
+        from flatfile.client import AsyncFlatfile
+
+        client = AsyncFlatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        await client.get_environment_agent_executions(
+            environment_id="us_env_YOUR_ID",
+            space_id="us_sp_YOUR_ID",
+            success=True,
+            page_size=20,
+            page_number=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents/executions"),
             params=remove_none_from_dict(
                 {
                     "environmentId": environment_id,
@@ -597,24 +692,38 @@
             raise NotFoundError(pydantic.parse_obj_as(Errors, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, agent_id: AgentId) -> Success:
+    async def delete(self, agent_id: AgentId, *, environment_id: EnvironmentId) -> Success:
         """
         Deletes a single agent
 
         Parameters:
             - agent_id: AgentId.
+
+            - environment_id: EnvironmentId.
+        ---
+        from flatfile.client import AsyncFlatfile
+
+        client = AsyncFlatfile(
+            x_disable_hooks="YOUR_X_DISABLE_HOOKS",
+            token="YOUR_TOKEN",
+        )
+        await client.delete(
+            agent_id="us_ag_YOUR_ID",
+            environment_id="us_env_YOUR_ID",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"),
+            params=remove_none_from_dict({"environmentId": environment_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Success, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(Errors, _response.json()))  # type: ignore
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/agent.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Agent(AgentConfig):
     """
     from flatfile import Agent, Compiler, EventTopic
 
     Agent(
-        id="123",
+        id="us_ag_YOUR_ID",
         topics=[EventTopic.FILE_CREATED],
         compiler=Compiler.JS,
         source="module.exports = { routeEvent: async (...args) => { console.log(args) } }",
     )
     """
 
     id: AgentId
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/agent_config.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/agent_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/agent_log.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/agent_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class AgentLog(pydantic.BaseModel):
     """
     A log of an agent execution
     ---
     from flatfile import AgentLog
 
     AgentLog(
-        event_id="us_evt_9cuesESa7W9cuesE",
+        event_id="us_evt_YOUR_ID",
         success=True,
         created_at="2022-09-18T00:19:57.007Z",
         completed_at="2022-09-18T00:20:04.007Z",
         log="SUCCESS",
     )
     """
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/agent_response.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/agent_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class AgentResponse(pydantic.BaseModel):
     """
     from flatfile import Agent, AgentResponse, Compiler, EventTopic
 
     AgentResponse(
         data=Agent(
-            id="123",
+            id="us_ag_YOUR_ID",
             topics=[EventTopic.FILE_CREATED],
             compiler=Compiler.JS,
             source="module.exports = { routeEvent: async (...args) => { console.log(args) } }",
         ),
     )
     """
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/detailed_agent_log.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/detailed_agent_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     A log of an agent execution
     ---
     import datetime
 
     from flatfile import DetailedAgentLog
 
     DetailedAgentLog(
-        event_id="us_evt_9cuesESa7W9cuesE",
+        event_id="us_evt_YOUR_ID",
         success=True,
         created_at=datetime.datetime.fromisoformat(
             "2022-09-18 00:19:57.007000+00:00",
         ),
         completed_at=datetime.datetime.fromisoformat(
             "2022-09-18 00:20:04.007000+00:00",
         ),
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/execution.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     An execution of an agent
     ---
     import datetime
 
     from flatfile import Execution
 
     Execution(
-        event_id="us_evt_9cuesESa7W9cuesE",
+        event_id="us_evt_YOUR_ID",
         success=True,
         created_at=datetime.datetime.fromisoformat(
             "2022-09-18 00:19:57.007000+00:00",
         ),
         completed_at=datetime.datetime.fromisoformat(
             "2022-09-18 00:20:04.007000+00:00",
         ),
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/get_agent_logs_response.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/get_agent_logs_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         pagination=Pagination(
             current_page=3,
             page_count=50,
             total_count=100,
         ),
         data=[
             AgentLog(
-                event_id="us_evt_9cuesESa7W9cuesE",
+                event_id="us_evt_YOUR_ID",
                 success=True,
                 created_at="2022-09-18T00:19:57.007Z",
                 completed_at="2022-09-18T00:20:04.007Z",
                 log="SUCCESS",
             )
         ],
     )
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/get_detailed_agent_log_response.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/guest_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .detailed_agent_log import DetailedAgentLog
+from .guest import Guest
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetDetailedAgentLogResponse(pydantic.BaseModel):
-    data: DetailedAgentLog
+class GuestResponse(pydantic.BaseModel):
+    data: Guest
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/get_detailed_agent_logs_response.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/get_detailed_agent_logs_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         pagination=Pagination(
             current_page=3,
             page_count=50,
             total_count=100,
         ),
         data=[
             DetailedAgentLog(
-                event_id="us_evt_9cuesESa7W9cuesE",
+                event_id="us_evt_YOUR_ID",
                 success=True,
                 created_at=datetime.datetime.fromisoformat(
                     "2022-09-18 00:19:57.007000+00:00",
                 ),
                 completed_at=datetime.datetime.fromisoformat(
                     "2022-09-18 00:20:04.007000+00:00",
                 ),
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/get_executions_response.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/get_executions_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         pagination=Pagination(
             current_page=3,
             page_count=50,
             total_count=100,
         ),
         data=[
             Execution(
-                event_id="us_evt_9cuesESa7W9cuesE",
+                event_id="us_evt_YOUR_ID",
                 success=True,
                 created_at=datetime.datetime.fromisoformat(
                     "2022-09-18 00:19:57.007000+00:00",
                 ),
                 completed_at=datetime.datetime.fromisoformat(
                     "2022-09-18 00:20:04.007000+00:00",
                 ),
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/agents/types/list_agents_response.py` & `flatfile-0.0.9/src/flatfile/resources/agents/types/list_agents_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class ListAgentsResponse(pydantic.BaseModel):
     """
     from flatfile import Agent, Compiler, EventTopic, ListAgentsResponse
 
     ListAgentsResponse(
         data=[
             Agent(
-                id="123",
+                id="us_ag_YOUR_ID",
                 topics=[EventTopic.FILE_CREATED],
                 compiler=Compiler.JS,
                 source="module.exports = { routeEvent: async (...args) => { console.log(args) } }",
             )
         ],
     )
     """
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/auth/client.py` & `flatfile-0.0.9/src/flatfile/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/auth/types/api_key.py` & `flatfile-0.0.9/src/flatfile/resources/auth/types/api_key.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/auth/types/api_key_operation.py` & `flatfile-0.0.9/src/flatfile/resources/auth/types/api_key_operation.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/auth/types/api_keys_response.py` & `flatfile-0.0.9/src/flatfile/resources/auth/types/api_keys_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/cells/client.py` & `flatfile-0.0.9/src/flatfile/resources/cells/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/cells/types/cell_value_with_counts.py` & `flatfile-0.0.9/src/flatfile/resources/cells/types/cell_value_with_counts.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/cells/types/cells_response.py` & `flatfile-0.0.9/src/flatfile/resources/cells/types/cells_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commits/client.py` & `flatfile-0.0.9/src/flatfile/resources/commits/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commits/types/commit.py` & `flatfile-0.0.9/src/flatfile/resources/commits/types/commit.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commits/types/commit_response.py` & `flatfile-0.0.9/src/flatfile/resources/commits/types/commit_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commits/types/list_commits_response.py` & `flatfile-0.0.9/src/flatfile/resources/commits/types/list_commits_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/commons/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     AccountId,
     Action,
+    ActionConstraint,
+    ActionConstraintType,
     ActionMode,
     ActionSchedule,
     AgentId,
     DocumentId,
     EnvironmentId,
     Error,
     Errors,
@@ -20,36 +22,41 @@
     InputConstraintType,
     InputEnumPropertyOption,
     InputField,
     InputForm,
     InputFormType,
     JobId,
     MappingId,
+    PageNumber,
+    PageSize,
     Pagination,
     RecordId,
     SearchField,
     SearchValue,
     SecretId,
     SheetId,
     SnapshotId,
     SortDirection,
     SortField,
     SpaceConfigId,
     SpaceId,
     Success,
     SuccessData,
+    SuccessQueryParameter,
     UserId,
     VersionId,
     WorkbookId,
 )
 from .errors import BadRequestError, NotFoundError
 
 __all__ = [
     "AccountId",
     "Action",
+    "ActionConstraint",
+    "ActionConstraintType",
     "ActionMode",
     "ActionSchedule",
     "AgentId",
     "BadRequestError",
     "DocumentId",
     "EnvironmentId",
     "Error",
@@ -65,24 +72,27 @@
     "InputEnumPropertyOption",
     "InputField",
     "InputForm",
     "InputFormType",
     "JobId",
     "MappingId",
     "NotFoundError",
+    "PageNumber",
+    "PageSize",
     "Pagination",
     "RecordId",
     "SearchField",
     "SearchValue",
     "SecretId",
     "SheetId",
     "SnapshotId",
     "SortDirection",
     "SortField",
     "SpaceConfigId",
     "SpaceId",
     "Success",
     "SuccessData",
+    "SuccessQueryParameter",
     "UserId",
     "VersionId",
     "WorkbookId",
 ]
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .errors import Errors
 from .account_id import AccountId
 from .action import Action
+from .action_constraint import ActionConstraint
+from .action_constraint_type import ActionConstraintType
 from .action_mode import ActionMode
 from .action_schedule import ActionSchedule
 from .agent_id import AgentId
 from .document_id import DocumentId
 from .environment_id import EnvironmentId
 from .error import Error
 from .event_id import EventId
@@ -19,34 +21,39 @@
 from .input_constraint_type import InputConstraintType
 from .input_enum_property_option import InputEnumPropertyOption
 from .input_field import InputField
 from .input_form import InputForm
 from .input_form_type import InputFormType
 from .job_id import JobId
 from .mapping_id import MappingId
+from .page_number import PageNumber
+from .page_size import PageSize
 from .pagination import Pagination
 from .record_id import RecordId
 from .search_field import SearchField
 from .search_value import SearchValue
 from .secret_id import SecretId
 from .sheet_id import SheetId
 from .snapshot_id import SnapshotId
 from .sort_direction import SortDirection
 from .sort_field import SortField
 from .space_config_id import SpaceConfigId
 from .space_id import SpaceId
 from .success import Success
 from .success_data import SuccessData
+from .success_query_parameter import SuccessQueryParameter
 from .user_id import UserId
 from .version_id import VersionId
 from .workbook_id import WorkbookId
 
 __all__ = [
     "AccountId",
     "Action",
+    "ActionConstraint",
+    "ActionConstraintType",
     "ActionMode",
     "ActionSchedule",
     "AgentId",
     "DocumentId",
     "EnvironmentId",
     "Error",
     "Errors",
@@ -60,24 +67,27 @@
     "InputConstraintType",
     "InputEnumPropertyOption",
     "InputField",
     "InputForm",
     "InputFormType",
     "JobId",
     "MappingId",
+    "PageNumber",
+    "PageSize",
     "Pagination",
     "RecordId",
     "SearchField",
     "SearchValue",
     "SecretId",
     "SheetId",
     "SnapshotId",
     "SortDirection",
     "SortField",
     "SpaceConfigId",
     "SpaceId",
     "Success",
     "SuccessData",
+    "SuccessQueryParameter",
     "UserId",
     "VersionId",
     "WorkbookId",
 ]
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/action.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from .action_constraint import ActionConstraint
 from .action_mode import ActionMode
 from .action_schedule import ActionSchedule
 from .input_form import InputForm
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
@@ -25,14 +26,15 @@
     schedule: typing.Optional[ActionSchedule]
     primary: typing.Optional[bool]
     confirm: typing.Optional[bool]
     icon: typing.Optional[str]
     require_all_valid: typing.Optional[bool] = pydantic.Field(alias="requireAllValid")
     require_selection: typing.Optional[bool] = pydantic.Field(alias="requireSelection")
     input_form: typing.Optional[InputForm] = pydantic.Field(alias="inputForm")
+    constraints: typing.Optional[typing.List[ActionConstraint]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/action_mode.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/action_mode.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/action_schedule.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/action_schedule.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/error.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/error.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/errors.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/errors.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/filter.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/filter.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/input_config.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/input_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/input_constraint.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/input_constraint.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/input_enum_property_option.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/input_enum_property_option.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/input_field.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/input_field.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/input_form.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/input_form.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/pagination.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/pagination.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/sort_direction.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/sort_direction.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/success.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/success.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/commons/types/success_data.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/success_data.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/documents/client.py` & `flatfile-0.0.9/src/flatfile/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/documents/types/document.py` & `flatfile-0.0.9/src/flatfile/resources/documents/types/document.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/documents/types/document_config.py` & `flatfile-0.0.9/src/flatfile/resources/documents/types/document_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/documents/types/document_response.py` & `flatfile-0.0.9/src/flatfile/resources/documents/types/document_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/documents/types/list_documents_response.py` & `flatfile-0.0.9/src/flatfile/resources/documents/types/list_documents_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/client.py` & `flatfile-0.0.9/src/flatfile/resources/environments/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         from flatfile.client import Flatfile
 
         client = Flatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         client.get(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"environments/{environment_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -180,15 +180,15 @@
         from flatfile.client import Flatfile
 
         client = Flatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         client.update(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
             request=EnvironmentConfigUpdate(
                 name="dev",
                 is_prod=False,
                 guest_authentication=[GuestAuthenticationEnum.MAGIC_LINK],
                 metadata={"key": "value"},
                 namespaces=["default"],
             ),
@@ -348,15 +348,15 @@
         from flatfile.client import AsyncFlatfile
 
         client = AsyncFlatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         await client.get(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"environments/{environment_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -386,15 +386,15 @@
         from flatfile.client import AsyncFlatfile
 
         client = AsyncFlatfile(
             x_disable_hooks="YOUR_X_DISABLE_HOOKS",
             token="YOUR_TOKEN",
         )
         await client.update(
-            environment_id="us_env_hVXkXs0b",
+            environment_id="us_env_YOUR_ID",
             request=EnvironmentConfigUpdate(
                 name="dev",
                 is_prod=False,
                 guest_authentication=[GuestAuthenticationEnum.MAGIC_LINK],
                 metadata={"key": "value"},
                 namespaces=["default"],
             ),
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/environment.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 
 class Environment(pydantic.BaseModel):
     """
     from flatfile import Environment, GuestAuthenticationEnum
 
     Environment(
-        id="us_env_hVXkXs0b",
-        account_id="us_acc_uj6s91wc",
+        id="us_env_YOUR_ID",
+        account_id="us_acc_YOUR_ID",
         name="dev",
         is_prod=False,
         guest_authentication=[GuestAuthenticationEnum.MAGIC_LINK],
         features={},
         metadata={},
         namespaces=["default"],
     )
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/environment_config_create.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/environment_config_create.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/environment_config_update.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/environment_config_update.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/environment_response.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/environment_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/guest_authentication_enum.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/guest_authentication_enum.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/environments/types/list_environments_response.py` & `flatfile-0.0.9/src/flatfile/resources/environments/types/list_environments_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/events/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/client.py` & `flatfile-0.0.9/src/flatfile/resources/events/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/base_event.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/base_event.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/context.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     environment_id: EnvironmentId = pydantic.Field(alias="environmentId")
     space_id: typing.Optional[SpaceId] = pydantic.Field(alias="spaceId")
     workbook_id: typing.Optional[WorkbookId] = pydantic.Field(alias="workbookId")
     sheet_id: typing.Optional[SheetId] = pydantic.Field(alias="sheetId")
     sheet_slug: typing.Optional[SheetSlug] = pydantic.Field(alias="sheetSlug")
     snapshot_id: typing.Optional[SnapshotId] = pydantic.Field(alias="snapshotId")
     version_id: typing.Optional[VersionId] = pydantic.Field(alias="versionId")
+    commit_id: typing.Optional[VersionId] = pydantic.Field(alias="commitId")
     job_id: typing.Optional[JobId] = pydantic.Field(alias="jobId")
     file_id: typing.Optional[FileId] = pydantic.Field(alias="fileId")
     document_id: typing.Optional[DocumentId] = pydantic.Field(alias="documentId")
     preceding_event_id: typing.Optional[EventId] = pydantic.Field(alias="precedingEventId")
     actor_id: typing.Optional[str] = pydantic.Field(alias="actorId", description="Can be a UserId, GuestId, or AgentId")
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/create_event_config.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/create_event_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/domain.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/domain.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/event.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/event.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/event_attributes.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/event_attributes.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/event_context_slugs.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/event_context_slugs.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/event_response.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/event_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/event_topic.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/event_topic.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/generic_event.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/generic_event.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/list_all_events_response.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/list_all_events_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/origin.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/origin.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/events/types/progress.py` & `flatfile-0.0.9/src/flatfile/resources/events/types/progress.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/files/client.py` & `flatfile-0.0.9/src/flatfile/resources/files/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/files/types/file.py` & `flatfile-0.0.9/src/flatfile/resources/files/types/file.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/files/types/file_response.py` & `flatfile-0.0.9/src/flatfile/resources/files/types/file_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/files/types/list_files_response.py` & `flatfile-0.0.9/src/flatfile/resources/files/types/list_files_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/files/types/model_file_status_enum.py` & `flatfile-0.0.9/src/flatfile/resources/files/types/model_file_status_enum.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/client.py` & `flatfile-0.0.9/src/flatfile/resources/guests/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/create_guest_response.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/create_guest_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/guest.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/guest.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/guest_config.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/guest_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/guest_config_update.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/guest_config_update.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/guest_response.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/list_guests_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GuestResponse(pydantic.BaseModel):
-    data: Guest
+class ListGuestsResponse(pydantic.BaseModel):
+    data: typing.List[Guest]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/guest_space.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/guest_space.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/guest_workbook.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/guest_workbook.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/invite.py` & `flatfile-0.0.9/src/flatfile/resources/guests/types/invite.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/guests/types/list_guests_response.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshots_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .guest import Guest
+from .snapshot import Snapshot
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ListGuestsResponse(pydantic.BaseModel):
-    data: typing.List[Guest]
+class SnapshotsResponse(pydantic.BaseModel):
+    data: typing.List[Snapshot]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/client.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/category_mapping.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/category_mapping.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/certainty.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/certainty.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/collection_job_subject.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/collection_job_subject.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/delete_records_job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/delete_records_job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/destination_field.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/destination_field.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/edge.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/edge.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/empty_object.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/empty_object.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/enum_details.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/enum_details.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/export_job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/export_job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/export_options.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/export_options.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/file_job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/file_job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/find_and_replace_job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/find_and_replace_job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_ack_details.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_ack_details.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_cancel_details.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_cancel_details.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_complete_details.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_complete_details.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan_config_request.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan_config_request.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_execution_plan_request.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_execution_plan_request.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_mode.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_mode.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_download.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_download.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_id.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_id.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_url.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_url.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_outcome_next_wait.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_outcome_next_wait.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_plan.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_plan.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_plan_response.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_plan_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_response.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_status.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_status.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_subject.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_subject.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_type.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_type.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_update.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_update.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/job_update_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/job_update_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/list_jobs_response.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/metadata.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/metadata.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/mutate_job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/mutate_job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/pipeline_job_config.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/pipeline_job_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/resource_job_subject.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/resource_job_subject.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/source_field.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/source_field.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/jobs/types/trigger.py` & `flatfile-0.0.9/src/flatfile/resources/jobs/types/trigger.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/client.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_base.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_base.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_config.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_one_to_one.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_one_to_one.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rule_response.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rule_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/mapping/types/mapping_rules_response.py` & `flatfile-0.0.9/src/flatfile/resources/mapping/types/mapping_rules_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/property/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/arrayable_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/arrayable_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/base_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/base_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/boolean_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/boolean_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/boolean_property_config.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/boolean_property_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/constraint.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/constraint.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/date_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/date_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/enum_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/enum_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/enum_property_config.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/enum_property_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/enum_property_option.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/enum_property_option.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/number_config.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/number_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/number_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/number_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/reference_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/reference_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/reference_property_config.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/reference_property_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/reference_property_relationship.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/reference_property_relationship.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/string_config.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/string_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/string_config_options.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/string_config_options.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/string_property.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/string_property.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/unique_constraint.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/unique_constraint.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/property/types/unique_constraint_config.py` & `flatfile-0.0.9/src/flatfile/resources/property/types/unique_constraint_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/client.py` & `flatfile-0.0.9/src/flatfile/resources/records/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/cell_value.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/cell_value.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/cell_value_with_links.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/cell_value_with_links.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/diff_record.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/diff_record.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/diff_records_response.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/diff_records_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/diff_value.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/diff_value.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/get_records_response.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/get_records_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/get_records_response_data.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/get_records_response_data.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/record.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/record.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/record_base.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/record_base.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/record_counts.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/record_counts.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/record_with_links.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/record_with_links.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/records_response.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/records_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/records_response_data.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/records_response_data.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/validation_message.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/validation_message.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/validation_source.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/validation_source.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/records/types/validation_type.py` & `flatfile-0.0.9/src/flatfile/resources/records/types/validation_type.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/secrets/client.py` & `flatfile-0.0.9/src/flatfile/resources/secrets/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/secrets/types/secret.py` & `flatfile-0.0.9/src/flatfile/resources/secrets/types/secret.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/secrets/types/secrets_response.py` & `flatfile-0.0.9/src/flatfile/resources/secrets/types/secrets_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/secrets/types/write_secret.py` & `flatfile-0.0.9/src/flatfile/resources/secrets/types/write_secret.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/client.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/field_config_response.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/field_config_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/list_sheets_response.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/list_sheets_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/record_counts_response.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/record_counts_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/record_counts_response_data.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/record_counts_response_data.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_access.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_access.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_config.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """
 
     name: str
     description: typing.Optional[str]
     slug: typing.Optional[str]
     readonly: typing.Optional[bool]
     allow_additional_fields: typing.Optional[bool] = pydantic.Field(alias="allowAdditionalFields")
+    mapping_confidence_threshold: typing.Optional[float] = pydantic.Field(alias="mappingConfidenceThreshold")
     access: typing.Optional[typing.List[SheetAccess]]
     fields: typing.List[Property]
     actions: typing.Optional[typing.List[Action]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_config_or_update.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_config_or_update.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_config_update.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_config_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """
 
     name: typing.Optional[str]
     description: typing.Optional[str]
     slug: typing.Optional[str]
     readonly: typing.Optional[bool]
     allow_additional_fields: typing.Optional[bool] = pydantic.Field(alias="allowAdditionalFields")
+    mapping_confidence_threshold: typing.Optional[float] = pydantic.Field(alias="mappingConfidenceThreshold")
     access: typing.Optional[typing.List[SheetAccess]]
     fields: typing.Optional[typing.List[Property]]
     actions: typing.Optional[typing.List[Action]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_response.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/sheets/types/sheet_update.py` & `flatfile-0.0.9/src/flatfile/resources/sheets/types/sheet_update.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/client.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/change_type.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/change_type.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/restore_options.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/restore_options.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshot.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshot.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshot_response.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshot_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshot_summary.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/snapshot_summary.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/snapshots_response.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/event_token_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .snapshot import Snapshot
+from .event_token import EventToken
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SnapshotsResponse(pydantic.BaseModel):
-    data: typing.List[Snapshot]
+class EventTokenResponse(pydantic.BaseModel):
+    data: EventToken
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/snapshots/types/summary_section.py` & `flatfile-0.0.9/src/flatfile/resources/snapshots/types/summary_section.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/client.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/event_token.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/event_token.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/event_token_response.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/list_users_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .event_token import EventToken
+from .user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class EventTokenResponse(pydantic.BaseModel):
-    data: EventToken
+class ListUsersResponse(pydantic.BaseModel):
+    data: typing.List[User]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/get_spaces_sort_field.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/get_spaces_sort_field.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/internal_space_config_base.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/internal_space_config_base.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/list_spaces_response.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/list_spaces_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/space.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/space.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/space_config.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/space_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/space_response.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/space_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/spaces/types/space_size.py` & `flatfile-0.0.9/src/flatfile/resources/spaces/types/space_size.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/client.py` & `flatfile-0.0.9/src/flatfile/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/api_token.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/api_token.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/api_token_response.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/api_token_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/exchange_token_data.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/exchange_token_data.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/exchange_token_response.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/exchange_token_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/list_api_tokens_response.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/list_users_response.py` & `flatfile-0.0.9/src/flatfile/resources/commons/types/action_constraint.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .user import User
+from .action_constraint_type import ActionConstraintType
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ListUsersResponse(pydantic.BaseModel):
-    data: typing.List[User]
+class ActionConstraint(pydantic.BaseModel):
+    type: ActionConstraintType
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/user.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/user.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/user_config.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/user_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/users/types/user_response.py` & `flatfile-0.0.9/src/flatfile/resources/users/types/user_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/versions/client.py` & `flatfile-0.0.9/src/flatfile/resources/versions/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/versions/types/version.py` & `flatfile-0.0.9/src/flatfile/resources/versions/types/version.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/versions/types/version_response.py` & `flatfile-0.0.9/src/flatfile/resources/versions/types/version_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/client.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/client.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/__init__.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/create_workbook_config.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/create_workbook_config.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/list_workbooks_response.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/list_workbooks_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook_config_settings.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook_config_settings.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook_response.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook_response.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/src/flatfile/resources/workbooks/types/workbook_update.py` & `flatfile-0.0.9/src/flatfile/resources/workbooks/types/workbook_update.py`

 * *Files identical despite different names*

### Comparing `flatfile-0.0.8/PKG-INFO` & `flatfile-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatfile
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

