# Comparing `tmp/buildz-0.4.3.tar.gz` & `tmp/buildz-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.4.3.tar", last modified: Sun Mar 31 10:48:28 2024, max compression
+gzip compressed data, was "buildz-0.4.4.tar", last modified: Mon Apr  1 13:52:43 2024, max compression
```

## Comparing `buildz-0.4.3.tar` & `buildz-0.4.4.tar`

### file list

```diff
@@ -1,132 +1,143 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.822745 buildz-0.4.3/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.3/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2024-03-31 10:48:28.822745 buildz-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5335 2023-10-16 14:40:02.000000 buildz-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.728994 buildz-0.4.3/buildz/
--rw-rw-rw-   0        0        0     1067 2024-03-31 08:21:57.000000 buildz-0.4.3/buildz/__init__.py
--rw-rw-rw-   0        0        0      355 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/__main__.py
--rw-rw-rw-   0        0        0     1775 2024-02-28 03:15:25.000000 buildz-0.4.3/buildz/base.py
--rw-rw-rw-   0        0        0     7869 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/build.py
--rw-rw-rw-   0        0        0    10964 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/confz.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.713366 buildz-0.4.3/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.744629 buildz-0.4.3/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      814 2024-03-31 10:45:00.000000 buildz-0.4.3/buildz/demo/ioc/test.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.744629 buildz-0.4.3/buildz/demo/ioc/test_conf/
--rw-rw-rw-   0        0        0      573 2024-03-30 10:09:18.000000 buildz-0.4.3/buildz/demo/ioc/test_conf/base.js
--rw-rw-rw-   0        0        0     1102 2024-03-31 10:45:53.000000 buildz-0.4.3/buildz/demo/ioc/test_conf/data1.js
--rw-rw-rw-   0        0        0      398 2024-03-31 08:55:33.000000 buildz-0.4.3/buildz/demo/ioc/test_conf/data2.js
--rw-rw-rw-   0        0        0      362 2024-03-30 15:22:31.000000 buildz-0.4.3/buildz/demo/ioc/test_conf/data3.js
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.760249 buildz-0.4.3/buildz/demo/x/
--rw-rw-rw-   0        0        0      546 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/demo.confz
--rw-rw-rw-   0        0        0      522 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/demo.py
--rw-rw-rw-   0        0        0      476 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/run.confz
--rw-rw-rw-   0        0        0      464 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/test.confz
--rw-rw-rw-   0        0        0      217 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/test.py
--rw-rw-rw-   0        0        0      240 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/testc.py
--rw-rw-rw-   0        0        0      780 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/testf.py
--rw-rw-rw-   0        0        0     1197 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/testz.py
--rw-rw-rw-   0        0        0      375 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/value.confz
--rw-rw-rw-   0        0        0      174 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/demo/x/x.py
--rw-rw-rw-   0        0        0        0 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/dj.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.760249 buildz-0.4.3/buildz/ioc/
--rw-rw-rw-   0        0        0       40 2024-03-31 10:20:19.000000 buildz-0.4.3/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.3/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.760249 buildz-0.4.3/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0      971 2024-03-31 09:07:56.000000 buildz-0.4.3/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     4266 2024-03-31 10:19:09.000000 buildz-0.4.3/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0     9786 2024-03-31 08:54:57.000000 buildz-0.4.3/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.775870 buildz-0.4.3/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4522 2024-03-31 09:45:12.000000 buildz-0.4.3/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1128 2024-03-31 09:56:22.000000 buildz-0.4.3/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0      936 2024-03-31 10:45:14.000000 buildz-0.4.3/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.775870 buildz-0.4.3/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-03-31 10:41:23.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-03-31 10:41:10.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      984 2024-03-31 10:43:16.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-03-31 09:29:07.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      476 2024-03-31 09:44:23.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0       94 2024-03-31 03:42:49.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      626 2024-03-31 09:33:20.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      411 2024-03-31 10:04:44.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      416 2024-03-31 07:52:50.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.3/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.3/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      524 2024-03-31 09:08:42.000000 buildz-0.4.3/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0     1487 2024-03-31 10:48:09.000000 buildz-0.4.3/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     2861 2024-03-31 10:00:11.000000 buildz-0.4.3/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1096 2024-03-31 10:05:27.000000 buildz-0.4.3/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0      536 2024-03-31 09:09:01.000000 buildz-0.4.3/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      279 2024-03-31 07:26:16.000000 buildz-0.4.3/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0      823 2024-03-31 10:07:06.000000 buildz-0.4.3/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/keys.py
--rw-rw-rw-   0        0        0     1112 2024-03-31 02:32:18.000000 buildz-0.4.3/buildz/pyz.py
--rw-rw-rw-   0        0        0     1750 2024-02-22 17:23:17.000000 buildz-0.4.3/buildz/test_loader copy.py
--rw-rw-rw-   0        0        0      336 2024-03-01 16:45:49.000000 buildz-0.4.3/buildz/test_loader.py
--rw-rw-rw-   0        0        0      658 2024-03-01 16:51:21.000000 buildz-0.4.3/buildz/test_writer.py
--rw-rw-rw-   0        0        0      843 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.791496 buildz-0.4.3/buildz/xconfz/
--rw-rw-rw-   0        0        0      563 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/__init__.py
--rw-rw-rw-   0        0        0     6031 2024-02-27 10:34:54.000000 buildz-0.4.3/buildz/xconfz/base.py
--rw-rw-rw-   0        0        0     1688 2023-10-29 17:50:27.000000 buildz-0.4.3/buildz/xconfz/buff.py
--rw-rw-rw-   0        0        0      234 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fc.py
--rw-rw-rw-   0        0        0     2307 2024-02-27 10:34:12.000000 buildz-0.4.3/buildz/xconfz/fc_item.py
--rw-rw-rw-   0        0        0     2704 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fc_list.py
--rw-rw-rw-   0        0        0     3043 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fc_map.py
--rw-rw-rw-   0        0        0     1791 2024-02-27 10:33:39.000000 buildz-0.4.3/buildz/xconfz/fc_set.py
--rw-rw-rw-   0        0        0     2900 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fc_str.py
--rw-rw-rw-   0        0        0     2862 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fc_type.py
--rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/file.py
--rw-rw-rw-   0        0        0     4031 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fmt_base.py
--rw-rw-rw-   0        0        0     1387 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fmt_str.py
--rw-rw-rw-   0        0        0     2121 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/fmt_type.py
--rw-rw-rw-   0        0        0     4378 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xconfz/mg.py
--rw-rw-rw-   0        0        0     4264 2024-02-27 10:36:33.000000 buildz-0.4.3/buildz/xconfz/mg_fmt.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.791496 buildz-0.4.3/buildz/xf/
--rw-rw-rw-   0        0        0      105 2024-03-31 08:22:13.000000 buildz-0.4.3/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.3/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.807123 buildz-0.4.3/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.3/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.3/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.807123 buildz-0.4.3/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.3/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.3/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.3/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.3/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.3/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.3/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.3/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.3/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.3/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     2806 2024-03-21 08:07:18.000000 buildz-0.4.3/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.3/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.3/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.3/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.3/buildz/xf/loader/pos.py
--rw-rw-rw-   0        0        0     1093 2024-03-31 03:05:04.000000 buildz-0.4.3/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2385 2024-03-06 07:06:32.000000 buildz-0.4.3/buildz/xf/read.py
--rw-rw-rw-   0        0        0     1314 2024-02-24 09:19:50.000000 buildz-0.4.3/buildz/xf/test_write.py
--rw-rw-rw-   0        0        0     1203 2024-03-01 16:51:07.000000 buildz-0.4.3/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.807123 buildz-0.4.3/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.3/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.3/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.822745 buildz-0.4.3/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.3/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.3/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.3/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.3/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1377 2024-02-24 09:43:55.000000 buildz-0.4.3/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.3/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.3/buildz/xf/writer/mg.py
-drwxrwxrwx   0        0        0        0 2024-03-31 10:48:28.744629 buildz-0.4.3/buildz.egg-info/
--rw-rw-rw-   0        0        0     5750 2024-03-31 10:48:28.000000 buildz-0.4.3/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2983 2024-03-31 10:48:28.000000 buildz-0.4.3/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 10:48:28.000000 buildz-0.4.3/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-31 10:48:28.000000 buildz-0.4.3/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 10:48:28.822745 buildz-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-03-31 10:48:19.000000 buildz-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.719395 buildz-0.4.4/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5750 2024-04-01 13:52:43.719395 buildz-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5335 2023-10-16 14:40:02.000000 buildz-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.294190 buildz-0.4.4/buildz/
+-rw-rw-rw-   0        0        0       81 2024-04-01 13:50:26.000000 buildz-0.4.4/buildz/__init__.py
+-rw-rw-rw-   0        0        0     1165 2024-04-01 13:42:56.000000 buildz-0.4.4/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.238638 buildz-0.4.4/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.309809 buildz-0.4.4/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      964 2024-04-01 13:51:18.000000 buildz-0.4.4/buildz/demo/ioc/test.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.325412 buildz-0.4.4/buildz/demo/ioc/test_conf/
+-rw-rw-rw-   0        0        0      573 2024-03-30 10:09:18.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/base.js
+-rw-rw-rw-   0        0        0     1328 2024-04-01 11:15:14.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/data1.js
+-rw-rw-rw-   0        0        0      398 2024-03-31 08:55:33.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/data2.js
+-rw-rw-rw-   0        0        0      362 2024-03-30 15:22:31.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/data3.js
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.325412 buildz-0.4.4/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      162 2024-04-01 11:24:41.000000 buildz-0.4.4/buildz/demo/xf/test.js
+-rw-rw-rw-   0        0        0      251 2024-04-01 12:36:42.000000 buildz-0.4.4/buildz/demo/xf/test.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/dj.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.341064 buildz-0.4.4/buildz/ioc/
+-rw-rw-rw-   0        0        0       40 2024-03-31 10:20:19.000000 buildz-0.4.4/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.4/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.356691 buildz-0.4.4/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0      971 2024-03-31 09:07:56.000000 buildz-0.4.4/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     4266 2024-03-31 10:19:09.000000 buildz-0.4.4/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0     9786 2024-03-31 08:54:57.000000 buildz-0.4.4/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.404564 buildz-0.4.4/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     4522 2024-03-31 09:45:12.000000 buildz-0.4.4/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1128 2024-03-31 09:56:22.000000 buildz-0.4.4/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0      936 2024-03-31 10:45:14.000000 buildz-0.4.4/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.419600 buildz-0.4.4/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-03-31 10:41:23.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-03-31 10:41:10.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0     1089 2024-04-01 11:12:34.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-03-31 09:29:07.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      476 2024-03-31 09:44:23.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0       94 2024-03-31 03:42:49.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      626 2024-03-31 09:33:20.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      411 2024-03-31 10:04:44.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 07:52:50.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.4/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      524 2024-03-31 09:08:42.000000 buildz-0.4.4/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      606 2024-04-01 11:11:54.000000 buildz-0.4.4/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0     1487 2024-03-31 10:48:09.000000 buildz-0.4.4/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     2861 2024-03-31 10:00:11.000000 buildz-0.4.4/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1096 2024-03-31 10:05:27.000000 buildz-0.4.4/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0      536 2024-03-31 09:09:01.000000 buildz-0.4.4/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      279 2024-03-31 07:26:16.000000 buildz-0.4.4/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0      823 2024-03-31 10:07:06.000000 buildz-0.4.4/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/keys.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.450893 buildz-0.4.4/buildz/old_version/
+-rw-rw-rw-   0        0        0     1055 2024-04-01 11:19:41.000000 buildz-0.4.4/buildz/old_version/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-04-01 11:19:32.000000 buildz-0.4.4/buildz/old_version/__main__.py
+-rw-rw-rw-   0        0        0     1775 2024-02-28 03:15:25.000000 buildz-0.4.4/buildz/old_version/base.py
+-rw-rw-rw-   0        0        0     7859 2024-04-01 11:19:19.000000 buildz-0.4.4/buildz/old_version/build.py
+-rw-rw-rw-   0        0        0    10964 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/confz.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.242235 buildz-0.4.4/buildz/old_version/demo/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.513811 buildz-0.4.4/buildz/old_version/demo/x/
+-rw-rw-rw-   0        0        0      546 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/demo.confz
+-rw-rw-rw-   0        0        0      522 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/demo.py
+-rw-rw-rw-   0        0        0      476 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/run.confz
+-rw-rw-rw-   0        0        0      464 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/test.confz
+-rw-rw-rw-   0        0        0      217 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/test.py
+-rw-rw-rw-   0        0        0      240 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/testc.py
+-rw-rw-rw-   0        0        0      780 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/testf.py
+-rw-rw-rw-   0        0        0     1197 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/testz.py
+-rw-rw-rw-   0        0        0      375 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/value.confz
+-rw-rw-rw-   0        0        0      174 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/x.py
+-rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/keys.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.593439 buildz-0.4.4/buildz/old_version/xconfz/
+-rw-rw-rw-   0        0        0      524 2024-04-01 11:20:18.000000 buildz-0.4.4/buildz/old_version/xconfz/__init__.py
+-rw-rw-rw-   0        0        0     6026 2024-04-01 11:20:26.000000 buildz-0.4.4/buildz/old_version/xconfz/base.py
+-rw-rw-rw-   0        0        0     1675 2024-04-01 11:20:36.000000 buildz-0.4.4/buildz/old_version/xconfz/buff.py
+-rw-rw-rw-   0        0        0      156 2024-04-01 11:21:03.000000 buildz-0.4.4/buildz/old_version/xconfz/fc.py
+-rw-rw-rw-   0        0        0     2281 2024-04-01 11:20:44.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_item.py
+-rw-rw-rw-   0        0        0     2678 2024-04-01 11:20:47.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_list.py
+-rw-rw-rw-   0        0        0     3017 2024-04-01 11:20:50.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_map.py
+-rw-rw-rw-   0        0        0     1778 2024-04-01 11:20:53.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_set.py
+-rw-rw-rw-   0        0        0     2887 2024-04-01 11:20:56.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_str.py
+-rw-rw-rw-   0        0        0     2823 2024-04-01 11:20:59.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_type.py
+-rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/xconfz/file.py
+-rw-rw-rw-   0        0        0     4018 2024-04-01 11:21:08.000000 buildz-0.4.4/buildz/old_version/xconfz/fmt_base.py
+-rw-rw-rw-   0        0        0     1322 2024-04-01 11:21:16.000000 buildz-0.4.4/buildz/old_version/xconfz/fmt_str.py
+-rw-rw-rw-   0        0        0     2069 2024-04-01 11:21:20.000000 buildz-0.4.4/buildz/old_version/xconfz/fmt_type.py
+-rw-rw-rw-   0        0        0     4326 2024-04-01 11:21:30.000000 buildz-0.4.4/buildz/old_version/xconfz/mg.py
+-rw-rw-rw-   0        0        0     4186 2024-04-01 11:21:23.000000 buildz-0.4.4/buildz/old_version/xconfz/mg_fmt.py
+-rw-rw-rw-   0        0        0     1112 2024-03-31 02:32:18.000000 buildz-0.4.4/buildz/pyz.py
+-rw-rw-rw-   0        0        0     1750 2024-02-22 17:23:17.000000 buildz-0.4.4/buildz/test_loader copy.py
+-rw-rw-rw-   0        0        0      336 2024-03-01 16:45:49.000000 buildz-0.4.4/buildz/test_loader.py
+-rw-rw-rw-   0        0        0      658 2024-03-01 16:51:21.000000 buildz-0.4.4/buildz/test_writer.py
+-rw-rw-rw-   0        0        0      843 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.624698 buildz-0.4.4/buildz/xf/
+-rw-rw-rw-   0        0        0      139 2024-04-01 13:46:42.000000 buildz-0.4.4/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.646804 buildz-0.4.4/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.4/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.4/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.688145 buildz-0.4.4/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.4/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.4/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.4/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.4/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.4/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.4/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.4/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.4/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.4/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     2806 2024-03-21 08:07:18.000000 buildz-0.4.4/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.4/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.4/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.4/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.4/buildz/xf/loader/pos.py
+-rw-rw-rw-   0        0        0     1093 2024-03-31 03:05:04.000000 buildz-0.4.4/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2385 2024-03-06 07:06:32.000000 buildz-0.4.4/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     1314 2024-02-24 09:19:50.000000 buildz-0.4.4/buildz/xf/test_write.py
+-rw-rw-rw-   0        0        0     1203 2024-03-01 16:51:07.000000 buildz-0.4.4/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.703801 buildz-0.4.4/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.4/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.4/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.719395 buildz-0.4.4/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.4/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.4/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.4/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.4/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1377 2024-02-24 09:43:55.000000 buildz-0.4.4/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.4/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.4/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.4/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.309809 buildz-0.4.4/buildz.egg-info/
+-rw-rw-rw-   0        0        0     5750 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3546 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 13:52:43.719395 buildz-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-01 11:15:48.000000 buildz-0.4.4/setup.py
```

### Comparing `buildz-0.4.3/LICENSE` & `buildz-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/PKG-INFO` & `buildz-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.3
+Version: 0.4.4
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.3/README.md` & `buildz-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/__init__.py` & `buildz-0.4.4/buildz/old_version/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #from buildz.confz import read, loadfile, output, fread
-from buildz.build import Builder, main
-from buildz.keys import help
+from .build import Builder, main
+from .keys import help
 """
 json-like(called 'confz' in here) data format function:
     read: string -> obj
     output: obj -> string
     fread(filepath, coding="utf-8"): filepath -> string 
         #open(filepath, 'rb').read().decode(coding)
     loadfile(filepath, coding="utf-8"): filepath -> obj
```

### Comparing `buildz-0.4.3/buildz/base.py` & `buildz-0.4.4/buildz/old_version/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/build.py` & `buildz-0.4.4/buildz/old_version/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,22 @@
     return dict(maps)
 
 pass
 builtins._list = build_list
 builtins._dict = build_dict
 g_default_import = "buildz"+".base"
 def read_confz(filepath):
-    from buildz import confz
+    from . import confz
     s = confz.fread(filepath)
     obj = confz.read(s)
     return obj
 
 pass
 def read_json(filepath):
-    from buildz import confz
+    from . import confz
     import json
     s = confz.fread(filepath)
     obj = json.loads(s)
     return obj
 
 pass
```

### Comparing `buildz-0.4.3/buildz/confz.py` & `buildz-0.4.4/buildz/old_version/confz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/demo/ioc/test.py` & `buildz-0.4.4/buildz/demo/ioc/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #
 from buildz.ioc import build
 from buildz import xf
+from buildz import argx
 import os
 join = os.path.join
 class Test:
     def __init__(self, *args, **maps):
         print(f"Test init args: {args}, maps: {maps}")
         self.args = args
         self.maps = maps
     def run(self):
         print(f"get obj:{self}")
         print("get_obj.obj:", self.obj)
+        print(f"ioc: {self.ioc}")
+        print(f"ioc env: {self.ioc.get_env('path')}")
 
 pass
 fps = xf.loads("[data1.js, data2.js, data3.js]")[:2]
 
 fps = [join('test_conf', fp) for fp in fps]
 def show():
     print("run show")
@@ -26,14 +29,15 @@
         confs.add_fp(fp)
     #obj =  confs.get("data1.test")
     confs.get("data1.run")
     obj = confs.get("data1.test.obj")
     print(f"obj: {obj}")
     print("DO CALLS")
     confs.get("data1.calls")
+    print("ARGS: ", argx.fetch())
 
 pass
 
 if __name__=="__main__":
     test()
 
 pass
```

### Comparing `buildz-0.4.3/buildz/demo/ioc/test_conf/base.js` & `buildz-0.4.4/buildz/demo/ioc/test_conf/base.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/demo/x/demo.confz` & `buildz-0.4.4/buildz/old_version/demo/x/demo.confz`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/demo/x/demo.py` & `buildz-0.4.4/buildz/old_version/demo/x/demo.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/demo/x/testf.py` & `buildz-0.4.4/buildz/old_version/demo/x/testf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/demo/x/testz.py` & `buildz-0.4.4/buildz/old_version/demo/x/testz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc/base.py` & `buildz-0.4.4/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc/conf.py` & `buildz-0.4.4/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc/confs.py` & `buildz-0.4.4/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/base.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/call.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/calls.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.4.4/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -23,9 +23,12 @@
         build: buildz.ioc.ioc_deal.call.CallDeal
     }, {
         type: var,
         build: buildz.ioc.ioc_deal.var.VarDeal
     }, {
         type: calls,
         build: buildz.ioc.ioc_deal.calls.CallsDeal
+    }, {
+        type: ioc,
+        build: buildz.ioc.ioc_deal.ioc.IOCObjectDeal
     }]
 }
```

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/env.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/obj.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/ref.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/ioc/ioc_deal/var.py` & `buildz-0.4.4/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/keys.py` & `buildz-0.4.4/buildz/keys.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/pyz.py` & `buildz-0.4.4/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/test_loader copy.py` & `buildz-0.4.4/buildz/test_loader copy.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/test_writer.py` & `buildz-0.4.4/buildz/test_writer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/tools.py` & `buildz-0.4.4/buildz/tools.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xconfz/__init__.py` & `buildz-0.4.4/buildz/old_version/xconfz/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #coding=utf-8
 
-from buildz.xconfz.mg import *
-from buildz.xconfz.mg_fmt import *
-from buildz.xconfz.file import *
+from .mg import *
+from .mg_fmt import *
+from .file import *
 
 """
 loads(string) => object
 
 dumps(object, format = False, simple = 1, as_json = False, t_single = True) => string
 format: 是否格式化
 as_json: 数值用json方法生成
