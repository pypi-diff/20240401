# Comparing `tmp/donkeycar-5.0.0.tar.gz` & `tmp/donkeycar-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donkeycar-5.0.0.tar", last modified: Wed Dec 20 22:50:32 2023, max compression
+gzip compressed data, was "donkeycar-5.1.0.tar", last modified: Mon Apr  1 16:52:40 2024, max compression
```

## Comparing `donkeycar-5.0.0.tar` & `donkeycar-5.1.0.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.439806 donkeycar-5.0.0/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1068 2023-08-26 20:46:01.000000 donkeycar-5.0.0/LICENSE
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      108 2023-12-20 21:01:33.000000 donkeycar-5.0.0/MANIFEST.in
--rw-r--r--   0 dirk      (1000) dirk      (1000)     5609 2023-12-20 22:50:32.439806 donkeycar-5.0.0/PKG-INFO
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2843 2022-11-29 22:11:04.000000 donkeycar-5.0.0/README.md
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      669 2023-12-20 21:06:09.000000 donkeycar-5.0.0/donkeycar/__init__.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/benchmarks/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1116 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/benchmarks/tub.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      907 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/benchmarks/tub_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2150 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/config.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/contrib/
--rw-r--r--   0 dirk      (1000) dirk      (1000)        0 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/contrib/__init__.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/contrib/robohat/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5559 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/contrib/robohat/code-robocarstore.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5531 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/contrib/robohat/code.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1198 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/contrib/robohat/rear_light.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)      900 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/geom.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/gym/
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)        0 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/gym/__init__.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2493 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/gym/gym_real.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1097 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/gym/remote_controller.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    17401 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/la.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.419805 donkeycar-5.0.0/donkeycar/management/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)        0 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/__init__.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    24240 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/base.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     6007 2022-11-29 22:04:22.000000 donkeycar-5.0.0/donkeycar/management/graph.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    20101 2022-11-29 22:11:04.000000 donkeycar-5.0.0/donkeycar/management/joystick_creator.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    51242 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/kivy_ui.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    11799 2023-12-20 21:01:33.000000 donkeycar-5.0.0/donkeycar/management/makemovie.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     3371 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/management/tub.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.419805 donkeycar-5.0.0/donkeycar/management/tub_web/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1169 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/tub_web/base.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2786 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/tub_web/tub.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      257 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/tub_web/tubs.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    23849 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/management/ui.kv
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1463 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/memory.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.423805 donkeycar-5.0.0/donkeycar/parts/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)        0 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/__init__.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    42618 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/actuator.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1577 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/behavior.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    12984 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/camera.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    54458 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/controller.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)     2794 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/coral.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    27466 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/cv.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    18590 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/datastore.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    19025 2023-12-20 21:01:33.000000 donkeycar-5.0.0/donkeycar/parts/datastore_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     3421 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/dgym.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     7441 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/encoder.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      755 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/explode.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2507 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/fast_stretch.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    10031 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/fastai.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      730 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/file_watcher.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1333 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/fps.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    25121 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/gps.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)     1135 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/graph.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     3110 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/image.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    19545 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/image_transformations.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     3475 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/imu.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    13795 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/interpreter.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    45139 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/keras.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    28493 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/kinematics.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1475 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/launch.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     3678 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/led_status.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2142 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/leopard_imaging.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    34557 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/lidar.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5730 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/line_follower.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1238 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/logger.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    13335 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/network.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.423805 donkeycar-5.0.0/donkeycar/parts/object_detector/
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     5344 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/object_detector/stop_sign_detector.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2354 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/odometer.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5314 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/oled.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    15146 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/path.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1464 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/perfmon.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2623 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/pigpio_enc.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    38605 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/pins.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      306 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/pipe.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    10800 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/pose.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.423805 donkeycar-5.0.0/donkeycar/parts/pytorch/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     3295 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/pytorch/ResNet18.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5979 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/pytorch/torch_data.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2070 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/pytorch/torch_train.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1130 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/pytorch/torch_utils.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4052 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/realsense2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    13360 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/realsense435i.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    10086 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/robohat.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1255 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/ros.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)     4711 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/salient.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)     1511 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/serial_controller.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    11032 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/serial_port.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1977 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/simulation.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)      717 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/sombrero.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    26521 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/tachometer.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)     2817 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/teensy.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     6320 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/telemetry.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4018 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/text_writer.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2207 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/tfmini.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      683 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/parts/throttle_filter.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4972 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/transform.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     6383 2023-12-20 21:01:33.000000 donkeycar-5.0.0/donkeycar/parts/tub_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4438 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/velocity.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.423805 donkeycar-5.0.0/donkeycar/parts/voice_control/
--rw-r--r--   0 dirk      (1000) dirk      (1000)     2477 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/voice_control/alexa.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.423805 donkeycar-5.0.0/donkeycar/parts/web_controller/
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.423805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1290 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/base.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1629 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/base_fpv.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     8873 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/calibrate.html
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)      564 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/home.html
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)      483 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/pilots_list.html
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     4289 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/session.html
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)      482 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/session_list.html
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.427805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.427805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/css/
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)   121200 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/css/bootstrap.min.css
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.427805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)    45404 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.ttf
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)    23424 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)    18028 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.427805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/js/
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)    37045 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/js/bootstrap.min.js
--rw-r--r--   0 dirk      (1000) dirk      (1000)    20646 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/donkeycar-logo-sideways.png
--rw-rw-r--   0 dirk      (1000) dirk      (1000)   101198 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/img_placeholder.jpg
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)    86709 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/jquery-3.1.1.min.js
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    21917 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/main.js
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)    37617 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/nipple.js
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2112 2023-02-14 22:39:57.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/style.css
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.415805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/ui/
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.427805 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/ui/1.12.1/
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)   253668 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/ui/1.12.1/jquery-ui.min.js
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     7641 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/vehicle.html
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)      485 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/vehicle_list.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1605 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/templates/wsTest.html
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    15077 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/parts/web_controller/web.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.427805 donkeycar-5.0.0/donkeycar/pipeline/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)       39 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/pipeline/__init__.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1849 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/pipeline/augmentations.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5160 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/pipeline/database.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5560 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/pipeline/sequence.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     8431 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/pipeline/training.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5232 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/pipeline/types.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.431805 donkeycar-5.0.0/donkeycar/templates/
--rw-r--r--   0 dirk      (1000) dirk      (1000)     2223 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/templates/arduino_drive.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    10717 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/templates/basic.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4848 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/templates/calibrate.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)      967 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/templates/calibration_odometry.json
--rw-r--r--   0 dirk      (1000) dirk      (1000)     2019 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/templates/cfg_arduino_drive.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     7850 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/cfg_basic.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    40765 2023-12-20 21:01:33.000000 donkeycar-5.0.0/donkeycar/templates/cfg_complete.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)    30434 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/cfg_cv_control.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    34978 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/cfg_path_follow.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    15642 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/cfg_simulator.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2196 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/templates/cfg_square.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    47672 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/complete.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     9164 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/cv_control.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     2275 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/templates/just_drive.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      236 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/templates/myconfig.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    19711 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/path_follow.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    16910 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/templates/simulator.py
--rw-r--r--   0 dirk      (1000) dirk      (1000)     5146 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/templates/square.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      728 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/templates/train.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.435805 donkeycar-5.0.0/donkeycar/tests/
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)       24 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/tests/__init__.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      121 2022-11-29 22:09:53.000000 donkeycar-5.0.0/donkeycar/tests/pytest.ini
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2120 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/setup.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      347 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/tests/test_actuator.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1233 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/test_catalog_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4105 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_circular_buffer.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      829 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/tests/test_controller.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2413 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/test_datastore_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2577 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_keras.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    32575 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_kinematics.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1905 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/tests/test_launch.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2535 2022-11-29 21:59:47.000000 donkeycar-5.0.0/donkeycar/tests/test_lidar.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1916 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/tests/test_memory.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1409 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_odometer.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)        1 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/tests/test_parts.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    10598 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_path.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5531 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/tests/test_pipeline.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     8409 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/test_robohat.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2595 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_scripts.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2909 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/test_seekable_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5839 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/tests/test_tachometer.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1385 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/test_telemetry.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1147 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/tests/test_template.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4207 2023-12-20 21:01:33.000000 donkeycar-5.0.0/donkeycar/tests/test_torch.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     8829 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/tests/test_train.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2464 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/tests/test_tub_v2.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1267 2023-07-16 15:39:04.000000 donkeycar-5.0.0/donkeycar/tests/test_tubwriter.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     4562 2022-11-29 21:48:58.000000 donkeycar-5.0.0/donkeycar/tests/test_util_data.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1453 2020-05-18 19:23:14.000000 donkeycar-5.0.0/donkeycar/tests/test_vehicle.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      726 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/tests/test_web_controller.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     5209 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/tests/test_web_socket.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.435805 donkeycar-5.0.0/donkeycar/utilities/
--rw-rw-r--   0 dirk      (1000) dirk      (1000)        0 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/utilities/__init__.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     4852 2023-11-20 21:15:19.000000 donkeycar-5.0.0/donkeycar/utilities/circular_buffer.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     2341 2022-11-30 21:40:51.000000 donkeycar-5.0.0/donkeycar/utilities/deprecated.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      657 2023-11-17 19:52:20.000000 donkeycar-5.0.0/donkeycar/utilities/dk_platform.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)    16065 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/utils.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     7352 2023-12-20 20:53:37.000000 donkeycar-5.0.0/donkeycar/vehicle.py
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.435805 donkeycar-5.0.0/donkeycar.egg-info/
--rw-r--r--   0 dirk      (1000) dirk      (1000)     5609 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/PKG-INFO
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     6851 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/SOURCES.txt
--rw-rw-r--   0 dirk      (1000) dirk      (1000)        1 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/dependency_links.txt
--rw-rw-r--   0 dirk      (1000) dirk      (1000)       79 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/entry_points.txt
--rw-rw-r--   0 dirk      (1000) dirk      (1000)      702 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/requires.txt
--rw-rw-r--   0 dirk      (1000) dirk      (1000)       31 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/top_level.txt
--rw-rw-r--   0 dirk      (1000) dirk      (1000)        1 2023-12-20 22:50:32.000000 donkeycar-5.0.0/donkeycar.egg-info/zip-safe
--rw-rw-r--   0 dirk      (1000) dirk      (1000)       93 2023-12-20 21:01:33.000000 donkeycar-5.0.0/pyproject.toml
-drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2023-12-20 22:50:32.435805 donkeycar-5.0.0/scripts/
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1407 2023-11-20 21:15:19.000000 donkeycar-5.0.0/scripts/convert_to_tflite.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     3209 2023-12-20 20:53:37.000000 donkeycar-5.0.0/scripts/convert_to_tub_v2.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1830 2022-11-29 21:48:58.000000 donkeycar-5.0.0/scripts/freeze_model.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1280 2022-11-29 21:48:58.000000 donkeycar-5.0.0/scripts/graph_listener.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     9812 2023-11-20 21:15:19.000000 donkeycar-5.0.0/scripts/hsv_picker.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1857 2022-11-29 21:48:58.000000 donkeycar-5.0.0/scripts/multi_train.py
--rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1994 2020-05-18 19:23:14.000000 donkeycar-5.0.0/scripts/pigpio_donkey.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1372 2022-12-18 21:12:10.000000 donkeycar-5.0.0/scripts/preview_augumentations.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1050 2023-12-20 21:01:33.000000 donkeycar-5.0.0/scripts/profile.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      737 2022-11-29 21:48:58.000000 donkeycar-5.0.0/scripts/profile_coral.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1605 2023-11-17 19:52:20.000000 donkeycar-5.0.0/scripts/remote_cam_view.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1361 2022-11-29 21:48:58.000000 donkeycar-5.0.0/scripts/remote_cam_view_tcp.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1284 2023-11-17 19:52:20.000000 donkeycar-5.0.0/scripts/salient_vis_listener.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)      415 2022-11-29 21:59:47.000000 donkeycar-5.0.0/scripts/tflite_convert.py
--rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1174 2022-11-29 21:48:58.000000 donkeycar-5.0.0/scripts/tflite_profile.py
--rw-rw-r--   0 dirk      (1000) dirk      (1000)     1676 2023-12-20 22:50:32.439806 donkeycar-5.0.0/setup.cfg
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.267599 donkeycar-5.1.0/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1068 2023-08-26 20:46:01.000000 donkeycar-5.1.0/LICENSE
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      108 2024-01-21 20:45:16.000000 donkeycar-5.1.0/MANIFEST.in
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     5581 2024-04-01 16:52:40.267599 donkeycar-5.1.0/PKG-INFO
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2843 2024-01-19 21:48:36.000000 donkeycar-5.1.0/README.md
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      671 2024-04-01 15:15:24.000000 donkeycar-5.1.0/donkeycar/__init__.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/benchmarks/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1116 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/benchmarks/tub.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      907 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/benchmarks/tub_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2150 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/config.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/contrib/
+-rw-r--r--   0 dirk      (1000) dirk      (1000)        0 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/contrib/__init__.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/contrib/robohat/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5559 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/contrib/robohat/code-robocarstore.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5531 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/contrib/robohat/code.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1198 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/contrib/robohat/rear_light.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)      900 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/geom.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/gym/
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)        0 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/gym/__init__.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2493 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/gym/gym_real.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1097 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/gym/remote_controller.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    17401 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/la.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/management/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)        0 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/management/__init__.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    24240 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/management/base.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     6007 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/management/graph.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    20101 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/management/joystick_creator.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    51245 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/management/kivy_ui.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    11799 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/management/makemovie.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     3371 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/management/tub.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.235597 donkeycar-5.1.0/donkeycar/management/tub_web/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1169 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/management/tub_web/base.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2786 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/management/tub_web/tub.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      257 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/management/tub_web/tubs.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    23850 2024-03-31 18:43:51.000000 donkeycar-5.1.0/donkeycar/management/ui.kv
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1463 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/memory.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.247598 donkeycar-5.1.0/donkeycar/parts/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)        0 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/__init__.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    42645 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/actuator.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1577 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/behavior.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    12984 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/camera.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    54467 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/controller.py
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     2794 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/coral.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    27466 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/cv.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    18590 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/datastore.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    19025 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/datastore_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     3421 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/dgym.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     7441 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/encoder.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      755 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/explode.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2507 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/parts/fast_stretch.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     9966 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/fastai.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      730 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/file_watcher.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1333 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/fps.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    25121 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/gps.py
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     1135 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/graph.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     3110 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/parts/image.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    19545 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/image_transformations.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     3475 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/imu.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    13759 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/interpreter.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    45139 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/keras.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    28502 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/kinematics.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1475 2023-11-17 19:52:20.000000 donkeycar-5.1.0/donkeycar/parts/launch.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     3678 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/led_status.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2142 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/parts/leopard_imaging.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    34557 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/lidar.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5730 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/line_follower.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1238 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/logger.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    13335 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/network.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.247598 donkeycar-5.1.0/donkeycar/parts/object_detector/
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     5344 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/object_detector/stop_sign_detector.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2354 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/odometer.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5314 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/oled.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    15146 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/path.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1464 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/parts/perfmon.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2623 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/pigpio_enc.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    38611 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/pins.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      306 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/pipe.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    10800 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/pose.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.247598 donkeycar-5.1.0/donkeycar/parts/pytorch/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     3295 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/pytorch/ResNet18.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5979 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/pytorch/torch_data.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2078 2024-03-31 18:43:51.000000 donkeycar-5.1.0/donkeycar/parts/pytorch/torch_train.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1130 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/parts/pytorch/torch_utils.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4052 2023-11-17 19:52:20.000000 donkeycar-5.1.0/donkeycar/parts/realsense2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    13360 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/realsense435i.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    10086 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/robohat.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1255 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/ros.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4711 2024-03-10 12:39:15.000000 donkeycar-5.1.0/donkeycar/parts/salient.py
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     1511 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/serial_controller.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    11044 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/serial_port.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1977 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/simulation.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)      717 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/sombrero.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    26524 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/parts/tachometer.py
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     2817 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/teensy.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     6415 2024-03-31 18:43:51.000000 donkeycar-5.1.0/donkeycar/parts/telemetry.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4018 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/text_writer.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2207 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/tfmini.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      683 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/throttle_filter.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4972 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/transform.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     6383 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/tub_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4438 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/velocity.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.247598 donkeycar-5.1.0/donkeycar/parts/voice_control/
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     2477 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/voice_control/alexa.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.247598 donkeycar-5.1.0/donkeycar/parts/web_controller/
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.247598 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1290 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/base.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1629 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/base_fpv.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     8873 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/calibrate.html
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)      564 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/home.html
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)      483 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/pilots_list.html
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     4289 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/session.html
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)      482 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/session_list.html
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.251598 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.231597 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.231597 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.251598 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/css/
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)   121200 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/css/bootstrap.min.css
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.251598 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)    45404 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.ttf
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)    23424 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)    18028 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.251598 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/js/
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)    37045 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/js/bootstrap.min.js
+-rw-r--r--   0 dirk      (1000) dirk      (1000)    20646 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/donkeycar-logo-sideways.png
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)   101198 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/img_placeholder.jpg
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)    86709 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/jquery-3.1.1.min.js
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    21917 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/main.js
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)    37617 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/nipple.js
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2112 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/style.css
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.231597 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/ui/
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.251598 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/ui/1.12.1/
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)   253668 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/ui/1.12.1/jquery-ui.min.js
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     7641 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/vehicle.html
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)      485 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/vehicle_list.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1605 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/templates/wsTest.html
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    15077 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/parts/web_controller/web.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.255598 donkeycar-5.1.0/donkeycar/pipeline/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)       39 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/pipeline/__init__.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1849 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/pipeline/augmentations.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5160 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/pipeline/database.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5560 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/pipeline/sequence.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     8431 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/pipeline/training.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5232 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/pipeline/types.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.255598 donkeycar-5.1.0/donkeycar/templates/
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     2223 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/templates/arduino_drive.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    10717 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/templates/basic.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4848 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/calibrate.py
+-rw-r--r--   0 dirk      (1000) dirk      (1000)      967 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/templates/calibration_odometry.json
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     2019 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/templates/cfg_arduino_drive.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     7850 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/cfg_basic.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    40765 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/templates/cfg_complete.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)    30434 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/cfg_cv_control.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    34978 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/cfg_path_follow.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    15642 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/cfg_simulator.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2196 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/cfg_square.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    47672 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/complete.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     9164 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/cv_control.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     2275 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/templates/just_drive.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      236 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/templates/myconfig.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    19711 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/path_follow.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    16910 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/templates/simulator.py
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     5146 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/templates/square.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      728 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/templates/train.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.259598 donkeycar-5.1.0/donkeycar/tests/
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)       24 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/tests/__init__.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      121 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/pytest.ini
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2120 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/tests/setup.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      347 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/tests/test_actuator.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1233 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/tests/test_catalog_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4105 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_circular_buffer.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      829 2023-11-17 19:52:20.000000 donkeycar-5.1.0/donkeycar/tests/test_controller.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2413 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/tests/test_datastore_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2600 2024-04-01 13:50:21.000000 donkeycar-5.1.0/donkeycar/tests/test_keras.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    32575 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_kinematics.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1905 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/tests/test_launch.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2535 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_lidar.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1916 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/tests/test_memory.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1409 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_odometer.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)        1 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/tests/test_parts.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    10598 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_path.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5531 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/tests/test_pipeline.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     8409 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/tests/test_robohat.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     2595 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_scripts.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2909 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/tests/test_seekable_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5839 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_tachometer.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1378 2024-03-31 18:43:51.000000 donkeycar-5.1.0/donkeycar/tests/test_telemetry.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1147 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/tests/test_template.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4215 2024-03-31 18:43:51.000000 donkeycar-5.1.0/donkeycar/tests/test_torch.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     8829 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/tests/test_train.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2464 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/tests/test_tub_v2.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1267 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_tubwriter.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     4562 2022-11-29 21:48:58.000000 donkeycar-5.1.0/donkeycar/tests/test_util_data.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1453 2020-05-18 19:23:14.000000 donkeycar-5.1.0/donkeycar/tests/test_vehicle.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      726 2023-11-17 19:52:20.000000 donkeycar-5.1.0/donkeycar/tests/test_web_controller.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     5209 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/tests/test_web_socket.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.259598 donkeycar-5.1.0/donkeycar/utilities/
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)        0 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/utilities/__init__.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     4852 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/utilities/circular_buffer.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     2341 2024-03-31 11:14:44.000000 donkeycar-5.1.0/donkeycar/utilities/deprecated.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      657 2024-01-19 21:48:36.000000 donkeycar-5.1.0/donkeycar/utilities/dk_platform.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)    16065 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/utils.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     7352 2024-03-14 21:48:53.000000 donkeycar-5.1.0/donkeycar/vehicle.py
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.263599 donkeycar-5.1.0/donkeycar.egg-info/
+-rw-r--r--   0 dirk      (1000) dirk      (1000)     5581 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/PKG-INFO
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     6851 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/SOURCES.txt
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)        1 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/dependency_links.txt
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)       79 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/entry_points.txt
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)      699 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/requires.txt
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)       31 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/top_level.txt
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)        1 2024-04-01 16:52:40.000000 donkeycar-5.1.0/donkeycar.egg-info/zip-safe
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)       93 2024-01-21 20:45:16.000000 donkeycar-5.1.0/pyproject.toml
+drwxrwxr-x   0 dirk      (1000) dirk      (1000)        0 2024-04-01 16:52:40.263599 donkeycar-5.1.0/scripts/
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1407 2024-01-19 21:48:36.000000 donkeycar-5.1.0/scripts/convert_to_tflite.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     3209 2024-03-14 21:48:53.000000 donkeycar-5.1.0/scripts/convert_to_tub_v2.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1830 2022-11-29 21:48:58.000000 donkeycar-5.1.0/scripts/freeze_model.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1280 2022-11-29 21:48:58.000000 donkeycar-5.1.0/scripts/graph_listener.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     9812 2024-01-19 21:48:36.000000 donkeycar-5.1.0/scripts/hsv_picker.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1857 2022-11-29 21:48:58.000000 donkeycar-5.1.0/scripts/multi_train.py
+-rwxr-xr-x   0 dirk      (1000) dirk      (1000)     1994 2020-05-18 19:23:14.000000 donkeycar-5.1.0/scripts/pigpio_donkey.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1372 2024-01-19 21:48:36.000000 donkeycar-5.1.0/scripts/preview_augumentations.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1050 2024-03-14 21:48:53.000000 donkeycar-5.1.0/scripts/profile.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      737 2022-11-29 21:48:58.000000 donkeycar-5.1.0/scripts/profile_coral.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1605 2023-11-17 19:52:20.000000 donkeycar-5.1.0/scripts/remote_cam_view.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1361 2022-11-29 21:48:58.000000 donkeycar-5.1.0/scripts/remote_cam_view_tcp.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1284 2023-11-17 19:52:20.000000 donkeycar-5.1.0/scripts/salient_vis_listener.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)      415 2024-01-19 21:48:36.000000 donkeycar-5.1.0/scripts/tflite_convert.py
+-rwxrwxr-x   0 dirk      (1000) dirk      (1000)     1174 2022-11-29 21:48:58.000000 donkeycar-5.1.0/scripts/tflite_profile.py
+-rw-rw-r--   0 dirk      (1000) dirk      (1000)     1641 2024-04-01 16:52:40.267599 donkeycar-5.1.0/setup.cfg
```

### Comparing `donkeycar-5.0.0/LICENSE` & `donkeycar-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/PKG-INFO` & `donkeycar-5.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 Metadata-Version: 2.1
 Name: donkeycar
