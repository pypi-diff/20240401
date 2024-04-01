# Comparing `tmp/seven_cloudapp_frame-1.1.8.tar.gz` & `tmp/seven_cloudapp_frame-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\Project\Gao7Git\seven_cloudapp_frame\dist\.tmp-sbcxz_b0\seven_cloudapp_frame-1.1.8.tar", last modified: Fri Mar 15 09:55:24 2024, max compression
+gzip compressed data, was "E:\Project\Gao7Git\seven_cloudapp_frame\dist\.tmp-5gx6wskp\seven_cloudapp_frame-1.1.9.tar", last modified: Tue Mar 19 03:16:01 2024, max compression
```

## Comparing `seven_cloudapp_frame-1.1.8.tar` & `seven_cloudapp_frame-1.1.9.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.834888 seven_cloudapp_frame-1.1.8/
--rw-rw-rw-   0        0        0     1081 2021-04-09 01:22:35.000000 seven_cloudapp_frame-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     8848 2024-03-15 09:55:24.828891 seven_cloudapp_frame-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7779 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-15 09:55:24.834888 seven_cloudapp_frame-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1514 2024-03-15 09:53:27.000000 seven_cloudapp_frame-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.232802 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/
--rw-rw-rw-   0        0        0      164 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.289770 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/
--rw-rw-rw-   0        0        0      182 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.410701 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/
--rw-rw-rw-   0        0        0      263 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/__init__.py
--rw-rw-rw-   0        0        0    14310 2024-03-08 06:09:58.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/act.py
--rw-rw-rw-   0        0        0   411248 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/address.py
--rw-rw-rw-   0        0        0     7958 2024-03-05 04:00:38.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/app.py
--rw-rw-rw-   0        0        0     3849 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/goods.py
--rw-rw-rw-   0        0        0     1825 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/ip_c.py
--rw-rw-rw-   0        0        0    17250 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/order.py
--rw-rw-rw-   0        0        0    35041 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/pay.py
--rw-rw-rw-   0        0        0     5038 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/stat.py
--rw-rw-rw-   0        0        0    64645 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/task.py
--rw-rw-rw-   0        0        0     5070 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/theme.py
--rw-rw-rw-   0        0        0    23456 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/user.py
--rw-rw-rw-   0        0        0     1243 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/core.py
--rw-rw-rw-   0        0        0     3428 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/filter_base.py
--rw-rw-rw-   0        0        0    42301 2024-03-06 10:11:10.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/frame_base.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.544626 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/
--rw-rw-rw-   0        0        0      331 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/__init__.py
--rw-rw-rw-   0        0        0    22907 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/act_s.py
--rw-rw-rw-   0        0        0    25924 2024-03-15 09:53:13.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/app_s.py
--rw-rw-rw-   0        0        0     5115 2024-03-15 06:41:29.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/base_s.py
--rw-rw-rw-   0        0        0    11160 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/cms_s.py
--rw-rw-rw-   0        0        0     9789 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/goods_s.py
--rw-rw-rw-   0        0        0    14810 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/ip_s.py
--rw-rw-rw-   0        0        0    14383 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/launch_s.py
--rw-rw-rw-   0        0        0    16221 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/module_s.py
--rw-rw-rw-   0        0        0    35999 2023-08-15 02:54:26.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/order_s.py
--rw-rw-rw-   0        0        0     8771 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/price_s.py
--rw-rw-rw-   0        0        0    19798 2023-09-12 08:53:49.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/prize_s.py
--rw-rw-rw-   0        0        0     5568 2023-12-25 08:01:51.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/report_s.py
--rw-rw-rw-   0        0        0     7616 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/task_s.py
--rw-rw-rw-   0        0        0     2746 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/theme_s.py
--rw-rw-rw-   0        0        0    23860 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/user_s.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.553619 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/
--rw-rw-rw-   0        0        0      139 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.586601 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/
--rw-rw-rw-   0        0        0      190 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/__init__.py
--rw-rw-rw-   0        0        0     4222 2023-12-04 03:08:22.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/frame_console.py
--rw-rw-rw-   0        0        0     5441 2024-03-08 11:10:07.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/frame_db.py
--rw-rw-rw-   0        0        0      443 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/frame_tornado.py
--rw-rw-rw-   0        0        0     1864 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/share_config.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:23.855447 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/
--rw-rw-rw-   0        0        0      162 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/__init__.py
--rw-rw-rw-   0        0        0     5792 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/action_helper.py
--rw-rw-rw-   0        0        0    10880 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/alipay_helper.py
--rw-rw-rw-   0        0        0     3195 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py
--rw-rw-rw-   0        0        0     9671 2023-12-13 02:15:22.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/content_censor_helper.py
--rw-rw-rw-   0        0        0     7562 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/counter_helper.py
--rw-rw-rw-   0        0        0     6437 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/cryptography_helper.py
--rw-rw-rw-   0        0        0     2430 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/email_helper.py
--rw-rw-rw-   0        0        0    12704 2023-11-20 09:47:19.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/file_helper.py
--rw-rw-rw-   0        0        0     8991 2023-08-30 05:52:34.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/logistics_helper.py
--rw-rw-rw-   0        0        0     1397 2023-08-15 02:54:26.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/oss2_helper.py
--rw-rw-rw-   0        0        0    36622 2023-12-07 05:48:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/queue_up_helper.py
--rw-rw-rw-   0        0        0     4954 2023-11-23 06:40:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/redis_helper.py
--rw-rw-rw-   0        0        0    12084 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/safe_helper.py
--rw-rw-rw-   0        0        0    24985 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/seven_helper.py
--rw-rw-rw-   0        0        0    14907 2023-10-24 06:42:56.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/sms_helper.py
--rw-rw-rw-   0        0        0    36659 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/tiktok_helper.py
--rw-rw-rw-   0        0        0     6301 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/time_helper.py
--rw-rw-rw-   0        0        0    97363 2023-12-19 09:52:20.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/wechat_helper.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.046338 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/
--rw-rw-rw-   0        0        0      139 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/__init__.py
--rw-rw-rw-   0        0        0    23079 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/act_base_model.py
--rw-rw-rw-   0        0        0    21921 2024-03-15 07:59:39.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/app_base_model.py
--rw-rw-rw-   0        0        0    49508 2024-03-08 02:12:21.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/asset_base_model.py
--rw-rw-rw-   0        0        0    34046 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/cache_model.py
--rw-rw-rw-   0        0        0    13052 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/cms_base_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.100307 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/__init__.py
--rw-rw-rw-   0        0        0    16563 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/asset_console_model.py
--rw-rw-rw-   0        0        0    20564 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/erp_console_model.py
--rw-rw-rw-   0        0        0    10876 2023-11-27 03:54:27.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/launch_console_model.py
--rw-rw-rw-   0        0        0    24895 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/stat_console_model.py
--rw-rw-rw-   0        0        0     2922 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/task_console_model.py
--rw-rw-rw-   0        0        0     5432 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/timing_work_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.106305 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.138285 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/
--rw-rw-rw-   0        0        0       81 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/__init__.py
--rw-rw-rw-   0        0        0     3833 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_info_model.py
--rw-rw-rw-   0        0        0     3050 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_module_model.py
--rw-rw-rw-   0        0        0     3834 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_prize_model.py
--rw-rw-rw-   0        0        0     2611 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_type_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.161273 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/
--rw-rw-rw-   0        0        0       70 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/__init__.py
--rw-rw-rw-   0        0        0     3271 2024-03-15 05:52:45.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/app_info_model.py
--rw-rw-rw-   0        0        0     1317 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/app_relation_model.py
--rw-rw-rw-   0        0        0     1670 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/app_template_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.195253 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/
--rw-rw-rw-   0        0        0       97 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/__init__.py
--rw-rw-rw-   0        0        0     2331 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py
--rw-rw-rw-   0        0        0     3211 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py
--rw-rw-rw-   0        0        0     1691 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py
--rw-rw-rw-   0        0        0     2176 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.207246 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/base/
--rw-rw-rw-   0        0        0       28 2023-12-25 09:05:34.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/base/__init__.py
--rw-rw-rw-   0        0        0     3180 2024-03-15 05:51:14.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/base/base_info_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.218240 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/browse/
--rw-rw-rw-   0        0        0       29 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/browse/__init__.py
--rw-rw-rw-   0        0        0     1709 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.242226 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/cms/
--rw-rw-rw-   0        0        0       45 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/cms/__init__.py
--rw-rw-rw-   0        0        0     2862 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py
--rw-rw-rw-   0        0        0     1871 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.252220 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/collect/
--rw-rw-rw-   0        0        0       30 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/collect/__init__.py
--rw-rw-rw-   0        0        0     1702 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.262215 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/counter/
--rw-rw-rw-   0        0        0       32 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/counter/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.273209 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/dict/
--rw-rw-rw-   0        0        0      191 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/dict/__init__.py
--rw-rw-rw-   0        0        0     1811 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.286201 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/erp/
--rw-rw-rw-   0        0        0       31 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/erp/__init__.py
--rw-rw-rw-   0        0        0     1736 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.303191 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/friend/
--rw-rw-rw-   0        0        0       30 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/friend/__init__.py
--rw-rw-rw-   0        0        0     1855 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.343169 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/
--rw-rw-rw-   0        0        0      132 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_info_model.py
--rw-rw-rw-   0        0        0     1980 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_module_model.py
--rw-rw-rw-   0        0        0     1584 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_product_model.py
--rw-rw-rw-   0        0        0     2752 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_shop_model.py
--rw-rw-rw-   0        0        0     1716 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_skin_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.362158 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/invite/
--rw-rw-rw-   0        0        0       48 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/invite/__init__.py
--rw-rw-rw-   0        0        0     2480 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py
--rw-rw-rw-   0        0        0     2059 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.383146 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/ip/
--rw-rw-rw-   0        0        0       42 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/ip/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py
--rw-rw-rw-   0        0        0     1602 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.403134 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/launch/
--rw-rw-rw-   0        0        0       51 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/launch/__init__.py
--rw-rw-rw-   0        0        0     1755 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py
--rw-rw-rw-   0        0        0     1734 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.418126 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/marketing/
--rw-rw-rw-   0        0        0       36 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/marketing/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.430120 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/middler/
--rw-rw-rw-   0        0        0       34 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/middler/__init__.py
--rw-rw-rw-   0        0        0     1847 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.451107 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/operation/
--rw-rw-rw-   0        0        0       61 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/operation/__init__.py
--rw-rw-rw-   0        0        0     1476 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py
--rw-rw-rw-   0        0        0     2707 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.461103 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/pay/
--rw-rw-rw-   0        0        0       28 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/pay/__init__.py
--rw-rw-rw-   0        0        0     3251 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.472096 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/price/
--rw-rw-rw-   0        0        0       29 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/price/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/price/price_gear_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.491085 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/prize/
--rw-rw-rw-   0        0        0       51 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/prize/__init__.py
--rw-rw-rw-   0        0        0     4168 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py
--rw-rw-rw-   0        0        0     4181 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.501079 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/product/
--rw-rw-rw-   0        0        0       32 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/product/__init__.py
--rw-rw-rw-   0        0        0     2012 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/product/product_price_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.512072 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/refund/
--rw-rw-rw-   0        0        0       31 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/refund/__init__.py
--rw-rw-rw-   0        0        0     2314 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.530063 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/saas/
--rw-rw-rw-   0        0        0       30 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/saas/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.543055 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/skin/
--rw-rw-rw-   0        0        0       28 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/skin/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.555049 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/special/
--rw-rw-rw-   0        0        0       32 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/special/__init__.py
--rw-rw-rw-   0        0        0     1458 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/special/special_goods_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.601021 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/
--rw-rw-rw-   0        0        0      130 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/__init__.py
--rw-rw-rw-   0        0        0     1838 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py
--rw-rw-rw-   0        0        0     2240 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py
--rw-rw-rw-   0        0        0     1851 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py
--rw-rw-rw-   0        0        0     1814 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py
--rw-rw-rw-   0        0        0     1871 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py
--rw-rw-rw-   0        0        0     2803 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.623009 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/store/
--rw-rw-rw-   0        0        0       54 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/store/__init__.py
--rw-rw-rw-   0        0        0     3010 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py
--rw-rw-rw-   0        0        0     2046 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/store/store_asset_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.649994 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/
--rw-rw-rw-   0        0        0       73 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/__init__.py
--rw-rw-rw-   0        0        0     2152 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py
--rw-rw-rw-   0        0        0     1610 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py
--rw-rw-rw-   0        0        0     3205 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.679977 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/
--rw-rw-rw-   0        0        0       94 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/__init__.py
--rw-rw-rw-   0        0        0     2292 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_count_model.py
--rw-rw-rw-   0        0        0     2154 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py
--rw-rw-rw-   0        0        0     2428 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_info_model.py
--rw-rw-rw-   0        0        0     2420 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_log_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.697966 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/theme/
--rw-rw-rw-   0        0        0       47 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/theme/__init__.py
--rw-rw-rw-   0        0        0     1775 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py
--rw-rw-rw-   0        0        0     1490 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.708960 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/third/
--rw-rw-rw-   0        0        0       34 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/third/__init__.py
--rw-rw-rw-   0        0        0     2944 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.744940 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/
--rw-rw-rw-   0        0        0      108 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/__init__.py
--rw-rw-rw-   0        0        0     2477 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_account_model.py
--rw-rw-rw-   0        0        0     1999 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_address_model.py
--rw-rw-rw-   0        0        0     2158 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_asset_model.py
--rw-rw-rw-   0        0        0     2103 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_black_model.py
--rw-rw-rw-   0        0        0     3392 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_info_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.755934 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/version/
--rw-rw-rw-   0        0        0       31 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/version/__init__.py
--rw-rw-rw-   0        0        0     1849 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/version/version_info_model.py
--rw-rw-rw-   0        0        0    10176 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/enum.py
--rw-rw-rw-   0        0        0    30058 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/frame_base_model.py
--rw-rw-rw-   0        0        0    11894 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/goods_base_model.py
--rw-rw-rw-   0        0        0    14908 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/ip_base_model.py
--rw-rw-rw-   0        0        0    28969 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/launch_base_model.py
--rw-rw-rw-   0        0        0    12767 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/module_base_model.py
--rw-rw-rw-   0        0        0    21120 2023-07-30 08:03:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/mp_base_model.py
--rw-rw-rw-   0        0        0    14717 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/operate_base_model.py
--rw-rw-rw-   0        0        0    65922 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/order_base_model.py
--rw-rw-rw-   0        0        0    11494 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/price_base_model.py
--rw-rw-rw-   0        0        0    16061 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/prize_base_model.py
--rw-rw-rw-   0        0        0     4592 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/push_base_model.py
--rw-rw-rw-   0        0        0    14750 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/seven_model.py
--rw-rw-rw-   0        0        0    24830 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/stat_base_model.py
--rw-rw-rw-   0        0        0   274501 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/task_base_model.py
--rw-rw-rw-   0        0        0    13626 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/theme_base_model.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.803907 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/third/
--rw-rw-rw-   0        0        0        0 2023-10-24 06:42:56.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/third/__init__.py
--rw-rw-rw-   0        0        0    90805 2023-12-08 09:03:57.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/third/jd_base_model.py
--rw-rw-rw-   0        0        0    22812 2024-03-08 07:17:24.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/third/shakeshop_base_model.py
--rw-rw-rw-   0        0        0    95900 2024-03-14 10:42:46.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/top_base_model.py
--rw-rw-rw-   0        0        0    48576 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/user_base_model.py
--rw-rw-rw-   0        0        0    14840 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/route.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:55:24.821895 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/
--rw-rw-rw-   0        0        0     8848 2024-03-15 09:55:22.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11177 2024-03-15 09:55:23.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 09:55:22.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-03-15 09:55:22.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-03-15 09:55:22.000000 seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.988448 seven_cloudapp_frame-1.1.9/
+-rw-rw-rw-   0        0        0     1081 2021-04-09 01:22:35.000000 seven_cloudapp_frame-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     8848 2024-03-19 03:16:00.983447 seven_cloudapp_frame-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7779 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-19 03:16:00.988448 seven_cloudapp_frame-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1514 2024-03-19 03:15:16.000000 seven_cloudapp_frame-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.204051 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/
+-rw-rw-rw-   0        0        0      164 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.268163 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/
+-rw-rw-rw-   0        0        0      182 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.348199 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/
+-rw-rw-rw-   0        0        0      263 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/__init__.py
+-rw-rw-rw-   0        0        0    14310 2024-03-08 06:09:58.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/act.py
+-rw-rw-rw-   0        0        0   411248 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/address.py
+-rw-rw-rw-   0        0        0     7958 2024-03-05 04:00:38.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/app.py
+-rw-rw-rw-   0        0        0     3849 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/goods.py
+-rw-rw-rw-   0        0        0     1825 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/ip_c.py
+-rw-rw-rw-   0        0        0    17250 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/order.py
+-rw-rw-rw-   0        0        0    35041 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/pay.py
+-rw-rw-rw-   0        0        0     5038 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/stat.py
+-rw-rw-rw-   0        0        0    64645 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/task.py
+-rw-rw-rw-   0        0        0     5070 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/theme.py
+-rw-rw-rw-   0        0        0    23456 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/user.py
+-rw-rw-rw-   0        0        0     1243 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/core.py
+-rw-rw-rw-   0        0        0     3428 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/filter_base.py
+-rw-rw-rw-   0        0        0    42301 2024-03-06 10:11:10.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/frame_base.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.482948 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/
+-rw-rw-rw-   0        0        0      331 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/__init__.py
+-rw-rw-rw-   0        0        0    22907 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/act_s.py
+-rw-rw-rw-   0        0        0    24244 2024-03-19 02:48:58.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/app_s.py
+-rw-rw-rw-   0        0        0     5115 2024-03-15 06:41:29.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/base_s.py
+-rw-rw-rw-   0        0        0    11160 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/cms_s.py
+-rw-rw-rw-   0        0        0     9789 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/goods_s.py
+-rw-rw-rw-   0        0        0    14810 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/ip_s.py
+-rw-rw-rw-   0        0        0    14383 2023-07-26 11:29:42.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/launch_s.py
+-rw-rw-rw-   0        0        0    16221 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/module_s.py
+-rw-rw-rw-   0        0        0    35999 2023-08-15 02:54:26.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/order_s.py
+-rw-rw-rw-   0        0        0     8771 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/price_s.py
+-rw-rw-rw-   0        0        0    19798 2023-09-12 08:53:49.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/prize_s.py
+-rw-rw-rw-   0        0        0     5568 2023-12-25 08:01:51.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/report_s.py
+-rw-rw-rw-   0        0        0     7616 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/task_s.py
+-rw-rw-rw-   0        0        0     2746 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/theme_s.py
+-rw-rw-rw-   0        0        0    23860 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/user_s.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.489944 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/
+-rw-rw-rw-   0        0        0      139 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.517194 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/
+-rw-rw-rw-   0        0        0      190 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/__init__.py
+-rw-rw-rw-   0        0        0     4222 2023-12-04 03:08:22.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/frame_console.py
+-rw-rw-rw-   0        0        0     5441 2024-03-08 11:10:07.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/frame_db.py
+-rw-rw-rw-   0        0        0      443 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/frame_tornado.py
+-rw-rw-rw-   0        0        0     1864 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/share_config.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.647109 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/
+-rw-rw-rw-   0        0        0      162 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/__init__.py
+-rw-rw-rw-   0        0        0     5792 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/action_helper.py
+-rw-rw-rw-   0        0        0    10880 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/alipay_helper.py
+-rw-rw-rw-   0        0        0     3195 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py
+-rw-rw-rw-   0        0        0     9671 2023-12-13 02:15:22.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/content_censor_helper.py
+-rw-rw-rw-   0        0        0     7562 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/counter_helper.py
+-rw-rw-rw-   0        0        0     6437 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/cryptography_helper.py
+-rw-rw-rw-   0        0        0     2430 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/email_helper.py
+-rw-rw-rw-   0        0        0    12704 2023-11-20 09:47:19.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/file_helper.py
+-rw-rw-rw-   0        0        0     8991 2023-08-30 05:52:34.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/logistics_helper.py
+-rw-rw-rw-   0        0        0     1397 2023-08-15 02:54:26.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/oss2_helper.py
+-rw-rw-rw-   0        0        0    36622 2023-12-07 05:48:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/queue_up_helper.py
+-rw-rw-rw-   0        0        0     4954 2023-11-23 06:40:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/redis_helper.py
+-rw-rw-rw-   0        0        0    12084 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/safe_helper.py
+-rw-rw-rw-   0        0        0    25856 2024-03-18 09:51:51.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/seven_helper.py
+-rw-rw-rw-   0        0        0    14907 2023-10-24 06:42:56.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/sms_helper.py
+-rw-rw-rw-   0        0        0    36659 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/tiktok_helper.py
+-rw-rw-rw-   0        0        0     6301 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/time_helper.py
+-rw-rw-rw-   0        0        0    97363 2023-12-19 09:52:20.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/wechat_helper.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.921675 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/
+-rw-rw-rw-   0        0        0      139 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/__init__.py
+-rw-rw-rw-   0        0        0    23079 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/act_base_model.py
+-rw-rw-rw-   0        0        0    21921 2024-03-15 07:59:39.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/app_base_model.py
+-rw-rw-rw-   0        0        0    49508 2024-03-08 02:12:21.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/asset_base_model.py
+-rw-rw-rw-   0        0        0    34046 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/cache_model.py
+-rw-rw-rw-   0        0        0    13052 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/cms_base_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:15:59.968550 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/__init__.py
+-rw-rw-rw-   0        0        0    16563 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/asset_console_model.py
+-rw-rw-rw-   0        0        0    20564 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/erp_console_model.py
+-rw-rw-rw-   0        0        0    10876 2023-11-27 03:54:27.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/launch_console_model.py
+-rw-rw-rw-   0        0        0    24895 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/stat_console_model.py
+-rw-rw-rw-   0        0        0     2922 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/task_console_model.py
+-rw-rw-rw-   0        0        0     5432 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/timing_work_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.022573 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.154664 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/
+-rw-rw-rw-   0        0        0       81 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/__init__.py
+-rw-rw-rw-   0        0        0     3833 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_info_model.py
+-rw-rw-rw-   0        0        0     3050 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_module_model.py
+-rw-rw-rw-   0        0        0     3834 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_prize_model.py
+-rw-rw-rw-   0        0        0     2611 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_type_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.186209 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/
+-rw-rw-rw-   0        0        0       70 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/__init__.py
+-rw-rw-rw-   0        0        0     3271 2024-03-15 05:52:45.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/app_info_model.py
+-rw-rw-rw-   0        0        0     1317 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/app_relation_model.py
+-rw-rw-rw-   0        0        0     1670 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/app_template_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.216881 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/
+-rw-rw-rw-   0        0        0       97 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/__init__.py
+-rw-rw-rw-   0        0        0     2331 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py
+-rw-rw-rw-   0        0        0     3211 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py
+-rw-rw-rw-   0        0        0     1691 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py
+-rw-rw-rw-   0        0        0     2176 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.234373 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/base/
+-rw-rw-rw-   0        0        0       28 2023-12-25 09:05:34.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/base/__init__.py
+-rw-rw-rw-   0        0        0     3180 2024-03-15 05:51:14.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/base/base_info_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.248842 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/browse/
+-rw-rw-rw-   0        0        0       29 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/browse/__init__.py
+-rw-rw-rw-   0        0        0     1709 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.266835 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/cms/
+-rw-rw-rw-   0        0        0       45 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/cms/__init__.py
+-rw-rw-rw-   0        0        0     2862 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py
+-rw-rw-rw-   0        0        0     1871 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.281901 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/collect/
+-rw-rw-rw-   0        0        0       30 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/collect/__init__.py
+-rw-rw-rw-   0        0        0     1702 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.295563 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/counter/
+-rw-rw-rw-   0        0        0       32 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/counter/__init__.py
+-rw-rw-rw-   0        0        0     1679 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.317727 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/dict/
+-rw-rw-rw-   0        0        0      191 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/dict/__init__.py
+-rw-rw-rw-   0        0        0     1811 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.335640 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/erp/
+-rw-rw-rw-   0        0        0       31 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/erp/__init__.py
+-rw-rw-rw-   0        0        0     1736 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.354724 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/friend/
+-rw-rw-rw-   0        0        0       30 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/friend/__init__.py
+-rw-rw-rw-   0        0        0     1855 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.415676 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/
+-rw-rw-rw-   0        0        0      132 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_info_model.py
+-rw-rw-rw-   0        0        0     1980 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_module_model.py
+-rw-rw-rw-   0        0        0     1584 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_product_model.py
+-rw-rw-rw-   0        0        0     2752 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_shop_model.py
+-rw-rw-rw-   0        0        0     1716 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_skin_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.435204 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/invite/
+-rw-rw-rw-   0        0        0       48 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/invite/__init__.py
+-rw-rw-rw-   0        0        0     2480 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py
+-rw-rw-rw-   0        0        0     2059 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.459496 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/ip/
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/ip/__init__.py
+-rw-rw-rw-   0        0        0     2016 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py
+-rw-rw-rw-   0        0        0     1602 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.479635 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/launch/
+-rw-rw-rw-   0        0        0       51 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/launch/__init__.py
+-rw-rw-rw-   0        0        0     1755 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py
+-rw-rw-rw-   0        0        0     1734 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.495628 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/marketing/
+-rw-rw-rw-   0        0        0       36 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/marketing/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.511875 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/middler/
+-rw-rw-rw-   0        0        0       34 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/middler/__init__.py
+-rw-rw-rw-   0        0        0     1847 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.606162 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/operation/
+-rw-rw-rw-   0        0        0       61 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/operation/__init__.py
+-rw-rw-rw-   0        0        0     1476 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py
+-rw-rw-rw-   0        0        0     2707 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.616155 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/pay/
+-rw-rw-rw-   0        0        0       28 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/pay/__init__.py
+-rw-rw-rw-   0        0        0     3251 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.629967 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/price/
+-rw-rw-rw-   0        0        0       29 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/price/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/price/price_gear_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.649745 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/prize/
+-rw-rw-rw-   0        0        0       51 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/prize/__init__.py
+-rw-rw-rw-   0        0        0     4168 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py
+-rw-rw-rw-   0        0        0     4181 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.664739 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/product/
+-rw-rw-rw-   0        0        0       32 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/product/__init__.py
+-rw-rw-rw-   0        0        0     2012 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/product/product_price_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.679834 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/refund/
+-rw-rw-rw-   0        0        0       31 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/refund/__init__.py
+-rw-rw-rw-   0        0        0     2314 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.693901 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/saas/
+-rw-rw-rw-   0        0        0       30 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/saas/__init__.py
+-rw-rw-rw-   0        0        0     1891 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.706657 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/skin/
+-rw-rw-rw-   0        0        0       28 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/skin/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.722631 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/special/
+-rw-rw-rw-   0        0        0       32 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/special/__init__.py
+-rw-rw-rw-   0        0        0     1458 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/special/special_goods_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.778152 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/
+-rw-rw-rw-   0        0        0      130 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/__init__.py
+-rw-rw-rw-   0        0        0     1838 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py
+-rw-rw-rw-   0        0        0     2240 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py
+-rw-rw-rw-   0        0        0     1851 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py
+-rw-rw-rw-   0        0        0     1814 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py
+-rw-rw-rw-   0        0        0     1871 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py
+-rw-rw-rw-   0        0        0     2803 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.797736 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/store/
+-rw-rw-rw-   0        0        0       54 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/store/__init__.py
+-rw-rw-rw-   0        0        0     3010 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py
+-rw-rw-rw-   0        0        0     2046 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/store/store_asset_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.827456 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/
+-rw-rw-rw-   0        0        0       73 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/__init__.py
+-rw-rw-rw-   0        0        0     2152 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py
+-rw-rw-rw-   0        0        0     1610 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py
+-rw-rw-rw-   0        0        0     3205 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.860870 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/
+-rw-rw-rw-   0        0        0       94 2023-07-26 11:29:43.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/__init__.py
+-rw-rw-rw-   0        0        0     2292 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_count_model.py
+-rw-rw-rw-   0        0        0     2154 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py
+-rw-rw-rw-   0        0        0     2428 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_info_model.py
+-rw-rw-rw-   0        0        0     2420 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_log_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.881531 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/theme/
+-rw-rw-rw-   0        0        0       47 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/theme/__init__.py
+-rw-rw-rw-   0        0        0     1775 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py
+-rw-rw-rw-   0        0        0     1490 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.897335 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/third/
+-rw-rw-rw-   0        0        0       34 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/third/__init__.py
+-rw-rw-rw-   0        0        0     2944 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.939517 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/
+-rw-rw-rw-   0        0        0      108 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/__init__.py
+-rw-rw-rw-   0        0        0     2477 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_account_model.py
+-rw-rw-rw-   0        0        0     1999 2024-03-06 10:10:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_address_model.py
+-rw-rw-rw-   0        0        0     2158 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_asset_model.py
+-rw-rw-rw-   0        0        0     2103 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_black_model.py
+-rw-rw-rw-   0        0        0     3392 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_info_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.952844 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/version/
+-rw-rw-rw-   0        0        0       31 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/version/__init__.py
+-rw-rw-rw-   0        0        0     1849 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/version/version_info_model.py
+-rw-rw-rw-   0        0        0    10176 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/enum.py
+-rw-rw-rw-   0        0        0    31722 2024-03-18 01:53:41.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/frame_base_model.py
+-rw-rw-rw-   0        0        0    11894 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/goods_base_model.py
+-rw-rw-rw-   0        0        0    14908 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/ip_base_model.py
+-rw-rw-rw-   0        0        0    28969 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/launch_base_model.py
+-rw-rw-rw-   0        0        0    12767 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/module_base_model.py
+-rw-rw-rw-   0        0        0    21120 2023-07-30 08:03:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/mp_base_model.py
+-rw-rw-rw-   0        0        0    14717 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/operate_base_model.py
+-rw-rw-rw-   0        0        0    65922 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/order_base_model.py
+-rw-rw-rw-   0        0        0    11494 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/price_base_model.py
+-rw-rw-rw-   0        0        0    16061 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/prize_base_model.py
+-rw-rw-rw-   0        0        0     4592 2023-07-26 11:29:44.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/push_base_model.py
+-rw-rw-rw-   0        0        0    14750 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/seven_model.py
+-rw-rw-rw-   0        0        0    24830 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/stat_base_model.py
+-rw-rw-rw-   0        0        0   274501 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/task_base_model.py
+-rw-rw-rw-   0        0        0    13626 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/theme_base_model.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.971463 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/third/
+-rw-rw-rw-   0        0        0        0 2023-10-24 06:42:56.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/third/__init__.py
+-rw-rw-rw-   0        0        0    90805 2023-12-08 09:03:57.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/third/jd_base_model.py
+-rw-rw-rw-   0        0        0    22812 2024-03-08 07:17:24.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/third/shakeshop_base_model.py
+-rw-rw-rw-   0        0        0    95900 2024-03-14 10:42:46.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/top_base_model.py
+-rw-rw-rw-   0        0        0    48576 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/user_base_model.py
+-rw-rw-rw-   0        0        0    14840 2024-03-06 10:10:25.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/route.py
+drwxrwxrwx   0        0        0        0 2024-03-19 03:16:00.979458 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/
+-rw-rw-rw-   0        0        0     8848 2024-03-19 03:15:58.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11177 2024-03-19 03:15:59.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 03:15:58.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2024-03-19 03:15:58.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-03-19 03:15:58.000000 seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/top_level.txt
```

### Comparing `seven_cloudapp_frame-1.1.8/LICENSE` & `seven_cloudapp_frame-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/PKG-INFO` & `seven_cloudapp_frame-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_cloudapp_frame
-Version: 1.1.8
+Version: 1.1.9
 Summary: seven cloudapp frame
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_frame.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
```

### Comparing `seven_cloudapp_frame-1.1.8/README.md` & `seven_cloudapp_frame-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/setup.py` & `seven_cloudapp_frame-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_cloudapp_frame",
-    version="1.1.8",
+    version="1.1.9",
     author="seven",
     author_email="tech@gao7.com",
     description="seven cloudapp frame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_frame.git",
