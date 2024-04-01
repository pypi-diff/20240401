# Comparing `tmp/gridworks_protocol-0.7.1.tar.gz` & `tmp/gridworks_protocol-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.7.1.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.7.2.tar", max compression
```

## Comparing `gridworks_protocol-0.7.1.tar` & `gridworks_protocol-0.7.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1070 2024-02-09 20:10:06.493739 gridworks_protocol-0.7.1/LICENSE
--rw-r--r--   0        0        0     3087 2024-02-09 20:10:06.493739 gridworks_protocol-0.7.1/README.md
--rw-r--r--   0        0        0     2326 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2030 2024-02-09 20:10:06.497739 gridworks_protocol-0.7.1/src/gwproto/__init__.py
--rw-r--r--   0        0        0     1339 2024-02-09 20:10:06.497739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0      147 2024-02-09 20:10:06.497739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/fibaro_smart_implant_cac.py
--rw-r--r--   0        0        0      136 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/hubitat_cac.py
--rw-r--r--   0        0        0      142 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/hubitat_poller_cac.py
--rw-r--r--   0        0        0      146 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/hubitat_tank_module_cac.py
--rw-r--r--   0        0        0     1488 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      995 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1112 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/relay_cac.py
--rw-r--r--   0        0        0     1118 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0      139 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/rest_poller_cac.py
--rw-r--r--   0        0        0     1580 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1094 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1659 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0      533 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/fibaro_smart_implant_component.py
--rw-r--r--   0        0        0      769 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/hubitat_component.py
--rw-r--r--   0        0        0     3141 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/hubitat_poller_component.py
--rw-r--r--   0        0        0     3701 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/hubitat_tank_component.py
--rw-r--r--   0        0        0     1479 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1481 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1267 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/relay_component.py
--rw-r--r--   0        0        0     1465 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0      674 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/rest_poller_component.py
--rw-r--r--   0        0        0     1308 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    19797 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0      377 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/resolver.py
--rw-r--r--   0        0        0     2400 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    14876 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/decoders.py
--rw-r--r--   0        0        0     3498 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/default_decoders.py
--rw-r--r--   0        0        0     3167 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     8424 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     4686 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0    10910 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     8099 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     7060 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     4742 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0      160 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      460 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      442 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3058 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0       40 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/topic.py
--rw-r--r--   0        0        0     1051 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/type_helpers/__init__.py
--rw-r--r--   0        0        0     8903 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     9989 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0    10682 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0     9167 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     7733 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     8182 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    13382 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    18081 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     2670 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/fibaro_smart_implant_cac_gt.py
--rw-r--r--   0        0        0     2957 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/fibaro_smart_implant_component_gt.py
--rw-r--r--   0        0        0    12879 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0    10675 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     9578 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     9643 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     9257 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    11994 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11089 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    15694 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    11586 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8429 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0    12903 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0     2281 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_cac_gt.py
--rw-r--r--   0        0        0     4802 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_component_gt.py
--rw-r--r--   0        0        0     2131 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_gt.py
--rw-r--r--   0        0        0     1328 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_poller_cac_gt.py
--rw-r--r--   0        0        0     1573 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_poller_component_gt.py
--rw-r--r--   0        0        0     1554 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_poller_gt.py
--rw-r--r--   0        0        0     2469 2024-02-09 20:10:06.501739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_tank_cac_gt.py
--rw-r--r--   0        0        0     3017 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_tank_component_gt.py
--rw-r--r--   0        0        0     8759 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/types/hubitat_tank_gt.py
--rw-r--r--   0        0        0    13944 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0    13876 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    10162 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0    12225 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     5914 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0     9931 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/relay_cac_gt.py
--rw-r--r--   0        0        0    11584 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/relay_component_gt.py
--rw-r--r--   0        0        0    11464 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0    11818 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0     2364 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/types/rest_poller_cac_gt.py
--rw-r--r--   0        0        0     3032 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/types/rest_poller_component_gt.py
--rw-r--r--   0        0        0     8899 2024-02-09 20:10:25.841795 gridworks_protocol-0.7.1/src/gwproto/types/rest_poller_gt.py
--rw-r--r--   0        0        0    12487 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0    11391 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     9455 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    14589 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    12355 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/ta_data_channels.py
--rw-r--r--   0        0        0    11280 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    11368 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2890 2024-02-09 20:10:06.505739 gridworks_protocol-0.7.1/src/gwproto/utils.py
--rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 gridworks_protocol-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 16:03:09.123299 gridworks_protocol-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3087 2024-04-01 16:03:09.123299 gridworks_protocol-0.7.2/README.md
+-rw-r--r--   0        0        0     2291 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2030 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     1340 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0      143 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/fibaro_smart_implant_cac.py
+-rw-r--r--   0        0        0      132 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/hubitat_cac.py
+-rw-r--r--   0        0        0      138 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/hubitat_poller_cac.py
+-rw-r--r--   0        0        0      142 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/hubitat_tank_module_cac.py
+-rw-r--r--   0        0        0     1489 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      996 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1113 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1119 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0      135 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/rest_poller_cac.py
+-rw-r--r--   0        0        0     1581 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0     1388 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1095 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1660 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0      533 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/fibaro_smart_implant_component.py
+-rw-r--r--   0        0        0      769 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_component.py
+-rw-r--r--   0        0        0     3141 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_poller_component.py
+-rw-r--r--   0        0        0     3701 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_tank_component.py
+-rw-r--r--   0        0        0     1480 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1482 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1268 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1466 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0      674 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/rest_poller_component.py
+-rw-r--r--   0        0        0     1309 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      165 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    19818 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0      377 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/resolver.py
+-rw-r--r--   0        0        0     2401 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    14860 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/decoders.py
+-rw-r--r--   0        0        0     3498 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/default_decoders.py
+-rw-r--r--   0        0        0     3167 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     8424 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     4686 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0    10910 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     8099 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     7060 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     4742 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0      336 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      442 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3168 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0    11428 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/topic.py
+-rw-r--r--   0        0        0     1051 2024-04-01 16:03:09.131298 gridworks_protocol-0.7.2/src/gwproto/type_helpers/__init__.py
+-rw-r--r--   0        0        0     8903 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     9990 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0    10683 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0     9168 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     7734 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     8183 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    13383 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    18082 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     2670 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_cac_gt.py
+-rw-r--r--   0        0        0     2959 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_component_gt.py
+-rw-r--r--   0        0        0    12880 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    10676 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     9579 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     9646 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     9258 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    11997 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11090 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    15695 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    11589 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8430 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0    12904 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0     2281 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_cac_gt.py
+-rw-r--r--   0        0        0     4802 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_component_gt.py
+-rw-r--r--   0        0        0     2129 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_gt.py
+-rw-r--r--   0        0        0     1328 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_cac_gt.py
+-rw-r--r--   0        0        0     1573 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_component_gt.py
+-rw-r--r--   0        0        0     1554 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_gt.py
+-rw-r--r--   0        0        0     2469 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_cac_gt.py
+-rw-r--r--   0        0        0     3017 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_component_gt.py
+-rw-r--r--   0        0        0     8759 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_gt.py
+-rw-r--r--   0        0        0    13945 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0    13879 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    10163 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0    12226 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     5915 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0     9932 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0    11585 2024-04-01 16:03:23.135277 gridworks_protocol-0.7.2/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11465 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0    11819 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0     2364 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_cac_gt.py
+-rw-r--r--   0        0        0     3033 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_component_gt.py
+-rw-r--r--   0        0        0     8900 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_gt.py
+-rw-r--r--   0        0        0    12488 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0    11394 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     9456 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    14590 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    12356 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/ta_data_channels.py
+-rw-r--r--   0        0        0    11281 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    11369 2024-04-01 16:03:23.139277 gridworks_protocol-0.7.2/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     2890 2024-04-01 16:03:09.135299 gridworks_protocol-0.7.2/src/gwproto/utils.py
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 gridworks_protocol-0.7.2/PKG-INFO
```

### Comparing `gridworks_protocol-0.7.1/LICENSE` & `gridworks_protocol-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/README.md` & `gridworks_protocol-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/pyproject.toml` & `gridworks_protocol-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.7.1"
+version = "0.7.2"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
@@ -15,20 +15,20 @@
     "Development Status :: 2 - Pre-Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks-protocol/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <4.0"
