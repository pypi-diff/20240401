# Comparing `tmp/libdyson-neon-1.4.0.tar.gz` & `tmp/libdyson-neon-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdyson-neon-1.4.0.tar", last modified: Mon Apr  1 02:18:05 2024, max compression
+gzip compressed data, was "libdyson-neon-1.4.1.tar", last modified: Mon Apr  1 13:57:20 2024, max compression
```

## Comparing `libdyson-neon-1.4.0.tar` & `libdyson-neon-1.4.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:18:05.633252 libdyson-neon-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-01 02:18:05.633252 libdyson-neon-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:18:05.625252 libdyson-neon-1.4.0/libdyson/
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:18:05.625252 libdyson-neon-1.4.0/libdyson/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/cloud_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_360_vis_nav.py
--rw-r--r--   0 runner    (1001) docker     (127)    14714 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_pure_hot_cool.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_purifier_big_quiet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/dyson_vacuum_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/libdyson/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:18:05.625252 libdyson-neon-1.4.0/libdyson_neon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-01 02:18:05.000000 libdyson-neon-1.4.0/libdyson_neon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-01 02:18:05.000000 libdyson-neon-1.4.0/libdyson_neon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 02:18:05.000000 libdyson-neon-1.4.0/libdyson_neon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 02:18:05.000000 libdyson-neon-1.4.0/libdyson_neon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 02:18:05.000000 libdyson-neon-1.4.0/libdyson_neon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-01 02:18:05.633252 libdyson-neon-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:18:05.629253 libdyson-neon-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:18:05.633252 libdyson-neon-1.4.0/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/test_bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/test_cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/test_dyson_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/mocked_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_fan_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_heating_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_pure_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_pure_cool_missing_env_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_purifier_big_quiet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_purifier_humidify_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-01 02:17:57.000000 libdyson-neon-1.4.0/tests/test_vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:57:20.837917 libdyson-neon-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-01 13:57:20.837917 libdyson-neon-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:57:20.829917 libdyson-neon-1.4.1/libdyson/
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:57:20.833917 libdyson-neon-1.4.1/libdyson/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/cloud_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_360_vis_nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14714 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_pure_hot_cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_purifier_big_quiet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/dyson_vacuum_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/libdyson/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:57:20.833917 libdyson-neon-1.4.1/libdyson_neon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-01 13:57:20.000000 libdyson-neon-1.4.1/libdyson_neon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-01 13:57:20.000000 libdyson-neon-1.4.1/libdyson_neon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:57:20.000000 libdyson-neon-1.4.1/libdyson_neon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 13:57:20.000000 libdyson-neon-1.4.1/libdyson_neon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 13:57:20.000000 libdyson-neon-1.4.1/libdyson_neon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-01 13:57:20.837917 libdyson-neon-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:57:20.837917 libdyson-neon-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:57:20.837917 libdyson-neon-1.4.1/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/test_bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/test_cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/test_dyson_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/mocked_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_fan_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_heating_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_pure_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_pure_cool_missing_env_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_purifier_big_quiet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_purifier_humidify_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-01 13:57:10.000000 libdyson-neon-1.4.1/tests/test_vacuum.py
```

### Comparing `libdyson-neon-1.4.0/LICENSE` & `libdyson-neon-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/PKG-INFO` & `libdyson-neon-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-1.4.0/libdyson/__init__.py` & `libdyson-neon-1.4.1/libdyson/__init__.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/cloud/account.py` & `libdyson-neon-1.4.1/libdyson/cloud/account.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/cloud/cloud_360_eye.py` & `libdyson-neon-1.4.1/libdyson/cloud/cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/cloud/device_info.py` & `libdyson-neon-1.4.1/libdyson/cloud/device_info.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/cloud/regions.py` & `libdyson-neon-1.4.1/libdyson/cloud/regions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/cloud/utils.py` & `libdyson-neon-1.4.1/libdyson/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/const.py` & `libdyson-neon-1.4.1/libdyson/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 DEVICE_TYPE_PURIFIER_HOT_COOL_E = "527E"  # HP07 AND HP09
 DEVICE_TYPE_PURIFIER_HOT_COOL_K = "527K"  # HP07 AND HP09
 DEVICE_TYPE_PURIFIER_BIG_QUIET = "664"  # BP02, BP03, and BP04
 
 DEVICE_TYPE_NAMES = {
     DEVICE_TYPE_360_EYE: "360 Eye robot vacuum",
     DEVICE_TYPE_360_HEURIST: "360 Heurist robot vacuum",
+    DEVICE_TYPE_360_VIS_NAV: "360 Vis Nav robot vacuum",
     DEVICE_TYPE_PURE_COOL: "Pure Cool",
     DEVICE_TYPE_PURIFIER_COOL_K: "Purifier Cool",
     DEVICE_TYPE_PURIFIER_COOL_E: "Purifier Cool",
     DEVICE_TYPE_PURE_COOL_DESK: "Pure Cool Link Desk",
     DEVICE_TYPE_PURE_COOL_LINK: "Pure Cool Link",
     DEVICE_TYPE_PURE_COOL_LINK_DESK: "Pure Cool Link Desk",
     DEVICE_TYPE_PURE_HOT_COOL: "Pure Hot+Cool",
```

### Comparing `libdyson-neon-1.4.0/libdyson/discovery.py` & `libdyson-neon-1.4.1/libdyson/discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_360_eye.py` & `libdyson-neon-1.4.1/libdyson/dyson_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_360_heurist.py` & `libdyson-neon-1.4.1/libdyson/dyson_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_device.py` & `libdyson-neon-1.4.1/libdyson/dyson_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_pure_cool.py` & `libdyson-neon-1.4.1/libdyson/dyson_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_pure_cool_link.py` & `libdyson-neon-1.4.1/libdyson/dyson_pure_cool_link.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 from .const import AirQualityTarget
 from .dyson_device import DysonFanDevice
 
 
 class DysonPureCoolLink(DysonFanDevice):
     """Dyson Pure Cool Link device."""
 
+    def __init__(self, serial: str, credential: str, device_type: str):
+        super().__init__(serial, credential, device_type)
+        self.preset_mode = "FAN"
+
     @property
     def fan_mode(self) -> str:
         """Return the fan mode of the fan."""
         return self._get_field_value(self._status, "fmod")
 
     @property
     def is_on(self) -> bool:
         """Return if the device is on."""
         return self.fan_mode in ["FAN", "AUTO"]
 
     @property
     def auto_mode(self) -> bool:
         """Return auto mode status."""
-        return self.fan_mode == "AUTO"
+        if not self.is_on:
+            return self.preset_mode == "AUTO"
+        else:
+            self.preset_mode = self.fan_mode
+            return self.preset_mode == "AUTO"
 
     @property
     def oscillation(self) -> bool:
         """Return oscillation status."""
         return self._get_field_value(self._status, "oson") == "ON"
 
     @property
@@ -45,29 +53,31 @@
     @property
     def volatile_organic_compounds(self) -> int:
         """Return VOCs in unknown unit."""
         return self._get_environmental_field_value("vact")
 
     def turn_on(self) -> None:
         """Turn on the device."""
-        self._set_configuration(fmod="FAN")
+        self._set_configuration(fmod=self.preset_mode)
 
     def turn_off(self) -> None:
         """Turn off the device."""
         self._set_configuration(fmod="OFF")
 
     def _set_speed(self, speed: int) -> None:
         self._set_configuration(fmod="FAN", fnsp=f"{speed:04d}")
 
     def enable_auto_mode(self) -> None:
         """Turn on auto mode."""
+        self.preset_mode = "AUTO"
         self._set_configuration(fmod="AUTO")
 
     def disable_auto_mode(self) -> None:
         """Turn off auto mode."""
+        self.preset_mode = "FAN"
         self._set_configuration(fmod="FAN")
 
     def enable_oscillation(self) -> None:
         """Turn on oscillation."""
         self._set_configuration(oson="ON")
 
     def disable_oscillation(self) -> None:
```

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_pure_hot_cool_link.py` & `libdyson-neon-1.4.1/libdyson/dyson_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_pure_humidify_cool.py` & `libdyson-neon-1.4.1/libdyson/dyson_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_purifier_big_quiet.py` & `libdyson-neon-1.4.1/libdyson/dyson_purifier_big_quiet.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/dyson_vacuum_device.py` & `libdyson-neon-1.4.1/libdyson/dyson_vacuum_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/exceptions.py` & `libdyson-neon-1.4.1/libdyson/exceptions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson/utils.py` & `libdyson-neon-1.4.1/libdyson/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/libdyson_neon.egg-info/PKG-INFO` & `libdyson-neon-1.4.1/libdyson_neon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-1.4.0/libdyson_neon.egg-info/SOURCES.txt` & `libdyson-neon-1.4.1/libdyson_neon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/pyproject.toml` & `libdyson-neon-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/setup.cfg` & `libdyson-neon-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libdyson-neon
-version = 1.4.0
+version = 1.4.1
 author = The libdyson Working Group
 author_email = dotvezz@gmail.com
 license = MIT License
 license_file = LICENSE
 platforms = any
 description = A Python library for Dyson devices.
 long_description = file: README.md
```

### Comparing `libdyson-neon-1.4.0/tests/cloud/mocked_requests.py` & `libdyson-neon-1.4.1/tests/cloud/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/cloud/test_bearer_auth.py` & `libdyson-neon-1.4.1/tests/cloud/test_bearer_auth.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/cloud/test_cloud_360_eye.py` & `libdyson-neon-1.4.1/tests/cloud/test_cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/cloud/test_dyson_account.py` & `libdyson-neon-1.4.1/tests/cloud/test_dyson_account.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/cloud/utils.py` & `libdyson-neon-1.4.1/tests/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/conftest.py` & `libdyson-neon-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/mocked_mqtt.py` & `libdyson-neon-1.4.1/tests/mocked_mqtt.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_360_eye.py` & `libdyson-neon-1.4.1/tests/test_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_360_heurist.py` & `libdyson-neon-1.4.1/tests/test_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_device.py` & `libdyson-neon-1.4.1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_discovery.py` & `libdyson-neon-1.4.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_fan_device.py` & `libdyson-neon-1.4.1/tests/test_fan_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_heating_device.py` & `libdyson-neon-1.4.1/tests/test_heating_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_init.py` & `libdyson-neon-1.4.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_pure_cool.py` & `libdyson-neon-1.4.1/tests/test_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_pure_cool_formaldehyde.py` & `libdyson-neon-1.4.1/tests/test_pure_cool_formaldehyde.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_pure_cool_link.py` & `libdyson-neon-1.4.1/tests/test_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_pure_cool_missing_env_data.py` & `libdyson-neon-1.4.1/tests/test_pure_cool_missing_env_data.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_pure_hot_cool_link.py` & `libdyson-neon-1.4.1/tests/test_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_pure_humidify_cool.py` & `libdyson-neon-1.4.1/tests/test_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_purifier_big_quiet.py` & `libdyson-neon-1.4.1/tests/test_purifier_big_quiet.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_purifier_humidify_cool_formaldehyde.py` & `libdyson-neon-1.4.1/tests/test_purifier_humidify_cool_formaldehyde.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_utils.py` & `libdyson-neon-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.4.0/tests/test_vacuum.py` & `libdyson-neon-1.4.1/tests/test_vacuum.py`

 * *Files identical despite different names*

