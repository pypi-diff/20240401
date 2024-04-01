# Comparing `tmp/yandexcloud-0.98.0.tar.gz` & `tmp/yandexcloud-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandexcloud-0.98.0.tar", last modified: Mon Jul 19 08:51:03 2021, max compression
+gzip compressed data, was "dist/yandexcloud-0.99.0.tar", last modified: Tue Jul 27 07:45:52 2021, max compression
```

## Comparing `yandexcloud-0.98.0.tar` & `yandexcloud-0.99.0.tar`

### file list

```diff
@@ -1,797 +1,799 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/
--rw-r--r--   0 root         (0) root         (0)      264 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1077 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      530 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1203 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      936 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/access/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/access/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21702 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/access/access_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/access/access_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/stt/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/stt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/stt/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/stt/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33534 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/stt/v2/stt_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4984 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4820 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25558 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6987 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31252 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2313 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2818 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4391 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/classification_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/classification_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4296 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/face_detection_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/face_detection_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6001 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/image_copy_search_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/image_copy_search_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4165 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/primitives_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/primitives_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    17089 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/text_detection_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/text_detection_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    27715 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2961 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/vision_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3633 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/api/operation_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/api/operation_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50686 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    62641 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18504 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8481 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    41305 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    12714 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    56264 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   111149 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30528 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3281 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/payload_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/payload_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10504 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    49531 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16533 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4182 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/tls_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/tls_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    50196 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48494 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14567 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7130 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3222 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    30650 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    57513 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20445 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15419 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12213 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48844 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15087 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    42232 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    12329 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3327 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9056 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4886 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    19295 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    53796 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16164 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3286 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9085 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4759 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13715 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/image_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/image_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    45901 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/image_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14045 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/image_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48933 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   136667 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30819 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171571 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   106992 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39405 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9812 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    43705 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14762 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    11060 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    38292 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    12319 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4395 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8717 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4725 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3841 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/blob_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/blob_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6657 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    16562 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6824 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8240 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/ip_permission_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/ip_permission_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    11553 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    58677 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    19585 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8765 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    47919 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22122 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3024 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25731 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16596 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18952 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25410 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10850 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41478 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12236 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4898 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    45328 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2961 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27437 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    80059 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    19442 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4814 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    40648 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25440 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8153 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3875 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9750 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5129 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18503 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    35793 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10405 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6620 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/node_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2838 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9451 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    31777 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11901 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/dns/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/dns/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dns/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14298 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    63230 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    25471 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/endpoint/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/endpoint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2884 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8655 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4791 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4058 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28868 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11954 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4900 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    31450 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13154 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9981 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/iam_token_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4843 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7209 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/key_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    31124 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/key_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11657 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/key_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2732 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/role_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/role_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9126 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/role_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4554 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/role_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4824 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    35177 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18212 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12947 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4316 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3187 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4553 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3259 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/iot/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6507 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_data_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3096 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_data_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20538 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    75241 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    25554 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6608 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3146 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    17622 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    79410 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27977 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/k8s/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45954 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    86154 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    19172 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    14014 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/maintenance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    34046 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    61676 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14039 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48989 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6779 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6953 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2835 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/kms/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30971 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9175 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20651 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    73017 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28381 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11012 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/health_check_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/health_check_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29420 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    92193 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27604 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10410 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    49878 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16364 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5875 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4838 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2954 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    16231 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    77237 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28847 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/logging/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16678 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_entry_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_entry_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10458 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    53343 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    23464 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9647 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_ingestion_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2916 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_ingestion_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    14142 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_reading_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2876 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_reading_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5584 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_resource_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/logging/v1/log_resource_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8837 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3306 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10988 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/usage_record_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/usage_record_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5336 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9804 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5017 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    59126 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   221733 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    60171 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127100 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/config/clickhouse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/config/clickhouse_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4676 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    21534 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9134 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5550 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    30243 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10817 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12238 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/maintenance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5073 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28984 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10623 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3968 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9923 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5311 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    92472 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    41024 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14446 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3866 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/version_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/version_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7120 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2981 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16966 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    32902 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14690 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    43260 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   113634 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28117 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7043 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/config/elasticsearch_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/config/elasticsearch_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4017 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10131 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5368 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5200 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    27381 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10435 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71851 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    82726 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    23705 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3633 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3885 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9805 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5176 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    45336 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    27144 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10191 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9735 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    39267 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13842 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7417 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13800 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6832 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   100270 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   243346 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    49675 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49439 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb3_6_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb3_6_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48785 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_0_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_0_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48785 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_2_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_2_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48785 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_4_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_4_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4630 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    21317 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8744 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12139 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/maintenance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3918 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9766 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5248 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8028 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    39352 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14010 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4997 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9697 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    44988 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   148656 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38244 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60337 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/mysql5_7_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/mysql5_7_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    58885 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/mysql8_0_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/mysql8_0_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4580 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    21164 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8612 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12074 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/maintenance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3885 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9808 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5158 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24009 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    41335 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13845 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5078 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9904 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4944 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    36245 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   110668 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29401 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7648 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/config/mysql5_7_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/config/mysql5_7_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4666 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    21527 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8767 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3958 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9997 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5263 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13043 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    39844 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14075 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4843 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9914 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5017 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    75566 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   176341 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39015 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68372 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host10_1c_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host10_1c_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    67655 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host10_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host10_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    67664 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host11_1c_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host11_1c_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    66953 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host11_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host11_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    67664 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host12_1c_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host12_1c_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    66953 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host12_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host12_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    66953 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host13_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host13_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    58943 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host9_6_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host9_6_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   110897 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_1c_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_1c_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   108309 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   115327 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_1c_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_1c_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   114089 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   118465 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_1c_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_1c_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   117183 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   127212 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql13_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql13_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    83725 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql9_6_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql9_6_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10960 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28153 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10680 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12238 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/maintenance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3968 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10004 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5311 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    22979 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    42493 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14181 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5240 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9590 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    45409 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   163136 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    45584 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12730 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis5_0_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis5_0_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12732 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis6_0_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis6_0_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12732 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis6_2_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis6_2_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    12074 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/maintenance_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3885 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9448 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5170 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5301 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9875 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4953 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    40400 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   111932 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27660 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/config/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18106 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/config/sqlserver2016sp2_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/config/sqlserver2016sp2_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4670 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29992 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10630 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3964 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9973 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5242 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    11025 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    39735 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14085 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/operation/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/operation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7838 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/operation/operation_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/operation/operation_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6411 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/operation/operation_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4698 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/operation/operation_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/quota/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/quota/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8337 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/quota/quota_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/quota/quota_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/reference/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/reference/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5845 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/reference/reference_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/reference/reference_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4203 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29637 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16147 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9124 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    41778 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18049 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14557 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    60281 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24679 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36166 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   114725 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    40588 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14429 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    42652 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18196 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9908 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/predicate_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    63095 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    46953 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16409 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9111 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/validation_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/validation_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16970 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    47552 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15536 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7485 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    46388 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15738 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13396 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    43725 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14193 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25271 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    65985 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    17864 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13350 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    52993 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15641 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ydb/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28465 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18682 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8137 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    34017 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    66885 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16865 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2798 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8855 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4641 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3322 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9401 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4907 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3347 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9141 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4791 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandexcloud/
--rw-r--r--   0 root         (0) root         (0)      269 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3567 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_auth_fabric.py
--rw-r--r--   0 root         (0) root         (0)     2636 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_auth_plugin.py
--rw-r--r--   0 root         (0) root         (0)      563 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_backoff.py
--rw-r--r--   0 root         (0) root         (0)     1914 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_channels.py
--rw-r--r--   0 root         (0) root         (0)     3392 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_helpers.py
--rw-r--r--   0 root         (0) root         (0)     3908 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandexcloud/_operation_waiter.py
--rw-r--r--   0 root         (0) root         (0)     6398 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandexcloud/_retry_interceptor.py
--rw-r--r--   0 root         (0) root         (0)     3793 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_sdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandexcloud/_wrappers/
--rw-r--r--   0 root         (0) root         (0)      172 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/_wrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandexcloud/_wrappers/dataproc/
--rw-r--r--   0 root         (0) root         (0)    29150 2021-07-19 08:50:48.000000 yandexcloud-0.98.0/yandexcloud/_wrappers/dataproc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2021-07-12 09:52:21.000000 yandexcloud-0.98.0/yandexcloud/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandexcloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)      530 2021-07-19 08:51:02.000000 yandexcloud-0.98.0/yandexcloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    33976 2021-07-19 08:51:03.000000 yandexcloud-0.98.0/yandexcloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-19 08:51:02.000000 yandexcloud-0.98.0/yandexcloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-12 09:52:39.000000 yandexcloud-0.98.0/yandexcloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      108 2021-07-19 08:51:02.000000 yandexcloud-0.98.0/yandexcloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2021-07-19 08:51:02.000000 yandexcloud-0.98.0/yandexcloud.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/
+-rw-r--r--   0 root         (0) root         (0)      264 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1077 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      530 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1203 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      936 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/access/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/access/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21702 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/access/access_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/access/access_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/stt/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/stt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/stt/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/stt/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33534 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/stt/v2/stt_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4820 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25558 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6987 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31252 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2818 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/classification_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/classification_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/face_detection_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/face_detection_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6001 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/image_copy_search_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/image_copy_search_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/primitives_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/primitives_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    17089 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/text_detection_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/text_detection_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    27715 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/vision_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/api/operation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/api/operation_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53094 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    62641 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18504 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8481 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    41305 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    12714 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    56264 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   111149 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30528 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/payload_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/payload_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    49531 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4182 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/tls_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/tls_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    50196 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48494 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14567 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7130 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    30650 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    57513 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20445 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15419 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12213 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48844 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15087 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    42232 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    12329 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9056 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4886 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    19295 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    53796 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16164 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4759 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13715 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/image_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/image_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    45901 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/image_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14045 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/image_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48933 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   136667 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30819 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171571 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   106992 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39405 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9812 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    43705 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14762 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    38292 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    12319 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4395 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8717 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4725 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3841 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/blob_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/blob_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    16562 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6824 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8240 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/ip_permission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/ip_permission_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    11553 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    58677 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    19585 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8765 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    47919 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22122 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25731 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16596 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18952 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25410 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10850 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41478 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12236 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    45328 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27437 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    80059 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    19442 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    40648 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25440 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8153 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18503 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    35793 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10405 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/app_token_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6620 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/node_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12371 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    40143 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15693 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/dns/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/dns/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dns/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14298 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    63230 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    25471 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/endpoint/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/endpoint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8655 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28868 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11954 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4900 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    31450 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13154 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9981 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/iam_token_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/key_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    31124 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/key_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11657 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/key_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/role_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/role_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9126 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/role_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4554 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/role_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    35177 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18212 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4316 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/iot/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6507 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_data_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_data_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20538 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    75241 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    25554 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6608 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    79410 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27977 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/k8s/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45954 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    86154 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    19172 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    14014 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/maintenance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    34046 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    61676 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14039 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48989 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6953 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/kms/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30971 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9175 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20651 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    73017 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28381 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11012 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/health_check_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/health_check_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29420 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    92193 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27604 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10410 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    49878 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16364 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5875 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    16231 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    77237 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28847 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/logging/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16678 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_entry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_entry_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10458 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    53343 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9647 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_ingestion_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_ingestion_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    14142 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_reading_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_reading_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5584 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_resource_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/logging/v1/log_resource_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8837 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10988 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/usage_record_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/usage_record_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9804 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5017 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    59126 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   221733 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    60171 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127100 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/config/clickhouse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/config/clickhouse_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4676 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    21534 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9134 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5550 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    30243 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10817 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12238 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/maintenance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5073 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28984 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10623 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9923 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    41024 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14446 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/version_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/version_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7120 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16966 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    32902 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14690 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    43260 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   113634 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28117 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7043 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/config/elasticsearch_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/config/elasticsearch_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4017 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10131 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    27381 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71851 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    82726 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    23705 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9805 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    45336 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    27144 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10191 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9735 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    39267 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13842 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7417 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13800 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6832 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   100270 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   243346 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    49675 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49439 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb3_6_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb3_6_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48785 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_0_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_0_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48785 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_2_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48785 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_4_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_4_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4630 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    21317 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8744 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12139 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/maintenance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3918 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5248 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8028 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    39352 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14010 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9697 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    44988 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   148656 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38244 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60337 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/mysql5_7_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/mysql5_7_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    58885 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/mysql8_0_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/mysql8_0_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    21164 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8612 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12074 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/maintenance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9808 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24009 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    41335 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13845 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    36245 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   110668 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29401 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/config/mysql5_7_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/config/mysql5_7_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    21527 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9997 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13043 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    39844 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14075 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9914 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5017 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    75566 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   176341 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39015 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68372 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host10_1c_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host10_1c_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    67655 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host10_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host10_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    67664 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host11_1c_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host11_1c_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    66953 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host11_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host11_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    67664 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host12_1c_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host12_1c_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    66953 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host12_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host12_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    66953 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host13_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host13_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    58943 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host9_6_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host9_6_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   110897 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_1c_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_1c_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   108309 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   115327 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_1c_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_1c_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   114089 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   118465 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_1c_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_1c_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   117183 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   127212 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql13_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql13_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    83725 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql9_6_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql9_6_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10960 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28153 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10680 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12238 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/maintenance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10004 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    22979 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    42493 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14181 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5240 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9590 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    45409 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   163136 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    45584 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12730 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis5_0_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis5_0_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12732 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis6_0_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis6_0_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12732 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis6_2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis6_2_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    12074 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/maintenance_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9448 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9875 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4953 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    40400 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   111932 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27660 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18106 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/config/sqlserver2016sp2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/config/sqlserver2016sp2_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29992 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10630 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3964 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5242 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    39735 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14085 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/operation/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/operation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7838 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/operation/operation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/operation/operation_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/operation/operation_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/operation/operation_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/quota/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/quota/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8337 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/quota/quota_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/quota/quota_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/reference/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/reference/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5845 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/reference/reference_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/reference/reference_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29637 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16147 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9124 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    41778 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18049 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14557 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    60281 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24679 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36709 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   115422 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    40588 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14429 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    42652 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18196 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9908 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/predicate_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    63095 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    46953 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16409 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9111 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/validation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/validation_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16970 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    47552 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15536 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    46388 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15738 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13396 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    43725 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14193 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25271 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    65985 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17864 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13350 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    52993 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15641 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/ydb/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28465 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18682 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8137 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    34017 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    66885 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16865 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8855 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9401 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandexcloud/
+-rw-r--r--   0 root         (0) root         (0)      269 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3567 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_auth_fabric.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_auth_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      563 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_backoff.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_channels.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_operation_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     6398 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_retry_interceptor.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_sdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandexcloud/_wrappers/
+-rw-r--r--   0 root         (0) root         (0)      172 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_wrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandexcloud/_wrappers/dataproc/
+-rw-r--r--   0 root         (0) root         (0)    29150 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/_wrappers/dataproc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      408 2021-07-27 07:45:28.000000 yandexcloud-0.99.0/yandexcloud/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-27 07:45:52.000000 yandexcloud-0.99.0/yandexcloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      530 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandexcloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34085 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandexcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandexcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandexcloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      108 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandexcloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2021-07-27 07:45:51.000000 yandexcloud-0.99.0/yandexcloud.egg-info/top_level.txt
```

### Comparing `yandexcloud-0.98.0/LICENSE` & `yandexcloud-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/PKG-INFO` & `yandexcloud-0.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandexcloud
-Version: 0.98.0
+Version: 0.99.0
 Summary: The Yandex.Cloud official SDK
 Home-page: https://github.com/yandex-cloud/python-sdk
 Author: Yandex LLC
 Author-email: cloud@support.yandex.ru
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `yandexcloud-0.98.0/README.md` & `yandexcloud-0.99.0/README.md`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/setup.py` & `yandexcloud-0.99.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 packages = find_packages('.', include=['yandexcloud*', 'yandex*'])
 
 setup(name='yandexcloud',
-      version='0.98.0',
+      version='0.99.0',
       description='The Yandex.Cloud official SDK',
       url='https://github.com/yandex-cloud/python-sdk',
       author='Yandex LLC',
       author_email='cloud@support.yandex.ru',
       license='MIT',
       install_requires=[
           'cryptography>=2.8',
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/access/access_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/access/access_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/stt/v2/stt_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/stt/v2/stt_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ai/stt/v2/stt_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/translate/v2/translation_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ai/translate/v2/translation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/tts/v3/tts_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ai/tts/v3/tts_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/classification_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/classification_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/face_detection_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/face_detection_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/image_copy_search_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/image_copy_search_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/primitives_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/primitives_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/text_detection_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/text_detection_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/vision_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ai/vision/v1/vision_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ai/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/api/operation_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/api/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yandex/cloud/apploadbalancer/v1/backend_group.proto',
   package='yandex.cloud.apploadbalancer.v1',
   syntax='proto3',
   serialized_options=b'\n#yandex.cloud.api.apploadbalancer.v1ZSgithub.com/yandex-cloud/go-genproto/yandex/cloud/apploadbalancer/v1;apploadbalancer',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n3yandex/cloud/apploadbalancer/v1/backend_group.proto\x12\x1fyandex.cloud.apploadbalancer.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a-yandex/cloud/apploadbalancer/v1/payload.proto\x1a)yandex/cloud/apploadbalancer/v1/tls.proto\x1a\x1dyandex/cloud/validation.proto\"\x8b\x03\n\x0c\x42\x61\x63kendGroup\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x11\n\tfolder_id\x18\x04 \x01(\t\x12I\n\x06labels\x18\x05 \x03(\x0b\x32\x39.yandex.cloud.apploadbalancer.v1.BackendGroup.LabelsEntry\x12\x41\n\x04http\x18\x06 \x01(\x0b\x32\x31.yandex.cloud.apploadbalancer.v1.HttpBackendGroupH\x00\x12\x41\n\x04grpc\x18\x07 \x01(\x0b\x32\x31.yandex.cloud.apploadbalancer.v1.GrpcBackendGroupH\x00\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\t\n\x07\x62\x61\x63kend\"R\n\x10HttpBackendGroup\x12>\n\x08\x62\x61\x63kends\x18\x01 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.HttpBackend\"R\n\x10GrpcBackendGroup\x12>\n\x08\x62\x61\x63kends\x18\x01 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.GrpcBackend\"7\n\x15HeaderSessionAffinity\x12\x1e\n\x0bheader_name\x18\x01 \x01(\tB\t\x8a\xc8\x31\x05\x31-256\"X\n\x15\x43ookieSessionAffinity\x12\x17\n\x04name\x18\x01 \x01(\tB\t\x8a\xc8\x31\x05\x31-256\x12&\n\x03ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\".\n\x19\x43onnectionSessionAffinity\x12\x11\n\tsource_ip\x18\x01 \x01(\x08\"\x85\x01\n\x13LoadBalancingConfig\x12\"\n\x0fpanic_threshold\x18\x01 \x01(\x03\x42\t\xfa\xc7\x31\x05\x30-100\x12\x31\n\x1elocality_aware_routing_percent\x18\x02 \x01(\x03\x42\t\xfa\xc7\x31\x05\x30-100\x12\x17\n\x0fstrict_locality\x18\x03 \x01(\x08\"\xdc\x03\n\x0bHttpBackend\x12\x32\n\x04name\x18\x01 \x01(\tB$\xe8\xc7\x31\x01\xf2\xc7\x31\x1c[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x33\n\x0e\x62\x61\x63kend_weight\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12S\n\x15load_balancing_config\x18\x03 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.LoadBalancingConfig\x12\x19\n\x04port\x18\x04 \x01(\x03\x42\x0b\xfa\xc7\x31\x07\x30-65535\x12M\n\rtarget_groups\x18\x05 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.TargetGroupsBackendH\x00\x12\x42\n\x0chealthchecks\x18\x06 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.HealthCheck\x12\x38\n\x03tls\x18\x07 \x01(\x0b\x32+.yandex.cloud.apploadbalancer.v1.BackendTls\x12\x11\n\tuse_http2\x18\x08 \x01(\x08\x42\x14\n\x0c\x62\x61\x63kend_type\x12\x04\xc0\xc1\x31\x01\"\xc9\x03\n\x0bGrpcBackend\x12\x32\n\x04name\x18\x01 \x01(\tB$\xe8\xc7\x31\x01\xf2\xc7\x31\x1c[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x33\n\x0e\x62\x61\x63kend_weight\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12S\n\x15load_balancing_config\x18\x03 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.LoadBalancingConfig\x12\x19\n\x04port\x18\x04 \x01(\x03\x42\x0b\xfa\xc7\x31\x07\x30-65535\x12M\n\rtarget_groups\x18\x05 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.TargetGroupsBackendH\x00\x12\x42\n\x0chealthchecks\x18\x07 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.HealthCheck\x12\x38\n\x03tls\x18\x08 \x01(\x0b\x32+.yandex.cloud.apploadbalancer.v1.BackendTlsB\x14\n\x0c\x62\x61\x63kend_type\x12\x04\xc0\xc1\x31\x01\"7\n\x13TargetGroupsBackend\x12 \n\x10target_group_ids\x18\x01 \x03(\tB\x06\x82\xc8\x31\x02>0\"i\n\nBackendTls\x12\x0b\n\x03sni\x18\x01 \x01(\t\x12N\n\x12validation_context\x18\x03 \x01(\x0b\x32\x32.yandex.cloud.apploadbalancer.v1.ValidationContext\"\xef\x05\n\x0bHealthCheck\x12\x30\n\x07timeout\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x04\xe8\xc7\x31\x01\x12\x31\n\x08interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x04\xe8\xc7\x31\x01\x12\x1f\n\x17interval_jitter_percent\x18\x03 \x01(\x01\x12\x19\n\x11healthy_threshold\x18\x04 \x01(\x03\x12\x1b\n\x13unhealthy_threshold\x18\x05 \x01(\x03\x12%\n\x10healthcheck_port\x18\x06 \x01(\x03\x42\x0b\xfa\xc7\x31\x07\x30-65535\x12P\n\x06stream\x18\x07 \x01(\x0b\x32>.yandex.cloud.apploadbalancer.v1.HealthCheck.StreamHealthCheckH\x00\x12L\n\x04http\x18\x08 \x01(\x0b\x32<.yandex.cloud.apploadbalancer.v1.HealthCheck.HttpHealthCheckH\x00\x12L\n\x04grpc\x18\t \x01(\x0b\x32<.yandex.cloud.apploadbalancer.v1.HealthCheck.GrpcHealthCheckH\x00\x1a\x86\x01\n\x11StreamHealthCheck\x12\x36\n\x04send\x18\x01 \x01(\x0b\x32(.yandex.cloud.apploadbalancer.v1.Payload\x12\x39\n\x07receive\x18\x02 \x01(\x0b\x32(.yandex.cloud.apploadbalancer.v1.Payload\x1a\x46\n\x0fHttpHealthCheck\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x12\n\x04path\x18\x02 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x11\n\tuse_http2\x18\x03 \x01(\x08\x1a\'\n\x0fGrpcHealthCheck\x12\x14\n\x0cservice_name\x18\x01 \x01(\tB\x13\n\x0bhealthcheck\x12\x04\xc0\xc1\x31\x01\x42z\n#yandex.cloud.api.apploadbalancer.v1ZSgithub.com/yandex-cloud/go-genproto/yandex/cloud/apploadbalancer/v1;apploadbalancerb\x06proto3'
+  serialized_pb=b'\n3yandex/cloud/apploadbalancer/v1/backend_group.proto\x12\x1fyandex.cloud.apploadbalancer.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a-yandex/cloud/apploadbalancer/v1/payload.proto\x1a)yandex/cloud/apploadbalancer/v1/tls.proto\x1a\x1dyandex/cloud/validation.proto\"\x8b\x03\n\x0c\x42\x61\x63kendGroup\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x11\n\tfolder_id\x18\x04 \x01(\t\x12I\n\x06labels\x18\x05 \x03(\x0b\x32\x39.yandex.cloud.apploadbalancer.v1.BackendGroup.LabelsEntry\x12\x41\n\x04http\x18\x06 \x01(\x0b\x32\x31.yandex.cloud.apploadbalancer.v1.HttpBackendGroupH\x00\x12\x41\n\x04grpc\x18\x07 \x01(\x0b\x32\x31.yandex.cloud.apploadbalancer.v1.GrpcBackendGroupH\x00\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\t\n\x07\x62\x61\x63kend\"R\n\x10HttpBackendGroup\x12>\n\x08\x62\x61\x63kends\x18\x01 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.HttpBackend\"R\n\x10GrpcBackendGroup\x12>\n\x08\x62\x61\x63kends\x18\x01 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.GrpcBackend\"7\n\x15HeaderSessionAffinity\x12\x1e\n\x0bheader_name\x18\x01 \x01(\tB\t\x8a\xc8\x31\x05\x31-256\"X\n\x15\x43ookieSessionAffinity\x12\x17\n\x04name\x18\x01 \x01(\tB\t\x8a\xc8\x31\x05\x31-256\x12&\n\x03ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\".\n\x19\x43onnectionSessionAffinity\x12\x11\n\tsource_ip\x18\x01 \x01(\x08\"\x85\x01\n\x13LoadBalancingConfig\x12\"\n\x0fpanic_threshold\x18\x01 \x01(\x03\x42\t\xfa\xc7\x31\x05\x30-100\x12\x31\n\x1elocality_aware_routing_percent\x18\x02 \x01(\x03\x42\t\xfa\xc7\x31\x05\x30-100\x12\x17\n\x0fstrict_locality\x18\x03 \x01(\x08\"\xad\x04\n\x0bHttpBackend\x12\x32\n\x04name\x18\x01 \x01(\tB$\xe8\xc7\x31\x01\xf2\xc7\x31\x1c[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x33\n\x0e\x62\x61\x63kend_weight\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12S\n\x15load_balancing_config\x18\x03 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.LoadBalancingConfig\x12\x19\n\x04port\x18\x04 \x01(\x03\x42\x0b\xfa\xc7\x31\x07\x30-65535\x12M\n\rtarget_groups\x18\x05 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.TargetGroupsBackendH\x00\x12O\n\x0estorage_bucket\x18\t \x01(\x0b\x32\x35.yandex.cloud.apploadbalancer.v1.StorageBucketBackendH\x00\x12\x42\n\x0chealthchecks\x18\x06 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.HealthCheck\x12\x38\n\x03tls\x18\x07 \x01(\x0b\x32+.yandex.cloud.apploadbalancer.v1.BackendTls\x12\x11\n\tuse_http2\x18\x08 \x01(\x08\x42\x14\n\x0c\x62\x61\x63kend_type\x12\x04\xc0\xc1\x31\x01\"\xc9\x03\n\x0bGrpcBackend\x12\x32\n\x04name\x18\x01 \x01(\tB$\xe8\xc7\x31\x01\xf2\xc7\x31\x1c[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x33\n\x0e\x62\x61\x63kend_weight\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12S\n\x15load_balancing_config\x18\x03 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.LoadBalancingConfig\x12\x19\n\x04port\x18\x04 \x01(\x03\x42\x0b\xfa\xc7\x31\x07\x30-65535\x12M\n\rtarget_groups\x18\x05 \x01(\x0b\x32\x34.yandex.cloud.apploadbalancer.v1.TargetGroupsBackendH\x00\x12\x42\n\x0chealthchecks\x18\x07 \x03(\x0b\x32,.yandex.cloud.apploadbalancer.v1.HealthCheck\x12\x38\n\x03tls\x18\x08 \x01(\x0b\x32+.yandex.cloud.apploadbalancer.v1.BackendTlsB\x14\n\x0c\x62\x61\x63kend_type\x12\x04\xc0\xc1\x31\x01\"7\n\x13TargetGroupsBackend\x12 \n\x10target_group_ids\x18\x01 \x03(\tB\x06\x82\xc8\x31\x02>0\"i\n\nBackendTls\x12\x0b\n\x03sni\x18\x01 \x01(\t\x12N\n\x12validation_context\x18\x03 \x01(\x0b\x32\x32.yandex.cloud.apploadbalancer.v1.ValidationContext\",\n\x14StorageBucketBackend\x12\x14\n\x06\x62ucket\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\"\xef\x05\n\x0bHealthCheck\x12\x30\n\x07timeout\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x04\xe8\xc7\x31\x01\x12\x31\n\x08interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x04\xe8\xc7\x31\x01\x12\x1f\n\x17interval_jitter_percent\x18\x03 \x01(\x01\x12\x19\n\x11healthy_threshold\x18\x04 \x01(\x03\x12\x1b\n\x13unhealthy_threshold\x18\x05 \x01(\x03\x12%\n\x10healthcheck_port\x18\x06 \x01(\x03\x42\x0b\xfa\xc7\x31\x07\x30-65535\x12P\n\x06stream\x18\x07 \x01(\x0b\x32>.yandex.cloud.apploadbalancer.v1.HealthCheck.StreamHealthCheckH\x00\x12L\n\x04http\x18\x08 \x01(\x0b\x32<.yandex.cloud.apploadbalancer.v1.HealthCheck.HttpHealthCheckH\x00\x12L\n\x04grpc\x18\t \x01(\x0b\x32<.yandex.cloud.apploadbalancer.v1.HealthCheck.GrpcHealthCheckH\x00\x1a\x86\x01\n\x11StreamHealthCheck\x12\x36\n\x04send\x18\x01 \x01(\x0b\x32(.yandex.cloud.apploadbalancer.v1.Payload\x12\x39\n\x07receive\x18\x02 \x01(\x0b\x32(.yandex.cloud.apploadbalancer.v1.Payload\x1a\x46\n\x0fHttpHealthCheck\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x12\n\x04path\x18\x02 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x11\n\tuse_http2\x18\x03 \x01(\x08\x1a\'\n\x0fGrpcHealthCheck\x12\x14\n\x0cservice_name\x18\x01 \x01(\tB\x13\n\x0bhealthcheck\x12\x04\xc0\xc1\x31\x01\x42z\n#yandex.cloud.api.apploadbalancer.v1ZSgithub.com/yandex-cloud/go-genproto/yandex/cloud/apploadbalancer/v1;apploadbalancerb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,yandex_dot_cloud_dot_apploadbalancer_dot_v1_dot_payload__pb2.DESCRIPTOR,yandex_dot_cloud_dot_apploadbalancer_dot_v1_dot_tls__pb2.DESCRIPTOR,yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,])
 
 
 
 
 _BACKENDGROUP_LABELSENTRY = _descriptor.Descriptor(
@@ -409,29 +409,36 @@
       name='target_groups', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.target_groups', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='healthchecks', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.healthchecks', index=5,
+      name='storage_bucket', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.storage_bucket', index=5,
+      number=9, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='healthchecks', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.healthchecks', index=6,
       number=6, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='tls', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.tls', index=6,
+      name='tls', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.tls', index=7,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='use_http2', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.use_http2', index=7,
+      name='use_http2', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.use_http2', index=8,
       number=8, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -447,15 +454,15 @@
     _descriptor.OneofDescriptor(
       name='backend_type', full_name='yandex.cloud.apploadbalancer.v1.HttpBackend.backend_type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\300\3011\001'),
   ],
   serialized_start=1204,
-  serialized_end=1680,
+  serialized_end=1761,
 )
 
 
 _GRPCBACKEND = _descriptor.Descriptor(
   name='GrpcBackend',
   full_name='yandex.cloud.apploadbalancer.v1.GrpcBackend',
   filename=None,
@@ -525,16 +532,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='backend_type', full_name='yandex.cloud.apploadbalancer.v1.GrpcBackend.backend_type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\300\3011\001'),
   ],
