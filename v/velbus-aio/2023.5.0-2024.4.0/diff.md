# Comparing `tmp/velbus-aio-2023.5.0.tar.gz` & `tmp/velbus-aio-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velbus-aio-2023.5.0.tar", last modified: Fri May  5 17:41:24 2023, max compression
+gzip compressed data, was "velbus-aio-2024.4.0.tar", last modified: Mon Apr  1 10:44:45 2024, max compression
```

## Comparing `velbus-aio-2023.5.0.tar` & `velbus-aio-2024.4.0.tar`

### file list

```diff
@@ -1,117 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.764804 velbus-aio-2023.5.0/velbus_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.768804 velbus-aio-2023.5.0/velbusaio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/command_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/velbusaio/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/blind_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_part1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_part2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_part3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/clear_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/counter_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_down.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dali_dim_value_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dimmer_channel_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dimmer_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/edge_set_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/edge_set_custom_color.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/forced_off.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/forced_on.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/interface_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/ir_receiver_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/kwh_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/light_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memo_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memory_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memory_data_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memory_dump_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/meteo_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_type_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/push_button_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/read_data_block_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/read_data_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/realtime_clock_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/receive_buffer_full.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/receive_ready.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/relay_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/restore_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/select_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/sensor_temp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/sensor_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_daylight_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_realtime_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/slider_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/slow_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/start_relay_blinking_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/start_relay_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_relay_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_relay_on.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_comfort.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_night.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part1.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part2.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part3.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part4.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_set_cooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_set_heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/update_led_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/very_fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/write_data_to_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/write_memory_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/write_module_address_and_serial_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/velbusaio/moduleprotocol/
--rw-r--r--   0 runner    (1001) docker     (123)   883766 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/moduleprotocol/protocol.json
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/raw_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/velbus_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 10:44:45.000000 velbus-aio-2024.4.0/velbus_aio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.607878 velbus-aio-2024.4.0/velbusaio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22998 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:45.619878 velbus-aio-2024.4.0/velbusaio/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/blind_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/bus_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_part3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/channel_name_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/clear_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/cover_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dali_dim_value_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dimmer_channel_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/dimmer_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/edge_set_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/edge_set_custom_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/forced_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/forced_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/interface_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/ir_receiver_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/kwh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/light_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memo_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memory_data_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/memory_dump_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/module_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/push_button_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/read_data_block_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/read_data_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/realtime_clock_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/receive_buffer_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/receive_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/relay_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/restore_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/select_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/sensor_temp_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/sensor_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_daylight_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_realtime_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/set_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/slider_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/slow_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/start_relay_blinking_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/start_relay_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_relay_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_relay_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_comfort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_night.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/switch_to_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_set_cooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/temp_set_heating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/update_led_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/very_fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/write_data_to_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/write_memory_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/messages/write_module_address_and_serial_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34978 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250285 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/protocol.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/raw_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-01 10:44:41.000000 velbus-aio-2024.4.0/velbusaio/util.py
```

### Comparing `velbus-aio-2023.5.0/LICENSE` & `velbus-aio-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.5.0/PKG-INFO` & `velbus-aio-2024.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
@@ -14,22 +14,27 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial>=3.5.0
+Requires-Dist: pyserial-asyncio>=0.5
+Requires-Dist: backoff>=1.10.0
 
 ![CI](https://github.com/Cereal2nd/velbus-aio/actions/workflows/main.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Cereal2nd/velbus-aio/master.svg)](https://results.pre-commit.ci/latest/github/Cereal2nd/velbus-aio/master)
 
 # velbus-aio
 
 Velbus Asyncio, a library to support the [Velbus](https://www.velbus.eu/) home automation system.
 
 This Lib is a rewrite in python3 with asyncio of the [python-velbus](https://github.com/thomasdelaet/python-velbus/) module.
 Part of the code from the above lib is reused.
```

### Comparing `velbus-aio-2023.5.0/README.md` & `velbus-aio-2024.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ![CI](https://github.com/Cereal2nd/velbus-aio/actions/workflows/main.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Cereal2nd/velbus-aio/master.svg)](https://results.pre-commit.ci/latest/github/Cereal2nd/velbus-aio/master)
 
 # velbus-aio
 
 Velbus Asyncio, a library to support the [Velbus](https://www.velbus.eu/) home automation system.
 
 This Lib is a rewrite in python3 with asyncio of the [python-velbus](https://github.com/thomasdelaet/python-velbus/) module.
 Part of the code from the above lib is reused.
```

### Comparing `velbus-aio-2023.5.0/pyproject.toml` & `velbus-aio-2024.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
-name        = "velbus-aio"
-license     = {text = "MIT"}
-version     = "2023.5.0"
+name = "velbus-aio"
+license = {text = "MIT"}
+version = "2024.4.0"
 description = "Open-source home automation platform running on Python 3."
-readme      = "README.md"
-authors     = [
+readme = "README.md"
+authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
-keywords    = ["home", "velbus", "automation"]
+keywords = ["home", "velbus", "automation"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Home Automation",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8.0"
-dependencies    = [
+dependencies = [
     "pyserial>=3.5.0",
     "pyserial-asyncio>=0.5",
     "backoff>=1.10.0",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/Cereal2nd/velbus-aio"
@@ -41,28 +42,24 @@
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*", "examples"]
 
+[tool.bandit]
+exclude_dirs = ["tests"]
+skips = ["B301", "B403", "B323", "B104", "B110"]
+
 [tool.bumpver]
-current_version = "2023.5.0"
+current_version = "2024.4.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'version = "{version}"',
-    'current_version = "{version}"',
-]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
+    '^version = "{version}"',
+    '^current_version = "{version}"',
 ]
```

### Comparing `velbus-aio-2023.5.0/velbus_aio.egg-info/PKG-INFO` & `velbus-aio-2024.4.0/velbus_aio.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
@@ -14,22 +14,27 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyserial>=3.5.0
+Requires-Dist: pyserial-asyncio>=0.5
+Requires-Dist: backoff>=1.10.0
 
 ![CI](https://github.com/Cereal2nd/velbus-aio/actions/workflows/main.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Cereal2nd/velbus-aio/master.svg)](https://results.pre-commit.ci/latest/github/Cereal2nd/velbus-aio/master)
 
 # velbus-aio
 
 Velbus Asyncio, a library to support the [Velbus](https://www.velbus.eu/) home automation system.
 
 This Lib is a rewrite in python3 with asyncio of the [python-velbus](https://github.com/thomasdelaet/python-velbus/) module.
 Part of the code from the above lib is reused.
```

### Comparing `velbus-aio-2023.5.0/velbus_aio.egg-info/SOURCES.txt` & `velbus-aio-2024.4.0/velbus_aio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 velbusaio/controller.py
 velbusaio/discovery.py
 velbusaio/exceptions.py
 velbusaio/handler.py
 velbusaio/helpers.py
 velbusaio/message.py
 velbusaio/module.py
+velbusaio/protocol.json
 velbusaio/protocol.py
 velbusaio/py.typed
 velbusaio/raw_message.py
 velbusaio/util.py
 velbusaio/messages/__init__.py
 velbusaio/messages/blind_status.py
 velbusaio/messages/bus_active.py
@@ -56,21 +57,21 @@
 velbusaio/messages/ir_receiver_status.py
 velbusaio/messages/kwh_status.py
 velbusaio/messages/light_value_request.py
 velbusaio/messages/memo_text.py
 velbusaio/messages/memory_data.py
 velbusaio/messages/memory_data_block.py
 velbusaio/messages/memory_dump_request.py
-velbusaio/messages/meteo_raw.py
 velbusaio/messages/module_status.py
 velbusaio/messages/module_status_request.py
 velbusaio/messages/module_subtype.py
 velbusaio/messages/module_type.py
 velbusaio/messages/module_type_request.py
 velbusaio/messages/push_button_status.py
+velbusaio/messages/raw.py
 velbusaio/messages/read_data_block_from_memory.py
 velbusaio/messages/read_data_from_memory.py
 velbusaio/messages/realtime_clock_status_request.py
 velbusaio/messages/receive_buffer_full.py
 velbusaio/messages/receive_ready.py
 velbusaio/messages/relay_status.py
 velbusaio/messages/restore_dimmer.py
@@ -102,9 +103,8 @@
 velbusaio/messages/temp_sensor_status.py
 velbusaio/messages/temp_set_cooling.py
 velbusaio/messages/temp_set_heating.py
 velbusaio/messages/update_led_status.py
 velbusaio/messages/very_fast_blinking_led.py
 velbusaio/messages/write_data_to_memory.py
 velbusaio/messages/write_memory_block.py
-velbusaio/messages/write_module_address_and_serial_number.py
-velbusaio/moduleprotocol/protocol.json
+velbusaio/messages/write_module_address_and_serial_number.py
```

### Comparing `velbus-aio-2023.5.0/velbusaio/channels.py` & `velbus-aio-2024.4.0/velbusaio/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 import asyncio
 import math
 import string
 from typing import TYPE_CHECKING, Any, Awaitable, Callable
 
@@ -131,14 +132,26 @@
         d = self.__dict__
         return {
             k: d[k]
             for k in d
             if k != "_writer" and k != "_on_status_update" and k != "_name_parts"
         }
 
+    def to_json(self) -> dict:
+        d = self.__dict__
+        return {
+            k: d[k]
+            for k in d
+            if k != "_writer"
+            and k != "_on_status_update"
+            and k != "_name_parts"
+            and k != "_module"
+            and k != "__name__"
+        }
+
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._on_status_update = []
         self._name_parts = {}
 
     def __repr__(self) -> str:
         items = []
@@ -187,14 +200,17 @@
 
     def get_max(self) -> int:
         raise NotImplementedError()
 
     def get_min(self) -> int:
         raise NotImplementedError()
 
+    def is_water(self) -> bool:
+        return False
+
     async def press(self) -> None:
         raise NotImplementedError()
 
 
 class Blind(Channel):
     """
     A blind channel
@@ -257,14 +273,18 @@
         cls = commandRegistry.get_command(0x04, self._module.get_type())
         msg = cls(self._address)
         msg.channel = self._num
         await self._writer(msg)
 
     async def set_position(self, position: int) -> None:
         # may not be supported by the module
+        if position == 100:
+            # at least VMB1BLS ignores command 0x1C with position 0x64
+            await self.close()
+            return
         cls = commandRegistry.get_command(0x1C, self._module.get_type())
         msg = cls(self._address)
         msg.channel = self._num
         msg.position = position
         await self._writer(msg)
 
 
@@ -339,14 +359,16 @@
         await self._writer(msg)
 
 
 class ButtonCounter(Button):
     """
     A ButtonCounter channel
     This channel can act as a button and as a counter
+    => standard     this is the calculated value
+    => is_counter   this is the numeric value
     """
 
     _Unit = None
     _pulses = None
     _counter = None
     _delay = None
 
@@ -375,28 +397,33 @@
         elif self._Unit == ENERGY_KILO_WATT_HOUR:
             val = (1000 * 1000 * 3600) / (self._delay * self._pulses)
         else:
             val = 0
         return round(val, 2)
 
     def get_unit(self) -> str | None:
-        if self._Unit in (
-            VOLUME_LITERS_HOUR,
-            VOLUME_CUBIC_METER_HOUR,
-            ENERGY_KILO_WATT_HOUR,
-        ):
-            return self._Unit
+        if self._Unit == VOLUME_LITERS_HOUR:
+            return "L"
+        if self._Unit == VOLUME_CUBIC_METER_HOUR:
+            return "m3"
+        if self._Unit == ENERGY_KILO_WATT_HOUR:
+            return "W"
         return None
 
     def get_counter_state(self) -> int:
         return round((self._counter / self._pulses), 2)
 
     def get_counter_unit(self) -> str:
         return self._Unit
 
+    def is_water(self) -> bool:
+        if self._counter and self._Unit == VOLUME_LITERS_HOUR:
+            return True
+        return False
+
 
 class Sensor(Button):
     """
     A Sensor channel
     This is a bit weird, but this happens because of code sharing with openhab
     A sensor in this case is actually a Button
     """
@@ -523,14 +550,17 @@
 
     def get_climate_preset(self) -> str:
         return self._cmode
 
     def get_climate_mode(self) -> str:
         return self._cstatus
 
+    def get_cool_mode(self) -> str:
+        return self._cool_mode
+
     async def set_temp(self, temp: float) -> None:
         cls = commandRegistry.get_command(0xE4, self._module.get_type())
         msg = cls(self._address)
         msg.temp = temp * 2  # TODO: int()
         await self._writer(msg)
 
     async def _switch_mode(self) -> None:
@@ -611,23 +641,24 @@
 
 class SensorNumber(Channel):
     """
     A Numeric Sensor channel
     """
 
     _cur = 0
+    _unit = None
 
     def get_categories(self) -> list[str]:
         return ["sensor"]
 
     def get_class(self) -> None:
         return None
 
     def get_unit(self) -> None:
-        return None
+        return self._unit
 
     def get_state(self) -> float:
         return round(self._cur, 2)
 
 
 class LightSensor(Channel):
     """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/command_registry.py` & `velbus-aio-2024.4.0/velbusaio/command_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com> and Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 MODULE_DIRECTORY = {
     0x01: "VMB8PB",
     0x02: "VMB1RY",
     0x03: "VMB1BL",
+    0x04: "VMB4LEDPWM-20",
     0x05: "VMB6IN",
     0x07: "VMB1DM",
     0x08: "VMB4RY",
     0x09: "VMB2BL",
     0x0A: "VMB8IR",
     0x0B: "VMB4PD",
     0x0C: "VMB1TS",
@@ -61,14 +63,30 @@
     0x3F: "VMCM3",
     0x40: "VMBUSBIP",
     0x41: "VMB1RYS",
     0x42: "VMBKP",
     0x43: "VMBIN",
     0x44: "VMB4PB",
     0x45: "VMBDALI",
+    0x48: "VMB4RYLD-10",
+    0x49: "VMB4RYNO-10",
+    0x4A: "VMB2BLE-10",
+    0x4B: "VMB8DC-20",
+    0x4C: "VMB6PB-20",
+    0x4F: "VMBEL1-20",
+    0x50: "VMBEL2-20",
+    0x51: "VMBEL4-20",
+    0x52: "VMBELO-20",
+    0x53: "VMBGP1-20",
+    0x54: "VMBGP2-20",
+    0x55: "VMBGP4-20",
+    0x56: "VMBGPO-20",
+    0x5A: "VMBDALI-20",
+    0x5C: "VMBEL4PIR-20",
+    0x5F: "VMBGP4PIR-20",
 }
 
 
 class CommandRegistry:
     def __init__(self, module_directory: dict) -> None:
         self._module_directory = module_directory
         self._default_commands = {}
```

### Comparing `velbus-aio-2023.5.0/velbusaio/const.py` & `velbus-aio-2024.4.0/velbusaio/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from typing import Final
 
 PRIORITY_HIGH: Final = 0xF8
 PRIORITY_FIRMWARE: Final = 0xF9
 PRIORITY_LOW: Final = 0xFB
@@ -39,16 +40,16 @@
 LOAD_TIMEOUT: Final = 600
 
 DEVICE_CLASS_ILLUMINANCE: Final = "illuminance"
 DEVICE_CLASS_TEMPERATURE: Final = "temperature"
 TEMP_CELSIUS: Final = "°C"
 ENERGY_KILO_WATT_HOUR: Final = "kWh"
 ENERGY_WATT_HOUR: Final = "Wh"
-VOLUME_CUBIC_METER: Final = "m3"  # Not an official constant at HA yet
-VOLUME_CUBIC_METER_HOUR: Final = "m3/h"  # Not an official constant at HA yet
+VOLUME_CUBIC_METER: Final = "m³"  # Not an official constant at HA yet
+VOLUME_CUBIC_METER_HOUR: Final = "m³/h"  # Not an official constant at HA yet
 VOLUME_LITERS: Final = "L"
 VOLUME_LITERS_HOUR: Final = "L/h"  # Not an official constant at HA yet
 
 CHANNEL_SELECTED_PROGRAM: Final = 96
 CHANNEL_EDGE_LIT: Final = 97
 CHANNEL_MEMO_TEXT: Final = 98
 CHANNEL_LIGHT_VALUE: Final = 99
```

### Comparing `velbus-aio-2023.5.0/velbusaio/controller.py` & `velbus-aio-2024.4.0/velbusaio/controller.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Main interface for the velbusaio lib
 """
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import pathlib
 import pickle
 import re
@@ -196,15 +197,14 @@
                     xonxoff=0,
                     rtscts=1,
                 )
             except (FileNotFoundError, serial.SerialException) as err:
                 raise VelbusConnectionFailed() from err
         if test_connect:
             return
-
         # if auth is required send the auth key
         if auth:
             await self._protocol.write_auth_key(auth)
 
         # scan the bus
         await self.scan()
```

### Comparing `velbus-aio-2023.5.0/velbusaio/discovery.py` & `velbus-aio-2024.4.0/velbusaio/discovery.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.5.0/velbusaio/handler.py` & `velbus-aio-2024.4.0/velbusaio/handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Velbus packet handler
 :Author maikel punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import re
 from typing import TYPE_CHECKING, Awaitable, Callable
-
 import pkg_resources
 
 from velbusaio.command_registry import commandRegistry
 from velbusaio.helpers import h2, keys_exists
 from velbusaio.message import Message
 from velbusaio.messages.module_subtype import ModuleSubTypeMessage
 from velbusaio.messages.module_type import ModuleTypeMessage
@@ -35,15 +35,15 @@
     ) -> None:
         self._log = logging.getLogger("velbus-packet")
         self._writer = writer
         self._velbus = velbus
         self._scan_complete = False
         self._scan_complete_event = asyncio.Event()
         with open(
-            pkg_resources.resource_filename(__name__, "moduleprotocol/protocol.json")
+            pkg_resources.resource_filename(__name__, "protocol.json")
         ) as protocol_file:
             self.pdata = json.load(protocol_file)
 
     def scan_finished(self) -> None:
         self._scan_complete = True
         self._scan_complete_event.set()
         self._log.debug("Scan complete")
@@ -114,71 +114,14 @@
                 "UNKNOWN module, you should initialize a full new velbus scan: packet={}, address={}, modules={}".format(
                     ":".join(format(x, "02x") for x in data),
                     address,
                     self._velbus.get_modules().keys(),
                 )
             )
 
-    # def _handle_message(self, rawMsg: RawMessage) -> None:
-    #    module_type = self._velbus.get_module(rawMsg.address).get_type()
-    #    this_msg = keys_exists(
-    #        self.pdata, "ModuleTypes", h2(module_type), "Messages", h2(rawMsg.command), "Data"
-    #    )
-    #    if this_msg and "PerByte" in this_msg:
-    #        self._per_byte(this_msg["PerByte"], rawMsg)
-
-    # def _per_byte(self, cmsg, rawMsg: RawMessage) -> dict:
-    #    result = {}
-    #    byte_index = 0
-    #    for byte in rawMsg.data:
-    #        num = str(byte_index)
-    #        # only do something if its defined
-    #        if num not in cmsg:
-    #            continue
-    #        # check if we can do a binary match
-    #        for mat in cmsg[num]["Match"]:
-    #            if (
-    #                (mat.startswith("%") and re.match(mat[1:], f"{byte:08b}"))
-    #                or mat == f"{byte:08b}"
-    #                or mat == f"{byte:02x}"
-    #            ):
-    #                result = self._per_byte_handle(
-    #                    result, cmsg[num]["Match"][mat], byte
-    #                )
-    #        byte_index += 1
-    #    return result
-
-    # def _per_byte_handle(self, result: dict, todo: dict, byte: int) -> dict:
-    #    if "Channel" in todo:
-    #        result["Channel"] = todo["Channel"]
-    #    if "Value" in todo:
-    #        result["Value"] = todo["Value"]
-    #    if "Convert" in todo:
-    #        result["ValueList"] = []
-    #        if todo["Convert"] == "Decimal":
-    #            result["ValueList"].append(int(byte))
-    #        elif todo["Convert"] == "Counter":
-    #            result["ValueList"].append(f"{byte:02x}")
-    #        elif todo["Convert"] == "Temperature":
-    #            print("CONVERT temperature")
-    #        elif todo["Convert"] == "Divider":
-    #            bin_str = f"{byte:08b}"
-    #            chan = bin_str[6:]
-    #            val = bin_str[:5]
-    #            print(f"CONVERT Divider {chan} {val}")
-    #        elif todo["Convert"] == "Channel":
-    #            print("CONVERT Channel")
-    #        elif todo["Convert"] == "ChannelBit":
-    #            print("CONVERT ChannelBit")
-    #        elif todo["Convert"].startswith("ChannelBitStatus"):
-    #            print("CONVERT ChannelBitStatus")
-    #        else:
-    #            self._log.error("UNKNOWN convert requested: {}".format(todo["Convert"]))
-    #    return result
-
     async def _handle_module_type(self, msg: Message) -> None:
         """
         load the module data
         """
         data = keys_exists(self.pdata, "ModuleTypes", h2(msg.module_type))
         if not data:
             self._log.warning(f"Module not recognized: {msg.module_type}")
```

### Comparing `velbus-aio-2023.5.0/velbusaio/helpers.py` & `velbus-aio-2024.4.0/velbusaio/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Helper functions
 """
+
 from __future__ import annotations
 
 import os
 import re
 from typing import Any, Dict
 
 from velbusaio.const import CACHEDIR
```

### Comparing `velbus-aio-2023.5.0/velbusaio/message.py` & `velbus-aio-2024.4.0/velbusaio/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The velbus abstract message class
 """
+
 from __future__ import annotations
 
 import json
 from typing import Optional
 
 from velbusaio.const import PRIORITY_FIRMWARE, PRIORITY_HIGH, PRIORITY_LOW
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/__init__.py` & `velbus-aio-2024.4.0/velbusaio/messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.messages.blind_status import BlindStatusMessage, BlindStatusNgMessage
 from velbusaio.messages.bus_active import BusActiveMessage
 from velbusaio.messages.bus_error_counter_status import BusErrorCounterStatusMessage
 from velbusaio.messages.bus_error_counter_status_request import (
     BusErrorStatusRequestMessage,
@@ -46,19 +47,19 @@
 from velbusaio.messages.ir_receiver_status import IRReceiverStatusMessage
 from velbusaio.messages.kwh_status import KwhStatusMessage
 from velbusaio.messages.light_value_request import LightValueRequest
 from velbusaio.messages.memo_text import MemoTextMessage
 from velbusaio.messages.memory_data import MemoryDataMessage
 from velbusaio.messages.memory_data_block import MemoryDataBlockMessage
 from velbusaio.messages.memory_dump_request import MemoryDumpRequestMessage
-from velbusaio.messages.meteo_raw import MeteoRawMessage
+from velbusaio.messages.raw import MeteoRawMessage, SensorRawMessage
 from velbusaio.messages.module_status import ModuleStatusMessage, ModuleStatusMessage2
 from velbusaio.messages.module_status_request import ModuleStatusRequestMessage
 from velbusaio.messages.module_subtype import ModuleSubTypeMessage
-from velbusaio.messages.module_type import ModuleTypeMessage
+from velbusaio.messages.module_type import ModuleTypeMessage, ModuleType2Message
 from velbusaio.messages.module_type_request import ModuleTypeRequestMessage
 from velbusaio.messages.push_button_status import PushButtonStatusMessage
 from velbusaio.messages.read_data_block_from_memory import (
     ReadDataBlockFromMemoryMessage,
 )
 from velbusaio.messages.read_data_from_memory import ReadDataFromMemoryMessage
 from velbusaio.messages.realtime_clock_status_request import RealtimeClockStatusRequest
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/blind_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/blind_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Tom Dupré <gitd8400@gmail.com>
 """
+
 from __future__ import annotations
 
 import json
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/bus_active.py` & `velbus-aio-2024.4.0/velbusaio/messages/bus_active.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x0A
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xDA
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/bus_error_counter_status_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xD9
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/bus_off.py` & `velbus-aio-2024.4.0/velbusaio/messages/bus_off.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x09
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/channel_name_part1.py` & `velbus-aio-2024.4.0/velbusaio/messages/channel_name_part2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xF0
+COMMAND_CODE = 0xF1
 
 
 @register(COMMAND_CODE)
-class ChannelNamePart1Message(Message):
+class ChannelNamePart2Message(Message):
     """
     send by: VMB6IN, VMB4RYLD
     received by:
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
@@ -64,17 +65,31 @@
         "VMBGP4PIR-2",
         "VMBDMI",
         "VMBDMI-R",
         "VMBIN",
         "VMBKP",
         "VMBELPIR",
         "VMBDALI",
+        "VMB4AN",
+        "VMB6PB-20",
+        "VMBEL1-20",
+        "VMBEL2-20",
+        "VMBEL4-20",
+        "VMBELO-20",
+        "VMBGP1-20",
+        "VMBGP2-20",
+        "VMBGP4-20",
+        "VMBGPO-20",
+        "VMBDALI-20",
+        "VMBEL4PIR-20",
+        "VMBGP4PIR-20",
+        "VMB8DC-20",
     ],
 )
-class ChannelNamePart1Message2(ChannelNamePart1Message):
+class ChannelNamePart2Message2(ChannelNamePart2Message):
     """
     send by: VMBGP*, VMBDALI
     received by:
     """
 
     def populate(self, priority, address, rtr, data):
         """
@@ -85,15 +100,15 @@
         self.needs_data(data, 7)
         self.set_attributes(priority, address, rtr)
         self.channel = data[0]
         self.name = "".join([chr(x) for x in data[1:]])
 
 
 @register(COMMAND_CODE, ["VMB1BL", "VMB2BL"])
-class ChannelNamePart1Message3(ChannelNamePart1Message):
+class ChannelNamePart2Message3(ChannelNamePart2Message):
     """
     send by: VMBGP*
     received by:
     """
 
     def populate(self, priority, address, rtr, data):
         """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/channel_name_part2.py` & `velbus-aio-2024.4.0/velbusaio/messages/channel_name_part1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xF1
+COMMAND_CODE = 0xF0
 
 
 @register(COMMAND_CODE)
-class ChannelNamePart2Message(Message):
+class ChannelNamePart1Message(Message):
     """
     send by: VMB6IN, VMB4RYLD
     received by:
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
@@ -64,17 +65,32 @@
         "VMBGP4PIR-2",
         "VMBDMI",
         "VMBDMI-R",
         "VMBIN",
         "VMBKP",
         "VMBELPIR",
         "VMBDALI",
+        "VMB4AN",
+        "VMB6PB-20",
+        "VMBEL1-20",
+        "VMBEL2-20",
+        "VMBEL4-20",
+        "VMBELO-20",
+        "VMBGP1-20",
+        "VMBGP2-20",
+        "VMBGP4-20",
+        "VMBGPO-20",
+        "VMBDALI-20",
+        "VMBEL4PIR-20",
+        "VMBGP4PIR-20",
+        "VMB4LEDPWM-20",
+        "VMB8DC-20",
     ],
 )
-class ChannelNamePart2Message2(ChannelNamePart2Message):
+class ChannelNamePart1Message2(ChannelNamePart1Message):
     """
     send by: VMBGP*, VMBDALI
     received by:
     """
 
     def populate(self, priority, address, rtr, data):
         """
@@ -85,15 +101,15 @@
         self.needs_data(data, 7)
         self.set_attributes(priority, address, rtr)
         self.channel = data[0]
         self.name = "".join([chr(x) for x in data[1:]])
 
 
 @register(COMMAND_CODE, ["VMB1BL", "VMB2BL"])
-class ChannelNamePart2Message3(ChannelNamePart2Message):
+class ChannelNamePart1Message3(ChannelNamePart1Message):
     """
     send by: VMBGP*
     received by:
     """
 
     def populate(self, priority, address, rtr, data):
         """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/channel_name_part3.py` & `velbus-aio-2024.4.0/velbusaio/messages/channel_name_part3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xF2
 
@@ -64,14 +65,28 @@
         "VMBGP4PIR-2",
         "VMBDMI",
         "VMBDMI-R",
         "VMBIN",
         "VMBKP",
         "VMBELPIR",
         "VMBDALI",
+        "VMB4AN",
+        "VMB6PB-20",
+        "VMBEL1-20",
+        "VMBEL2-20",
+        "VMBEL4-20",
+        "VMBELO-20",
+        "VMBGP1-20",
+        "VMBGP2-20",
+        "VMBGP4-20",
+        "VMBGPO-20",
+        "VMBDALI-20",
+        "VMBEL4PIR-20",
+        "VMBGP4PIR-20",
+        "VMB8DC-20",
     ],
 )
 class ChannelNamePart3Message2(ChannelNamePart3Message):
     """
     send by: VMBGP*, VMBDALI
     received by:
     """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/channel_name_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/channel_name_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org> and Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xEF
 
@@ -66,15 +67,15 @@
         if 1 in self.channels:
             tmp += 0x03
         if 2 in self.channels:
             tmp += 0x0C
         return bytes([COMMAND_CODE, tmp])
 
 
-@register(COMMAND_CODE, ["VMBDALI"])
+@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20"])
 class ChannelNameRequestMessage3(ChannelNameRequestMessage):
     """
     send by:
     received by: VMBDALI
     """
 
     def populate(self, priority, address, rtr, data):
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/clear_led.py` & `velbus-aio-2024.4.0/velbusaio/messages/clear_led.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xF5
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/counter_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/counter_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xBE
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/counter_status_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/counter_status_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xBD
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/cover_down.py` & `velbus-aio-2024.4.0/velbusaio/messages/cover_down.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Tom Dupré <gitd8400@gmail.com>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/cover_off.py` & `velbus-aio-2024.4.0/velbusaio/messages/cover_off.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Tom Dupré <gitd8400@gmail.com>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/cover_position.py` & `velbus-aio-2024.4.0/velbusaio/messages/cover_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/cover_up.py` & `velbus-aio-2024.4.0/velbusaio/messages/cover_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Tom Dupré <gitd8400@gmail.com>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings.py` & `velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 :author: Niels Laukens
 """
+
 from __future__ import annotations
 
 import dataclasses
 import enum
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xE8
 
 
-@register(COMMAND_CODE, ["VMBDALI"])
+@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20"])
 class DaliDeviceSettingMsg(Message):
     """
     send by: VMBDALI
     received by:
     """
 
     def __init__(self, address: int | None = None):
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/dali_device_settings_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Niels Laukens
 """
+
 from __future__ import annotations
 
 import enum
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 from velbusaio.messages.dali_device_settings import DaliDeviceSetting
@@ -13,15 +14,15 @@
 
 
 class DataSource(enum.Enum):
     FromMemory = 0
     FromDaliDevice = 1
 
 
-@register(COMMAND_CODE, ["VMBDALI"])
+@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20"])
 class DaliDeviceSettingsRequest(Message):
     """
     send by:
     received by: VMBDALI
 
     Note: requesting a single setting for all (81) channels does not work (no response)
     """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/dali_dim_value_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/dali_dim_value_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 :author: Niels Laukens
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xA5
 
 
-@register(COMMAND_CODE, ["VMBDALI"])
+@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20"])
 class DimValueStatus(Message):
     """
     send by: VMBDALI
     received by:
     """
 
     def __init__(self, address: int = None) -> None:
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/dimmer_channel_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/dimmer_channel_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Frank van Breugel
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
@@ -17,15 +18,15 @@
 LED_OFF = 0
 LED_ON = 1 << 7
 LED_SLOW_BLINKING = 1 << 6
 LED_FAST_BLINKING = 1 << 5
 LED_VERY_FAST_BLINKING = 1 << 4
 
 
-@register(COMMAND_CODE, ["VMB4DC", "VMBDMI", "VMBDMI-R"])
+@register(COMMAND_CODE, ["VMB4DC", "VMBDMI", "VMBDMI-R", "VMB8DC-20"])
 class DimmerChannelStatusMessage(Message):
     """
     sent by: VMB4DC
     received by:
     """
 
     def __init__(self, address=None):
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/dimmer_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/dimmer_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Frank van Breugel
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
@@ -20,15 +21,15 @@
 LED_OFF = 0
 LED_ON = 1 << 7
 LED_SLOW_BLINKING = 1 << 6
 LED_FAST_BLINKING = 1 << 5
 LED_VERY_FAST_BLINKING = 1 << 4
 
 
-@register(COMMAND_CODE, ["VMBDME", "VMB1LED"])
+@register(COMMAND_CODE, ["VMB1DM", "VMBDME", "VMB1LED"])
 class DimmerStatusMessage(Message):
     """
     sent by: VMBDME
     received by:
     """
 
     def __init__(self, address=None):
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/edge_set_color.py` & `velbus-aio-2024.4.0/velbusaio/messages/edge_set_color.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/edge_set_custom_color.py` & `velbus-aio-2024.4.0/velbusaio/messages/edge_set_custom_color.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xD4
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/fast_blinking_led.py` & `velbus-aio-2024.4.0/velbusaio/messages/fast_blinking_led.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xF8
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/forced_off.py` & `velbus-aio-2024.4.0/velbusaio/messages/forced_off.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x12
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/forced_on.py` & `velbus-aio-2024.4.0/velbusaio/messages/forced_on.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x14
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/interface_status_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/interface_status_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x0E
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/kwh_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/kwh_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xBE
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/light_value_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/sensor_temp_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xAA
+COMMAND_CODE = 0xE5
 
 
 @register(COMMAND_CODE)
-class LightValueRequest(Message):
+class SensorTempRequest(Message):
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.set_attributes(priority, address, rtr)
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/memo_text.py` & `velbus-aio-2024.4.0/velbusaio/messages/memo_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xAC
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/memory_data.py` & `velbus-aio-2024.4.0/velbusaio/messages/memory_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xFE
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/memory_data_block.py` & `velbus-aio-2024.4.0/velbusaio/messages/memory_data_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xCC
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/memory_dump_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 """
-:author: Thomas Delaet <thomas@delaet.org>
+:author: Danny De Gaspari
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xCB
+COMMAND_CODE = 0xE9
 
 
 @register(COMMAND_CODE)
-class MemoryDumpRequestMessage(Message):
-    """
-    send by:
-    received by: VMB6IN, VMB4RYLD
-    """
-
+class TempSensorSettingsPart2(Message):
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_no_data(data)
         self.set_attributes(priority, address, rtr)
 
     def data_to_binary(self):
         """
         :return: bytes
         """
         return bytes([COMMAND_CODE])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/meteo_raw.py` & `velbus-aio-2024.4.0/velbusaio/messages/module_status_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """
-:author: Maikel Punie <maikel.punie@gmail.com>
+:author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xA9
+COMMAND_CODE = 0xFA
 
 
-@register(COMMAND_CODE, ["VMBMETEO"])
-class MeteoRawMessage(Message):
+@register(COMMAND_CODE)
+class ModuleStatusRequestMessage(Message):
     """
-    send by: VMBMETEO
-    received by:
+    send by:
+    received by: VMB6IN, VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.rain = 0
-        self.light = 0
-        self.wind = 0
+        self.channels = []
+        self.wait_after_send = 500
+        self.set_defaults(address)
 
     def populate(self, priority, address, rtr, data):
         """
-        data bytes (high + low)
-            1 + 2   = current temp
-            3 + 4   = min temp
-            5 + 6   = max temp
         :return: None
         """
+        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 6)
+        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self.rain = (((data[0] << 8) | data[1]) / 32) * 0.1
-        self.light = ((data[2] << 8) | data[3]) / 32
-        self.wind = (((data[4] << 8) | data[5]) / 32) * 0.1
+        self.channels = self.byte_to_channels(data[0])
+
+    def data_to_binary(self):
+        """
+        :return: bytes
+        """
+        return bytes([COMMAND_CODE, self.channels_to_byte(self.channels)])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/module_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/module_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xED
 
@@ -71,14 +72,25 @@
         "VMBEL4",
         "VMBGP4-2",
         "VMBGPO",
         "VMBGPOD",
         "VMBGPOD-2",
         "VMBELO",
         "VMB7IN",
+        "VMB6PB-20",
+        "VMBEL1-20",
+        "VMBEL2-20",
+        "VMBEL4-20",
+        "VMBELO-20",
+        "VMBGP1-20",
+        "VMBGP2-20",
+        "VMBGP4-20",
+        "VMBGPO-20",
+        "VMBEL4PIR-20",
+        "VMBGP4PIR-20",
     ],
 )
 class ModuleStatusMessage2(Message):
     def __init__(self, address=None):
         Message.__init__(self)
         self.closed = []
         self.enabled = []
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/module_status_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/very_fast_blinking_led.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xFA
+COMMAND_CODE = 0xF9
 
 
 @register(COMMAND_CODE)
-class ModuleStatusRequestMessage(Message):
+class VeryFastBlinkingLedMessage(Message):
     """
-    send by:
-    received by: VMB6IN, VMB4RYLD
+    send by: VMB4RYLD
+    received by: VMB6IN
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.channels = []
-        self.wait_after_send = 500
+        self.leds = []
         self.set_defaults(address)
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self.channels = self.byte_to_channels(data[0])
+        self.leds = self.byte_to_channels(data[0])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.channels_to_byte(self.channels)])
+        return bytes([COMMAND_CODE, self.channels_to_byte(self.leds)])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/module_subtype.py` & `velbus-aio-2024.4.0/velbusaio/messages/module_subtype.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/module_type.py` & `velbus-aio-2024.4.0/velbusaio/messages/write_module_address_and_serial_number.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,60 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xFF
-MODULES_WITHOUT_SERIAL = {
-    0x01: "VMB8PB",
-    0x02: "VMB1RY",
-    0x03: "VMB1BL",
-    0x05: "VMB6IN",
-    0x07: "VMB1DM",
-    0x08: "VMB4RY",
-    0x09: "VMB2BL",
-    0x0C: "VMB1TS",
-    0x0D: "VMB1TH",
-    0x0E: "VMB1TC",
-    0x0F: "VMB1LED",
-    0x14: "VMBDME",
-}
+COMMAND_CODE = 0x6A
 
 
 @register(COMMAND_CODE)
-class ModuleTypeMessage(Message):
+class WriteModuleAddressAndSerialNumberMessage(Message):
     """
-    send by: VMB6IN, VMB4RYLD
-    received by:
+    send by:
+    received by: VMB4RYLD
     """
 
-    # pylint: disable-msg=R0902
-
     def __init__(self, address=None):
         Message.__init__(self)
         self.module_type = 0x00
-        self.led_on = []
-        self.led_slow_blinking = []
-        self.led_fast_blinking = []
-        self.serial = 0
-        self.memory_map_version = 0
-        self.build_year = 0
-        self.build_week = 0
+        self.current_serial = 0
+        self.module_address = 0x00
+        self.new_serial = 0
         self.set_defaults(address)
 
-    def module_name(self):
-        """
-        :return: str
-        """
-        return "Unknown"
+    def set_defaults(self, address):
+        if address is not None:
+            self.set_address(address)
+        self.set_firmware_priority()
+        self.set_no_rtr()
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_low_priority(priority)
+        self.needs_firmware_priority(priority)
         self.needs_no_rtr(rtr)
+        self.needs_data(data, 6)
         self.set_attributes(priority, address, rtr)
         self.module_type = data[0]
-        if data[0] not in MODULES_WITHOUT_SERIAL:
-            (self.serial,) = struct.unpack(">L", bytes([0, 0, data[1], data[2]]))
-            self.memory_map_version = data[3]
-        self.build_year = data[-2]
-        self.build_week = data[-1]
+        prefix = bytes([0, 0])
+        (self.current_serial,) = struct.unpack(">L", prefix + data[1] + data[2])
+        self.module_address = data[3]
+        (self.new_serial,) = struct.unpack(">L", prefix + data[4] + data[5])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes(
-            [
-                COMMAND_CODE,
-                self.module_type,
-                self.channels_to_byte(self.led_on),
-                self.channels_to_byte(self.led_slow_blinking),
-                self.channels_to_byte(self.led_fast_blinking),
-                self.build_year,
-                self.build_week,
-            ]
+        return (
+            chr(COMMAND_CODE)
+            + chr(self.module_type)
+            + struct.pack(">L", self.current_serial)[2:]
+            + chr(self.module_address)
+            + struct.pack(">L", self.new_serial)[2:]
         )
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/module_type_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/module_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.message import Message
 
 
 class ModuleTypeRequestMessage(Message):
     """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/push_button_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/push_button_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x00
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/read_data_block_from_memory.py` & `velbus-aio-2024.4.0/velbusaio/messages/read_data_block_from_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xC9
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/read_data_from_memory.py` & `velbus-aio-2024.4.0/velbusaio/messages/read_data_from_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xFD
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/realtime_clock_status_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/realtime_clock_status_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xD7
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/receive_buffer_full.py` & `velbus-aio-2024.4.0/velbusaio/messages/receive_buffer_full.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x0B
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/receive_ready.py` & `velbus-aio-2024.4.0/velbusaio/messages/receive_ready.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x0C
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/relay_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/relay_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/restore_dimmer.py` & `velbus-aio-2024.4.0/velbusaio/messages/set_dimmer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 """
 :author: Frank van Breugel
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x11
+COMMAND_CODE = 0x07
 
 
-@register(COMMAND_CODE)
-class RestoreDimmerMessage(Message):
+@register(
+    COMMAND_CODE,
+    ["VMB1DM", "VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED", "VMB8DC-20"],
+)
+class SetDimmerMessage(Message):
     """
     send by:
     received by: VMBDME, VMB4DC
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.dimmer_channels = []
+        self.dimmer_state = 0
+        self.dimmer_transitiontime = 0
         self.set_defaults(address)
 
     def set_defaults(self, address):
         if address is not None:
             self.set_address(address)
         self.set_high_priority()
         self.set_no_rtr()
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
+        self.needs_data(data, 4)
         self.set_attributes(priority, address, rtr)
         self.dimmer_channels = self.byte_to_channels(data[0])
+        self.dimmer_state = data[1]
         self.dimmer_transitiontime = int.from_bytes(
             data[2:3], byteorder="big", signed=False
         )
 
     def data_to_binary(self):
         """
         :return: bytes
         """
         return bytes(
             [
                 COMMAND_CODE,
                 self.channels_to_byte(self.dimmer_channels),
-                0,
+                self.dimmer_state,
             ]
         ) + self.dimmer_transitiontime.to_bytes(2, byteorder="big", signed=False)
 
 
-@register(COMMAND_CODE, ["VMBDALI"])
-class RestoreDimmerMessage2(RestoreDimmerMessage):
+@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20"])
+class SetDimmerMessage2(SetDimmerMessage):
+    """
+    send by:
+    received by: VMBDALI
+    """
+
     def byte_to_channels(self, byte: int) -> list[int]:
         return [byte]
 
-    def channels_to_byte(self, channels: list[int]) -> int:
+    def channels_to_byte(self, channels) -> int:
         if len(channels) != 1:
             raise ValueError("We should have exact one channel")
         return channels[0]
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/select_program.py` & `velbus-aio-2024.4.0/velbusaio/messages/select_program.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Danny De Gaspari
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xB3
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/sensor_settings_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/sensor_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xE7
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/sensor_temp_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
-:author: Maikel Punie <maikel.punie@gmail.com>
+:author: Danny De Gaspari
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xE5
+COMMAND_CODE = 0xC6
 
 
 @register(COMMAND_CODE)
-class SensorTempRequest(Message):
+class TempSensorSettingsPart3(Message):
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.set_attributes(priority, address, rtr)
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/sensor_temperature.py` & `velbus-aio-2024.4.0/velbusaio/messages/sensor_temperature.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xE6
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/set_date.py` & `velbus-aio-2024.4.0/velbusaio/messages/set_date.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 import time
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
@@ -13,44 +14,44 @@
 
 @register(COMMAND_CODE)
 class SetDate(Message):
     """
     received by all modules
     """
 
-    def __init__(self, address=0x00):
+    def __init__(self, address=0x00) -> None:
         Message.__init__(self)
         self._day = None
         self._mon = None
         self._year = None
         self.set_defaults(address)
 
-    def set_defaults(self, address):
+    def set_defaults(self, address) -> None:
         if address is not None:
             self.set_address(address)
         self.set_low_priority()
         self.set_no_rtr()
         lclt = time.localtime()
         self._day = lclt[2]
         self._mon = lclt[1]
         self._year = lclt[0]
 
-    def populate(self, priority, address, rtr, data):
+    def populate(self, priority, address, rtr, data) -> None:
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.needs_data(data, 4)
         self.set_attributes(priority, address, rtr)
         self._day = data[0]
         self._mon = data[1]
         self._year = (data[2] << 8) + data[3]
 
-    def data_to_binary(self):
+    def data_to_binary(self) -> bytes:
         """
         :return: bytes
         """
         return bytes(
             [
                 COMMAND_CODE,
                 self._day,
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/set_daylight_saving.py` & `velbus-aio-2024.4.0/velbusaio/messages/start_relay_timer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """
-:author: Maikel Punie <maikel.punie@gmail.com>
+:author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
-import time
+import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xAF
+COMMAND_CODE = 0x03
 
 
 @register(COMMAND_CODE)
-class SetDaylightSaving(Message):
+class StartRelayTimerMessage(Message):
     """
-    received by all modules
+    send by:
+    received by: VMB4RYLD
     """
 
-    def __init__(self, address=0x00):
+    def __init__(self, address=None):
         Message.__init__(self)
-        self._ds = None
+        self.relay_channels = []
+        self.delay_time = 0
         self.set_defaults(address)
 
     def set_defaults(self, address):
         if address is not None:
             self.set_address(address)
-        self.set_low_priority()
+        self.set_high_priority()
         self.set_no_rtr()
-        lclt = time.localtime()
-        self._ds = not lclt[8]
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_low_priority(priority)
+        self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
+        self.needs_data(data, 4)
         self.set_attributes(priority, address, rtr)
-        self._ds = data[0]
+        self.relay_channels = self.byte_to_channels(data)
+        (self.delay_time,) = struct.unpack(">L", bytes([0]) + data[1:])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self._ds])
+        return (
+            bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
+            + struct.pack(">L", self.delay_time)[-3:]
+        )
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/set_dimmer.py` & `velbus-aio-2024.4.0/velbusaio/messages/raw.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 """
-:author: Frank van Breugel
+:author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x07
+COMMAND_CODE = 0xA9
 
 
-@register(COMMAND_CODE, ["VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED"])
-class SetDimmerMessage(Message):
+@register(COMMAND_CODE, ["VMBMETEO"])
+class MeteoRawMessage(Message):
     """
-    send by:
-    received by: VMBDME, VMB4DC
+    send by: VMBMETEO
+    received by:
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.dimmer_channels = []
-        self.dimmer_state = 0
-        self.dimmer_transitiontime = 0
-        self.set_defaults(address)
-
-    def set_defaults(self, address):
-        if address is not None:
-            self.set_address(address)
-        self.set_high_priority()
-        self.set_no_rtr()
+        self.rain = 0
+        self.light = 0
+        self.wind = 0
 
     def populate(self, priority, address, rtr, data):
         """
+        data bytes (high + low)
+            1 + 2   = current temp
+            3 + 4   = min temp
+            5 + 6   = max temp
         :return: None
         """
-        self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 4)
+        self.needs_data(data, 6)
         self.set_attributes(priority, address, rtr)
-        self.dimmer_channels = self.byte_to_channels(data[0])
-        self.dimmer_state = data[1]
-        self.dimmer_transitiontime = int.from_bytes(
-            data[2:3], byteorder="big", signed=False
-        )
+        self.rain = (((data[0] << 8) | data[1]) / 32) * 0.1
+        self.light = ((data[2] << 8) | data[3]) / 32
+        self.wind = (((data[4] << 8) | data[5]) / 32) * 0.1
 
-    def data_to_binary(self):
-        """
-        :return: bytes
-        """
-        return bytes(
-            [
-                COMMAND_CODE,
-                self.channels_to_byte(self.dimmer_channels),
-                self.dimmer_state,
-            ]
-        ) + self.dimmer_transitiontime.to_bytes(2, byteorder="big", signed=False)
 
-
-@register(COMMAND_CODE, ["VMBDALI"])
-class SetDimmerMessage2(SetDimmerMessage):
+@register(COMMAND_CODE, ["VMB4AN"])
+class SensorRawMessage(Message):
     """
-    send by:
-    received by: VMBDALI
+    send by: VMB4AN
+    received by:
     """
 
-    def byte_to_channels(self, byte: int) -> list[int]:
-        return [byte]
+    def __init__(self, address=None):
+        Message.__init__(self)
+        self.sensor = 0
+        self.mode = 0
+        self.value = 0
+        self.unit = None
 
-    def channels_to_byte(self, channels) -> int:
-        if len(channels) != 1:
-            raise ValueError("We should have exact one channel")
-        return channels[0]
+    def populate(self, priority, address, rtr, data):
+        self.needs_no_rtr(rtr)
+        self.needs_data(data, 5)
+        self.set_attributes(priority, address, rtr)
+        self.sensor = data[0]
+        self.mode = data[1]
+        self.value = (data[2] << 16) | (data[3] << 8) | data[4]
+        if self.mode == 0:
+            self.value = self.value * 0.25
+            self.unit = "mV"
+        elif self.mode == 1:
+            self.value = self.value * 5
+            self.unit = "µA"
+        elif self.mode == 2:
+            self.value = self.value * 0.25
+            self.unit = "ohm"
+        elif self.mode == 3:
+            self.value = self.value * 0.5
+            self.unit = "µS"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/set_led.py` & `velbus-aio-2024.4.0/velbusaio/messages/slow_blinking_led.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xF6
+COMMAND_CODE = 0xF7
 
 
 @register(COMMAND_CODE)
-class SetLedMessage(Message):
+class SlowBlinkingLedMessage(Message):
     """
     send by: VMB4RYLD
     received by: VMB6IN
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/set_realtime_clock.py` & `velbus-aio-2024.4.0/velbusaio/messages/set_realtime_clock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 import time
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
@@ -13,41 +14,41 @@
 
 @register(COMMAND_CODE)
 class SetRealtimeClock(Message):
     """
     received by all modules
     """
 
-    def __init__(self, address=0x00):
+    def __init__(self, address=0x00) -> None:
         Message.__init__(self)
         self._wday = None
         self._hour = None
         self._min = None
         self.set_defaults(address)
 
-    def set_defaults(self, address):
+    def set_defaults(self, address) -> None:
         if address is not None:
             self.set_address(address)
         self.set_low_priority()
         self.set_no_rtr()
         lclt = time.localtime()
         self._wday = lclt[6]
         self._hour = lclt[3]
         self._min = lclt[4]
 
-    def populate(self, priority, address, rtr, data):
+    def populate(self, priority, address, rtr, data) -> None:
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.needs_data(data, 3)
         self.set_attributes(priority, address, rtr)
         self._wday = data[0]
         self._hour = data[1]
         self._min = data[2]
 
-    def data_to_binary(self):
+    def data_to_binary(self) -> bytes:
         """
         :return: bytes
         """
         return bytes([COMMAND_CODE, self._wday, self._hour, self._min])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/set_temperature.py` & `velbus-aio-2024.4.0/velbusaio/messages/set_temperature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xE4
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/slider_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/slider_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 :author: Frank van Breugel
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x0F
 
 
-@register(COMMAND_CODE, ["VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED"])
+@register(
+    COMMAND_CODE,
+    ["VMB1DM", "VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED", "VMB8DC-20"],
+)
 class SliderStatusMessage(Message):
     """
     sent by: VMBDME
     received by:
     """
 
     def __init__(self, address=None):
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/slow_blinking_led.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_set_cooling.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xF7
+COMMAND_CODE = 0xDF
 
 
 @register(COMMAND_CODE)
-class SlowBlinkingLedMessage(Message):
+class TempSetCoolingMessage(Message):
     """
-    send by: VMB4RYLD
-    received by: VMB6IN
+    send by:
+    received by: VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.leds = []
         self.set_defaults(address)
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self.leds = self.byte_to_channels(data[0])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.channels_to_byte(self.leds)])
+        return bytes([COMMAND_CODE, 0xAA])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/start_relay_blinking_timer.py` & `velbus-aio-2024.4.0/velbusaio/messages/start_relay_blinking_timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 import struct
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/start_relay_timer.py` & `velbus-aio-2024.4.0/velbusaio/messages/switch_relay_on.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
-from __future__ import annotations
 
-import struct
+from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x03
+COMMAND_CODE = 0x02
 
 
 @register(COMMAND_CODE)
-class StartRelayTimerMessage(Message):
+class SwitchRelayOnMessage(Message):
     """
     send by:
     received by: VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.relay_channels = []
-        self.delay_time = 0
         self.set_defaults(address)
 
     def set_defaults(self, address):
         if address is not None:
             self.set_address(address)
         self.set_high_priority()
         self.set_no_rtr()
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 4)
+        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self.relay_channels = self.byte_to_channels(data)
-        (self.delay_time,) = struct.unpack(">L", bytes([0]) + data[1:])
+        self.relay_channels = self.byte_to_channels(data[0])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return (
-            bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
-            + struct.pack(">L", self.delay_time)[-3:]
-        )
+        return bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/switch_relay_off.py` & `velbus-aio-2024.4.0/velbusaio/messages/switch_relay_off.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x01
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/switch_relay_on.py` & `velbus-aio-2024.4.0/velbusaio/messages/switch_to_safe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x02
+COMMAND_CODE = 0xDE
 
 
 @register(COMMAND_CODE)
-class SwitchRelayOnMessage(Message):
+class SwitchToSafeMessage(Message):
     """
     send by:
     received by: VMB4RYLD
     """
 
-    def __init__(self, address=None):
+    def __init__(self, address=None, sleep=0):
         Message.__init__(self)
-        self.relay_channels = []
+        self.sleep = sleep
         self.set_defaults(address)
 
-    def set_defaults(self, address):
-        if address is not None:
-            self.set_address(address)
-        self.set_high_priority()
-        self.set_no_rtr()
-
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
-        self.relay_channels = self.byte_to_channels(data[0])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.channels_to_byte(self.relay_channels)])
+        return bytes([COMMAND_CODE, self.sleep >> 8, self.sleep & 0xFF])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/switch_to_comfort.py` & `velbus-aio-2024.4.0/velbusaio/messages/switch_to_comfort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xDB
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/switch_to_day.py` & `velbus-aio-2024.4.0/velbusaio/messages/switch_to_day.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xDC
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/switch_to_night.py` & `velbus-aio-2024.4.0/velbusaio/messages/switch_to_night.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xDD
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/switch_to_safe.py` & `velbus-aio-2024.4.0/velbusaio/messages/memory_dump_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xDE
+COMMAND_CODE = 0xCB
 
 
 @register(COMMAND_CODE)
-class SwitchToSafeMessage(Message):
+class MemoryDumpRequestMessage(Message):
     """
     send by:
-    received by: VMB4RYLD
+    received by: VMB6IN, VMB4RYLD
     """
 
-    def __init__(self, address=None, sleep=0):
-        Message.__init__(self)
-        self.sleep = sleep
-        self.set_defaults(address)
-
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
+        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
+        self.needs_no_data(data)
         self.set_attributes(priority, address, rtr)
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.sleep >> 8, self.sleep & 0xFF])
+        return bytes([COMMAND_CODE])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part1.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
-:author: Maikel Punie <maikel.punie@gmail.com>
+:author: Danny De Gaspari
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xE8
+COMMAND_CODE = 0xB9
 
 
 @register(COMMAND_CODE)
-class TempSensorSettingsPart1(Message):
+class TempSensorSettingsPart4(Message):
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.set_attributes(priority, address, rtr)
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part2.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_part1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
-:author: Danny De Gaspari
+:author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xE9
+COMMAND_CODE = 0xE8
 
 
 @register(COMMAND_CODE)
-class TempSensorSettingsPart2(Message):
+class TempSensorSettingsPart1(Message):
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.set_attributes(priority, address, rtr)
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part3.py` & `velbus-aio-2024.4.0/velbusaio/messages/set_led.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 """
-:author: Danny De Gaspari
+:author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xC6
+COMMAND_CODE = 0xF6
 
 
 @register(COMMAND_CODE)
-class TempSensorSettingsPart3(Message):
+class SetLedMessage(Message):
+    """
+    send by: VMB4RYLD
+    received by: VMB6IN
+    """
+
+    def __init__(self, address=None):
+        Message.__init__(self)
+        self.leds = []
+        self.set_defaults(address)
+
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
+        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
+        self.leds = self.byte_to_channels(data[0])
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE])
+        return bytes([COMMAND_CODE, self.channels_to_byte(self.leds)])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part4.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_set_heating.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 """
-:author: Danny De Gaspari
+:author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xB9
+COMMAND_CODE = 0xE0
 
 
 @register(COMMAND_CODE)
-class TempSensorSettingsPart4(Message):
+class TempSetHeatingMessage(Message):
+    """
+    send by:
+    received by: VMB4RYLD
+    """
+
+    def __init__(self, address=None):
+        Message.__init__(self)
+        self.set_defaults(address)
+
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
-        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
         self.set_attributes(priority, address, rtr)
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE])
+        return bytes([COMMAND_CODE, 0xAA])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_request.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xE7
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/temp_sensor_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 import json
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_set_cooling.py` & `velbus-aio-2024.4.0/velbusaio/messages/write_data_to_memory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xDF
+COMMAND_CODE = 0xFC
 
 
 @register(COMMAND_CODE)
-class TempSetCoolingMessage(Message):
+class WriteDataToMemoryMessage(Message):
     """
     send by:
