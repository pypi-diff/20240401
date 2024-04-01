# Comparing `tmp/xingchen-1.1.0.tar.gz` & `tmp/xingchen-1.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingchen-1.1.0.tar", last modified: Fri Mar 15 02:36:54 2024, max compression
+gzip compressed data, was "xingchen-1.1.1.1.tar", last modified: Mon Apr  1 09:21:23 2024, max compression
```

## Comparing `xingchen-1.1.0.tar` & `xingchen-1.1.1.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.894846 xingchen-1.1.0/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-03-15 02:36:54.895000 xingchen-1.1.0/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)    11507 2024-03-05 07:56:13.000000 xingchen-1.1.0/README.md
--rw-r--r--   0 frankin    (501) staff       (20)      771 2024-03-05 07:58:36.000000 xingchen-1.1.0/pyproject.toml
--rw-r--r--   0 frankin    (501) staff       (20)       69 2024-03-15 02:36:54.895373 xingchen-1.1.0/setup.cfg
--rw-r--r--   0 frankin    (501) staff       (20)     1152 2024-03-15 02:36:47.000000 xingchen-1.1.0/setup.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.873138 xingchen-1.1.0/test/
--rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.0/test/test_base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     3169 2024-03-05 07:23:22.000000 xingchen-1.1.0/test/test_base_chat_request_aca_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.0/test/test_character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.0/test/test_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.0/test/test_character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.0/test/test_character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.0/test/test_character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.0/test/test_chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.0/test/test_chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_message.py
--rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.0/test/test_message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.0/test/test_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.0/test/test_result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.0/test/test_result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.0/test/test_result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.0/test/test_sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.0/test/test_user_profile.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.875877 xingchen-1.1.0/xingchen/
--rw-r--r--   0 frankin    (501) staff       (20)     4083 2024-03-06 06:57:10.000000 xingchen-1.1.0/xingchen/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2161 2024-02-01 06:42:31.000000 xingchen-1.1.0/xingchen/aca_util.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.878309 xingchen-1.1.0/xingchen/api/
--rw-r--r--   0 frankin    (501) staff       (20)      220 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/api/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)    55637 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/api/character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     9376 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/api/chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    25469 2024-02-01 06:52:29.000000 xingchen-1.1.0/xingchen/api/chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/api_client.py
--rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/api_response.py
--rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/configuration.py
--rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/exceptions.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.892387 xingchen-1.1.0/xingchen/models/
--rw-r--r--   0 frankin    (501) staff       (20)     2988 2024-03-05 07:09:19.000000 xingchen-1.1.0/xingchen/models/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.0/xingchen/models/advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2973 2024-03-05 07:28:35.000000 xingchen-1.1.0/xingchen/models/base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     3093 2024-03-05 07:28:35.000000 xingchen-1.1.0/xingchen/models/base_chat_request_aca_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     4106 2024-03-07 08:00:51.000000 xingchen-1.1.0/xingchen/models/character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.0/xingchen/models/character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.0/xingchen/models/character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2408 2023-11-24 13:03:37.000000 xingchen-1.1.0/xingchen/models/character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.0/xingchen/models/character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     5127 2024-03-07 08:02:16.000000 xingchen-1.1.0/xingchen/models/character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4748 2024-03-06 06:39:36.000000 xingchen-1.1.0/xingchen/models/character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.0/xingchen/models/chat_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.0/xingchen/models/chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     6702 2024-03-05 07:40:25.000000 xingchen-1.1.0/xingchen/models/chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.0/xingchen/models/context.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.894490 xingchen-1.1.0/xingchen/models/custom/
--rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/custom/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/custom/base_response.py
--rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.0/xingchen/models/custom/character_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4815 2024-03-05 07:11:26.000000 xingchen-1.1.0/xingchen/models/custom/chat_response.py
--rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.0/xingchen/models/custom/platform_publish_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.0/xingchen/models/custom/reset_history_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.0/xingchen/models/function_call.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2505 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/input.py
--rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.0/xingchen/models/message.py
--rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.0/xingchen/models/message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.0/xingchen/models/model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.0/xingchen/models/scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.0/xingchen/models/sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/models/user_profile.py
--rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/py.typed
--rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.0/xingchen/rest.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-03-15 02:36:54.877030 xingchen-1.1.0/xingchen.egg-info/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-03-15 02:36:54.000000 xingchen-1.1.0/xingchen.egg-info/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)     3793 2024-03-15 02:36:54.000000 xingchen-1.1.0/xingchen.egg-info/SOURCES.txt
--rw-r--r--   0 frankin    (501) staff       (20)        1 2024-03-15 02:36:54.000000 xingchen-1.1.0/xingchen.egg-info/dependency_links.txt
--rw-r--r--   0 frankin    (501) staff       (20)       85 2024-03-15 02:36:54.000000 xingchen-1.1.0/xingchen.egg-info/requires.txt
--rw-r--r--   0 frankin    (501) staff       (20)        9 2024-03-15 02:36:54.000000 xingchen-1.1.0/xingchen.egg-info/top_level.txt
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.269419 xingchen-1.1.1.1/
+-rw-r--r--   0 frankin    (501) staff       (20)      335 2024-04-01 09:21:23.269535 xingchen-1.1.1.1/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)    11507 2024-03-05 07:56:13.000000 xingchen-1.1.1.1/README.md
+-rw-r--r--   0 frankin    (501) staff       (20)      773 2024-04-01 09:19:09.000000 xingchen-1.1.1.1/pyproject.toml
+-rw-r--r--   0 frankin    (501) staff       (20)       69 2024-04-01 09:21:23.269965 xingchen-1.1.1.1/setup.cfg
+-rw-r--r--   0 frankin    (501) staff       (20)     1154 2024-04-01 09:18:50.000000 xingchen-1.1.1.1/setup.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.223782 xingchen-1.1.1.1/test/
+-rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.1.1/test/test_base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3169 2024-03-05 07:23:22.000000 xingchen-1.1.1.1/test/test_base_chat_request_aca_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.1.1/test/test_character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.1.1/test/test_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.1.1/test/test_character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.1.1/test/test_character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.1.1/test/test_character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.1.1/test/test_chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.1.1/test/test_chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.1.1/test/test_message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.1.1/test/test_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.1.1/test/test_result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.1.1/test/test_result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.1.1/test/test_result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.1.1/test/test_sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_user_profile.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.226255 xingchen-1.1.1.1/xingchen/
+-rw-r--r--   0 frankin    (501) staff       (20)     4083 2024-03-06 06:57:10.000000 xingchen-1.1.1.1/xingchen/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2161 2024-02-01 06:42:31.000000 xingchen-1.1.1.1/xingchen/aca_util.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.229699 xingchen-1.1.1.1/xingchen/api/
+-rw-r--r--   0 frankin    (501) staff       (20)      220 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)    55637 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api/character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     9376 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api/chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    25469 2024-02-01 06:52:29.000000 xingchen-1.1.1.1/xingchen/api/chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api_client.py
+-rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/configuration.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/exceptions.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.265954 xingchen-1.1.1.1/xingchen/models/
+-rw-r--r--   0 frankin    (501) staff       (20)     2988 2024-03-05 07:09:19.000000 xingchen-1.1.1.1/xingchen/models/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.1.1/xingchen/models/advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2973 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3093 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/base_chat_request_aca_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4106 2024-03-07 08:00:51.000000 xingchen-1.1.1.1/xingchen/models/character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.1.1/xingchen/models/character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.1.1/xingchen/models/character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2408 2023-11-24 13:03:37.000000 xingchen-1.1.1.1/xingchen/models/character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5127 2024-03-07 08:02:16.000000 xingchen-1.1.1.1/xingchen/models/character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4748 2024-03-06 06:39:36.000000 xingchen-1.1.1.1/xingchen/models/character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.1.1/xingchen/models/chat_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     6702 2024-03-05 07:40:25.000000 xingchen-1.1.1.1/xingchen/models/chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.1.1/xingchen/models/context.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.268890 xingchen-1.1.1.1/xingchen/models/custom/
+-rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/custom/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/custom/base_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.1.1/xingchen/models/custom/character_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4815 2024-03-05 07:11:26.000000 xingchen-1.1.1.1/xingchen/models/custom/chat_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.1.1/xingchen/models/custom/platform_publish_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.1.1/xingchen/models/custom/reset_history_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.1.1/xingchen/models/function_call.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2505 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.1.1/xingchen/models/message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.1.1/xingchen/models/model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.1.1/xingchen/models/scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/user_profile.py
+-rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/py.typed
+-rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/rest.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.227676 xingchen-1.1.1.1/xingchen.egg-info/
+-rw-r--r--   0 frankin    (501) staff       (20)      335 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)     3793 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/SOURCES.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        1 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/dependency_links.txt
+-rw-r--r--   0 frankin    (501) staff       (20)       85 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/requires.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        9 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/top_level.txt
```

### Comparing `xingchen-1.1.0/README.md` & `xingchen-1.1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/pyproject.toml` & `xingchen-1.1.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xingchen"
-version = "1.1.0"
+version = "1.1.1.1"
 description = "XingChen 开放接口定义"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "XingChen 开放接口定义"]
 include = ["xingchen/py.typed"]
