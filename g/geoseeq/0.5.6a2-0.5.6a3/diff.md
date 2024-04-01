# Comparing `tmp/geoseeq-0.5.6a2.tar.gz` & `tmp/geoseeq-0.5.6a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.5.6a2.tar", last modified: Tue Mar 19 14:43:37 2024, max compression
+gzip compressed data, was "geoseeq-0.5.6a3.tar", last modified: Mon Apr  1 15:54:39 2024, max compression
```

## Comparing `geoseeq-0.5.6a2.tar` & `geoseeq-0.5.6a3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.743690 geoseeq-0.5.6a2/
--rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a2/LICENSE
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-03-19 14:43:37.743441 geoseeq-0.5.6a2/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a2/README.md
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.730695 geoseeq-0.5.6a2/geoseeq/
--rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a2/geoseeq/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a2/geoseeq/app.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a2/geoseeq/blob_constructors.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a2/geoseeq/bulk_creators.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.733919 geoseeq-0.5.6a2/geoseeq/cli/
--rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/cli/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/cli/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/copy.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/detail.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a2/geoseeq/cli/download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a2/geoseeq/cli/fastq_utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/get_eula.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2910 2024-03-19 14:43:29.000000 geoseeq-0.5.6a2/geoseeq/cli/main.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/manage.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a2/geoseeq/cli/progress_bar.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/run.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/search.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.735024 geoseeq-0.5.6a2/geoseeq/cli/shared_params/
--rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a2/geoseeq/cli/shared_params/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3555 2024-03-06 20:26:27.000000 geoseeq-0.5.6a2/geoseeq/cli/shared_params/common_state.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a2/geoseeq/cli/shared_params/config.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a2/geoseeq/cli/shared_params/id_handlers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a2/geoseeq/cli/shared_params/obj_getters.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a2/geoseeq/cli/shared_params/opts_and_args.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.735697 geoseeq-0.5.6a2/geoseeq/cli/upload/
--rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a2/geoseeq/cli/upload/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8963 2024-03-18 23:39:08.000000 geoseeq-0.5.6a2/geoseeq/cli/upload/upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a2/geoseeq/cli/upload/upload_advanced.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7264 2024-03-19 00:09:27.000000 geoseeq-0.5.6a2/geoseeq/cli/upload/upload_reads.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a2/geoseeq/cli/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a2/geoseeq/cli/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a2/geoseeq/cli/view.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a2/geoseeq/constants.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.735879 geoseeq-0.5.6a2/geoseeq/contrib/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/contrib/__init__.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.736594 geoseeq-0.5.6a2/geoseeq/contrib/ncbi/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/contrib/ncbi/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a2/geoseeq/contrib/ncbi/api.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a2/geoseeq/contrib/ncbi/bioproject.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a2/geoseeq/contrib/ncbi/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/contrib/ncbi/setup_logging.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3405 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/file_system_cache.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.737702 geoseeq-0.5.6a2/geoseeq/id_constructors/
--rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5652 2024-03-19 03:24:22.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/from_blobs.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3050 2024-02-26 20:06:48.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/from_ids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/from_names.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/from_uuids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/resolvers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a2/geoseeq/id_constructors/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a2/geoseeq/knex.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a2/geoseeq/organization.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a2/geoseeq/pipeline.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.738328 geoseeq-0.5.6a2/geoseeq/plotting/
--rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a2/geoseeq/plotting/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a2/geoseeq/plotting/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a2/geoseeq/plotting/highcharts.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.738983 geoseeq-0.5.6a2/geoseeq/plotting/map/
--rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a2/geoseeq/plotting/map/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a2/geoseeq/plotting/map/base_layer.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a2/geoseeq/plotting/map/map.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a2/geoseeq/plotting/map/overlay.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a2/geoseeq/plotting/selectable.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a2/geoseeq/project.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6816 2024-03-19 00:06:20.000000 geoseeq-0.5.6a2/geoseeq/remote_object.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.740987 geoseeq-0.5.6a2/geoseeq/result/
--rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a2/geoseeq/result/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a2/geoseeq/result/bioinfo.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4589 2024-03-06 22:35:53.000000 geoseeq-0.5.6a2/geoseeq/result/file_download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7390 2024-03-18 21:44:44.000000 geoseeq-0.5.6a2/geoseeq/result/file_upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a2/geoseeq/result/result_file.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a2/geoseeq/result/result_folder.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a2/geoseeq/result/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a2/geoseeq/sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a2/geoseeq/search.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7090 2024-03-19 13:53:30.000000 geoseeq-0.5.6a2/geoseeq/upload_download_manager.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a2/geoseeq/utils.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.742398 geoseeq-0.5.6a2/geoseeq/vc/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a2/geoseeq/vc/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a2/geoseeq/vc/checksum.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a2/geoseeq/vc/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/vc/clone.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/vc/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/vc/vc_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a2/geoseeq/vc/vc_dir.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a2/geoseeq/vc/vc_sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a2/geoseeq/vc/vc_stub.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a2/geoseeq/work_orders.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.743140 geoseeq-0.5.6a2/geoseeq.egg-info/
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-03-19 14:43:37.000000 geoseeq-0.5.6a2/geoseeq.egg-info/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-03-19 14:43:37.000000 geoseeq-0.5.6a2/geoseeq.egg-info/SOURCES.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-03-19 14:43:37.000000 geoseeq-0.5.6a2/geoseeq.egg-info/dependency_links.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-03-19 14:43:37.000000 geoseeq-0.5.6a2/geoseeq.egg-info/entry_points.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-03-19 14:43:37.000000 geoseeq-0.5.6a2/geoseeq.egg-info/top_level.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-03-19 14:43:23.000000 geoseeq-0.5.6a2/pyproject.toml
--rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-03-19 14:43:37.743752 geoseeq-0.5.6a2/setup.cfg
--rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-03-19 14:09:17.000000 geoseeq-0.5.6a2/setup.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-03-19 14:43:37.742890 geoseeq-0.5.6a2/tests/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a2/tests/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a2/tests/test_api_client.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a2/tests/test_plotting.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.788587 geoseeq-0.5.6a3/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a3/LICENSE
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-01 15:54:39.788297 geoseeq-0.5.6a3/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a3/README.md
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.759268 geoseeq-0.5.6a3/geoseeq/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a3/geoseeq/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a3/geoseeq/app.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a3/geoseeq/blob_constructors.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a3/geoseeq/bulk_creators.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.768121 geoseeq-0.5.6a3/geoseeq/cli/
+-rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/cli/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/cli/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/copy.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/detail.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a3/geoseeq/cli/download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a3/geoseeq/cli/fastq_utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/get_eula.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3199 2024-04-01 15:48:20.000000 geoseeq-0.5.6a3/geoseeq/cli/main.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/manage.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a3/geoseeq/cli/progress_bar.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/run.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/search.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.770275 geoseeq-0.5.6a3/geoseeq/cli/shared_params/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/common_state.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/config.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/id_handlers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/obj_getters.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a3/geoseeq/cli/shared_params/opts_and_args.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.771592 geoseeq-0.5.6a3/geoseeq/cli/upload/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8963 2024-03-18 23:39:08.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/upload_advanced.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7264 2024-03-19 00:09:27.000000 geoseeq-0.5.6a3/geoseeq/cli/upload/upload_reads.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a3/geoseeq/cli/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a3/geoseeq/cli/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a3/geoseeq/cli/view.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a3/geoseeq/constants.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.771983 geoseeq-0.5.6a3/geoseeq/contrib/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/contrib/__init__.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.773336 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/api.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/bioproject.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/contrib/ncbi/setup_logging.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4101 2024-03-21 02:53:18.000000 geoseeq-0.5.6a3/geoseeq/file_system_cache.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.775758 geoseeq-0.5.6a3/geoseeq/id_constructors/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_blobs.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_ids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_names.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/from_uuids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/resolvers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a3/geoseeq/id_constructors/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a3/geoseeq/knex.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a3/geoseeq/organization.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a3/geoseeq/pipeline.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.777161 geoseeq-0.5.6a3/geoseeq/plotting/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a3/geoseeq/plotting/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a3/geoseeq/plotting/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a3/geoseeq/plotting/highcharts.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.778512 geoseeq-0.5.6a3/geoseeq/plotting/map/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/base_layer.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/map.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a3/geoseeq/plotting/map/overlay.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a3/geoseeq/plotting/selectable.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a3/geoseeq/project.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6816 2024-03-19 00:06:20.000000 geoseeq-0.5.6a3/geoseeq/remote_object.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.781800 geoseeq-0.5.6a3/geoseeq/result/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a3/geoseeq/result/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a3/geoseeq/result/bioinfo.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4589 2024-03-06 22:35:53.000000 geoseeq-0.5.6a3/geoseeq/result/file_download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7390 2024-03-18 21:44:44.000000 geoseeq-0.5.6a3/geoseeq/result/file_upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a3/geoseeq/result/result_file.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a3/geoseeq/result/result_folder.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a3/geoseeq/result/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a3/geoseeq/sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a3/geoseeq/search.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7090 2024-03-19 13:53:30.000000 geoseeq-0.5.6a3/geoseeq/upload_download_manager.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a3/geoseeq/utils.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.785713 geoseeq-0.5.6a3/geoseeq/vc/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a3/geoseeq/vc/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a3/geoseeq/vc/checksum.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a3/geoseeq/vc/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/clone.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_cache.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_dir.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a3/geoseeq/vc/vc_stub.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a3/geoseeq/work_orders.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.787799 geoseeq-0.5.6a3/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/SOURCES.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/dependency_links.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/entry_points.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-01 15:54:39.000000 geoseeq-0.5.6a3/geoseeq.egg-info/top_level.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-01 15:48:31.000000 geoseeq-0.5.6a3/pyproject.toml
+-rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-01 15:54:39.788649 geoseeq-0.5.6a3/setup.cfg
+-rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-04-01 15:48:45.000000 geoseeq-0.5.6a3/setup.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-01 15:54:39.787349 geoseeq-0.5.6a3/tests/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a3/tests/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a3/tests/test_api_client.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a3/tests/test_plotting.py
```

### Comparing `geoseeq-0.5.6a2/LICENSE` & `geoseeq-0.5.6a3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/PKG-INFO` & `geoseeq-0.5.6a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a2
+Version: 0.5.6a3
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a2/README.md` & `geoseeq-0.5.6a3/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/__init__.py` & `geoseeq-0.5.6a3/geoseeq/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/app.py` & `geoseeq-0.5.6a3/geoseeq/app.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/bulk_creators.py` & `geoseeq-0.5.6a3/geoseeq/bulk_creators.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/copy.py` & `geoseeq-0.5.6a3/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/detail.py` & `geoseeq-0.5.6a3/geoseeq/cli/detail.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/download.py` & `geoseeq-0.5.6a3/geoseeq/cli/download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/fastq_utils.py` & `geoseeq-0.5.6a3/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/get_eula.py` & `geoseeq-0.5.6a3/geoseeq/cli/get_eula.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/main.py` & `geoseeq-0.5.6a3/geoseeq/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .upload import cli_upload, cli_upload_advanced
 from .user import cli_user
 from .view import cli_view
 from .search import cli_search
 from geoseeq.vc.cli import cli_vc
 from geoseeq.knex import DEFAULT_ENDPOINT
 from geoseeq.utils import set_profile