-    received by: VMB4RYLD
+    received by: VMB6IN, VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
+        self.high_address = 0x00
+        self.low_address = 0x00
+        self.data = ""
         self.set_defaults(address)
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
+        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
+        self.needs_data(data, 3)
         self.set_attributes(priority, address, rtr)
+        self.high_address = data[0]
+        self.low_address = data[1]
+        self.data = data[2]
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, 0xAA])
+        return bytes([COMMAND_CODE, self.high_address, self.low_address, self.data])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/temp_set_heating.py` & `velbus-aio-2024.4.0/velbusaio/messages/set_daylight_saving.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 """
-:author: Thomas Delaet <thomas@delaet.org>
+:author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
+import time
+
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xE0
+COMMAND_CODE = 0xAF
 
 
 @register(COMMAND_CODE)
-class TempSetHeatingMessage(Message):
+class SetDaylightSaving(Message):
     """
-    send by:
-    received by: VMB4RYLD
+    received by all modules
     """
 
-    def __init__(self, address=None):
+    def __init__(self, address=0x00) -> None:
         Message.__init__(self)
+        self._ds = None
         self.set_defaults(address)
 
-    def populate(self, priority, address, rtr, data):
+    def set_defaults(self, address) -> None:
+        if address is not None:
+            self.set_address(address)
+        self.set_low_priority()
+        self.set_no_rtr()
+        lclt = time.localtime()
+        self._ds = not lclt[8]
+
+    def populate(self, priority, address, rtr, data) -> None:
         """
         :return: None
         """
+        self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
+        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
+        self._ds = data[0]
 
-    def data_to_binary(self):
+    def data_to_binary(self) -> bytes:
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, 0xAA])
+        return bytes([COMMAND_CODE, self._ds])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/update_led_status.py` & `velbus-aio-2024.4.0/velbusaio/messages/update_led_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xF4
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/very_fast_blinking_led.py` & `velbus-aio-2024.4.0/velbusaio/messages/write_memory_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """
 :author: Thomas Delaet <thomas@delaet.org>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xF9
