# Comparing `tmp/cassandra-medusa-0.9.0.tar.gz` & `tmp/cassandra-medusa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cassandra-medusa-0.9.0.tar", last modified: Wed Feb 24 11:58:01 2021, max compression
+gzip compressed data, was "dist/cassandra-medusa-0.9.1.tar", last modified: Tue Mar  9 16:53:28 2021, max compression
```

## Comparing `cassandra-medusa-0.9.0.tar` & `cassandra-medusa-0.9.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-24 11:58:00.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      490 2021-02-24 11:58:00.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-02-24 11:58:00.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1841 2021-02-24 11:58:00.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2535 2021-02-24 11:58:00.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-02-24 11:58:00.000000 cassandra-medusa-0.9.0/cassandra_medusa.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)      864 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/bin/medusa-wrapper
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)    14757 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/storage_test_with_prefix.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/tests/integration/features/
--rw-r--r--   0 runner    (1001) docker     (116)     1476 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/integration/features/environment.py
--rw-r--r--   0 runner    (1001) docker     (116)      594 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/integration/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/tests/integration/features/steps/
--rw-r--r--   0 runner    (1001) docker     (116)    44292 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/integration/features/steps/integration_steps.py
--rw-r--r--   0 runner    (1001) docker     (116)      594 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/integration/features/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      616 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1748 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     5474 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/filtering_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3185 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2383 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/backup_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1068 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3543 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/restore_node_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    16645 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/cassandra_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    14851 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    10177 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/restore_cluster_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      594 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5540 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/tests/purge_test.py
--rw-r--r--   0 runner    (1001) docker     (116)       41 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/
--rw-r--r--   0 runner    (1001) docker     (116)     3923 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/verify_restore.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/storage/
--rw-r--r--   0 runner    (1001) docker     (116)     4385 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/s3_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     9366 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/abstract_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2864 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/cluster_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/storage/azure_blobs_storage/
--rw-r--r--   0 runner    (1001) docker     (116)     8473 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/azure_blobs_storage/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/azure_blobs_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4603 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/azure_blobs_storage/azcli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/storage/google_cloud_storage/
--rw-r--r--   0 runner    (1001) docker     (116)     5127 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/google_cloud_storage/gsutil.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/google_cloud_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6725 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (116)     6451 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/google_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2471 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/s3_rgw.py
--rw-r--r--   0 runner    (1001) docker     (116)     5073 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2503 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     7428 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/s3_base_storage.py
--rw-r--r--   0 runner    (1001) docker     (116)     8154 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/node_backup.py
--rw-r--r--   0 runner    (1001) docker     (116)    18711 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/storage/s3_compat_storage/
--rw-r--r--   0 runner    (1001) docker     (116)     8290 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/s3_compat_storage/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (116)     5816 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/s3_compat_storage/awscli.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/storage/s3_compat_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7814 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/backup_cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)     3388 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/download.py
--rw-r--r--   0 runner    (1001) docker     (116)    28227 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/cassandra_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     7497 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/purge.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/libcloud/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/libcloud/storage/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/libcloud/storage/drivers/
--rw-r--r--   0 runner    (1001) docker     (116)    10412 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/libcloud/storage/drivers/ibm.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/libcloud/storage/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/libcloud/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/libcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    19530 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/restore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)     7881 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/report_latest.py
--rw-r--r--   0 runner    (1001) docker     (116)     1437 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1002 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/fetch_tokenmap.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/monitoring/
--rw-r--r--   0 runner    (1001) docker     (116)     1544 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/monitoring/local.py
--rw-r--r--   0 runner    (1001) docker     (116)     1747 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/monitoring/ffwd.py
--rw-r--r--   0 runner    (1001) docker     (116)      832 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/monitoring/noop.py
--rw-r--r--   0 runner    (1001) docker     (116)      813 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/monitoring/abstract.py
--rw-r--r--   0 runner    (1001) docker     (116)     1713 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2608 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     3709 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/verify.py
--rw-r--r--   0 runner    (1001) docker     (116)     2092 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/filtering.py
--rw-r--r--   0 runner    (1001) docker     (116)     8152 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    15483 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/restore_node.py
--rw-r--r--   0 runner    (1001) docker     (116)    14800 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/backup_node.py
--rw-r--r--   0 runner    (1001) docker     (116)     2323 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     2139 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/listing.py
--rw-r--r--   0 runner    (1001) docker     (116)     3909 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/orchestration.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/network/
--rw-r--r--   0 runner    (1001) docker     (116)     1133 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/network/hostname_resolver.py
--rw-r--r--   0 runner    (1001) docker     (116)      597 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      616 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13711 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/medusacli.py
--rw-r--r--   0 runner    (1001) docker     (116)     5647 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/index.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/service/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/medusa/service/grpc/
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/grpc/restore.py
--rw-r--r--   0 runner    (1001) docker     (116)     6123 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (116)     7164 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/grpc/medusa_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (116)     2321 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (116)    17862 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/grpc/medusa_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)      620 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      620 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      956 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1841 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/medusa-example.ini
--rw-r--r--   0 runner    (1001) docker     (116)       52 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-24 11:58:01.000000 cassandra-medusa-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2581 2021-02-24 11:57:47.000000 cassandra-medusa-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-09 16:53:27.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      490 2021-03-09 16:53:27.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2021-03-09 16:53:27.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1841 2021-03-09 16:53:27.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2546 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-09 16:53:27.000000 cassandra-medusa-0.9.1/cassandra_medusa.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (116)      864 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/bin/medusa-wrapper
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)    14757 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/storage_test_with_prefix.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/tests/integration/features/
+-rw-r--r--   0 runner    (1001) docker     (116)     1476 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/integration/features/environment.py
+-rw-r--r--   0 runner    (1001) docker     (116)      594 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/integration/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/tests/integration/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (116)    44914 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/integration/features/steps/integration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (116)      594 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/integration/features/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      616 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1748 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5474 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/filtering_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3185 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2383 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/backup_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1068 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3543 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/restore_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16645 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/cassandra_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14851 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10177 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/restore_cluster_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      594 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5540 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/tests/purge_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)       41 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/
+-rw-r--r--   0 runner    (1001) docker     (116)     3923 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/verify_restore.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/storage/
+-rw-r--r--   0 runner    (1001) docker     (116)     4385 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/s3_storage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9366 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/abstract_storage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2864 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/cluster_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/storage/azure_blobs_storage/
+-rw-r--r--   0 runner    (1001) docker     (116)     8473 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/azure_blobs_storage/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/azure_blobs_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4603 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/azure_blobs_storage/azcli.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/storage/google_cloud_storage/
+-rw-r--r--   0 runner    (1001) docker     (116)     5127 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/google_cloud_storage/gsutil.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/google_cloud_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6725 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6451 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/google_storage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2471 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/s3_rgw.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5073 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2503 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7485 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/s3_base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8154 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/node_backup.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18711 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/storage/s3_compat_storage/
+-rw-r--r--   0 runner    (1001) docker     (116)     8290 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/s3_compat_storage/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5865 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/s3_compat_storage/awscli.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/storage/s3_compat_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7814 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/backup_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3388 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/download.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28227 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/cassandra_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7497 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/purge.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/libcloud/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/libcloud/storage/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/libcloud/storage/drivers/
+-rw-r--r--   0 runner    (1001) docker     (116)     2857 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/libcloud/storage/drivers/s3_base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/libcloud/storage/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/libcloud/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/libcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19530 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/restore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7881 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/report_latest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1437 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1002 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/fetch_tokenmap.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (116)     1544 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/monitoring/local.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1747 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/monitoring/ffwd.py
+-rw-r--r--   0 runner    (1001) docker     (116)      832 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/monitoring/noop.py
+-rw-r--r--   0 runner    (1001) docker     (116)      813 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/monitoring/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1713 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2608 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/schema.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3709 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/verify.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2092 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8152 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15483 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/restore_node.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14800 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/backup_node.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2323 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2139 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/listing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3909 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/orchestration.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/network/
+-rw-r--r--   0 runner    (1001) docker     (116)     1133 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/network/hostname_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (116)      597 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      616 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13711 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/medusacli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5647 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/index.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/service/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/medusa/service/grpc/
+-rw-r--r--   0 runner    (1001) docker     (116)     2303 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/grpc/restore.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6123 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7164 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/grpc/medusa_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2321 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17862 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/grpc/medusa_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (116)      620 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      620 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      956 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1841 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/medusa-example.ini
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-09 16:53:28.000000 cassandra-medusa-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2581 2021-03-09 16:53:13.000000 cassandra-medusa-0.9.1/setup.py
```

### Comparing `cassandra-medusa-0.9.0/LICENSE` & `cassandra-medusa-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/cassandra_medusa.egg-info/PKG-INFO` & `cassandra-medusa-0.9.1/cassandra_medusa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassandra-medusa
-Version: 0.9.0
+Version: 0.9.1
 Summary: Apache Cassandra backup and restore tool
 Home-page: https://github.com/thelastpickle/cassandra-medusa
 Author: The Last Pickle
 Author-email: medusa@thelastpickle.com
 License: Apache
 Description: <!--
         # Copyright 2019 Spotify AB. All rights reserved.
