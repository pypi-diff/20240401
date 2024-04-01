# Comparing `tmp/cloudquery-plugin-sdk-0.1.8.tar.gz` & `tmp/cloudquery-plugin-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-sdk-0.1.8.tar", last modified: Fri Nov 10 08:58:17 2023, max compression
+gzip compressed data, was "cloudquery-plugin-sdk-0.1.9.tar", last modified: Mon Dec 18 08:44:01 2023, max compression
```

## Comparing `cloudquery-plugin-sdk-0.1.8.tar` & `cloudquery-plugin-sdk-0.1.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.931194 cloudquery-plugin-sdk-0.1.8/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.931194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.931194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.931194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/memdb/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/memdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/memdb/memdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.931194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.931194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.935194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.935194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/message/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/message/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/message/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.935194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.935194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/date32.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/date64.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/int.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/scalar_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/uint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scheduler/table_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/column.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/serve/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/serve/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/transformers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/transformers/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/types/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/types/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/types/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 08:58:17.939194 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-11-10 08:58:17.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-11-10 08:58:17.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 08:58:17.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-10 08:58:17.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 08:57:59.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-11-10 08:58:17.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-10 08:58:17.000000 cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-10 08:58:17.943194 cloudquery-plugin-sdk-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2023-11-10 08:57:54.000000 cloudquery-plugin-sdk-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.650579 cloudquery-plugin-sdk-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-12-18 08:44:01.650579 cloudquery-plugin-sdk-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.638579 cloudquery-plugin-sdk-0.1.9/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/memdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/memdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/memdb/memdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/message/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/message/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.642579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.646579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/date32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/date64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/scalar_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/uint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.646579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scheduler/table_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.646579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.646579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/serve/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.646579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/transformers/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/transformers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.646579 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/types/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 08:44:01.650579 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-12-18 08:44:01.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-12-18 08:44:01.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 08:44:01.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-18 08:44:01.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 08:43:41.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-18 08:44:01.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-18 08:44:01.000000 cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-18 08:44:01.650579 cloudquery-plugin-sdk-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2023-12-18 08:43:34.000000 cloudquery-plugin-sdk-0.1.9/setup.py
```

### Comparing `cloudquery-plugin-sdk-0.1.8/PKG-INFO` & `cloudquery-plugin-sdk-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
@@ -16,32 +16,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Requires-Dist: cloudquery-plugin-pb==0.0.20
-Requires-Dist: exceptiongroup==1.1.3
-Requires-Dist: black==23.10.1
-Requires-Dist: grpcio==1.59.2
-Requires-Dist: grpcio-tools==1.59.2
+Requires-Dist: exceptiongroup==1.2.0
+Requires-Dist: black==23.12.0
+Requires-Dist: grpcio==1.60.0
+Requires-Dist: grpcio-tools==1.60.0
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: MarkupSafe==2.1.3
-Requires-Dist: numpy==1.26.1
+Requires-Dist: numpy==1.26.2
 Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.1.2
+Requires-Dist: pandas==2.1.4
 Requires-Dist: pluggy==1.3.0
-Requires-Dist: protobuf==4.24.4
+Requires-Dist: protobuf==4.25.1
 Requires-Dist: pyarrow==14.0.1
 Requires-Dist: pytest==7.4.3
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2023.3.post1
 Requires-Dist: six==1.16.0
-Requires-Dist: structlog==23.1.0
+Requires-Dist: structlog==23.2.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: tzdata==2023.3
 
 
 CloudQuery Plugin SDK for Python
 ================================================
```

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/internal/servers/plugin_v3/plugin.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/internal/servers/plugin_v3/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/message/write.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/message/write.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/binary.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/binary.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/bool.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/bool.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/date32.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/date32.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/date64.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/date64.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/float.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/float.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/int.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/int.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/json.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/json.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/list.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/list.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/scalar.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/scalar.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/scalar_factory.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/scalar_factory.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/string.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/string.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/timestamp.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/timestamp.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/uint.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/uint.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/uuid.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/uuid.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scalar/vector.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scalar/vector.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scheduler/scheduler.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/scheduler/table_resolver.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/scheduler/table_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/column.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/column.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/resource.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/resource.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/schema/table.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/schema/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,16 @@
     return filter_dfs_func(tables, include_func, exclude_func, skip_dependent_tables)
 
 
 def filter_dfs_func(tt: List[Table], include, exclude, skip_dependent_tables: bool):
     filtered_tables = []
     for t in tt:
         filtered_table = copy.deepcopy(t)
+        for r in filtered_table.relations:
+            r.parent = filtered_table
         filtered_table = _filter_dfs_impl(
             filtered_table, False, include, exclude, skip_dependent_tables
         )
         if filtered_table is not None:
             filtered_tables.append(filtered_table)
     return filtered_tables
```

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/transformers/openapi.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/transformers/openapi.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/types/json.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/types/json.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,12 +9,15 @@
         return JSONType, ()
 
     def __arrow_ext_serialize__(self):
         # since we don't have a parameterized type, we don't need extra
         # metadata to be deserialized
         return b"json-serialized"
 