+COMMAND_CODE = 0xCA
 
 
 @register(COMMAND_CODE)
-class VeryFastBlinkingLedMessage(Message):
+class WriteMemoryBlockMessage(Message):
     """
-    send by: VMB4RYLD
-    received by: VMB6IN
+    send by:
+    received by: VMB4RYLD
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
-        self.leds = []
+        self.high_address = 0x00
+        self.low_address = 0x00
+        self.data = ""
         self.set_defaults(address)
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
+        self.needs_data(data, 6)
         self.set_attributes(priority, address, rtr)
-        self.leds = self.byte_to_channels(data[0])
+        self.high_address = data[0]
+        self.low_address = data[1]
+        self.data = data[2:]
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.channels_to_byte(self.leds)])
+        return bytes([COMMAND_CODE, self.high_address, self.low_address] + self.data)
```

### Comparing `velbus-aio-2023.5.0/velbusaio/messages/write_memory_block.py` & `velbus-aio-2024.4.0/velbusaio/messages/light_value_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 """
-:author: Thomas Delaet <thomas@delaet.org>
+:author: Maikel Punie <maikel.punie@gmail.com>
 """
+
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0xCA
+COMMAND_CODE = 0xAA
 
 
 @register(COMMAND_CODE)
-class WriteMemoryBlockMessage(Message):
-    """
-    send by:
-    received by: VMB4RYLD
-    """
-
-    def __init__(self, address=None):
-        Message.__init__(self)
-        self.high_address = 0x00
-        self.low_address = 0x00
-        self.data = ""
-        self.set_defaults(address)
-
+class LightValueRequest(Message):
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_low_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 6)
         self.set_attributes(priority, address, rtr)
-        self.high_address = data[0]
-        self.low_address = data[1]
-        self.data = data[2:]
 
     def data_to_binary(self):
         """
         :return: bytes
         """
-        return bytes([COMMAND_CODE, self.high_address, self.low_address] + self.data)
+        return bytes([COMMAND_CODE])
```

### Comparing `velbus-aio-2023.5.0/velbusaio/module.py` & `velbus-aio-2024.4.0/velbusaio/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This represents a velbus module
 """
