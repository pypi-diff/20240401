# Comparing `tmp/neops_graphql-1.7.9.tar.gz` & `tmp/neops_graphql-1.7.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neops_graphql-1.7.9.tar", max compression
+gzip compressed data, was "neops_graphql-1.7.9.dev0.tar", max compression
```

## Comparing `neops_graphql-1.7.9.tar` & `neops_graphql-1.7.9.dev0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      514 2024-03-07 14:27:54.001267 neops_graphql-1.7.9/README.md
--rw-r--r--   0        0        0    28824 2024-03-07 14:29:19.149273 neops_graphql-1.7.9/neops_graphql/__init__.py
--rw-r--r--   0        0        0      952 2024-03-07 14:29:13.709272 neops_graphql-1.7.9/neops_graphql/abort_execution.py
--rw-r--r--   0        0        0      451 2024-03-07 14:29:13.721272 neops_graphql-1.7.9/neops_graphql/add_api_key.py
--rw-r--r--   0        0        0      640 2024-03-07 14:29:13.733272 neops_graphql-1.7.9/neops_graphql/add_role.py
--rw-r--r--   0        0        0     1922 2024-03-07 14:29:13.765272 neops_graphql-1.7.9/neops_graphql/add_role_device_group.py
--rw-r--r--   0        0        0     1419 2024-03-07 14:29:13.793272 neops_graphql-1.7.9/neops_graphql/add_role_neops_task.py
--rw-r--r--   0        0        0      822 2024-03-07 14:29:13.813272 neops_graphql-1.7.9/neops_graphql/add_user.py
--rw-r--r--   0        0        0      755 2024-03-07 14:29:13.829272 neops_graphql-1.7.9/neops_graphql/add_users_to_role.py
--rw-r--r--   0        0        0      634 2024-03-07 14:29:13.845272 neops_graphql-1.7.9/neops_graphql/archive_or_delete_task.py
--rw-r--r--   0        0        0    12578 2024-03-07 14:29:16.021272 neops_graphql-1.7.9/neops_graphql/async_base_client.py
--rw-r--r--   0        0        0      268 2024-03-07 14:29:13.857272 neops_graphql-1.7.9/neops_graphql/autocomplete_fields.py
--rw-r--r--   0        0        0      620 2024-03-07 14:29:16.021272 neops_graphql-1.7.9/neops_graphql/base_model.py
--rw-r--r--   0        0        0    90618 2024-03-07 14:29:18.893272 neops_graphql-1.7.9/neops_graphql/client.py
--rw-r--r--   0        0        0      756 2024-03-07 14:29:13.877272 neops_graphql-1.7.9/neops_graphql/client_aggregation.py
--rw-r--r--   0        0        0     2205 2024-03-07 14:29:13.929272 neops_graphql-1.7.9/neops_graphql/clients.py
--rw-r--r--   0        0        0      827 2024-03-07 14:29:13.949272 neops_graphql-1.7.9/neops_graphql/cron_execution_type.py
--rw-r--r--   0        0        0      756 2024-03-07 14:29:13.977272 neops_graphql-1.7.9/neops_graphql/device_aggregation.py
--rw-r--r--   0        0        0     1926 2024-03-07 14:29:14.033272 neops_graphql-1.7.9/neops_graphql/device_group_elastic.py
--rw-r--r--   0        0        0     1033 2024-03-07 14:29:14.049272 neops_graphql-1.7.9/neops_graphql/device_group_upsert.py
--rw-r--r--   0        0        0     1037 2024-03-07 14:29:14.081272 neops_graphql-1.7.9/neops_graphql/device_upsert.py
--rw-r--r--   0        0        0     3188 2024-03-07 14:29:14.145272 neops_graphql-1.7.9/neops_graphql/devices.py
--rw-r--r--   0        0        0      554 2024-03-07 14:29:14.157272 neops_graphql-1.7.9/neops_graphql/discovery.py
--rw-r--r--   0        0        0     3511 2024-03-07 14:29:18.953273 neops_graphql-1.7.9/neops_graphql/enums.py
--rw-r--r--   0        0        0     2411 2024-03-07 14:29:16.021272 neops_graphql-1.7.9/neops_graphql/exceptions.py
--rw-r--r--   0        0        0     3325 2024-03-07 14:29:14.357272 neops_graphql-1.7.9/neops_graphql/execute_neops_task.py
--rw-r--r--   0        0        0     5493 2024-03-07 14:29:14.489272 neops_graphql-1.7.9/neops_graphql/execution.py
--rw-r--r--   0        0        0     2026 2024-03-07 14:29:14.553272 neops_graphql-1.7.9/neops_graphql/execution_subscription.py
--rw-r--r--   0        0        0     4724 2024-03-07 14:29:14.665272 neops_graphql-1.7.9/neops_graphql/executions.py
--rw-r--r--   0        0        0     2155 2024-03-07 14:29:14.725272 neops_graphql-1.7.9/neops_graphql/executions_elastic.py
--rw-r--r--   0        0        0      405 2024-03-07 14:29:14.737272 neops_graphql-1.7.9/neops_graphql/get_role.py
--rw-r--r--   0        0        0      742 2024-03-07 14:29:14.749272 neops_graphql-1.7.9/neops_graphql/group_aggregation.py
--rw-r--r--   0        0        0       60 2024-03-07 14:29:13.633272 neops_graphql-1.7.9/neops_graphql/input_types.py
--rw-r--r--   0        0        0      798 2024-03-07 14:29:14.765272 neops_graphql-1.7.9/neops_graphql/interface_aggregation.py
--rw-r--r--   0        0        0     3091 2024-03-07 14:29:14.821272 neops_graphql-1.7.9/neops_graphql/interfaces.py
--rw-r--r--   0        0        0     1421 2024-03-07 14:29:15.973272 neops_graphql-1.7.9/neops_graphql/json_form.py
--rw-r--r--   0        0        0     1077 2024-03-07 14:29:14.861272 neops_graphql-1.7.9/neops_graphql/location_upsert.py
--rw-r--r--   0        0        0      594 2024-03-07 14:29:14.897272 neops_graphql-1.7.9/neops_graphql/login.py
--rw-r--r--   0        0        0     1203 2024-03-07 14:29:15.185272 neops_graphql-1.7.9/neops_graphql/neops_provider.py
--rw-r--r--   0        0        0      686 2024-03-07 14:29:14.949272 neops_graphql-1.7.9/neops_graphql/neops_task_create_mutation.py
--rw-r--r--   0        0        0      713 2024-03-07 14:29:14.937272 neops_graphql-1.7.9/neops_graphql/neops_task_unarchive.py
--rw-r--r--   0        0        0     2297 2024-03-07 14:29:14.997272 neops_graphql-1.7.9/neops_graphql/neops_tasks.py
--rw-r--r--   0        0        0      930 2024-03-07 14:29:15.021272 neops_graphql-1.7.9/neops_graphql/permissions.py
--rw-r--r--   0        0        0      449 2024-03-07 14:29:15.029272 neops_graphql-1.7.9/neops_graphql/platforms.py
--rw-r--r--   0        0        0     3949 2024-03-07 14:29:15.145272 neops_graphql-1.7.9/neops_graphql/process_overview.py
--rw-r--r--   0        0        0     1175 2024-03-07 14:29:15.217272 neops_graphql-1.7.9/neops_graphql/providers.py
--rw-r--r--   0        0        0      463 2024-03-07 14:29:15.269272 neops_graphql-1.7.9/neops_graphql/refresh_token.py
--rw-r--r--   0        0        0      997 2024-03-07 14:29:15.253272 neops_graphql-1.7.9/neops_graphql/reports.py
--rw-r--r--   0        0        0      698 2024-03-07 14:29:14.925272 neops_graphql-1.7.9/neops_graphql/reports_execute.py
--rw-r--r--   0        0        0     1053 2024-03-07 14:29:15.297272 neops_graphql-1.7.9/neops_graphql/role_device_group.py
--rw-r--r--   0        0        0      809 2024-03-07 14:29:15.321272 neops_graphql-1.7.9/neops_graphql/role_device_group_upsert.py
--rw-r--r--   0        0        0      967 2024-03-07 14:29:15.349272 neops_graphql-1.7.9/neops_graphql/role_neops_task.py
--rw-r--r--   0        0        0      773 2024-03-07 14:29:15.369272 neops_graphql-1.7.9/neops_graphql/role_neops_task_upsert.py
--rw-r--r--   0        0        0     1052 2024-03-07 14:29:15.401272 neops_graphql-1.7.9/neops_graphql/role_permission_element.py
--rw-r--r--   0        0        0      921 2024-03-07 14:29:15.421272 neops_graphql-1.7.9/neops_graphql/role_permission_element_upsert.py
--rw-r--r--   0        0        0      818 2024-03-07 14:29:15.441272 neops_graphql-1.7.9/neops_graphql/role_permission_upsert.py
--rw-r--r--   0        0        0     5473 2024-03-07 14:29:15.589272 neops_graphql-1.7.9/neops_graphql/role_permissions.py
--rw-r--r--   0        0        0      697 2024-03-07 14:29:15.613272 neops_graphql-1.7.9/neops_graphql/role_scope_upsert.py
--rw-r--r--   0        0        0      412 2024-03-07 14:29:15.773272 neops_graphql-1.7.9/neops_graphql/role_user.py
--rw-r--r--   0        0        0      622 2024-03-07 14:29:15.789272 neops_graphql-1.7.9/neops_graphql/rollback.py
--rw-r--r--   0        0        0      723 2024-03-07 14:29:15.801272 neops_graphql-1.7.9/neops_graphql/saved_search_create.py
--rw-r--r--   0        0        0      642 2024-03-07 14:29:15.821272 neops_graphql-1.7.9/neops_graphql/saved_search_delete.py
--rw-r--r--   0        0        0      632 2024-03-07 14:29:15.841272 neops_graphql-1.7.9/neops_graphql/saved_searches.py
--rw-r--r--   0        0        0      481 2024-03-07 14:29:15.857272 neops_graphql-1.7.9/neops_graphql/scope_delete.py
--rw-r--r--   0        0        0     1600 2024-03-07 14:29:15.925272 neops_graphql-1.7.9/neops_graphql/scopes.py
--rw-r--r--   0        0        0      519 2024-03-07 14:29:15.873272 neops_graphql-1.7.9/neops_graphql/scopes_upsert.py
--rw-r--r--   0        0        0      608 2024-03-07 14:29:15.941272 neops_graphql-1.7.9/neops_graphql/single_discovery.py
--rw-r--r--   0        0        0     1915 2024-03-07 14:29:16.021272 neops_graphql-1.7.9/neops_graphql/topology.py
--rw-r--r--   0        0        0      578 2024-03-07 14:28:37.253270 neops_graphql-1.7.9/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 neops_graphql-1.7.9/PKG-INFO
+-rw-r--r--   0        0        0      514 2024-03-07 14:27:57.269267 neops_graphql-1.7.9.dev0/README.md
+-rw-r--r--   0        0        0    28824 2024-03-07 14:29:19.945273 neops_graphql-1.7.9.dev0/neops_graphql/__init__.py
+-rw-r--r--   0        0        0      952 2024-03-07 14:29:14.257272 neops_graphql-1.7.9.dev0/neops_graphql/abort_execution.py
+-rw-r--r--   0        0        0      451 2024-03-07 14:29:14.281272 neops_graphql-1.7.9.dev0/neops_graphql/add_api_key.py
+-rw-r--r--   0        0        0      640 2024-03-07 14:29:14.309272 neops_graphql-1.7.9.dev0/neops_graphql/add_role.py
+-rw-r--r--   0        0        0     1922 2024-03-07 14:29:14.353272 neops_graphql-1.7.9.dev0/neops_graphql/add_role_device_group.py
+-rw-r--r--   0        0        0     1419 2024-03-07 14:29:14.389272 neops_graphql-1.7.9.dev0/neops_graphql/add_role_neops_task.py
+-rw-r--r--   0        0        0      822 2024-03-07 14:29:14.421272 neops_graphql-1.7.9.dev0/neops_graphql/add_user.py
+-rw-r--r--   0        0        0      755 2024-03-07 14:29:14.441272 neops_graphql-1.7.9.dev0/neops_graphql/add_users_to_role.py
+-rw-r--r--   0        0        0      634 2024-03-07 14:29:14.461272 neops_graphql-1.7.9.dev0/neops_graphql/archive_or_delete_task.py
+-rw-r--r--   0        0        0    12578 2024-03-07 14:29:16.645272 neops_graphql-1.7.9.dev0/neops_graphql/async_base_client.py
+-rw-r--r--   0        0        0      268 2024-03-07 14:29:14.473272 neops_graphql-1.7.9.dev0/neops_graphql/autocomplete_fields.py
+-rw-r--r--   0        0        0      620 2024-03-07 14:29:16.645272 neops_graphql-1.7.9.dev0/neops_graphql/base_model.py
+-rw-r--r--   0        0        0    90618 2024-03-07 14:29:19.625273 neops_graphql-1.7.9.dev0/neops_graphql/client.py
+-rw-r--r--   0        0        0      756 2024-03-07 14:29:14.497272 neops_graphql-1.7.9.dev0/neops_graphql/client_aggregation.py
+-rw-r--r--   0        0        0     2205 2024-03-07 14:29:14.581272 neops_graphql-1.7.9.dev0/neops_graphql/clients.py
+-rw-r--r--   0        0        0      827 2024-03-07 14:29:14.605272 neops_graphql-1.7.9.dev0/neops_graphql/cron_execution_type.py
+-rw-r--r--   0        0        0      756 2024-03-07 14:29:14.625272 neops_graphql-1.7.9.dev0/neops_graphql/device_aggregation.py
+-rw-r--r--   0        0        0     1926 2024-03-07 14:29:14.681272 neops_graphql-1.7.9.dev0/neops_graphql/device_group_elastic.py
+-rw-r--r--   0        0        0     1033 2024-03-07 14:29:14.701272 neops_graphql-1.7.9.dev0/neops_graphql/device_group_upsert.py
+-rw-r--r--   0        0        0     1037 2024-03-07 14:29:14.725272 neops_graphql-1.7.9.dev0/neops_graphql/device_upsert.py
+-rw-r--r--   0        0        0     3188 2024-03-07 14:29:14.789272 neops_graphql-1.7.9.dev0/neops_graphql/devices.py
+-rw-r--r--   0        0        0      554 2024-03-07 14:29:14.805272 neops_graphql-1.7.9.dev0/neops_graphql/discovery.py
+-rw-r--r--   0        0        0     3511 2024-03-07 14:29:19.709273 neops_graphql-1.7.9.dev0/neops_graphql/enums.py
+-rw-r--r--   0        0        0     2411 2024-03-07 14:29:16.645272 neops_graphql-1.7.9.dev0/neops_graphql/exceptions.py
+-rw-r--r--   0        0        0     3325 2024-03-07 14:29:14.989272 neops_graphql-1.7.9.dev0/neops_graphql/execute_neops_task.py
+-rw-r--r--   0        0        0     5493 2024-03-07 14:29:15.113272 neops_graphql-1.7.9.dev0/neops_graphql/execution.py
+-rw-r--r--   0        0        0     2026 2024-03-07 14:29:15.157272 neops_graphql-1.7.9.dev0/neops_graphql/execution_subscription.py
+-rw-r--r--   0        0        0     4724 2024-03-07 14:29:15.229272 neops_graphql-1.7.9.dev0/neops_graphql/executions.py
+-rw-r--r--   0        0        0     2155 2024-03-07 14:29:15.277272 neops_graphql-1.7.9.dev0/neops_graphql/executions_elastic.py
+-rw-r--r--   0        0        0      405 2024-03-07 14:29:15.289272 neops_graphql-1.7.9.dev0/neops_graphql/get_role.py
+-rw-r--r--   0        0        0      742 2024-03-07 14:29:15.301272 neops_graphql-1.7.9.dev0/neops_graphql/group_aggregation.py
+-rw-r--r--   0        0        0       60 2024-03-07 14:29:14.213272 neops_graphql-1.7.9.dev0/neops_graphql/input_types.py
+-rw-r--r--   0        0        0      798 2024-03-07 14:29:15.325272 neops_graphql-1.7.9.dev0/neops_graphql/interface_aggregation.py
+-rw-r--r--   0        0        0     3091 2024-03-07 14:29:15.401272 neops_graphql-1.7.9.dev0/neops_graphql/interfaces.py
+-rw-r--r--   0        0        0     1421 2024-03-07 14:29:16.589272 neops_graphql-1.7.9.dev0/neops_graphql/json_form.py
+-rw-r--r--   0        0        0     1077 2024-03-07 14:29:15.465272 neops_graphql-1.7.9.dev0/neops_graphql/location_upsert.py
+-rw-r--r--   0        0        0      594 2024-03-07 14:29:15.493272 neops_graphql-1.7.9.dev0/neops_graphql/login.py
+-rw-r--r--   0        0        0     1203 2024-03-07 14:29:15.837272 neops_graphql-1.7.9.dev0/neops_graphql/neops_provider.py
+-rw-r--r--   0        0        0      686 2024-03-07 14:29:15.601272 neops_graphql-1.7.9.dev0/neops_graphql/neops_task_create_mutation.py
+-rw-r--r--   0        0        0      713 2024-03-07 14:29:15.569272 neops_graphql-1.7.9.dev0/neops_graphql/neops_task_unarchive.py
+-rw-r--r--   0        0        0     2297 2024-03-07 14:29:15.677272 neops_graphql-1.7.9.dev0/neops_graphql/neops_tasks.py
+-rw-r--r--   0        0        0      930 2024-03-07 14:29:15.705272 neops_graphql-1.7.9.dev0/neops_graphql/permissions.py
+-rw-r--r--   0        0        0      449 2024-03-07 14:29:15.717272 neops_graphql-1.7.9.dev0/neops_graphql/platforms.py
+-rw-r--r--   0        0        0     3949 2024-03-07 14:29:15.805272 neops_graphql-1.7.9.dev0/neops_graphql/process_overview.py
+-rw-r--r--   0        0        0     1175 2024-03-07 14:29:15.865272 neops_graphql-1.7.9.dev0/neops_graphql/providers.py
+-rw-r--r--   0        0        0      463 2024-03-07 14:29:15.921272 neops_graphql-1.7.9.dev0/neops_graphql/refresh_token.py
+-rw-r--r--   0        0        0      997 2024-03-07 14:29:15.905272 neops_graphql-1.7.9.dev0/neops_graphql/reports.py
+-rw-r--r--   0        0        0      698 2024-03-07 14:29:15.537272 neops_graphql-1.7.9.dev0/neops_graphql/reports_execute.py
+-rw-r--r--   0        0        0     1053 2024-03-07 14:29:15.949272 neops_graphql-1.7.9.dev0/neops_graphql/role_device_group.py
+-rw-r--r--   0        0        0      809 2024-03-07 14:29:15.969272 neops_graphql-1.7.9.dev0/neops_graphql/role_device_group_upsert.py
+-rw-r--r--   0        0        0      967 2024-03-07 14:29:15.989272 neops_graphql-1.7.9.dev0/neops_graphql/role_neops_task.py
+-rw-r--r--   0        0        0      773 2024-03-07 14:29:16.013272 neops_graphql-1.7.9.dev0/neops_graphql/role_neops_task_upsert.py
+-rw-r--r--   0        0        0     1052 2024-03-07 14:29:16.037272 neops_graphql-1.7.9.dev0/neops_graphql/role_permission_element.py
+-rw-r--r--   0        0        0      921 2024-03-07 14:29:16.053272 neops_graphql-1.7.9.dev0/neops_graphql/role_permission_element_upsert.py
+-rw-r--r--   0        0        0      818 2024-03-07 14:29:16.073272 neops_graphql-1.7.9.dev0/neops_graphql/role_permission_upsert.py
+-rw-r--r--   0        0        0     5473 2024-03-07 14:29:16.197272 neops_graphql-1.7.9.dev0/neops_graphql/role_permissions.py
+-rw-r--r--   0        0        0      697 2024-03-07 14:29:16.213272 neops_graphql-1.7.9.dev0/neops_graphql/role_scope_upsert.py
+-rw-r--r--   0        0        0      412 2024-03-07 14:29:16.377272 neops_graphql-1.7.9.dev0/neops_graphql/role_user.py
+-rw-r--r--   0        0        0      622 2024-03-07 14:29:16.397272 neops_graphql-1.7.9.dev0/neops_graphql/rollback.py
+-rw-r--r--   0        0        0      723 2024-03-07 14:29:16.417272 neops_graphql-1.7.9.dev0/neops_graphql/saved_search_create.py
+-rw-r--r--   0        0        0      642 2024-03-07 14:29:16.433272 neops_graphql-1.7.9.dev0/neops_graphql/saved_search_delete.py
+-rw-r--r--   0        0        0      632 2024-03-07 14:29:16.457272 neops_graphql-1.7.9.dev0/neops_graphql/saved_searches.py
+-rw-r--r--   0        0        0      481 2024-03-07 14:29:16.469272 neops_graphql-1.7.9.dev0/neops_graphql/scope_delete.py
+-rw-r--r--   0        0        0     1600 2024-03-07 14:29:16.533272 neops_graphql-1.7.9.dev0/neops_graphql/scopes.py
+-rw-r--r--   0        0        0      519 2024-03-07 14:29:16.485273 neops_graphql-1.7.9.dev0/neops_graphql/scopes_upsert.py
+-rw-r--r--   0        0        0      608 2024-03-07 14:29:16.549272 neops_graphql-1.7.9.dev0/neops_graphql/single_discovery.py
+-rw-r--r--   0        0        0     1915 2024-03-07 14:29:16.645272 neops_graphql-1.7.9.dev0/neops_graphql/topology.py
+-rw-r--r--   0        0        0      582 2024-03-07 14:28:37.457270 neops_graphql-1.7.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 neops_graphql-1.7.9.dev0/PKG-INFO
```

### Comparing `neops_graphql-1.7.9/README.md` & `neops_graphql-1.7.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/__init__.py` & `neops_graphql-1.7.9.dev0/neops_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/abort_execution.py` & `neops_graphql-1.7.9.dev0/neops_graphql/abort_execution.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/add_role.py` & `neops_graphql-1.7.9.dev0/neops_graphql/add_role.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/add_role_device_group.py` & `neops_graphql-1.7.9.dev0/neops_graphql/add_role_device_group.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/add_role_neops_task.py` & `neops_graphql-1.7.9.dev0/neops_graphql/add_role_neops_task.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/add_user.py` & `neops_graphql-1.7.9.dev0/neops_graphql/add_user.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/add_users_to_role.py` & `neops_graphql-1.7.9.dev0/neops_graphql/add_users_to_role.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/archive_or_delete_task.py` & `neops_graphql-1.7.9.dev0/neops_graphql/archive_or_delete_task.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/async_base_client.py` & `neops_graphql-1.7.9.dev0/neops_graphql/async_base_client.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/base_model.py` & `neops_graphql-1.7.9.dev0/neops_graphql/base_model.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/client.py` & `neops_graphql-1.7.9.dev0/neops_graphql/client.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/client_aggregation.py` & `neops_graphql-1.7.9.dev0/neops_graphql/client_aggregation.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/clients.py` & `neops_graphql-1.7.9.dev0/neops_graphql/clients.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/cron_execution_type.py` & `neops_graphql-1.7.9.dev0/neops_graphql/cron_execution_type.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/device_aggregation.py` & `neops_graphql-1.7.9.dev0/neops_graphql/device_aggregation.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/device_group_elastic.py` & `neops_graphql-1.7.9.dev0/neops_graphql/device_group_elastic.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/device_group_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/device_group_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/device_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/device_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/devices.py` & `neops_graphql-1.7.9.dev0/neops_graphql/devices.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/discovery.py` & `neops_graphql-1.7.9.dev0/neops_graphql/discovery.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/enums.py` & `neops_graphql-1.7.9.dev0/neops_graphql/enums.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/exceptions.py` & `neops_graphql-1.7.9.dev0/neops_graphql/exceptions.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/execute_neops_task.py` & `neops_graphql-1.7.9.dev0/neops_graphql/execute_neops_task.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/execution.py` & `neops_graphql-1.7.9.dev0/neops_graphql/execution.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/execution_subscription.py` & `neops_graphql-1.7.9.dev0/neops_graphql/execution_subscription.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/executions.py` & `neops_graphql-1.7.9.dev0/neops_graphql/executions.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/executions_elastic.py` & `neops_graphql-1.7.9.dev0/neops_graphql/executions_elastic.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/group_aggregation.py` & `neops_graphql-1.7.9.dev0/neops_graphql/group_aggregation.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/interface_aggregation.py` & `neops_graphql-1.7.9.dev0/neops_graphql/interface_aggregation.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/interfaces.py` & `neops_graphql-1.7.9.dev0/neops_graphql/interfaces.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/json_form.py` & `neops_graphql-1.7.9.dev0/neops_graphql/json_form.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/location_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/location_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/login.py` & `neops_graphql-1.7.9.dev0/neops_graphql/login.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/neops_provider.py` & `neops_graphql-1.7.9.dev0/neops_graphql/neops_provider.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/neops_task_create_mutation.py` & `neops_graphql-1.7.9.dev0/neops_graphql/neops_task_create_mutation.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/neops_task_unarchive.py` & `neops_graphql-1.7.9.dev0/neops_graphql/neops_task_unarchive.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/neops_tasks.py` & `neops_graphql-1.7.9.dev0/neops_graphql/neops_tasks.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/permissions.py` & `neops_graphql-1.7.9.dev0/neops_graphql/permissions.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/process_overview.py` & `neops_graphql-1.7.9.dev0/neops_graphql/process_overview.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/providers.py` & `neops_graphql-1.7.9.dev0/neops_graphql/providers.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/reports.py` & `neops_graphql-1.7.9.dev0/neops_graphql/reports.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/reports_execute.py` & `neops_graphql-1.7.9.dev0/neops_graphql/reports_execute.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_device_group.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_device_group.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_device_group_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_device_group_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_neops_task.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_neops_task.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_neops_task_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_neops_task_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_permission_element.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_permission_element.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_permission_element_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_permission_element_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_permission_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_permission_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_permissions.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_permissions.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/role_scope_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/role_scope_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/rollback.py` & `neops_graphql-1.7.9.dev0/neops_graphql/rollback.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/saved_search_create.py` & `neops_graphql-1.7.9.dev0/neops_graphql/saved_search_create.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/saved_search_delete.py` & `neops_graphql-1.7.9.dev0/neops_graphql/saved_search_delete.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/saved_searches.py` & `neops_graphql-1.7.9.dev0/neops_graphql/saved_searches.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/scopes.py` & `neops_graphql-1.7.9.dev0/neops_graphql/scopes.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/scopes_upsert.py` & `neops_graphql-1.7.9.dev0/neops_graphql/scopes_upsert.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/single_discovery.py` & `neops_graphql-1.7.9.dev0/neops_graphql/single_discovery.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/neops_graphql/topology.py` & `neops_graphql-1.7.9.dev0/neops_graphql/topology.py`

 * *Files identical despite different names*

### Comparing `neops_graphql-1.7.9/pyproject.toml` & `neops_graphql-1.7.9.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neops_graphql"
-version = "1.7.9"
+version = "1.7.9.dev"
 description = "A low-level generated GraphQL for Neops"
 authors = ["Leandro Lerena <leandro.lerena@zebbra.ch>"]
 readme = "README.md"
 include = ["neops_graphql/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `neops_graphql-1.7.9/PKG-INFO` & `neops_graphql-1.7.9.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neops_graphql
-Version: 1.7.9
+Version: 1.7.9.dev0
 Summary: A low-level generated GraphQL for Neops
 Author: Leandro Lerena
 Author-email: leandro.lerena@zebbra.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