```

### Comparing `buildz-0.4.3/buildz/xconfz/base.py` & `buildz-0.4.4/buildz/old_version/xconfz/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #coding=utf-8
 
-from buildz.base import Map
+from ..base import Map
 '''
 格式化报错
 '''
 class FormatExp(Exception):
     def __init__(self, err, data, s = ""):
         if len(s)==0:
             errs = "Error: {err}, line: {line}, index: {index}".format(err = err, line = data[0], index = data[1])
```

### Comparing `buildz-0.4.3/buildz/xconfz/buff.py` & `buildz-0.4.4/buildz/old_version/xconfz/buff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #coding=utf-8
 
-from buildz.xconfz.base import *
+from .base import *
 
 class BufferImpl(Buffer):
     def cal_pos(self, s):
         n = "\n"
         if type(s)==bytes:
             n = b"\n"
         arr= s.split(n)
```

### Comparing `buildz-0.4.3/buildz/xconfz/fc_item.py` & `buildz-0.4.4/buildz/old_version/xconfz/fc_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #coding=utf-8
-from buildz.xconfz.base import *
+from .base import *
 
-from buildz.xconfz.fmt_base import *
+from .fmt_base import *
 
 """
 去左空格
 """
 class SpcDeal(BaseDeal):
     def prev(self, buff, stack):
         if buff.remain_size()==0:
```

### Comparing `buildz-0.4.3/buildz/xconfz/fc_list.py` & `buildz-0.4.4/buildz/old_version/xconfz/fc_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #coding=utf-8
-from buildz.xconfz.base import *
+from .base import *
 
-from buildz.xconfz.fmt_base import *
+from .fmt_base import *
 
 class ListDeal(BaseDeal):
     def init(self, reg):
         self.k_l = reg(self.l)
         self.k_r = reg(self.r)
     def __init__(self, left, right):
         self.l = left
```

### Comparing `buildz-0.4.3/buildz/xconfz/fc_map.py` & `buildz-0.4.4/buildz/old_version/xconfz/fc_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #coding=utf-8
-from buildz.xconfz.base import *
+from .base import *
 
-from buildz.xconfz.fmt_base import *
+from .fmt_base import *
 
 class MapDeal(BaseDeal):
     def init(self, reg):
         self.k_l = reg(self.l)
         self.k_r = reg(self.r)
     def __init__(self, left, right):
         self.l = left
```

### Comparing `buildz-0.4.3/buildz/xconfz/fc_set.py` & `buildz-0.4.4/buildz/old_version/xconfz/fc_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #coding=utf-8
-from buildz.xconfz.base import *
+from .base import *
 
 class TypeSet:
     def __str__(self):
         return "@@TypeSet"
     def __repr__(self):
         return str(self)
