# Comparing `tmp/spice_rack-0.2.0.tar.gz` & `tmp/spice_rack-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_rack-0.2.0.tar", max compression
+gzip compressed data, was "spice_rack-0.3.0.tar", max compression
```

## Comparing `spice_rack-0.2.0.tar` & `spice_rack-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,92 @@
--rw-r--r--   0        0        0      176 2024-03-18 20:11:42.902072 spice_rack-0.2.0/README.md
--rw-r--r--   0        0        0     2486 2024-03-18 20:12:02.282235 spice_rack-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      191 2024-03-18 20:11:42.906072 spice_rack-0.2.0/src/spice_rack/__init__.py
--rw-r--r--   0        0        0      243 2024-03-18 20:11:42.906072 spice_rack-0.2.0/src/spice_rack/_bases/__init__.py
--rw-r--r--   0        0        0     4559 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_base_base.py
--rw-r--r--   0        0        0    11658 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_dispatchable.py
--rw-r--r--   0        0        0      239 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_exception/__init__.py
--rw-r--r--   0        0        0     1489 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_exception/_error_info.py
--rw-r--r--   0        0        0     5340 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_exception/_exception_base.py
--rw-r--r--   0        0        0      778 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_exception/_exception_exception.py
--rw-r--r--   0        0        0     1145 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_exception/_external_wrapper.py
--rw-r--r--   0        0        0      105 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_mixins/__init__.py
--rw-r--r--   0        0        0      332 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_mixins/_guid_mixin.py
--rw-r--r--   0        0        0     1570 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_mixins/_timestamped.py
--rw-r--r--   0        0        0      108 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_settings/__init__.py
--rw-r--r--   0        0        0     2757 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_settings/_base.py
--rw-r--r--   0        0        0      126 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_settings/_sources/__init__.py
--rw-r--r--   0        0        0      403 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_settings/_sources/_base.py
--rw-r--r--   0        0        0     2062 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py
--rw-r--r--   0        0        0     2829 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_special_str.py
--rw-r--r--   0        0        0      452 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_bases/_value_model.py
--rw-r--r--   0        0        0      218 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/__init__.py
--rw-r--r--   0        0        0     3138 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_exceptions.py
--rw-r--r--   0        0        0     3377 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_info.py
--rw-r--r--   0        0        0      351 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/__init__.py
--rw-r--r--   0        0        0    13051 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_base.py
--rw-r--r--   0        0        0     3299 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py
--rw-r--r--   0        0        0      752 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_local.py
--rw-r--r--   0        0        0     6273 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py
--rw-r--r--   0        0        0    13980 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_fs_models.py
--rw-r--r--   0        0        0     1022 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_helpers.py
--rw-r--r--   0        0        0      358 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_open_modes.py
--rw-r--r--   0        0        0      909 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/__init__.py
--rw-r--r--   0        0        0     4619 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_abs.py
--rw-r--r--   0        0        0     1775 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_base.py
--rw-r--r--   0        0        0     1227 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py
--rw-r--r--   0        0        0     4437 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_rel.py
--rw-r--r--   0        0        0      120 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/__init__.py
--rw-r--r--   0        0        0      939 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/_any_auth_strat.py
--rw-r--r--   0        0        0      243 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/__init__.py
--rw-r--r--   0        0        0      403 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_anon.py
--rw-r--r--   0        0        0      736 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py
--rw-r--r--   0        0        0     2088 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py
--rw-r--r--   0        0        0     2045 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py
--rw-r--r--   0        0        0      260 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/__init__.py
--rw-r--r--   0        0        0      113 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_log_aug/__init__.py
--rw-r--r--   0        0        0     2509 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_log_aug/_container.py
--rw-r--r--   0        0        0     1015 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py
--rw-r--r--   0        0        0     2362 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_log_level.py
--rw-r--r--   0        0        0     6258 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_logger.py
--rw-r--r--   0        0        0      421 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_logger_getter.py
--rw-r--r--   0        0        0     3342 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_setup.py
--rw-r--r--   0        0        0      140 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_sinks/__init__.py
--rw-r--r--   0        0        0     3843 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_sinks/_base.py
--rw-r--r--   0        0        0     1200 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_sinks/_file.py
--rw-r--r--   0        0        0      967 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_logging/_sinks/_sys.py
--rw-r--r--   0        0        0       53 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_misc/__init__.py
--rw-r--r--   0        0        0      603 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_misc/_empty.py
--rw-r--r--   0        0        0      135 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_timestamp/__init__.py
--rw-r--r--   0        0        0      622 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_timestamp/_fields.py
--rw-r--r--   0        0        0     6070 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_timestamp/_timestamp.py
--rw-r--r--   0        0        0     2639 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_timestamp/_tz_key.py
--rw-r--r--   0        0        0       50 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_utils/__init__.py
--rw-r--r--   0        0        0     1131 2024-03-18 20:11:42.910072 spice_rack-0.2.0/src/spice_rack/_utils/_container_differ.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 spice_rack-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-04-01 20:44:12.351219 spice_rack-0.3.0/README.md
+-rw-r--r--   0        0        0     2983 2024-04-01 20:44:32.163178 spice_rack-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      431 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/__init__.py
+-rw-r--r--   0        0        0     5064 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_base_base.py
+-rw-r--r--   0        0        0    12393 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_dispatchable.py
+-rw-r--r--   0        0        0      294 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_exception/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_exception/_error_info.py
+-rw-r--r--   0        0        0     6079 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_exception/_exception_base.py
+-rw-r--r--   0        0        0      778 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_exception/_exception_exception.py
+-rw-r--r--   0        0        0     1145 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_exception/_external_wrapper.py
+-rw-r--r--   0        0        0     5359 2024-04-01 20:44:12.351219 spice_rack-0.3.0/src/spice_rack/_bases/_exception/_http.py
+-rw-r--r--   0        0        0      157 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_mixins/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_mixins/_guid_mixin.py
+-rw-r--r--   0        0        0      628 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_mixins/_mixin_base.py
+-rw-r--r--   0        0        0     1637 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_mixins/_timestamped.py
+-rw-r--r--   0        0        0     4355 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_root.py
+-rw-r--r--   0        0        0      108 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_settings/__init__.py
+-rw-r--r--   0        0        0     2785 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_settings/_base.py
+-rw-r--r--   0        0        0      126 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_settings/_sources/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_settings/_sources/_base.py
+-rw-r--r--   0        0        0     2062 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py
+-rw-r--r--   0        0        0     4874 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_special_str.py
+-rw-r--r--   0        0        0      446 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_bases/_value_model.py
+-rw-r--r--   0        0        0      114 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/__init__.py
+-rw-r--r--   0        0        0    17738 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/_base.py
+-rw-r--r--   0        0        0      277 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/_exceptions/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/_exceptions/_dupe_keys.py
+-rw-r--r--   0        0        0     1835 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/_exceptions/_item_ix_invalid.py
+-rw-r--r--   0        0        0     1364 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/_exceptions/_key_already_exists.py
+-rw-r--r--   0        0        0     1510 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_frozen_registry/_exceptions/_missing_key.py
+-rw-r--r--   0        0        0      244 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/__init__.py
+-rw-r--r--   0        0        0     5589 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_exceptions.py
+-rw-r--r--   0        0        0     3377 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_info.py
+-rw-r--r--   0        0        0      464 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/__init__.py
+-rw-r--r--   0        0        0    13876 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_base.py
+-rw-r--r--   0        0        0      498 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_fs_inference.py
+-rw-r--r--   0        0        0     3462 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py
+-rw-r--r--   0        0        0      752 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_local.py
+-rw-r--r--   0        0        0     6385 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py
+-rw-r--r--   0        0        0    18138 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_fs_models.py
+-rw-r--r--   0        0        0      650 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_helpers.py
+-rw-r--r--   0        0        0      358 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_open_modes.py
+-rw-r--r--   0        0        0     1003 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/__init__.py
+-rw-r--r--   0        0        0     4666 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_abs.py
+-rw-r--r--   0        0        0     1775 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_base.py
+-rw-r--r--   0        0        0     1227 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py
+-rw-r--r--   0        0        0     4484 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_rel.py
+-rw-r--r--   0        0        0     1626 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_fs_ops/_services.py
+-rw-r--r--   0        0        0      163 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/_any_auth_strat.py
+-rw-r--r--   0        0        0      311 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_anon.py
+-rw-r--r--   0        0        0      736 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py
+-rw-r--r--   0        0        0     2088 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py
+-rw-r--r--   0        0        0     2045 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py
+-rw-r--r--   0        0        0      322 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_guid_service.py
+-rw-r--r--   0        0        0      306 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_log_aug/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_log_aug/_container.py
+-rw-r--r--   0        0        0     1015 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py
+-rw-r--r--   0        0        0     2395 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_log_level.py
+-rw-r--r--   0        0        0     6258 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_logger.py
+-rw-r--r--   0        0        0      421 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_logger_getter.py
+-rw-r--r--   0        0        0     3342 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_setup.py
+-rw-r--r--   0        0        0      140 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_sinks/__init__.py
+-rw-r--r--   0        0        0     3843 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_sinks/_base.py
+-rw-r--r--   0        0        0     1200 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_sinks/_file.py
+-rw-r--r--   0        0        0      967 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_logging/_sinks/_sys.py
+-rw-r--r--   0        0        0       53 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_misc/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_misc/_empty.py
+-rw-r--r--   0        0        0      149 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/__init__.py
+-rw-r--r--   0        0        0      123 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_services/__init__.py
+-rw-r--r--   0        0        0     1894 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_services/_joiner.py
+-rw-r--r--   0        0        0     1458 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_services/_json_dumper.py
+-rw-r--r--   0        0        0        0 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_services/_misc.py
+-rw-r--r--   0        0        0      234 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_types/__init__.py
+-rw-r--r--   0        0        0     5099 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_types/_collected_df.py
+-rw-r--r--   0        0        0      789 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_types/_dicts.py
+-rw-r--r--   0        0        0     1046 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_types/_discrim_helper.py
+-rw-r--r--   0        0        0     5258 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_types/_lazy_df.py
+-rw-r--r--   0        0        0     1652 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_polars_service/_types/_maybe_lazy.py
+-rw-r--r--   0        0        0      189 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_ts_service/__init__.py
+-rw-r--r--   0        0        0      623 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_ts_service/_fields.py
+-rw-r--r--   0        0        0     6271 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_ts_service/_timestamp.py
+-rw-r--r--   0        0        0     2643 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_ts_service/_tz_key.py
+-rw-r--r--   0        0        0      251 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_ts_service/_utils.py
+-rw-r--r--   0        0        0       97 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_utils/__init__.py
+-rw-r--r--   0        0        0     1131 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_utils/_container_differ.py
+-rw-r--r--   0        0        0     1406 2024-04-01 20:44:12.355219 spice_rack-0.3.0/src/spice_rack/_utils/_type_checkers.py
+-rw-r--r--   0        0        0      152 2024-04-01 20:44:12.359219 spice_rack-0.3.0/src/spice_rack/_version_getter.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 spice_rack-0.3.0/PKG-INFO
```

### Comparing `spice_rack-0.2.0/pyproject.toml` & `spice_rack-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_rack"
-version = "0.2.0"   # keep as 0.0.0 placeholder for poetry-dynamic-versioning
+version = "0.3.0"   # keep as 0.0.0 placeholder for poetry-dynamic-versioning
 description = "group of common things we use across different python packages"
 license = "Proprietary"
 authors = ["Tim Robin <timo.a.robin@gmail.com>",]
 readme = "README.md"
 
 packages = [
     {include = "spice_rack", from = "src"},
@@ -32,31 +32,43 @@
 devtools = { version = "*", extras = ["pygments"] }
 inflection = { version = "*", extras = [] }
 
 # why?
 tabulate = { version = "*", extras = [] }
 
 # optional dependencies
-
+#  Note: not actually optional at the moment
 # gcp
-gcsfs = { version = "==2024.2.0", optional = true}
-
+#gcsfs = { version = "==2024.2.0", optional = true}
+gcsfs = { version = "==2024.2.0" }
 
 # s3
-s3fs = { version = "*", optional = true }
-jmespath = { version = "*", optional = true }  # dep of s3fs that isn't picked up for some reason
-urllib3 = { version = "<2", optional = true }  # https://stackoverflow.com/questions/76414514/cannot-import-name-default-ciphers-from-urllib3-util-ssl-on-aws-lambda-us
+#s3fs = { version = "*", optional = true }
+#jmespath = { version = "*", optional = true }  # dep of s3fs that isn't picked up for some reason
+#urllib3 = { version = "<2", optional = true }  # https://stackoverflow.com/questions/76414514/cannot-import-name-default-ciphers-from-urllib3-util-ssl-on-aws-lambda-us
+
+s3fs = { version = "*" }
+jmespath = { version = "*" }  # dep of s3fs that isn't picked up for some reason
+urllib3 = { version = "<2" }  # https://stackoverflow.com/questions/76414514/cannot-import-name-default-ciphers-from-urllib3-util-ssl-on-aws-lambda-us
+
 
 # sftp
-paramiko = { version = "*", optional = true }
+#paramiko = { version = "*", optional = true }
+paramiko = { version = "*" }
+
+# dataframe stuff
+#polars = { version = "*", optional = true }
+polars = { version = "*" }
 
 [tool.poetry.extras]
-gcp = ["gcsfs"]
-aws = ["s3fs", "jmespath", "urrlib3"]
-sftp = ["paramiko", ]
+all = []
+#gcp = ["gcsfs"]
+#aws = ["s3fs", "jmespath", "urrlib3"]
+#sftp = ["paramiko", ]
+#polars = ["polars", ]
 
 [tool.poetry.dev-dependencies]
 
 # linter
 ruff = { version = "*", extras = [] }
 
 # mypy for static type checking
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_base_base.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_base_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 from __future__ import annotations
 import typing as t
-import json
 
 import pydantic
 
 
 __all__ = (
     "BASE_MODEL_CONFIG",
-    "CommonModelMethods"
+    "PydanticBase"
 )
 
 BASE_MODEL_CONFIG = pydantic.ConfigDict(
     extra="forbid",
 )
 
 
-SelfTV = t.TypeVar("SelfTV", bound=pydantic.BaseModel)
+SelfTV = t.TypeVar("SelfTV", bound="PydanticBase")
 
 
-class CommonModelMethods(pydantic.BaseModel):
+class PydanticBase(pydantic.BaseModel):
     """a base model we use for all pydantic models, even the other bases"""
-    def __iter__(self) -> t.Any:
-        raise NotImplementedError(
-            f"'{self.__class__.__name__}' doesn't have iteration implemented"
-        )
+
+    @classmethod
+    def get_cls_name(cls) -> str:
+        return cls.__name__
 
     def _post_init_setup(self) -> None:
+        """
+        Overwrite this hook to set perform misc. logic before calling _post_init_validation.
+        Common use case for this is initializing private attributes.
+        Notes: Make sure to call super()._post_init_setup
+        """
         return
 
     def _post_init_validation(self) -> None:
+        """
+        Overwrite this hook to set perform misc. validation logic on the instance, after
+        all other validators have been executed.
+        This is also called after the '_post_init_setup' hook is called
+        Notes: Make sure to call super()._post_init_validation
+        """
         return
 
-    def model_post_init(self, __context: t.Any) -> None:
+    @pydantic.model_validator(mode="after")
+    def _pydantic_post_init_val_hook(self: SelfTV) -> SelfTV:
+        """
+        Pydantic's hook that gets executed after we initialize an instance.
+        rather than overwrite this, overwrite the '_post_init_setup' and '_post_init_validation'
+        hooks
+        """
         self._post_init_setup()
         self._post_init_validation()
-        return
+        return self
 
     def json_dict(
             self,
-            use_str_fallback: bool = False,
+            use_str_fallback: bool = True,
             **pydantic_kwargs
     ) -> dict:
         """
         Converts a pydantic instance to a dict, going through json first.
         This is a convenience function for when you want a dict, but want to use the json
         encoders connected to the pydantic object.
 
         Args:
             use_str_fallback: if true, we cast anything we cannot encode to a string
             **pydantic_kwargs: any kwargs available for pydantic's json method. see their docs
 
         Returns:
-            dict: a natively json-encodable dict
-
-        Notes:
-            If the obj is a RootModel, calling `obj.json` would not necessarily return a dict,
-            so we convert it to the form, `{"__root__": data}` to align with how pydantic
-            would return `obj.dict()` in this scenario.
+            dict: a natively json-encodeable dict
 
         Examples:
             simple class with custom date encoder::
 
                 class Data(PydanticBase):
                     class Config:
                         json_encoders = {
@@ -80,26 +91,20 @@
                 # class. I just used a familiar string format, it could be whatever is specified
         """
         pydantic_kwargs = pydantic_kwargs if pydantic_kwargs is not None else {}
         if use_str_fallback:
             fallback = str
         else:
             fallback = None
-
-        pydantic_model_inst: pydantic.BaseModel = t.cast(
-            pydantic.BaseModel, self
-        )
-
-        pydantic_model_inst.model_dump_json()
-        dumped_json = pydantic_model_inst.__pydantic_serializer__.to_json(
+        return self.__pydantic_serializer__.to_python(
             self,
+            mode="json",
             fallback=fallback,
             **pydantic_kwargs,
         )
-        return json.loads(dumped_json)
 
     @classmethod
     def _import_forward_refs(cls) -> dict:
         """
         hook provided for convenience when you define a subclass with forward refs,
         to avoid circular import issue. Overwrite this method to do the imports and
         add the newly imported objects to a dict.
@@ -112,24 +117,30 @@
         Returns:
             dict: a dict of references to update
 
         """
         return {}
 
     @classmethod
-    def update_forward_refs(cls, **kwargs) -> None:
+    def model_rebuild(
+            cls,
+            *,
+            force: bool = False,
+            raise_errors: bool = True,
+            _parent_namespace_depth: int = 2,
+            _types_namespace: dict[str, t.Any] | None = None,
+    ) -> None:
         """
         This extends pydantic's builtin hook for updating forward refs.
         We call our special '_import_forward_refs' hook to automatically bring in the things
         imported there, but also if you want to use it like pydantic, i.e. call it directly and
         provide your refs to update via kwargs, that is still supported.
-
-        Returns:
-            None: doesn't return anything, mutates the class calling this method
-
-        Raises:
-            NameError: pydantic raises a NameError if a forward ref is not accounted for
-             in the kwargs
         """
+        _types_namespace_dict: dict[str, t.Any] = _types_namespace if _types_namespace else {}
         imported_refs = cls._import_forward_refs()
-        kwargs.update(imported_refs)
-        return super().update_forward_refs(**kwargs)  # type: ignore
+        _types_namespace_dict.update(imported_refs)
+        return super().model_rebuild(
+            force=force,
+            raise_errors=raise_errors,
+            _types_namespace=_types_namespace_dict,
+            _parent_namespace_depth=_parent_namespace_depth
+        )  # type: ignore
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_dispatchable.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_dispatchable.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 class ClassId(_special_str.SpecialStrBase):
     """the unique class id for a member of the dispatched family"""
     ...
 
 
+
 ClassIdPathT = t.Tuple[ClassId, ...]
 
 
 SelfTV = t.TypeVar("SelfTV", bound="DispatchedModelMixin")
 
 _LiteralT: t_ext.TypeAlias = type(t.Literal["xxx"])  # type: ignore
 
@@ -46,19 +47,24 @@
 
     CONCRETE = "concrete"
     """actual concrete type of the dispatched family tree. 
     You cannot inherit from this class it is Final
     """
 
 
-# looks like we could remove this and just use ClassId, but we have to use this
-# or the typing won't dispatch. I'm not sure why.
-
+# this has to be setup exactly as is. Anything overwriting __get_pydantic_core_schema__ will
+# break the way we generate the pydantic core schema. I am not sure exactly why, but for now
+# leave as is. This current setup does cause issues with pydantic_autodoc though.
 class _ClassIdStr(str):
     ...
+    # @classmethod
+    # def __get_pydantic_core_schema__(
+    #         cls, _: t.Any, __: pydantic.GetCoreSchemaHandler
+    # ) -> pydantic_core.CoreSchema:
+    #     return pydantic_core.core_schema.str_schema()
 
 
 class _PydanticSchemaGenerator(pydantic.GenerateSchema):
     _specified_class_id: t.ClassVar[t.Optional[str]] = None
 
     def __class_getitem__(cls, item: ClassId) -> t.Type[_PydanticSchemaGenerator]:
         new_cls = types.new_class(f"{item}_schema_gen", bases=(cls, ))
@@ -85,15 +91,15 @@
             )
         
 
 _model_config = _base_base.BASE_MODEL_CONFIG
 _model_config["schema_generator"] = _PydanticSchemaGenerator
 
 
-class DispatchedModelMixin(_base_base.CommonModelMethods):
+class DispatchedModelMixin(_base_base.PydanticBase):
     """
     the entrypoint for creating dispatchable family trees using pydantic's internal
     engine for schema generation. Be careful not to inherit from two different
     dispatchable family trees at once. It will cause weird behavior and there
     are no checks to protect against this.
 
     """
@@ -130,15 +136,18 @@
 
         # if super root parent, we assume root
         if parent_class_type == ClassType.SUPER_ROOT:
             class_type_actual = ClassType.ROOT
 
         # if root parent, we assume concrete
         elif parent_class_type == ClassType.ROOT:
-            class_type_actual = ClassType.CONCRETE
+            if cls.__name__.startswith("Abstract"):
+                class_type_actual = ClassType.ROOT
+            else:
+                class_type_actual = ClassType.CONCRETE
 
         # if concrete parent, we raise ValueError
         elif parent_class_type == ClassType.CONCRETE:
             raise ValueError(
                 f"'{cls.__name__}' direct parent is '{parent_class.__name__}' which is a"
                 f" concrete class, so we shouldn't be inheriting from it."
             )
@@ -299,14 +308,23 @@
         """
         use the type annotation created by `build_dispatched_ann` in a pydantic TypeAdapter
         that allows us to get the "discriminated union" parsing functionality outside a
         pydantic class context. see pydantic type adapter docs
         """
         return pydantic.TypeAdapter(cls.build_dispatched_ann())
 
+    @classmethod
+    def get_all_concrete_subclass_ids(cls) -> t.List[ClassId]:
+        res = []
+        for concrete_sub_c in cls.iter_concrete_subclasses():
+            res.append(
+                concrete_sub_c.get_class_id()
+            )
+        return res
+
 
 DispatchedClsTV = t.TypeVar("DispatchedClsTV", bound=DispatchedModelMixin)
 
 
 class DispatchedClassContainer(pydantic.RootModel[DispatchedClsTV], t.Generic[DispatchedClsTV]):
     """
     convenience wrapper allowing you to specify a dispatched family root class as the class
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_exception/_error_info.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_exception/_error_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,10 +37,7 @@
 
     error_type: str = Field(
         description="the name of the error class this payload is connected to"
     )
     info: ErrorInfoTV = Field(
         description="object containing more detailed information about the error"
     )
-
-    def json_dict(self, use_str_fallback: bool = True, **pydantic_kwargs) -> dict:
-        return super().json_dict(use_str_fallback=use_str_fallback, **pydantic_kwargs)
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_exception/_exception_exception.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_exception/_exception_exception.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_exception/_external_wrapper.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_exception/_external_wrapper.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_mixins/_timestamped.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_mixins/_timestamped.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 import datetime as dt
 import pydantic
 
+from spice_rack._bases._mixins._mixin_base import PydanticMixinBase
+
 
 __all__ = ("CreatedAtMixin", "UpdatedAtMixin", "CreatedAtUpdatedAtMixin")
 
 
 def _get_current_utc_datetime() -> dt.datetime:
     return dt.datetime.utcnow()
 
 
-class CreatedAtMixin(pydantic.BaseModel):
+class CreatedAtMixin(PydanticMixinBase):
     """
     adds a datetime field, 'created_at' that can be timezone aware or naive
     """
     created_at: dt.datetime = pydantic.Field(
         description="timestamp the object was created at",
         default_factory=_get_current_utc_datetime
     )
@@ -24,15 +26,15 @@
         return data.isoformat()
 
     @property
     def created_at_str(self) -> str:
         return self.created_at.isoformat()
 
 
-class UpdatedAtMixin(pydantic.BaseModel):
+class UpdatedAtMixin(PydanticMixinBase):
     """
     adds a datetime field, 'updated_at' that can be timezone aware or naive
     """
     updated_at: dt.datetime = pydantic.Field(
         description="timestamp the object was last updated",
         default_factory=_get_current_utc_datetime
     )
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_settings/_base.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_settings/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
         use double underscores, '__', as the nested delimiter
 
     References:
         - https://docs.pydantic.dev/1.10/usage/settings/
     """
     _singleton_source: t.ClassVar[t.Optional[_sources.SingletonSource]] = None
 
-    model_config = pydantic_settings.SettingsConfigDict()
+    model_config = pydantic_settings.SettingsConfigDict(
+        extra="ignore"
+    )
 
     def __init_subclass__(cls, singleton_mode: bool = True, **kwargs):
         if singleton_mode:
             cls._singleton_source = _sources.SingletonSource(
                 settings_cls=cls
             )
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py` & `spice_rack-0.3.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_exceptions.py` & `spice_rack-0.3.0/src/spice_rack/_ts_service/_tz_key.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,97 @@
 from __future__ import annotations
-import typing as t
-import pydantic
+from typing import Optional
+import zoneinfo
+import tzlocal
 
 from spice_rack import _bases
 
-if t.TYPE_CHECKING:
-    from spice_rack._fs_ops import _path_strs, _file_systems
 
 __all__ = (
-    "InvalidPathStrException",
-    "NonExistentPathException",
-    "PathAlreadyExistsException",
+    "TimeZoneKey",
+    "InvalidTimeZoneKeyException"
 )
 
-ErrorInfoBase = _bases.exceptions.ErrorInfoBase
-CustomExceptionBase = _bases.exceptions.CustomExceptionBase
 
+# todo: specify these or find another way
+class TimeZoneKey(_bases.special_str.SpecialStrBase):
+    """
+    a special string representing a timezone.
+
+    see python docs for "zoneinfo" for options:
+        https://docs.python.org/3/library/zoneinfo.html
+    """
+
+    @classmethod
+    def timezone_choices(cls) -> list[str]:
+        return list(zoneinfo.available_timezones())
+
+    @classmethod
+    def _format_str_val(cls, root_data: str) -> str:
+        # ensure it is a valid zone info
+        choices = zoneinfo.available_timezones()
+        if root_data not in choices:
+            raise InvalidTimeZoneKeyException(
+                invalid_value=root_data,
+                options=list(choices)
+            )
 
-class _InvalidPathStrErrorInfo(ErrorInfoBase):
-    """this is raised when one of the path string classes fails to validate a raw string"""
-    raw_str: str
-    issues: t.List[str]
-
-
-class InvalidPathStrException(CustomExceptionBase[_InvalidPathStrErrorInfo]):
-    """this is raised when one of the path string classes fails to validate a raw string"""
-    def __init__(
-            self,
-            detail: str,
-            raw_str: str,
-            issues: t.Union[str, list[str]],
-            verbose: bool = True,
-            extra_info: t.Dict = None
-    ):
-
-        issue_lst: t.List[str]
-        if isinstance(issues, str):
-            issue_lst = [issues]
         else:
-            issue_lst = issues
-
-        super().__init__(
-            detail=detail,
-            error_info={
-                "raw_str": raw_str,
-                "issues": issue_lst
-            },
-            verbose=verbose,
-            extra_info=extra_info
-        )
-
-
-class _NonExistentPathErrorInfo(ErrorInfoBase):
-    """path not found on file system"""
-    file_system_info: t.Dict = pydantic.Field(description="the file system we were using")
-    path: str
+            return root_data
 
+    def as_zone_info(self) -> zoneinfo.ZoneInfo:
+        return zoneinfo.ZoneInfo(str(self))
 
-class NonExistentPathException(CustomExceptionBase[_NonExistentPathErrorInfo]):
-    def __init__(
-            self,
-            file_system: _file_systems.AbstractFileSystem,
-            path: _path_strs.FileOrDirAbsPathT,
-            verbose: bool = True,
-            extra_info: t.Dict = None
-    ):
-        detail = "either the file path does not exist or we do not have access to it"
-        error_info = {
-            "file_system_info": file_system.__get_logger_data__(),
-            "path": file_system.contextualize_abs_path(path)
-        }
-        super().__init__(
-            detail=detail,
-            error_info=error_info,
-            verbose=verbose,
-            extra_info=extra_info
-        )
-
-
-class _PathAlreadyExistsErrorInfo(ErrorInfoBase):
-    """path found when we didn't expect to"""
-    file_system_info: t.Dict = pydantic.Field(description="the file system we were using")
-    path: str
+    @classmethod
+    def local(cls) -> TimeZoneKey:
+        """gets timezone info for where this process is running"""
+        return TimeZoneKey(tzlocal.get_localzone().key)
+
+
+# class _InvalidTimeZoneKeyErrorInfo(exception_base.ErrorInfoBase):
+#     invalid_value: str
+#     options: list[str]
+#
+#
+# class InvalidTimeZoneKeyException(exception_base.ExceptionBase[_InvalidTimeZoneKeyErrorInfo]):
+#     def __init__(
+#             self,
+#             invalid_value: str,
+#             options: list[str],
+#             extra_info: Optional[dict] = None,
+#             verbose: bool = False
+#     ):
+#         error_info = {
+#             "invalid_value": invalid_value,
+#             "options": options
+#         }
+#
+#         detail = f"'{invalid_value}' is not a valid timezone key."
+#         super().__init__(
+#             detail=detail,
+#             error_info=error_info,
+#             extra_info=extra_info,
+#             verbose=verbose
+#         )
 
 
-class PathAlreadyExistsException(CustomExceptionBase[_PathAlreadyExistsErrorInfo]):
+# for now
+class InvalidTimeZoneKeyException(Exception):
     def __init__(
             self,
-            file_system: _file_systems.AbstractFileSystem,
-            path: _path_strs.FileOrDirAbsPathT,
-            verbose: bool = True,
-            extra_info: t.Dict = None
+            invalid_value: str,
+            options: list[str],
+            extra_info: Optional[dict] = None,
+            verbose: bool = False
     ):
-        detail = "this path already exists"
-        error_info = {
-            "file_system_info": file_system.__get_logger_data__(),
-            "path": file_system.contextualize_abs_path(path)
-        }
-        super().__init__(
-            detail=detail,
-            error_info=error_info,
-            verbose=verbose,
-            extra_info=extra_info
-        )
+        # error_info = {
+        #     "invalid_value": invalid_value,
+        #     "options": options
+        # }
+        detail = f"'{invalid_value}' is not a valid timezone key."
+        # super().__init__(
+        #     detail=detail,
+        #     error_info=error_info,
+        #     extra_info=extra_info,
+        #     verbose=verbose
+        # )
+        super().__init__(detail)
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_info.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_info.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_base.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from abc import abstractmethod
 import typing as t
 from fsspec.spec import AbstractFileSystem as AbstractFsSpecFileSystem
+import pydantic
 
 from spice_rack import _bases, _logging
 from spice_rack._fs_ops import _path_strs, _file_info, _open_modes, _exceptions
 
 
 __all__ = (
     "AbstractFileSystem",
@@ -27,37 +28,44 @@
         return self.build_fsspec_file_system()
 
     @classmethod
     @abstractmethod
     def get_fs_specific_prefix(cls) -> str:
         ...
 
+    @classmethod
+    @pydantic.validate_call
     def clean_raw_path_str(
-            self,
-            raw_path: str,
+            cls,
+            __raw_path: str,
     ) -> _path_strs.FileOrDirAbsPathT:
-        assert isinstance(raw_path, str), type(raw_path)
-        cleaned_path = raw_path.replace(
-            self.get_fs_specific_prefix(),
+        """
+        strip the raw path of the file system-specific prefix, and cast it to a
+        standardized directory or file path representation.
+
+        This is the inverse of 'contextualize_abs_path'.
+        """
+        cleaned_path = __raw_path.replace(
+            cls.get_fs_specific_prefix(),
             "/",
             1
         )
         return _path_strs.FileOrDirAbsPathTypeAdapter.validate_python(
             cleaned_path
         )
 
-    def contextualize_abs_path(self, path: _path_strs.FileOrDirAbsPathT) -> str:
+    @pydantic.validate_call
+    def contextualize_abs_path(self, __path: _path_strs.FileOrDirAbsPathT) -> str:
         """
-        take an absolute path, in the general representation
-        and add the file system specific prefix
+        convert a standardized file or directory path representation into a
+        str starting with the file system-specific prefix.
+        This is the inverse of 'clean_raw_path_str'.
         """
-        if not isinstance(path, (_path_strs.AbsoluteFilePathStr, _path_strs.AbsoluteDirPathStr)):
-            raise ValueError(f"should be an absolute path type, encountered type: {type(path)}")
         prefix_val = self.get_fs_specific_prefix()
-        formatted_path_str = prefix_val + str(path)[1:]
+        formatted_path_str = prefix_val + str(__path)[1:]
         return formatted_path_str
 
     @abstractmethod
     def get_home_dir(self) -> _path_strs.AbsoluteDirPathStr:
         ...
 
     def __hash__(self) -> int:
@@ -76,201 +84,195 @@
 
     def __get_logger_data__(self) -> t.Dict:
         return {
             "file_system_type": self.class_id,
             "file_system_home_dir": self.contextualize_abs_path(self.get_home_dir())
         }
 
-    @t.final
-    def exists(self, path: _path_strs.FileOrDirAbsPathT) -> bool:
+    @pydantic.validate_call
+    def exists(self, __path: _path_strs.FileOrDirAbsPathT) -> bool:
         """
         returns True if this file system object exists, false otherwise
         """
 
         # todo: what if perms issue not existence issue?
-        return self.fsspec_obj.exists(self.contextualize_abs_path(path))
+        return self.fsspec_obj.exists(self.contextualize_abs_path(__path))
 
-    def ensure_exists(self, path: _path_strs.FileOrDirAbsPathT) -> None:
+    @pydantic.validate_call
+    def ensure_exists(self, __path: _path_strs.FileOrDirAbsPathT) -> None:
         """
         ensure the file or dir path exists, raising an exception if not
 
         Args:
-            path: the path to the file or directory
+            __path: the path to the file or directory
 
         Returns: Nothing
 
         Raises:
             NonExistentPathException: if the path doesn't exist, or we cannot access it
 
         """
-        exists = self.exists(path)
+        exists = self.exists(__path)
         if not exists:
             raise _exceptions.NonExistentPathException(
                 file_system=self,
-                path=path,
+                path=__path,
+            )
+        else:
+            return
+
+    @pydantic.validate_call
+    def ensure_nonexistent(self, __path: _path_strs.FileOrDirAbsPathT) -> None:
+        """
+        ensure the file or dir path does exist, raising an exception if it does
+
+        Args:
+            __path: the path to the file or directory
+
+        Returns: Nothing
+
+        Raises:
+            PathAlreadyExistsException: if the path does exist
+        """
+        exists = self.exists(__path)
+        if exists:
+            raise _exceptions.PathAlreadyExistsException(
+                file_system=self,
+                path=__path,
             )
         else:
             return
 
-    @staticmethod
+    @pydantic.validate_call
     def ensure_correct_file_ext(
-            path: _path_strs.RelOrAbsFilePathT,
+            self,
+            __path: _path_strs.RelOrAbsFilePathT,
+            *,
             choices: list[_file_info.FileExt]
     ) -> None:
         """
         ensure the file path has one of the specified extensions
         Args:
-            path: the path we are checking
+            __path: the path we are checking
             choices: the valid extensions
 
         Returns: Nothing
 
         Raises:
             FilePathInvalidException: if the file path has no extension of it isn't
                 one of the choices
-
         """
-        file_ext = path.get_file_ext()
-        if file_ext is None:
-            raise ValueError(
-                f"'{path}' has no file extensions"
-            )
-            # raise _exceptions.FilePathInvalidException(
-            #     file_system=self,
-            #     path=path,
-            #     reason="no file extension found on the file path",
-            #     extra_info={
-            #         "choices": choices,
-            #     }
-            # )
-
-        if file_ext not in choices:
-            raise ValueError(
-                f"'{path}' file extension isn't one of {choices}"
+        file_ext = __path.get_file_ext()
+        if file_ext is None or file_ext not in choices:
+            raise _exceptions.InvalidFileExtensionException(
+                path=__path,
+                file_ext_found=file_ext,
+                file_ext_choices=choices,
             )
-            # raise _exceptions.FilePathInvalidException(
-            #     file_system=self,
-            #     path=path,
-            #     reason=f"the file extension, '{file_ext}', not one of the choices",
-            #     extra_info={
-            #         "file_path": path,
-            #         "choices": choices,
-            #     }
-            # )
         return
 
-    # def ensure_correct_mime_type(
-    #         self,
-    #         path: _path_strs.AbsoluteFilePathStr,
-    #         choices: list[_special_types.MimeType]
-    # ) -> None:
-    #     """
-    #     ensure the file path is one of the specified mime types
-    #     Args:
-    #         path: the path we are checking
-    #         choices: the valid mime types
-    #
-    #     Returns: Nothing
-    #
-    #     Raises:
-    #         FilePathInvalidException: if we cannot determine the mime type, or it is not one
-    #             of the specified choices
-    #     """
-    #     mime_type = path.get_file_ext()
-    #     if mime_type is None:
-    #         raise _exceptions.FilePathInvalidException(
-    #             file_system=self,
-    #             path=path,
-    #             reason="unable to infer mime type from the file path",
-    #             extra_info={
-    #                 "choices": choices,
-    #             }
-    #         )
-    #     if mime_type not in choices:
-    #         raise _exceptions.FilePathInvalidException(
-    #             file_system=self,
-    #             path=path,
-    #             reason=f"the inferred mime type, '{mime_type}', not one of the choices",
-    #             extra_info={
-    #                 "choices": choices,
-    #             }
-    #         )
-    #     return
+    @pydantic.validate_call
+    def ensure_correct_mime_type(
+            self,
+            __path: _path_strs.AbsoluteFilePathStr,
+            *,
+            choices: list[_file_info.MimeType]
+    ) -> None:
+        """
+        ensure the file path is one of the specified mime types
+        Args:
+            __path: the path we are checking
+            choices: the valid mime types
+
+        Returns: Nothing
+
+        Raises:
+            InvalidFileMimeTypeException: if we cannot determine the mime type, or it is not one
+                of the specified choices
+        """
+        mime_type_found = __path.get_mime_type()
+        if not mime_type_found or mime_type_found not in choices:
+            raise _exceptions.InvalidFileMimeTypeException(
+                path=__path,
+                mime_type_found=mime_type_found,
+                mime_type_choices=choices,
+                verbose=True
+            )
 
+    @pydantic.validate_call
     def open_file(
             self,
-            path: _path_strs.AbsoluteFilePathStr,
+            __path: _path_strs.AbsoluteFilePathStr,
             mode: _open_modes.SupportedOpenModesT
     ) -> _open_modes.OpenFileT:
         """
         return a readable open file object. todo: revisit type annotations of the return type here
 
         Args:
-            path: the file path str
+            __path: the file path str
             mode: the mode we are opening in
 
         Returns:
             the readable open file object
         """
         if mode != "wb":
-            self.ensure_exists(path=path)
-        return self.fsspec_obj.open(path=self.contextualize_abs_path(path), mode=mode)
+            self.ensure_exists(__path)
+        return self.fsspec_obj.open(
+            path=self.contextualize_abs_path(__path), mode=mode
+        )
 
+    @pydantic.validate_call
     def delete_file(
             self,
-            path: _path_strs.AbsoluteFilePathStr,
+            __path: _path_strs.AbsoluteFilePathStr,
+            *,
             if_non_existent: t.Literal["raise", "return"] = "return"
     ) -> None:
         """
         delete the file
         """
-
-        exists = self.exists(path)
+        exists = self.exists(__path)
         if not exists:
             if if_non_existent == "raise":
-                self.ensure_exists(path)
+                self.ensure_exists(__path)
 
         else:
             # what if perms issue not existence issue?
-            self.fsspec_obj.delete(path=self.contextualize_abs_path(path), recursive=True)
+            self.fsspec_obj.delete(path=self.contextualize_abs_path(__path), recursive=True)
         return
 
+    @pydantic.validate_call
     def delete_dir(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
+            __path: _path_strs.AbsoluteDirPathStr,
+            *,
             recursive: bool = True,
             if_non_existent: t.Literal["raise", "return"] = "return"
     ) -> None:
         """
-        delete the directory
+        delete the directory, if recursive is true, we delete all files and subdirectories
         """
-
-        from devtools import debug
-        debug(path)
-
-        exists = self.exists(path)
-
-        debug(path)
-
+        exists = self.exists(__path)
         if not exists:
             if if_non_existent == "raise":
-                self.ensure_exists(path)
+                self.ensure_exists(__path)
 
         else:
             # what if perms issue not existence issue?
-            self.fsspec_obj.delete(path=self.contextualize_abs_path(path), recursive=recursive)
+            self.fsspec_obj.delete(path=self.contextualize_abs_path(__path), recursive=recursive)
         return
 
+    @pydantic.validate_call
     def iter_dir_contents(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
+            __path: _path_strs.AbsoluteDirPathStr,
     ) -> t.Iterator[_path_strs.FileOrDirAbsPathT]:
         """iterate over the top level dir contents"""
         for raw_info_rec_i in self.fsspec_obj.listdir(
-            self.contextualize_abs_path(path)
+            self.contextualize_abs_path(__path)
         ):
             raw_path_i = raw_info_rec_i.get("name")
             if raw_path_i is None:
                 raise ValueError(
                     "'name' not found in record?"
                 )
                 # raise _exceptions.FileSystemException(
@@ -295,101 +297,122 @@
                 path_i = _path_strs.AbsoluteDirPathStr(formatted_path_i)
 
             else:
                 raise ValueError(f"unexpected type val: '{raw_type}'")
 
             yield path_i
 
+    @pydantic.validate_call
     def list_dir_contents(
             self,
-            path: _path_strs.AbsoluteDirPathStr
+            __path: _path_strs.AbsoluteDirPathStr
     ) -> list[_path_strs.FileOrDirAbsPathT]:
-        return list(self.iter_dir_contents(path=path))
+        """exhaust the iterator built from 'iter_dir_contents' returning
+        the items in a list"""
+        return list(self.iter_dir_contents(__path))
 
+    @pydantic.validate_call
     def iter_dir_contents_files_only(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
+            __path: _path_strs.AbsoluteDirPathStr,
+            *,
             recursive: bool = True
     ) -> t.Iterator[_path_strs.AbsoluteFilePathStr]:
-        for path_i in self.iter_dir_contents(path=path):
+        """iterate over every file in a directory, recursing into subdirectories if
+        recursive is True"""
+        for path_i in self.iter_dir_contents(__path):
             if isinstance(path_i, _path_strs.AbsoluteFilePathStr):
                 yield path_i
             elif isinstance(path_i, _path_strs.AbsoluteDirPathStr):
                 if recursive:
                     for path_ij in self.iter_dir_contents_files_only(
                         path=path_i,
                         recursive=recursive,
                     ):
                         yield path_ij
                 else:
                     continue
             else:
                 raise ValueError(type(path_i))
 
+    @pydantic.validate_call
     def make_dir(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
+            __path: _path_strs.AbsoluteDirPathStr,
+            *,
             if_exists: t.Literal["raise", "return"] = "return",
             create_parents: bool = True
     ) -> None:
-        if self.exists(path=path):
+        """create a new directory, and parents if the parent directory doesn't exist"""
+        if self.exists(__path):
             if if_exists == "raise":
-                raise ValueError(
-                    f"'{path}'already exists, cannot make it."
+                raise _exceptions.PathAlreadyExistsException(
+                    file_system=self,
+                    path=__path,
+                    extra_info={
+                        "action_attempted": "make_dir"
+                    }
                 )
-                # raise _exceptions.PathAlreadyExistsException(
-                #     file_system=self,
-                #     path=path,
-                #     extra_info={
-                #         "action_attempted": "make_dir"
-                #     }
-                # )
             else:
                 return
 
         else:
             self.fsspec_obj.mkdir(
-                path=self.contextualize_abs_path(path),
+                path=self.contextualize_abs_path(__path),
                 create_parents=create_parents
             )
 
+    @pydantic.validate_call
     def download_file_locally(
             self,
-            path: _path_strs.AbsoluteFilePathStr,
-            dest_dir: _path_strs.AbsoluteDirPathStr
+            __source_path: _path_strs.AbsoluteFilePathStr,
+            __local_dest_dir: _path_strs.AbsoluteDirPathStr
     ) -> _path_strs.AbsoluteFilePathStr:
+        """
+        download file from current file system into the local file system.
+
+        the downloaded file will have the same name as the source file, inside the
+        specified local directory.
+        """
         from spice_rack._fs_ops._file_systems import _local
         local_fs = _local.LocalFileSystem()
-        local_fs.make_dir(dest_dir, if_exists="return", create_parents=True)
+        local_fs.make_dir(__local_dest_dir, if_exists="return", create_parents=True)
 
-        local_path = dest_dir.joinpath(
-            _path_strs.RelFilePathStr(path.get_name(include_suffixes=True))
+        local_path = __local_dest_dir.joinpath(
+            _path_strs.RelFilePathStr(__source_path.get_name(include_suffixes=True))
         )
         self.fsspec_obj.download(
             lpath=local_fs.contextualize_abs_path(local_path),
-            rpath=self.contextualize_abs_path(path)
+            rpath=self.contextualize_abs_path(__source_path)
         )
         return local_path
 
+    @pydantic.validate_call
     def download_dir_locally(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
-            dest_dir: _path_strs.AbsoluteDirPathStr
+            __source_dir: _path_strs.AbsoluteDirPathStr,
+            __local_dest_dir: _path_strs.AbsoluteDirPathStr
     ) -> _path_strs.AbsoluteDirPathStr:
+        """
+        download directory from current file system into the local file system.
+
+        the downloaded directory will have the same name as the source directory, inside the
+        specified local directory.
+        """
         from spice_rack._fs_ops._file_systems import _local
         from spice_rack._fs_ops._helpers import is_placeholder_file_path
         local_fs = _local.LocalFileSystem()
-        local_fs.make_dir(dest_dir, if_exists="return", create_parents=True)
+        local_fs.make_dir(__local_dest_dir, if_exists="return", create_parents=True)
 
-        local_path = dest_dir.joinpath(
-            _path_strs.RelDirPathStr(path.get_name())
+        local_path = __local_dest_dir.joinpath(
+            _path_strs.RelDirPathStr(__source_dir.get_name())
         )
         self.fsspec_obj.download(
             lpath=local_fs.contextualize_abs_path(local_path),
-            rpath=self.contextualize_abs_path(path),
+            rpath=self.contextualize_abs_path(__source_dir),
             recursive=True
         )
 
         # remove possible placeholder files
         for local_path_i in local_fs.iter_dir_contents_files_only(local_path):
             if is_placeholder_file_path(local_path_i):
                 local_fs.delete_file(
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
-from typing import final, Union, Literal, Iterator
+import typing as t
 import gcsfs  # noqa
-from pydantic import Field
+import pydantic
 
 from spice_rack._fs_ops import _path_strs, _helpers
 from spice_rack._fs_ops._file_systems import _base
 from spice_rack import _gcp_auth
 
 
 __all__ = (
     "GcsFileSystem",
 )
 
 
-@final
+@t.final
 class GcsFileSystem(_base.AbstractFileSystem, class_id="gcs"):
     """wrapper for the GCSFileSystem file system"""
-    creds: _gcp_auth.AnyGcpAuthStrat = Field(
+    creds: _gcp_auth.AnyGcpAuthStrat = pydantic.Field(
         description="the credentials we use to authenticate to the gcs bucket",
         default_factory=_gcp_auth.AnyGcpAuthStrat.init_default
     )
 
     @classmethod
     def get_fs_specific_prefix(cls) -> str:
         return "gs://"
 
     def _get_gcsfs_token(
             self,
-    ) -> Union[str, dict]:
+    ) -> t.Union[str, dict]:
         creds: _gcp_auth.auth_strategies.AbstractGcpAuthStrategy = self.creds.root
 
         if isinstance(creds, _gcp_auth.auth_strategies.AnonAuthStrategy):
             return "anon"
 
         elif isinstance(creds, _gcp_auth.auth_strategies.DefaultAuthStrategy):
             if creds.default_creds_found():
@@ -56,35 +56,41 @@
 
     def build_fsspec_file_system(self) -> gcsfs.GCSFileSystem:
         token = self._get_gcsfs_token()
         return gcsfs.GCSFileSystem(
             token=token
         )
 
+    @pydantic.validate_call
     def make_dir(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
-            if_exists: Literal["raise", "return"] = "return",
+            __path: _path_strs.AbsoluteDirPathStr,
+            *,
+            if_exists: t.Literal["raise", "return"] = "return",
             create_parents: bool = True
     ) -> None:
 
         # creating cloud dir doesn't work like local bc how
         # they treat directories. We create a placeholder
         # file when making a directory to imitate this.
-        super().make_dir(path=path, if_exists=if_exists, create_parents=create_parents)
-        if not self.exists(path):
-            placeholder_path = path.joinpath(rel_path=_helpers.get_placeholder_rel_path())
+        super().make_dir(__path, if_exists=if_exists, create_parents=create_parents)
+        if not self.exists(__path):
+            placeholder_path = __path.joinpath(rel_path=_helpers.get_placeholder_rel_path())
             with self.open_file(placeholder_path, "wb") as f:
                 f.write("placeholder text".encode())
 
+    @pydantic.validate_call
     def iter_dir_contents(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
-    ) -> Iterator[_path_strs.FileOrDirAbsPathT]:
-        for path_i in super().iter_dir_contents(path=path):
+            __path: _path_strs.AbsoluteDirPathStr,
+    ) -> t.Iterator[_path_strs.FileOrDirAbsPathT]:
+        """
+        same iter as base class, except we also skip the file if it is the placeholder file
+        """
+        for path_i in super().iter_dir_contents(__path):
             if _helpers.is_placeholder_file_path(path_i):
                 continue
             else:
                 yield path_i
 
     def get_home_dir(self) -> _path_strs.AbsoluteDirPathStr:
         return _path_strs.AbsoluteDirPathStr("/")
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_local.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_local.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import typing as t
-from pydantic import Field
+from pydantic import Field, validate_call
 from fsspec.implementations import sftp
 from paramiko.sftp_file import SFTPFile as ParamikoSftpFile
 from paramiko.sftp_client import SFTPClient as ParamikoSftpClient
 
 from spice_rack._fs_ops import _path_strs
 from spice_rack._fs_ops._file_systems import _base
 
@@ -75,30 +75,33 @@
         _paramiko_sftp_get(
             sftp_client=paramiko_client,
             sftp_file=self.contextualize_abs_path(path),
             local_file=str(local_path),
         )
         return local_path
 
+    @validate_call
     def download_dir_locally(
             self,
-            path: _path_strs.AbsoluteDirPathStr,
-            dest_dir: _path_strs.AbsoluteDirPathStr
+            __source_dir: _path_strs.AbsoluteDirPathStr,
+            __local_dest_dir: _path_strs.AbsoluteDirPathStr
     ) -> _path_strs.AbsoluteDirPathStr:
         from spice_rack._fs_ops._file_systems import _local
         local_fs = _local.LocalFileSystem()
-        local_fs.make_dir(dest_dir, if_exists="return", create_parents=True)
+        local_fs.make_dir(__source_dir, if_exists="return", create_parents=True)
 
-        local_path = dest_dir.joinpath(
-            _path_strs.RelDirPathStr(path.get_name())
+        local_path = __local_dest_dir.joinpath(
+            _path_strs.RelDirPathStr(__source_dir.get_name())
         )
 
-        for source_abs_file_path in self.iter_dir_contents_files_only(path, recursive=True):
+        for source_abs_file_path in self.iter_dir_contents_files_only(
+                __source_dir, recursive=True
+        ):
             rel_file_path = _path_strs.RelFilePathStr(
-                str(source_abs_file_path).replace(str(path), "")
+                str(source_abs_file_path).replace(str(__source_dir), "")
             )
             dest_abs_file_path = local_path.joinpath(rel_file_path)
             self.download_file_locally(
                 path=source_abs_file_path, dest_dir=dest_abs_file_path.get_parent()
             )
         return local_path
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/__init__.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,20 +19,24 @@
 RelOrAbsFilePathT = t.Annotated[
     t.Union[
         t.Annotated[AbsoluteFilePathStr, pydantic.Tag("abs")],
         t.Annotated[RelFilePathStr, pydantic.Tag("rel")],
     ],
     pydantic.Discriminator(_discrim)
 ]
-RelOrAbsFilePathTypeAdapter = pydantic.TypeAdapter(RelOrAbsFilePathT)
+RelOrAbsFilePathTypeAdapter: pydantic.TypeAdapter[RelOrAbsFilePathT] = pydantic.TypeAdapter(
+    RelOrAbsFilePathT
+)
 
 
 RelOrAbsDirPathT = t.Annotated[
     t.Union[
         t.Annotated[AbsoluteDirPathStr, pydantic.Tag("abs")],
         t.Annotated[RelDirPathStr, pydantic.Tag("rel")],
     ],
     pydantic.Discriminator(_discrim)
 ]
 
 
-RelOrAbsDirPathTypeAdapter = pydantic.TypeAdapter(RelOrAbsDirPathT)
+RelOrAbsDirPathTypeAdapter: pydantic.TypeAdapter[RelOrAbsDirPathT] = pydantic.TypeAdapter(
+    RelOrAbsDirPathT
+)
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_abs.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_abs.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,8 +147,10 @@
         t.Annotated[AbsoluteFilePathStr, pydantic.Tag("file")],
         t.Annotated[AbsoluteDirPathStr, pydantic.Tag("dir")],
     ],
     pydantic.Discriminator(_discrim)
 ]
 
 
-FileOrDirAbsPathTypeAdapter = pydantic.TypeAdapter(FileOrDirAbsPathT)
+FileOrDirAbsPathTypeAdapter: pydantic.TypeAdapter[FileOrDirAbsPathT] = pydantic.TypeAdapter(
+    FileOrDirAbsPathT
+)
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_base.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_fs_ops/_path_strs/_rel.py` & `spice_rack-0.3.0/src/spice_rack/_fs_ops/_path_strs/_rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,8 +146,10 @@
         t.Annotated[RelFilePathStr, pydantic.Tag("file")],
         t.Annotated[RelDirPathStr, pydantic.Tag("dir")],
     ],
     pydantic.Discriminator(_discrim)
 ]
 
 
-FileOrDirRelPathTypeAdapter = pydantic.TypeAdapter(FileOrDirRelPathT)
+FileOrDirRelPathTypeAdapter: pydantic.TypeAdapter[FileOrDirRelPathT] = pydantic.TypeAdapter(
+    FileOrDirRelPathT
+)
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_gcp_auth/_any_auth_strat.py` & `spice_rack-0.3.0/src/spice_rack/_gcp_auth/_any_auth_strat.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py` & `spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py` & `spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py` & `spice_rack-0.3.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_log_aug/_container.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_log_aug/_container.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_log_level.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_log_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import typing as t
 import pydantic
 
+from spice_rack import _bases
 
 __all__ = (
     "LogLevel",
 )
 
 
 _LogLevelStrLiteralT = t.Literal[
@@ -30,15 +31,15 @@
     zip(t.get_args(_LogLevelStrLiteralT), t.get_args(_LogLevelIntLiteralT))
 )
 _int_to_str: t.Dict[_LogLevelIntLiteralT, _LogLevelStrLiteralT] = dict(
     zip(t.get_args(_LogLevelIntLiteralT), t.get_args(_LogLevelStrLiteralT))
 )
 
 
-class LogLevel(pydantic.RootModel[_LogLevelLiteralT]):
+class LogLevel(_bases.root.RootModel[_LogLevelLiteralT]):
     """
     a root model holding enum values.
     """
     _str_to_int: t.ClassVar[t.Dict[_LogLevelStrLiteralT, _LogLevelIntLiteralT]] = _str_to_int
     _int_to_str: t.ClassVar[t.Dict[_LogLevelIntLiteralT, _LogLevelStrLiteralT]] = _int_to_str
 
     @pydantic.model_validator(mode="before")
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_logger.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_logger.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_setup.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_setup.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_sinks/_base.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_sinks/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_sinks/_file.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_sinks/_file.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_logging/_sinks/_sys.py` & `spice_rack-0.3.0/src/spice_rack/_logging/_sinks/_sys.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_misc/_empty.py` & `spice_rack-0.3.0/src/spice_rack/_misc/_empty.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.2.0/src/spice_rack/_timestamp/_fields.py` & `spice_rack-0.3.0/src/spice_rack/_ts_service/_fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import typing as t
 import pydantic
 
-from spice_rack._timestamp._timestamp import Timestamp
+from spice_rack._ts_service._timestamp import Timestamp
 
 
 __all__ = (
     "CreatedAtFieldAnn",
     "CreatedAtWithDefaultFieldAnn"
 )
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_timestamp/_timestamp.py` & `spice_rack-0.3.0/src/spice_rack/_ts_service/_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import typing as t
 import datetime as dt
 import dateparser
 import pydantic
 
-from spice_rack._timestamp._tz_key import TimeZoneKey
+from spice_rack._ts_service._tz_key import TimeZoneKey
 from spice_rack import _logging
 
 
 __all__ = (
     "Timestamp",
 )
 
@@ -32,29 +32,31 @@
 
     def to_dt_obj(
             self,
             with_tz: t.Optional[_TzKeyT] = None
     ) -> dt.datetime:
         res: dt.datetime
 
-        utc_dt_obj = dt.datetime.fromtimestamp(
-            self.to_python_timestamp(), tz=TimeZoneKey("UTC").as_zone_info()
-        )
         if with_tz:
+            utc_dt_obj = dt.datetime.fromtimestamp(
+                self.to_python_timestamp(), tz=TimeZoneKey("UTC").as_zone_info()
+            )
             tz_key: TimeZoneKey
             if with_tz == "local":
                 tz_key = TimeZoneKey.local()
             else:
                 tz_key = TimeZoneKey(str(with_tz))
 
             new_tz_info = tz_key.as_zone_info()
             obj_new_tz = utc_dt_obj.astimezone(tz=new_tz_info)
             res = obj_new_tz
         else:
-            res = utc_dt_obj
+            res = dt.datetime.fromtimestamp(
+                self.to_python_timestamp(), tz=None
+            )
         return res
 
     def to_iso_str(
             self,
             with_tz: t.Optional[_TzKeyT] = None
     ) -> str:
         """
@@ -93,14 +95,17 @@
         """
         dt_obj = self.to_dt_obj(with_tz=with_tz)
         return dt_obj.strftime(fmat)
 
     def special_repr(self, with_tz: t.Optional[_TzKeyT] = None) -> str:
         return f"{self.__class__.__name__}['{self.to_iso_str(with_tz=with_tz)}']"
 
+    def to_file_path_fmat(self) -> str:
+        return self.to_dt_obj().strftime("%Y_%m_%dT%H_%M_%S_%f")
+
     @classmethod
     def _from_datetime_obj(
             cls,
             value: dt.datetime,
             assumed_tz: TimeZoneKey
     ) -> int:
         tz_info: TimeZoneKey
```

### Comparing `spice_rack-0.2.0/src/spice_rack/_utils/_container_differ.py` & `spice_rack-0.3.0/src/spice_rack/_utils/_container_differ.py`

 * *Files identical despite different names*