+    def __str__(self):
+        return "json"
+
     @classmethod
     def __arrow_ext_deserialize__(self, storage_type, serialized):
         # return an instance of this subclass given the serialized
         # metadata.
         return JSONType()
```

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery/sdk/types/uuid.py` & `cloudquery-plugin-sdk-0.1.9/cloudquery/sdk/types/uuid.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,12 +11,15 @@
         return UUIDType, ()
 
     def __arrow_ext_serialize__(self):
         # since we don't have a parameterized type, we don't need extra
         # metadata to be deserialized
         return b"uuid-serialized"
 
+    def __str__(self):
+        return "uuid"
+
     @classmethod
     def __arrow_ext_deserialize__(self, storage_type, serialized):
         # return an instance of this subclass given the serialized
         # metadata.
         return UUIDType()
```

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/PKG-INFO` & `cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
@@ -16,32 +16,32 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Requires-Dist: cloudquery-plugin-pb==0.0.20
-Requires-Dist: exceptiongroup==1.1.3
-Requires-Dist: black==23.10.1
-Requires-Dist: grpcio==1.59.2
-Requires-Dist: grpcio-tools==1.59.2
+Requires-Dist: exceptiongroup==1.2.0
+Requires-Dist: black==23.12.0
+Requires-Dist: grpcio==1.60.0
+Requires-Dist: grpcio-tools==1.60.0
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: MarkupSafe==2.1.3
-Requires-Dist: numpy==1.26.1
+Requires-Dist: numpy==1.26.2
 Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.1.2
+Requires-Dist: pandas==2.1.4
 Requires-Dist: pluggy==1.3.0
-Requires-Dist: protobuf==4.24.4
+Requires-Dist: protobuf==4.25.1
 Requires-Dist: pyarrow==14.0.1
 Requires-Dist: pytest==7.4.3
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2023.3.post1
 Requires-Dist: six==1.16.0
-Requires-Dist: structlog==23.1.0
+Requires-Dist: structlog==23.2.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: tzdata==2023.3
 
 
 CloudQuery Plugin SDK for Python
 ================================================
```

### Comparing `cloudquery-plugin-sdk-0.1.8/cloudquery_plugin_sdk.egg-info/SOURCES.txt` & `cloudquery-plugin-sdk-0.1.9/cloudquery_plugin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.1.8/setup.py` & `cloudquery-plugin-sdk-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 
 name = "cloudquery-plugin-sdk"
 
 description = "CloudQuery Plugin SDK for Python"
 
 dependencies = [
     "cloudquery-plugin-pb==0.0.20",
-    "exceptiongroup==1.1.3",
-    "black==23.10.1",
-    "grpcio==1.59.2",
-    "grpcio-tools==1.59.2",
+    "exceptiongroup==1.2.0",
+    "black==23.12.0",
+    "grpcio==1.60.0",
+    "grpcio-tools==1.60.0",
     "iniconfig==2.0.0",
     "Jinja2==3.1.2",
     "MarkupSafe==2.1.3",
-    "numpy==1.26.1",
+    "numpy==1.26.2",
     "packaging==23.2",
-    "pandas==2.1.2",
+    "pandas==2.1.4",
     "pluggy==1.3.0",
-    "protobuf==4.24.4",
+    "protobuf==4.25.1",
     "pyarrow==14.0.1",
     "pytest==7.4.3",
     "python-dateutil==2.8.2",
     "pytz==2023.3.post1",
     "six==1.16.0",
-    "structlog==23.1.0",
+    "structlog==23.2.0",
     "tomli==2.0.1",
     "tzdata==2023.3",
 ]
 url = "https://github.com/cloudquery/plugin-sdk-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
@@ -49,15 +49,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.1.8",
+    version="0.1.9",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