```

### Comparing `buildz-0.4.3/buildz/xconfz/fc_str.py` & `buildz-0.4.4/buildz/old_version/xconfz/fc_str.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #coding=utf-8
-from buildz.xconfz.base import *
+from .base import *
 
 
 class StrDeal(BaseDeal):
     def __init__(self, left = '"', right= '"', single_line = False, note = False):
         self.left = left
         self.right = right
         self.single_line = single_line
```

### Comparing `buildz-0.4.3/buildz/xconfz/fc_type.py` & `buildz-0.4.4/buildz/old_version/xconfz/fc_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #coding=utf-8
-from buildz.xconfz.base import *
-from buildz.xconfz.fc_list import *
-from buildz.xconfz.fc_set import *
+from .base import *
+from .fc_list import *
+from .fc_set import *
 
 
 """
 二元符<val, type>
 
 """
```

### Comparing `buildz-0.4.3/buildz/xconfz/file.py` & `buildz-0.4.4/buildz/old_version/xconfz/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xconfz/fmt_base.py` & `buildz-0.4.4/buildz/old_version/xconfz/fmt_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #coding=utf-8
-from buildz.xconfz.base import *
+from .base import *
 """
 返回Node
 """
 class BaseFormat:
     def init(self):
         return self
     def deal(self, data, fc, **params):