```

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/act.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/act.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/address.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/address.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/app.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/app.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/goods.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/goods.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/ip_c.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/ip_c.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/order.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/order.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/pay.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/pay.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/stat.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/stat.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/task.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/task.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/theme.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/theme.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/client/user.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/client/user.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/core.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/core.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/filter_base.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/filter_base.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/frame_base.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/frame_base.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/act_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/act_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/app_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/app_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-08-03 10:43:58
-@LastEditTime: 2024-03-15 17:52:27
+@LastEditTime: 2024-03-19 10:48:25
 @LastEditors: HuangJianYi
 @Description: 应用模块
 """
 from seven_cloudapp_frame.models.enum import *
 from seven_cloudapp_frame.handlers.frame_base import *
 from seven_cloudapp_frame.models.top_base_model import *
 from seven_cloudapp_frame.models.app_base_model import *
@@ -127,22 +127,20 @@
     """
     :description: 前端版本更新
     """
     def get_async(self):
         """
         :description: 前端版本更新
         :param app_id:应用标识
-        :param is_multiple:是否批量版本更新
         :return: 
         :last_editors: HuangJianYi
         """
         app_id = self.get_app_id()
         access_token = self.get_access_token()
         user_nick = self.get_user_nick()
-        is_multiple = self.get_param_int("is_multiple", 0)
         is_log = int(self.get_param("is_log", 0))
         is_log = True if is_log == 1 else False
 
         base_info = BaseInfoModel(context=self).get_entity()
         client_ver = base_info.client_ver
         store_user_nick = user_nick.split(':')[0]
 
@@ -171,32 +169,15 @@
         top_base_model = TopBaseModel(context=self)
         app_key, app_secret = self.get_app_key_secret()
         if client_ver != app_info.template_ver:
             invoke_result_data = top_base_model.version_upgrade(app_id, client_template_id, client_ver, access_token, app_key, app_secret, app_info, is_log)
             if invoke_result_data.success == False:
                 return self.response_json_error(invoke_result_data.error_code, invoke_result_data.error_message)
             app_info_model.delete_dependency_key(DependencyKey.app_info(app_id))
-        is_update_project_ver = True # 是否更新版本号项目版本号
-        if is_multiple == 1:
-            app_template_model = AppTemplateModel(context=self)
-            app_info_list = app_info_model.get_list(where="store_user_nick=%s", params=store_user_nick)
-            app_info_list = query(app_info_list).where(lambda x: x.app_id != app_id)
-            if len(app_info_list) > 0:
-                app_template_dict_list = app_template_model.get_dict_list()
-                for item in app_info_list:
-                    app_template_dict = query(app_template_dict_list).first_or_default(None, lambda x:x["template_id"] == item.template_id) 
-                    if app_template_dict and app_template_dict['client_ver'] != item.template_ver:
-                        relation_invoke_result_data = top_base_model.version_upgrade(item.app_id, app_template_dict['template_id'], 
-                                                                                     app_template_dict['client_ver'], access_token, app_key, app_secret, item, is_log)
-                        if relation_invoke_result_data.success == False:
-                            is_update_project_ver = False
-                            self.logging_link_error(f"模板ID：{app_template_dict['template_id']}更新失败，原因：{relation_invoke_result_data.error_message}")
-        
-        if base_info and base_info.project_ver and is_update_project_ver == True:
-            app_info_model.update_table("project_ver=%s", "app_id=%s", [base_info.project_ver, app_id])
+
         return self.response_json_success(invoke_result_data.data)
 
 
 class AppInfoHandler(ClientBaseHandler):
     """
     :description: 获取小程序信息
     """
```

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/base_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/base_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/cms_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/cms_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/goods_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/goods_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/ip_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/ip_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/launch_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/launch_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/module_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/module_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/order_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/order_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/price_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/price_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/prize_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/prize_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/report_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/report_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/task_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/task_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/theme_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/theme_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/handlers/server/user_s.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/handlers/server/user_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/frame_console.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/frame_console.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/frame_db.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/frame_db.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/common/share_config.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/common/share_config.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/action_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/action_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/alipay_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/alipay_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/content_censor_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/content_censor_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/counter_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/counter_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/cryptography_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/cryptography_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/email_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/email_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/file_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/file_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/logistics_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/logistics_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/oss2_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/oss2_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/queue_up_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/queue_up_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/redis_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/redis_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/safe_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/safe_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/seven_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/seven_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJianYi
 :Date: 2021-07-15 11:54:54
