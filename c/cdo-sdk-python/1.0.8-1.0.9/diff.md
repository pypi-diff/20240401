# Comparing `tmp/cdo-sdk-python-1.0.8.tar.gz` & `tmp/cdo-sdk-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdo-sdk-python-1.0.8.tar", last modified: Thu Mar 21 10:21:31 2024, max compression
+gzip compressed data, was "cdo-sdk-python-1.0.9.tar", last modified: Thu Mar 21 10:28:06 2024, max compression
```

## Comparing `cdo-sdk-python-1.0.8.tar` & `cdo-sdk-python-1.0.9.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:21:31.192874 cdo-sdk-python-1.0.8/
--rw-r--r--   0 talhazi    (501) staff       (20)      487 2024-03-21 10:21:31.192755 cdo-sdk-python-1.0.8/PKG-INFO
--rw-r--r--   0 talhazi    (501) staff       (20)    17897 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/README.md
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:21:31.152075 cdo-sdk-python-1.0.8/cdo_sdk_python/
--rw-r--r--   0 talhazi    (501) staff       (20)     7187 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/__init__.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:21:31.155821 cdo-sdk-python-1.0.8/cdo_sdk_python/api/
--rw-r--r--   0 talhazi    (501) staff       (20)      741 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/__init__.py
--rw-r--r--   0 talhazi    (501) staff       (20)    47311 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/change_requests_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    28620 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/changelogs_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    25448 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/connectors_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)   288736 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/inventory_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    29485 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/meta_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    92507 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/object_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    47688 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/remote_access_monitoring_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    20940 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/search_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    64302 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/tenant_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    11540 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/transactions_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    85366 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api/users_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    25814 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api_client.py
--rw-r--r--   0 talhazi    (501) staff       (20)      652 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/api_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)    15498 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/configuration.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5995 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/exceptions.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:21:31.171438 cdo-sdk-python-1.0.8/cdo_sdk_python/models/
--rw-r--r--   0 talhazi    (501) staff       (20)     5950 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/__init__.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2608 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/api_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4440 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/asa_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3282 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/asa_failover_mate.py
--rw-r--r--   0 talhazi    (501) staff       (20)      852 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/asa_failover_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2864 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/authentication_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3992 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cd_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2950 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cd_fmc_object.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4247 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cd_fmc_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2960 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_region.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3005 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_region_list.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3717 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5194 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_transaction.py
--rw-r--r--   0 talhazi    (501) staff       (20)      859 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_transaction_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1297 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_transaction_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2871 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/change_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2800 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/change_request_create_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3675 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/change_request_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3860 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/changelog.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3642 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/changelog_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3894 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/common_api_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1128 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/config_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      997 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/conflict_detection_interval.py
--rw-r--r--   0 talhazi    (501) staff       (20)      906 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/conflict_detection_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1069 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/connectivity_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      935 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/connector_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3702 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/create_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)    10882 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/device.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3618 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/device_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2958 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/device_patch_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)      865 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/device_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3617 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3370 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/entity.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1403 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/entity_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4330 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/event.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5134 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/ftd_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2665 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/ftd_registration_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4126 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/global_search_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3340 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/group_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6090 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/icmp4_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6408 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/icmp6_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4187 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/inventory.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4132 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/ios_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2617 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/issues_dto.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3330 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/json_web_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2976 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/jwk_set.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2933 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/labels.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3788 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/list_object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3085 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/location.py
--rw-r--r--   0 talhazi    (501) staff       (20)      849 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/meraki_deployment_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2744 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/meta.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2601 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/msp_add_tenant_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3096 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/network.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2614 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/network_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     7141 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5839 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2895 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/on_prem_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2861 2024-03-21 10:20:35.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/os.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3131 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/override.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2761 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/policy.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3109 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/ports_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5985 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/ra_vpn_session.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3668 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/ra_vpn_session_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3409 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/reference_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4129 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3594 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3024 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc_public_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)      876 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5594 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/service_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6005 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/service_object_value_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4210 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/shared_object_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6359 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/single_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2673 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/sort_criteria_param.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3051 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/state_machine_details.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2920 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/state_machine_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2578 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/status_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3673 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/target.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2667 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/targets_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3531 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3618 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      921 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant_pay_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4891 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant_settings.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4001 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/unified_object_list_view.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3453 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/update_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2545 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/url_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3512 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/user.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3036 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/user_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3602 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/user_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1038 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/models/user_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)        0 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/py.typed
--rw-r--r--   0 talhazi    (501) staff       (20)     9255 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/cdo_sdk_python/rest.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:21:31.192325 cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/
--rw-r--r--   0 talhazi    (501) staff       (20)      487 2024-03-21 10:21:31.000000 cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 talhazi    (501) staff       (20)     7359 2024-03-21 10:21:31.000000 cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 talhazi    (501) staff       (20)        1 2024-03-21 10:21:31.000000 cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 talhazi    (501) staff       (20)       76 2024-03-21 10:21:31.000000 cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/requires.txt
--rw-r--r--   0 talhazi    (501) staff       (20)       15 2024-03-21 10:21:31.000000 cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 talhazi    (501) staff       (20)     1956 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/pyproject.toml
--rw-r--r--   0 talhazi    (501) staff       (20)       69 2024-03-21 10:21:31.193374 cdo-sdk-python-1.0.8/setup.cfg
--rw-r--r--   0 talhazi    (501) staff       (20)     1334 2024-03-21 10:20:36.000000 cdo-sdk-python-1.0.8/setup.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:21:31.192023 cdo-sdk-python-1.0.8/test/
--rw-r--r--   0 talhazi    (501) staff       (20)     1372 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_api_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2123 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_asa_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1504 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_asa_failover_mate.py
--rw-r--r--   0 talhazi    (501) staff       (20)      720 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_asa_failover_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1515 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_authentication_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1582 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cd_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1634 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cd_fmc_object.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2711 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cd_fmc_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1389 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cdo_region.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1579 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cdo_region_list.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1658 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cdo_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2201 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cdo_transaction.py
--rw-r--r--   0 talhazi    (501) staff       (20)      755 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cdo_transaction_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)      741 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_cdo_transaction_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1616 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_change_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1648 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_change_request_create_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1793 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_change_request_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1338 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_change_requests_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2060 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_changelog.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2353 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_changelog_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      952 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_changelogs_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1528 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_common_api_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)      691 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_config_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      790 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_conflict_detection_interval.py
--rw-r--r--   0 talhazi    (501) staff       (20)      769 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_conflict_detection_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      733 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_connectivity_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      705 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_connector_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)      934 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_connectors_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2365 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_create_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4224 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_device.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4807 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_device_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1651 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_device_patch_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)      684 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_device_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2219 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_duo_admin_panel_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1559 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_entity.py
--rw-r--r--   0 talhazi    (501) staff       (20)      684 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_entity_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1619 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_event.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2094 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_ftd_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1558 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_ftd_registration_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3863 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_global_search_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1537 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_group_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1409 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_icmp4_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1413 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_icmp6_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2713 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_inventory.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5153 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_inventory_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2085 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_ios_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1377 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_issues_dto.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1458 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_json_web_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1579 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_jwk_set.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1422 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_labels.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2724 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_list_object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1382 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_location.py
--rw-r--r--   0 talhazi    (501) staff       (20)      755 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_meraki_deployment_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1318 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_meta.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1069 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_meta_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1475 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_msp_add_tenant_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1391 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_network.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1502 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_network_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1813 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1929 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_object_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2631 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1444 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_on_prem_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1280 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_os.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1448 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_override.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1362 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_policy.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1372 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_ports_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2429 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_ra_vpn_session.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2672 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_ra_vpn_session_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1456 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_reference_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1042 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_remote_access_monitoring_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2508 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_sdc.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2781 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_sdc_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2186 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_sdc_public_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)      677 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_sdc_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)      964 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_search_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1520 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_service_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1763 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_service_object_value_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1748 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_shared_object_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1607 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_single_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1539 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_sort_criteria_param.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1663 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_state_machine_details.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1499 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_state_machine_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1336 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_status_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1390 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_target.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1427 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_targets_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1545 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_tenant.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1632 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_tenant_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1831 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_tenant_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      706 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_tenant_pay_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1816 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_tenant_settings.py
--rw-r--r--   0 talhazi    (501) staff       (20)      822 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_transactions_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2335 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_unified_object_list_view.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1896 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_update_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1474 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_url_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1482 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_user.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1634 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_user_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1764 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_user_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      670 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_user_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1826 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.8/test/test_users_api.py
+drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.437774 cdo-sdk-python-1.0.9/
+-rw-r--r--   0 talhazi    (501) staff       (20)      487 2024-03-21 10:28:06.437679 cdo-sdk-python-1.0.9/PKG-INFO
+-rw-r--r--   0 talhazi    (501) staff       (20)    17897 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/README.md
+drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.381449 cdo-sdk-python-1.0.9/cdo_sdk_python/
+-rw-r--r--   0 talhazi    (501) staff       (20)     7187 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/__init__.py
+drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.387199 cdo-sdk-python-1.0.9/cdo_sdk_python/api/
+-rw-r--r--   0 talhazi    (501) staff       (20)      741 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/__init__.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    47311 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/change_requests_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    28620 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/changelogs_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    25448 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/connectors_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)   288736 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/inventory_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    29485 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/meta_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    92507 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/object_management_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    47688 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/remote_access_monitoring_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    20940 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/search_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    64302 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/tenant_management_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    11540 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/transactions_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    85366 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/users_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    25814 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api_client.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      652 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api_response.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    15498 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/configuration.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5995 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/exceptions.py
+drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.403154 cdo-sdk-python-1.0.9/cdo_sdk_python/models/
+-rw-r--r--   0 talhazi    (501) staff       (20)     5950 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/__init__.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2608 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/api_token_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4440 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3282 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mate.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      852 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mode.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2864 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/authentication_error.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3992 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2950 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_object.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4247 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_result.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2960 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3005 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region_list.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3717 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_token_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5194 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      859 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_status.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1297 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2871 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2800 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_create_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3675 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3860 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3642 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3894 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/common_api_error.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1128 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/config_state.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      997 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_interval.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      906 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_state.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1069 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/connectivity_state.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      935 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/connector_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3702 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/create_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)    10882 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3618 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2958 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_patch_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      865 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_role.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3617 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3370 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1403 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4330 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/event.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5134 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2665 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_registration_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4126 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/global_search_result.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3340 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/group_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     6090 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp4_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     6408 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp6_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4187 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/inventory.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4132 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ios_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2617 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/issues_dto.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3330 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/json_web_key.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2976 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/jwk_set.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2933 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/labels.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3788 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/list_object_response.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3085 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/location.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      849 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/meraki_deployment_mode.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2744 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/meta.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2601 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/msp_add_tenant_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3096 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/network.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2614 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/network_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     7141 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5839 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_response.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2895 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/on_prem_fmc_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2861 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/os.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3131 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/override.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2761 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/policy.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3109 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ports_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5985 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3668 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3409 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/reference_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4129 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3594 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3024 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_public_key.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      876 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_status.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5594 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     6005 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_value_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4210 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/shared_object_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     6359 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/single_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2673 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sort_criteria_param.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3051 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_details.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2920 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_error.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2578 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/status_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3673 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/target.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2667 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/targets_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3531 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3618 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      921 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_pay_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4891 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_settings.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4001 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/unified_object_list_view.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3453 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/update_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2545 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/url_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3512 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3036 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3602 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1038 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_role.py
+-rw-r--r--   0 talhazi    (501) staff       (20)        0 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/py.typed
+-rw-r--r--   0 talhazi    (501) staff       (20)     9255 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/rest.py
+drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.437271 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/
+-rw-r--r--   0 talhazi    (501) staff       (20)      487 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 talhazi    (501) staff       (20)     7359 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 talhazi    (501) staff       (20)        1 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 talhazi    (501) staff       (20)       76 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 talhazi    (501) staff       (20)       15 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 talhazi    (501) staff       (20)     1956 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/pyproject.toml
+-rw-r--r--   0 talhazi    (501) staff       (20)       69 2024-03-21 10:28:06.438079 cdo-sdk-python-1.0.9/setup.cfg
+-rw-r--r--   0 talhazi    (501) staff       (20)     1334 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/setup.py
+drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.436840 cdo-sdk-python-1.0.9/test/
+-rw-r--r--   0 talhazi    (501) staff       (20)     1372 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_api_token_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2123 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_asa_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1504 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_asa_failover_mate.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      720 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_asa_failover_mode.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1515 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_authentication_error.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1582 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cd_fmc_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1634 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cd_fmc_object.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2711 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cd_fmc_result.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1389 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_region.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1579 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_region_list.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1658 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_token_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2201 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_transaction.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      755 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_transaction_status.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      741 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_transaction_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1616 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1648 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_request_create_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1793 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_request_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1338 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_requests_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2060 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_changelog.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2353 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_changelog_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      952 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_changelogs_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1528 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_common_api_error.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      691 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_config_state.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      790 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_conflict_detection_interval.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      769 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_conflict_detection_state.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      733 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_connectivity_state.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      705 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_connector_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      934 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_connectors_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2365 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_create_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4224 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     4807 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1651 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device_patch_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      684 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device_role.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2219 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_duo_admin_panel_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1559 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_entity.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      684 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_entity_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1619 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_event.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2094 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ftd_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1558 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ftd_registration_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     3863 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_global_search_result.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1537 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_group_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1409 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_icmp4_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1413 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_icmp6_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2713 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_inventory.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     5153 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_inventory_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2085 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ios_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1377 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_issues_dto.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1458 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_json_web_key.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1579 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_jwk_set.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1422 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_labels.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2724 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_list_object_response.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1382 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_location.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      755 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_meraki_deployment_mode.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1318 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_meta.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1069 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_meta_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1475 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_msp_add_tenant_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1391 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_network.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1502 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_network_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1813 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1929 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_object_management_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2631 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_object_response.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1444 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_on_prem_fmc_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1280 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_os.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1448 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_override.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1362 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_policy.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1372 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ports_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2429 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ra_vpn_session.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2672 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ra_vpn_session_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1456 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_reference_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1042 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_remote_access_monitoring_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2508 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2781 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2186 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc_public_key.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      677 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc_status.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      964 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_search_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1520 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_service_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1763 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_service_object_value_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1748 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_shared_object_value.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1607 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_single_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1539 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sort_criteria_param.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1663 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_state_machine_details.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1499 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_state_machine_error.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1336 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_status_info.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1390 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_target.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1427 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_targets_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1545 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1632 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_management_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1831 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      706 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_pay_type.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1816 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_settings.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      822 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_transactions_api.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     2335 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_unified_object_list_view.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1896 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_update_request.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1474 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_url_object_content.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1482 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1634 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user_create_or_update_input.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1764 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user_page.py
+-rw-r--r--   0 talhazi    (501) staff       (20)      670 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user_role.py
+-rw-r--r--   0 talhazi    (501) staff       (20)     1826 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_users_api.py
```

### Comparing `cdo-sdk-python-1.0.8/README.md` & `cdo-sdk-python-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cdo-sdk-python
 Use the interactive documentation to explore the endpoints CDO has to offer
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.0.1
-- Package version: 1.0.8
+- Package version: 1.0.9
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/__init__.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 # import apis into sdk package
 from cdo_sdk_python.api.change_requests_api import ChangeRequestsApi
 from cdo_sdk_python.api.changelogs_api import ChangelogsApi
 from cdo_sdk_python.api.connectors_api import ConnectorsApi
 from cdo_sdk_python.api.inventory_api import InventoryApi
 from cdo_sdk_python.api.meta_api import MetaApi