+
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
 import pickle
 import struct
@@ -68,33 +69,34 @@
 )
 from velbusaio.messages.dali_device_settings_request import DaliDeviceSettingsRequest
 from velbusaio.messages.dali_dim_value_status import DimValueStatus
 from velbusaio.messages.dimmer_channel_status import DimmerChannelStatusMessage
 from velbusaio.messages.dimmer_status import DimmerStatusMessage
 from velbusaio.messages.fast_blinking_led import FastBlinkingLedMessage
 from velbusaio.messages.memory_data import MemoryDataMessage
-from velbusaio.messages.meteo_raw import MeteoRawMessage
+from velbusaio.messages.raw import MeteoRawMessage, SensorRawMessage
 from velbusaio.messages.module_status import (
     ModuleStatusGP4PirMessage,
     ModuleStatusMessage,
     ModuleStatusMessage2,
     ModuleStatusPirMessage,
 )
 from velbusaio.messages.module_status_request import ModuleStatusRequestMessage
 from velbusaio.messages.module_subtype import ModuleSubTypeMessage
-from velbusaio.messages.module_type import ModuleTypeMessage
+from velbusaio.messages.module_type import ModuleTypeMessage, ModuleType2Message
 from velbusaio.messages.push_button_status import PushButtonStatusMessage
 from velbusaio.messages.read_data_from_memory import ReadDataFromMemoryMessage
 from velbusaio.messages.relay_status import RelayStatusMessage, RelayStatusMessage2
 from velbusaio.messages.sensor_temperature import SensorTemperatureMessage
 from velbusaio.messages.set_led import SetLedMessage
 from velbusaio.messages.slider_status import SliderStatusMessage
 from velbusaio.messages.slow_blinking_led import SlowBlinkingLedMessage
 from velbusaio.messages.temp_sensor_status import TempSensorStatusMessage
 from velbusaio.messages.update_led_status import UpdateLedStatusMessage