+python = "^3.10"
 pydantic = "^1.10.2"
-pendulum = "^2.1.2"
-fastapi-utils = "^0.2.1"
-gridworks = "^0.2.9"
+pendulum = "^3"
 yarl = "^1.9.2"
+pytz = "^2024.1"
+fastapi-utils = "^0.2.1"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
@@ -40,15 +40,14 @@
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
-safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/__init__.py` & `gridworks_protocol-0.7.2/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ElectricMeterCac definition"""
+
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import LocalCommInterface
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MultipurposeSensorCac definition"""
+
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import MakeModel
 from gwproto.enums import TelemetryName
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PipeFlowSensorCac definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/relay_cac.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RelayCac definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import MakeModel
 from gwproto.enums import TelemetryName
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ElectricHeaterCac definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SimpleTempSensorCac definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
 from gwproto.enums import MakeModel
 from gwproto.enums import TelemetryName
 from gwproto.enums import Unit
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/component_attribute_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ ComponentAttributeClass"""
+
 from abc import ABC
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.mixin import StreamlinedSerializerMixin
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ElectricMeterComponent definition"""
+
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from gwproto.data_classes.cacs.electric_meter_cac import ElectricMeterCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/fibaro_smart_implant_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/fibaro_smart_implant_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/hubitat_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/hubitat_poller_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_poller_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/hubitat_tank_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/hubitat_tank_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MutlipurposeSensorComponent definition"""
+
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from gwproto.data_classes.cacs.multipurpose_sensor_cac import MultipurposeSensorCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PipeFlowSensorComponent definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.cacs.pipe_flow_sensor_cac import PipeFlowSensorCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/relay_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/relay_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RelayComponent definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.cacs.relay_cac import RelayCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ResistiveHeaterComponent definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.cacs.resistive_heater_cac import ResistiveHeaterCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/rest_poller_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/rest_poller_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SimpleTempSensorComponent definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.cacs.simple_temp_sensor_cac import SimpleTempSensorCac
 from gwproto.data_classes.component import Component
 from gwproto.enums import MakeModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/hardware_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """(Mostly) static functions describing ShNodes that were in Actor/ActorBase Scada/ScadaBase.
 
 This will probably be refactored as we implement our local registry. Currently separated out here for clarity
 because content is static (except for needing a path to the houses.json file, which we should be able to do
 away with).
 """
+
 import copy
 import json
 import re
 import typing
 from dataclasses import dataclass
 from functools import cached_property
 from pathlib import Path
@@ -78,18 +79,18 @@
         ("ElectricMeterCacs", ElectricMeterCacGt_Maker),
         ("PipeFlowSensorCacs", PipeFlowSensorCacGt_Maker),
         ("MultipurposeSensorCacs", MultipurposeSensorCacGt_Maker),
         ("SimpleTempSensorCacs", SimpleTempSensorCacGt_Maker),
     ]:
         for d in layout.get(type_name, []):
             try:
-                cacs[
-                    d["ComponentAttributeClassId"]
-                ] = maker_class.dict_to_dc(  # type:ignore[attr-defined]
-                    d
+                cacs[d["ComponentAttributeClassId"]] = (
+                    maker_class.dict_to_dc(  # type:ignore[attr-defined]
+                        d
+                    )
                 )
             except Exception as e:
                 if raise_errors:
                     raise e
                 errors.append(LoadError(type_name, d, e))
     if cac_decoder is None:
         cac_decoder = default_cac_decoder
@@ -125,18 +126,18 @@
         ("ElectricMeterComponents", ElectricMeterComponentGt_Maker),
         ("PipeFlowSensorComponents", PipeFlowSensorComponentGt_Maker),
         ("MultipurposeSensorComponents", MultipurposeSensorComponentGt_Maker),
         ("SimpleTempSensorComponents", SimpleTempSensorComponentGt_Maker),
     ]:
         for d in layout.get(type_name, []):
             try:
-                components[
-                    d["ComponentId"]
-                ] = maker_class.dict_to_dc(  # type:ignore[attr-defined]
-                    d
+                components[d["ComponentId"]] = (
+                    maker_class.dict_to_dc(  # type:ignore[attr-defined]
+                        d
+                    )
                 )
             except Exception as e:
                 if raise_errors:
                     raise e
                 errors.append(LoadError(type_name, d, e))
     if component_decoder is None:
         component_decoder = default_component_decoder
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.7.2/src/gwproto/data_classes/sh_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ShNode definition"""
+
 from typing import Dict
 from typing import Optional
 
 from gwproto.data_classes.component import Component
 from gwproto.data_classes.errors import DataClassLoadingError
 from gwproto.enums import ActorClass
 from gwproto.enums import Role
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/decoders.py` & `gridworks_protocol-0.7.2/src/gwproto/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 class Decoder(abc.ABC):
     def decode_str(self, content: str | bytes, encoding: str = "utf-8") -> Any:
         if isinstance(content, bytes):
             content = content.decode(encoding)
         return self.decode_obj(json.loads(content))
 
     @abstractmethod