```

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/__init__.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/change_requests_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/change_requests_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/changelogs_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/changelogs_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/connectors_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/connectors_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/inventory_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/inventory_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/meta_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/meta_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/object_management_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/object_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/remote_access_monitoring_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/remote_access_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/search_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/search_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/tenant_management_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/transactions_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api/users_api.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api/users_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api_client.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.8/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/api_response.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/api_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/configuration.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 1.0.8".\
+               "SDK Package Version: 1.0.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/exceptions.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/__init__.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/api_token_info.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/api_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/asa_create_or_update_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/asa_failover_mate.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mate.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/asa_failover_mode.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/authentication_error.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/authentication_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cd_fmc_info.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cd_fmc_object.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_object.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cd_fmc_result.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_region.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_region_list.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region_list.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_token_info.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_transaction.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_transaction_status.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/cdo_transaction_type.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/change_request.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/change_request_create_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_create_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/change_request_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/changelog.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/changelog_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/common_api_error.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/common_api_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/config_state.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/config_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/conflict_detection_interval.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_interval.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/conflict_detection_state.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/connectivity_state.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/connectivity_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/connector_type.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/connector_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/create_request.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/create_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/device.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/device_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/device_patch_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_patch_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/device_role.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/entity.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/entity_type.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/event.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/event.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/ftd_create_or_update_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/ftd_registration_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_registration_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/global_search_result.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/global_search_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/group_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/group_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/icmp4_value.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp4_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/icmp6_value.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp6_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/inventory.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/inventory.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/ios_create_or_update_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ios_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/issues_dto.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/issues_dto.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/json_web_key.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/json_web_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/jwk_set.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/jwk_set.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/labels.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/labels.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/list_object_response.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/list_object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/location.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/location.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/meraki_deployment_mode.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/meraki_deployment_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/meta.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/meta.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/msp_add_tenant_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/msp_add_tenant_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/network.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/network.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/network_object_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/network_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/object_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/object_response.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/on_prem_fmc_info.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/on_prem_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/os.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/os.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/override.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/override.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/policy.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/policy.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/ports_value.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ports_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/ra_vpn_session.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/ra_vpn_session_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/reference_info.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/reference_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc_public_key.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/sdc_status.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/service_object_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/service_object_value_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_value_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/shared_object_value.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/shared_object_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/single_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/single_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/sort_criteria_param.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sort_criteria_param.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/state_machine_details.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_details.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/state_machine_error.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/status_info.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/status_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/target.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/target.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/targets_request.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/targets_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant_pay_type.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_pay_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/tenant_settings.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_settings.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/unified_object_list_view.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/unified_object_list_view.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/update_request.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/update_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/url_object_content.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/url_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/user.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/user_create_or_update_input.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/user_page.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/models/user_role.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python/rest.py` & `cdo-sdk-python-1.0.9/cdo_sdk_python/rest.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/cdo_sdk_python.egg-info/SOURCES.txt` & `cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/pyproject.toml` & `cdo-sdk-python-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdo_sdk_python"
-version = "1.0.8"
+version = "1.0.9"
 description = "Cisco Defense Orchestrator API"
 authors = ["CDO TAC <cdo.tac@cisco.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Cisco Defense Orchestrator API"]
 include = ["cdo_sdk_python/py.typed"]
```