+from velbusaio.channels import Temperature as TemperatureChannelType
 
 
 class Module:
     """
     Abstract class for Velbus hardware modules.
     """
 
@@ -106,15 +108,15 @@
         module_data: dict,
         serial: int | None = None,
         memorymap: int | None = None,
         build_year: int | None = None,
         build_week: int | None = None,
         cache_dir: str | None = None,
     ) -> Module:
-        if module_type == 0x45:
+        if module_type == 0x45 or module_type == 0x5A:
             return VmbDali(
                 module_address,
                 module_type,
                 module_data,
                 serial,
                 memorymap,
                 build_year,
@@ -171,20 +173,22 @@
         # The last subaddress contain typically the temperature channels, has more then 8 channels
         # and doesn't start on a boundary of 8.
         # E.g. The VMBGP4 has one subaddress, so since the second subaddress is not defined,
         # this function will delete channels 17-24 while 17 and 18 belong to the temperature channels.
         #
         # The solution would be that this functions knows were the temperature channels are located
         # and/or what the max number of subaddresses are for each module.
-        if self._sub_address == {}:
-            raise Exception("No subaddresses defined")
+        # if self._sub_address == {} and self.loaded:
+        #   raise Exception("No subaddresses defined")
         for sub in range(1, 4):
             if sub not in self._sub_address:
                 for i in range(((sub * 8) + 1), (((sub + 1) * 8) + 1)):
-                    if i in self._channels:
+                    if i in self._channels and not isinstance(
+                        self._channels[i], TemperatureChannelType
+                    ):
                         del self._channels[i]
 
     def _cache(self) -> None:
         cfile = pathlib.Path(f"{self._cache_dir}/{self._address}.p")
         with cfile.open("wb") as fl:
             pickle.dump(self, fl)
 
@@ -317,14 +321,15 @@
                 await self._update_channel(
                     chan,
                     {
                         "target": message.target_temp,
                         "cmode": message.mode_str,
                         "cstatus": message.status_str,
                         "sleep_timer": message.sleep_timer,
+                        "cool_mode": message.cool_mode,
                     },
                 )
                 await self._channels[chan].maybe_update_temperature(
                     message.current_temp, 1 / 2
                 )
             # update the thermostat channels
             channel_name_to_msg_prop_map = {
@@ -441,15 +446,15 @@
                 CHANNEL_LIGHT_VALUE, {"cur": message.light_value}
             )
             for channel_id in range(1, 9):
                 channel = self._translate_channel_name(channel_id + _channel_offset)
                 await self._update_channel(
                     channel, {"closed": channel_id in message.closed}
                 )
-                if type(self._channels[channel]) == Button:
+                if type(self._channels[channel]) is Button:
                     # only treat 'enabled' if the channel is a Button
                     await self._update_channel(
                         channel, {"enabled": channel_id in message.enabled}
                     )
             # self.selected_program_str = message.selected_program_str
             await self._update_channel(
                 CHANNEL_SELECTED_PROGRAM,
@@ -503,15 +508,19 @@
             )
         elif isinstance(message, BlindStatusMessage):
             channel = self._translate_channel_name(message.channel)
             await self._update_channel(channel, {"state": message.status})
         elif isinstance(message, MeteoRawMessage):
             await self._update_channel(11, {"cur": message.rain})
             await self._update_channel(12, {"cur": message.light})
-            await self._update_channel(23, {"cur": message.wind})
+            await self._update_channel(13, {"cur": message.wind})
+        elif isinstance(message, SensorRawMessage):
+            await self._update_channel(
+                message.sensor, {"cur": message.value, "unit": message.unit}
+            )
 
         self._cache()
 
     async def _update_channel(self, channel: int, updates: dict):
         try:
             await self._channels[channel].update(updates)
         except KeyError:
@@ -574,15 +583,19 @@
             return
         await self._channels[CHANNEL_MEMO_TEXT].set(txt)
 
     async def _process_memory_data_message(self, message: MemoryDataMessage) -> None:
         addr = "{high:02X}{low:02X}".format(
             high=message.high_address, low=message.low_address
         )
-        mdata = self._data["Memory"]["1"]["Address"][addr]
+        if "Memory" not in self._data:
+            return
+        if "Address" not in self._data["Memory"]:
+            return
+        mdata = self._data["Memory"]["Address"][addr]
         if "ModuleName" in mdata and isinstance(self._name, dict):
             # if self._name is a dict we are still loading
             # if its a string it was already complete
             char_and_save = mdata["ModuleName"].split(":")
             char = char_and_save[0]
             self._name[int(char)] = chr(message.data)
             if len(char_and_save) > 1 and char_and_save[1] == "Save":
@@ -690,17 +703,18 @@
             self._name = None
             return
 
         if self._type == 0x0C:
             self._name = None
             return
 
-        for _memory_key, memory_part in self._data["Memory"].items():
-            if "Address" in memory_part:
-                for addr_int in memory_part["Address"].keys():
+        for memory_key, memory_part in self._data["Memory"].items():
+
+            if memory_key == "Address":
+                for addr_int in memory_part.keys():
                     addr = struct.unpack(
                         ">BB", struct.pack(">h", int("0x" + addr_int, 0))
                     )
                     msg = ReadDataFromMemoryMessage(self._address)
                     msg.priority = PRIORITY_LOW
                     msg.high_address = addr[0]
                     msg.low_address = addr[1]
@@ -719,25 +733,14 @@
                 self, int(chan), chan_data["Name"], edit, self._writer, self._address
             )
             if chan_data["Type"] == "Temperature":
                 if "Thermostat" in self._data or (
                     "ThermostatAddr" in self._data and self._data["ThermostatAddr"] != 0
                 ):
                     await self._update_channel(int(chan), {"thermostat": True})