-from .shared_params.opts_and_args import overwrite_option
+from .shared_params.opts_and_args import overwrite_option, yes_option
 from .detail import cli_detail
 from .run import cli_app
 from .get_eula import cli_eula
 
 logger = logging.getLogger('geoseeq_api')
 handler = logging.StreamHandler()
 handler.setFormatter(logging.Formatter('[%(levelname)s] %(name)s :: %(message)s'))
@@ -49,15 +49,15 @@
     """Print the version of the Geoseeq API being used.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    click.echo('0.5.6a2')  # remember to update setup
+    click.echo('0.5.6a3')  # remember to update setup
 
 
 @main.group('advanced')
 def cli_advanced():
     """Advanced commands."""
     pass
 
@@ -70,27 +70,33 @@
 def cli_experimental():
     """Experimental commands."""
     pass
 
 cli_experimental.add_command(cli_vc)
 
 @main.command('config')
+@yes_option
+@click.option('--api-token', default=None, help='The API token to use.')
+@click.option('--endpoint', default=None, help='The endpoint to use.')
 @click.option('-p', '--profile', default=None, help='The profile name to use.')
 @overwrite_option
-def cli_config(profile, overwrite):
+def cli_config(yes, api_token, endpoint, profile, overwrite):
     """Configure the GeoSeeq API.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    if not profile:
+    if not profile and not yes:
         profile = click.prompt(f'Set custom profile name? (Leave blank for default)', default="").strip(' \"\'')
-    endpoint = click.prompt(f'Enter the URL to use for GeoSeeq (Most users can use the default)', default=DEFAULT_ENDPOINT).strip(' \"\'')
-    api_token = click.prompt(f'Enter your GeoSeeq API token', hide_input=True).strip(' \"\'')
-    eula_accepted = click.confirm(f'Have you read and accepted the GeoSeeq End User License Agreement? Use `geoseeq eula show` to view the EULA.')
-    if not eula_accepted:
-        click.echo('You must accept the EULA to use the GeoSeeq API.')
-        return
+    if not endpoint:
+        endpoint = click.prompt(f'Enter the URL to use for GeoSeeq (Most users can use the default)', default=DEFAULT_ENDPOINT).strip(' \"\'')
+    if not api_token:
+        api_token = click.prompt(f'Enter your GeoSeeq API token', hide_input=True).strip(' \"\'')
+    if not yes:
+        eula_accepted = click.confirm(f'Have you read and accepted the GeoSeeq End User License Agreement? Use `geoseeq eula show` to view the EULA.')
+        if not eula_accepted:
+            click.echo('You must accept the EULA to use the GeoSeeq API.')
+            return
     set_profile(api_token, endpoint=endpoint, profile=profile, overwrite=overwrite)
     click.echo(f'Profile configured.')