-Version: 5.0.0
+Version: 5.1.0
 Summary: Self driving library for python.
 Home-page: https://github.com/autorope/donkeycar
 Author: Will Roscoe, Adam Conway, Tawn Kramer
 License: MIT
 Keywords: selfdriving cars donkeycar diyrobocars
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: <4,>=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: docopt
 Requires-Dist: tornado
 Requires-Dist: requests
 Requires-Dist: PrettyTable
 Requires-Dist: paho-mqtt
 Requires-Dist: simple_pid
 Requires-Dist: progress
-Requires-Dist: typing_extensions
 Requires-Dist: pyfiglet
 Requires-Dist: psutil
 Requires-Dist: pynmea2
 Requires-Dist: pyserial
 Requires-Dist: utm
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Provides-Extra: pi
 Requires-Dist: picamera2; extra == "pi"
 Requires-Dist: Adafruit_PCA9685; extra == "pi"
 Requires-Dist: adafruit-circuitpython-ssd1306; extra == "pi"
 Requires-Dist: adafruit-circuitpython-rplidar; extra == "pi"
 Requires-Dist: RPi.GPIO; extra == "pi"
-Requires-Dist: tensorflow-aarch64==2.9.3; extra == "pi"
+Requires-Dist: tensorflow-aarch64==2.15.*; extra == "pi"
 Requires-Dist: opencv-contrib-python; extra == "pi"
 Provides-Extra: nano
 Requires-Dist: Adafruit_PCA9685; extra == "nano"
 Requires-Dist: adafruit-circuitpython-ssd1306; extra == "nano"
 Requires-Dist: adafruit-circuitpython-rplidar; extra == "nano"
 Requires-Dist: Jetson.GPIO; extra == "nano"