@@ -32,10 +32,10 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Archiving :: Backup
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Provides-Extra: AZURE
 Provides-Extra: S3
+Provides-Extra: AZURE
 Provides-Extra: GCS
```

### Comparing `cassandra-medusa-0.9.0/cassandra_medusa.egg-info/SOURCES.txt` & `cassandra-medusa-0.9.1/cassandra_medusa.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 medusa/status.py
 medusa/utils.py
 medusa/verify.py
 medusa/verify_restore.py
 medusa/libcloud/__init__.py
 medusa/libcloud/storage/__init__.py
 medusa/libcloud/storage/drivers/__init__.py
-medusa/libcloud/storage/drivers/ibm.py
+medusa/libcloud/storage/drivers/s3_base_driver.py
 medusa/monitoring/__init__.py
 medusa/monitoring/abstract.py
 medusa/monitoring/ffwd.py
 medusa/monitoring/local.py
 medusa/monitoring/noop.py
 medusa/network/__init__.py
 medusa/network/hostname_resolver.py
```

### Comparing `cassandra-medusa-0.9.0/bin/medusa-wrapper` & `cassandra-medusa-0.9.1/bin/medusa-wrapper`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/storage_test_with_prefix.py` & `cassandra-medusa-0.9.1/tests/storage_test_with_prefix.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/integration/features/environment.py` & `cassandra-medusa-0.9.1/tests/integration/features/environment.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/integration/features/__init__.py` & `cassandra-medusa-0.9.1/tests/integration/features/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/integration/features/steps/integration_steps.py` & `cassandra-medusa-0.9.1/tests/integration/features/steps/integration_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             "api_key_or_username": "",
             "api_secret_or_password": "",
             "base_path": "/tmp",
             "concurrent_transfers": 4,
             "multi_part_upload_threshold": 1 * 1024,
             "prefix": storage_prefix
         }
-    elif storage_provider.startswith("s3"):
+    elif storage_provider == "s3_us_west_oregon":
         config["storage"] = {
             "host_file_separator": ",",
             "bucket_name": "tlp-medusa-dev",
             "key_file": "~/.aws/credentials",
             "storage_provider": storage_provider,
             "fqdn": "127.0.0.1",
             "api_key_or_username": "",
@@ -290,14 +290,31 @@
             "api_profile": "default",
             "base_path": "/tmp",
             "multi_part_upload_threshold": 1 * 1024,
             "concurrent_transfers": 4,
             "prefix": storage_prefix,
             "aws_cli_path": "aws"
         }
+    elif storage_provider == "minio":
+        config["storage"] = {
+            "host_file_separator": ",",
+            "bucket_name": "medusa-dev",
+            "key_file": "~/.aws/minio_credentials",
+            "storage_provider": "s3_compatible",
+            "fqdn": "127.0.0.1",
+            "api_profile": "default",
+            "base_path": "/tmp",
+            "multi_part_upload_threshold": 1 * 1024,
+            "concurrent_transfers": 1,
+            "prefix": storage_prefix,
+            "aws_cli_path": "aws",
+            "host": "localhost",
+            "port": 9000,
+            "secure": False
+        }
     elif storage_provider.startswith("ibm"):
         config["storage"] = {
             "host_file_separator": ",",
             "bucket_name": "medusa-experiment-2",
             "key_file": "~/.aws/ibm_credentials",
             "storage_provider": storage_provider,
             "fqdn": "127.0.0.1",
```

