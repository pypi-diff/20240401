# Comparing `tmp/damo-2.2.7.tar.gz` & `tmp/damo-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.2.7.tar", last modified: Mon Mar 25 23:03:06 2024, max compression
+gzip compressed data, was "damo-2.2.8.tar", last modified: Mon Apr  1 21:19:31 2024, max compression
```

## Comparing `damo-2.2.7.tar` & `damo-2.2.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-03-25 23:03:06.229832 damo-2.2.7/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-03-25 23:03:06.229832 damo-2.2.7/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-03-25 23:03:02.000000 damo-2.2.7/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.2.7/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-03-25 23:03:06.229832 damo-2.2.7/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.2.7/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-03-25 23:03:06.213832 damo-2.2.7/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-03-25 23:03:06.225832 damo-2.2.7/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-03-25 23:03:02.000000 damo-2.2.7/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.2.7/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.2.7/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.2.7/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.2.7/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.2.7/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2350 2024-03-17 18:57:51.000000 damo-2.2.7/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.2.7/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.2.7/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.2.7/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    46939 2024-03-17 17:23:48.000000 damo-2.2.7/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    21260 2024-03-09 20:09:49.000000 damo-2.2.7/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.2.7/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    36716 2024-03-03 19:31:14.000000 damo-2.2.7/src/damo/_damon_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.2.7/src/damo/_damon_sysfs.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-02-18 16:32:32.000000 damo-2.2.7/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1865 2024-02-17 20:38:17.000000 damo-2.2.7/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1099 2024-02-17 20:38:29.000000 damo-2.2.7/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.2.7/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.2.7/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12167 2024-01-28 17:56:07.000000 damo-2.2.7/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.2.7/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.2.7/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2580 2024-01-28 17:57:01.000000 damo-2.2.7/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.2.7/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6459 2024-02-25 19:12:52.000000 damo-2.2.7/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3868 2024-02-18 16:55:50.000000 damo-2.2.7/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4280 2024-02-25 19:26:23.000000 damo-2.2.7/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1425 2024-03-02 20:08:09.000000 damo-2.2.7/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1676 2024-03-03 18:44:22.000000 damo-2.2.7/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3888 2024-01-28 17:58:41.000000 damo-2.2.7/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1497 2024-03-03 18:44:22.000000 damo-2.2.7/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.2.7/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26321 2024-03-24 18:19:45.000000 damo-2.2.7/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.2.7/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.2.7/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.2.7/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-02-17 20:35:23.000000 damo-2.2.7/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3765 2024-02-17 20:38:04.000000 damo-2.2.7/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-03-25 23:01:19.000000 damo-2.2.7/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5440 2024-01-28 18:00:29.000000 damo-2.2.7/src/damo/damo_wss.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      463 2024-02-18 18:54:40.000000 damo-2.2.7/src/damo/python_access_perf.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-03-25 23:03:06.229832 damo-2.2.7/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-03-25 23:03:06.000000 damo-2.2.7/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1275 2024-03-25 23:03:06.000000 damo-2.2.7/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-03-25 23:03:06.000000 damo-2.2.7/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-03-25 23:03:06.000000 damo-2.2.7/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-03-25 23:03:06.000000 damo-2.2.7/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.140222 damo-2.2.8/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-01 21:19:31.140222 damo-2.2.8/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-01 21:19:27.000000 damo-2.2.8/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.2.8/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-01 21:19:31.140222 damo-2.2.8/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.2.8/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.124222 damo-2.2.8/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.136222 damo-2.2.8/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:27.000000 damo-2.2.8/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.2.8/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.2.8/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.2.8/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.2.8/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.2.8/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2350 2024-03-17 18:57:51.000000 damo-2.2.8/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.2.8/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.2.8/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.2.8/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    46939 2024-03-17 17:23:48.000000 damo-2.2.8/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    21260 2024-03-09 20:09:49.000000 damo-2.2.8/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.2.8/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    36716 2024-03-30 18:14:07.000000 damo-2.2.8/src/damo/_damon_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.2.8/src/damo/_damon_sysfs.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-02-18 16:32:32.000000 damo-2.2.8/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1865 2024-02-17 20:38:17.000000 damo-2.2.8/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1099 2024-02-17 20:38:29.000000 damo-2.2.8/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.2.8/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.2.8/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12167 2024-01-28 17:56:07.000000 damo-2.2.8/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.2.8/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.2.8/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2580 2024-01-28 17:57:01.000000 damo-2.2.8/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.2.8/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10047 2024-03-31 18:01:53.000000 damo-2.2.8/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3868 2024-02-18 16:55:50.000000 damo-2.2.8/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4280 2024-02-25 19:26:23.000000 damo-2.2.8/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1425 2024-03-02 20:08:09.000000 damo-2.2.8/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1676 2024-03-03 18:44:22.000000 damo-2.2.8/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3888 2024-01-28 17:58:41.000000 damo-2.2.8/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1497 2024-03-03 18:44:22.000000 damo-2.2.8/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.2.8/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26321 2024-03-24 18:19:45.000000 damo-2.2.8/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.2.8/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.2.8/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.2.8/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-02-17 20:35:23.000000 damo-2.2.8/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3765 2024-02-17 20:38:04.000000 damo-2.2.8/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-01 21:18:18.000000 damo-2.2.8/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5440 2024-01-28 18:00:29.000000 damo-2.2.8/src/damo/damo_wss.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      463 2024-02-18 18:54:40.000000 damo-2.2.8/src/damo/python_access_perf.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.140222 damo-2.2.8/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1275 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.2.7/PKG-INFO` & `damo-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.2.7
+Version: 2.2.8
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.7/README.md` & `damo-2.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,29 +75,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.7/setup.py` & `damo-2.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_ascii_color.py` & `damo-2.2.8/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_deprecated.py` & `damo-2.2.8/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_deprecation_notice.py` & `damo-2.2.8/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_dist.py` & `damo-2.2.8/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_fmt_str.py` & `damo-2.2.8/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_fs.py` & `damo-2.2.8/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_paddr_layout.py` & `damo-2.2.8/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_print.py` & `damo-2.2.8/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damo_subcmds.py` & `damo-2.2.8/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damon.py` & `damo-2.2.8/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damon_args.py` & `damo-2.2.8/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damon_dbgfs.py` & `damo-2.2.8/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damon_records.py` & `damo-2.2.8/src/damo/_damon_records.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/_damon_sysfs.py` & `damo-2.2.8/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo.py` & `damo-2.2.8/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_adjust.py` & `damo-2.2.8/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_convert_record_format.py` & `damo-2.2.8/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_features.py` & `damo-2.2.8/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_fmt_json.py` & `damo-2.2.8/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_heats.py` & `damo-2.2.8/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_lru_sort.py` & `damo-2.2.8/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_monitor.py` & `damo-2.2.8/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_nr_regions.py` & `damo-2.2.8/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_reclaim.py` & `damo-2.2.8/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_record_info.py` & `damo-2.2.8/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_replay.py` & `damo-2.2.8/src/damo/damo_replay.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_report.py` & `damo-2.2.8/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_report_profile.py` & `damo-2.2.8/src/damo/damo_report_profile.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_report_raw.py` & `damo-2.2.8/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_report_times.py` & `damo-2.2.8/src/damo/damo_report_times.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_schemes.py` & `damo-2.2.8/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_show.py` & `damo-2.2.8/src/damo/damo_show.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_start.py` & `damo-2.2.8/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_status.py` & `damo-2.2.8/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_stop.py` & `damo-2.2.8/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_tune.py` & `damo-2.2.8/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_validate.py` & `damo-2.2.8/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo/damo_wss.py` & `damo-2.2.8/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.7/src/damo.egg-info/PKG-INFO` & `damo-2.2.8/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.2.7
+Version: 2.2.8
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.7/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.7/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.7/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.7/src/damo.egg-info/SOURCES.txt` & `damo-2.2.8/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