-        # add extra channel for program selection which is not in the channel list of the protocol.json file,
-        # but is available in the messages list of the corresponding module.
-        if keys_exists(self._data, "Messages", "B3"):
-            self._channels[CHANNEL_SELECTED_PROGRAM] = SelectedProgram(
-                self,
-                CHANNEL_SELECTED_PROGRAM,
-                "Selected Program",
-                False,
-                self._writer,
-                self._address,
-            )
 
 
 class VmbDali(Module):
     """
     DALI has a variable number of channels: the number of channels
     depends on the number of DALI devices on the DALI bus
     """
```

### Comparing `velbus-aio-2023.5.0/velbusaio/protocol.py` & `velbus-aio-2024.4.0/velbusaio/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             new_buffer[: len(remaining_data)] = remaining_data
 
         self._buffer = new_buffer
         self._buffer_pos = len(remaining_data) if remaining_data else 0
         self._buffer_view = memoryview(self._buffer)
 
     async def _process_message(self, msg: RawMessage) -> None:
-        self._log.debug(f"RX: {msg}")
+        # self._log.debug(f"RX: {msg}")
         await self._message_received_callback(msg)
 
     # Everything write-related
 
     async def write_auth_key(self, authkey: str) -> None:
         self._log.debug("TX: authentication key")
         if not self.transport.is_closing():
