# Comparing `tmp/ubo_app-0.9.8a4.tar.gz` & `tmp/ubo_app-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubo_app-0.9.8a4.tar", max compression
+gzip compressed data, was "ubo_app-0.9.9.tar", max compression
```

## Comparing `ubo_app-0.9.8a4.tar` & `ubo_app-0.9.9.tar`

### file list

```diff
@@ -1,93 +1,96 @@
--rw-r--r--   0        0        0     2453 2024-02-04 17:16:07.105521 ubo_app-0.9.8a4/README.md
--rw-r--r--   0        0        0     2054 2024-02-05 08:37:13.277880 ubo_app-0.9.8a4/pyproject.toml
--rw-r--r--   0        0        0     2035 2024-02-05 06:15:58.932859 ubo_app-0.9.8a4/ubo_app/__init__.py
--rw-r--r--   0        0        0      716 2024-02-04 13:12:10.955673 ubo_app-0.9.8a4/ubo_app/constants.py
--rw-r--r--   0        0        0      463 2023-12-31 22:27:21.060771 ubo_app-0.9.8a4/ubo_app/home_page.kv
--rw-r--r--   0        0        0     7384 2024-02-04 13:12:10.956025 ubo_app-0.9.8a4/ubo_app/load_services.py
--rw-r--r--   0        0        0     2820 2024-02-04 13:12:10.956373 ubo_app-0.9.8a4/ubo_app/logging.py
--rw-r--r--   0        0        0      407 2024-01-21 22:07:20.690579 ubo_app-0.9.8a4/ubo_app/menu.py
--rw-r--r--   0        0        0     6038 2024-02-04 13:12:10.956684 ubo_app-0.9.8a4/ubo_app/menu_central.py
--rw-r--r--   0        0        0     6882 2024-01-22 06:10:12.342578 ubo_app-0.9.8a4/ubo_app/menu_footer.py
--rw-r--r--   0        0        0     3563 2024-02-04 13:12:10.956968 ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/reducer.py
--rw-r--r--   0        0        0     1922 2024-02-04 13:12:10.957238 ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/rgb_ring_client.py
--rw-r--r--   0        0        0      546 2024-01-22 04:08:50.895118 ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/setup.py
--rw-r--r--   0        0        0      273 2024-01-22 04:08:50.895417 ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/ubo_handle.py
--rw-r--r--   0        0        0     7427 2024-02-04 16:47:47.218610 ubo_app-0.9.8a4/ubo_app/services/000-sound/audio_manager.py
--rw-r--r--   0        0        0      135 2024-01-22 04:08:50.895922 ubo_app-0.9.8a4/ubo_app/services/000-sound/constants.py
--rw-r--r--   0        0        0     3741 2024-02-04 13:12:38.771594 ubo_app-0.9.8a4/ubo_app/services/000-sound/reducer.py
--rw-r--r--   0        0        0     1362 2024-01-23 02:47:45.412608 ubo_app-0.9.8a4/ubo_app/services/000-sound/setup.py
--rw-r--r--   0        0        0    25808 2024-01-18 12:01:59.451193 ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/add.wav
--rw-r--r--   0        0        0    42370 2024-01-18 12:01:16.751690 ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/done.wav
--rw-r--r--   0        0        0    48078 2024-01-18 12:01:26.086005 ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/failure.wav
--rw-r--r--   0        0        0   320078 2024-01-18 12:02:21.042828 ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/scan.wav
--rw-r--r--   0        0        0    10214 2024-01-19 01:21:35.228994 ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/volume.wav
--rw-r--r--   0        0        0      267 2024-01-22 04:08:50.896635 ubo_app-0.9.8a4/ubo_app/services/000-sound/ubo_handle.py
--rw-r--r--   0        0        0      132 2024-01-22 04:08:50.896914 ubo_app-0.9.8a4/ubo_app/services/010-ethernet/constants.py
--rw-r--r--   0        0        0     2789 2024-01-22 04:08:50.897171 ubo_app-0.9.8a4/ubo_app/services/010-ethernet/ethernet_manager.py
--rw-r--r--   0        0        0     1559 2024-01-22 04:08:50.897435 ubo_app-0.9.8a4/ubo_app/services/010-ethernet/setup.py
--rw-r--r--   0        0        0      216 2024-01-22 04:08:50.897810 ubo_app-0.9.8a4/ubo_app/services/010-ethernet/ubo_handle.py
--rw-r--r--   0        0        0      135 2024-01-22 04:08:50.898084 ubo_app-0.9.8a4/ubo_app/services/010-ip/constants.py
--rw-r--r--   0        0        0     1071 2024-01-22 04:08:50.898258 ubo_app-0.9.8a4/ubo_app/services/010-ip/reducer.py
--rw-r--r--   0        0        0     3552 2024-02-04 13:12:10.958097 ubo_app-0.9.8a4/ubo_app/services/010-ip/setup.py
--rw-r--r--   0        0        0      261 2024-01-22 04:08:50.898964 ubo_app-0.9.8a4/ubo_app/services/010-ip/ubo_handle.py
--rw-r--r--   0        0        0      387 2024-01-22 04:08:50.899169 ubo_app-0.9.8a4/ubo_app/services/010-wifi/constants.py
--rw-r--r--   0        0        0       49 2024-01-22 04:08:50.899527 ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/__init__.py
--rw-r--r--   0        0        0      829 2024-01-22 04:08:50.899839 ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/create_wireless_connection.kv
--rw-r--r--   0        0        0     3922 2024-02-04 13:12:10.958438 ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/create_wireless_connection.py
--rw-r--r--   0        0        0     5027 2024-02-01 18:21:41.895205 ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/main.py
--rw-r--r--   0        0        0     3538 2024-01-22 04:08:50.900613 ubo_app-0.9.8a4/ubo_app/services/010-wifi/reducer.py
--rw-r--r--   0        0        0     1645 2024-01-22 04:08:50.900861 ubo_app-0.9.8a4/ubo_app/services/010-wifi/setup.py
--rw-r--r--   0        0        0      265 2024-01-22 04:08:50.901097 ubo_app-0.9.8a4/ubo_app/services/010-wifi/ubo_handle.py
--rw-r--r--   0        0        0    12123 2024-01-22 22:31:06.119958 ubo_app-0.9.8a4/ubo_app/services/010-wifi/wifi_manager.py
--rw-r--r--   0        0        0     1586 2024-01-22 04:08:50.901739 ubo_app-0.9.8a4/ubo_app/services/020-keyboard/setup.py
--rw-r--r--   0        0        0      224 2024-01-22 04:08:50.901959 ubo_app-0.9.8a4/ubo_app/services/020-keyboard/ubo_handle.py
--rw-r--r--   0        0        0    12342 2024-01-22 04:08:50.902206 ubo_app-0.9.8a4/ubo_app/services/020-keypad/setup.py
--rw-r--r--   0        0        0      268 2024-01-22 04:08:50.902493 ubo_app-0.9.8a4/ubo_app/services/020-keypad/ubo_handle.py
--rw-r--r--   0        0        0     3401 2024-01-22 04:08:50.902701 ubo_app-0.9.8a4/ubo_app/services/030-notifications/reducer.py
--rw-r--r--   0        0        0      236 2024-01-22 04:08:50.903014 ubo_app-0.9.8a4/ubo_app/services/030-notifications/ubo_handle.py
--rw-r--r--   0        0        0     1757 2024-01-22 04:08:50.903190 ubo_app-0.9.8a4/ubo_app/services/040-camera/reducer.py
--rw-r--r--   0        0        0     4203 2024-02-04 13:12:10.958896 ubo_app-0.9.8a4/ubo_app/services/040-camera/setup.py
--rw-r--r--   0        0        0      317 2024-01-22 04:08:50.903640 ubo_app-0.9.8a4/ubo_app/services/040-camera/ubo_handle.py
--rw-r--r--   0        0        0      971 2024-01-22 05:18:43.546200 ubo_app-0.9.8a4/ubo_app/services/040-sensors/reducer.py
--rw-r--r--   0        0        0     1100 2024-01-22 06:07:43.147729 ubo_app-0.9.8a4/ubo_app/services/040-sensors/setup.py
--rw-r--r--   0        0        0      271 2024-01-22 05:07:02.749392 ubo_app-0.9.8a4/ubo_app/services/040-sensors/ubo_handle.py
--rw-r--r--   0        0        0     3145 2024-02-04 13:12:38.772009 ubo_app-0.9.8a4/ubo_app/services/080-docker/reducer.py
--rw-r--r--   0        0        0    18108 2024-02-04 13:12:38.772511 ubo_app-0.9.8a4/ubo_app/services/080-docker/setup.py
--rw-r--r--   0        0        0      424 2024-02-04 13:12:10.959447 ubo_app-0.9.8a4/ubo_app/services/080-docker/ubo_handle.py
--rw-r--r--   0        0        0     1987 2024-02-04 13:12:10.959651 ubo_app-0.9.8a4/ubo_app/side_effects.py
--rw-r--r--   0        0        0     2993 2024-02-04 13:12:10.960463 ubo_app-0.9.8a4/ubo_app/store/__init__.py
--rw-r--r--   0        0        0     1115 2024-02-04 13:12:10.960728 ubo_app-0.9.8a4/ubo_app/store/main/__init__.py
--rw-r--r--   0        0        0     4233 2024-02-04 13:12:10.961342 ubo_app-0.9.8a4/ubo_app/store/main/_menus.py
--rw-r--r--   0        0        0     4165 2024-02-04 13:12:10.961541 ubo_app-0.9.8a4/ubo_app/store/main/reducer.py
--rw-r--r--   0        0        0      655 2024-01-20 02:39:43.784109 ubo_app-0.9.8a4/ubo_app/store/services/camera.py
--rw-r--r--   0        0        0     2217 2024-02-04 13:12:10.961828 ubo_app-0.9.8a4/ubo_app/store/services/docker.py
--rw-r--r--   0        0        0      298 2024-01-20 02:39:43.784322 ubo_app-0.9.8a4/ubo_app/store/services/ethernet.py
--rw-r--r--   0        0        0      588 2024-01-20 02:39:43.784547 ubo_app-0.9.8a4/ubo_app/store/services/ip.py
--rw-r--r--   0        0        0      583 2024-01-20 02:39:43.784723 ubo_app-0.9.8a4/ubo_app/store/services/keypad.py
--rw-r--r--   0        0        0     2830 2024-01-21 21:40:07.987830 ubo_app-0.9.8a4/ubo_app/store/services/notifications.py
--rw-r--r--   0        0        0     2093 2024-02-04 13:12:10.962067 ubo_app-0.9.8a4/ubo_app/store/services/rgb_ring.py
--rw-r--r--   0        0        0      869 2024-01-22 05:17:55.559542 ubo_app-0.9.8a4/ubo_app/store/services/sensors.py
--rw-r--r--   0        0        0      902 2024-01-20 02:39:43.785360 ubo_app-0.9.8a4/ubo_app/store/services/sound.py
--rw-r--r--   0        0        0     1414 2024-01-20 02:39:43.785567 ubo_app-0.9.8a4/ubo_app/store/services/wifi.py
--rw-r--r--   0        0        0      508 2024-01-22 00:41:10.125509 ubo_app-0.9.8a4/ubo_app/store/status_icons/__init__.py
--rw-r--r--   0        0        0     1286 2024-01-22 00:42:02.945066 ubo_app-0.9.8a4/ubo_app/store/status_icons/reducer.py
--rw-r--r--   0        0        0     1059 2024-02-04 13:12:10.962278 ubo_app-0.9.8a4/ubo_app/store/update_manager/__init__.py
--rw-r--r--   0        0        0     3326 2024-02-04 15:03:26.551436 ubo_app-0.9.8a4/ubo_app/store/update_manager/reducer.py
--rw-r--r--   0        0        0     5461 2024-02-04 13:12:10.962665 ubo_app-0.9.8a4/ubo_app/store/update_manager/utils.py
--rw-r--r--   0        0        0        0 2024-02-04 13:12:10.962703 ubo_app-0.9.8a4/ubo_app/system/__init__.py
--rw-r--r--   0        0        0     5972 2024-02-05 08:32:29.171761 ubo_app-0.9.8a4/ubo_app/system/bootstrap.py
--rwxr-xr-x   0        0        0     2786 2024-02-05 08:37:17.399214 ubo_app-0.9.8a4/ubo_app/system/install.sh
--rwxr-xr-x   0        0        0     1001 2024-02-04 13:12:10.963703 ubo_app-0.9.8a4/ubo_app/system/install_docker.sh
--rwxr-xr-x   0        0        0     2004 2024-02-05 04:08:43.165059 ubo_app-0.9.8a4/ubo_app/system/install_wm8960.sh
--rw-r--r--   0        0        0      468 2024-02-04 16:16:26.634705 ubo_app-0.9.8a4/ubo_app/system/polkit-reboot.rules
--rw-r--r--   0        0        0      330 2024-02-04 16:04:24.021806 ubo_app-0.9.8a4/ubo_app/system/services/app.service
--rw-r--r--   0        0        0      554 2024-02-04 13:12:10.964300 ubo_app-0.9.8a4/ubo_app/system/services/system.service
--rw-r--r--   0        0        0      401 2024-01-23 04:19:54.162152 ubo_app-0.9.8a4/ubo_app/system/services/update.service
--rw-r--r--   0        0        0        0 2024-02-04 13:12:10.964383 ubo_app-0.9.8a4/ubo_app/system/system_manager/__init__.py
--rw-r--r--   0        0        0     4276 2024-02-05 07:04:32.715697 ubo_app-0.9.8a4/ubo_app/system/system_manager/__main__.py
--rw-r--r--   0        0        0    12010 2024-02-04 13:12:10.964821 ubo_app-0.9.8a4/ubo_app/system/system_manager/led.py
--rw-r--r--   0        0        0     1067 2024-01-22 23:33:10.911357 ubo_app-0.9.8a4/ubo_app/utils/__init__.py
--rw-r--r--   0        0        0     1521 2024-02-04 13:12:10.965089 ubo_app-0.9.8a4/ubo_app/utils/async_.py
--rw-r--r--   0        0        0     1297 2024-01-20 02:51:33.651928 ubo_app-0.9.8a4/ubo_app/utils/fake.py
--rw-r--r--   0        0        0     1674 2024-02-04 13:12:10.965407 ubo_app-0.9.8a4/ubo_app/utils/loop.py
--rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 ubo_app-0.9.8a4/PKG-INFO
+-rw-r--r--   0        0        0     2453 2024-02-04 17:16:07.105521 ubo_app-0.9.9/README.md
+-rw-r--r--   0        0        0     2069 2024-02-08 23:52:35.502134 ubo_app-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2891 2024-02-08 22:03:59.740683 ubo_app-0.9.9/ubo_app/__init__.py
+-rw-r--r--   0        0        0      716 2024-02-04 13:12:10.955673 ubo_app-0.9.9/ubo_app/constants.py
+-rw-r--r--   0        0        0      463 2023-12-31 22:27:21.060771 ubo_app-0.9.9/ubo_app/home_page.kv
+-rw-r--r--   0        0        0     7381 2024-02-06 22:52:40.250834 ubo_app-0.9.9/ubo_app/load_services.py
+-rw-r--r--   0        0        0     2820 2024-02-04 13:12:10.956373 ubo_app-0.9.9/ubo_app/logging.py
+-rw-r--r--   0        0        0      407 2024-01-21 22:07:20.690579 ubo_app-0.9.9/ubo_app/menu.py
+-rw-r--r--   0        0        0     6038 2024-02-04 13:12:10.956684 ubo_app-0.9.9/ubo_app/menu_central.py
+-rw-r--r--   0        0        0     6882 2024-01-22 06:10:12.342578 ubo_app-0.9.9/ubo_app/menu_footer.py
+-rw-r--r--   0        0        0     3563 2024-02-04 13:12:10.956968 ubo_app-0.9.9/ubo_app/services/000-rgb-ring/reducer.py
+-rw-r--r--   0        0        0     1922 2024-02-04 13:12:10.957238 ubo_app-0.9.9/ubo_app/services/000-rgb-ring/rgb_ring_client.py
+-rw-r--r--   0        0        0      546 2024-01-22 04:08:50.895118 ubo_app-0.9.9/ubo_app/services/000-rgb-ring/setup.py
+-rw-r--r--   0        0        0      273 2024-01-22 04:08:50.895417 ubo_app-0.9.9/ubo_app/services/000-rgb-ring/ubo_handle.py
+-rw-r--r--   0        0        0     7427 2024-02-04 16:47:47.218610 ubo_app-0.9.9/ubo_app/services/000-sound/audio_manager.py
+-rw-r--r--   0        0        0      135 2024-01-22 04:08:50.895922 ubo_app-0.9.9/ubo_app/services/000-sound/constants.py
+-rw-r--r--   0        0        0     3741 2024-02-04 13:12:38.771594 ubo_app-0.9.9/ubo_app/services/000-sound/reducer.py
+-rw-r--r--   0        0        0     1362 2024-01-23 02:47:45.412608 ubo_app-0.9.9/ubo_app/services/000-sound/setup.py
+-rw-r--r--   0        0        0    25808 2024-01-18 12:01:59.451193 ubo_app-0.9.9/ubo_app/services/000-sound/sounds/add.wav
+-rw-r--r--   0        0        0    42370 2024-01-18 12:01:16.751690 ubo_app-0.9.9/ubo_app/services/000-sound/sounds/done.wav
+-rw-r--r--   0        0        0    48078 2024-01-18 12:01:26.086005 ubo_app-0.9.9/ubo_app/services/000-sound/sounds/failure.wav
+-rw-r--r--   0        0        0   320078 2024-01-18 12:02:21.042828 ubo_app-0.9.9/ubo_app/services/000-sound/sounds/scan.wav
+-rw-r--r--   0        0        0    10214 2024-01-19 01:21:35.228994 ubo_app-0.9.9/ubo_app/services/000-sound/sounds/volume.wav
+-rw-r--r--   0        0        0      267 2024-01-22 04:08:50.896635 ubo_app-0.9.9/ubo_app/services/000-sound/ubo_handle.py
+-rw-r--r--   0        0        0      132 2024-01-22 04:08:50.896914 ubo_app-0.9.9/ubo_app/services/010-ethernet/constants.py
+-rw-r--r--   0        0        0     2789 2024-01-22 04:08:50.897171 ubo_app-0.9.9/ubo_app/services/010-ethernet/ethernet_manager.py
+-rw-r--r--   0        0        0     1559 2024-01-22 04:08:50.897435 ubo_app-0.9.9/ubo_app/services/010-ethernet/setup.py
+-rw-r--r--   0        0        0      216 2024-01-22 04:08:50.897810 ubo_app-0.9.9/ubo_app/services/010-ethernet/ubo_handle.py
+-rw-r--r--   0        0        0      135 2024-01-22 04:08:50.898084 ubo_app-0.9.9/ubo_app/services/010-ip/constants.py
+-rw-r--r--   0        0        0     1071 2024-01-22 04:08:50.898258 ubo_app-0.9.9/ubo_app/services/010-ip/reducer.py
+-rw-r--r--   0        0        0     3552 2024-02-04 13:12:10.958097 ubo_app-0.9.9/ubo_app/services/010-ip/setup.py
+-rw-r--r--   0        0        0      261 2024-01-22 04:08:50.898964 ubo_app-0.9.9/ubo_app/services/010-ip/ubo_handle.py
+-rw-r--r--   0        0        0      387 2024-01-22 04:08:50.899169 ubo_app-0.9.9/ubo_app/services/010-wifi/constants.py
+-rw-r--r--   0        0        0       49 2024-01-22 04:08:50.899527 ubo_app-0.9.9/ubo_app/services/010-wifi/pages/__init__.py
+-rw-r--r--   0        0        0      829 2024-01-22 04:08:50.899839 ubo_app-0.9.9/ubo_app/services/010-wifi/pages/create_wireless_connection.kv
+-rw-r--r--   0        0        0     3922 2024-02-04 13:12:10.958438 ubo_app-0.9.9/ubo_app/services/010-wifi/pages/create_wireless_connection.py
+-rw-r--r--   0        0        0     5027 2024-02-01 18:21:41.895205 ubo_app-0.9.9/ubo_app/services/010-wifi/pages/main.py
+-rw-r--r--   0        0        0     3538 2024-01-22 04:08:50.900613 ubo_app-0.9.9/ubo_app/services/010-wifi/reducer.py
+-rw-r--r--   0        0        0     1645 2024-01-22 04:08:50.900861 ubo_app-0.9.9/ubo_app/services/010-wifi/setup.py
+-rw-r--r--   0        0        0      265 2024-01-22 04:08:50.901097 ubo_app-0.9.9/ubo_app/services/010-wifi/ubo_handle.py
+-rw-r--r--   0        0        0    11822 2024-02-07 22:43:12.503115 ubo_app-0.9.9/ubo_app/services/010-wifi/wifi_manager.py
+-rw-r--r--   0        0        0     1586 2024-01-22 04:08:50.901739 ubo_app-0.9.9/ubo_app/services/020-keyboard/setup.py
+-rw-r--r--   0        0        0      224 2024-01-22 04:08:50.901959 ubo_app-0.9.9/ubo_app/services/020-keyboard/ubo_handle.py
+-rw-r--r--   0        0        0    12342 2024-01-22 04:08:50.902206 ubo_app-0.9.9/ubo_app/services/020-keypad/setup.py
+-rw-r--r--   0        0        0      268 2024-01-22 04:08:50.902493 ubo_app-0.9.9/ubo_app/services/020-keypad/ubo_handle.py
+-rw-r--r--   0        0        0     3401 2024-01-22 04:08:50.902701 ubo_app-0.9.9/ubo_app/services/030-notifications/reducer.py
+-rw-r--r--   0        0        0      236 2024-01-22 04:08:50.903014 ubo_app-0.9.9/ubo_app/services/030-notifications/ubo_handle.py
+-rw-r--r--   0        0        0     1757 2024-01-22 04:08:50.903190 ubo_app-0.9.9/ubo_app/services/040-camera/reducer.py
+-rw-r--r--   0        0        0     4203 2024-02-04 13:12:10.958896 ubo_app-0.9.9/ubo_app/services/040-camera/setup.py
+-rw-r--r--   0        0        0      317 2024-01-22 04:08:50.903640 ubo_app-0.9.9/ubo_app/services/040-camera/ubo_handle.py
+-rw-r--r--   0        0        0      971 2024-01-22 05:18:43.546200 ubo_app-0.9.9/ubo_app/services/040-sensors/reducer.py
+-rw-r--r--   0        0        0     1100 2024-01-22 06:07:43.147729 ubo_app-0.9.9/ubo_app/services/040-sensors/setup.py
+-rw-r--r--   0        0        0      271 2024-01-22 05:07:02.749392 ubo_app-0.9.9/ubo_app/services/040-sensors/ubo_handle.py
+-rw-r--r--   0        0        0    14482 2024-02-08 23:48:40.855125 ubo_app-0.9.9/ubo_app/services/080-docker/image.py
+-rw-r--r--   0        0        0     3461 2024-02-08 23:47:54.052178 ubo_app-0.9.9/ubo_app/services/080-docker/reducer.py
+-rw-r--r--   0        0        0     6857 2024-02-08 23:23:08.607613 ubo_app-0.9.9/ubo_app/services/080-docker/setup.py
+-rw-r--r--   0        0        0      269 2024-02-06 13:18:15.004207 ubo_app-0.9.9/ubo_app/services/080-docker/ubo_handle.py
+-rw-r--r--   0        0        0     1987 2024-02-04 13:12:10.959651 ubo_app-0.9.9/ubo_app/side_effects.py
+-rw-r--r--   0        0        0     2993 2024-02-04 13:12:10.960463 ubo_app-0.9.9/ubo_app/store/__init__.py
+-rw-r--r--   0        0        0     1115 2024-02-04 13:12:10.960728 ubo_app-0.9.9/ubo_app/store/main/__init__.py
+-rw-r--r--   0        0        0     4233 2024-02-04 13:12:10.961342 ubo_app-0.9.9/ubo_app/store/main/_menus.py
+-rw-r--r--   0        0        0     4165 2024-02-04 13:12:10.961541 ubo_app-0.9.9/ubo_app/store/main/reducer.py
+-rw-r--r--   0        0        0      655 2024-01-20 02:39:43.784109 ubo_app-0.9.9/ubo_app/store/services/camera.py
+-rw-r--r--   0        0        0     2383 2024-02-08 23:32:26.694739 ubo_app-0.9.9/ubo_app/store/services/docker.py
+-rw-r--r--   0        0        0      298 2024-01-20 02:39:43.784322 ubo_app-0.9.9/ubo_app/store/services/ethernet.py
+-rw-r--r--   0        0        0      588 2024-01-20 02:39:43.784547 ubo_app-0.9.9/ubo_app/store/services/ip.py
+-rw-r--r--   0        0        0      583 2024-01-20 02:39:43.784723 ubo_app-0.9.9/ubo_app/store/services/keypad.py
+-rw-r--r--   0        0        0     2830 2024-01-21 21:40:07.987830 ubo_app-0.9.9/ubo_app/store/services/notifications.py
+-rw-r--r--   0        0        0     2093 2024-02-04 13:12:10.962067 ubo_app-0.9.9/ubo_app/store/services/rgb_ring.py
+-rw-r--r--   0        0        0      869 2024-01-22 05:17:55.559542 ubo_app-0.9.9/ubo_app/store/services/sensors.py
+-rw-r--r--   0        0        0      902 2024-01-20 02:39:43.785360 ubo_app-0.9.9/ubo_app/store/services/sound.py
+-rw-r--r--   0        0        0     1414 2024-01-20 02:39:43.785567 ubo_app-0.9.9/ubo_app/store/services/wifi.py
+-rw-r--r--   0        0        0      508 2024-01-22 00:41:10.125509 ubo_app-0.9.9/ubo_app/store/status_icons/__init__.py
+-rw-r--r--   0        0        0     1286 2024-01-22 00:42:02.945066 ubo_app-0.9.9/ubo_app/store/status_icons/reducer.py
+-rw-r--r--   0        0        0     1059 2024-02-04 13:12:10.962278 ubo_app-0.9.9/ubo_app/store/update_manager/__init__.py
+-rw-r--r--   0        0        0     3326 2024-02-04 15:03:26.551436 ubo_app-0.9.9/ubo_app/store/update_manager/reducer.py
+-rw-r--r--   0        0        0     5461 2024-02-04 13:12:10.962665 ubo_app-0.9.9/ubo_app/store/update_manager/utils.py
+-rw-r--r--   0        0        0        0 2024-02-04 13:12:10.962703 ubo_app-0.9.9/ubo_app/system/__init__.py
+-rw-r--r--   0        0        0     5972 2024-02-05 08:32:29.171761 ubo_app-0.9.9/ubo_app/system/bootstrap.py
+-rwxr-xr-x   0        0        0     2786 2024-02-05 08:37:17.399214 ubo_app-0.9.9/ubo_app/system/install.sh
+-rwxr-xr-x   0        0        0     1001 2024-02-04 13:12:10.963703 ubo_app-0.9.9/ubo_app/system/install_docker.sh
+-rwxr-xr-x   0        0        0     2004 2024-02-05 04:08:43.165059 ubo_app-0.9.9/ubo_app/system/install_wm8960.sh
+-rw-r--r--   0        0        0      468 2024-02-04 16:16:26.634705 ubo_app-0.9.9/ubo_app/system/polkit-reboot.rules
+-rw-r--r--   0        0        0      360 2024-02-06 18:23:33.047193 ubo_app-0.9.9/ubo_app/system/services/app.service
+-rw-r--r--   0        0        0      554 2024-02-04 13:12:10.964300 ubo_app-0.9.9/ubo_app/system/services/system.service
+-rw-r--r--   0        0        0      401 2024-01-23 04:19:54.162152 ubo_app-0.9.9/ubo_app/system/services/update.service
+-rw-r--r--   0        0        0        0 2024-02-04 13:12:10.964383 ubo_app-0.9.9/ubo_app/system/system_manager/__init__.py
+-rw-r--r--   0        0        0     5563 2024-02-06 19:31:41.674447 ubo_app-0.9.9/ubo_app/system/system_manager/__main__.py
+-rw-r--r--   0        0        0    12038 2024-02-06 19:33:33.119867 ubo_app-0.9.9/ubo_app/system/system_manager/led.py
+-rw-r--r--   0        0        0     1067 2024-01-22 23:33:10.911357 ubo_app-0.9.9/ubo_app/utils/__init__.py
+-rw-r--r--   0        0        0     1521 2024-02-04 13:12:10.965089 ubo_app-0.9.9/ubo_app/utils/async_.py
+-rw-r--r--   0        0        0      657 2024-02-07 22:44:15.074865 ubo_app-0.9.9/ubo_app/utils/bus_provider.py
+-rw-r--r--   0        0        0     1459 2024-02-07 22:18:11.492744 ubo_app-0.9.9/ubo_app/utils/fake.py
+-rw-r--r--   0        0        0     1674 2024-02-04 13:12:10.965407 ubo_app-0.9.9/ubo_app/utils/loop.py
+-rw-r--r--   0        0        0     1428 2024-02-07 22:59:42.606700 ubo_app-0.9.9/ubo_app/utils/monitor_unit.py
+-rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 ubo_app-0.9.9/PKG-INFO
```

### Comparing `ubo_app-0.9.8a4/README.md` & `ubo_app-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/pyproject.toml` & `ubo_app-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ubo-app"
-version = "0.9.8a4"
+version = "0.9.9"
 description = "Ubo main app, running on device initialization. A platform for running other apps."
 authors = ["Sassan Haradji <sassanh@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "ubo_app" }]
 include = ['ubo_app/services/*-sound/sounds/*']
 
@@ -14,18 +14,18 @@
 priority = "primary"
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 psutil = "^5.9.8"
 ubo-gui = [
-  { version = "^0.9.1", markers = "extra=='default'", extras = [
+  { version = "^0.9.2", markers = "extra=='default'", extras = [
     'default',
   ] },
-  { version = "^0.9.1", markers = "extra=='dev'", extras = [
+  { version = "^0.9.2", markers = "extra=='dev'", extras = [
     'dev',
   ] },
 ]
 python-redux = "^0.9.23"
 pyzbar = "^0.1.9"
 sdbus-networkmanager = { version = "^2.0.0", markers = "platform_machine=='aarch64'" }
 rpi_ws281x = { version = "^5.0.0", markers = "platform_machine=='aarch64'" }
@@ -40,14 +40,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.349"
 ruff = "^0.1.9"
+toml = "^0.10.2"
 
 [tool.poetry.extras]
 default = ['ubo-gui', 'headless-kivy-pi']
 dev = ['ubo-gui', 'headless-kivy-pi']
 
 [tool.poetry.scripts]
 ubo = "ubo_app:main"
```

### Comparing `ubo_app-0.9.8a4/ubo_app/constants.py` & `ubo_app-0.9.9/ubo_app/constants.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/load_services.py` & `ubo_app-0.9.9/ubo_app/load_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             if spec and spec.origin:
                 spec.name = module_name
                 spec.loader = UboServiceModuleLoader(fullname, spec.origin)
             return spec
         return None
 
 
-sys.meta_path.insert(0, UboServiceFinder())
+sys.meta_path.append(UboServiceFinder())
 
 
 class UboServiceThread(threading.Thread):
     def __init__(
         self: UboServiceThread,
         path: Path,
         service_uid: str,
```

### Comparing `ubo_app-0.9.8a4/ubo_app/logging.py` & `ubo_app-0.9.9/ubo_app/logging.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/menu_central.py` & `ubo_app-0.9.9/ubo_app/menu_central.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/menu_footer.py` & `ubo_app-0.9.9/ubo_app/menu_footer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/reducer.py` & `ubo_app-0.9.9/ubo_app/services/000-rgb-ring/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/rgb_ring_client.py` & `ubo_app-0.9.9/ubo_app/services/000-rgb-ring/rgb_ring_client.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-rgb-ring/setup.py` & `ubo_app-0.9.9/ubo_app/services/000-rgb-ring/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/audio_manager.py` & `ubo_app-0.9.9/ubo_app/services/000-sound/audio_manager.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/reducer.py` & `ubo_app-0.9.9/ubo_app/services/000-sound/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/setup.py` & `ubo_app-0.9.9/ubo_app/services/000-sound/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/add.wav` & `ubo_app-0.9.9/ubo_app/services/000-sound/sounds/add.wav`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/done.wav` & `ubo_app-0.9.9/ubo_app/services/000-sound/sounds/done.wav`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/failure.wav` & `ubo_app-0.9.9/ubo_app/services/000-sound/sounds/failure.wav`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/scan.wav` & `ubo_app-0.9.9/ubo_app/services/000-sound/sounds/scan.wav`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/000-sound/sounds/volume.wav` & `ubo_app-0.9.9/ubo_app/services/000-sound/sounds/volume.wav`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-ethernet/ethernet_manager.py` & `ubo_app-0.9.9/ubo_app/services/010-ethernet/ethernet_manager.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-ethernet/setup.py` & `ubo_app-0.9.9/ubo_app/services/010-ethernet/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-ip/reducer.py` & `ubo_app-0.9.9/ubo_app/services/010-ip/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-ip/setup.py` & `ubo_app-0.9.9/ubo_app/services/010-ip/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/create_wireless_connection.kv` & `ubo_app-0.9.9/ubo_app/services/010-wifi/pages/create_wireless_connection.kv`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/create_wireless_connection.py` & `ubo_app-0.9.9/ubo_app/services/010-wifi/pages/create_wireless_connection.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-wifi/pages/main.py` & `ubo_app-0.9.9/ubo_app/services/010-wifi/pages/main.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-wifi/reducer.py` & `ubo_app-0.9.9/ubo_app/services/010-wifi/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-wifi/setup.py` & `ubo_app-0.9.9/ubo_app/services/010-wifi/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/010-wifi/wifi_manager.py` & `ubo_app-0.9.9/ubo_app/services/010-wifi/wifi_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # pyright: reportMissingImports=false
 # ruff: noqa: D100, D101, D102, D103, D104, D105, D107
 from __future__ import annotations
 
 import asyncio
 import uuid
-from threading import current_thread
 from typing import TYPE_CHECKING, Any, Coroutine, TypeVar, cast
 
 from debouncer import DebounceOptions, debounce
 from ubo_gui.constants import DANGER_COLOR
 
 from ubo_app.store import dispatch
 from ubo_app.store.services.notifications import (
@@ -20,14 +19,15 @@
 from ubo_app.store.services.wifi import (
     ConnectionState,
     GlobalWiFiState,
     WiFiConnection,
     WiFiType,
 )
 from ubo_app.utils import IS_RPI
+from ubo_app.utils.bus_provider import get_system_bus
 
 if TYPE_CHECKING:
     from asyncio.tasks import _FutureLike
 
 
 T = TypeVar('T')
 
@@ -43,15 +43,14 @@
 
     sys.modules['sdbus'] = Fake()
     sys.modules['sdbus_async'] = Fake()
     sys.modules['sdbus_async.networkmanager'] = Fake()
     sys.modules['sdbus_async.networkmanager.enums'] = Fake()
 
 
-from sdbus import SdBus, sd_bus_open_system, set_default_bus  # noqa: E402
 from sdbus_async.networkmanager import (  # noqa: E402
     AccessPoint,
     ActiveConnection,
     DeviceState,
     NetworkConnectionSettings,
     NetworkDeviceGeneric,
     NetworkDeviceWireless,
@@ -60,24 +59,14 @@
     NetworkManagerSettings,
 )
 from sdbus_async.networkmanager.enums import (  # noqa: E402
     ConnectionState as SdBusConnectionState,
 )
 from sdbus_async.networkmanager.enums import DeviceType  # noqa: E402
 
-system_buses = {}
-
-
-def get_system_bus() -> SdBus:
-    thread = current_thread()
-    if thread not in system_buses:
-        system_buses[thread] = sd_bus_open_system()
-    set_default_bus(system_buses[thread])
-    return system_buses[thread]
-
 
 async def get_wifi_device() -> NetworkDeviceWireless | None:
     network_manager = NetworkManager(get_system_bus())
     devices_paths = await wait_for(
         network_manager.get_devices(),
     )
     for device_path in devices_paths:
```

### Comparing `ubo_app-0.9.8a4/ubo_app/services/020-keyboard/setup.py` & `ubo_app-0.9.9/ubo_app/services/020-keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/020-keypad/setup.py` & `ubo_app-0.9.9/ubo_app/services/020-keypad/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/030-notifications/reducer.py` & `ubo_app-0.9.9/ubo_app/services/030-notifications/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/040-camera/reducer.py` & `ubo_app-0.9.9/ubo_app/services/040-camera/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/040-camera/setup.py` & `ubo_app-0.9.9/ubo_app/services/040-camera/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/040-sensors/reducer.py` & `ubo_app-0.9.9/ubo_app/services/040-sensors/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/040-sensors/setup.py` & `ubo_app-0.9.9/ubo_app/services/040-sensors/setup.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/services/080-docker/reducer.py` & `ubo_app-0.9.9/ubo_app/services/080-docker/reducer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Docker reducer."""
 from __future__ import annotations
 
-from dataclasses import replace
+from dataclasses import field, replace
 
 from immutable import Immutable
 from redux import (
     BaseEvent,
     CombineReducerAction,
     CombineReducerInitAction,
     InitAction,
@@ -14,14 +14,15 @@
     combine_reducers,
 )
 
 from ubo_app.store.services.docker import (
     DockerAction,
     DockerImageAction,
     DockerImageEvent,
+    DockerImageSetDockerIdAction,
     DockerImageSetStatusAction,
     DockerServiceState,
     DockerSetStatusAction,
     DockerState,
     ImageState,
 )
 
@@ -47,15 +48,15 @@
 class ImageEntry(Immutable):
     """An image to be used in a Docker container."""
 
     id: str
     label: str
     icon: str
     path: str
-    ports: dict[str, str] | None = None
+    ports: dict[str, str] = field(default_factory=dict)
     volumes: list[str] | None = None
 
 
 IMAGES = {
     image.id: image
     for image in [
         ImageEntry(
@@ -80,14 +81,20 @@
         ),
         ImageEntry(
             id='pi_hole',
             label='Pi-hole',
             icon='dns',
             path='pihole/pihole:latest',
         ),
+        ImageEntry(
+            id='alpine',
+            label='Alpine',
+            icon='code',
+            path='alpine:latest',
+        ),
     ]
 }
 IMAGE_IDS = list(IMAGES.keys())
 
 
 def image_reducer(
     state: ImageState | None,
@@ -111,14 +118,17 @@
     if isinstance(action, DockerImageSetStatusAction):
         return replace(
             state,
             status=action.status,
             ports=action.ports if action.ports else state.ports,
         )
 
+    if isinstance(action, DockerImageSetDockerIdAction):
+        return replace(state, docker_id=action.docker_id)
+
     return state
 
 
 reducer, reducer_id = combine_reducers(
     state_type=DockerState,
     action_type=DockerImageAction,
     event_type=DockerImageEvent,
```

### Comparing `ubo_app-0.9.8a4/ubo_app/side_effects.py` & `ubo_app-0.9.9/ubo_app/side_effects.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/__init__.py` & `ubo_app-0.9.9/ubo_app/store/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/main/__init__.py` & `ubo_app-0.9.9/ubo_app/store/main/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/main/_menus.py` & `ubo_app-0.9.9/ubo_app/store/main/_menus.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/main/reducer.py` & `ubo_app-0.9.9/ubo_app/store/main/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/camera.py` & `ubo_app-0.9.9/ubo_app/store/services/camera.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/docker.py` & `ubo_app-0.9.9/ubo_app/store/services/docker.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,20 +42,26 @@
 class DockerImageAction(DockerAction):
     """Docker image action."""
 
     image: str
 
 
 class DockerImageSetStatusAction(DockerImageAction):
-    """Docker image action."""
+    """Docker image set status action."""
 
     status: ImageStatus
     ports: list[str] | None = None
 
 
+class DockerImageSetDockerIdAction(DockerImageAction):
+    """Docker image set docker id action."""
+
+    docker_id: str
+
+
 class DockerEvent(BaseEvent):
     """Docker event."""
 
 
 class DockerServiceState(Immutable):
     """Docker service state."""
 
@@ -72,14 +78,15 @@
     """Image state."""
 
     id: str
     label: str
     icon: str
     path: str
     status: ImageStatus = ImageStatus.NOT_AVAILABLE
+    docker_id: str | None = None
     ports: list[str] = field(default_factory=list)
 
     @property
     def is_fetching(self: ImageState) -> bool:
         """Check if image is available."""
         return self.status == ImageStatus.FETCHING
```

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/ip.py` & `ubo_app-0.9.9/ubo_app/store/services/ip.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/keypad.py` & `ubo_app-0.9.9/ubo_app/store/services/keypad.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/notifications.py` & `ubo_app-0.9.9/ubo_app/store/services/notifications.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/rgb_ring.py` & `ubo_app-0.9.9/ubo_app/store/services/rgb_ring.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/sensors.py` & `ubo_app-0.9.9/ubo_app/store/services/sensors.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/sound.py` & `ubo_app-0.9.9/ubo_app/store/services/sound.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/services/wifi.py` & `ubo_app-0.9.9/ubo_app/store/services/wifi.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/status_icons/reducer.py` & `ubo_app-0.9.9/ubo_app/store/status_icons/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/update_manager/__init__.py` & `ubo_app-0.9.9/ubo_app/store/update_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/update_manager/reducer.py` & `ubo_app-0.9.9/ubo_app/store/update_manager/reducer.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/store/update_manager/utils.py` & `ubo_app-0.9.9/ubo_app/store/update_manager/utils.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/system/bootstrap.py` & `ubo_app-0.9.9/ubo_app/system/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/system/install.sh` & `ubo_app-0.9.9/ubo_app/system/install.sh`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/system/install_docker.sh` & `ubo_app-0.9.9/ubo_app/system/install_docker.sh`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/system/install_wm8960.sh` & `ubo_app-0.9.9/ubo_app/system/install_wm8960.sh`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/system/services/system.service` & `ubo_app-0.9.9/ubo_app/system/services/system.service`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/system/system_manager/__main__.py` & `ubo_app-0.9.9/ubo_app/system/system_manager/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -87,20 +87,48 @@
                                     .parent.parent.joinpath('install_docker.sh')
                                     .as_posix(),
                                     env={'USERNAME': USERNAME},
                                     check=False,
                                 )
                             elif command == 'start':
                                 subprocess.run(
-                                    ['/usr/bin/env', 'systemctl', 'start', 'docker'],  # noqa: S603
+                                    [  # noqa: S603
+                                        '/usr/bin/env',
+                                        'systemctl',
+                                        'start',
+                                        'docker.socket',
+                                    ],
+                                    check=False,
+                                )
+                                subprocess.run(
+                                    [  # noqa: S603
+                                        '/usr/bin/env',
+                                        'systemctl',
+                                        'start',
+                                        'docker.service',
+                                    ],
                                     check=False,
                                 )
                             elif command == 'stop':
                                 subprocess.run(
-                                    ['/usr/bin/env', 'systemctl', 'stop', 'docker'],  # noqa: S603
+                                    [  # noqa: S603
+                                        '/usr/bin/env',
+                                        'systemctl',
+                                        'stop',
+                                        'docker.socket',
+                                    ],
+                                    check=False,
+                                )
+                                subprocess.run(
+                                    [  # noqa: S603
+                                        '/usr/bin/env',
+                                        'systemctl',
+                                        'stop',
+                                        'docker.service',
+                                    ],
                                     check=False,
                                 )
                         finally:
                             DOCKER_INSTALLATION_LOCK_FILE.unlink(missing_ok=True)
 
                     thread = Thread(target=install_docker, args=(incoming[0],))
                     thread.start()
```

### Comparing `ubo_app-0.9.8a4/ubo_app/system/system_manager/led.py` & `ubo_app-0.9.9/ubo_app/system/system_manager/led.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         ring[0 : int(self.num_leds * percentage)] = [color] * (
             int(self.num_leds * percentage)
         )
         self.pixels[:] = ring
         self.pixels.show()
 
     def run_command(self: LEDManager, incoming: Sequence[str]) -> None:  # noqa: C901, PLR0912
-        self.logger.info('---executing command---')
+        self.logger.info('Executing LED command', extra={'incoming': incoming})
         self.incoming = incoming
         self._stop = False
         if incoming[0] == 'set_enabled' and len(incoming) == 2:
             self.set_enabled(enabled=incoming[1] == '1')
         # set brightness of LEDs
         if incoming[0] == 'set_brightness' and len(incoming) == 2:
             brightness_value = float(incoming[1])
```

### Comparing `ubo_app-0.9.8a4/ubo_app/utils/__init__.py` & `ubo_app-0.9.9/ubo_app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/utils/async_.py` & `ubo_app-0.9.9/ubo_app/utils/async_.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/ubo_app/utils/fake.py` & `ubo_app-0.9.9/ubo_app/utils/fake.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from ubo_app.logging import logger
 
 
 class Fake(ModuleType):
     def __init__(self: Fake) -> None:
         super().__init__('')
 
+    def __init_subclass__(cls: type[Fake], **kwargs: dict[str, Any]) -> None:
+        logger.verbose('Subclassing `Fake`', extra={'cls': cls, 'kwargs': kwargs})
+
     def __getattr__(self: Fake, attr: str) -> Fake | str:
         logger.verbose(
             'Accessing fake attribute of a `Fake` insta',
             extra={'attr': attr},
         )
         if attr == '__file__':
             return ''
```

### Comparing `ubo_app-0.9.8a4/ubo_app/utils/loop.py` & `ubo_app-0.9.9/ubo_app/utils/loop.py`

 * *Files identical despite different names*

### Comparing `ubo_app-0.9.8a4/PKG-INFO` & `ubo_app-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubo-app
-Version: 0.9.8a4
+Version: 0.9.9
 Summary: Ubo main app, running on device initialization. A platform for running other apps.
 License: Apache-2.0
 Author: Sassan Haradji
 Author-email: sassanh@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,16 @@
 Requires-Dist: pulsectl (>=23.5.2,<24.0.0)
 Requires-Dist: python-debouncer (>=0.1.3,<0.2.0)
 Requires-Dist: python-redux (>=0.9.23,<0.10.0)
 Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
 Requires-Dist: rpi_ws281x (>=5.0.0,<6.0.0) ; platform_machine == "aarch64"
 Requires-Dist: sdbus-networkmanager (>=2.0.0,<3.0.0) ; platform_machine == "aarch64"
 Requires-Dist: semver (>=3.0.2,<4.0.0)
-Requires-Dist: ubo-gui[default] (>=0.9.1,<0.10.0) ; extra == "default"
-Requires-Dist: ubo-gui[dev] (>=0.9.1,<0.10.0) ; extra == "dev"
+Requires-Dist: ubo-gui[default] (>=0.9.2,<0.10.0) ; extra == "default"
+Requires-Dist: ubo-gui[dev] (>=0.9.2,<0.10.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # 🚀 Ubo App
 
 ## 🌟 Overview
 
 Ubo App is a Python application for managing Raspberry Pi utilities and UBo-specific
```