-@LastEditTime: 2024-01-26 15:12:00
+@LastEditTime: 2024-03-18 14:24:07
 @LastEditors: HuangJianYi
 :description: 常用帮助类
 """
 from seven_framework import *
 from seven_framework.redis import *
 from seven_cloudapp_frame.libs.common import *
 from seven_cloudapp_frame.libs.customize.redis_helper import RedisExHelper
@@ -223,17 +223,17 @@
             return f"{field_name} IN({list_str})"
         else:
             return f"{field_name} NOT IN({list_str})"
         
     @classmethod
     def exclude_field(self, s_model, exclude_field):
         """
-        :description: 排除不需要的字段
+        :description: 排除不需要的字段（查询时使用）
         :param s_model:对象实例
-        :param exclude_field:排除的字段，分隔
+        :param exclude_field:不进行查询的字段，分隔
         :return:字符串
         :last_editors: HuangJianYi
         """
         field = "*"
         try:
             field_list = set(s_model.get_field_list())
             exclude_field_list = set(exclude_field.split(','))
@@ -242,14 +242,15 @@
             pass
         return field
 
     @classmethod
     def get_row_by_dict_list(self, dict_list, field_name, field_type=1):
         """
         :description: 获取字典列表中指定列的集合
+        :param dict_list:字典列表
         :param field_name:字段名
         :param field_type:字段类型（1整形2字符串）
         :return:数组
         :last_editors: HuangJianYi
         """
         if isinstance(dict_list,list) == False:
             return []
@@ -269,14 +270,35 @@
         """
         try:
             data_index = data_list.index(old_item)
             data_list[data_index] = new_item
         except:
             pass
         return data_list