```

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/manage.py` & `geoseeq-0.5.6a3/geoseeq/cli/manage.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/progress_bar.py` & `geoseeq-0.5.6a3/geoseeq/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/run.py` & `geoseeq-0.5.6a3/geoseeq/cli/run.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/search.py` & `geoseeq-0.5.6a3/geoseeq/cli/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/shared_params/common_state.py` & `geoseeq-0.5.6a3/geoseeq/cli/shared_params/common_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 
 import click
 from geoseeq.knex import DEFAULT_ENDPOINT
-
+import geoseeq.file_system_cache
 from geoseeq import Knex
 from geoseeq.utils import load_auth_profile
 
 logger = logging.getLogger('geoseeq_api')
 
 
 class State(object):
 
     def __init__(self):
         self.api_token = None
         self.endpoint = DEFAULT_ENDPOINT
         self.outfile = None
         self.log_level = 20
         self._knex = None
+        self.use_cache = True
 
     def get_knex(self):
         logger.setLevel(self.log_level)
         self._knex = Knex(self.endpoint)
         if self.api_token:
             self._knex.add_api_token(self.api_token)
         return self._knex
@@ -33,16 +34,16 @@
 
 def log_level_option(f):
     def callback(ctx, param, value):
         state = ctx.ensure_object(State)
         state.log_level = value
         return value
     return click.option('-l', '--log-level',
-                        type=click.Choice(['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG']),
-                        default='WARNING',
+                        type=click.Choice(['CRITICAL', 'ERROR', 'WARN', 'INFO', 'DEBUG']),
+                        default='WARN',
                         envvar='GEOSEEQ_CLI_LOG_LEVEL',
                         expose_value=False,
                         callback=callback)(f)
 
 
 def api_token_option(f):
     def callback(ctx, param, value):
@@ -99,19 +100,33 @@
     return click.option('-o', '--outfile',
                         default='-', type=click.File('w'),
                         expose_value=False,
                         help='Output file path',
                         callback=callback)(f)
 
 
+def cache_option(f):
+    def callback(ctx, param, value):
+        state = ctx.ensure_object(State)
+        state.use_cache = value
+        geoseeq.file_system_cache.USE_GEOSEEQ_CACHE = value
+        return value
+    return click.option('--use-cache/--no-cache',
+                        default=True,
+                        expose_value=False,
+                        help='Cache data from the geoseeq server.',
+                        callback=callback)(f)
+
+
 def common_options(f):
     f = outfile_option(f)
     f = log_level_option(f)
     f = endpoint_option(f)
     f = profile_option(f)
+    f = cache_option(f)
     return f
 
 
 def use_common_state(f):
     f = common_options(f)
     f = pass_state(f)
     return f
```

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/shared_params/config.py` & `geoseeq-0.5.6a3/geoseeq/cli/shared_params/config.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/shared_params/id_handlers.py` & `geoseeq-0.5.6a3/geoseeq/cli/shared_params/id_handlers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/shared_params/obj_getters.py` & `geoseeq-0.5.6a3/geoseeq/cli/shared_params/obj_getters.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/shared_params/opts_and_args.py` & `geoseeq-0.5.6a3/geoseeq/cli/shared_params/opts_and_args.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/upload/__init__.py` & `geoseeq-0.5.6a3/geoseeq/cli/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/upload/upload.py` & `geoseeq-0.5.6a3/geoseeq/cli/upload/upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/upload/upload_advanced.py` & `geoseeq-0.5.6a3/geoseeq/cli/upload/upload_advanced.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/upload/upload_reads.py` & `geoseeq-0.5.6a3/geoseeq/cli/upload/upload_reads.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/user.py` & `geoseeq-0.5.6a3/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/utils.py` & `geoseeq-0.5.6a3/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/cli/view.py` & `geoseeq-0.5.6a3/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.5.6a3/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.5.6a3/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.5.6a3/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/file_system_cache.py` & `geoseeq-0.5.6a3/geoseeq/file_system_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import json
 import logging
 import os
