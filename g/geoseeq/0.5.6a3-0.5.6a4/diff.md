# Comparing `tmp/geoseeq-0.5.6a3.tar.gz` & `tmp/geoseeq-0.5.6a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.5.6a3.tar", last modified: Mon Apr  1 15:54:39 2024, max compression
+gzip compressed data, was "geoseeq-0.5.6a4.tar", last modified: Mon Apr  1 16:15:48 2024, max compression
```

## Comparing `geoseeq-0.5.6a3.tar` & `geoseeq-0.5.6a4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.788587 geoseeq-0.5.6a3/
--rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a3/LICENSE
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-01 15:54:39.788297 geoseeq-0.5.6a3/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a3/README.md
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.759268 geoseeq-0.5.6a3/geoseeq/
--rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a3/geoseeq/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a3/geoseeq/app.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a3/geoseeq/blob_constructors.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a3/geoseeq/bulk_creators.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.768121 geoseeq-0.5.6a3/geoseeq/cli/
--rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/cli/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/cli/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/copy.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/detail.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a3/geoseeq/cli/download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a3/geoseeq/cli/fastq_utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/get_eula.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3199 2024-04-01 15:48:20.000000 geoseeq-0.5.6a3/geoseeq/cli/main.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/manage.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a3/geoseeq/cli/progress_bar.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/run.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/search.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.770275 geoseeq-0.5.6a3/geoseeq/cli/shared_params/
--rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/common_state.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/config.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/id_handlers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/obj_getters.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/opts_and_args.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.771592 geoseeq-0.5.6a3/geoseeq/cli/upload/
--rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8963 2024-03-18 23:39:08.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/upload_advanced.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7264 2024-03-19 00:09:27.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/upload_reads.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a3/geoseeq/cli/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a3/geoseeq/cli/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/view.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a3/geoseeq/constants.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.771983 geoseeq-0.5.6a3/geoseeq/contrib/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/contrib/__init__.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.773336 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/api.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/bioproject.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/setup_logging.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4101 2024-03-21 02:53:18.000000 geoseeq-0.5.6a3/geoseeq/file_system_cache.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.775758 geoseeq-0.5.6a3/geoseeq/id_constructors/
--rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_blobs.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_ids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_names.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_uuids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/resolvers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a3/geoseeq/knex.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a3/geoseeq/organization.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a3/geoseeq/pipeline.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.777161 geoseeq-0.5.6a3/geoseeq/plotting/
--rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a3/geoseeq/plotting/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a3/geoseeq/plotting/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a3/geoseeq/plotting/highcharts.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.778512 geoseeq-0.5.6a3/geoseeq/plotting/map/
--rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/base_layer.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/map.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/overlay.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a3/geoseeq/plotting/selectable.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a3/geoseeq/project.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6816 2024-03-19 00:06:20.000000 geoseeq-0.5.6a3/geoseeq/remote_object.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.781800 geoseeq-0.5.6a3/geoseeq/result/
--rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a3/geoseeq/result/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a3/geoseeq/result/bioinfo.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4589 2024-03-06 22:35:53.000000 geoseeq-0.5.6a3/geoseeq/result/file_download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7390 2024-03-18 21:44:44.000000 geoseeq-0.5.6a3/geoseeq/result/file_upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a3/geoseeq/result/result_file.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a3/geoseeq/result/result_folder.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a3/geoseeq/result/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a3/geoseeq/sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a3/geoseeq/search.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7090 2024-03-19 13:53:30.000000 geoseeq-0.5.6a3/geoseeq/upload_download_manager.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a3/geoseeq/utils.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.785713 geoseeq-0.5.6a3/geoseeq/vc/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a3/geoseeq/vc/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a3/geoseeq/vc/checksum.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a3/geoseeq/vc/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/clone.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_dir.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_stub.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a3/geoseeq/work_orders.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.787799 geoseeq-0.5.6a3/geoseeq.egg-info/
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/SOURCES.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/dependency_links.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/entry_points.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/top_level.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-01 15:48:31.000000 geoseeq-0.5.6a3/pyproject.toml
--rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-01 15:54:39.788649 geoseeq-0.5.6a3/setup.cfg
--rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-04-01 15:48:45.000000 geoseeq-0.5.6a3/setup.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.787349 geoseeq-0.5.6a3/tests/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a3/tests/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a3/tests/test_api_client.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a3/tests/test_plotting.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.265193 geoseeq-0.5.6a4/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a4/LICENSE
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-01 16:15:48.264941 geoseeq-0.5.6a4/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a4/README.md
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.249949 geoseeq-0.5.6a4/geoseeq/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a4/geoseeq/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a4/geoseeq/app.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a4/geoseeq/blob_constructors.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a4/geoseeq/bulk_creators.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.253849 geoseeq-0.5.6a4/geoseeq/cli/
+-rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/cli/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/cli/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/copy.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/detail.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a4/geoseeq/cli/download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a4/geoseeq/cli/fastq_utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/get_eula.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3211 2024-04-01 16:15:34.000000 geoseeq-0.5.6a4/geoseeq/cli/main.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/manage.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a4/geoseeq/cli/progress_bar.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/run.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/search.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.255195 geoseeq-0.5.6a4/geoseeq/cli/shared_params/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a4/geoseeq/cli/shared_params/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a4/geoseeq/cli/shared_params/common_state.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a4/geoseeq/cli/shared_params/config.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a4/geoseeq/cli/shared_params/id_handlers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a4/geoseeq/cli/shared_params/obj_getters.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a4/geoseeq/cli/shared_params/opts_and_args.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.256040 geoseeq-0.5.6a4/geoseeq/cli/upload/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a4/geoseeq/cli/upload/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8963 2024-03-18 23:39:08.000000 geoseeq-0.5.6a4/geoseeq/cli/upload/upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a4/geoseeq/cli/upload/upload_advanced.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7264 2024-03-19 00:09:27.000000 geoseeq-0.5.6a4/geoseeq/cli/upload/upload_reads.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a4/geoseeq/cli/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a4/geoseeq/cli/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a4/geoseeq/cli/view.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a4/geoseeq/constants.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.256586 geoseeq-0.5.6a4/geoseeq/contrib/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/contrib/__init__.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.257515 geoseeq-0.5.6a4/geoseeq/contrib/ncbi/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/contrib/ncbi/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a4/geoseeq/contrib/ncbi/api.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a4/geoseeq/contrib/ncbi/bioproject.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a4/geoseeq/contrib/ncbi/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/contrib/ncbi/setup_logging.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4101 2024-03-21 02:53:18.000000 geoseeq-0.5.6a4/geoseeq/file_system_cache.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.259442 geoseeq-0.5.6a4/geoseeq/id_constructors/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/from_blobs.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/from_ids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/from_names.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/from_uuids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/resolvers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a4/geoseeq/id_constructors/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a4/geoseeq/knex.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a4/geoseeq/organization.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a4/geoseeq/pipeline.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.260133 geoseeq-0.5.6a4/geoseeq/plotting/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a4/geoseeq/plotting/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a4/geoseeq/plotting/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a4/geoseeq/plotting/highcharts.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.260852 geoseeq-0.5.6a4/geoseeq/plotting/map/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a4/geoseeq/plotting/map/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a4/geoseeq/plotting/map/base_layer.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a4/geoseeq/plotting/map/map.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a4/geoseeq/plotting/map/overlay.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a4/geoseeq/plotting/selectable.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a4/geoseeq/project.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6816 2024-03-19 00:06:20.000000 geoseeq-0.5.6a4/geoseeq/remote_object.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.262373 geoseeq-0.5.6a4/geoseeq/result/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a4/geoseeq/result/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a4/geoseeq/result/bioinfo.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4589 2024-03-06 22:35:53.000000 geoseeq-0.5.6a4/geoseeq/result/file_download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7390 2024-03-18 21:44:44.000000 geoseeq-0.5.6a4/geoseeq/result/file_upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a4/geoseeq/result/result_file.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a4/geoseeq/result/result_folder.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a4/geoseeq/result/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a4/geoseeq/sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a4/geoseeq/search.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7090 2024-03-19 13:53:30.000000 geoseeq-0.5.6a4/geoseeq/upload_download_manager.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a4/geoseeq/utils.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.263962 geoseeq-0.5.6a4/geoseeq/vc/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a4/geoseeq/vc/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a4/geoseeq/vc/checksum.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a4/geoseeq/vc/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/vc/clone.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/vc/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/vc/vc_cache.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a4/geoseeq/vc/vc_dir.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a4/geoseeq/vc/vc_sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a4/geoseeq/vc/vc_stub.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a4/geoseeq/work_orders.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.264621 geoseeq-0.5.6a4/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-01 16:15:48.000000 geoseeq-0.5.6a4/geoseeq.egg-info/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-01 16:15:48.000000 geoseeq-0.5.6a4/geoseeq.egg-info/SOURCES.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-01 16:15:48.000000 geoseeq-0.5.6a4/geoseeq.egg-info/dependency_links.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-01 16:15:48.000000 geoseeq-0.5.6a4/geoseeq.egg-info/entry_points.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-01 16:15:48.000000 geoseeq-0.5.6a4/geoseeq.egg-info/top_level.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-01 16:15:42.000000 geoseeq-0.5.6a4/pyproject.toml
+-rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-01 16:15:48.265241 geoseeq-0.5.6a4/setup.cfg
+-rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-04-01 15:48:45.000000 geoseeq-0.5.6a4/setup.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 16:15:48.264425 geoseeq-0.5.6a4/tests/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a4/tests/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a4/tests/test_api_client.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a4/tests/test_plotting.py
```

### Comparing `geoseeq-0.5.6a3/LICENSE` & `geoseeq-0.5.6a4/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/PKG-INFO` & `geoseeq-0.5.6a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a3
+Version: 0.5.6a4
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a3/README.md` & `geoseeq-0.5.6a4/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/__init__.py` & `geoseeq-0.5.6a4/geoseeq/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/app.py` & `geoseeq-0.5.6a4/geoseeq/app.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/bulk_creators.py` & `geoseeq-0.5.6a4/geoseeq/bulk_creators.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/copy.py` & `geoseeq-0.5.6a4/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/detail.py` & `geoseeq-0.5.6a4/geoseeq/cli/detail.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/download.py` & `geoseeq-0.5.6a4/geoseeq/cli/download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/fastq_utils.py` & `geoseeq-0.5.6a4/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/get_eula.py` & `geoseeq-0.5.6a4/geoseeq/cli/get_eula.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/main.py` & `geoseeq-0.5.6a4/geoseeq/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """Print the version of the Geoseeq API being used.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    click.echo('0.5.6a3')  # remember to update setup
+    click.echo('0.5.6a4')  # remember to update setup
 
 
 @main.group('advanced')
 def cli_advanced():
     """Advanced commands."""
     pass
 
@@ -85,15 +85,15 @@
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
     if not profile and not yes:
         profile = click.prompt(f'Set custom profile name? (Leave blank for default)', default="").strip(' \"\'')
-    if not endpoint:
+    if not endpoint and not yes:
         endpoint = click.prompt(f'Enter the URL to use for GeoSeeq (Most users can use the default)', default=DEFAULT_ENDPOINT).strip(' \"\'')
     if not api_token:
         api_token = click.prompt(f'Enter your GeoSeeq API token', hide_input=True).strip(' \"\'')
     if not yes:
         eula_accepted = click.confirm(f'Have you read and accepted the GeoSeeq End User License Agreement? Use `geoseeq eula show` to view the EULA.')
         if not eula_accepted:
             click.echo('You must accept the EULA to use the GeoSeeq API.')
```

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/manage.py` & `geoseeq-0.5.6a4/geoseeq/cli/manage.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/progress_bar.py` & `geoseeq-0.5.6a4/geoseeq/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/run.py` & `geoseeq-0.5.6a4/geoseeq/cli/run.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/search.py` & `geoseeq-0.5.6a4/geoseeq/cli/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/shared_params/common_state.py` & `geoseeq-0.5.6a4/geoseeq/cli/shared_params/common_state.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/shared_params/config.py` & `geoseeq-0.5.6a4/geoseeq/cli/shared_params/config.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/shared_params/id_handlers.py` & `geoseeq-0.5.6a4/geoseeq/cli/shared_params/id_handlers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/shared_params/obj_getters.py` & `geoseeq-0.5.6a4/geoseeq/cli/shared_params/obj_getters.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/shared_params/opts_and_args.py` & `geoseeq-0.5.6a4/geoseeq/cli/shared_params/opts_and_args.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/upload/__init__.py` & `geoseeq-0.5.6a4/geoseeq/cli/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/upload/upload.py` & `geoseeq-0.5.6a4/geoseeq/cli/upload/upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/upload/upload_advanced.py` & `geoseeq-0.5.6a4/geoseeq/cli/upload/upload_advanced.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/upload/upload_reads.py` & `geoseeq-0.5.6a4/geoseeq/cli/upload/upload_reads.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/user.py` & `geoseeq-0.5.6a4/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/utils.py` & `geoseeq-0.5.6a4/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/cli/view.py` & `geoseeq-0.5.6a4/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.5.6a4/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.5.6a4/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.5.6a4/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/file_system_cache.py` & `geoseeq-0.5.6a4/geoseeq/file_system_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/id_constructors/from_blobs.py` & `geoseeq-0.5.6a4/geoseeq/id_constructors/from_blobs.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/id_constructors/from_ids.py` & `geoseeq-0.5.6a4/geoseeq/id_constructors/from_ids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/id_constructors/from_names.py` & `geoseeq-0.5.6a4/geoseeq/id_constructors/from_names.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/id_constructors/from_uuids.py` & `geoseeq-0.5.6a4/geoseeq/id_constructors/from_uuids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/id_constructors/resolvers.py` & `geoseeq-0.5.6a4/geoseeq/id_constructors/resolvers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/id_constructors/utils.py` & `geoseeq-0.5.6a4/geoseeq/id_constructors/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/knex.py` & `geoseeq-0.5.6a4/geoseeq/knex.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/organization.py` & `geoseeq-0.5.6a4/geoseeq/organization.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/pipeline.py` & `geoseeq-0.5.6a4/geoseeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/plotting/highcharts.py` & `geoseeq-0.5.6a4/geoseeq/plotting/highcharts.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/plotting/map/base_layer.py` & `geoseeq-0.5.6a4/geoseeq/plotting/map/base_layer.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/plotting/map/map.py` & `geoseeq-0.5.6a4/geoseeq/plotting/map/map.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/plotting/map/overlay.py` & `geoseeq-0.5.6a4/geoseeq/plotting/map/overlay.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/plotting/selectable.py` & `geoseeq-0.5.6a4/geoseeq/plotting/selectable.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/project.py` & `geoseeq-0.5.6a4/geoseeq/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/remote_object.py` & `geoseeq-0.5.6a4/geoseeq/remote_object.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/result/bioinfo.py` & `geoseeq-0.5.6a4/geoseeq/result/bioinfo.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/result/file_download.py` & `geoseeq-0.5.6a4/geoseeq/result/file_download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/result/file_upload.py` & `geoseeq-0.5.6a4/geoseeq/result/file_upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/result/result_file.py` & `geoseeq-0.5.6a4/geoseeq/result/result_file.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/result/result_folder.py` & `geoseeq-0.5.6a4/geoseeq/result/result_folder.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/result/utils.py` & `geoseeq-0.5.6a4/geoseeq/result/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/sample.py` & `geoseeq-0.5.6a4/geoseeq/sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/search.py` & `geoseeq-0.5.6a4/geoseeq/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/upload_download_manager.py` & `geoseeq-0.5.6a4/geoseeq/upload_download_manager.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/user.py` & `geoseeq-0.5.6a4/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/utils.py` & `geoseeq-0.5.6a4/geoseeq/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/vc/checksum.py` & `geoseeq-0.5.6a4/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/vc/cli.py` & `geoseeq-0.5.6a4/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/vc/clone.py` & `geoseeq-0.5.6a4/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/vc/vc_cache.py` & `geoseeq-0.5.6a4/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/vc/vc_sample.py` & `geoseeq-0.5.6a4/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/vc/vc_stub.py` & `geoseeq-0.5.6a4/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq/work_orders.py` & `geoseeq-0.5.6a4/geoseeq/work_orders.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/geoseeq.egg-info/PKG-INFO` & `geoseeq-0.5.6a4/geoseeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a3
+Version: 0.5.6a4
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a3/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.5.6a4/geoseeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/pyproject.toml` & `geoseeq-0.5.6a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoseeq"
-version = "0.5.6a3"
+version = "0.5.6a4"
 authors = [
   { name="David C. Danko", email="dcdanko@biotia.io" },
 ]
 description = "GeoSeeq command line tools and python API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geoseeq-0.5.6a3/setup.py` & `geoseeq-0.5.6a4/setup.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/tests/test_api_client.py` & `geoseeq-0.5.6a4/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a3/tests/test_plotting.py` & `geoseeq-0.5.6a4/tests/test_plotting.py`

 * *Files identical despite different names*