+    
+    @classmethod
+    def remove_dict_field(self, data, remove_field_list=[]):
+        """
+        :description: 移除字典或字典列表中指定字段
+        :param data:字典或字典列表
+        :param remove_field_list:删除字段列表
+        :return:
+        :last_editors: HuangJianYi
+        """
+        if len(remove_field_list) > 0:
+            if isinstance(data, list):
+                for item in data:
+                    for remove_field in remove_field_list:
+                        if remove_field in item:
+                            del item[remove_field]
+            else:
+                for remove_field in remove_field_list:
+                    if remove_field in data.keys():
+                        del data[remove_field]
+        return data
 
     @classmethod
     def is_ip(self, ip_str):
         """
         :description: 判断是否IP地址
         :param ip_str: ip串
         :return:
```

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/sms_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/sms_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/tiktok_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/tiktok_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/time_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/time_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/libs/customize/wechat_helper.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/libs/customize/wechat_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/act_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/act_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/app_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/app_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/asset_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/asset_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/cache_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/cache_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/cms_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/cms_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/asset_console_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/asset_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/erp_console_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/erp_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/launch_console_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/launch_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/stat_console_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/stat_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/task_console_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/task_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/console_models/timing_work_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/console_models/timing_work_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_module_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_module_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_prize_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_prize_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/act/act_type_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/act/act_type_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/app_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/app_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/app_relation_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/app_relation_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/app/app_template_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/app/app_template_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/base/base_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/base/base_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_module_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_module_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_product_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_product_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_shop_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_shop_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/function/function_skin_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/function/function_skin_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/price/price_gear_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/price/price_gear_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/product/product_price_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/product/product_price_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/special/special_goods_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/special/special_goods_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/store/store_asset_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/store/store_asset_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_count_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_count_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/task/task_log_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/task/task_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_account_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_account_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_address_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_address_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_asset_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_asset_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_black_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_black_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/user/user_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/db_models/version/version_info_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/db_models/version/version_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/enum.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/frame_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/frame_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-08-11 09:10:33
-@LastEditTime: 2024-02-01 19:06:28
+@LastEditTime: 2024-03-18 09:53:41
 @LastEditors: HuangJianYi
 @Description: 
 """
 from seven_cloudapp_frame.libs.customize.seven_helper import *
 from seven_cloudapp_frame.libs.customize.safe_helper import SafeHelper
 from seven_cloudapp_frame.libs.common import *
 from seven_cloudapp_frame.models.seven_model import *