+from os.path import join, abspath
 from glob import glob
 from hashlib import sha256
 from random import randint
 from time import time
 
-logger = logging.getLogger(__name__)  # Same name as calling module
+logger = logging.getLogger("geoseeq_api")  # Same name as calling module
 logger.addHandler(logging.NullHandler())  # No output unless configured by calling program
-CACHED_BLOB_TIME = 3 * 60 * 60  # 3 hours in seconds
-CACHE_DIR = os.environ.get('GEOSEEQ_API_CACHE_DIR', '.')
+CACHED_BLOB_TIME = 5 * 60 # 5 minutes in seconds
+CACHE_DIR = join(
+    os.environ.get('XDG_CACHE_HOME', join(os.environ["HOME"], ".cache")),
+    "geoseeq"
+)
+USE_GEOSEEQ_CACHE = None
 
 
 def hash_obj(obj):
     val = obj
     if not isinstance(obj, str):
         val = obj.pre_hash()
     result = sha256(val.encode())
@@ -26,32 +31,54 @@
     elapsed_time = int(time()) - timestamp
     return elapsed_time
 
 
 class FileSystemCache:
 
     def __init__(self, timeout=CACHED_BLOB_TIME):
-        self.no_cache = 'false' in os.environ.get('USE_GEOSEEQ_CACHE', 'TRUE').lower()
         self.timeout = timeout