-    def decode_obj(self, o: Any) -> Any:
-        ...
+    def decode_obj(self, o: Any) -> Any: ...
 
 
 class CallableDecoder(Decoder):
     _decode_obj: Callable[[Any], Any]
 
     def __init__(self, decode_obj: Callable[[Any], Any]):
         if not callable(decode_obj):
@@ -265,16 +264,15 @@
             )
         self.validate_source_alias(decoded_topic.src)
         return self.decoders.decode_str(
             decoded_topic.envelope_type, payload, encoding=self.ENCODING
         )
 
     @abstractmethod
-    def validate_source_alias(self, source_alias: str):
-        ...
+    def validate_source_alias(self, source_alias: str): ...
 
 
 def get_pydantic_literal_type_name(
     o: Any, type_name_field: str = DEFAULT_TYPE_NAME_FIELD
 ) -> str:
     if hasattr(o, "__fields__"):
         if type_name_field in o.__fields__:
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/default_decoders.py` & `gridworks_protocol-0.7.2/src/gwproto/default_decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/__init__.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/actor_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/role.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/enums/unit.py` & `gridworks_protocol-0.7.2/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.7.2/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.7.2/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/message.py` & `gridworks_protocol-0.7.2/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.7.2/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/messages/event.py` & `gridworks_protocol-0.7.2/src/gwproto/messages/event.py`

 * *Files 24% similar despite different names*

```diff
@@ -67,57 +67,56 @@
         return as_enum(v, Problems, Problems.error)
 
 
 class CommEvent(EventBase):
     PeerName: str
 
 