@@ -214,13 +214,13 @@
     @backoff.on_predicate(
         backoff.expo,
         lambda is_sent: not is_sent,
         max_tries=10,
         on_backoff=_on_write_backoff,
     )
     async def _write_message(self, msg: RawMessage) -> bool:
-        self._log.debug(f"TX: {msg}")
+        # self._log.debug(f"TX: {msg}")
         if not self.transport.is_closing():
             self.transport.write(msg.to_bytes())
             return True
         else:
             return False
```

### Comparing `velbus-aio-2023.5.0/velbusaio/raw_message.py` & `velbus-aio-2024.4.0/velbusaio/raw_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,20 +126,20 @@
     Remove leading garbage bytes from a byte stream.
     """
 
     # A proper message byte stream begins with 0x0F.
     if rawmessage and rawmessage[0] != START_BYTE:
         start_index = rawmessage.find(START_BYTE)
         if start_index > -1:
-            logging.debug(
-                "Trimming leading garbage from buffer content: {buffer} becomes {new_buffer}".format(
-                    buffer=binascii.hexlify(rawmessage),
-                    new_buffer=binascii.hexlify(rawmessage[start_index:]),
-                )
-            )
+            #           logging.debug(
+            #                "Trimming leading garbage from buffer content: {buffer} becomes {new_buffer}".format(
+            #                    buffer=binascii.hexlify(rawmessage),
+            #                    new_buffer=binascii.hexlify(rawmessage[start_index:]),
+            #                )
+            #            )
             return rawmessage[start_index:]
         else:
             logging.debug(
                 "Trimming whole buffer as it does not contain the start byte: {buffer}".format(
                     buffer=binascii.hexlify(rawmessage)
                 )
             )
```

### Comparing `velbus-aio-2023.5.0/velbusaio/util.py` & `velbus-aio-2024.4.0/velbusaio/util.py`

 * *Files identical despite different names*

