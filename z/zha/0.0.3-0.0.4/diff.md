# Comparing `tmp/zha-0.0.3.tar.gz` & `tmp/zha-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zha-0.0.3.tar", last modified: Sun Mar 31 01:20:20 2024, max compression
+gzip compressed data, was "zha-0.0.4.tar", last modified: Mon Apr  1 15:02:33 2024, max compression
```

## Comparing `zha-0.0.3.tar` & `zha-0.0.4.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.259336 zha-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-31 01:20:15.000000 zha-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-31 01:20:20.259336 zha-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-31 01:20:15.000000 zha-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-31 01:20:15.000000 zha-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 01:20:20.259336 zha-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 01:20:15.000000 zha-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.247336 zha-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_alarm_control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19916 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_async_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    50919 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_cluster_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_debouncer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_discover.py
--rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_fan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    38131 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-03-31 01:20:15.000000 zha-0.0.3/tests/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.247336 zha-0.0.3/zha/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-31 01:20:15.000000 zha-0.0.3/zha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/alarm_control_panel/
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/alarm_control_panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/alarm_control_panel/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/binary_sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/binary_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/binary_sensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/button/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/button/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/button/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/climate/
--rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/climate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/climate/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/cover/
--rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/cover/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/device_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.251336 zha-0.0.3/zha/application/platforms/fan/
--rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/fan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/fan/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/fan/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.255336 zha-0.0.3/zha/application/platforms/light/
--rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/light/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/light/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.255336 zha-0.0.3/zha/application/platforms/lock/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/lock/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.255336 zha-0.0.3/zha/application/platforms/number/
--rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/number/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.255336 zha-0.0.3/zha/application/platforms/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    57534 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/sensor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-03-31 01:20:15.000000 zha-0.0.3/zha/application/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-03-31 01:20:15.000000 zha-0.0.3/zha/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-31 01:20:15.000000 zha-0.0.3/zha/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-03-31 01:20:15.000000 zha-0.0.3/zha/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-31 01:20:15.000000 zha-0.0.3/zha/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-31 01:20:15.000000 zha-0.0.3/zha/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-31 01:20:15.000000 zha-0.0.3/zha/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-31 01:20:15.000000 zha-0.0.3/zha/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-31 01:20:15.000000 zha-0.0.3/zha/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.255336 zha-0.0.3/zha/zigbee/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.259336 zha-0.0.3/zha/zigbee/cluster_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/closures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/hvac.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/manufacturerspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/cluster_handlers/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37554 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-03-31 01:20:15.000000 zha-0.0.3/zha/zigbee/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:20:20.259336 zha-0.0.3/zha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-31 01:20:20.000000 zha-0.0.3/zha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-03-31 01:20:20.000000 zha-0.0.3/zha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 01:20:20.000000 zha-0.0.3/zha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-31 01:20:20.000000 zha-0.0.3/zha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 01:20:20.000000 zha-0.0.3/zha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.236570 zha-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 15:02:29.000000 zha-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 15:02:33.236570 zha-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 15:02:29.000000 zha-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-01 15:02:29.000000 zha-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:02:33.236570 zha-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 15:02:29.000000 zha-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.224570 zha-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_alarm_control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21035 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50919 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_cluster_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_debouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_fan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20939 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38131 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-01 15:02:29.000000 zha-0.0.4/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.224570 zha-0.0.4/zha/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 15:02:29.000000 zha-0.0.4/zha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.228570 zha-0.0.4/zha/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26987 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.228570 zha-0.0.4/zha/application/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.228570 zha-0.0.4/zha/application/platforms/alarm_control_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/alarm_control_panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/alarm_control_panel/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.228570 zha-0.0.4/zha/application/platforms/binary_sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/binary_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/binary_sensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.228570 zha-0.0.4/zha/application/platforms/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/button/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/button/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/climate/
+-rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/climate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/climate/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/cover/
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/cover/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/device_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/fan/
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/fan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/fan/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/fan/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/light/
+-rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/light/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/light/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/lock/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/number/
+-rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/number/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/application/platforms/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    57534 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/sensor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-01 15:02:29.000000 zha-0.0.4/zha/application/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19157 2024-04-01 15:02:29.000000 zha-0.0.4/zha/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 15:02:29.000000 zha-0.0.4/zha/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-01 15:02:29.000000 zha-0.0.4/zha/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-01 15:02:29.000000 zha-0.0.4/zha/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-01 15:02:29.000000 zha-0.0.4/zha/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 15:02:29.000000 zha-0.0.4/zha/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-01 15:02:29.000000 zha-0.0.4/zha/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-01 15:02:29.000000 zha-0.0.4/zha/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.232570 zha-0.0.4/zha/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.236570 zha-0.0.4/zha/zigbee/cluster_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/manufacturerspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/cluster_handlers/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37554 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-01 15:02:29.000000 zha-0.0.4/zha/zigbee/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:02:33.236570 zha-0.0.4/zha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 15:02:33.000000 zha-0.0.4/zha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-01 15:02:33.000000 zha-0.0.4/zha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:02:33.000000 zha-0.0.4/zha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-01 15:02:33.000000 zha-0.0.4/zha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 15:02:33.000000 zha-0.0.4/zha.egg-info/top_level.txt
```

### Comparing `zha-0.0.3/LICENSE` & `zha-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/PKG-INFO` & `zha-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.3/pyproject.toml` & `zha-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_alarm_control_panel.py` & `zha-0.0.4/tests/test_alarm_control_panel.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_async_.py` & `zha-0.0.4/tests/test_async_.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,7 +649,47 @@
     )
 
     # We should trust the job_type passed in
     assert (
         ZHAJob(not_callback_func, job_type=ZHAJobType.Callback).job_type
         == ZHAJobType.Callback
     )