### Comparing `cassandra-medusa-0.9.0/tests/integration/features/steps/__init__.py` & `cassandra-medusa-0.9.1/tests/integration/features/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/integration/__init__.py` & `cassandra-medusa-0.9.1/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/config_test.py` & `cassandra-medusa-0.9.1/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/filtering_test.py` & `cassandra-medusa-0.9.1/tests/filtering_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/schema_test.py` & `cassandra-medusa-0.9.1/tests/schema_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/backup_test.py` & `cassandra-medusa-0.9.1/tests/backup_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/utils_test.py` & `cassandra-medusa-0.9.1/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/restore_node_test.py` & `cassandra-medusa-0.9.1/tests/restore_node_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/cassandra_utils_test.py` & `cassandra-medusa-0.9.1/tests/cassandra_utils_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/storage_test.py` & `cassandra-medusa-0.9.1/tests/storage_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/restore_cluster_test.py` & `cassandra-medusa-0.9.1/tests/restore_cluster_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/__init__.py` & `cassandra-medusa-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/tests/purge_test.py` & `cassandra-medusa-0.9.1/tests/purge_test.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/verify_restore.py` & `cassandra-medusa-0.9.1/medusa/verify_restore.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/s3_storage.py` & `cassandra-medusa-0.9.1/medusa/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/abstract_storage.py` & `cassandra-medusa-0.9.1/medusa/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/cluster_backup.py` & `cassandra-medusa-0.9.1/medusa/storage/cluster_backup.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/azure_blobs_storage/concurrent.py` & `cassandra-medusa-0.9.1/medusa/storage/azure_blobs_storage/concurrent.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/azure_blobs_storage/azcli.py` & `cassandra-medusa-0.9.1/medusa/storage/azure_blobs_storage/azcli.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/google_cloud_storage/gsutil.py` & `cassandra-medusa-0.9.1/medusa/storage/google_cloud_storage/gsutil.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/concurrent.py` & `cassandra-medusa-0.9.1/medusa/storage/concurrent.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/google_storage.py` & `cassandra-medusa-0.9.1/medusa/storage/google_storage.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/s3_rgw.py` & `cassandra-medusa-0.9.1/medusa/storage/s3_rgw.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/azure_storage.py` & `cassandra-medusa-0.9.1/medusa/storage/azure_storage.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/local_storage.py` & `cassandra-medusa-0.9.1/medusa/storage/local_storage.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/s3_base_storage.py` & `cassandra-medusa-0.9.1/medusa/storage/s3_base_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import itertools
 import subprocess
 import configparser
 from subprocess import PIPE
 from dateutil import parser
 from pathlib import Path
 