-class MQTTCommEvent(CommEvent):
-    ...
+class MQTTCommEvent(CommEvent): ...
 
 
 class MQTTConnectEvent(MQTTCommEvent):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.comm.mqtt.connect"] = (
         "gridworks.event.comm.mqtt.connect"
-    ] = "gridworks.event.comm.mqtt.connect"
+    )
 
 
 class MQTTConnectFailedEvent(MQTTCommEvent):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.comm.mqtt.connect.failed"] = (
         "gridworks.event.comm.mqtt.connect.failed"
-    ] = "gridworks.event.comm.mqtt.connect.failed"
+    )
 
 
 class MQTTDisconnectEvent(MQTTCommEvent):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.comm.mqtt.disconnect"] = (
         "gridworks.event.comm.mqtt.disconnect"
-    ] = "gridworks.event.comm.mqtt.disconnect"
+    )
 
 
 class MQTTFullySubscribedEvent(CommEvent):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.comm.mqtt.fully.subscribed"] = (
         "gridworks.event.comm.mqtt.fully.subscribed"
-    ] = "gridworks.event.comm.mqtt.fully.subscribed"
+    )
 
 
 class ResponseTimeoutEvent(CommEvent):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.comm.response.timeout"] = (
         "gridworks.event.comm.response.timeout"
-    ] = "gridworks.event.comm.response.timeout"
+    )
 
 
 class PeerActiveEvent(CommEvent):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.comm.peer.active"] = (
         "gridworks.event.comm.peer.active"