-  serialized_start=1683,
-  serialized_end=2140,
+  serialized_start=1764,
+  serialized_end=2221,
 )
 
 
 _TARGETGROUPSBACKEND = _descriptor.Descriptor(
   name='TargetGroupsBackend',
   full_name='yandex.cloud.apploadbalancer.v1.TargetGroupsBackend',
   filename=None,
@@ -557,16 +564,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2142,
-  serialized_end=2197,
+  serialized_start=2223,
+  serialized_end=2278,
 )
 
 
 _BACKENDTLS = _descriptor.Descriptor(
   name='BackendTls',
   full_name='yandex.cloud.apploadbalancer.v1.BackendTls',
   filename=None,
@@ -596,16 +603,48 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2199,
-  serialized_end=2304,
+  serialized_start=2280,
+  serialized_end=2385,
+)
+
+
+_STORAGEBUCKETBACKEND = _descriptor.Descriptor(
+  name='StorageBucketBackend',
+  full_name='yandex.cloud.apploadbalancer.v1.StorageBucketBackend',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='bucket', full_name='yandex.cloud.apploadbalancer.v1.StorageBucketBackend.bucket', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\350\3071\001', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2387,
+  serialized_end=2431,
 )
 
 
 _HEALTHCHECK_STREAMHEALTHCHECK = _descriptor.Descriptor(
   name='StreamHealthCheck',
   full_name='yandex.cloud.apploadbalancer.v1.HealthCheck.StreamHealthCheck',
   filename=None,
@@ -635,16 +674,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2790,
-  serialized_end=2924,
+  serialized_start=2917,
+  serialized_end=3051,
 )
 
 _HEALTHCHECK_HTTPHEALTHCHECK = _descriptor.Descriptor(
   name='HttpHealthCheck',
   full_name='yandex.cloud.apploadbalancer.v1.HealthCheck.HttpHealthCheck',
   filename=None,
   file=DESCRIPTOR,
@@ -680,16 +719,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2926,
-  serialized_end=2996,
+  serialized_start=3053,
+  serialized_end=3123,
 )
 
 _HEALTHCHECK_GRPCHEALTHCHECK = _descriptor.Descriptor(
   name='GrpcHealthCheck',
   full_name='yandex.cloud.apploadbalancer.v1.HealthCheck.GrpcHealthCheck',
   filename=None,
   file=DESCRIPTOR,
@@ -711,16 +750,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2998,
-  serialized_end=3037,
+  serialized_start=3125,
+  serialized_end=3164,
 )
 
 _HEALTHCHECK = _descriptor.Descriptor(
   name='HealthCheck',
   full_name='yandex.cloud.apploadbalancer.v1.HealthCheck',
   filename=None,
   file=DESCRIPTOR,
@@ -803,16 +842,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='healthcheck', full_name='yandex.cloud.apploadbalancer.v1.HealthCheck.healthcheck',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[], serialized_options=b'\300\3011\001'),
   ],
-  serialized_start=2307,
-  serialized_end=3058,
+  serialized_start=2434,
+  serialized_end=3185,
 )
 
 _BACKENDGROUP_LABELSENTRY.containing_type = _BACKENDGROUP
 _BACKENDGROUP.fields_by_name['labels'].message_type = _BACKENDGROUP_LABELSENTRY
 _BACKENDGROUP.fields_by_name['http'].message_type = _HTTPBACKENDGROUP
 _BACKENDGROUP.fields_by_name['grpc'].message_type = _GRPCBACKENDGROUP
 _BACKENDGROUP.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