@@ -147,14 +147,48 @@
             probability_list.append(current_prize)
             init_value = init_value + prize[field_name]
         prize_index = random.randint(0, init_value - 1)
         for prize in probability_list:
             if (prize["start_probability"] <= prize_index and prize_index < prize["end_probability"]):
                 return prize
 
+    def rounding_algorithm(self, number):
+        """
+        :description: "四舍六入五成双"（也称为 banker's rounding 或 commercial rounding）算法通常在金融、会计、计量等领域中被广泛应用，尤其是在需要精确计数和汇总大量数据以避免系统性偏差的情况下。这种舍入方法的主要目的是减少长时间多次舍入累积误差，使得统计结果更为准确   
+        :param number: 数值
+        :return: number
+        :last_editors: HuangJianYi
+        """
+        
+        import math
+        
+        if number < 0.001:
+            return 0
+
+        int_part = int(number)
+        decimal_part = abs(number - int_part)  # 直接取绝对值的小数部分
+
+        # 如果小数部分长度不足三位，则直接四舍五入到两位小数
+        if decimal_part * 1000 % 1 == 0:
+            return round(number, 2)
+
+        third_decimal_digit = (decimal_part * 100) % 10  # 获取第三位小数
+
+        if third_decimal_digit != 5 or decimal_part * 10 % 1 == 0:  # 不是五或没有更精确的小数位
+            rounded_number = round(number, 2)
+        else:
+            second_decimal_digit = (decimal_part * 100) // 10 % 10  # 获取第二位小数
+            if second_decimal_digit % 2 == 0:  # 第二位小数为偶数，则向下舍弃
+                decimal_part = math.floor(decimal_part * 100) / 100
+            else:  # 第二位小数为奇数，则向上进位
+                decimal_part = math.ceil(decimal_part * 100) / 100
+            rounded_number = int_part + decimal_part
+            
+        return rounded_number
+    
     def rewards_status(self):
         """
         :description: 给予奖励的子订单状态
         :param 
         :return: 
         :last_editors: HuangJianYi
         """
```

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/goods_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/goods_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/ip_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/ip_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/launch_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/launch_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/module_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/module_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/mp_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/mp_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/operate_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/operate_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/order_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/order_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/price_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/price_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/prize_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/prize_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/push_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/push_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/seven_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/stat_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/stat_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/task_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/task_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/theme_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/theme_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/third/jd_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/third/jd_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/third/shakeshop_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/third/shakeshop_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/top_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/top_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/models/user_base_model.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/models/user_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame/route.py` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame/route.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/PKG-INFO` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_cloudapp_frame
-Version: 1.1.8
+Version: 1.1.9
 Summary: seven cloudapp frame
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_frame.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
```

### Comparing `seven_cloudapp_frame-1.1.8/seven_cloudapp_frame.egg-info/SOURCES.txt` & `seven_cloudapp_frame-1.1.9/seven_cloudapp_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