-    ] = "gridworks.event.comm.peer.active"
+    )
 
 
 class GtShStatusEvent(EventBase):
     status: GtShStatus | dict
     TypeName: Literal["gridworks.event.gt.sh.status"] = "gridworks.event.gt.sh.status"
 
 
 class SnapshotSpaceheatEvent(EventBase):
     snap: SnapshotSpaceheat | dict
-    TypeName: Literal[
+    TypeName: Literal["gridworks.event.snapshot.spaceheat"] = (
         "gridworks.event.snapshot.spaceheat"
-    ] = "gridworks.event.snapshot.spaceheat"
+    )
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/messages/misc.py` & `gridworks_protocol-0.7.2/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/topic.py` & `gridworks_protocol-0.7.2/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/type_helpers/__init__.py` & `gridworks_protocol-0.7.2/src/gwproto/type_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/__init__.py` & `gridworks_protocol-0.7.2/src/gwproto/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/component_attribute_class_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type component.attribute.class.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/component_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.7.2/src/gwproto/types/data_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type data.channel, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.7.2/src/gwproto/types/egauge_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type egauge.io, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.7.2/src/gwproto/types/egauge_register_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type egauge.register.config, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type electric.meter.cac.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/electric_meter_component_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type electric.meter.component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/fibaro_smart_implant_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/fibaro_smart_implant_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/fibaro_smart_implant_component_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     FibaroSmartImplantComponent,
 )
 from gwproto.types import ComponentGt
 
 
 class FibaroSmartImplantComponentGt(ComponentGt):
     ZWaveDSK: str = ""
-    TypeName: Literal[
+    TypeName: Literal["fibaro.smart.implant.component.gt"] = (
         "fibaro.smart.implant.component.gt"
-    ] = "fibaro.smart.implant.component.gt"
+    )
     Version: Literal["000"] = "000"
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))
 
     @classmethod
     def from_data_class(
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.dispatch.boolean, version 110"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.dispatch.boolean.local, version 110"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.driver.booleanactuator.cmd, version 100"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.sh.booleanactuator.cmd.status, version 100"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 
@@ -41,17 +42,17 @@
     )
     RelayStateCommandList: List[int] = Field(
         title="List of RelayStateCommands",
     )
     CommandTimeUnixMsList: List[int] = Field(
         title="List of Command Times",
     )
-    TypeName: Literal[
+    TypeName: Literal["gt.sh.booleanactuator.cmd.status"] = (
         "gt.sh.booleanactuator.cmd.status"
-    ] = "gt.sh.booleanactuator.cmd.status"
+    )
     Version: Literal["100"] = "100"
 
     @validator("ShNodeAlias")
     def _check_sh_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.sh.cli.atn.cmd, version 110"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.sh.multipurpose.telemetry.status, version 100"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 
@@ -61,17 +62,17 @@
         title="List of Values",
         description="The values of the readings.",
     )
     ReadTimeUnixMsList: List[int] = Field(
         title="List of Read Times",
         description="The times that the MultipurposeSensor took the readings, in unix milliseconds",
     )
-    TypeName: Literal[
+    TypeName: Literal["gt.sh.multipurpose.telemetry.status"] = (
         "gt.sh.multipurpose.telemetry.status"
-    ] = "gt.sh.multipurpose.telemetry.status"
+    )
     Version: Literal["100"] = "100"
 
     @validator("AboutNodeAlias")
     def _check_about_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.sh.simple.telemetry.status, version 100"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.sh.status, version 110"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.sh.telemetry.from.multipurpose.sensor, version 100"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 
@@ -47,17 +48,17 @@
             "of the nth alias in the AboutNodeAliasList."
             "[More info](https://gridworks-protocol.readthedocs.io/en/latest/enums.html#gridworks-protocol.enums.TelemetryName)"
         ),
     )
     ValueList: List[int] = Field(
         title="ValueList",
     )