+        self._no_cache = False
+        self.setup()
+
+    @property
+    def cache_dir_path(self):
+        return abspath(f'{CACHE_DIR}/geoseeq_api_cache/v1/')
+
+    def setup(self):
+        if self.no_cache:
+            return
+        try:
+            os.makedirs(self.cache_dir_path, exist_ok=True)
+            open(join(self.cache_dir_path, 'flag'), 'w').close()
+        except Exception as e:
+            logger.warning(f'Could not create cache directory. {e}')
+            self._no_cache = True
+    
+    @property
+    def no_cache(self):
+        if self._no_cache or not USE_GEOSEEQ_CACHE:
+            logger.debug('Cache is disabled.')
+            return True
+        logger.debug('Cache is enabled.')
+        return not USE_GEOSEEQ_CACHE
 
     def clear_blob(self, obj):
         if self.no_cache:
             return
         blob_filepath, path_exists = self.get_cached_blob_filepath(obj)
         if path_exists:
             logger.debug(f'Clearing cached blob. {blob_filepath}')
             try:
                 os.remove(blob_filepath)
             except FileNotFoundError:
                 logger.debug(f'Blob was deleted before it could be removed. {obj}')
                 pass
 
     def get_cached_blob_filepath(self, obj):
-        path_base = f'{CACHE_DIR}/.geoseeq_api_cache/v1/geoseeq_api_cache__{hash_obj(obj)}'
-        os.makedirs(os.path.dirname(path_base), exist_ok=True)
+        path_base = join(self.cache_dir_path, f'geoseeq_api_cache__{hash_obj(obj)}')
         paths = sorted(glob(f'{path_base}__*.json'))
         if paths:
             return paths[-1], True
         timestamp = int(time())
         blob_filepath = f'{path_base}__{timestamp}.json'
         return blob_filepath, False
```

### Comparing `geoseeq-0.5.6a2/geoseeq/id_constructors/from_blobs.py` & `geoseeq-0.5.6a3/geoseeq/id_constructors/from_blobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         knex, blob["analysis_result_obj"], already_fetched=already_fetched, modified=modified
     )
     from geoseeq.result import SampleResultFile  # import here to avoid circular import
     arf = SampleResultFile(knex, ar, blob["name"], data=blob["stored_data"])
     arf.load_blob(blob)
     ar._already_fetched = already_fetched
     ar._modified = modified
+    arf.cache_blob(blob)
     return arf
 
 
 sample_ar_field_from_blob = sample_result_file_from_blob  # Alias
 
 
 @with_knex
@@ -106,14 +107,15 @@
         knex, blob["analysis_result_obj"], already_fetched=already_fetched, modified=modified
     )
     from geoseeq.result import ProjectResultFile  # import here to avoid circular import
     arf = ProjectResultFile(knex, ar, blob["name"], data=blob["stored_data"])
     arf.load_blob(blob)
     ar._already_fetched = already_fetched
     ar._modified = modified
+    arf.cache_blob(blob)
     return arf
 
 
 sample_group_ar_field_from_blob = project_result_file_from_blob  # Alias
 
 
 @with_knex
```

### Comparing `geoseeq-0.5.6a2/geoseeq/id_constructors/from_ids.py` & `geoseeq-0.5.6a3/geoseeq/id_constructors/from_ids.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .utils import is_grn_or_uuid, is_name
 from geoseeq.knex import with_knex
 
 
 def _generic_from_id(knex, id, from_uuid_func, from_name_func):
     """Return the object which the id points to."""
     if is_grn_or_uuid(id):
+        id = id.split(':')[-1]  # if this is a GRN, get the UUID. Won't hurt if it's already a UUID.
         return from_uuid_func(knex, id)
     if is_name(id):
         return from_name_func(knex, id)
     raise ValueError(f'"{id}" is not a GRN, UUID, or name')
 
 
 @with_knex