@@ -824,19 +863,23 @@
 _BACKENDGROUP.fields_by_name['grpc'].containing_oneof = _BACKENDGROUP.oneofs_by_name['backend']
 _HTTPBACKENDGROUP.fields_by_name['backends'].message_type = _HTTPBACKEND
 _GRPCBACKENDGROUP.fields_by_name['backends'].message_type = _GRPCBACKEND
 _COOKIESESSIONAFFINITY.fields_by_name['ttl'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _HTTPBACKEND.fields_by_name['backend_weight'].message_type = google_dot_protobuf_dot_wrappers__pb2._INT64VALUE
 _HTTPBACKEND.fields_by_name['load_balancing_config'].message_type = _LOADBALANCINGCONFIG
 _HTTPBACKEND.fields_by_name['target_groups'].message_type = _TARGETGROUPSBACKEND
+_HTTPBACKEND.fields_by_name['storage_bucket'].message_type = _STORAGEBUCKETBACKEND
 _HTTPBACKEND.fields_by_name['healthchecks'].message_type = _HEALTHCHECK
 _HTTPBACKEND.fields_by_name['tls'].message_type = _BACKENDTLS
 _HTTPBACKEND.oneofs_by_name['backend_type'].fields.append(
   _HTTPBACKEND.fields_by_name['target_groups'])
 _HTTPBACKEND.fields_by_name['target_groups'].containing_oneof = _HTTPBACKEND.oneofs_by_name['backend_type']
+_HTTPBACKEND.oneofs_by_name['backend_type'].fields.append(
+  _HTTPBACKEND.fields_by_name['storage_bucket'])
+_HTTPBACKEND.fields_by_name['storage_bucket'].containing_oneof = _HTTPBACKEND.oneofs_by_name['backend_type']
 _GRPCBACKEND.fields_by_name['backend_weight'].message_type = google_dot_protobuf_dot_wrappers__pb2._INT64VALUE
 _GRPCBACKEND.fields_by_name['load_balancing_config'].message_type = _LOADBALANCINGCONFIG
 _GRPCBACKEND.fields_by_name['target_groups'].message_type = _TARGETGROUPSBACKEND
 _GRPCBACKEND.fields_by_name['healthchecks'].message_type = _HEALTHCHECK
 _GRPCBACKEND.fields_by_name['tls'].message_type = _BACKENDTLS
 _GRPCBACKEND.oneofs_by_name['backend_type'].fields.append(
   _GRPCBACKEND.fields_by_name['target_groups'])
@@ -868,14 +911,15 @@
 DESCRIPTOR.message_types_by_name['CookieSessionAffinity'] = _COOKIESESSIONAFFINITY
 DESCRIPTOR.message_types_by_name['ConnectionSessionAffinity'] = _CONNECTIONSESSIONAFFINITY
 DESCRIPTOR.message_types_by_name['LoadBalancingConfig'] = _LOADBALANCINGCONFIG
 DESCRIPTOR.message_types_by_name['HttpBackend'] = _HTTPBACKEND
 DESCRIPTOR.message_types_by_name['GrpcBackend'] = _GRPCBACKEND
 DESCRIPTOR.message_types_by_name['TargetGroupsBackend'] = _TARGETGROUPSBACKEND
 DESCRIPTOR.message_types_by_name['BackendTls'] = _BACKENDTLS
+DESCRIPTOR.message_types_by_name['StorageBucketBackend'] = _STORAGEBUCKETBACKEND
 DESCRIPTOR.message_types_by_name['HealthCheck'] = _HEALTHCHECK
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 BackendGroup = _reflection.GeneratedProtocolMessageType('BackendGroup', (_message.Message,), {
 
   'LabelsEntry' : _reflection.GeneratedProtocolMessageType('LabelsEntry', (_message.Message,), {
     'DESCRIPTOR' : _BACKENDGROUP_LABELSENTRY,
@@ -956,14 +1000,21 @@
 BackendTls = _reflection.GeneratedProtocolMessageType('BackendTls', (_message.Message,), {
   'DESCRIPTOR' : _BACKENDTLS,
   '__module__' : 'yandex.cloud.apploadbalancer.v1.backend_group_pb2'
   # @@protoc_insertion_point(class_scope:yandex.cloud.apploadbalancer.v1.BackendTls)
   })
 _sym_db.RegisterMessage(BackendTls)
 
+StorageBucketBackend = _reflection.GeneratedProtocolMessageType('StorageBucketBackend', (_message.Message,), {
+  'DESCRIPTOR' : _STORAGEBUCKETBACKEND,
+  '__module__' : 'yandex.cloud.apploadbalancer.v1.backend_group_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.apploadbalancer.v1.StorageBucketBackend)
+  })
+_sym_db.RegisterMessage(StorageBucketBackend)
+
 HealthCheck = _reflection.GeneratedProtocolMessageType('HealthCheck', (_message.Message,), {
 
   'StreamHealthCheck' : _reflection.GeneratedProtocolMessageType('StreamHealthCheck', (_message.Message,), {
     'DESCRIPTOR' : _HEALTHCHECK_STREAMHEALTHCHECK,
     '__module__' : 'yandex.cloud.apploadbalancer.v1.backend_group_pb2'
     # @@protoc_insertion_point(class_scope:yandex.cloud.apploadbalancer.v1.HealthCheck.StreamHealthCheck)
     })
@@ -1001,13 +1052,14 @@
 _HTTPBACKEND.oneofs_by_name['backend_type']._options = None
 _HTTPBACKEND.fields_by_name['name']._options = None
 _HTTPBACKEND.fields_by_name['port']._options = None
 _GRPCBACKEND.oneofs_by_name['backend_type']._options = None
 _GRPCBACKEND.fields_by_name['name']._options = None
 _GRPCBACKEND.fields_by_name['port']._options = None
 _TARGETGROUPSBACKEND.fields_by_name['target_group_ids']._options = None
+_STORAGEBUCKETBACKEND.fields_by_name['bucket']._options = None
 _HEALTHCHECK_HTTPHEALTHCHECK.fields_by_name['path']._options = None
 _HEALTHCHECK.oneofs_by_name['healthcheck']._options = None
 _HEALTHCHECK.fields_by_name['timeout']._options = None
 _HEALTHCHECK.fields_by_name['interval']._options = None
 _HEALTHCHECK.fields_by_name['healthcheck_port']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/backend_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/http_router_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/load_balancer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/payload_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/payload_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/target_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/tls_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/tls_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/apploadbalancer/v1/virtual_host_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_content_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/certificatemanager/v1/certificate_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_placement_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/disk_type_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/disk_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/host_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/host_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/host_type_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/host_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/image_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/image_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/image_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/image_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/image_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/image_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/instance_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/instancegroup/instance_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/placement_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/placement_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/snapshot_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/snapshot_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/compute/v1/zone_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/compute/v1/zone_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/blob_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/image_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/image_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/ip_permission_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/ip_permission_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/lifecycle_policy_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/registry_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/registry_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/repository_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/repository_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/containerregistry/v1/scanner_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/containerregistry/v1/scanner_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/job_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/manager/v1/manager_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/common_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/job_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dataproc/v1/subcluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dataproc/v1/subcluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/datasphere/v1/node_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/datasphere/v1/node_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,224 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: yandex/cloud/datasphere/v1/project.proto
+# source: yandex/cloud/logging/v1/log_group.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='yandex/cloud/datasphere/v1/project.proto',
-  package='yandex.cloud.datasphere.v1',
+  name='yandex/cloud/logging/v1/log_group.proto',
+  package='yandex.cloud.logging.v1',
   syntax='proto3',
-  serialized_options=b'\n\036yandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphere',
+  serialized_options=b'\n\033yandex.cloud.api.logging.v1ZCgithub.com/yandex-cloud/go-genproto/yandex/cloud/logging/v1;logging',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n(yandex/cloud/datasphere/v1/project.proto\x12\x1ayandex.cloud.datasphere.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa6\x03\n\x07Project\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12>\n\x08settings\x18\x06 \x01(\x0b\x32,.yandex.cloud.datasphere.v1.Project.Settings\x1a\xe8\x01\n\x08Settings\x12\x1a\n\x12service_account_id\x18\x01 \x01(\t\x12\x11\n\tsubnet_id\x18\x02 \x01(\t\x12\x1c\n\x14\x64\x61ta_proc_cluster_id\x18\x03 \x01(\t\x12L\n\x0b\x63ommit_mode\x18\x04 \x01(\x0e\x32\x37.yandex.cloud.datasphere.v1.Project.Settings.CommitMode\"A\n\nCommitMode\x12\x1b\n\x17\x43OMMIT_MODE_UNSPECIFIED\x10\x00\x12\x0c\n\x08STANDARD\x10\x01\x12\x08\n\x04\x41UTO\x10\x02\x42k\n\x1eyandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphereb\x06proto3'
+  serialized_pb=b'\n\'yandex/cloud/logging/v1/log_group.proto\x12\x17yandex.cloud.logging.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc0\x03\n\x08LogGroup\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12\x10\n\x08\x63loud_id\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12=\n\x06labels\x18\x07 \x03(\x0b\x32-.yandex.cloud.logging.v1.LogGroup.LabelsEntry\x12\x38\n\x06status\x18\x08 \x01(\x0e\x32(.yandex.cloud.logging.v1.LogGroup.Status\x12\x33\n\x10retention_period\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"S\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x44\x45LETING\x10\x03\x12\t\n\x05\x45RROR\x10\x04\x42\x62\n\x1byandex.cloud.api.logging.v1ZCgithub.com/yandex-cloud/go-genproto/yandex/cloud/logging/v1;loggingb\x06proto3'
   ,
-  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 
 
-_PROJECT_SETTINGS_COMMITMODE = _descriptor.EnumDescriptor(
-  name='CommitMode',
-  full_name='yandex.cloud.datasphere.v1.Project.Settings.CommitMode',
+_LOGGROUP_STATUS = _descriptor.EnumDescriptor(
+  name='Status',
+  full_name='yandex.cloud.logging.v1.LogGroup.Status',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='COMMIT_MODE_UNSPECIFIED', index=0, number=0,
+      name='STATUS_UNSPECIFIED', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='STANDARD', index=1, number=1,
+      name='CREATING', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='AUTO', index=2, number=2,
+      name='ACTIVE', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DELETING', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='ERROR', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=463,
-  serialized_end=528,
+  serialized_start=499,
+  serialized_end=582,
 )
-_sym_db.RegisterEnumDescriptor(_PROJECT_SETTINGS_COMMITMODE)
+_sym_db.RegisterEnumDescriptor(_LOGGROUP_STATUS)
 
 
-_PROJECT_SETTINGS = _descriptor.Descriptor(
-  name='Settings',
-  full_name='yandex.cloud.datasphere.v1.Project.Settings',
+_LOGGROUP_LABELSENTRY = _descriptor.Descriptor(
+  name='LabelsEntry',
+  full_name='yandex.cloud.logging.v1.LogGroup.LabelsEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='service_account_id', full_name='yandex.cloud.datasphere.v1.Project.Settings.service_account_id', index=0,
+      name='key', full_name='yandex.cloud.logging.v1.LogGroup.LabelsEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='subnet_id', full_name='yandex.cloud.datasphere.v1.Project.Settings.subnet_id', index=1,
+      name='value', full_name='yandex.cloud.logging.v1.LogGroup.LabelsEntry.value', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='data_proc_cluster_id', full_name='yandex.cloud.datasphere.v1.Project.Settings.data_proc_cluster_id', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='commit_mode', full_name='yandex.cloud.datasphere.v1.Project.Settings.commit_mode', index=3,
-      number=4, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
-    _PROJECT_SETTINGS_COMMITMODE,
   ],
-  serialized_options=None,
+  serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=296,
-  serialized_end=528,
+  serialized_start=452,
+  serialized_end=497,
 )
 
-_PROJECT = _descriptor.Descriptor(
-  name='Project',
-  full_name='yandex.cloud.datasphere.v1.Project',
+_LOGGROUP = _descriptor.Descriptor(
+  name='LogGroup',
+  full_name='yandex.cloud.logging.v1.LogGroup',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='yandex.cloud.datasphere.v1.Project.id', index=0,
+      name='id', full_name='yandex.cloud.logging.v1.LogGroup.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='folder_id', full_name='yandex.cloud.datasphere.v1.Project.folder_id', index=1,
+      name='folder_id', full_name='yandex.cloud.logging.v1.LogGroup.folder_id', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='created_at', full_name='yandex.cloud.datasphere.v1.Project.created_at', index=2,
-      number=3, type=11, cpp_type=10, label=1,
+      name='cloud_id', full_name='yandex.cloud.logging.v1.LogGroup.cloud_id', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='created_at', full_name='yandex.cloud.logging.v1.LogGroup.created_at', index=3,
+      number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='name', full_name='yandex.cloud.datasphere.v1.Project.name', index=3,
-      number=4, type=9, cpp_type=9, label=1,
+      name='name', full_name='yandex.cloud.logging.v1.LogGroup.name', index=4,
+      number=5, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='description', full_name='yandex.cloud.datasphere.v1.Project.description', index=4,
-      number=5, type=9, cpp_type=9, label=1,
+      name='description', full_name='yandex.cloud.logging.v1.LogGroup.description', index=5,
+      number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='settings', full_name='yandex.cloud.datasphere.v1.Project.settings', index=5,
-      number=6, type=11, cpp_type=10, label=1,
+      name='labels', full_name='yandex.cloud.logging.v1.LogGroup.labels', index=6,
+      number=7, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='status', full_name='yandex.cloud.logging.v1.LogGroup.status', index=7,
+      number=8, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='retention_period', full_name='yandex.cloud.logging.v1.LogGroup.retention_period', index=8,
+      number=9, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_PROJECT_SETTINGS, ],
+  nested_types=[_LOGGROUP_LABELSENTRY, ],
   enum_types=[
+    _LOGGROUP_STATUS,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=106,
-  serialized_end=528,
+  serialized_start=134,
+  serialized_end=582,
 )
 
-_PROJECT_SETTINGS.fields_by_name['commit_mode'].enum_type = _PROJECT_SETTINGS_COMMITMODE
-_PROJECT_SETTINGS.containing_type = _PROJECT
-_PROJECT_SETTINGS_COMMITMODE.containing_type = _PROJECT_SETTINGS
-_PROJECT.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
-_PROJECT.fields_by_name['settings'].message_type = _PROJECT_SETTINGS
-DESCRIPTOR.message_types_by_name['Project'] = _PROJECT
+_LOGGROUP_LABELSENTRY.containing_type = _LOGGROUP
+_LOGGROUP.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_LOGGROUP.fields_by_name['labels'].message_type = _LOGGROUP_LABELSENTRY
+_LOGGROUP.fields_by_name['status'].enum_type = _LOGGROUP_STATUS
+_LOGGROUP.fields_by_name['retention_period'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
+_LOGGROUP_STATUS.containing_type = _LOGGROUP
+DESCRIPTOR.message_types_by_name['LogGroup'] = _LOGGROUP
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-Project = _reflection.GeneratedProtocolMessageType('Project', (_message.Message,), {
+LogGroup = _reflection.GeneratedProtocolMessageType('LogGroup', (_message.Message,), {
 
-  'Settings' : _reflection.GeneratedProtocolMessageType('Settings', (_message.Message,), {
-    'DESCRIPTOR' : _PROJECT_SETTINGS,
-    '__module__' : 'yandex.cloud.datasphere.v1.project_pb2'
-    # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.Project.Settings)
+  'LabelsEntry' : _reflection.GeneratedProtocolMessageType('LabelsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _LOGGROUP_LABELSENTRY,
+    '__module__' : 'yandex.cloud.logging.v1.log_group_pb2'
+    # @@protoc_insertion_point(class_scope:yandex.cloud.logging.v1.LogGroup.LabelsEntry)
     })
   ,
-  'DESCRIPTOR' : _PROJECT,
-  '__module__' : 'yandex.cloud.datasphere.v1.project_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.Project)
+  'DESCRIPTOR' : _LOGGROUP,
+  '__module__' : 'yandex.cloud.logging.v1.log_group_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.logging.v1.LogGroup)
   })
-_sym_db.RegisterMessage(Project)
-_sym_db.RegisterMessage(Project.Settings)
+_sym_db.RegisterMessage(LogGroup)
+_sym_db.RegisterMessage(LogGroup.LabelsEntry)
 
 
 DESCRIPTOR._options = None
+_LOGGROUP_LABELSENTRY._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_service_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from yandex.cloud.api import operation_pb2 as yandex_dot_cloud_dot_api_dot_operation__pb2
 from yandex.cloud import validation_pb2 as yandex_dot_cloud_dot_validation__pb2
 from yandex.cloud.operation import operation_pb2 as yandex_dot_cloud_dot_operation_dot_operation__pb2
 from yandex.cloud.datasphere.v1 import project_pb2 as yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yandex/cloud/datasphere/v1/project_service.proto',
   package='yandex.cloud.datasphere.v1',
   syntax='proto3',
   serialized_options=b'\n\036yandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphere',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n0yandex/cloud/datasphere/v1/project_service.proto\x12\x1ayandex.cloud.datasphere.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a yandex/cloud/api/operation.proto\x1a\x1dyandex/cloud/validation.proto\x1a&yandex/cloud/operation/operation.proto\x1a(yandex/cloud/datasphere/v1/project.proto\"\xd2\x01\n\x14\x43reateProjectRequest\x12\x1f\n\tfolder_id\x18\x01 \x01(\tB\x0c\xe8\xc7\x31\x01\x8a\xc8\x31\x04<=50\x12\x39\n\x04name\x18\x02 \x01(\tB+\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x1f[a-z]([-a-z0-9]{0,61}[a-z0-9])?\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12>\n\x08settings\x18\x04 \x01(\x0b\x32,.yandex.cloud.datasphere.v1.Project.Settings\"+\n\x15\x43reateProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"\x85\x02\n\x14UpdateProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x39\n\x04name\x18\x03 \x01(\tB+\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x1f[a-z]([-a-z0-9]{0,61}[a-z0-9])?\x12\x1e\n\x0b\x64\x65scription\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12>\n\x08settings\x18\x05 \x01(\x0b\x32,.yandex.cloud.datasphere.v1.Project.Settings\"+\n\x15UpdateProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"9\n\x14\x44\x65leteProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\"+\n\x15\x44\x65leteProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"7\n\x12OpenProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\")\n\x13OpenProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"A\n\x13OpenProjectResponse\x12\x13\n\x0bproject_url\x18\x01 \x01(\t\x12\x15\n\rsession_token\x18\x02 \x01(\t\"6\n\x11GetProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\"t\n\x13ListProjectsRequest\x12\x1f\n\tfolder_id\x18\x01 \x01(\tB\x0c\xe8\xc7\x31\x01\x8a\xc8\x31\x04<=50\x12\x1d\n\tpage_size\x18\x02 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=100\"f\n\x14ListProjectsResponse\x12\x35\n\x08projects\x18\x01 \x03(\x0b\x32#.yandex.cloud.datasphere.v1.Project\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\x81\x08\n\x0eProjectService\x12\xa5\x01\n\x06\x43reate\x12\x30.yandex.cloud.datasphere.v1.CreateProjectRequest\x1a!.yandex.cloud.operation.Operation\"F\x82\xd3\xe4\x93\x02\x1c\"\x17/datasphere/v1/projects:\x01*\xb2\xd2* \n\x15\x43reateProjectMetadata\x12\x07Project\x12\xb2\x01\n\x06Update\x12\x30.yandex.cloud.datasphere.v1.UpdateProjectRequest\x1a!.yandex.cloud.operation.Operation\"S\x82\xd3\xe4\x93\x02)2$/datasphere/v1/projects/{project_id}:\x01*\xb2\xd2* \n\x15UpdateProjectMetadata\x12\x07Project\x12\xbd\x01\n\x06\x44\x65lete\x12\x30.yandex.cloud.datasphere.v1.DeleteProjectRequest\x1a!.yandex.cloud.operation.Operation\"^\x82\xd3\xe4\x93\x02&*$/datasphere/v1/projects/{project_id}\xb2\xd2*.\n\x15\x44\x65leteProjectMetadata\x12\x15google.protobuf.Empty\x12\xba\x01\n\x04Open\x12..yandex.cloud.datasphere.v1.OpenProjectRequest\x1a!.yandex.cloud.operation.Operation\"_\x82\xd3\xe4\x93\x02+\")/datasphere/v1/projects/{project_id}:open\xb2\xd2**\n\x13OpenProjectMetadata\x12\x13OpenProjectResponse\x12\x87\x01\n\x03Get\x12-.yandex.cloud.datasphere.v1.GetProjectRequest\x1a#.yandex.cloud.datasphere.v1.Project\",\x82\xd3\xe4\x93\x02&\x12$/datasphere/v1/projects/{project_id}\x12\x8a\x01\n\x04List\x12/.yandex.cloud.datasphere.v1.ListProjectsRequest\x1a\x30.yandex.cloud.datasphere.v1.ListProjectsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/datasphere/v1/projectsBk\n\x1eyandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphereb\x06proto3'
+  serialized_pb=b'\n0yandex/cloud/datasphere/v1/project_service.proto\x12\x1ayandex.cloud.datasphere.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a yandex/cloud/api/operation.proto\x1a\x1dyandex/cloud/validation.proto\x1a&yandex/cloud/operation/operation.proto\x1a(yandex/cloud/datasphere/v1/project.proto\"\x8e\x02\n\x14\x43reateProjectRequest\x12\x1f\n\tfolder_id\x18\x01 \x01(\tB\x0c\xe8\xc7\x31\x01\x8a\xc8\x31\x04<=50\x12\x39\n\x04name\x18\x02 \x01(\tB+\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x1f[a-z]([-a-z0-9]{0,61}[a-z0-9])?\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12>\n\x08settings\x18\x04 \x01(\x0b\x32,.yandex.cloud.datasphere.v1.Project.Settings\x12:\n\x06limits\x18\x05 \x01(\x0b\x32*.yandex.cloud.datasphere.v1.Project.Limits\"+\n\x15\x43reateProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"\xc1\x02\n\x14UpdateProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x39\n\x04name\x18\x03 \x01(\tB+\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x1f[a-z]([-a-z0-9]{0,61}[a-z0-9])?\x12\x1e\n\x0b\x64\x65scription\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12>\n\x08settings\x18\x05 \x01(\x0b\x32,.yandex.cloud.datasphere.v1.Project.Settings\x12:\n\x06limits\x18\x06 \x01(\x0b\x32*.yandex.cloud.datasphere.v1.Project.Limits\"+\n\x15UpdateProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"9\n\x14\x44\x65leteProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\"+\n\x15\x44\x65leteProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"7\n\x12OpenProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\")\n\x13OpenProjectMetadata\x12\x12\n\nproject_id\x18\x01 \x01(\t\"A\n\x13OpenProjectResponse\x12\x13\n\x0bproject_url\x18\x01 \x01(\t\x12\x15\n\rsession_token\x18\x02 \x01(\t\"6\n\x11GetProjectRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\"t\n\x13ListProjectsRequest\x12\x1f\n\tfolder_id\x18\x01 \x01(\tB\x0c\xe8\xc7\x31\x01\x8a\xc8\x31\x04<=50\x12\x1d\n\tpage_size\x18\x02 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=100\"f\n\x14ListProjectsResponse\x12\x35\n\x08projects\x18\x01 \x03(\x0b\x32#.yandex.cloud.datasphere.v1.Project\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\":\n\x15GetUnitBalanceRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\"K\n\x16GetUnitBalanceResponse\x12\x31\n\x0cunit_balance\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\"m\n\x15SetUnitBalanceRequest\x12!\n\nproject_id\x18\x01 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05<=200\x12\x31\n\x0cunit_balance\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value2\xd0\n\n\x0eProjectService\x12\xa5\x01\n\x06\x43reate\x12\x30.yandex.cloud.datasphere.v1.CreateProjectRequest\x1a!.yandex.cloud.operation.Operation\"F\x82\xd3\xe4\x93\x02\x1c\"\x17/datasphere/v1/projects:\x01*\xb2\xd2* \n\x15\x43reateProjectMetadata\x12\x07Project\x12\xb2\x01\n\x06Update\x12\x30.yandex.cloud.datasphere.v1.UpdateProjectRequest\x1a!.yandex.cloud.operation.Operation\"S\x82\xd3\xe4\x93\x02)2$/datasphere/v1/projects/{project_id}:\x01*\xb2\xd2* \n\x15UpdateProjectMetadata\x12\x07Project\x12\xbd\x01\n\x06\x44\x65lete\x12\x30.yandex.cloud.datasphere.v1.DeleteProjectRequest\x1a!.yandex.cloud.operation.Operation\"^\x82\xd3\xe4\x93\x02&*$/datasphere/v1/projects/{project_id}\xb2\xd2*.\n\x15\x44\x65leteProjectMetadata\x12\x15google.protobuf.Empty\x12\xba\x01\n\x04Open\x12..yandex.cloud.datasphere.v1.OpenProjectRequest\x1a!.yandex.cloud.operation.Operation\"_\x82\xd3\xe4\x93\x02+\")/datasphere/v1/projects/{project_id}:open\xb2\xd2**\n\x13OpenProjectMetadata\x12\x13OpenProjectResponse\x12\x87\x01\n\x03Get\x12-.yandex.cloud.datasphere.v1.GetProjectRequest\x1a#.yandex.cloud.datasphere.v1.Project\",\x82\xd3\xe4\x93\x02&\x12$/datasphere/v1/projects/{project_id}\x12\x8a\x01\n\x04List\x12/.yandex.cloud.datasphere.v1.ListProjectsRequest\x1a\x30.yandex.cloud.datasphere.v1.ListProjectsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/datasphere/v1/projects\x12\xb1\x01\n\x0eGetUnitBalance\x12\x31.yandex.cloud.datasphere.v1.GetUnitBalanceRequest\x1a\x32.yandex.cloud.datasphere.v1.GetUnitBalanceResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/datasphere/v1/projects/{project_id}:unitBalance\x12\x98\x01\n\x0eSetUnitBalance\x12\x31.yandex.cloud.datasphere.v1.SetUnitBalanceRequest\x1a\x16.google.protobuf.Empty\";\x82\xd3\xe4\x93\x02\x35\"0/datasphere/v1/projects/{project_id}:unitBalance:\x01*Bk\n\x1eyandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphereb\x06proto3'
   ,
-  dependencies=[google_dot_api_dot_annotations__pb2.DESCRIPTOR,google_dot_protobuf_dot_field__mask__pb2.DESCRIPTOR,yandex_dot_cloud_dot_api_dot_operation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_operation_dot_operation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_api_dot_annotations__pb2.DESCRIPTOR,google_dot_protobuf_dot_field__mask__pb2.DESCRIPTOR,google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,yandex_dot_cloud_dot_api_dot_operation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_operation_dot_operation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2.DESCRIPTOR,])
 
 
 
 
 _CREATEPROJECTREQUEST = _descriptor.Descriptor(
   name='CreateProjectRequest',
   full_name='yandex.cloud.datasphere.v1.CreateProjectRequest',
@@ -64,28 +66,35 @@
     _descriptor.FieldDescriptor(
       name='settings', full_name='yandex.cloud.datasphere.v1.CreateProjectRequest.settings', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='limits', full_name='yandex.cloud.datasphere.v1.CreateProjectRequest.limits', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=292,
-  serialized_end=502,
+  serialized_start=353,
+  serialized_end=623,
 )
 
 
 _CREATEPROJECTMETADATA = _descriptor.Descriptor(
   name='CreateProjectMetadata',
   full_name='yandex.cloud.datasphere.v1.CreateProjectMetadata',
   filename=None,
@@ -108,16 +117,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=504,
-  serialized_end=547,
+  serialized_start=625,
+  serialized_end=668,
 )
 
 
 _UPDATEPROJECTREQUEST = _descriptor.Descriptor(
   name='UpdateProjectRequest',
   full_name='yandex.cloud.datasphere.v1.UpdateProjectRequest',
   filename=None,
@@ -156,28 +165,35 @@
     _descriptor.FieldDescriptor(
       name='settings', full_name='yandex.cloud.datasphere.v1.UpdateProjectRequest.settings', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='limits', full_name='yandex.cloud.datasphere.v1.UpdateProjectRequest.limits', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=550,
-  serialized_end=811,
+  serialized_start=671,
+  serialized_end=992,
 )
 
 
 _UPDATEPROJECTMETADATA = _descriptor.Descriptor(
   name='UpdateProjectMetadata',
   full_name='yandex.cloud.datasphere.v1.UpdateProjectMetadata',
   filename=None,
@@ -200,16 +216,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=813,
-  serialized_end=856,
+  serialized_start=994,
+  serialized_end=1037,
 )
 
 
 _DELETEPROJECTREQUEST = _descriptor.Descriptor(
   name='DeleteProjectRequest',
   full_name='yandex.cloud.datasphere.v1.DeleteProjectRequest',
   filename=None,
@@ -232,16 +248,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=858,
-  serialized_end=915,
+  serialized_start=1039,
+  serialized_end=1096,
 )
 
 
 _DELETEPROJECTMETADATA = _descriptor.Descriptor(
   name='DeleteProjectMetadata',
   full_name='yandex.cloud.datasphere.v1.DeleteProjectMetadata',
   filename=None,
@@ -264,16 +280,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=917,
-  serialized_end=960,
+  serialized_start=1098,
+  serialized_end=1141,
 )
 
 
 _OPENPROJECTREQUEST = _descriptor.Descriptor(
   name='OpenProjectRequest',
   full_name='yandex.cloud.datasphere.v1.OpenProjectRequest',
   filename=None,
@@ -296,16 +312,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=962,
-  serialized_end=1017,
+  serialized_start=1143,
+  serialized_end=1198,
 )
 
 
 _OPENPROJECTMETADATA = _descriptor.Descriptor(
   name='OpenProjectMetadata',
   full_name='yandex.cloud.datasphere.v1.OpenProjectMetadata',
   filename=None,
@@ -328,16 +344,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1019,
-  serialized_end=1060,
+  serialized_start=1200,
+  serialized_end=1241,
 )
 
 
 _OPENPROJECTRESPONSE = _descriptor.Descriptor(
   name='OpenProjectResponse',
   full_name='yandex.cloud.datasphere.v1.OpenProjectResponse',
   filename=None,
@@ -367,16 +383,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1062,
-  serialized_end=1127,
+  serialized_start=1243,
+  serialized_end=1308,
 )
 
 
 _GETPROJECTREQUEST = _descriptor.Descriptor(
   name='GetProjectRequest',
   full_name='yandex.cloud.datasphere.v1.GetProjectRequest',
   filename=None,
@@ -399,16 +415,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1129,
-  serialized_end=1183,
+  serialized_start=1310,
+  serialized_end=1364,
 )
 
 
 _LISTPROJECTSREQUEST = _descriptor.Descriptor(
   name='ListProjectsRequest',
   full_name='yandex.cloud.datasphere.v1.ListProjectsRequest',
   filename=None,
@@ -445,16 +461,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1185,
-  serialized_end=1301,
+  serialized_start=1366,
+  serialized_end=1482,
 )
 
 
 _LISTPROJECTSRESPONSE = _descriptor.Descriptor(
   name='ListProjectsResponse',
   full_name='yandex.cloud.datasphere.v1.ListProjectsResponse',
   filename=None,
@@ -484,34 +500,144 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1303,
-  serialized_end=1405,
+  serialized_start=1484,
+  serialized_end=1586,
+)
+
+
+_GETUNITBALANCEREQUEST = _descriptor.Descriptor(
+  name='GetUnitBalanceRequest',
+  full_name='yandex.cloud.datasphere.v1.GetUnitBalanceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='project_id', full_name='yandex.cloud.datasphere.v1.GetUnitBalanceRequest.project_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\350\3071\001\212\3101\005<=200', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1588,
+  serialized_end=1646,
+)
+
+
+_GETUNITBALANCERESPONSE = _descriptor.Descriptor(
+  name='GetUnitBalanceResponse',
+  full_name='yandex.cloud.datasphere.v1.GetUnitBalanceResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='unit_balance', full_name='yandex.cloud.datasphere.v1.GetUnitBalanceResponse.unit_balance', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1648,
+  serialized_end=1723,
+)
+
+
+_SETUNITBALANCEREQUEST = _descriptor.Descriptor(
+  name='SetUnitBalanceRequest',
+  full_name='yandex.cloud.datasphere.v1.SetUnitBalanceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='project_id', full_name='yandex.cloud.datasphere.v1.SetUnitBalanceRequest.project_id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\350\3071\001\212\3101\005<=200', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='unit_balance', full_name='yandex.cloud.datasphere.v1.SetUnitBalanceRequest.unit_balance', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1725,
+  serialized_end=1834,
 )
 
 _CREATEPROJECTREQUEST.fields_by_name['settings'].message_type = yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2._PROJECT_SETTINGS
+_CREATEPROJECTREQUEST.fields_by_name['limits'].message_type = yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2._PROJECT_LIMITS
 _UPDATEPROJECTREQUEST.fields_by_name['update_mask'].message_type = google_dot_protobuf_dot_field__mask__pb2._FIELDMASK
 _UPDATEPROJECTREQUEST.fields_by_name['settings'].message_type = yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2._PROJECT_SETTINGS
+_UPDATEPROJECTREQUEST.fields_by_name['limits'].message_type = yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2._PROJECT_LIMITS
 _LISTPROJECTSRESPONSE.fields_by_name['projects'].message_type = yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2._PROJECT
+_GETUNITBALANCERESPONSE.fields_by_name['unit_balance'].message_type = google_dot_protobuf_dot_wrappers__pb2._INT64VALUE
+_SETUNITBALANCEREQUEST.fields_by_name['unit_balance'].message_type = google_dot_protobuf_dot_wrappers__pb2._INT64VALUE
 DESCRIPTOR.message_types_by_name['CreateProjectRequest'] = _CREATEPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['CreateProjectMetadata'] = _CREATEPROJECTMETADATA
 DESCRIPTOR.message_types_by_name['UpdateProjectRequest'] = _UPDATEPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['UpdateProjectMetadata'] = _UPDATEPROJECTMETADATA
 DESCRIPTOR.message_types_by_name['DeleteProjectRequest'] = _DELETEPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['DeleteProjectMetadata'] = _DELETEPROJECTMETADATA
 DESCRIPTOR.message_types_by_name['OpenProjectRequest'] = _OPENPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['OpenProjectMetadata'] = _OPENPROJECTMETADATA
 DESCRIPTOR.message_types_by_name['OpenProjectResponse'] = _OPENPROJECTRESPONSE
 DESCRIPTOR.message_types_by_name['GetProjectRequest'] = _GETPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['ListProjectsRequest'] = _LISTPROJECTSREQUEST
 DESCRIPTOR.message_types_by_name['ListProjectsResponse'] = _LISTPROJECTSRESPONSE
+DESCRIPTOR.message_types_by_name['GetUnitBalanceRequest'] = _GETUNITBALANCEREQUEST
+DESCRIPTOR.message_types_by_name['GetUnitBalanceResponse'] = _GETUNITBALANCERESPONSE
+DESCRIPTOR.message_types_by_name['SetUnitBalanceRequest'] = _SETUNITBALANCEREQUEST
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 CreateProjectRequest = _reflection.GeneratedProtocolMessageType('CreateProjectRequest', (_message.Message,), {
   'DESCRIPTOR' : _CREATEPROJECTREQUEST,
   '__module__' : 'yandex.cloud.datasphere.v1.project_service_pb2'
   # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.CreateProjectRequest)
   })
@@ -590,38 +716,61 @@
 ListProjectsResponse = _reflection.GeneratedProtocolMessageType('ListProjectsResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTPROJECTSRESPONSE,
   '__module__' : 'yandex.cloud.datasphere.v1.project_service_pb2'
   # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.ListProjectsResponse)
   })
 _sym_db.RegisterMessage(ListProjectsResponse)
 
+GetUnitBalanceRequest = _reflection.GeneratedProtocolMessageType('GetUnitBalanceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETUNITBALANCEREQUEST,
+  '__module__' : 'yandex.cloud.datasphere.v1.project_service_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.GetUnitBalanceRequest)
+  })
+_sym_db.RegisterMessage(GetUnitBalanceRequest)
+
+GetUnitBalanceResponse = _reflection.GeneratedProtocolMessageType('GetUnitBalanceResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETUNITBALANCERESPONSE,
+  '__module__' : 'yandex.cloud.datasphere.v1.project_service_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.GetUnitBalanceResponse)
+  })
+_sym_db.RegisterMessage(GetUnitBalanceResponse)
+
+SetUnitBalanceRequest = _reflection.GeneratedProtocolMessageType('SetUnitBalanceRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETUNITBALANCEREQUEST,
+  '__module__' : 'yandex.cloud.datasphere.v1.project_service_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.SetUnitBalanceRequest)
+  })
+_sym_db.RegisterMessage(SetUnitBalanceRequest)
+
 
 DESCRIPTOR._options = None
 _CREATEPROJECTREQUEST.fields_by_name['folder_id']._options = None
 _CREATEPROJECTREQUEST.fields_by_name['name']._options = None
 _CREATEPROJECTREQUEST.fields_by_name['description']._options = None
 _UPDATEPROJECTREQUEST.fields_by_name['project_id']._options = None
 _UPDATEPROJECTREQUEST.fields_by_name['name']._options = None
 _UPDATEPROJECTREQUEST.fields_by_name['description']._options = None
 _DELETEPROJECTREQUEST.fields_by_name['project_id']._options = None
 _OPENPROJECTREQUEST.fields_by_name['project_id']._options = None
 _GETPROJECTREQUEST.fields_by_name['project_id']._options = None
 _LISTPROJECTSREQUEST.fields_by_name['folder_id']._options = None
 _LISTPROJECTSREQUEST.fields_by_name['page_size']._options = None
 _LISTPROJECTSREQUEST.fields_by_name['page_token']._options = None
+_GETUNITBALANCEREQUEST.fields_by_name['project_id']._options = None
+_SETUNITBALANCEREQUEST.fields_by_name['project_id']._options = None
 
 _PROJECTSERVICE = _descriptor.ServiceDescriptor(
   name='ProjectService',
   full_name='yandex.cloud.datasphere.v1.ProjectService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1408,
-  serialized_end=2433,
+  serialized_start=1837,
+  serialized_end=3197,
   methods=[
   _descriptor.MethodDescriptor(
     name='Create',
     full_name='yandex.cloud.datasphere.v1.ProjectService.Create',
     index=0,
     containing_service=None,
     input_type=_CREATEPROJECTREQUEST,
@@ -675,13 +824,33 @@
     index=5,
     containing_service=None,
     input_type=_LISTPROJECTSREQUEST,
     output_type=_LISTPROJECTSRESPONSE,
     serialized_options=b'\202\323\344\223\002\031\022\027/datasphere/v1/projects',
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='GetUnitBalance',
+    full_name='yandex.cloud.datasphere.v1.ProjectService.GetUnitBalance',
+    index=6,
+    containing_service=None,
+    input_type=_GETUNITBALANCEREQUEST,
+    output_type=_GETUNITBALANCERESPONSE,
+    serialized_options=b'\202\323\344\223\0022\0220/datasphere/v1/projects/{project_id}:unitBalance',
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetUnitBalance',
+    full_name='yandex.cloud.datasphere.v1.ProjectService.SetUnitBalance',
+    index=7,
+    containing_service=None,
+    input_type=_SETUNITBALANCEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=b'\202\323\344\223\0025\"0/datasphere/v1/projects/{project_id}:unitBalance:\001*',
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_PROJECTSERVICE)
 
 DESCRIPTOR.services_by_name['ProjectService'] = _PROJECTSERVICE
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from yandex.cloud.datasphere.v1 import project_pb2 as yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2
 from yandex.cloud.datasphere.v1 import project_service_pb2 as yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2
 from yandex.cloud.operation import operation_pb2 as yandex_dot_cloud_dot_operation_dot_operation__pb2
 
 
 class ProjectServiceStub(object):
     """A set of methods for managing Project resources.
@@ -43,14 +44,24 @@
                 response_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2.Project.FromString,
                 )
         self.List = channel.unary_unary(
                 '/yandex.cloud.datasphere.v1.ProjectService/List',
                 request_serializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.ListProjectsRequest.SerializeToString,
                 response_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.ListProjectsResponse.FromString,
                 )
+        self.GetUnitBalance = channel.unary_unary(
+                '/yandex.cloud.datasphere.v1.ProjectService/GetUnitBalance',
+                request_serializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.GetUnitBalanceRequest.SerializeToString,
+                response_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.GetUnitBalanceResponse.FromString,
+                )
+        self.SetUnitBalance = channel.unary_unary(
+                '/yandex.cloud.datasphere.v1.ProjectService/SetUnitBalance',
+                request_serializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.SetUnitBalanceRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
 
 
 class ProjectServiceServicer(object):
     """A set of methods for managing Project resources.
     """
 
     def Create(self, request, context):
@@ -91,14 +102,28 @@
     def List(self, request, context):
         """Lists projects for the specified folder.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetUnitBalance(self, request, context):
+        """Returns the unit balance of the specified project.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SetUnitBalance(self, request, context):
+        """Sets the unit balance of the specified project.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ProjectServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Create': grpc.unary_unary_rpc_method_handler(
                     servicer.Create,
                     request_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.CreateProjectRequest.FromString,
                     response_serializer=yandex_dot_cloud_dot_operation_dot_operation__pb2.Operation.SerializeToString,
@@ -124,14 +149,24 @@
                     response_serializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__pb2.Project.SerializeToString,
             ),
             'List': grpc.unary_unary_rpc_method_handler(
                     servicer.List,
                     request_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.ListProjectsRequest.FromString,
                     response_serializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.ListProjectsResponse.SerializeToString,
             ),
+            'GetUnitBalance': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetUnitBalance,
+                    request_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.GetUnitBalanceRequest.FromString,
+                    response_serializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.GetUnitBalanceResponse.SerializeToString,
+            ),
+            'SetUnitBalance': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetUnitBalance,
+                    request_deserializer=yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.SetUnitBalanceRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'yandex.cloud.datasphere.v1.ProjectService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -236,7 +271,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/yandex.cloud.datasphere.v1.ProjectService/List',
             yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.ListProjectsRequest.SerializeToString,
             yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.ListProjectsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUnitBalance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/yandex.cloud.datasphere.v1.ProjectService/GetUnitBalance',
+            yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.GetUnitBalanceRequest.SerializeToString,
+            yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.GetUnitBalanceResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetUnitBalance(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/yandex.cloud.datasphere.v1.ProjectService/SetUnitBalance',
+            yandex_dot_cloud_dot_datasphere_dot_v1_dot_project__service__pb2.SetUnitBalanceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/dns/v1/dns_zone_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/dns/v1/dns_zone_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/endpoint/api_endpoint_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/endpoint/api_endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/iam_token_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/iam_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/key_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/key_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/key_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/role_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/role_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/role_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_data_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_data_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/device_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/device_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/iot/devices/v1/registry_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/iot/devices/v1/registry_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/maintenance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/node_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/node_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/k8s/v1/version_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/k8s/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_crypto_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/kms/v1/symmetric_key_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/kms/v1/symmetric_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/health_check_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/health_check_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/network_load_balancer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/loadbalancer/v1/target_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/lockbox/v1/payload_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/lockbox/v1/payload_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/lockbox/v1/secret_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/lockbox/v1/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_entry_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,224 +1,261 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: yandex/cloud/logging/v1/log_group.proto
+# source: yandex/cloud/mdb/sqlserver/v1/user.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from yandex.cloud import validation_pb2 as yandex_dot_cloud_dot_validation__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='yandex/cloud/logging/v1/log_group.proto',
-  package='yandex.cloud.logging.v1',
+  name='yandex/cloud/mdb/sqlserver/v1/user.proto',
+  package='yandex.cloud.mdb.sqlserver.v1',
   syntax='proto3',
-  serialized_options=b'\n\033yandex.cloud.api.logging.v1ZCgithub.com/yandex-cloud/go-genproto/yandex/cloud/logging/v1;logging',
+  serialized_options=b'\n!yandex.cloud.api.mdb.sqlserver.v1B\003PSUZKgithub.com/yandex-cloud/go-genproto/yandex/cloud/mdb/sqlserver/v1;sqlserver',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\'yandex/cloud/logging/v1/log_group.proto\x12\x17yandex.cloud.logging.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc0\x03\n\x08LogGroup\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12\x10\n\x08\x63loud_id\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12=\n\x06labels\x18\x07 \x03(\x0b\x32-.yandex.cloud.logging.v1.LogGroup.LabelsEntry\x12\x38\n\x06status\x18\x08 \x01(\x0e\x32(.yandex.cloud.logging.v1.LogGroup.Status\x12\x33\n\x10retention_period\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"S\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x44\x45LETING\x10\x03\x12\t\n\x05\x45RROR\x10\x04\x42\x62\n\x1byandex.cloud.api.logging.v1ZCgithub.com/yandex-cloud/go-genproto/yandex/cloud/logging/v1;loggingb\x06proto3'
+  serialized_pb=b'\n(yandex/cloud/mdb/sqlserver/v1/user.proto\x12\x1dyandex.cloud.mdb.sqlserver.v1\x1a\x1dyandex/cloud/validation.proto\"h\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12>\n\x0bpermissions\x18\x03 \x03(\x0b\x32).yandex.cloud.mdb.sqlserver.v1.Permission\"\xbe\x02\n\nPermission\x12\x15\n\rdatabase_name\x18\x01 \x01(\t\x12\x46\n\x05roles\x18\x02 \x03(\x0e\x32..yandex.cloud.mdb.sqlserver.v1.Permission.RoleB\x07\x82\xc8\x31\x03>=1\"\xd0\x01\n\x04Role\x12\x14\n\x10ROLE_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x44\x42_OWNER\x10\x01\x12\x14\n\x10\x44\x42_SECURITYADMIN\x10\x02\x12\x12\n\x0e\x44\x42_ACCESSADMIN\x10\x03\x12\x15\n\x11\x44\x42_BACKUPOPERATOR\x10\x04\x12\x0f\n\x0b\x44\x42_DDLADMIN\x10\x05\x12\x11\n\rDB_DATAWRITER\x10\x06\x12\x11\n\rDB_DATAREADER\x10\x07\x12\x15\n\x11\x44\x42_DENYDATAWRITER\x10\x08\x12\x15\n\x11\x44\x42_DENYDATAREADER\x10\t\"\x98\x01\n\x08UserSpec\x12+\n\x04name\x18\x01 \x01(\tB\x1d\xe8\xc7\x31\x01\x8a\xc8\x31\x04<=32\xf2\xc7\x31\r[a-zA-Z0-9_]*\x12\x1f\n\x08password\x18\x02 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05\x38-128\x12>\n\x0bpermissions\x18\x03 \x03(\x0b\x32).yandex.cloud.mdb.sqlserver.v1.PermissionBu\n!yandex.cloud.api.mdb.sqlserver.v1B\x03PSUZKgithub.com/yandex-cloud/go-genproto/yandex/cloud/mdb/sqlserver/v1;sqlserverb\x06proto3'
   ,
-  dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
+  dependencies=[yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,])
 
 
 
-_LOGGROUP_STATUS = _descriptor.EnumDescriptor(
-  name='Status',
-  full_name='yandex.cloud.logging.v1.LogGroup.Status',
+_PERMISSION_ROLE = _descriptor.EnumDescriptor(
+  name='Role',
+  full_name='yandex.cloud.mdb.sqlserver.v1.Permission.Role',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='STATUS_UNSPECIFIED', index=0, number=0,
+      name='ROLE_UNSPECIFIED', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CREATING', index=1, number=1,
+      name='DB_OWNER', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='ACTIVE', index=2, number=2,
+      name='DB_SECURITYADMIN', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='DELETING', index=3, number=3,
+      name='DB_ACCESSADMIN', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='ERROR', index=4, number=4,
+      name='DB_BACKUPOPERATOR', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DB_DDLADMIN', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DB_DATAWRITER', index=6, number=6,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DB_DATAREADER', index=7, number=7,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DB_DENYDATAWRITER', index=8, number=8,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DB_DENYDATAREADER', index=9, number=9,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=499,
-  serialized_end=582,
+  serialized_start=323,
+  serialized_end=531,
 )
-_sym_db.RegisterEnumDescriptor(_LOGGROUP_STATUS)
+_sym_db.RegisterEnumDescriptor(_PERMISSION_ROLE)
 
 
-_LOGGROUP_LABELSENTRY = _descriptor.Descriptor(
-  name='LabelsEntry',
-  full_name='yandex.cloud.logging.v1.LogGroup.LabelsEntry',
+_USER = _descriptor.Descriptor(
+  name='User',
+  full_name='yandex.cloud.mdb.sqlserver.v1.User',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='yandex.cloud.logging.v1.LogGroup.LabelsEntry.key', index=0,
+      name='name', full_name='yandex.cloud.mdb.sqlserver.v1.User.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='yandex.cloud.logging.v1.LogGroup.LabelsEntry.value', index=1,
+      name='cluster_id', full_name='yandex.cloud.mdb.sqlserver.v1.User.cluster_id', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='permissions', full_name='yandex.cloud.mdb.sqlserver.v1.User.permissions', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
-  serialized_options=b'8\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=452,
-  serialized_end=497,
+  serialized_start=106,
+  serialized_end=210,
 )
 
-_LOGGROUP = _descriptor.Descriptor(
-  name='LogGroup',
-  full_name='yandex.cloud.logging.v1.LogGroup',
+
+_PERMISSION = _descriptor.Descriptor(
+  name='Permission',
+  full_name='yandex.cloud.mdb.sqlserver.v1.Permission',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='yandex.cloud.logging.v1.LogGroup.id', index=0,
+      name='database_name', full_name='yandex.cloud.mdb.sqlserver.v1.Permission.database_name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='folder_id', full_name='yandex.cloud.logging.v1.LogGroup.folder_id', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='cloud_id', full_name='yandex.cloud.logging.v1.LogGroup.cloud_id', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='created_at', full_name='yandex.cloud.logging.v1.LogGroup.created_at', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='roles', full_name='yandex.cloud.mdb.sqlserver.v1.Permission.roles', index=1,
+      number=2, type=14, cpp_type=8, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=b'\202\3101\003>=1', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+    _PERMISSION_ROLE,
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=213,
+  serialized_end=531,
+)
+
+
+_USERSPEC = _descriptor.Descriptor(
+  name='UserSpec',
+  full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='yandex.cloud.logging.v1.LogGroup.name', index=4,
-      number=5, type=9, cpp_type=9, label=1,
+      name='name', full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=b'\350\3071\001\212\3101\004<=32\362\3071\r[a-zA-Z0-9_]*', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='description', full_name='yandex.cloud.logging.v1.LogGroup.description', index=5,
-      number=6, type=9, cpp_type=9, label=1,
+      name='password', full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec.password', index=1,
+      number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=b'\350\3071\001\212\3101\0058-128', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='labels', full_name='yandex.cloud.logging.v1.LogGroup.labels', index=6,
-      number=7, type=11, cpp_type=10, label=3,
+      name='permissions', full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec.permissions', index=2,
+      number=3, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='status', full_name='yandex.cloud.logging.v1.LogGroup.status', index=7,
-      number=8, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='retention_period', full_name='yandex.cloud.logging.v1.LogGroup.retention_period', index=8,
-      number=9, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_LOGGROUP_LABELSENTRY, ],
+  nested_types=[],
   enum_types=[
-    _LOGGROUP_STATUS,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=134,
-  serialized_end=582,
+  serialized_start=534,
+  serialized_end=686,
 )
 
-_LOGGROUP_LABELSENTRY.containing_type = _LOGGROUP
-_LOGGROUP.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
-_LOGGROUP.fields_by_name['labels'].message_type = _LOGGROUP_LABELSENTRY
-_LOGGROUP.fields_by_name['status'].enum_type = _LOGGROUP_STATUS
-_LOGGROUP.fields_by_name['retention_period'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
-_LOGGROUP_STATUS.containing_type = _LOGGROUP
-DESCRIPTOR.message_types_by_name['LogGroup'] = _LOGGROUP
+_USER.fields_by_name['permissions'].message_type = _PERMISSION
+_PERMISSION.fields_by_name['roles'].enum_type = _PERMISSION_ROLE
+_PERMISSION_ROLE.containing_type = _PERMISSION
+_USERSPEC.fields_by_name['permissions'].message_type = _PERMISSION
+DESCRIPTOR.message_types_by_name['User'] = _USER
+DESCRIPTOR.message_types_by_name['Permission'] = _PERMISSION
+DESCRIPTOR.message_types_by_name['UserSpec'] = _USERSPEC
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-LogGroup = _reflection.GeneratedProtocolMessageType('LogGroup', (_message.Message,), {
+User = _reflection.GeneratedProtocolMessageType('User', (_message.Message,), {
+  'DESCRIPTOR' : _USER,
+  '__module__' : 'yandex.cloud.mdb.sqlserver.v1.user_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.mdb.sqlserver.v1.User)
+  })
+_sym_db.RegisterMessage(User)
 
-  'LabelsEntry' : _reflection.GeneratedProtocolMessageType('LabelsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _LOGGROUP_LABELSENTRY,
-    '__module__' : 'yandex.cloud.logging.v1.log_group_pb2'
-    # @@protoc_insertion_point(class_scope:yandex.cloud.logging.v1.LogGroup.LabelsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _LOGGROUP,
-  '__module__' : 'yandex.cloud.logging.v1.log_group_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.logging.v1.LogGroup)
+Permission = _reflection.GeneratedProtocolMessageType('Permission', (_message.Message,), {
+  'DESCRIPTOR' : _PERMISSION,
+  '__module__' : 'yandex.cloud.mdb.sqlserver.v1.user_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.mdb.sqlserver.v1.Permission)
+  })
+_sym_db.RegisterMessage(Permission)
+
+UserSpec = _reflection.GeneratedProtocolMessageType('UserSpec', (_message.Message,), {
+  'DESCRIPTOR' : _USERSPEC,
+  '__module__' : 'yandex.cloud.mdb.sqlserver.v1.user_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.mdb.sqlserver.v1.UserSpec)
   })
-_sym_db.RegisterMessage(LogGroup)
-_sym_db.RegisterMessage(LogGroup.LabelsEntry)
+_sym_db.RegisterMessage(UserSpec)
 
 
 DESCRIPTOR._options = None
-_LOGGROUP_LABELSENTRY._options = None
+_PERMISSION.fields_by_name['roles']._options = None
+_USERSPEC.fields_by_name['name']._options = None
+_USERSPEC.fields_by_name['password']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_ingestion_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_ingestion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_ingestion_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_ingestion_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_reading_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_reading_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_reading_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_reading_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/logging/v1/log_resource_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/logging/v1/log_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/image_product_usage_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/marketplace/v1/metering/usage_record_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/marketplace/v1/metering/usage_record_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/config/clickhouse_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/config/clickhouse_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/format_schema_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/maintenance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/ml_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/version_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/clickhouse/v1/versions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/config/elasticsearch_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/config/elasticsearch_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/elasticsearch/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/common_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/topic_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/kafka/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/kafka/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb3_6_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb3_6_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_0_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_0_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_2_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_2_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_4_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/config/mongodb4_4_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/maintenance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mongodb/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/mysql5_7_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/mysql5_7_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/config/mysql8_0_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/config/mysql8_0_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/maintenance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/config/mysql5_7_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/config/mysql5_7_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/mysql/v1alpha/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host10_1c_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host10_1c_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host10_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host10_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host11_1c_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host11_1c_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host11_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host11_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host12_1c_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host12_1c_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host12_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host12_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host13_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host13_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/host9_6_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/host9_6_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_1c_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_1c_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql10_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_1c_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_1c_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql11_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_1c_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_1c_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql12_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql13_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql13_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/config/postgresql9_6_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/config/postgresql9_6_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/maintenance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/postgresql/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis5_0_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis5_0_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis6_0_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis6_0_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/config/redis6_2_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/config/redis6_2_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/maintenance_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/redis/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/config/sqlserver2016sp2_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/config/sqlserver2016sp2_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,212 +1,243 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: yandex/cloud/mdb/sqlserver/v1/user.proto
+# source: yandex/cloud/vpc/v1/subnet.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from yandex.cloud import validation_pb2 as yandex_dot_cloud_dot_validation__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='yandex/cloud/mdb/sqlserver/v1/user.proto',
-  package='yandex.cloud.mdb.sqlserver.v1',
+  name='yandex/cloud/vpc/v1/subnet.proto',
+  package='yandex.cloud.vpc.v1',
   syntax='proto3',
-  serialized_options=b'\n!yandex.cloud.api.mdb.sqlserver.v1B\003PSUZKgithub.com/yandex-cloud/go-genproto/yandex/cloud/mdb/sqlserver/v1;sqlserver',
+  serialized_options=b'\n\027yandex.cloud.api.vpc.v1Z;github.com/yandex-cloud/go-genproto/yandex/cloud/vpc/v1;vpc',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n(yandex/cloud/mdb/sqlserver/v1/user.proto\x12\x1dyandex.cloud.mdb.sqlserver.v1\x1a\x1dyandex/cloud/validation.proto\"h\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12>\n\x0bpermissions\x18\x03 \x03(\x0b\x32).yandex.cloud.mdb.sqlserver.v1.Permission\"\xbe\x02\n\nPermission\x12\x15\n\rdatabase_name\x18\x01 \x01(\t\x12\x46\n\x05roles\x18\x02 \x03(\x0e\x32..yandex.cloud.mdb.sqlserver.v1.Permission.RoleB\x07\x82\xc8\x31\x03>=1\"\xd0\x01\n\x04Role\x12\x14\n\x10ROLE_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x44\x42_OWNER\x10\x01\x12\x14\n\x10\x44\x42_SECURITYADMIN\x10\x02\x12\x12\n\x0e\x44\x42_ACCESSADMIN\x10\x03\x12\x15\n\x11\x44\x42_BACKUPOPERATOR\x10\x04\x12\x0f\n\x0b\x44\x42_DDLADMIN\x10\x05\x12\x11\n\rDB_DATAWRITER\x10\x06\x12\x11\n\rDB_DATAREADER\x10\x07\x12\x15\n\x11\x44\x42_DENYDATAWRITER\x10\x08\x12\x15\n\x11\x44\x42_DENYDATAREADER\x10\t\"\x98\x01\n\x08UserSpec\x12+\n\x04name\x18\x01 \x01(\tB\x1d\xe8\xc7\x31\x01\x8a\xc8\x31\x04<=32\xf2\xc7\x31\r[a-zA-Z0-9_]*\x12\x1f\n\x08password\x18\x02 \x01(\tB\r\xe8\xc7\x31\x01\x8a\xc8\x31\x05\x38-128\x12>\n\x0bpermissions\x18\x03 \x03(\x0b\x32).yandex.cloud.mdb.sqlserver.v1.PermissionBu\n!yandex.cloud.api.mdb.sqlserver.v1B\x03PSUZKgithub.com/yandex-cloud/go-genproto/yandex/cloud/mdb/sqlserver/v1;sqlserverb\x06proto3'
+  serialized_pb=b'\n yandex/cloud/vpc/v1/subnet.proto\x12\x13yandex.cloud.vpc.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\x87\x03\n\x06Subnet\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x37\n\x06labels\x18\x06 \x03(\x0b\x32\'.yandex.cloud.vpc.v1.Subnet.LabelsEntry\x12\x12\n\nnetwork_id\x18\x07 \x01(\t\x12\x0f\n\x07zone_id\x18\x08 \x01(\t\x12\x16\n\x0ev4_cidr_blocks\x18\n \x03(\t\x12\x16\n\x0ev6_cidr_blocks\x18\x0b \x03(\t\x12\x16\n\x0eroute_table_id\x18\x0c \x01(\t\x12\x36\n\x0c\x64hcp_options\x18\r \x01(\x0b\x32 .yandex.cloud.vpc.v1.DhcpOptions\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"T\n\x0b\x44hcpOptions\x12\x1b\n\x13\x64omain_name_servers\x18\x01 \x03(\t\x12\x13\n\x0b\x64omain_name\x18\x02 \x01(\t\x12\x13\n\x0bntp_servers\x18\x03 \x03(\t*;\n\tIpVersion\x12\x1a\n\x16IP_VERSION_UNSPECIFIED\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x42V\n\x17yandex.cloud.api.vpc.v1Z;github.com/yandex-cloud/go-genproto/yandex/cloud/vpc/v1;vpcb\x06proto3'
   ,
-  dependencies=[yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
-
-
-_PERMISSION_ROLE = _descriptor.EnumDescriptor(
-  name='Role',
-  full_name='yandex.cloud.mdb.sqlserver.v1.Permission.Role',
+_IPVERSION = _descriptor.EnumDescriptor(
+  name='IpVersion',
+  full_name='yandex.cloud.vpc.v1.IpVersion',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='ROLE_UNSPECIFIED', index=0, number=0,
+      name='IP_VERSION_UNSPECIFIED', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='DB_OWNER', index=1, number=1,
+      name='IPV4', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='DB_SECURITYADMIN', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_ACCESSADMIN', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_BACKUPOPERATOR', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_DDLADMIN', index=5, number=5,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_DATAWRITER', index=6, number=6,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_DATAREADER', index=7, number=7,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_DENYDATAWRITER', index=8, number=8,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='DB_DENYDATAREADER', index=9, number=9,
+      name='IPV6', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=323,
-  serialized_end=531,
+  serialized_start=570,
+  serialized_end=629,
 )
-_sym_db.RegisterEnumDescriptor(_PERMISSION_ROLE)
+_sym_db.RegisterEnumDescriptor(_IPVERSION)
+
+IpVersion = enum_type_wrapper.EnumTypeWrapper(_IPVERSION)
+IP_VERSION_UNSPECIFIED = 0
+IPV4 = 1
+IPV6 = 2
 
 
-_USER = _descriptor.Descriptor(
-  name='User',
-  full_name='yandex.cloud.mdb.sqlserver.v1.User',
+
+_SUBNET_LABELSENTRY = _descriptor.Descriptor(
+  name='LabelsEntry',
+  full_name='yandex.cloud.vpc.v1.Subnet.LabelsEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='yandex.cloud.mdb.sqlserver.v1.User.name', index=0,
+      name='key', full_name='yandex.cloud.vpc.v1.Subnet.LabelsEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='cluster_id', full_name='yandex.cloud.mdb.sqlserver.v1.User.cluster_id', index=1,
+      name='value', full_name='yandex.cloud.vpc.v1.Subnet.LabelsEntry.value', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='permissions', full_name='yandex.cloud.mdb.sqlserver.v1.User.permissions', index=2,
-      number=3, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
-  serialized_options=None,
+  serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=106,
-  serialized_end=210,
+  serialized_start=437,
+  serialized_end=482,
 )
 
-
-_PERMISSION = _descriptor.Descriptor(
-  name='Permission',
-  full_name='yandex.cloud.mdb.sqlserver.v1.Permission',
+_SUBNET = _descriptor.Descriptor(
+  name='Subnet',
+  full_name='yandex.cloud.vpc.v1.Subnet',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='database_name', full_name='yandex.cloud.mdb.sqlserver.v1.Permission.database_name', index=0,
+      name='id', full_name='yandex.cloud.vpc.v1.Subnet.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='roles', full_name='yandex.cloud.mdb.sqlserver.v1.Permission.roles', index=1,
-      number=2, type=14, cpp_type=8, label=3,
+      name='folder_id', full_name='yandex.cloud.vpc.v1.Subnet.folder_id', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='created_at', full_name='yandex.cloud.vpc.v1.Subnet.created_at', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='name', full_name='yandex.cloud.vpc.v1.Subnet.name', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='description', full_name='yandex.cloud.vpc.v1.Subnet.description', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='labels', full_name='yandex.cloud.vpc.v1.Subnet.labels', index=5,
+      number=6, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='network_id', full_name='yandex.cloud.vpc.v1.Subnet.network_id', index=6,
+      number=7, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='zone_id', full_name='yandex.cloud.vpc.v1.Subnet.zone_id', index=7,
+      number=8, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='v4_cidr_blocks', full_name='yandex.cloud.vpc.v1.Subnet.v4_cidr_blocks', index=8,
+      number=10, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='v6_cidr_blocks', full_name='yandex.cloud.vpc.v1.Subnet.v6_cidr_blocks', index=9,
+      number=11, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=b'\202\3101\003>=1', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='route_table_id', full_name='yandex.cloud.vpc.v1.Subnet.route_table_id', index=10,
+      number=12, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dhcp_options', full_name='yandex.cloud.vpc.v1.Subnet.dhcp_options', index=11,
+      number=13, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_SUBNET_LABELSENTRY, ],
   enum_types=[
-    _PERMISSION_ROLE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=213,
-  serialized_end=531,
+  serialized_start=91,
+  serialized_end=482,
 )
 
 
-_USERSPEC = _descriptor.Descriptor(
-  name='UserSpec',
-  full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec',
+_DHCPOPTIONS = _descriptor.Descriptor(
+  name='DhcpOptions',
+  full_name='yandex.cloud.vpc.v1.DhcpOptions',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec.name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='domain_name_servers', full_name='yandex.cloud.vpc.v1.DhcpOptions.domain_name_servers', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=b'\350\3071\001\212\3101\004<=32\362\3071\r[a-zA-Z0-9_]*', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='password', full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec.password', index=1,
+      name='domain_name', full_name='yandex.cloud.vpc.v1.DhcpOptions.domain_name', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=b'\350\3071\001\212\3101\0058-128', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='permissions', full_name='yandex.cloud.mdb.sqlserver.v1.UserSpec.permissions', index=2,
-      number=3, type=11, cpp_type=10, label=3,
+      name='ntp_servers', full_name='yandex.cloud.vpc.v1.DhcpOptions.ntp_servers', index=2,
+      number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -215,47 +246,46 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=534,
-  serialized_end=686,
+  serialized_start=484,
+  serialized_end=568,
 )
 
-_USER.fields_by_name['permissions'].message_type = _PERMISSION
-_PERMISSION.fields_by_name['roles'].enum_type = _PERMISSION_ROLE
-_PERMISSION_ROLE.containing_type = _PERMISSION
-_USERSPEC.fields_by_name['permissions'].message_type = _PERMISSION
-DESCRIPTOR.message_types_by_name['User'] = _USER
-DESCRIPTOR.message_types_by_name['Permission'] = _PERMISSION
-DESCRIPTOR.message_types_by_name['UserSpec'] = _USERSPEC
+_SUBNET_LABELSENTRY.containing_type = _SUBNET
+_SUBNET.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_SUBNET.fields_by_name['labels'].message_type = _SUBNET_LABELSENTRY
+_SUBNET.fields_by_name['dhcp_options'].message_type = _DHCPOPTIONS
+DESCRIPTOR.message_types_by_name['Subnet'] = _SUBNET
+DESCRIPTOR.message_types_by_name['DhcpOptions'] = _DHCPOPTIONS
+DESCRIPTOR.enum_types_by_name['IpVersion'] = _IPVERSION
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-User = _reflection.GeneratedProtocolMessageType('User', (_message.Message,), {
-  'DESCRIPTOR' : _USER,
-  '__module__' : 'yandex.cloud.mdb.sqlserver.v1.user_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.mdb.sqlserver.v1.User)
-  })
-_sym_db.RegisterMessage(User)
+Subnet = _reflection.GeneratedProtocolMessageType('Subnet', (_message.Message,), {
 
-Permission = _reflection.GeneratedProtocolMessageType('Permission', (_message.Message,), {
-  'DESCRIPTOR' : _PERMISSION,
-  '__module__' : 'yandex.cloud.mdb.sqlserver.v1.user_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.mdb.sqlserver.v1.Permission)
+  'LabelsEntry' : _reflection.GeneratedProtocolMessageType('LabelsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _SUBNET_LABELSENTRY,
+    '__module__' : 'yandex.cloud.vpc.v1.subnet_pb2'
+    # @@protoc_insertion_point(class_scope:yandex.cloud.vpc.v1.Subnet.LabelsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _SUBNET,
+  '__module__' : 'yandex.cloud.vpc.v1.subnet_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.vpc.v1.Subnet)
   })
-_sym_db.RegisterMessage(Permission)
+_sym_db.RegisterMessage(Subnet)
+_sym_db.RegisterMessage(Subnet.LabelsEntry)
 
-UserSpec = _reflection.GeneratedProtocolMessageType('UserSpec', (_message.Message,), {
-  'DESCRIPTOR' : _USERSPEC,
-  '__module__' : 'yandex.cloud.mdb.sqlserver.v1.user_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.mdb.sqlserver.v1.UserSpec)
+DhcpOptions = _reflection.GeneratedProtocolMessageType('DhcpOptions', (_message.Message,), {
+  'DESCRIPTOR' : _DHCPOPTIONS,
+  '__module__' : 'yandex.cloud.vpc.v1.subnet_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.vpc.v1.DhcpOptions)
   })
-_sym_db.RegisterMessage(UserSpec)
+_sym_db.RegisterMessage(DhcpOptions)
 
 
 DESCRIPTOR._options = None
-_PERMISSION.fields_by_name['roles']._options = None
-_USERSPEC.fields_by_name['name']._options = None
-_USERSPEC.fields_by_name['password']._options = None
+_SUBNET_LABELSENTRY._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/mdb/sqlserver/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/operation/operation_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/operation/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/operation/operation_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/operation/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/operation/operation_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/operation/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/quota/quota_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/quota/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/reference/reference_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/reference/reference_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/cloud_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/resourcemanager/v1/folder_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/resourcemanager/v1/folder_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/apigateway/v1/apigateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yandex/cloud/serverless/functions/v1/function.proto',
   package='yandex.cloud.serverless.functions.v1',
   syntax='proto3',
   serialized_options=b'\n(yandex.cloud.api.serverless.functions.v1ZRgithub.com/yandex-cloud/go-genproto/yandex/cloud/serverless/functions/v1;functions',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n3yandex/cloud/serverless/functions/v1/function.proto\x12$yandex.cloud.serverless.functions.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1dyandex/cloud/validation.proto\"\xe1\x03\n\x08\x46unction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x04name\x18\x04 \x01(\tB\x08\x8a\xc8\x31\x04\x33-63\x12\x1e\n\x0b\x64\x65scription\x18\x05 \x01(\tB\t\x8a\xc8\x31\x05\x30-256\x12T\n\x06labels\x18\x06 \x03(\x0b\x32:.yandex.cloud.serverless.functions.v1.Function.LabelsEntryB\x08\x82\xc8\x31\x04<=64\x12\x14\n\x0clog_group_id\x18\x07 \x01(\t\x12\x17\n\x0fhttp_invoke_url\x18\x08 \x01(\t\x12\x45\n\x06status\x18\t \x01(\x0e\x32\x35.yandex.cloud.serverless.functions.v1.Function.Status\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"S\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x44\x45LETING\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xe8\x06\n\x07Version\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x66unction_id\x18\x02 \x01(\t\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05\x30-256\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07runtime\x18\x06 \x01(\t\x12\x12\n\nentrypoint\x18\x07 \x01(\t\x12\x42\n\tresources\x18\x08 \x01(\x0b\x32/.yandex.cloud.serverless.functions.v1.Resources\x12\x34\n\x11\x65xecution_timeout\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x1a\n\x12service_account_id\x18\n \x01(\t\x12\x12\n\nimage_size\x18\x0c \x01(\x03\x12\x44\n\x06status\x18\r \x01(\x0e\x32\x34.yandex.cloud.serverless.functions.v1.Version.Status\x12\x0c\n\x04tags\x18\x0e \x03(\t\x12\x14\n\x0clog_group_id\x18\x0f \x01(\t\x12S\n\x0b\x65nvironment\x18\x10 \x03(\x0b\x32>.yandex.cloud.serverless.functions.v1.Version.EnvironmentEntry\x12H\n\x0c\x63onnectivity\x18\x11 \x01(\x0b\x32\x32.yandex.cloud.serverless.functions.v1.Connectivity\x12g\n\x16named_service_accounts\x18\x12 \x03(\x0b\x32G.yandex.cloud.serverless.functions.v1.Version.NamedServiceAccountsEntry\x1a\x32\n\x10\x45nvironmentEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a;\n\x19NamedServiceAccountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\"5\n\tResources\x12(\n\x06memory\x18\x01 \x01(\x03\x42\x18\xfa\xc7\x31\x14\x31\x33\x34\x32\x31\x37\x37\x32\x38-2147483648\"O\n\x07Package\x12\x19\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x19\n\x0bobject_name\x18\x02 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x0e\n\x06sha256\x18\x03 \x01(\t\"5\n\x0c\x43onnectivity\x12\x12\n\nnetwork_id\x18\x01 \x01(\t\x12\x11\n\tsubnet_id\x18\x02 \x03(\t\"\xcd\x01\n\rScalingPolicy\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14zone_instances_limit\x18\x07 \x01(\x03\x12\x1b\n\x13zone_requests_limit\x18\x08 \x01(\x03\x42~\n(yandex.cloud.api.serverless.functions.v1ZRgithub.com/yandex-cloud/go-genproto/yandex/cloud/serverless/functions/v1;functionsb\x06proto3'
+  serialized_pb=b'\n3yandex/cloud/serverless/functions/v1/function.proto\x12$yandex.cloud.serverless.functions.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1dyandex/cloud/validation.proto\"\xe1\x03\n\x08\x46unction\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x04name\x18\x04 \x01(\tB\x08\x8a\xc8\x31\x04\x33-63\x12\x1e\n\x0b\x64\x65scription\x18\x05 \x01(\tB\t\x8a\xc8\x31\x05\x30-256\x12T\n\x06labels\x18\x06 \x03(\x0b\x32:.yandex.cloud.serverless.functions.v1.Function.LabelsEntryB\x08\x82\xc8\x31\x04<=64\x12\x14\n\x0clog_group_id\x18\x07 \x01(\t\x12\x17\n\x0fhttp_invoke_url\x18\x08 \x01(\t\x12\x45\n\x06status\x18\t \x01(\x0e\x32\x35.yandex.cloud.serverless.functions.v1.Function.Status\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"S\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x44\x45LETING\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xe8\x06\n\x07Version\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x66unction_id\x18\x02 \x01(\t\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05\x30-256\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07runtime\x18\x06 \x01(\t\x12\x12\n\nentrypoint\x18\x07 \x01(\t\x12\x42\n\tresources\x18\x08 \x01(\x0b\x32/.yandex.cloud.serverless.functions.v1.Resources\x12\x34\n\x11\x65xecution_timeout\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x1a\n\x12service_account_id\x18\n \x01(\t\x12\x12\n\nimage_size\x18\x0c \x01(\x03\x12\x44\n\x06status\x18\r \x01(\x0e\x32\x34.yandex.cloud.serverless.functions.v1.Version.Status\x12\x0c\n\x04tags\x18\x0e \x03(\t\x12\x14\n\x0clog_group_id\x18\x0f \x01(\t\x12S\n\x0b\x65nvironment\x18\x10 \x03(\x0b\x32>.yandex.cloud.serverless.functions.v1.Version.EnvironmentEntry\x12H\n\x0c\x63onnectivity\x18\x11 \x01(\x0b\x32\x32.yandex.cloud.serverless.functions.v1.Connectivity\x12g\n\x16named_service_accounts\x18\x12 \x03(\x0b\x32G.yandex.cloud.serverless.functions.v1.Version.NamedServiceAccountsEntry\x1a\x32\n\x10\x45nvironmentEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a;\n\x19NamedServiceAccountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\"5\n\tResources\x12(\n\x06memory\x18\x01 \x01(\x03\x42\x18\xfa\xc7\x31\x14\x31\x33\x34\x32\x31\x37\x37\x32\x38-2147483648\"O\n\x07Package\x12\x19\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x19\n\x0bobject_name\x18\x02 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x0e\n\x06sha256\x18\x03 \x01(\t\"5\n\x0c\x43onnectivity\x12\x12\n\nnetwork_id\x18\x01 \x01(\t\x12\x11\n\tsubnet_id\x18\x02 \x03(\t\"\xf7\x01\n\rScalingPolicy\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n zone_provisioned_instances_count\x18\x06 \x01(\x03\x12\x1c\n\x14zone_instances_limit\x18\x07 \x01(\x03\x12\x1b\n\x13zone_requests_limit\x18\x08 \x01(\x03\x42~\n(yandex.cloud.api.serverless.functions.v1ZRgithub.com/yandex-cloud/go-genproto/yandex/cloud/serverless/functions/v1;functionsb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,])
 
 
 
 _FUNCTION_STATUS = _descriptor.EnumDescriptor(
   name='Status',
@@ -590,22 +590,29 @@
       name='modified_at', full_name='yandex.cloud.serverless.functions.v1.ScalingPolicy.modified_at', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='zone_instances_limit', full_name='yandex.cloud.serverless.functions.v1.ScalingPolicy.zone_instances_limit', index=4,
+      name='zone_provisioned_instances_count', full_name='yandex.cloud.serverless.functions.v1.ScalingPolicy.zone_provisioned_instances_count', index=4,
+      number=6, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='zone_instances_limit', full_name='yandex.cloud.serverless.functions.v1.ScalingPolicy.zone_instances_limit', index=5,
       number=7, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='zone_requests_limit', full_name='yandex.cloud.serverless.functions.v1.ScalingPolicy.zone_requests_limit', index=5,
+      name='zone_requests_limit', full_name='yandex.cloud.serverless.functions.v1.ScalingPolicy.zone_requests_limit', index=6,
       number=8, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -616,15 +623,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1740,
-  serialized_end=1945,
+  serialized_end=1987,
 )
 
 _FUNCTION_LABELSENTRY.containing_type = _FUNCTION
 _FUNCTION.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _FUNCTION.fields_by_name['labels'].message_type = _FUNCTION_LABELSENTRY
 _FUNCTION.fields_by_name['status'].enum_type = _FUNCTION_STATUS
 _FUNCTION_STATUS.containing_type = _FUNCTION
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yandex/cloud/serverless/functions/v1/function_service.proto',
   package='yandex.cloud.serverless.functions.v1',
   syntax='proto3',
   serialized_options=b'\n(yandex.cloud.api.serverless.functions.v1ZRgithub.com/yandex-cloud/go-genproto/yandex/cloud/serverless/functions/v1;functions',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n;yandex/cloud/serverless/functions/v1/function_service.proto\x12$yandex.cloud.serverless.functions.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a yandex/cloud/api/operation.proto\x1a yandex/cloud/access/access.proto\x1a\x33yandex/cloud/serverless/functions/v1/function.proto\x1a&yandex/cloud/operation/operation.proto\x1a\x1dyandex/cloud/validation.proto\"/\n\x12GetFunctionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\">\n\x19GetFunctionVersionRequest\x12!\n\x13\x66unction_version_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\"h\n\x1eGetFunctionVersionByTagRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12+\n\x03tag\x18\x02 \x01(\tB\x1e\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\"f\n\x14ListFunctionsRequest\x12\x17\n\tfolder_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x11\n\tpage_size\x18\x02 \x01(\x03\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\"s\n\x15ListFunctionsResponse\x12\x41\n\tfunctions\x18\x01 \x03(\x0b\x32..yandex.cloud.serverless.functions.v1.Function\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xcb\x02\n\x15\x43reateFunctionRequest\x12\x17\n\tfolder_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x04name\x18\x02 \x01(\tB!\xf2\xc7\x31\x1d|[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12\x98\x01\n\x06labels\x18\x04 \x03(\x0b\x32G.yandex.cloud.serverless.functions.v1.CreateFunctionRequest.LabelsEntryB?\x82\xc8\x31\x04<=64\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x0b[-_0-9a-z]*\xb2\xc8\x31\x06\x1a\x04\x31-63\xb2\xc8\x31\x12\x12\x10[a-z][-_0-9a-z]*\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x16\x43reateFunctionMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"\xfe\x02\n\x15UpdateFunctionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12/\n\x04name\x18\x03 \x01(\tB!\xf2\xc7\x31\x1d|[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x1e\n\x0b\x64\x65scription\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12\x98\x01\n\x06labels\x18\x05 \x03(\x0b\x32G.yandex.cloud.serverless.functions.v1.UpdateFunctionRequest.LabelsEntryB?\x82\xc8\x31\x04<=64\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x0b[-_0-9a-z]*\xb2\xc8\x31\x06\x1a\x04\x31-63\xb2\xc8\x31\x12\x12\x10[a-z][-_0-9a-z]*\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x16UpdateFunctionMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"2\n\x15\x44\x65leteFunctionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\"-\n\x16\x44\x65leteFunctionMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"\x15\n\x13ListRuntimesRequest\"(\n\x14ListRuntimesResponse\x12\x10\n\x08runtimes\x18\x01 \x03(\t\"\xb0\x01\n\x1cListFunctionsVersionsRequest\x12\x13\n\tfolder_id\x18\x01 \x01(\tH\x00\x12\x15\n\x0b\x66unction_id\x18\x02 \x01(\tH\x00\x12\x1d\n\tpage_size\x18\x03 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=100\x12\x1a\n\x06\x66ilter\x18\x05 \x01(\tB\n\x8a\xc8\x31\x06<=1000B\n\n\x02id\x12\x04\xc0\xc1\x31\x01\"y\n\x1dListFunctionsVersionsResponse\x12?\n\x08versions\x18\x01 \x03(\x0b\x32-.yandex.cloud.serverless.functions.v1.Version\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x94\x01\n\x1dListFunctionOperationsRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x1d\n\tpage_size\x18\x02 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=100\x12\x1a\n\x06\x66ilter\x18\x04 \x01(\tB\n\x8a\xc8\x31\x06<=1000\"p\n\x1eListFunctionOperationsResponse\x12\x35\n\noperations\x18\x01 \x03(\x0b\x32!.yandex.cloud.operation.Operation\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xad\x07\n\x1c\x43reateFunctionVersionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x15\n\x07runtime\x18\x02 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05\x30-256\x12\x18\n\nentrypoint\x18\x04 \x01(\tB\x04\xe8\xc7\x31\x01\x12H\n\tresources\x18\x05 \x01(\x0b\x32/.yandex.cloud.serverless.functions.v1.ResourcesB\x04\xe8\xc7\x31\x01\x12:\n\x11\x65xecution_timeout\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB\x04\xe8\xc7\x31\x01\x12\x1a\n\x12service_account_id\x18\x07 \x01(\t\x12@\n\x07package\x18\t \x01(\x0b\x32-.yandex.cloud.serverless.functions.v1.PackageH\x00\x12!\n\x07\x63ontent\x18\n \x01(\x0c\x42\x0e\x8a\xc8\x31\n<=52428800H\x00\x12\x14\n\nversion_id\x18\x0b \x01(\tH\x00\x12\x8f\x01\n\x0b\x65nvironment\x18\x0c \x03(\x0b\x32S.yandex.cloud.serverless.functions.v1.CreateFunctionVersionRequest.EnvironmentEntryB%\x8a\xc8\x31\x06<=4096\xb2\xc8\x31\x17\x12\x15[a-zA-Z][a-zA-Z0-9_]*\x12!\n\x03tag\x18\r \x03(\tB\x14\xf2\xc7\x31\x10[a-z][-_0-9a-z]*\x12H\n\x0c\x63onnectivity\x18\x11 \x01(\x0b\x32\x32.yandex.cloud.serverless.functions.v1.Connectivity\x12|\n\x16named_service_accounts\x18\x0f \x03(\x0b\x32\\.yandex.cloud.serverless.functions.v1.CreateFunctionVersionRequest.NamedServiceAccountsEntry\x1a\x32\n\x10\x45nvironmentEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a;\n\x19NamedServiceAccountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x16\n\x0epackage_source\x12\x04\xc0\xc1\x31\x01\"<\n\x1d\x43reateFunctionVersionMetadata\x12\x1b\n\x13\x66unction_version_id\x18\x01 \x01(\t\"]\n\x15SetFunctionTagRequest\x12!\n\x13\x66unction_version_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12!\n\x03tag\x18\x02 \x01(\tB\x14\xf2\xc7\x31\x10[a-z][-_0-9a-z]*\"`\n\x18RemoveFunctionTagRequest\x12!\n\x13\x66unction_version_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12!\n\x03tag\x18\x02 \x01(\tB\x14\xf2\xc7\x31\x10[a-z][-_0-9a-z]*\"5\n\x16SetFunctionTagMetadata\x12\x1b\n\x13\x66unction_version_id\x18\x01 \x01(\t\"8\n\x19RemoveFunctionTagMetadata\x12\x1b\n\x13\x66unction_version_id\x18\x01 \x01(\t\"\xc1\x01\n\x1dListFunctionTagHistoryRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12+\n\x03tag\x18\x02 \x01(\tB\x1e\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\x12\x1d\n\tpage_size\x18\x03 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=100\x12\x1a\n\x06\x66ilter\x18\x05 \x01(\tB\n\x8a\xc8\x31\x06<=1000\"\x80\x03\n\x1eListFunctionTagHistoryResponse\x12\x82\x01\n\x1b\x66unction_tag_history_record\x18\x01 \x03(\x0b\x32].yandex.cloud.serverless.functions.v1.ListFunctionTagHistoryResponse.FunctionTagHistoryRecord\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x1a\xbf\x01\n\x18\x46unctionTagHistoryRecord\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66unction_version_id\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x12\x32\n\x0e\x65\x66\x66\x65\x63tive_from\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65\x66\x66\x65\x63tive_to\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"u\n\x1aListScalingPoliciesRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x1d\n\tpage_size\x18\x02 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=100\"\x85\x01\n\x1bListScalingPoliciesResponse\x12M\n\x10scaling_policies\x18\x01 \x03(\x0b\x32\x33.yandex.cloud.serverless.functions.v1.ScalingPolicy\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xb8\x01\n\x17SetScalingPolicyRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x03tag\x18\x02 \x01(\tB\"\xe8\xc7\x31\x01\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\x12(\n\x14zone_instances_limit\x18\x05 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\'\n\x13zone_requests_limit\x18\x06 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\"/\n\x18SetScalingPolicyMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"h\n\x1aRemoveScalingPolicyRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x03tag\x18\x02 \x01(\tB\"\xe8\xc7\x31\x01\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\"2\n\x1bRemoveScalingPolicyMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t2\xdb\x1f\n\x0f\x46unctionService\x12\x9e\x01\n\x03Get\x12\x38.yandex.cloud.serverless.functions.v1.GetFunctionRequest\x1a..yandex.cloud.serverless.functions.v1.Function\"-\x82\xd3\xe4\x93\x02\'\x12%/functions/v1/functions/{function_id}\x12\xa0\x01\n\x04List\x12:.yandex.cloud.serverless.functions.v1.ListFunctionsRequest\x1a;.yandex.cloud.serverless.functions.v1.ListFunctionsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/functions/v1/functions\x12\xb2\x01\n\x06\x43reate\x12;.yandex.cloud.serverless.functions.v1.CreateFunctionRequest\x1a!.yandex.cloud.operation.Operation\"H\x82\xd3\xe4\x93\x02\x1c\"\x17/functions/v1/functions:\x01*\xb2\xd2*\"\n\x16\x43reateFunctionMetadata\x12\x08\x46unction\x12\xc0\x01\n\x06Update\x12;.yandex.cloud.serverless.functions.v1.UpdateFunctionRequest\x1a!.yandex.cloud.operation.Operation\"V\x82\xd3\xe4\x93\x02*2%/functions/v1/functions/{function_id}:\x01*\xb2\xd2*\"\n\x16UpdateFunctionMetadata\x12\x08\x46unction\x12\xca\x01\n\x06\x44\x65lete\x12;.yandex.cloud.serverless.functions.v1.DeleteFunctionRequest\x1a!.yandex.cloud.operation.Operation\"`\x82\xd3\xe4\x93\x02\'*%/functions/v1/functions/{function_id}\xb2\xd2*/\n\x16\x44\x65leteFunctionMetadata\x12\x15google.protobuf.Empty\x12\xb2\x01\n\nGetVersion\x12?.yandex.cloud.serverless.functions.v1.GetFunctionVersionRequest\x1a-.yandex.cloud.serverless.functions.v1.Version\"4\x82\xd3\xe4\x93\x02.\x12,/functions/v1/versions/{function_version_id}\x12\xac\x01\n\x0fGetVersionByTag\x12\x44.yandex.cloud.serverless.functions.v1.GetFunctionVersionByTagRequest\x1a-.yandex.cloud.serverless.functions.v1.Version\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/functions/v1/versions:byTag\x12\xb7\x01\n\x0cListVersions\x12\x42.yandex.cloud.serverless.functions.v1.ListFunctionsVersionsRequest\x1a\x43.yandex.cloud.serverless.functions.v1.ListFunctionsVersionsResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/functions/v1/versions\x12\xcd\x01\n\x06SetTag\x12;.yandex.cloud.serverless.functions.v1.SetFunctionTagRequest\x1a!.yandex.cloud.operation.Operation\"c\x82\xd3\xe4\x93\x02\x38\"3/functions/v1/versions/{function_version_id}:setTag:\x01*\xb2\xd2*!\n\x16SetFunctionTagMetadata\x12\x07Version\x12\xd9\x01\n\tRemoveTag\x12>.yandex.cloud.serverless.functions.v1.RemoveFunctionTagRequest\x1a!.yandex.cloud.operation.Operation\"i\x82\xd3\xe4\x93\x02;\"6/functions/v1/versions/{function_version_id}:removeTag:\x01*\xb2\xd2*$\n\x19RemoveFunctionTagMetadata\x12\x07Version\x12\xd5\x01\n\x0eListTagHistory\x12\x43.yandex.cloud.serverless.functions.v1.ListFunctionTagHistoryRequest\x1a\x44.yandex.cloud.serverless.functions.v1.ListFunctionTagHistoryResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/functions/v1/functions/{function_id}:tagHistory\x12\xc5\x01\n\rCreateVersion\x12\x42.yandex.cloud.serverless.functions.v1.CreateFunctionVersionRequest\x1a!.yandex.cloud.operation.Operation\"M\x82\xd3\xe4\x93\x02\x1b\"\x16/functions/v1/versions:\x01*\xb2\xd2*(\n\x1d\x43reateFunctionVersionMetadata\x12\x07Version\x12\xa5\x01\n\x0cListRuntimes\x12\x39.yandex.cloud.serverless.functions.v1.ListRuntimesRequest\x1a:.yandex.cloud.serverless.functions.v1.ListRuntimesResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/functions/v1/runtimes\x12\xd5\x01\n\x0eListOperations\x12\x43.yandex.cloud.serverless.functions.v1.ListFunctionOperationsRequest\x1a\x44.yandex.cloud.serverless.functions.v1.ListFunctionOperationsResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/functions/v1/functions/{function_id}/operations\x12\xb7\x01\n\x12ListAccessBindings\x12..yandex.cloud.access.ListAccessBindingsRequest\x1a/.yandex.cloud.access.ListAccessBindingsResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/functions/v1/functions/{resource_id}:listAccessBindings\x12\xe6\x01\n\x11SetAccessBindings\x12-.yandex.cloud.access.SetAccessBindingsRequest\x1a!.yandex.cloud.operation.Operation\"\x7f\x82\xd3\xe4\x93\x02<\"7/functions/v1/functions/{resource_id}:setAccessBindings:\x01*\xb2\xd2*9\n access.SetAccessBindingsMetadata\x12\x15google.protobuf.Empty\x12\xf3\x01\n\x14UpdateAccessBindings\x12\x30.yandex.cloud.access.UpdateAccessBindingsRequest\x1a!.yandex.cloud.operation.Operation\"\x85\x01\x82\xd3\xe4\x93\x02?\":/functions/v1/functions/{resource_id}:updateAccessBindings:\x01*\xb2\xd2*<\n#access.UpdateAccessBindingsMetadata\x12\x15google.protobuf.Empty\x12\xd9\x01\n\x13ListScalingPolicies\x12@.yandex.cloud.serverless.functions.v1.ListScalingPoliciesRequest\x1a\x41.yandex.cloud.serverless.functions.v1.ListScalingPoliciesResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/functions/v1/functions/{function_id}/scalingPolicies\x12\xe4\x01\n\x10SetScalingPolicy\x12=.yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest\x1a!.yandex.cloud.operation.Operation\"n\x82\xd3\xe4\x93\x02;\"6/functions/v1/functions/{function_id}:setScalingPolicy:\x01*\xb2\xd2*)\n\x18SetScalingPolicyMetadata\x12\rScalingPolicy\x12\xf8\x01\n\x13RemoveScalingPolicy\x12@.yandex.cloud.serverless.functions.v1.RemoveScalingPolicyRequest\x1a!.yandex.cloud.operation.Operation\"|\x82\xd3\xe4\x93\x02>\"9/functions/v1/functions/{function_id}:removeScalingPolicy:\x01*\xb2\xd2*4\n\x1bRemoveScalingPolicyMetadata\x12\x15google.protobuf.EmptyB~\n(yandex.cloud.api.serverless.functions.v1ZRgithub.com/yandex-cloud/go-genproto/yandex/cloud/serverless/functions/v1;functionsb\x06proto3'
+  serialized_pb=b'\n;yandex/cloud/serverless/functions/v1/function_service.proto\x12$yandex.cloud.serverless.functions.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a yandex/cloud/api/operation.proto\x1a yandex/cloud/access/access.proto\x1a\x33yandex/cloud/serverless/functions/v1/function.proto\x1a&yandex/cloud/operation/operation.proto\x1a\x1dyandex/cloud/validation.proto\"/\n\x12GetFunctionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\">\n\x19GetFunctionVersionRequest\x12!\n\x13\x66unction_version_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\"h\n\x1eGetFunctionVersionByTagRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12+\n\x03tag\x18\x02 \x01(\tB\x1e\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\"f\n\x14ListFunctionsRequest\x12\x17\n\tfolder_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x11\n\tpage_size\x18\x02 \x01(\x03\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t\"s\n\x15ListFunctionsResponse\x12\x41\n\tfunctions\x18\x01 \x03(\x0b\x32..yandex.cloud.serverless.functions.v1.Function\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xcb\x02\n\x15\x43reateFunctionRequest\x12\x17\n\tfolder_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x04name\x18\x02 \x01(\tB!\xf2\xc7\x31\x1d|[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12\x98\x01\n\x06labels\x18\x04 \x03(\x0b\x32G.yandex.cloud.serverless.functions.v1.CreateFunctionRequest.LabelsEntryB?\x82\xc8\x31\x04<=64\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x0b[-_0-9a-z]*\xb2\xc8\x31\x06\x1a\x04\x31-63\xb2\xc8\x31\x12\x12\x10[a-z][-_0-9a-z]*\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x16\x43reateFunctionMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"\xfe\x02\n\x15UpdateFunctionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12/\n\x04name\x18\x03 \x01(\tB!\xf2\xc7\x31\x1d|[a-z][-a-z0-9]{1,61}[a-z0-9]\x12\x1e\n\x0b\x64\x65scription\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=256\x12\x98\x01\n\x06labels\x18\x05 \x03(\x0b\x32G.yandex.cloud.serverless.functions.v1.UpdateFunctionRequest.LabelsEntryB?\x82\xc8\x31\x04<=64\x8a\xc8\x31\x04<=63\xf2\xc7\x31\x0b[-_0-9a-z]*\xb2\xc8\x31\x06\x1a\x04\x31-63\xb2\xc8\x31\x12\x12\x10[a-z][-_0-9a-z]*\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x16UpdateFunctionMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"2\n\x15\x44\x65leteFunctionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\"-\n\x16\x44\x65leteFunctionMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"\x15\n\x13ListRuntimesRequest\"(\n\x14ListRuntimesResponse\x12\x10\n\x08runtimes\x18\x01 \x03(\t\"\xb0\x01\n\x1cListFunctionsVersionsRequest\x12\x13\n\tfolder_id\x18\x01 \x01(\tH\x00\x12\x15\n\x0b\x66unction_id\x18\x02 \x01(\tH\x00\x12\x1d\n\tpage_size\x18\x03 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=100\x12\x1a\n\x06\x66ilter\x18\x05 \x01(\tB\n\x8a\xc8\x31\x06<=1000B\n\n\x02id\x12\x04\xc0\xc1\x31\x01\"y\n\x1dListFunctionsVersionsResponse\x12?\n\x08versions\x18\x01 \x03(\x0b\x32-.yandex.cloud.serverless.functions.v1.Version\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x94\x01\n\x1dListFunctionOperationsRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x1d\n\tpage_size\x18\x02 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=100\x12\x1a\n\x06\x66ilter\x18\x04 \x01(\tB\n\x8a\xc8\x31\x06<=1000\"p\n\x1eListFunctionOperationsResponse\x12\x35\n\noperations\x18\x01 \x03(\x0b\x32!.yandex.cloud.operation.Operation\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xad\x07\n\x1c\x43reateFunctionVersionRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x15\n\x07runtime\x18\x02 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x1e\n\x0b\x64\x65scription\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05\x30-256\x12\x18\n\nentrypoint\x18\x04 \x01(\tB\x04\xe8\xc7\x31\x01\x12H\n\tresources\x18\x05 \x01(\x0b\x32/.yandex.cloud.serverless.functions.v1.ResourcesB\x04\xe8\xc7\x31\x01\x12:\n\x11\x65xecution_timeout\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB\x04\xe8\xc7\x31\x01\x12\x1a\n\x12service_account_id\x18\x07 \x01(\t\x12@\n\x07package\x18\t \x01(\x0b\x32-.yandex.cloud.serverless.functions.v1.PackageH\x00\x12!\n\x07\x63ontent\x18\n \x01(\x0c\x42\x0e\x8a\xc8\x31\n<=52428800H\x00\x12\x14\n\nversion_id\x18\x0b \x01(\tH\x00\x12\x8f\x01\n\x0b\x65nvironment\x18\x0c \x03(\x0b\x32S.yandex.cloud.serverless.functions.v1.CreateFunctionVersionRequest.EnvironmentEntryB%\x8a\xc8\x31\x06<=4096\xb2\xc8\x31\x17\x12\x15[a-zA-Z][a-zA-Z0-9_]*\x12!\n\x03tag\x18\r \x03(\tB\x14\xf2\xc7\x31\x10[a-z][-_0-9a-z]*\x12H\n\x0c\x63onnectivity\x18\x11 \x01(\x0b\x32\x32.yandex.cloud.serverless.functions.v1.Connectivity\x12|\n\x16named_service_accounts\x18\x0f \x03(\x0b\x32\\.yandex.cloud.serverless.functions.v1.CreateFunctionVersionRequest.NamedServiceAccountsEntry\x1a\x32\n\x10\x45nvironmentEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a;\n\x19NamedServiceAccountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x16\n\x0epackage_source\x12\x04\xc0\xc1\x31\x01\"<\n\x1d\x43reateFunctionVersionMetadata\x12\x1b\n\x13\x66unction_version_id\x18\x01 \x01(\t\"]\n\x15SetFunctionTagRequest\x12!\n\x13\x66unction_version_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12!\n\x03tag\x18\x02 \x01(\tB\x14\xf2\xc7\x31\x10[a-z][-_0-9a-z]*\"`\n\x18RemoveFunctionTagRequest\x12!\n\x13\x66unction_version_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12!\n\x03tag\x18\x02 \x01(\tB\x14\xf2\xc7\x31\x10[a-z][-_0-9a-z]*\"5\n\x16SetFunctionTagMetadata\x12\x1b\n\x13\x66unction_version_id\x18\x01 \x01(\t\"8\n\x19RemoveFunctionTagMetadata\x12\x1b\n\x13\x66unction_version_id\x18\x01 \x01(\t\"\xc1\x01\n\x1dListFunctionTagHistoryRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12+\n\x03tag\x18\x02 \x01(\tB\x1e\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\x12\x1d\n\tpage_size\x18\x03 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x04 \x01(\tB\t\x8a\xc8\x31\x05<=100\x12\x1a\n\x06\x66ilter\x18\x05 \x01(\tB\n\x8a\xc8\x31\x06<=1000\"\x80\x03\n\x1eListFunctionTagHistoryResponse\x12\x82\x01\n\x1b\x66unction_tag_history_record\x18\x01 \x03(\x0b\x32].yandex.cloud.serverless.functions.v1.ListFunctionTagHistoryResponse.FunctionTagHistoryRecord\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x1a\xbf\x01\n\x18\x46unctionTagHistoryRecord\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66unction_version_id\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x12\x32\n\x0e\x65\x66\x66\x65\x63tive_from\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65\x66\x66\x65\x63tive_to\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"u\n\x1aListScalingPoliciesRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12\x1d\n\tpage_size\x18\x02 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\x1d\n\npage_token\x18\x03 \x01(\tB\t\x8a\xc8\x31\x05<=100\"\x85\x01\n\x1bListScalingPoliciesResponse\x12M\n\x10scaling_policies\x18\x01 \x03(\x0b\x32\x33.yandex.cloud.serverless.functions.v1.ScalingPolicy\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xee\x01\n\x17SetScalingPolicyRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x03tag\x18\x02 \x01(\tB\"\xe8\xc7\x31\x01\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\x12\x34\n zone_provisioned_instances_count\x18\x04 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12(\n\x14zone_instances_limit\x18\x05 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\x12\'\n\x13zone_requests_limit\x18\x06 \x01(\x03\x42\n\xfa\xc7\x31\x06\x30-1000\"/\n\x18SetScalingPolicyMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t\"h\n\x1aRemoveScalingPolicyRequest\x12\x19\n\x0b\x66unction_id\x18\x01 \x01(\tB\x04\xe8\xc7\x31\x01\x12/\n\x03tag\x18\x02 \x01(\tB\"\xe8\xc7\x31\x01\xf2\xc7\x31\x1a[a-z][-_0-9a-z]*|[$]latest\"2\n\x1bRemoveScalingPolicyMetadata\x12\x13\n\x0b\x66unction_id\x18\x01 \x01(\t2\xdb\x1f\n\x0f\x46unctionService\x12\x9e\x01\n\x03Get\x12\x38.yandex.cloud.serverless.functions.v1.GetFunctionRequest\x1a..yandex.cloud.serverless.functions.v1.Function\"-\x82\xd3\xe4\x93\x02\'\x12%/functions/v1/functions/{function_id}\x12\xa0\x01\n\x04List\x12:.yandex.cloud.serverless.functions.v1.ListFunctionsRequest\x1a;.yandex.cloud.serverless.functions.v1.ListFunctionsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/functions/v1/functions\x12\xb2\x01\n\x06\x43reate\x12;.yandex.cloud.serverless.functions.v1.CreateFunctionRequest\x1a!.yandex.cloud.operation.Operation\"H\x82\xd3\xe4\x93\x02\x1c\"\x17/functions/v1/functions:\x01*\xb2\xd2*\"\n\x16\x43reateFunctionMetadata\x12\x08\x46unction\x12\xc0\x01\n\x06Update\x12;.yandex.cloud.serverless.functions.v1.UpdateFunctionRequest\x1a!.yandex.cloud.operation.Operation\"V\x82\xd3\xe4\x93\x02*2%/functions/v1/functions/{function_id}:\x01*\xb2\xd2*\"\n\x16UpdateFunctionMetadata\x12\x08\x46unction\x12\xca\x01\n\x06\x44\x65lete\x12;.yandex.cloud.serverless.functions.v1.DeleteFunctionRequest\x1a!.yandex.cloud.operation.Operation\"`\x82\xd3\xe4\x93\x02\'*%/functions/v1/functions/{function_id}\xb2\xd2*/\n\x16\x44\x65leteFunctionMetadata\x12\x15google.protobuf.Empty\x12\xb2\x01\n\nGetVersion\x12?.yandex.cloud.serverless.functions.v1.GetFunctionVersionRequest\x1a-.yandex.cloud.serverless.functions.v1.Version\"4\x82\xd3\xe4\x93\x02.\x12,/functions/v1/versions/{function_version_id}\x12\xac\x01\n\x0fGetVersionByTag\x12\x44.yandex.cloud.serverless.functions.v1.GetFunctionVersionByTagRequest\x1a-.yandex.cloud.serverless.functions.v1.Version\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/functions/v1/versions:byTag\x12\xb7\x01\n\x0cListVersions\x12\x42.yandex.cloud.serverless.functions.v1.ListFunctionsVersionsRequest\x1a\x43.yandex.cloud.serverless.functions.v1.ListFunctionsVersionsResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/functions/v1/versions\x12\xcd\x01\n\x06SetTag\x12;.yandex.cloud.serverless.functions.v1.SetFunctionTagRequest\x1a!.yandex.cloud.operation.Operation\"c\x82\xd3\xe4\x93\x02\x38\"3/functions/v1/versions/{function_version_id}:setTag:\x01*\xb2\xd2*!\n\x16SetFunctionTagMetadata\x12\x07Version\x12\xd9\x01\n\tRemoveTag\x12>.yandex.cloud.serverless.functions.v1.RemoveFunctionTagRequest\x1a!.yandex.cloud.operation.Operation\"i\x82\xd3\xe4\x93\x02;\"6/functions/v1/versions/{function_version_id}:removeTag:\x01*\xb2\xd2*$\n\x19RemoveFunctionTagMetadata\x12\x07Version\x12\xd5\x01\n\x0eListTagHistory\x12\x43.yandex.cloud.serverless.functions.v1.ListFunctionTagHistoryRequest\x1a\x44.yandex.cloud.serverless.functions.v1.ListFunctionTagHistoryResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/functions/v1/functions/{function_id}:tagHistory\x12\xc5\x01\n\rCreateVersion\x12\x42.yandex.cloud.serverless.functions.v1.CreateFunctionVersionRequest\x1a!.yandex.cloud.operation.Operation\"M\x82\xd3\xe4\x93\x02\x1b\"\x16/functions/v1/versions:\x01*\xb2\xd2*(\n\x1d\x43reateFunctionVersionMetadata\x12\x07Version\x12\xa5\x01\n\x0cListRuntimes\x12\x39.yandex.cloud.serverless.functions.v1.ListRuntimesRequest\x1a:.yandex.cloud.serverless.functions.v1.ListRuntimesResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/functions/v1/runtimes\x12\xd5\x01\n\x0eListOperations\x12\x43.yandex.cloud.serverless.functions.v1.ListFunctionOperationsRequest\x1a\x44.yandex.cloud.serverless.functions.v1.ListFunctionOperationsResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/functions/v1/functions/{function_id}/operations\x12\xb7\x01\n\x12ListAccessBindings\x12..yandex.cloud.access.ListAccessBindingsRequest\x1a/.yandex.cloud.access.ListAccessBindingsResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/functions/v1/functions/{resource_id}:listAccessBindings\x12\xe6\x01\n\x11SetAccessBindings\x12-.yandex.cloud.access.SetAccessBindingsRequest\x1a!.yandex.cloud.operation.Operation\"\x7f\x82\xd3\xe4\x93\x02<\"7/functions/v1/functions/{resource_id}:setAccessBindings:\x01*\xb2\xd2*9\n access.SetAccessBindingsMetadata\x12\x15google.protobuf.Empty\x12\xf3\x01\n\x14UpdateAccessBindings\x12\x30.yandex.cloud.access.UpdateAccessBindingsRequest\x1a!.yandex.cloud.operation.Operation\"\x85\x01\x82\xd3\xe4\x93\x02?\":/functions/v1/functions/{resource_id}:updateAccessBindings:\x01*\xb2\xd2*<\n#access.UpdateAccessBindingsMetadata\x12\x15google.protobuf.Empty\x12\xd9\x01\n\x13ListScalingPolicies\x12@.yandex.cloud.serverless.functions.v1.ListScalingPoliciesRequest\x1a\x41.yandex.cloud.serverless.functions.v1.ListScalingPoliciesResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/functions/v1/functions/{function_id}/scalingPolicies\x12\xe4\x01\n\x10SetScalingPolicy\x12=.yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest\x1a!.yandex.cloud.operation.Operation\"n\x82\xd3\xe4\x93\x02;\"6/functions/v1/functions/{function_id}:setScalingPolicy:\x01*\xb2\xd2*)\n\x18SetScalingPolicyMetadata\x12\rScalingPolicy\x12\xf8\x01\n\x13RemoveScalingPolicy\x12@.yandex.cloud.serverless.functions.v1.RemoveScalingPolicyRequest\x1a!.yandex.cloud.operation.Operation\"|\x82\xd3\xe4\x93\x02>\"9/functions/v1/functions/{function_id}:removeScalingPolicy:\x01*\xb2\xd2*4\n\x1bRemoveScalingPolicyMetadata\x12\x15google.protobuf.EmptyB~\n(yandex.cloud.api.serverless.functions.v1ZRgithub.com/yandex-cloud/go-genproto/yandex/cloud/serverless/functions/v1;functionsb\x06proto3'
   ,
   dependencies=[google_dot_api_dot_annotations__pb2.DESCRIPTOR,google_dot_protobuf_dot_field__mask__pb2.DESCRIPTOR,google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,yandex_dot_cloud_dot_api_dot_operation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_access_dot_access__pb2.DESCRIPTOR,yandex_dot_cloud_dot_serverless_dot_functions_dot_v1_dot_function__pb2.DESCRIPTOR,yandex_dot_cloud_dot_operation_dot_operation__pb2.DESCRIPTOR,yandex_dot_cloud_dot_validation__pb2.DESCRIPTOR,])
 
 
 
 
 _GETFUNCTIONREQUEST = _descriptor.Descriptor(
@@ -1440,22 +1440,29 @@
       name='tag', full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest.tag', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=b'\350\3071\001\362\3071\032[a-z][-_0-9a-z]*|[$]latest', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='zone_instances_limit', full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest.zone_instances_limit', index=2,
+      name='zone_provisioned_instances_count', full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest.zone_provisioned_instances_count', index=2,
+      number=4, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\372\3071\0060-1000', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='zone_instances_limit', full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest.zone_instances_limit', index=3,
       number=5, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=b'\372\3071\0060-1000', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='zone_requests_limit', full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest.zone_requests_limit', index=3,
+      name='zone_requests_limit', full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyRequest.zone_requests_limit', index=4,
       number=6, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=b'\372\3071\0060-1000', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1466,15 +1473,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=4557,
-  serialized_end=4741,
+  serialized_end=4795,
 )
 
 
 _SETSCALINGPOLICYMETADATA = _descriptor.Descriptor(
   name='SetScalingPolicyMetadata',
   full_name='yandex.cloud.serverless.functions.v1.SetScalingPolicyMetadata',
   filename=None,
@@ -1497,16 +1504,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4743,
-  serialized_end=4790,
+  serialized_start=4797,
+  serialized_end=4844,
 )
 
 
 _REMOVESCALINGPOLICYREQUEST = _descriptor.Descriptor(
   name='RemoveScalingPolicyRequest',
   full_name='yandex.cloud.serverless.functions.v1.RemoveScalingPolicyRequest',
   filename=None,
@@ -1536,16 +1543,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4792,
-  serialized_end=4896,
+  serialized_start=4846,
+  serialized_end=4950,
 )
 
 
 _REMOVESCALINGPOLICYMETADATA = _descriptor.Descriptor(
   name='RemoveScalingPolicyMetadata',
   full_name='yandex.cloud.serverless.functions.v1.RemoveScalingPolicyMetadata',
   filename=None,
@@ -1568,16 +1575,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4898,
-  serialized_end=4948,
+  serialized_start=4952,
+  serialized_end=5002,
 )
 
 _LISTFUNCTIONSRESPONSE.fields_by_name['functions'].message_type = yandex_dot_cloud_dot_serverless_dot_functions_dot_v1_dot_function__pb2._FUNCTION
 _CREATEFUNCTIONREQUEST_LABELSENTRY.containing_type = _CREATEFUNCTIONREQUEST
 _CREATEFUNCTIONREQUEST.fields_by_name['labels'].message_type = _CREATEFUNCTIONREQUEST_LABELSENTRY
 _UPDATEFUNCTIONREQUEST_LABELSENTRY.containing_type = _UPDATEFUNCTIONREQUEST
 _UPDATEFUNCTIONREQUEST.fields_by_name['update_mask'].message_type = google_dot_protobuf_dot_field__mask__pb2._FIELDMASK
@@ -1950,28 +1957,29 @@
 _LISTFUNCTIONTAGHISTORYREQUEST.fields_by_name['page_token']._options = None
 _LISTFUNCTIONTAGHISTORYREQUEST.fields_by_name['filter']._options = None
 _LISTSCALINGPOLICIESREQUEST.fields_by_name['function_id']._options = None
 _LISTSCALINGPOLICIESREQUEST.fields_by_name['page_size']._options = None
 _LISTSCALINGPOLICIESREQUEST.fields_by_name['page_token']._options = None
 _SETSCALINGPOLICYREQUEST.fields_by_name['function_id']._options = None
 _SETSCALINGPOLICYREQUEST.fields_by_name['tag']._options = None
+_SETSCALINGPOLICYREQUEST.fields_by_name['zone_provisioned_instances_count']._options = None
 _SETSCALINGPOLICYREQUEST.fields_by_name['zone_instances_limit']._options = None
 _SETSCALINGPOLICYREQUEST.fields_by_name['zone_requests_limit']._options = None
 _REMOVESCALINGPOLICYREQUEST.fields_by_name['function_id']._options = None
 _REMOVESCALINGPOLICYREQUEST.fields_by_name['tag']._options = None
 
 _FUNCTIONSERVICE = _descriptor.ServiceDescriptor(
   name='FunctionService',
   full_name='yandex.cloud.serverless.functions.v1.FunctionService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=4951,
-  serialized_end=9010,
+  serialized_start=5005,
+  serialized_end=9064,
   methods=[
   _descriptor.MethodDescriptor(
     name='Get',
     full_name='yandex.cloud.serverless.functions.v1.FunctionService.Get',
     index=0,
     containing_service=None,
     input_type=_GETFUNCTIONREQUEST,
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/functions/v1/function_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/functions/v1/function_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/mdbproxy/v1/proxy_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/predicate_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/serverless/triggers/v1/trigger_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/validation_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/address_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/address_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/network_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/network_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/route_table_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/route_table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/security_group_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/security_group_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/datasphere/v1/project_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,291 +1,262 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: yandex/cloud/vpc/v1/subnet.proto
+# source: yandex/cloud/datasphere/v1/project.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='yandex/cloud/vpc/v1/subnet.proto',
-  package='yandex.cloud.vpc.v1',
+  name='yandex/cloud/datasphere/v1/project.proto',
+  package='yandex.cloud.datasphere.v1',
   syntax='proto3',
-  serialized_options=b'\n\027yandex.cloud.api.vpc.v1Z;github.com/yandex-cloud/go-genproto/yandex/cloud/vpc/v1;vpc',
+  serialized_options=b'\n\036yandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphere',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n yandex/cloud/vpc/v1/subnet.proto\x12\x13yandex.cloud.vpc.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\x87\x03\n\x06Subnet\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x37\n\x06labels\x18\x06 \x03(\x0b\x32\'.yandex.cloud.vpc.v1.Subnet.LabelsEntry\x12\x12\n\nnetwork_id\x18\x07 \x01(\t\x12\x0f\n\x07zone_id\x18\x08 \x01(\t\x12\x16\n\x0ev4_cidr_blocks\x18\n \x03(\t\x12\x16\n\x0ev6_cidr_blocks\x18\x0b \x03(\t\x12\x16\n\x0eroute_table_id\x18\x0c \x01(\t\x12\x36\n\x0c\x64hcp_options\x18\r \x01(\x0b\x32 .yandex.cloud.vpc.v1.DhcpOptions\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"T\n\x0b\x44hcpOptions\x12\x1b\n\x13\x64omain_name_servers\x18\x01 \x03(\t\x12\x13\n\x0b\x64omain_name\x18\x02 \x01(\t\x12\x13\n\x0bntp_servers\x18\x03 \x03(\t*;\n\tIpVersion\x12\x1a\n\x16IP_VERSION_UNSPECIFIED\x10\x00\x12\x08\n\x04IPV4\x10\x01\x12\x08\n\x04IPV6\x10\x02\x42V\n\x17yandex.cloud.api.vpc.v1Z;github.com/yandex-cloud/go-genproto/yandex/cloud/vpc/v1;vpcb\x06proto3'
+  serialized_pb=b'\n(yandex/cloud/datasphere/v1/project.proto\x12\x1ayandex.cloud.datasphere.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xe3\x04\n\x07Project\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tfolder_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12>\n\x08settings\x18\x06 \x01(\x0b\x32,.yandex.cloud.datasphere.v1.Project.Settings\x12:\n\x06limits\x18\x07 \x01(\x0b\x32*.yandex.cloud.datasphere.v1.Project.Limits\x1a\xe8\x01\n\x08Settings\x12\x1a\n\x12service_account_id\x18\x01 \x01(\t\x12\x11\n\tsubnet_id\x18\x02 \x01(\t\x12\x1c\n\x14\x64\x61ta_proc_cluster_id\x18\x03 \x01(\t\x12L\n\x0b\x63ommit_mode\x18\x04 \x01(\x0e\x32\x37.yandex.cloud.datasphere.v1.Project.Settings.CommitMode\"A\n\nCommitMode\x12\x1b\n\x17\x43OMMIT_MODE_UNSPECIFIED\x10\x00\x12\x0c\n\x08STANDARD\x10\x01\x12\x08\n\x04\x41UTO\x10\x02\x1a\x7f\n\x06Limits\x12\x37\n\x12max_units_per_hour\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12<\n\x17max_units_per_execution\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueBk\n\x1eyandex.cloud.api.datasphere.v1ZIgithub.com/yandex-cloud/go-genproto/yandex/cloud/datasphere/v1;datasphereb\x06proto3'
   ,
-  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,])
 
-_IPVERSION = _descriptor.EnumDescriptor(
-  name='IpVersion',
-  full_name='yandex.cloud.vpc.v1.IpVersion',
+
+
+_PROJECT_SETTINGS_COMMITMODE = _descriptor.EnumDescriptor(
+  name='CommitMode',
+  full_name='yandex.cloud.datasphere.v1.Project.Settings.CommitMode',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='IP_VERSION_UNSPECIFIED', index=0, number=0,
+      name='COMMIT_MODE_UNSPECIFIED', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='IPV4', index=1, number=1,
+      name='STANDARD', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='IPV6', index=2, number=2,
+      name='AUTO', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=570,
-  serialized_end=629,
+  serialized_start=555,
+  serialized_end=620,
 )
-_sym_db.RegisterEnumDescriptor(_IPVERSION)
-
-IpVersion = enum_type_wrapper.EnumTypeWrapper(_IPVERSION)
-IP_VERSION_UNSPECIFIED = 0
-IPV4 = 1
-IPV6 = 2
-
+_sym_db.RegisterEnumDescriptor(_PROJECT_SETTINGS_COMMITMODE)
 
 
-_SUBNET_LABELSENTRY = _descriptor.Descriptor(
-  name='LabelsEntry',
-  full_name='yandex.cloud.vpc.v1.Subnet.LabelsEntry',
+_PROJECT_SETTINGS = _descriptor.Descriptor(
+  name='Settings',
+  full_name='yandex.cloud.datasphere.v1.Project.Settings',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='yandex.cloud.vpc.v1.Subnet.LabelsEntry.key', index=0,
+      name='service_account_id', full_name='yandex.cloud.datasphere.v1.Project.Settings.service_account_id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='yandex.cloud.vpc.v1.Subnet.LabelsEntry.value', index=1,
+      name='subnet_id', full_name='yandex.cloud.datasphere.v1.Project.Settings.subnet_id', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='data_proc_cluster_id', full_name='yandex.cloud.datasphere.v1.Project.Settings.data_proc_cluster_id', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='commit_mode', full_name='yandex.cloud.datasphere.v1.Project.Settings.commit_mode', index=3,
+      number=4, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
+    _PROJECT_SETTINGS_COMMITMODE,
   ],
-  serialized_options=b'8\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=437,
-  serialized_end=482,
+  serialized_start=388,
+  serialized_end=620,
 )
 
-_SUBNET = _descriptor.Descriptor(
-  name='Subnet',
-  full_name='yandex.cloud.vpc.v1.Subnet',
+_PROJECT_LIMITS = _descriptor.Descriptor(
+  name='Limits',
+  full_name='yandex.cloud.datasphere.v1.Project.Limits',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='yandex.cloud.vpc.v1.Subnet.id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='folder_id', full_name='yandex.cloud.vpc.v1.Subnet.folder_id', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='max_units_per_hour', full_name='yandex.cloud.datasphere.v1.Project.Limits.max_units_per_hour', index=0,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='created_at', full_name='yandex.cloud.vpc.v1.Subnet.created_at', index=2,
+      name='max_units_per_execution', full_name='yandex.cloud.datasphere.v1.Project.Limits.max_units_per_execution', index=1,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=622,
+  serialized_end=749,
+)
+
+_PROJECT = _descriptor.Descriptor(
+  name='Project',
+  full_name='yandex.cloud.datasphere.v1.Project',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='yandex.cloud.vpc.v1.Subnet.name', index=3,
-      number=4, type=9, cpp_type=9, label=1,
+      name='id', full_name='yandex.cloud.datasphere.v1.Project.id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='description', full_name='yandex.cloud.vpc.v1.Subnet.description', index=4,
-      number=5, type=9, cpp_type=9, label=1,
+      name='folder_id', full_name='yandex.cloud.datasphere.v1.Project.folder_id', index=1,
+      number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='labels', full_name='yandex.cloud.vpc.v1.Subnet.labels', index=5,
-      number=6, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='network_id', full_name='yandex.cloud.vpc.v1.Subnet.network_id', index=6,
-      number=7, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='created_at', full_name='yandex.cloud.datasphere.v1.Project.created_at', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='zone_id', full_name='yandex.cloud.vpc.v1.Subnet.zone_id', index=7,
-      number=8, type=9, cpp_type=9, label=1,
+      name='name', full_name='yandex.cloud.datasphere.v1.Project.name', index=3,
+      number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='v4_cidr_blocks', full_name='yandex.cloud.vpc.v1.Subnet.v4_cidr_blocks', index=8,
-      number=10, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='v6_cidr_blocks', full_name='yandex.cloud.vpc.v1.Subnet.v6_cidr_blocks', index=9,
-      number=11, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='route_table_id', full_name='yandex.cloud.vpc.v1.Subnet.route_table_id', index=10,
-      number=12, type=9, cpp_type=9, label=1,
+      name='description', full_name='yandex.cloud.datasphere.v1.Project.description', index=4,
+      number=5, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='dhcp_options', full_name='yandex.cloud.vpc.v1.Subnet.dhcp_options', index=11,
-      number=13, type=11, cpp_type=10, label=1,
+      name='settings', full_name='yandex.cloud.datasphere.v1.Project.settings', index=5,
+      number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_SUBNET_LABELSENTRY, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=91,
-  serialized_end=482,
-)
-
-
-_DHCPOPTIONS = _descriptor.Descriptor(
-  name='DhcpOptions',
-  full_name='yandex.cloud.vpc.v1.DhcpOptions',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='domain_name_servers', full_name='yandex.cloud.vpc.v1.DhcpOptions.domain_name_servers', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='domain_name', full_name='yandex.cloud.vpc.v1.DhcpOptions.domain_name', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='ntp_servers', full_name='yandex.cloud.vpc.v1.DhcpOptions.ntp_servers', index=2,
-      number=3, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='limits', full_name='yandex.cloud.datasphere.v1.Project.limits', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_PROJECT_SETTINGS, _PROJECT_LIMITS, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=484,
-  serialized_end=568,
+  serialized_start=138,
+  serialized_end=749,
 )
 
-_SUBNET_LABELSENTRY.containing_type = _SUBNET
-_SUBNET.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
-_SUBNET.fields_by_name['labels'].message_type = _SUBNET_LABELSENTRY
-_SUBNET.fields_by_name['dhcp_options'].message_type = _DHCPOPTIONS
-DESCRIPTOR.message_types_by_name['Subnet'] = _SUBNET
-DESCRIPTOR.message_types_by_name['DhcpOptions'] = _DHCPOPTIONS
-DESCRIPTOR.enum_types_by_name['IpVersion'] = _IPVERSION
+_PROJECT_SETTINGS.fields_by_name['commit_mode'].enum_type = _PROJECT_SETTINGS_COMMITMODE
+_PROJECT_SETTINGS.containing_type = _PROJECT
+_PROJECT_SETTINGS_COMMITMODE.containing_type = _PROJECT_SETTINGS
+_PROJECT_LIMITS.fields_by_name['max_units_per_hour'].message_type = google_dot_protobuf_dot_wrappers__pb2._INT64VALUE
+_PROJECT_LIMITS.fields_by_name['max_units_per_execution'].message_type = google_dot_protobuf_dot_wrappers__pb2._INT64VALUE
+_PROJECT_LIMITS.containing_type = _PROJECT
+_PROJECT.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_PROJECT.fields_by_name['settings'].message_type = _PROJECT_SETTINGS
+_PROJECT.fields_by_name['limits'].message_type = _PROJECT_LIMITS
+DESCRIPTOR.message_types_by_name['Project'] = _PROJECT
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-Subnet = _reflection.GeneratedProtocolMessageType('Subnet', (_message.Message,), {
+Project = _reflection.GeneratedProtocolMessageType('Project', (_message.Message,), {
 
-  'LabelsEntry' : _reflection.GeneratedProtocolMessageType('LabelsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _SUBNET_LABELSENTRY,
-    '__module__' : 'yandex.cloud.vpc.v1.subnet_pb2'
-    # @@protoc_insertion_point(class_scope:yandex.cloud.vpc.v1.Subnet.LabelsEntry)
+  'Settings' : _reflection.GeneratedProtocolMessageType('Settings', (_message.Message,), {
+    'DESCRIPTOR' : _PROJECT_SETTINGS,
+    '__module__' : 'yandex.cloud.datasphere.v1.project_pb2'
+    # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.Project.Settings)
     })
   ,
-  'DESCRIPTOR' : _SUBNET,
-  '__module__' : 'yandex.cloud.vpc.v1.subnet_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.vpc.v1.Subnet)
-  })
-_sym_db.RegisterMessage(Subnet)
-_sym_db.RegisterMessage(Subnet.LabelsEntry)
 
-DhcpOptions = _reflection.GeneratedProtocolMessageType('DhcpOptions', (_message.Message,), {
-  'DESCRIPTOR' : _DHCPOPTIONS,
-  '__module__' : 'yandex.cloud.vpc.v1.subnet_pb2'
-  # @@protoc_insertion_point(class_scope:yandex.cloud.vpc.v1.DhcpOptions)
+  'Limits' : _reflection.GeneratedProtocolMessageType('Limits', (_message.Message,), {
+    'DESCRIPTOR' : _PROJECT_LIMITS,
+    '__module__' : 'yandex.cloud.datasphere.v1.project_pb2'
+    # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.Project.Limits)
+    })
+  ,
+  'DESCRIPTOR' : _PROJECT,
+  '__module__' : 'yandex.cloud.datasphere.v1.project_pb2'
+  # @@protoc_insertion_point(class_scope:yandex.cloud.datasphere.v1.Project)
   })
-_sym_db.RegisterMessage(DhcpOptions)
+_sym_db.RegisterMessage(Project)
+_sym_db.RegisterMessage(Project.Settings)
+_sym_db.RegisterMessage(Project.Limits)
 
 
 DESCRIPTOR._options = None
-_SUBNET_LABELSENTRY._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/vpc/v1/subnet_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/vpc/v1/subnet_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/backup_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/database_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/database_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/location_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/location_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/resource_preset_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_service_pb2.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandex/cloud/ydb/v1/storage_type_service_pb2_grpc.py` & `yandexcloud-0.99.0/yandex/cloud/ydb/v1/storage_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_auth_fabric.py` & `yandexcloud-0.99.0/yandexcloud/_auth_fabric.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_auth_plugin.py` & `yandexcloud-0.99.0/yandexcloud/_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_backoff.py` & `yandexcloud-0.99.0/yandexcloud/_backoff.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_channels.py` & `yandexcloud-0.99.0/yandexcloud/_channels.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_helpers.py` & `yandexcloud-0.99.0/yandexcloud/_helpers.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_operation_waiter.py` & `yandexcloud-0.99.0/yandexcloud/_operation_waiter.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_retry_interceptor.py` & `yandexcloud-0.99.0/yandexcloud/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_sdk.py` & `yandexcloud-0.99.0/yandexcloud/_sdk.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud/_wrappers/dataproc/__init__.py` & `yandexcloud-0.99.0/yandexcloud/_wrappers/dataproc/__init__.py`

 * *Files identical despite different names*

### Comparing `yandexcloud-0.98.0/yandexcloud.egg-info/PKG-INFO` & `yandexcloud-0.99.0/yandexcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandexcloud
-Version: 0.98.0
+Version: 0.99.0
 Summary: The Yandex.Cloud official SDK
 Home-page: https://github.com/yandex-cloud/python-sdk
 Author: Yandex LLC
 Author-email: cloud@support.yandex.ru
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `yandexcloud-0.98.0/yandexcloud.egg-info/SOURCES.txt` & `yandexcloud-0.99.0/yandexcloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,16 @@
 yandex/cloud/dataproc/v1/resource_preset_service_pb2_grpc.py
 yandex/cloud/dataproc/v1/subcluster_pb2.py
 yandex/cloud/dataproc/v1/subcluster_pb2_grpc.py
 yandex/cloud/dataproc/v1/subcluster_service_pb2.py
 yandex/cloud/dataproc/v1/subcluster_service_pb2_grpc.py
 yandex/cloud/datasphere/__init__.py
 yandex/cloud/datasphere/v1/__init__.py
+yandex/cloud/datasphere/v1/app_token_service_pb2.py
+yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py
 yandex/cloud/datasphere/v1/node_service_pb2.py
 yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
 yandex/cloud/datasphere/v1/project_pb2.py
 yandex/cloud/datasphere/v1/project_pb2_grpc.py
 yandex/cloud/datasphere/v1/project_service_pb2.py
 yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
 yandex/cloud/dns/__init__.py
```