-Requires-Dist: numpy==1.23; extra == "nano"
-Requires-Dist: matplotlib==3.7; extra == "nano"
-Requires-Dist: kivy==2.1; extra == "nano"
+Requires-Dist: numpy==1.23.*; extra == "nano"
+Requires-Dist: matplotlib==3.7.*; extra == "nano"
+Requires-Dist: kivy; extra == "nano"
 Requires-Dist: plotly; extra == "nano"
-Requires-Dist: pandas==2.0; extra == "nano"
+Requires-Dist: pandas==2.0.*; extra == "nano"
 Provides-Extra: pc
-Requires-Dist: tensorflow==2.9; extra == "pc"
+Requires-Dist: tensorflow==2.15.*; extra == "pc"
 Requires-Dist: matplotlib; extra == "pc"
-Requires-Dist: kivy==2.1; extra == "pc"
+Requires-Dist: kivy; extra == "pc"
 Requires-Dist: pandas; extra == "pc"
 Requires-Dist: plotly; extra == "pc"
 Requires-Dist: albumentations; extra == "pc"
 Provides-Extra: macos
-Requires-Dist: tensorflow-macos==2.9; extra == "macos"
+Requires-Dist: tensorflow-macos==2.15.*; extra == "macos"
 Requires-Dist: matplotlib; extra == "macos"