```

### Comparing `geoseeq-0.5.6a2/geoseeq/id_constructors/from_names.py` & `geoseeq-0.5.6a3/geoseeq/id_constructors/from_names.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/id_constructors/from_uuids.py` & `geoseeq-0.5.6a3/geoseeq/id_constructors/from_uuids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/id_constructors/resolvers.py` & `geoseeq-0.5.6a3/geoseeq/id_constructors/resolvers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/id_constructors/utils.py` & `geoseeq-0.5.6a3/geoseeq/id_constructors/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/knex.py` & `geoseeq-0.5.6a3/geoseeq/knex.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/organization.py` & `geoseeq-0.5.6a3/geoseeq/organization.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/pipeline.py` & `geoseeq-0.5.6a3/geoseeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/plotting/highcharts.py` & `geoseeq-0.5.6a3/geoseeq/plotting/highcharts.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/plotting/map/base_layer.py` & `geoseeq-0.5.6a3/geoseeq/plotting/map/base_layer.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/plotting/map/map.py` & `geoseeq-0.5.6a3/geoseeq/plotting/map/map.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/plotting/map/overlay.py` & `geoseeq-0.5.6a3/geoseeq/plotting/map/overlay.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/plotting/selectable.py` & `geoseeq-0.5.6a3/geoseeq/plotting/selectable.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/project.py` & `geoseeq-0.5.6a3/geoseeq/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/remote_object.py` & `geoseeq-0.5.6a3/geoseeq/remote_object.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/result/bioinfo.py` & `geoseeq-0.5.6a3/geoseeq/result/bioinfo.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/result/file_download.py` & `geoseeq-0.5.6a3/geoseeq/result/file_download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/result/file_upload.py` & `geoseeq-0.5.6a3/geoseeq/result/file_upload.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/result/result_file.py` & `geoseeq-0.5.6a3/geoseeq/result/result_file.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/result/result_folder.py` & `geoseeq-0.5.6a3/geoseeq/result/result_folder.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/result/utils.py` & `geoseeq-0.5.6a3/geoseeq/result/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/sample.py` & `geoseeq-0.5.6a3/geoseeq/sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/search.py` & `geoseeq-0.5.6a3/geoseeq/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/upload_download_manager.py` & `geoseeq-0.5.6a3/geoseeq/upload_download_manager.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/user.py` & `geoseeq-0.5.6a3/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/utils.py` & `geoseeq-0.5.6a3/geoseeq/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/vc/checksum.py` & `geoseeq-0.5.6a3/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/vc/cli.py` & `geoseeq-0.5.6a3/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/vc/clone.py` & `geoseeq-0.5.6a3/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/vc/vc_cache.py` & `geoseeq-0.5.6a3/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/vc/vc_sample.py` & `geoseeq-0.5.6a3/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/vc/vc_stub.py` & `geoseeq-0.5.6a3/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq/work_orders.py` & `geoseeq-0.5.6a3/geoseeq/work_orders.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/geoseeq.egg-info/PKG-INFO` & `geoseeq-0.5.6a3/geoseeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a2
+Version: 0.5.6a3
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a2/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.5.6a3/geoseeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/pyproject.toml` & `geoseeq-0.5.6a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoseeq"
-version = "0.5.6a2"
+version = "0.5.6a3"
 authors = [
   { name="David C. Danko", email="dcdanko@biotia.io" },
 ]
 description = "GeoSeeq command line tools and python API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geoseeq-0.5.6a2/setup.py` & `geoseeq-0.5.6a3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import setuptools
 
 setuptools.setup(
     name='geoseeq',
-    version='0.5.6a1',  # remember to update version string in CLI as well
+    version='0.5.6a3',  # remember to update version string in CLI as well
     author="David C. Danko",
     author_email='dcdanko@biotia.io',
     description=open('README.md').read(),
     packages=setuptools.find_packages(),
     package_dir={'geoseeq': 'geoseeq'},
     install_requires=[
         'requests',
```

### Comparing `geoseeq-0.5.6a2/tests/test_api_client.py` & `geoseeq-0.5.6a3/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a2/tests/test_plotting.py` & `geoseeq-0.5.6a3/tests/test_plotting.py`

 * *Files identical despite different names*