```

### Comparing `buildz-0.4.3/buildz/xconfz/fmt_str.py` & `buildz-0.4.4/buildz/old_version/xconfz/fmt_str.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 """
 impl in class
 """
 
 import io
 # io.StringIO("asdf")
-from buildz.xconfz.buff import *
-from buildz.xconfz.fc import *
+from .buff import *
+from .fc import *
 
-from buildz.xconfz.fmt_base import *
-from buildz.xconfz.fmt_type import *
-from buildz.xconfz.mg import *
+from .fmt_base import *
+from .fmt_type import *
+from .mg import *
 
 
 
 class StrForamt(BaseFormat):
     def __init__(self, reg, symbol = '"', bts = False, single = True, t_single = False):
         self.symbol = symbol
         self.reg = reg
```

### Comparing `buildz-0.4.3/buildz/xconfz/fmt_type.py` & `buildz-0.4.4/buildz/old_version/xconfz/fmt_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #coding=utf-8
-from buildz.xconfz.base import *
-from buildz.xconfz.fc_list import *
-from buildz.xconfz.fc_set import *
+from .base import *
+from .fc_list import *
+from .fc_set import *
 
-from buildz.xconfz.fmt_base import *
+from .fmt_base import *
 
 """
 二元符<val, type>
 
 """
 
 class TypeDealAFormat(BaseFormat):