### Comparing `cdo-sdk-python-1.0.8/setup.py` & `cdo-sdk-python-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "cdo-sdk-python"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `cdo-sdk-python-1.0.8/test/test_api_token_info.py` & `cdo-sdk-python-1.0.9/test/test_api_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_asa_create_or_update_input.py` & `cdo-sdk-python-1.0.9/test/test_asa_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_asa_failover_mate.py` & `cdo-sdk-python-1.0.9/test/test_asa_failover_mate.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_asa_failover_mode.py` & `cdo-sdk-python-1.0.9/test/test_asa_failover_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_authentication_error.py` & `cdo-sdk-python-1.0.9/test/test_authentication_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cd_fmc_info.py` & `cdo-sdk-python-1.0.9/test/test_cd_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cd_fmc_object.py` & `cdo-sdk-python-1.0.9/test/test_cd_fmc_object.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cd_fmc_result.py` & `cdo-sdk-python-1.0.9/test/test_cd_fmc_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cdo_region.py` & `cdo-sdk-python-1.0.9/test/test_cdo_region.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cdo_region_list.py` & `cdo-sdk-python-1.0.9/test/test_cdo_region_list.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cdo_token_info.py` & `cdo-sdk-python-1.0.9/test/test_cdo_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cdo_transaction.py` & `cdo-sdk-python-1.0.9/test/test_cdo_transaction.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cdo_transaction_status.py` & `cdo-sdk-python-1.0.9/test/test_cdo_transaction_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_cdo_transaction_type.py` & `cdo-sdk-python-1.0.9/test/test_cdo_transaction_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_change_request.py` & `cdo-sdk-python-1.0.9/test/test_change_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_change_request_create_input.py` & `cdo-sdk-python-1.0.9/test/test_change_request_create_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_change_request_page.py` & `cdo-sdk-python-1.0.9/test/test_change_request_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_change_requests_api.py` & `cdo-sdk-python-1.0.9/test/test_change_requests_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_changelog.py` & `cdo-sdk-python-1.0.9/test/test_changelog.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_changelog_page.py` & `cdo-sdk-python-1.0.9/test/test_changelog_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_changelogs_api.py` & `cdo-sdk-python-1.0.9/test/test_changelogs_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_common_api_error.py` & `cdo-sdk-python-1.0.9/test/test_common_api_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_config_state.py` & `cdo-sdk-python-1.0.9/test/test_config_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_conflict_detection_interval.py` & `cdo-sdk-python-1.0.9/test/test_conflict_detection_interval.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_conflict_detection_state.py` & `cdo-sdk-python-1.0.9/test/test_conflict_detection_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_connectivity_state.py` & `cdo-sdk-python-1.0.9/test/test_connectivity_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_connector_type.py` & `cdo-sdk-python-1.0.9/test/test_connector_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_connectors_api.py` & `cdo-sdk-python-1.0.9/test/test_connectors_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_create_request.py` & `cdo-sdk-python-1.0.9/test/test_create_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_device.py` & `cdo-sdk-python-1.0.9/test/test_device.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_device_page.py` & `cdo-sdk-python-1.0.9/test/test_device_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_device_patch_input.py` & `cdo-sdk-python-1.0.9/test/test_device_patch_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_device_role.py` & `cdo-sdk-python-1.0.9/test/test_device_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_duo_admin_panel_create_or_update_input.py` & `cdo-sdk-python-1.0.9/test/test_duo_admin_panel_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_entity.py` & `cdo-sdk-python-1.0.9/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_entity_type.py` & `cdo-sdk-python-1.0.9/test/test_entity_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_event.py` & `cdo-sdk-python-1.0.9/test/test_event.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_ftd_create_or_update_input.py` & `cdo-sdk-python-1.0.9/test/test_ftd_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_ftd_registration_input.py` & `cdo-sdk-python-1.0.9/test/test_ftd_registration_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_global_search_result.py` & `cdo-sdk-python-1.0.9/test/test_global_search_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_group_content.py` & `cdo-sdk-python-1.0.9/test/test_group_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_icmp4_value.py` & `cdo-sdk-python-1.0.9/test/test_icmp4_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_icmp6_value.py` & `cdo-sdk-python-1.0.9/test/test_icmp6_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_inventory.py` & `cdo-sdk-python-1.0.9/test/test_inventory.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_inventory_api.py` & `cdo-sdk-python-1.0.9/test/test_inventory_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_ios_create_or_update_input.py` & `cdo-sdk-python-1.0.9/test/test_ios_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_issues_dto.py` & `cdo-sdk-python-1.0.9/test/test_issues_dto.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_json_web_key.py` & `cdo-sdk-python-1.0.9/test/test_json_web_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_jwk_set.py` & `cdo-sdk-python-1.0.9/test/test_jwk_set.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_labels.py` & `cdo-sdk-python-1.0.9/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_list_object_response.py` & `cdo-sdk-python-1.0.9/test/test_list_object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_location.py` & `cdo-sdk-python-1.0.9/test/test_location.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_meraki_deployment_mode.py` & `cdo-sdk-python-1.0.9/test/test_meraki_deployment_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_meta.py` & `cdo-sdk-python-1.0.9/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_meta_api.py` & `cdo-sdk-python-1.0.9/test/test_meta_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_msp_add_tenant_input.py` & `cdo-sdk-python-1.0.9/test/test_msp_add_tenant_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_network.py` & `cdo-sdk-python-1.0.9/test/test_network.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_network_object_content.py` & `cdo-sdk-python-1.0.9/test/test_network_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_object_content.py` & `cdo-sdk-python-1.0.9/test/test_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_object_management_api.py` & `cdo-sdk-python-1.0.9/test/test_object_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_object_response.py` & `cdo-sdk-python-1.0.9/test/test_object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_on_prem_fmc_info.py` & `cdo-sdk-python-1.0.9/test/test_on_prem_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_os.py` & `cdo-sdk-python-1.0.9/test/test_os.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_override.py` & `cdo-sdk-python-1.0.9/test/test_override.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_policy.py` & `cdo-sdk-python-1.0.9/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_ports_value.py` & `cdo-sdk-python-1.0.9/test/test_ports_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_ra_vpn_session.py` & `cdo-sdk-python-1.0.9/test/test_ra_vpn_session.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_ra_vpn_session_page.py` & `cdo-sdk-python-1.0.9/test/test_ra_vpn_session_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_reference_info.py` & `cdo-sdk-python-1.0.9/test/test_reference_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_remote_access_monitoring_api.py` & `cdo-sdk-python-1.0.9/test/test_remote_access_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_sdc.py` & `cdo-sdk-python-1.0.9/test/test_sdc.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_sdc_page.py` & `cdo-sdk-python-1.0.9/test/test_sdc_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_sdc_public_key.py` & `cdo-sdk-python-1.0.9/test/test_sdc_public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_sdc_status.py` & `cdo-sdk-python-1.0.9/test/test_sdc_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_search_api.py` & `cdo-sdk-python-1.0.9/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_service_object_content.py` & `cdo-sdk-python-1.0.9/test/test_service_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_service_object_value_content.py` & `cdo-sdk-python-1.0.9/test/test_service_object_value_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_shared_object_value.py` & `cdo-sdk-python-1.0.9/test/test_shared_object_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_single_content.py` & `cdo-sdk-python-1.0.9/test/test_single_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_sort_criteria_param.py` & `cdo-sdk-python-1.0.9/test/test_sort_criteria_param.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_state_machine_details.py` & `cdo-sdk-python-1.0.9/test/test_state_machine_details.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_state_machine_error.py` & `cdo-sdk-python-1.0.9/test/test_state_machine_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_status_info.py` & `cdo-sdk-python-1.0.9/test/test_status_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_target.py` & `cdo-sdk-python-1.0.9/test/test_target.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_targets_request.py` & `cdo-sdk-python-1.0.9/test/test_targets_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_tenant.py` & `cdo-sdk-python-1.0.9/test/test_tenant.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_tenant_management_api.py` & `cdo-sdk-python-1.0.9/test/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_tenant_page.py` & `cdo-sdk-python-1.0.9/test/test_tenant_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_tenant_pay_type.py` & `cdo-sdk-python-1.0.9/test/test_tenant_pay_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_tenant_settings.py` & `cdo-sdk-python-1.0.9/test/test_tenant_settings.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_transactions_api.py` & `cdo-sdk-python-1.0.9/test/test_transactions_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_unified_object_list_view.py` & `cdo-sdk-python-1.0.9/test/test_unified_object_list_view.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_update_request.py` & `cdo-sdk-python-1.0.9/test/test_update_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_url_object_content.py` & `cdo-sdk-python-1.0.9/test/test_url_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_user.py` & `cdo-sdk-python-1.0.9/test/test_user.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_user_create_or_update_input.py` & `cdo-sdk-python-1.0.9/test/test_user_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_user_page.py` & `cdo-sdk-python-1.0.9/test/test_user_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_user_role.py` & `cdo-sdk-python-1.0.9/test/test_user_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.8/test/test_users_api.py` & `cdo-sdk-python-1.0.9/test/test_users_api.py`

 * *Files identical despite different names*