-    TypeName: Literal[
+    TypeName: Literal["gt.sh.telemetry.from.multipurpose.sensor"] = (
         "gt.sh.telemetry.from.multipurpose.sensor"
-    ] = "gt.sh.telemetry.from.multipurpose.sensor"
+    )
     Version: Literal["100"] = "100"
 
     @validator("ScadaReadTimeUnixMs")
     def _check_scada_read_time_unix_ms(cls, v: int) -> int:
         try:
             check_is_reasonable_unix_time_ms(v)
         except ValueError as e:
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.7.2/src/gwproto/types/gt_telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type gt.telemetry, version 110"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.7.2/src/gwproto/types/heartbeat_b.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type heartbeat.b, version 001"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import yarl
-from gridworks.property_format import predicate_validator
 from pydantic import BaseModel
 
+from gwproto.property_format import predicate_validator
 from gwproto.types.rest_poller_gt import URLArgs
 from gwproto.types.rest_poller_gt import URLConfig
 from gwproto.utils import has_mac_address_format
 
 
 class HubitatGt(BaseModel):
     Host: str
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_poller_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_poller_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_poller_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_poller_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_tank_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_tank_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/hubitat_tank_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/hubitat_tank_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type multipurpose.sensor.cac.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type multipurpose.sensor.component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
@@ -68,17 +69,17 @@
         default=None,
     )
     DisplayName: Optional[str] = Field(
         title="DisplayName",
         description="Sample: Oak Multipurpose Temp Sensor Component <100>",
         default=None,
     )
-    TypeName: Literal[
+    TypeName: Literal["multipurpose.sensor.component.gt"] = (
         "multipurpose.sensor.component.gt"
-    ] = "multipurpose.sensor.component.gt"
+    )
     Version: Literal["000"] = "000"
 
     @validator("ComponentId")
     def _check_component_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type pipe.flow.sensor.cac.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type pipe.flow.sensor.component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.7.2/src/gwproto/types/power_watts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type power.watts, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/relay_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/relay_cac_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type relay.cac.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/relay_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/relay_component_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type relay.component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type resistive.heater.cac.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type resistive.heater.component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/rest_poller_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/rest_poller_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_component_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code for actors that use a simple rest interaction, converting the response to one or more
 REST commands into a message posted to main processing thread.
 
 """
+
 import json
 import typing
 from typing import Any
 from typing import Literal
 from typing import Optional
 
 from gwproto.data_classes.component import Component
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/rest_poller_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/rest_poller_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code for actors that use a simple rest interaction, converting the response to one or more
 REST commands into a message posted to main processing thread.
 
 """
+
 from functools import cached_property
 from typing import Literal
 from typing import Optional
 from typing import Tuple
 
 import yarl
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type simple.temp.sensor.cac.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type simple.temp.sensor.component.gt, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
 
@@ -62,17 +63,17 @@
         title="Hardware Unique Id",
         default=None,
     )
     Channel: Optional[int] = Field(
         title="Channel",
         default=None,
     )
-    TypeName: Literal[
+    TypeName: Literal["simple.temp.sensor.component.gt"] = (
         "simple.temp.sensor.component.gt"
-    ] = "simple.temp.sensor.component.gt"
+    )
     Version: Literal["000"] = "000"
 
     @validator("ComponentId")
     def _check_component_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.7.2/src/gwproto/types/snapshot_spaceheat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type snapshot.spaceheat, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.7.2/src/gwproto/types/spaceheat_node_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type spaceheat.node.gt, version 100"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/ta_data_channels.py` & `gridworks_protocol-0.7.2/src/gwproto/types/ta_data_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type ta.data.channels, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.7.2/src/gwproto/types/telemetry_reporting_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type telemetry.reporting.config, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.7.2/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type telemetry.snapshot.spaceheat, version 000"""
+
 import json
 import logging
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
```

### Comparing `gridworks_protocol-0.7.1/src/gwproto/utils.py` & `gridworks_protocol-0.7.2/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.7.1/PKG-INFO` & `gridworks_protocol-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.7.1
+Version: 0.7.2
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
-Requires-Dist: gridworks (>=0.2.9,<0.3.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: pendulum (>=3,<4)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-protocol/releases
 Project-URL: Documentation, https://gridworks-protocol.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-protocol
 Description-Content-Type: text/markdown
 
 # GridWorks Protocol
```