+
+
+async def test_async_add_executor_job_background(zha_gateway: Gateway) -> None:
+    """Test running an executor job in the background."""
+    calls = []
+
+    def job():
+        time.sleep(0.01)
+        calls.append(1)
+
+    async def _async_add_executor_job():
+        await zha_gateway.async_add_executor_job(job)
+
+    task = zha_gateway.async_create_background_task(
+        _async_add_executor_job(), "background", eager_start=True
+    )
+    await zha_gateway.async_block_till_done()
+    assert len(calls) == 0
+    await zha_gateway.async_block_till_done(wait_background_tasks=True)
+    assert len(calls) == 1
+    await task
+
+
+async def test_async_add_executor_job(zha_gateway: Gateway) -> None:
+    """Test running an executor job."""
+    calls = []
+
+    def job():
+        time.sleep(0.01)
+        calls.append(1)
+
+    async def _async_add_executor_job():
+        await zha_gateway.async_add_executor_job(job)
+
+    task = zha_gateway.async_create_task(
+        _async_add_executor_job(), "background", eager_start=True
+    )
+    await zha_gateway.async_block_till_done()
+    assert len(calls) == 1
+    await task
```

### Comparing `zha-0.0.3/tests/test_binary_sensor.py` & `zha-0.0.4/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_button.py` & `zha-0.0.4/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_climate.py` & `zha-0.0.4/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_cluster_handlers.py` & `zha-0.0.4/tests/test_cluster_handlers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_color.py` & `zha-0.0.4/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_cover.py` & `zha-0.0.4/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_debouncer.py` & `zha-0.0.4/tests/test_debouncer.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_device.py` & `zha-0.0.4/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_device_tracker.py` & `zha-0.0.4/tests/test_device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_discover.py` & `zha-0.0.4/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_fan.py` & `zha-0.0.4/tests/test_fan.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_gateway.py` & `zha-0.0.4/tests/test_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
     zha_gateway.raw_device_initialized(zigpy_dev_basic)
 
     assert zha_gateway.emit.call_count == 1
     assert zha_gateway.emit.call_args == call(
         "raw_device_initialized",
         RawDeviceInitializedEvent(
             device_info=RawDeviceInitializedDeviceInfo(
-                ieee="00:0d:6f:00:0a:90:69:e7",
+                ieee=zigpy.types.EUI64.convert("00:0d:6f:00:0a:90:69:e7"),
                 nwk=0xB79C,
                 pairing_status="INTERVIEW_COMPLETE",
                 model="FakeModel",
                 manufacturer="FakeManufacturer",
                 signature={
                     "manufacturer": "FakeManufacturer",
                     "model": "FakeModel",
```

### Comparing `zha-0.0.3/tests/test_light.py` & `zha-0.0.4/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_lock.py` & `zha-0.0.4/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_number.py` & `zha-0.0.4/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_registries.py` & `zha-0.0.4/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_select.py` & `zha-0.0.4/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_sensor.py` & `zha-0.0.4/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_siren.py` & `zha-0.0.4/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_switch.py` & `zha-0.0.4/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_units.py` & `zha-0.0.4/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/tests/test_update.py` & `zha-0.0.4/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/__init__.py` & `zha-0.0.4/zha/application/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/const.py` & `zha-0.0.4/zha/application/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,15 @@
 ZHA_CLUSTER_HANDLER_CFG_DONE = "zha_channel_cfg_done"
 ZHA_CLUSTER_HANDLER_READS_PER_REQ = 5
 ZHA_EVENT = "zha_event"
 ZHA_GW_MSG = "zha_gateway_message"
 ZHA_GW_MSG_DEVICE_FULL_INIT = "device_fully_initialized"
 ZHA_GW_MSG_DEVICE_INFO = "device_info"
 ZHA_GW_MSG_DEVICE_JOINED = "device_joined"
+ZHA_GW_MSG_DEVICE_LEFT = "device_left"
 ZHA_GW_MSG_DEVICE_REMOVED = "device_removed"
 ZHA_GW_MSG_GROUP_ADDED = "group_added"
 ZHA_GW_MSG_GROUP_INFO = "group_info"
 ZHA_GW_MSG_GROUP_MEMBER_ADDED = "group_member_added"
 ZHA_GW_MSG_GROUP_MEMBER_REMOVED = "group_member_removed"
 ZHA_GW_MSG_GROUP_REMOVED = "group_removed"
 ZHA_GW_MSG_LOG_ENTRY = "log_entry"
```

### Comparing `zha-0.0.3/zha/application/discovery.py` & `zha-0.0.4/zha/application/discovery.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/gateway.py` & `zha-0.0.4/zha/application/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     CONF_USE_THREAD,
     CONF_ZIGPY,
     UNKNOWN_MANUFACTURER,
     UNKNOWN_MODEL,
     ZHA_GW_MSG,
     ZHA_GW_MSG_DEVICE_FULL_INIT,
     ZHA_GW_MSG_DEVICE_JOINED,
+    ZHA_GW_MSG_DEVICE_LEFT,
     ZHA_GW_MSG_DEVICE_REMOVED,
     ZHA_GW_MSG_GROUP_ADDED,
     ZHA_GW_MSG_GROUP_MEMBER_ADDED,
     ZHA_GW_MSG_GROUP_MEMBER_REMOVED,
     ZHA_GW_MSG_GROUP_REMOVED,
     ZHA_GW_MSG_RAW_INIT,
     RadioType,
@@ -95,14 +96,24 @@
 
     device_info: DeviceJoinedDeviceInfo
     event_type: Final[str] = ZHA_GW_MSG
     event: Final[str] = ZHA_GW_MSG_DEVICE_JOINED
 
 
 @dataclass(kw_only=True, frozen=True)
+class DeviceLeftEvent:
+    """Event to signal that a device has joined the network."""
+
+    ieee: EUI64
+    nwk: int
+    event_type: Final[str] = ZHA_GW_MSG
+    event: Final[str] = ZHA_GW_MSG_DEVICE_LEFT
+
+
+@dataclass(kw_only=True, frozen=True)
 class RawDeviceInitializedDeviceInfo(DeviceJoinedDeviceInfo):
     """Information about a device that has been initialized without quirks loaded."""
 
     model: str
     manufacturer: str
     signature: dict[str, Any]
 
@@ -367,29 +378,29 @@
         address
         """
 
         self.emit(
             ZHA_GW_MSG_DEVICE_JOINED,
             DeviceJoinedEvent(
                 device_info=DeviceJoinedDeviceInfo(
-                    ieee=str(device.ieee),
+                    ieee=device.ieee,
                     nwk=device.nwk,
                     pairing_status=DevicePairingStatus.PAIRED.name,
                 )
             ),
         )
 
     def raw_device_initialized(self, device: zigpy.device.Device) -> None:  # pylint: disable=unused-argument
         """Handle a device initialization without quirks loaded."""
 
         self.emit(
             ZHA_GW_MSG_RAW_INIT,
             RawDeviceInitializedEvent(
                 device_info=RawDeviceInitializedDeviceInfo(
-                    ieee=str(device.ieee),
+                    ieee=device.ieee,
                     nwk=device.nwk,
                     pairing_status=DevicePairingStatus.INTERVIEW_COMPLETE.name,
                     model=device.model if device.model else UNKNOWN_MODEL,
                     manufacturer=device.manufacturer
                     if device.manufacturer
                     else UNKNOWN_MANUFACTURER,
                     signature=device.get_signature(),
@@ -414,14 +425,17 @@
 
     def device_left(self, device: zigpy.device.Device) -> None:
         """Handle device leaving the network."""
         zha_device: Device = self._devices.get(device.ieee)
         if zha_device is not None:
             zha_device.on_network = False
         self.async_update_device(device, available=False)
+        self.emit(
+            ZHA_GW_MSG_DEVICE_LEFT, DeviceLeftEvent(ieee=device.ieee, nwk=device.nwk)
+        )
 
     def group_member_removed(
         self, zigpy_group: zigpy.group.Group, endpoint: zigpy.endpoint.Endpoint
     ) -> None:
         """Handle zigpy group member removed event."""
         # need to handle endpoint correctly on groups
         zha_group = self.get_or_create_group(zigpy_group)
```

### Comparing `zha-0.0.3/zha/application/helpers.py` & `zha-0.0.4/zha/application/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/__init__.py` & `zha-0.0.4/zha/application/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/alarm_control_panel/__init__.py` & `zha-0.0.4/zha/application/platforms/alarm_control_panel/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/alarm_control_panel/const.py` & `zha-0.0.4/zha/application/platforms/alarm_control_panel/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/binary_sensor/__init__.py` & `zha-0.0.4/zha/application/platforms/binary_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/binary_sensor/const.py` & `zha-0.0.4/zha/application/platforms/binary_sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/button/__init__.py` & `zha-0.0.4/zha/application/platforms/button/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/climate/__init__.py` & `zha-0.0.4/zha/application/platforms/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/climate/const.py` & `zha-0.0.4/zha/application/platforms/climate/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/cover/__init__.py` & `zha-0.0.4/zha/application/platforms/cover/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/cover/const.py` & `zha-0.0.4/zha/application/platforms/cover/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/device_tracker.py` & `zha-0.0.4/zha/application/platforms/device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/fan/__init__.py` & `zha-0.0.4/zha/application/platforms/fan/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/fan/const.py` & `zha-0.0.4/zha/application/platforms/fan/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/fan/helpers.py` & `zha-0.0.4/zha/application/platforms/fan/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/helpers.py` & `zha-0.0.4/zha/application/platforms/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/light/__init__.py` & `zha-0.0.4/zha/application/platforms/light/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/light/const.py` & `zha-0.0.4/zha/application/platforms/light/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/light/helpers.py` & `zha-0.0.4/zha/application/platforms/light/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/lock/__init__.py` & `zha-0.0.4/zha/application/platforms/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/number/__init__.py` & `zha-0.0.4/zha/application/platforms/number/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/number/const.py` & `zha-0.0.4/zha/application/platforms/number/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/select.py` & `zha-0.0.4/zha/application/platforms/select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/sensor/__init__.py` & `zha-0.0.4/zha/application/platforms/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/sensor/const.py` & `zha-0.0.4/zha/application/platforms/sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/siren.py` & `zha-0.0.4/zha/application/platforms/siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/switch.py` & `zha-0.0.4/zha/application/platforms/switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/platforms/update.py` & `zha-0.0.4/zha/application/platforms/update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/application/registries.py` & `zha-0.0.4/zha/application/registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/async_.py` & `zha-0.0.4/zha/async_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Async utilities for Zigbee Home Automation."""
 
+from __future__ import annotations
+
 import asyncio
 from asyncio import AbstractEventLoop, Future, Semaphore, Task, gather, get_running_loop
 from collections.abc import Awaitable, Callable, Collection, Coroutine, Iterable
 from dataclasses import dataclass
 import enum
 import functools
 from functools import cached_property
@@ -227,15 +229,15 @@
                 functools.partial(self.async_create_task, target, eager_start=True)
             )
             return
         if TYPE_CHECKING:
             target = cast(Callable[..., Any], target)
         self.loop.call_soon_threadsafe(
             functools.partial(
-                self.async_add_job, ZHAJob(target), *args, eager_start=True
+                self.async_add_zha_job, ZHAJob(target), *args, eager_start=True
             )
         )
 
     def _cancel_cancellable_timers(self) -> None:
         """Cancel timer handles marked as cancellable."""
         # pylint: disable-next=protected-access
         handles: Iterable[asyncio.TimerHandle] = self.loop._scheduled  # type: ignore[attr-defined]
@@ -462,28 +464,31 @@
 
     @callback
     def async_add_executor_job(
         self, target: Callable[..., _T], *args: Any
     ) -> asyncio.Future[_T]:
         """Add an executor job from within the event loop."""
         task = self.loop.run_in_executor(None, target, *args)
-        self._tracked_completable_tasks.add(task)
-        task.add_done_callback(self._tracked_completable_tasks.remove)
-
+        tracked = asyncio.current_task() in self._tracked_completable_tasks
+        task_bucket = (
+            self._tracked_completable_tasks if tracked else self._background_tasks
+        )
+        task_bucket.add(task)
+        task.add_done_callback(task_bucket.remove)
         return task
 
     @callback
     def async_add_import_executor_job(
         self, target: Callable[..., _T], *args: Any
     ) -> asyncio.Future[_T]:
-        """Add an import executor job from within the event loop."""
-        task = self.loop.run_in_executor(self.import_executor, target, *args)
-        self._tracked_completable_tasks.add(task)
-        task.add_done_callback(self._tracked_completable_tasks.remove)
-        return task
+        """Add an import executor job from within the event loop.
+
+        The future returned from this method must be awaited in the event loop.
+        """
+        return self.loop.run_in_executor(self.import_executor, target, *args)
 
     @overload
     @callback
     def async_run_zha_job(
         self,
         zhajob: ZHAJob[..., Coroutine[Any, Any, _R]],
         *args: Any,
```

### Comparing `zha-0.0.3/zha/debounce.py` & `zha-0.0.4/zha/debounce.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/decorators.py` & `zha-0.0.4/zha/decorators.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/event.py` & `zha-0.0.4/zha/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,39 +46,40 @@
             if callback in self._golbal_listeners:
                 self._golbal_listeners.remove(callback)
 
         return unsubscribe
 
     def once(self, event_name: str, callback: Callable) -> Callable:
         """Listen for an event exactly once."""
+        if inspect.iscoroutinefunction(callback):
+
+            async def async_event_listener(data: dict) -> None:
+                unsub()
+                task = asyncio.create_task(callback(data))
+                self._event_tasks.append(task)
+                task.add_done_callback(self._event_tasks.remove)
+
+            unsub = self.on_event(event_name, async_event_listener)
+            return unsub
 
         def event_listener(data: dict) -> None:
             unsub()
             callback(data)
 
         unsub = self.on_event(event_name, event_listener)
-
         return unsub
 
     def emit(self, event_name: str, data=None) -> None:
         """Run all callbacks for an event."""
         for listener in [*self._listeners.get(event_name, []), *self._golbal_listeners]:
             if inspect.iscoroutinefunction(listener):
-                if data is None:
-                    task = asyncio.create_task(listener())
-                    self._event_tasks.append(task)
-                    task.add_done_callback(self._event_tasks.remove)
-                else:
-                    task = asyncio.create_task(listener(data))
-                    self._event_tasks.append(task)
-                    task.add_done_callback(self._event_tasks.remove)
-            elif data is None:
-                listener()
-            else:
-                listener(data)
+                task = asyncio.create_task(listener(data))
+                self._event_tasks.append(task)
+                task.add_done_callback(self._event_tasks.remove)
+            listener(data)
 
     def _handle_event_protocol(self, event) -> None:
         """Process an event based on event protocol."""
         _LOGGER.debug(
             "(%s) handling event protocol for event: %s", self.__class__.__name__, event
         )
         handler = getattr(self, f"handle_{event.event.replace(' ', '_')}", None)
```

### Comparing `zha-0.0.3/zha/mixins.py` & `zha-0.0.4/zha/mixins.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/units.py` & `zha-0.0.4/zha/units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/__init__.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/closures.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/closures.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/const.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/general.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/general.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/helpers.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/homeautomation.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/hvac.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/hvac.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/lighting.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/lighting.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/lightlink.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/lightlink.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/manufacturerspecific.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/manufacturerspecific.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/measurement.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/measurement.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/protocol.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/protocol.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/security.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/security.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/cluster_handlers/smartenergy.py` & `zha-0.0.4/zha/zigbee/cluster_handlers/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/device.py` & `zha-0.0.4/zha/zigbee/device.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/endpoint.py` & `zha-0.0.4/zha/zigbee/endpoint.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.3/zha/zigbee/group.py` & `zha-0.0.4/zha/zigbee/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,16 @@
 
     @cached_property
     def associated_entities(self) -> list[PlatformEntity]:
         """Return the list of entities that were derived from this endpoint."""
         return [
             platform_entity
             for platform_entity in self._device.platform_entities.values()
-            if platform_entity.endpoint.id == self.endpoint_id
+            if hasattr(platform_entity, "endpoint")
+            and platform_entity.endpoint.id == self.endpoint_id
         ]
 
     async def async_remove_from_group(self) -> None:
         """Remove the device endpoint from the provided zigbee group."""
         try:
             await self._device.device.endpoints[self._endpoint_id].remove_from_group(
                 self._group.group_id
```

### Comparing `zha-0.0.3/zha.egg-info/PKG-INFO` & `zha-0.0.4/zha.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.3/zha.egg-info/SOURCES.txt` & `zha-0.0.4/zha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 tests/test_cluster_handlers.py
 tests/test_color.py
 tests/test_cover.py
 tests/test_debouncer.py
 tests/test_device.py
 tests/test_device_tracker.py
 tests/test_discover.py
+tests/test_event.py
 tests/test_fan.py
 tests/test_gateway.py
 tests/test_light.py
 tests/test_lock.py
 tests/test_number.py
 tests/test_registries.py
 tests/test_select.py
```