```

### Comparing `xingchen-1.1.0/setup.py` & `xingchen-1.1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "xingchen"
-VERSION = "1.1.0"
+VERSION = "1.1.1.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum",
     "sseclient-py >= 1.8.0"
```

### Comparing `xingchen-1.1.0/test/test_advanced_settings.py` & `xingchen-1.1.1.1/test/test_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_base_chat_request.py` & `xingchen-1.1.1.1/test/test_base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_base_chat_request_aca_chat_ext_param.py` & `xingchen-1.1.1.1/test/test_base_chat_request_aca_chat_ext_param.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_advanced_config.py` & `xingchen-1.1.1.1/test/test_character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_api_sub.py` & `xingchen-1.1.1.1/test/test_character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_create_dto.py` & `xingchen-1.1.1.1/test/test_character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_dto.py` & `xingchen-1.1.1.1/test/test_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_key.py` & `xingchen-1.1.1.1/test/test_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_permission_config.py` & `xingchen-1.1.1.1/test/test_character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_query_dto.py` & `xingchen-1.1.1.1/test/test_character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_query_where.py` & `xingchen-1.1.1.1/test/test_character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_update_dto.py` & `xingchen-1.1.1.1/test/test_character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_character_version_create_or_update_dto.py` & `xingchen-1.1.1.1/test/test_character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_api_sub.py` & `xingchen-1.1.1.1/test/test_chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_history_query_dto.py` & `xingchen-1.1.1.1/test/test_chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_history_query_where.py` & `xingchen-1.1.1.1/test/test_chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_message_api_sub.py` & `xingchen-1.1.1.1/test/test_chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_message_dto.py` & `xingchen-1.1.1.1/test/test_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_req_params.py` & `xingchen-1.1.1.1/test/test_chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_chat_room_user_dto.py` & `xingchen-1.1.1.1/test/test_chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_context.py` & `xingchen-1.1.1.1/test/test_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_file_info_vo.py` & `xingchen-1.1.1.1/test/test_file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_gateway_context.py` & `xingchen-1.1.1.1/test/test_gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_gateway_issued_params.py` & `xingchen-1.1.1.1/test/test_gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_input.py` & `xingchen-1.1.1.1/test/test_input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_message.py` & `xingchen-1.1.1.1/test/test_message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_message_rating_request.py` & `xingchen-1.1.1.1/test/test_message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_meta.py` & `xingchen-1.1.1.1/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_model_parameters.py` & `xingchen-1.1.1.1/test/test_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_page_result_character_dto.py` & `xingchen-1.1.1.1/test/test_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_page_result_chat_message_dto.py` & `xingchen-1.1.1.1/test/test_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_repository.py` & `xingchen-1.1.1.1/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_repository_info.py` & `xingchen-1.1.1.1/test/test_repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_result_dto_boolean.py` & `xingchen-1.1.1.1/test/test_result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_result_dto_character_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_result_dto_character_key.py` & `xingchen-1.1.1.1/test/test_result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_result_dto_list_character_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_result_dto_page_result_character_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_scenario.py` & `xingchen-1.1.1.1/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_sys_reminder_request.py` & `xingchen-1.1.1.1/test/test_sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/test/test_user_profile.py` & `xingchen-1.1.1.1/test/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/__init__.py` & `xingchen-1.1.1.1/xingchen/__init__.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/aca_util.py` & `xingchen-1.1.1.1/xingchen/aca_util.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/api/character_api_sub.py` & `xingchen-1.1.1.1/xingchen/api/character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/api/chat_api_sub.py` & `xingchen-1.1.1.1/xingchen/api/chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/api/chat_message_api_sub.py` & `xingchen-1.1.1.1/xingchen/api/chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/api_client.py` & `xingchen-1.1.1.1/xingchen/api_client.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/api_response.py` & `xingchen-1.1.1.1/xingchen/api_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/configuration.py` & `xingchen-1.1.1.1/xingchen/configuration.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/exceptions.py` & `xingchen-1.1.1.1/xingchen/exceptions.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/__init__.py` & `xingchen-1.1.1.1/xingchen/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/advanced_settings.py` & `xingchen-1.1.1.1/xingchen/models/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/base_chat_request.py` & `xingchen-1.1.1.1/xingchen/models/base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/base_chat_request_aca_chat_ext_param.py` & `xingchen-1.1.1.1/xingchen/models/base_chat_request_aca_chat_ext_param.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_advanced_config.py` & `xingchen-1.1.1.1/xingchen/models/character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_create_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_key.py` & `xingchen-1.1.1.1/xingchen/models/character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_permission_config.py` & `xingchen-1.1.1.1/xingchen/models/character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_query_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_query_where.py` & `xingchen-1.1.1.1/xingchen/models/character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_update_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/character_version_create_or_update_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/chat_context.py` & `xingchen-1.1.1.1/xingchen/models/chat_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/chat_history_query_dto.py` & `xingchen-1.1.1.1/xingchen/models/chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/chat_history_query_where.py` & `xingchen-1.1.1.1/xingchen/models/chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/chat_message_dto.py` & `xingchen-1.1.1.1/xingchen/models/chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/chat_req_params.py` & `xingchen-1.1.1.1/xingchen/models/chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/chat_room_user_dto.py` & `xingchen-1.1.1.1/xingchen/models/chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/context.py` & `xingchen-1.1.1.1/xingchen/models/context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/custom/base_response.py` & `xingchen-1.1.1.1/xingchen/models/custom/base_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/custom/character_model_parameters.py` & `xingchen-1.1.1.1/xingchen/models/custom/character_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/custom/chat_response.py` & `xingchen-1.1.1.1/xingchen/models/custom/chat_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/custom/platform_publish_config.py` & `xingchen-1.1.1.1/xingchen/models/custom/platform_publish_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/custom/reset_history_request.py` & `xingchen-1.1.1.1/xingchen/models/custom/reset_history_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/file_info_vo.py` & `xingchen-1.1.1.1/xingchen/models/file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/function_call.py` & `xingchen-1.1.1.1/xingchen/models/function_call.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/gateway_context.py` & `xingchen-1.1.1.1/xingchen/models/gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/gateway_issued_params.py` & `xingchen-1.1.1.1/xingchen/models/gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/input.py` & `xingchen-1.1.1.1/xingchen/models/input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/message.py` & `xingchen-1.1.1.1/xingchen/models/message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/message_rating_request.py` & `xingchen-1.1.1.1/xingchen/models/message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/meta.py` & `xingchen-1.1.1.1/xingchen/models/meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/model_parameters.py` & `xingchen-1.1.1.1/xingchen/models/model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/page_result_character_dto.py` & `xingchen-1.1.1.1/xingchen/models/page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/page_result_chat_message_dto.py` & `xingchen-1.1.1.1/xingchen/models/page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/repository.py` & `xingchen-1.1.1.1/xingchen/models/repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/repository_info.py` & `xingchen-1.1.1.1/xingchen/models/repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/result_dto_boolean.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/result_dto_character_dto.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/result_dto_character_key.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/result_dto_list_character_dto.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/result_dto_page_result_character_dto.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/scenario.py` & `xingchen-1.1.1.1/xingchen/models/scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/sys_reminder_request.py` & `xingchen-1.1.1.1/xingchen/models/sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/models/user_profile.py` & `xingchen-1.1.1.1/xingchen/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen/rest.py` & `xingchen-1.1.1.1/xingchen/rest.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.0/xingchen.egg-info/SOURCES.txt` & `xingchen-1.1.1.1/xingchen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