```

### Comparing `buildz-0.4.3/buildz/xconfz/mg.py` & `buildz-0.4.4/buildz/old_version/xconfz/mg.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 """
 impl in class
 """
 
 import io
 # io.StringIO("asdf")
-from buildz.xconfz.buff import *
-from buildz.xconfz.fc import *
-from buildz.xconfz.fmt_base import *
+from .buff import *
+from .fc import *
+from .fmt_base import *
 
 class Confz:
     def fcs(self, fc, *args, **maps):
         return fc(*self.cs(*args), **maps)
     def add_fc(self, fc, *args, **maps):
         obj = self.fcs(fc, *args, **maps)
         self.add(obj)
@@ -151,13 +151,13 @@
 import io
 def loads(s):
     cfz = build(type(s)==bytes)
     return cfz.load(io.StringIO(s).read)
 
 pass
 
-from buildz.xconfz.file import *
+from .file import *
 
 def loadfile(fp, coding = 'utf-8'):
     return loads(fread(fp, coding))
 
 pass
```

### Comparing `buildz-0.4.3/buildz/xconfz/mg_fmt.py` & `buildz-0.4.4/buildz/old_version/xconfz/mg_fmt.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 """
 impl in class
 """
 
 import io
 # io.StringIO("asdf")
-from buildz.xconfz.buff import *
-from buildz.xconfz.fc import *
+from .buff import *
+from .fc import *
 