-Requires-Dist: kivy==2.1; extra == "macos"
+Requires-Dist: kivy; extra == "macos"
 Requires-Dist: pandas; extra == "macos"
 Requires-Dist: plotly; extra == "macos"
 Requires-Dist: albumentations; extra == "macos"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: responses; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Provides-Extra: torch
-Requires-Dist: pytorch; extra == "torch"
-Requires-Dist: torchvision==0.12; extra == "torch"
+Requires-Dist: torch==2.1.*; extra == "torch"
+Requires-Dist: pytorch-lightning; extra == "torch"
+Requires-Dist: torchvision; extra == "torch"
 Requires-Dist: torchaudio; extra == "torch"
 Requires-Dist: fastai; extra == "torch"
 
 # Donkeycar: a python self driving library
 
 
 ![Build Status](https://github.com/autorope/donkeycar/actions/workflows/python-package-conda.yml/badge.svg?branch=main)
```

### Comparing `donkeycar-5.0.0/README.md` & `donkeycar-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/benchmarks/tub.py` & `donkeycar-5.1.0/donkeycar/benchmarks/tub.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/benchmarks/tub_v2.py` & `donkeycar-5.1.0/donkeycar/benchmarks/tub_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/config.py` & `donkeycar-5.1.0/donkeycar/config.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/contrib/robohat/code-robocarstore.py` & `donkeycar-5.1.0/donkeycar/contrib/robohat/code-robocarstore.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/contrib/robohat/code.py` & `donkeycar-5.1.0/donkeycar/contrib/robohat/code.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/contrib/robohat/rear_light.py` & `donkeycar-5.1.0/donkeycar/contrib/robohat/rear_light.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/geom.py` & `donkeycar-5.1.0/donkeycar/geom.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/gym/gym_real.py` & `donkeycar-5.1.0/donkeycar/gym/gym_real.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/gym/remote_controller.py` & `donkeycar-5.1.0/donkeycar/gym/remote_controller.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/la.py` & `donkeycar-5.1.0/donkeycar/la.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/base.py` & `donkeycar-5.1.0/donkeycar/management/base.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/graph.py` & `donkeycar-5.1.0/donkeycar/management/graph.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/joystick_creator.py` & `donkeycar-5.1.0/donkeycar/management/joystick_creator.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/kivy_ui.py` & `donkeycar-5.1.0/donkeycar/management/kivy_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     def read_file(self):
         if os.path.exists(self.file_path):
             with open(self.file_path) as f:
                 data = yaml.load(f, Loader=yaml.FullLoader)
                 Logger.info(f'Donkeyrc: Donkey file {self.file_path} loaded.')
                 return data
         else:
-            Logger.warn(f'Donkeyrc: Donkey file {self.file_path} does not '
+            Logger.warning(f'Donkeyrc: Donkey file {self.file_path} does not '
                         f'exist.')
             return {}
 
     def write_file(self):
         if os.path.exists(self.file_path):
             Logger.info(f'Donkeyrc: Donkey file {self.file_path} updated.')
         with open(self.file_path, mode='w') as f:
```

### Comparing `donkeycar-5.0.0/donkeycar/management/makemovie.py` & `donkeycar-5.1.0/donkeycar/management/makemovie.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/tub.py` & `donkeycar-5.1.0/donkeycar/management/tub.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/tub_web/base.html` & `donkeycar-5.1.0/donkeycar/management/tub_web/base.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/tub_web/tub.html` & `donkeycar-5.1.0/donkeycar/management/tub_web/tub.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/management/ui.kv` & `donkeycar-5.1.0/donkeycar/management/ui.kv`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     Label:
         id: value_label
         text_size: self.size
         halign: 'right'
         valign: 'middle'
         font_size: 14 if platform == 'linux' else 28
         size_hint_x: 0.8
-        padding_x: 10
+        padding: 10, 0
         canvas.before:
             Color:
                 rgba: 0.14, 0.15, 0.22, 1
             Rectangle:
                 pos: self.pos
                 size: self.size
     ProgressBar:
```

### Comparing `donkeycar-5.0.0/donkeycar/memory.py` & `donkeycar-5.1.0/donkeycar/memory.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/actuator.py` & `donkeycar-5.1.0/donkeycar/parts/actuator.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from donkeycar.utils import clamp
 
 logger = logging.getLogger(__name__)
 
 try:
     import RPi.GPIO as GPIO
 except ImportError as e:
-    logger.warn(f"RPi.GPIO was not imported. {e}")
+    logger.warning(f"RPi.GPIO was not imported. {e}")
     globals()["GPIO"] = None
 
 from donkeycar.parts.pins import OutputPin, PwmPin, PinState
 from donkeycar.utilities.deprecated import deprecated
 
 logger = logging.getLogger(__name__)
 
@@ -796,18 +796,18 @@
     def run(self, throttle:float) -> None:
         """
         Update the speed of the motor
         :param throttle:float throttle value in range -1 to 1,
                         where 1 is full forward and -1 is full backwards.
         """
         if throttle is None:
-            logger.warn("TwoWheelSteeringThrottle throttle is None")
+            logger.warning("TwoWheelSteeringThrottle throttle is None")
             return
         if throttle > 1 or throttle < -1:
-            logger.warn( f"TwoWheelSteeringThrottle throttle is {throttle}, but it must be between 1(forward) and -1(reverse)")
+            logger.warning( f"TwoWheelSteeringThrottle throttle is {throttle}, but it must be between 1(forward) and -1(reverse)")
             throttle = clamp(throttle, -1, 1)
         
         self.speed = throttle
         self.throttle = dk.utils.map_range_float(throttle, -1, 1, -self.max_duty, self.max_duty)
         if self.throttle > self.zero_throttle:
             self.pwm_pin.duty_cycle(self.throttle)
             self.pin_backward.output(PinState.LOW)
@@ -839,24 +839,24 @@
                         where 1 is full forward and -1 is full backwards.
         :param steering:float steering value in range -1 to 1,
                         where -1 is full left and 1 is full right.
         :return: tuple of left motor and right motor throttle values in range -1 to 1
                  where 1 is full forward and -1 is full backwards.
         """
         if throttle is None:
-            logger.warn("TwoWheelSteeringThrottle throttle is None")
+            logger.warning("TwoWheelSteeringThrottle throttle is None")
             return
         if steering is None:
-            logger.warn("TwoWheelSteeringThrottle steering is None")
+            logger.warning("TwoWheelSteeringThrottle steering is None")
             return
         if throttle > 1 or throttle < -1:
-            logger.warn( f"TwoWheelSteeringThrottle throttle is {throttle}, but it must be between 1(forward) and -1(reverse)")
+            logger.warning( f"TwoWheelSteeringThrottle throttle is {throttle}, but it must be between 1(forward) and -1(reverse)")
             throttle = clamp(throttle, -1, 1)
         if steering > 1 or steering < -1:
-            logger.warn( f"TwoWheelSteeringThrottle steering is {steering}, but it must be between 1(right) and -1(left)")
+            logger.warning( f"TwoWheelSteeringThrottle steering is {steering}, but it must be between 1(right) and -1(left)")
             steering = clamp(steering, -1, 1)
 
         left_motor_speed = throttle
         right_motor_speed = throttle
 
         if steering < 0:
             left_motor_speed *= (1.0 - (-steering))
@@ -916,18 +916,18 @@
     def run(self, throttle:float) -> None:
         """
         Update the speed of the motor
         :param throttle:float throttle value in range -1 to 1,
                         where 1 is full forward and -1 is full backwards.
         """
         if throttle is None:
-            logger.warn("TwoWheelSteeringThrottle throttle is None")
+            logger.warning("TwoWheelSteeringThrottle throttle is None")
             return
         if throttle > 1 or throttle < -1:
-            logger.warn( f"TwoWheelSteeringThrottle throttle is {throttle}, but it must be between 1(forward) and -1(reverse)")
+            logger.warning( f"TwoWheelSteeringThrottle throttle is {throttle}, but it must be between 1(forward) and -1(reverse)")
             throttle = clamp(throttle, -1, 1)
 
         self.speed = throttle
         self.throttle = dk.utils.map_range_float(throttle, -1, 1, -self.max_duty, self.max_duty)
         
         if self.throttle > self.zero_throttle:
             self.pin_backward.duty_cycle(0)
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/behavior.py` & `donkeycar-5.1.0/donkeycar/parts/behavior.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/camera.py` & `donkeycar-5.1.0/donkeycar/parts/camera.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/controller.py` & `donkeycar-5.1.0/donkeycar/parts/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         a path in the linux device tree.
         """
         try:
             from fcntl import ioctl
         except ModuleNotFoundError:
             self.num_axes = 0
             self.num_buttons = 0
-            logger.warn("no support for fnctl module. joystick not enabled.")
+            logger.warning("no support for fnctl module. joystick not enabled.")
             return False
 
         if not os.path.exists(self.dev_fn):
-            logger.warn(f"{self.dev_fn} is missing")
+            logger.warning(f"{self.dev_fn} is missing")
             return False
 
         '''
         call once to setup connection to device and map buttons
         '''
         # Open the joystick device.
         logger.info(f'Opening %s... {self.dev_fn}')
@@ -961,15 +961,15 @@
                 logger.debug(f"JoystickController::on_throttle_changes() setting recording = {self.recording}")
 
 
     def emergency_stop(self):
         '''
         initiate a series of steps to try to stop the vehicle as quickly as possible
         '''
-        logger.warn('E-Stop!!!')
+        logger.warning('E-Stop!!!')
         self.mode = "user"
         self.recording = False
         self.constant_throttle = False
         self.estop_state = self.ES_START
         self.throttle = 0.0
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/coral.py` & `donkeycar-5.1.0/donkeycar/parts/coral.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/cv.py` & `donkeycar-5.1.0/donkeycar/parts/cv.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/datastore.py` & `donkeycar-5.1.0/donkeycar/parts/datastore.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/datastore_v2.py` & `donkeycar-5.1.0/donkeycar/parts/datastore_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/dgym.py` & `donkeycar-5.1.0/donkeycar/parts/dgym.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/encoder.py` & `donkeycar-5.1.0/donkeycar/parts/encoder.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/explode.py` & `donkeycar-5.1.0/donkeycar/parts/explode.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/fast_stretch.py` & `donkeycar-5.1.0/donkeycar/parts/fast_stretch.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/fastai.py` & `donkeycar-5.1.0/donkeycar/parts/fastai.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,19 +154,18 @@
         """
         trains the model
         """
         assert isinstance(self.interpreter, FastAIInterpreter)
         model = self.interpreter.model
 
         dataLoader = DataLoaders.from_dsets(train_data, validation_data, bs=batch_size, shuffle=False)
-        if torch.cuda.is_available():
-            dataLoader.cuda()
+        # old way of enabling gpu now crashes with torch 2.1.*
+        # if torch.cuda.is_available():
+        #     dataLoader.cuda()
 
-        #dataLoaderTest = self.dataBlock.dataloaders.test_dl(validation_data, with_labels=True)
-        #print(dataLoader.train[0])
 
         callbacks = [
             EarlyStoppingCallback(monitor='valid_loss',
                                   patience=patience,
                                   min_delta=min_delta),
             SaveModelCallback(monitor='valid_loss',
                               every_epoch=False
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/file_watcher.py` & `donkeycar-5.1.0/donkeycar/parts/file_watcher.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/fps.py` & `donkeycar-5.1.0/donkeycar/parts/fps.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/gps.py` & `donkeycar-5.1.0/donkeycar/parts/gps.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/graph.py` & `donkeycar-5.1.0/donkeycar/parts/graph.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/image.py` & `donkeycar-5.1.0/donkeycar/parts/image.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/image_transformations.py` & `donkeycar-5.1.0/donkeycar/parts/image_transformations.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/imu.py` & `donkeycar-5.1.0/donkeycar/parts/imu.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/interpreter.py` & `donkeycar-5.1.0/donkeycar/parts/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,20 +343,20 @@
             logger.info(f'Finished loading TensorRT model.')
         except Exception as e:
             logger.error(f'Could not load TensorRT model because: {e}')
 
     def predict_from_dict(self, input_dict):
         for k, v in input_dict.items():
             input_dict[k] = self.expand_and_convert(v)
-        out_dict = self.graph_func(**input_dict)
+        out_list = self.graph_func(**input_dict)
         # Squeeze here because we send a batch of size one, so pick first
         # element. To return the order of outputs as defined in the model we
         # need to iterate through the model's output shapes here
-        outputs = [out_dict[k].numpy().squeeze(axis=0) for k in
-                   self.output_keys]
+        outputs = [k.numpy().squeeze(axis=0) for k in out_list]
+
         # don't return list if output is 1d
         return outputs if len(outputs) > 1 else outputs[0]
 
     @staticmethod
     def expand_and_convert(arr):
         """ Helper function. """
         # expand each input to shape from [x, y, z] to [1, x, y, z] and
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/keras.py` & `donkeycar-5.1.0/donkeycar/parts/keras.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/kinematics.py` & `donkeycar-5.1.0/donkeycar/parts/kinematics.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,15 +578,15 @@
                 negative radians is a right turn
         """
         if not is_number_type(steering):
             logger.error("steering must be a number")
             return 0
 
         if steering > 1 or steering < -1:
-            logger.warn(f"steering = {steering}, but must be between 1(right) and -1(left)")
+            logger.warning(f"steering = {steering}, but must be between 1(right) and -1(left)")
 
         steering = clamp(steering, -1, 1)
         
         s = sign(steering)
         steering = abs(steering)
         if steering <= self.steering_zero:
             return 0.0
@@ -628,22 +628,22 @@
         @Param steering:float -1 to 1, -1 full left, 0 straight, 1 is full right
         @Param steering_zero:float values abs(steering) <= steering_zero are considered zero.
         """
         if not is_number_type(throttle):
             logger.error("throttle must be a number")
             return 0, 0
         if throttle > 1 or throttle < -1:
-            logger.warn(f"throttle = {throttle}, but must be between 1(right) and -1(left)")
+            logger.warning(f"throttle = {throttle}, but must be between 1(right) and -1(left)")
         throttle = clamp(throttle, -1, 1)
 
         if not is_number_type(steering):
             logger.error("steering must be a number")
             return 0, 0
         if steering > 1 or steering < -1:
-            logger.warn(f"steering = {steering}, but must be between 1(right) and -1(left)")
+            logger.warning(f"steering = {steering}, but must be between 1(right) and -1(left)")
         steering = clamp(steering, -1, 1)
 
         left_throttle = throttle
         right_throttle = throttle
  
         if steering < -steering_zero:
             left_throttle *= (1.0 + steering)
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/launch.py` & `donkeycar-5.1.0/donkeycar/parts/launch.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/led_status.py` & `donkeycar-5.1.0/donkeycar/parts/led_status.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/leopard_imaging.py` & `donkeycar-5.1.0/donkeycar/parts/leopard_imaging.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/lidar.py` & `donkeycar-5.1.0/donkeycar/parts/lidar.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/line_follower.py` & `donkeycar-5.1.0/donkeycar/parts/line_follower.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/logger.py` & `donkeycar-5.1.0/donkeycar/parts/logger.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/network.py` & `donkeycar-5.1.0/donkeycar/parts/network.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/object_detector/stop_sign_detector.py` & `donkeycar-5.1.0/donkeycar/parts/object_detector/stop_sign_detector.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/odometer.py` & `donkeycar-5.1.0/donkeycar/parts/odometer.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/oled.py` & `donkeycar-5.1.0/donkeycar/parts/oled.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/path.py` & `donkeycar-5.1.0/donkeycar/parts/path.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/perfmon.py` & `donkeycar-5.1.0/donkeycar/parts/perfmon.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/pigpio_enc.py` & `donkeycar-5.1.0/donkeycar/parts/pigpio_enc.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/pins.py` & `donkeycar-5.1.0/donkeycar/parts/pins.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 try:
     import RPi.GPIO as GPIO
     # lookups to convert abstact api to GPIO values
     gpio_pin_edge = [None, GPIO.RISING, GPIO.FALLING, GPIO.BOTH]
     gpio_pin_pull = [None, GPIO.PUD_OFF, GPIO.PUD_DOWN, GPIO.PUD_UP]
     gpio_pin_scheme = {PinScheme.BOARD: GPIO.BOARD, PinScheme.BCM: GPIO.BCM}
 except ImportError:
-    logger.warn("RPi.GPIO was not imported.")
+    logger.warning("RPi.GPIO was not imported.")
     globals()["GPIO"] = None
 
 
 def gpio_fn(pin_scheme:int, fn:Callable[[], Any]):
     """
     Convenience method to enforce the desired GPIO pin scheme
     before calling a GPIO function.
@@ -749,15 +749,15 @@
 
 # pigpio is an optional install
 try:
     import pigpio
     pigpio_pin_edge = [None, pigpio.RISING_EDGE, pigpio.FALLING_EDGE, pigpio.EITHER_EDGE]
     pigpio_pin_pull = [None, pigpio.PUD_OFF, pigpio.PUD_DOWN, pigpio.PUD_UP]
 except ImportError:
-    logger.warn("pigpio was not imported.")
+    logger.warning("pigpio was not imported.")
     globals()["pigpio"] = None
 
 
 class InputPinPigpio(InputPin):
     def __init__(self, pin_number: int, pull: int = PinPull.PULL_NONE, pgpio=None) -> None:
         """
         Input pin ttl HIGH/LOW using PiGPIO library
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/pose.py` & `donkeycar-5.1.0/donkeycar/parts/pose.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/pytorch/ResNet18.py` & `donkeycar-5.1.0/donkeycar/parts/pytorch/ResNet18.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/pytorch/torch_data.py` & `donkeycar-5.1.0/donkeycar/parts/pytorch/torch_data.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/pytorch/torch_train.py` & `donkeycar-5.1.0/donkeycar/parts/pytorch/torch_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         from pytorch_lightning.loggers import TensorBoardLogger
 
         # Create Tensorboard logger
         logger = TensorBoardLogger('tb_logs', name=model_name)
 
     if cfg.PRINT_MODEL_SUMMARY:
         summarize(model)
-    trainer = pl.Trainer(gpus=gpus, logger=logger, max_epochs=cfg.MAX_EPOCHS,
-                         default_root_dir=output_dir)
+    trainer = pl.Trainer(accelerator='cpu', logger=logger,
+                         max_epochs=cfg.MAX_EPOCHS, default_root_dir=output_dir)
 
     data_module = TorchTubDataModule(cfg, tub_paths)
     trainer.fit(model, data_module)
 
     if is_torch_model:
         checkpoint_model_path = f'{os.path.splitext(output_path)[0]}.ckpt'
         trainer.save_checkpoint(checkpoint_model_path)
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/pytorch/torch_utils.py` & `donkeycar-5.1.0/donkeycar/parts/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/realsense2.py` & `donkeycar-5.1.0/donkeycar/parts/realsense2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/realsense435i.py` & `donkeycar-5.1.0/donkeycar/parts/realsense435i.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/robohat.py` & `donkeycar-5.1.0/donkeycar/parts/robohat.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/ros.py` & `donkeycar-5.1.0/donkeycar/parts/ros.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/salient.py` & `donkeycar-5.1.0/donkeycar/parts/salient.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/serial_controller.py` & `donkeycar-5.1.0/donkeycar/parts/serial_controller.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/serial_port.py` & `donkeycar-5.1.0/donkeycar/parts/serial_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         try:
             input = ''
             waiting = self.buffered() >= count
             if waiting:   # read the serial port and see if there's any data there
                 input = self.ser.read(count)
             return (waiting, input)
         except (serial.serialutil.SerialException, TypeError):
-            logger.warn("failed reading bytes from serial port")
+            logger.warning("failed reading bytes from serial port")
             return (False, b'')
 
     def read(self, count:int=0) -> Tuple[bool, str]:
         """
         if there are characters waiting, 
         then read them from the serial port
         bytes: number of bytes to read 
@@ -131,30 +131,30 @@
             input = ''
             waiting = self.buffered() > 0
             if waiting:   # read the serial port and see if there's any data there
                 buffer = self.ser.readline()
                 input = buffer.decode(self.charset)
             return (waiting, input)
         except (serial.serialutil.SerialException, TypeError):
-            logger.warn("failed reading line from serial port")
+            logger.warning("failed reading line from serial port")
             return (False, "")
         except UnicodeDecodeError:
             # the first read often includes mis-framed garbase
-            logger.warn("failed decoding unicode line from serial port")
+            logger.warning("failed decoding unicode line from serial port")
             return (False, "")
 
     def writeBytes(self, value:bytes):
         """
         write byte string to serial port
         """
         if self.ser is not None and self.ser.is_open:
             try:
                 self.ser.write(value)  
             except (serial.serialutil.SerialException, TypeError):
-                logger.warn("Can't write to serial port")
+                logger.warning("Can't write to serial port")
 
     def write(self, value:str):
         """
         write string to serial port
         """
         self.writeBytes(value.encode())
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/simulation.py` & `donkeycar-5.1.0/donkeycar/parts/simulation.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/sombrero.py` & `donkeycar-5.1.0/donkeycar/parts/sombrero.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/tachometer.py` & `donkeycar-5.1.0/donkeycar/parts/tachometer.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         self.counter = 0
         self._cb_counter = 0
         self.direction = 0
         self.pin = gpio_pin
         self.debounce_ns:int = debounce_ns
         self.debounce_time:int = 0
         if self.debounce_ns > 0:
-            logger.warn("GpioEncoder debounce_ns will be ignored.")
+            logger.warning("GpioEncoder debounce_ns will be ignored.")
         self.lock = threading.Lock()
 
     def _cb(self):
         """
         Callback routine called by GPIO when a tick is detected
         :pin_number: int the pin number that generated the interrupt.
         :pin_state: int the state of the pin
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/teensy.py` & `donkeycar-5.1.0/donkeycar/parts/teensy.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/telemetry.py` & `donkeycar-5.1.0/donkeycar/parts/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import queue
 import time
 import json
 import logging
 import numpy as np
 from logging import StreamHandler
 from paho.mqtt.client import Client as MQTTClient
+from paho.mqtt.enums import CallbackAPIVersion
 
 logger = logging.getLogger()
 
 LOG_MQTT_KEY = 'log/default'
 
 
 class MqttTelemetry(StreamHandler):
@@ -36,15 +37,15 @@
         self._step_inputs = cfg.TELEMETRY_DEFAULT_INPUTS.split(',')
         self._step_types = cfg.TELEMETRY_DEFAULT_TYPES.split(',')
         self._total_updates = 0
         self._donkey_name = os.environ.get('DONKEY_NAME', cfg.TELEMETRY_DONKEY_NAME)
         self._mqtt_broker = os.environ.get('DONKEY_MQTT_BROKER', cfg.TELEMETRY_MQTT_BROKER_HOST)  # 'iot.eclipse.org'
         self._topic = cfg.TELEMETRY_MQTT_TOPIC_TEMPLATE % self._donkey_name
         self._use_json_format = cfg.TELEMETRY_MQTT_JSON_ENABLE
-        self._mqtt_client = MQTTClient()
+        self._mqtt_client = MQTTClient(callback_api_version=CallbackAPIVersion.VERSION2)
         self._mqtt_client.connect(self._mqtt_broker, cfg.TELEMETRY_MQTT_BROKER_PORT)
         self._mqtt_client.loop_start()
         self._on = True
         if cfg.TELEMETRY_LOGGING_ENABLE:
             self.setLevel(logging.getLevelName(cfg.TELEMETRY_LOGGING_LEVEL))
             self.setFormatter(logging.Formatter(cfg.TELEMETRY_LOGGING_FORMAT))
             logger.addHandler(self)
```

### Comparing `donkeycar-5.0.0/donkeycar/parts/text_writer.py` & `donkeycar-5.1.0/donkeycar/parts/text_writer.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/tfmini.py` & `donkeycar-5.1.0/donkeycar/parts/tfmini.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/throttle_filter.py` & `donkeycar-5.1.0/donkeycar/parts/throttle_filter.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/transform.py` & `donkeycar-5.1.0/donkeycar/parts/transform.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/tub_v2.py` & `donkeycar-5.1.0/donkeycar/parts/tub_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/velocity.py` & `donkeycar-5.1.0/donkeycar/parts/velocity.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/voice_control/alexa.py` & `donkeycar-5.1.0/donkeycar/parts/voice_control/alexa.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/base.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/base.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/base_fpv.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/base_fpv.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/calibrate.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/calibrate.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/home.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/home.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/session.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/session.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/css/bootstrap.min.css` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.ttf` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/js/bootstrap.min.js` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/bootstrap/3.3.7/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/donkeycar-logo-sideways.png` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/donkeycar-logo-sideways.png`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/img_placeholder.jpg` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/img_placeholder.jpg`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/jquery-3.1.1.min.js` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/jquery-3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/main.js` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/main.js`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/nipple.js` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/nipple.js`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/style.css` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/static/ui/1.12.1/jquery-ui.min.js` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/static/ui/1.12.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/vehicle.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/vehicle.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/templates/wsTest.html` & `donkeycar-5.1.0/donkeycar/parts/web_controller/templates/wsTest.html`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/parts/web_controller/web.py` & `donkeycar-5.1.0/donkeycar/parts/web_controller/web.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/pipeline/augmentations.py` & `donkeycar-5.1.0/donkeycar/pipeline/augmentations.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/pipeline/database.py` & `donkeycar-5.1.0/donkeycar/pipeline/database.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/pipeline/sequence.py` & `donkeycar-5.1.0/donkeycar/pipeline/sequence.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/pipeline/training.py` & `donkeycar-5.1.0/donkeycar/pipeline/training.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/pipeline/types.py` & `donkeycar-5.1.0/donkeycar/pipeline/types.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/arduino_drive.py` & `donkeycar-5.1.0/donkeycar/templates/arduino_drive.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/basic.py` & `donkeycar-5.1.0/donkeycar/templates/basic.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/calibrate.py` & `donkeycar-5.1.0/donkeycar/templates/calibrate.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/calibration_odometry.json` & `donkeycar-5.1.0/donkeycar/templates/calibration_odometry.json`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_arduino_drive.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_arduino_drive.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_basic.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_basic.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_complete.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_complete.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_cv_control.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_cv_control.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_path_follow.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_path_follow.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_simulator.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_simulator.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cfg_square.py` & `donkeycar-5.1.0/donkeycar/templates/cfg_square.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/complete.py` & `donkeycar-5.1.0/donkeycar/templates/complete.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/cv_control.py` & `donkeycar-5.1.0/donkeycar/templates/cv_control.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/just_drive.py` & `donkeycar-5.1.0/donkeycar/templates/just_drive.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/path_follow.py` & `donkeycar-5.1.0/donkeycar/templates/path_follow.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/simulator.py` & `donkeycar-5.1.0/donkeycar/templates/simulator.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/square.py` & `donkeycar-5.1.0/donkeycar/templates/square.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/templates/train.py` & `donkeycar-5.1.0/donkeycar/templates/train.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/setup.py` & `donkeycar-5.1.0/donkeycar/tests/setup.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_catalog_v2.py` & `donkeycar-5.1.0/donkeycar/tests/test_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_circular_buffer.py` & `donkeycar-5.1.0/donkeycar/tests/test_circular_buffer.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_controller.py` & `donkeycar-5.1.0/donkeycar/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_datastore_v2.py` & `donkeycar-5.1.0/donkeycar/tests/test_datastore_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_keras.py` & `donkeycar-5.1.0/donkeycar/tests/test_keras.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,12 +74,12 @@
     if k_tflite:
         out2 = k_tflite.run(*args)
         assert out2 == approx(out1, rel=TOLERANCE, abs=TOLERANCE)
     if k_trt:
         # lstm cells are not yet supported in tensor RT
         out3 = k_trt.run(*args)
         assert out3 == approx(out1, rel=TOLERANCE, abs=TOLERANCE)
-    print("\n", out1, out2, out3)
+    print('keras:', out1, 'tflite:', out2, 'trt:', out3)
```

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_kinematics.py` & `donkeycar-5.1.0/donkeycar/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_launch.py` & `donkeycar-5.1.0/donkeycar/tests/test_launch.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_lidar.py` & `donkeycar-5.1.0/donkeycar/tests/test_lidar.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_memory.py` & `donkeycar-5.1.0/donkeycar/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_odometer.py` & `donkeycar-5.1.0/donkeycar/tests/test_odometer.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_path.py` & `donkeycar-5.1.0/donkeycar/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_pipeline.py` & `donkeycar-5.1.0/donkeycar/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_robohat.py` & `donkeycar-5.1.0/donkeycar/tests/test_robohat.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_scripts.py` & `donkeycar-5.1.0/donkeycar/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_seekable_v2.py` & `donkeycar-5.1.0/donkeycar/tests/test_seekable_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_tachometer.py` & `donkeycar-5.1.0/donkeycar/tests/test_tachometer.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_telemetry.py` & `donkeycar-5.1.0/donkeycar/tests/test_telemetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import time
 from unittest import mock
 from paho.mqtt.client import Client
+from paho.mqtt.enums import CallbackAPIVersion
+
 import donkeycar.templates.cfg_complete as cfg
 from donkeycar.parts.telemetry import MqttTelemetry
-import pytest
 from random import randint
 
 
 def test_mqtt_telemetry():
 
     cfg.TELEMETRY_DEFAULT_INPUTS = 'pilot/angle,pilot/throttle'
     cfg.TELEMETRY_DONKEY_NAME = 'test{}'.format(randint(0, 1000))
     cfg.TELEMETRY_MQTT_JSON_ENABLE = True
 
     # Create receiver
-    sub = Client(clean_session=True)
-
-    # def on_message(client, userdata, message):
-    #     data = message.payload
-    #     print(message)
+    sub = Client(callback_api_version=CallbackAPIVersion.VERSION2,
+                 clean_session=True)
 
     on_message_mock = mock.Mock()
     sub.on_message = on_message_mock
     sub.connect(cfg.TELEMETRY_MQTT_BROKER_HOST)
     sub.loop_start()
     name = "donkey/%s/#" % cfg.TELEMETRY_DONKEY_NAME
     sub.subscribe(name)
```

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_template.py` & `donkeycar-5.1.0/donkeycar/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_torch.py` & `donkeycar-5.1.0/donkeycar/tests/test_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         print('Using CUDA')
         gpus = -1
     else:
         print('Not using CUDA')
         gpus = 0
 
     # Overfit the data
-    trainer = pl.Trainer(gpus=gpus, overfit_batches=2, max_epochs=30)
+    trainer = pl.Trainer(accelerator='cpu', overfit_batches=2, max_epochs=30)
     trainer.fit(model, data_module)
     final_loss = model.loss_history[-1]
     assert final_loss < 0.35, \
         f"final_loss of {final_loss} is too high. History: {model.loss_history}"
 
     # Check the batch data makes sense
     for batch in data_module.train_dataloader():
```

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_train.py` & `donkeycar-5.1.0/donkeycar/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_tub_v2.py` & `donkeycar-5.1.0/donkeycar/tests/test_tub_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_tubwriter.py` & `donkeycar-5.1.0/donkeycar/tests/test_tubwriter.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_util_data.py` & `donkeycar-5.1.0/donkeycar/tests/test_util_data.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_vehicle.py` & `donkeycar-5.1.0/donkeycar/tests/test_vehicle.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_web_controller.py` & `donkeycar-5.1.0/donkeycar/tests/test_web_controller.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/tests/test_web_socket.py` & `donkeycar-5.1.0/donkeycar/tests/test_web_socket.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/utilities/circular_buffer.py` & `donkeycar-5.1.0/donkeycar/utilities/circular_buffer.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/utilities/deprecated.py` & `donkeycar-5.1.0/donkeycar/utilities/deprecated.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/utilities/dk_platform.py` & `donkeycar-5.1.0/donkeycar/utilities/dk_platform.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/utils.py` & `donkeycar-5.1.0/donkeycar/utils.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar/vehicle.py` & `donkeycar-5.1.0/donkeycar/vehicle.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar.egg-info/PKG-INFO` & `donkeycar-5.1.0/donkeycar.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 Metadata-Version: 2.1
 Name: donkeycar
-Version: 5.0.0
+Version: 5.1.0
 Summary: Self driving library for python.
 Home-page: https://github.com/autorope/donkeycar
 Author: Will Roscoe, Adam Conway, Tawn Kramer
 License: MIT
 Keywords: selfdriving cars donkeycar diyrobocars
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: <4,>=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: docopt
 Requires-Dist: tornado
 Requires-Dist: requests
 Requires-Dist: PrettyTable
 Requires-Dist: paho-mqtt
 Requires-Dist: simple_pid
 Requires-Dist: progress
-Requires-Dist: typing_extensions
 Requires-Dist: pyfiglet
 Requires-Dist: psutil
 Requires-Dist: pynmea2
 Requires-Dist: pyserial
 Requires-Dist: utm
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Provides-Extra: pi
 Requires-Dist: picamera2; extra == "pi"
 Requires-Dist: Adafruit_PCA9685; extra == "pi"
 Requires-Dist: adafruit-circuitpython-ssd1306; extra == "pi"
 Requires-Dist: adafruit-circuitpython-rplidar; extra == "pi"
 Requires-Dist: RPi.GPIO; extra == "pi"
-Requires-Dist: tensorflow-aarch64==2.9.3; extra == "pi"
+Requires-Dist: tensorflow-aarch64==2.15.*; extra == "pi"
 Requires-Dist: opencv-contrib-python; extra == "pi"
 Provides-Extra: nano
 Requires-Dist: Adafruit_PCA9685; extra == "nano"
 Requires-Dist: adafruit-circuitpython-ssd1306; extra == "nano"
 Requires-Dist: adafruit-circuitpython-rplidar; extra == "nano"
 Requires-Dist: Jetson.GPIO; extra == "nano"
-Requires-Dist: numpy==1.23; extra == "nano"
-Requires-Dist: matplotlib==3.7; extra == "nano"
-Requires-Dist: kivy==2.1; extra == "nano"
+Requires-Dist: numpy==1.23.*; extra == "nano"
+Requires-Dist: matplotlib==3.7.*; extra == "nano"
+Requires-Dist: kivy; extra == "nano"
 Requires-Dist: plotly; extra == "nano"
-Requires-Dist: pandas==2.0; extra == "nano"
+Requires-Dist: pandas==2.0.*; extra == "nano"
 Provides-Extra: pc
-Requires-Dist: tensorflow==2.9; extra == "pc"
+Requires-Dist: tensorflow==2.15.*; extra == "pc"
 Requires-Dist: matplotlib; extra == "pc"
-Requires-Dist: kivy==2.1; extra == "pc"
+Requires-Dist: kivy; extra == "pc"
 Requires-Dist: pandas; extra == "pc"
 Requires-Dist: plotly; extra == "pc"
 Requires-Dist: albumentations; extra == "pc"
 Provides-Extra: macos
-Requires-Dist: tensorflow-macos==2.9; extra == "macos"
+Requires-Dist: tensorflow-macos==2.15.*; extra == "macos"
 Requires-Dist: matplotlib; extra == "macos"
-Requires-Dist: kivy==2.1; extra == "macos"
+Requires-Dist: kivy; extra == "macos"
 Requires-Dist: pandas; extra == "macos"
 Requires-Dist: plotly; extra == "macos"
 Requires-Dist: albumentations; extra == "macos"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: responses; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Provides-Extra: torch
-Requires-Dist: pytorch; extra == "torch"
-Requires-Dist: torchvision==0.12; extra == "torch"
+Requires-Dist: torch==2.1.*; extra == "torch"
+Requires-Dist: pytorch-lightning; extra == "torch"
+Requires-Dist: torchvision; extra == "torch"
 Requires-Dist: torchaudio; extra == "torch"
 Requires-Dist: fastai; extra == "torch"
 
 # Donkeycar: a python self driving library
 
 
 ![Build Status](https://github.com/autorope/donkeycar/actions/workflows/python-package-conda.yml/badge.svg?branch=main)
```

### Comparing `donkeycar-5.0.0/donkeycar.egg-info/SOURCES.txt` & `donkeycar-5.1.0/donkeycar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/donkeycar.egg-info/requires.txt` & `donkeycar-5.1.0/donkeycar.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 docopt
 tornado
 requests
 PrettyTable
 paho-mqtt
 simple_pid
 progress
-typing_extensions
 pyfiglet
 psutil
 pynmea2
 pyserial
 utm
 pandas
 pyyaml
@@ -19,47 +18,48 @@
 [dev]
 pytest
 pytest-cov
 responses
 mypy
 
 [macos]
-tensorflow-macos==2.9
+tensorflow-macos==2.15.*
 matplotlib
-kivy==2.1
+kivy
 pandas
 plotly
 albumentations
 
 [nano]
 Adafruit_PCA9685
 adafruit-circuitpython-ssd1306
 adafruit-circuitpython-rplidar
 Jetson.GPIO
-numpy==1.23
-matplotlib==3.7
-kivy==2.1
+numpy==1.23.*
+matplotlib==3.7.*
+kivy
 plotly
-pandas==2.0
+pandas==2.0.*
 
 [pc]
-tensorflow==2.9
+tensorflow==2.15.*
 matplotlib
-kivy==2.1
+kivy
 pandas
 plotly
 albumentations
 
 [pi]
 picamera2
 Adafruit_PCA9685
 adafruit-circuitpython-ssd1306
 adafruit-circuitpython-rplidar
 RPi.GPIO
-tensorflow-aarch64==2.9.3
+tensorflow-aarch64==2.15.*
 opencv-contrib-python
 
 [torch]
-pytorch
-torchvision==0.12
+torch==2.1.*
+pytorch-lightning
+torchvision
 torchaudio
 fastai
```

### Comparing `donkeycar-5.0.0/scripts/convert_to_tflite.py` & `donkeycar-5.1.0/scripts/convert_to_tflite.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/convert_to_tub_v2.py` & `donkeycar-5.1.0/scripts/convert_to_tub_v2.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/freeze_model.py` & `donkeycar-5.1.0/scripts/freeze_model.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/graph_listener.py` & `donkeycar-5.1.0/scripts/graph_listener.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/hsv_picker.py` & `donkeycar-5.1.0/scripts/hsv_picker.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/multi_train.py` & `donkeycar-5.1.0/scripts/multi_train.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/pigpio_donkey.py` & `donkeycar-5.1.0/scripts/pigpio_donkey.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/preview_augumentations.py` & `donkeycar-5.1.0/scripts/preview_augumentations.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/profile.py` & `donkeycar-5.1.0/scripts/profile.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/profile_coral.py` & `donkeycar-5.1.0/scripts/profile_coral.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/remote_cam_view.py` & `donkeycar-5.1.0/scripts/remote_cam_view.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/remote_cam_view_tcp.py` & `donkeycar-5.1.0/scripts/remote_cam_view_tcp.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/salient_vis_listener.py` & `donkeycar-5.1.0/scripts/salient_vis_listener.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/scripts/tflite_profile.py` & `donkeycar-5.1.0/scripts/tflite_profile.py`

 * *Files identical despite different names*

### Comparing `donkeycar-5.0.0/setup.cfg` & `donkeycar-5.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,31 @@
 long_description_content_type = text/markdown
 keywords = selfdriving cars donkeycar diyrobocars
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Topic :: Scientific/Engineering :: Artificial Intelligence
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find_namespace:
 zip_safe = True
 include_package_data = True
-python_requires = >=3.8,<4
+python_requires = >=3.11.0,<3.12
 install_requires = 
 	numpy
 	pillow
 	docopt
 	tornado
 	requests
 	PrettyTable
 	paho-mqtt
 	simple_pid
 	progress
-	typing_extensions
 	pyfiglet
 	psutil
 	pynmea2
 	pyserial
 	utm
 	pandas
 	pyyaml
@@ -42,48 +40,49 @@
 [options.extras_require]
 pi = 
 	picamera2
 	Adafruit_PCA9685
 	adafruit-circuitpython-ssd1306
 	adafruit-circuitpython-rplidar
 	RPi.GPIO
-	tensorflow-aarch64==2.9.3
+	tensorflow-aarch64==2.15.*
 	opencv-contrib-python
 nano = 
 	Adafruit_PCA9685
 	adafruit-circuitpython-ssd1306
 	adafruit-circuitpython-rplidar
 	Jetson.GPIO
-	numpy==1.23
-	matplotlib==3.7
-	kivy==2.1
+	numpy==1.23.*
+	matplotlib==3.7.*
+	kivy
 	plotly
-	pandas==2.0
+	pandas==2.0.*
 pc = 
-	tensorflow==2.9
+	tensorflow==2.15.*
 	matplotlib
-	kivy==2.1
+	kivy
 	pandas
 	plotly
 	albumentations
 macos = 
-	tensorflow-macos==2.9
+	tensorflow-macos==2.15.*
 	matplotlib
-	kivy==2.1
+	kivy
 	pandas
 	plotly
 	albumentations
 dev = 
 	pytest
 	pytest-cov
 	responses
 	mypy
 torch = 
-	pytorch
-	torchvision==0.12
+	torch==2.1.*
+	pytorch-lightning
+	torchvision
 	torchaudio
 	fastai
 
 [options.package_data]
 * = *.html, *.ini, *.txt, *.kv
 
 [options.entry_points]
```