-from libcloud.storage.drivers.minio import MinIOStorageDriver
+from medusa.libcloud.storage.drivers.s3_base_driver import S3BaseStorageDriver
 
 from medusa.storage.abstract_storage import AbstractStorage
 import medusa.storage.s3_compat_storage.concurrent
 from medusa.storage.s3_compat_storage.awscli import AwsCli
 
 import medusa
 
@@ -62,20 +62,21 @@
                 aws_secret_access_key = profile['aws_secret_access_key']
 
         if aws_access_key_id is None:
             raise NotImplementedError("No valid access key defined.")
 
         # MinIOStorageDriver is the only clean implementation of BaseS3StorageDriver in libcloud
         secure = False if self.config.secure is None or self.config.secure.lower() in ('0', 'false') else True
-        driver = MinIOStorageDriver(
+        driver = S3BaseStorageDriver(
             host=self.config.host,
             port=self.config.port,
             key=aws_access_key_id,
             secret=aws_secret_access_key,
-            secure=secure
+            secure=secure,
+            region=self.config.region
         )
 
         return driver
 
     def check_dependencies(self):
         if self.config.aws_cli_path == 'dynamic':
             aws_cli_path = AwsCli.find_aws_cli()
```

### Comparing `cassandra-medusa-0.9.0/medusa/storage/node_backup.py` & `cassandra-medusa-0.9.1/medusa/storage/node_backup.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/__init__.py` & `cassandra-medusa-0.9.1/medusa/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/s3_compat_storage/concurrent.py` & `cassandra-medusa-0.9.1/medusa/storage/s3_compat_storage/concurrent.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/storage/s3_compat_storage/awscli.py` & `cassandra-medusa-0.9.1/medusa/storage/s3_compat_storage/awscli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import subprocess
 import uuid
 import sys
 
 from retrying import retry
 
 from libcloud.storage.providers import get_driver, Provider
+from medusa import utils
 
 
 class AwsCli(object):
     def __init__(self, storage):
         self._config = storage.config
         self.storage = storage
 
@@ -45,15 +46,15 @@
         else:
             self._aws_cli_path = self._config.aws_cli_path
 
         self.endpoint_url = None
         if self._config.host is not None:
             self.endpoint_url = '{}:{}'.format(self._config.host, self._config.port) \
                 if self._config.port is not None else self._config.host
-            if self._config.secure:
+            if utils.evaluate_boolean(self._config.secure):
                 self.endpoint_url = 'https://{}'.format(self.endpoint_url)
             else:
                 self.endpoint_url = 'http://{}'.format(self.endpoint_url)
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `cassandra-medusa-0.9.0/medusa/backup_cluster.py` & `cassandra-medusa-0.9.1/medusa/backup_cluster.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/download.py` & `cassandra-medusa-0.9.1/medusa/download.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/cassandra_utils.py` & `cassandra-medusa-0.9.1/medusa/cassandra_utils.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/purge.py` & `cassandra-medusa-0.9.1/medusa/purge.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/restore_cluster.py` & `cassandra-medusa-0.9.1/medusa/restore_cluster.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/report_latest.py` & `cassandra-medusa-0.9.1/medusa/report_latest.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/utils.py` & `cassandra-medusa-0.9.1/medusa/utils.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/fetch_tokenmap.py` & `cassandra-medusa-0.9.1/medusa/fetch_tokenmap.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/monitoring/local.py` & `cassandra-medusa-0.9.1/medusa/monitoring/local.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/monitoring/ffwd.py` & `cassandra-medusa-0.9.1/medusa/monitoring/ffwd.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/monitoring/noop.py` & `cassandra-medusa-0.9.1/medusa/monitoring/noop.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/monitoring/abstract.py` & `cassandra-medusa-0.9.1/medusa/monitoring/abstract.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/monitoring/__init__.py` & `cassandra-medusa-0.9.1/medusa/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/schema.py` & `cassandra-medusa-0.9.1/medusa/schema.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/verify.py` & `cassandra-medusa-0.9.1/medusa/verify.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/filtering.py` & `cassandra-medusa-0.9.1/medusa/filtering.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/config.py` & `cassandra-medusa-0.9.1/medusa/config.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/restore_node.py` & `cassandra-medusa-0.9.1/medusa/restore_node.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/backup_node.py` & `cassandra-medusa-0.9.1/medusa/backup_node.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/status.py` & `cassandra-medusa-0.9.1/medusa/status.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/listing.py` & `cassandra-medusa-0.9.1/medusa/listing.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/orchestration.py` & `cassandra-medusa-0.9.1/medusa/orchestration.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/network/hostname_resolver.py` & `cassandra-medusa-0.9.1/medusa/network/hostname_resolver.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/network/__init__.py` & `cassandra-medusa-0.9.1/medusa/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/__init__.py` & `cassandra-medusa-0.9.1/medusa/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/medusacli.py` & `cassandra-medusa-0.9.1/medusa/medusacli.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/index.py` & `cassandra-medusa-0.9.1/medusa/index.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/grpc/restore.py` & `cassandra-medusa-0.9.1/medusa/service/grpc/restore.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/grpc/server.py` & `cassandra-medusa-0.9.1/medusa/service/grpc/server.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/grpc/medusa_pb2_grpc.py` & `cassandra-medusa-0.9.1/medusa/service/grpc/medusa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/grpc/client.py` & `cassandra-medusa-0.9.1/medusa/service/grpc/client.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/grpc/medusa_pb2.py` & `cassandra-medusa-0.9.1/medusa/service/grpc/medusa_pb2.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/grpc/__init__.py` & `cassandra-medusa-0.9.1/medusa/service/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/medusa/service/__init__.py` & `cassandra-medusa-0.9.1/medusa/service/__init__.py`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/README.md` & `cassandra-medusa-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/PKG-INFO` & `cassandra-medusa-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassandra-medusa
-Version: 0.9.0
+Version: 0.9.1
 Summary: Apache Cassandra backup and restore tool
 Home-page: https://github.com/thelastpickle/cassandra-medusa
 Author: The Last Pickle
 Author-email: medusa@thelastpickle.com
 License: Apache
 Description: <!--
         # Copyright 2019 Spotify AB. All rights reserved.
@@ -32,10 +32,10 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Archiving :: Backup
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Provides-Extra: AZURE
 Provides-Extra: S3
+Provides-Extra: AZURE
 Provides-Extra: GCS
```

### Comparing `cassandra-medusa-0.9.0/medusa-example.ini` & `cassandra-medusa-0.9.1/medusa-example.ini`

 * *Files identical despite different names*

### Comparing `cassandra-medusa-0.9.0/setup.py` & `cassandra-medusa-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cassandra-medusa',
-    version='0.9.0',
+    version='0.9.1',
     author='The Last Pickle',
     author_email='medusa@thelastpickle.com',
     url='https://github.com/thelastpickle/cassandra-medusa',
     description='Apache Cassandra backup and restore tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache',
```