-from buildz.xconfz.fmt_base import *
-from buildz.xconfz.fmt_type import *
-from buildz.xconfz.fmt_str import *
-from buildz.xconfz.mg import *
+from .fmt_base import *
+from .fmt_type import *
+from .fmt_str import *
+from .mg import *
 
 class Buildz:
     def __init__(self, bts= False):
         self.bts= bts
         self.deals = {}
         self._default = None
     def default(self, _def):
```

### Comparing `buildz-0.4.3/buildz/xf/file.py` & `buildz-0.4.4/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/base.py` & `buildz-0.4.4/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/buffer.py` & `buildz-0.4.4/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/listz.py` & `buildz-0.4.4/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/lr.py` & `buildz-0.4.4/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/lrval.py` & `buildz-0.4.4/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/mapz.py` & `buildz-0.4.4/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/nextz.py` & `buildz-0.4.4/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/reval.py` & `buildz-0.4.4/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/setz.py` & `buildz-0.4.4/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/spt.py` & `buildz-0.4.4/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/deal/strz.py` & `buildz-0.4.4/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/item.py` & `buildz-0.4.4/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/mg.py` & `buildz-0.4.4/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/loader/pos.py` & `buildz-0.4.4/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/mapz.py` & `buildz-0.4.4/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/read.py` & `buildz-0.4.4/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/test_write.py` & `buildz-0.4.4/buildz/xf/test_write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/write.py` & `buildz-0.4.4/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/base.py` & `buildz-0.4.4/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/conf.py` & `buildz-0.4.4/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/deal/listz.py` & `buildz-0.4.4/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/deal/mapz.py` & `buildz-0.4.4/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/deal/strz.py` & `buildz-0.4.4/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/itemz.py` & `buildz-0.4.4/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz/xf/writer/mg.py` & `buildz-0.4.4/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.3/buildz.egg-info/PKG-INFO` & `buildz-0.4.4/buildz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.3
+Version: 0.4.4
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.3/setup.py` & `buildz-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.4.3',
+    version = '0.4.4',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-like file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

