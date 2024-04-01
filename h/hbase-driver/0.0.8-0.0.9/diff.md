# Comparing `tmp/hbase-driver-0.0.8.tar.gz` & `tmp/hbase-driver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbase-driver-0.0.8.tar", last modified: Wed Feb 21 14:13:09 2024, max compression
+gzip compressed data, was "hbase-driver-0.0.9.tar", last modified: Wed Feb 21 14:14:48 2024, max compression
```

## Comparing `hbase-driver-0.0.8.tar` & `hbase-driver-0.0.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.872768 hbase-driver-0.0.8/
--rw-r--r--   0 jeffzhong   (501) staff       (20)    11324 2024-02-09 09:08:07.000000 hbase-driver-0.0.8/LICENSE
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1205 2024-02-21 14:13:09.872460 hbase-driver-0.0.8/PKG-INFO
--rw-r--r--   0 jeffzhong   (501) staff       (20)      920 2024-02-16 11:21:47.000000 hbase-driver-0.0.8/README.md
--rw-r--r--   0 jeffzhong   (501) staff       (20)      515 2024-02-21 14:13:03.000000 hbase-driver-0.0.8/pyproject.toml
--rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-21 14:13:09.872822 hbase-driver-0.0.8/setup.cfg
--rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-15 05:54:23.000000 hbase-driver-0.0.8/setup.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.846463 hbase-driver-0.0.8/src/
--rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:50.000000 hbase-driver-0.0.8/src/__init__.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.872192 hbase-driver-0.0.8/src/hbase_driver.egg-info/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1205 2024-02-21 14:13:09.000000 hbase-driver-0.0.8/src/hbase_driver.egg-info/PKG-INFO
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4590 2024-02-21 14:13:09.000000 hbase-driver-0.0.8/src/hbase_driver.egg-info/SOURCES.txt
--rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-21 14:13:09.000000 hbase-driver-0.0.8/src/hbase_driver.egg-info/dependency_links.txt
--rw-r--r--   0 jeffzhong   (501) staff       (20)        6 2024-02-21 14:13:09.000000 hbase-driver-0.0.8/src/hbase_driver.egg-info/requires.txt
--rw-r--r--   0 jeffzhong   (501) staff       (20)       12 2024-02-21 14:13:09.000000 hbase-driver-0.0.8/src/hbase_driver.egg-info/top_level.txt
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.849990 hbase-driver-0.0.8/src/hbasedriver/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     5564 2024-02-18 12:15:14.000000 hbase-driver-0.0.8/src/hbasedriver/Connection.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:42.000000 hbase-driver-0.0.8/src/hbasedriver/__init__.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.850690 hbase-driver-0.0.8/src/hbasedriver/client/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       27 2024-02-13 10:52:12.000000 hbase-driver-0.0.8/src/hbasedriver/client/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      875 2024-02-15 04:35:33.000000 hbase-driver-0.0.8/src/hbasedriver/client/client.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2549 2024-02-18 12:42:23.000000 hbase-driver-0.0.8/src/hbasedriver/client/table.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.851121 hbase-driver-0.0.8/src/hbasedriver/exceptions/
--rw-r--r--   0 jeffzhong   (501) staff       (20)      208 2024-02-13 11:06:09.000000 hbase-driver-0.0.8/src/hbasedriver/exceptions/RemoteException.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-15 04:48:34.000000 hbase-driver-0.0.8/src/hbasedriver/exceptions/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-18 12:14:57.000000 hbase-driver-0.0.8/src/hbasedriver/master.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1092 2024-02-18 12:50:33.000000 hbase-driver-0.0.8/src/hbasedriver/meta_server.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.851753 hbase-driver-0.0.8/src/hbasedriver/model/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       39 2024-02-15 09:44:07.000000 hbase-driver-0.0.8/src/hbasedriver/model/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      560 2024-02-16 06:16:01.000000 hbase-driver-0.0.8/src/hbasedriver/model/cell.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1076 2024-02-21 14:09:31.000000 hbase-driver-0.0.8/src/hbasedriver/model/row.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.853113 hbase-driver-0.0.8/src/hbasedriver/operations/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       60 2024-02-15 09:36:12.000000 hbase-driver-0.0.8/src/hbasedriver/operations/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1403 2024-02-16 06:24:06.000000 hbase-driver-0.0.8/src/hbasedriver/operations/delete.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      579 2024-02-15 09:10:08.000000 hbase-driver-0.0.8/src/hbasedriver/operations/get.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      565 2024-02-16 11:15:48.000000 hbase-driver-0.0.8/src/hbasedriver/operations/put.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1651 2024-02-21 14:05:47.000000 hbase-driver-0.0.8/src/hbasedriver/operations/scan.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.868935 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6557 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/AccessControl_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     7736 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    16699 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Admin_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    18884 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Admin_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3927 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4557 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2239 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Cell_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2408 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Cell_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    18228 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Client_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    28375 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Client_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1271 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterId_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      408 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterId_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    10609 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    20630 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3727 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Comparator_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3765 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Comparator_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1474 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Encryption_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      896 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Encryption_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1942 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1671 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/FS_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1057 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/FS_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     8649 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Filter_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    11171 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Filter_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     9434 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HBase_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    13837 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HBase_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2376 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HFile_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3041 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HFile_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1317 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      411 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LoadBalancer_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4388 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LockService_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     5485 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LockService_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1666 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MapReduce_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1232 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    32135 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    51191 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    52933 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Master_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    51311 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Master_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4819 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Procedure_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6880 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Procedure_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     7707 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Quota_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     9897 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Quota_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3846 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RPC_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     5095 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RPC_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1770 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RecentLogs_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1663 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1327 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      423 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     8348 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     9133 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4569 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Registry_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2771 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Registry_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6353 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Replication_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     7628 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Replication_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1345 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      466 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3910 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Snapshot_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4966 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1597 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1009 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1321 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TestProcedure_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      420 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TestProcedure_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2142 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2530 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2052 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Tracing_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1028 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Tracing_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6485 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/WAL_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    10882 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/WAL_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3168 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3381 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)      180 2024-02-15 08:37:54.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2070 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1164 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1837 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      164 2024-02-15 05:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_rpc_service_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1290 2024-02-15 09:13:14.000000 hbase-driver-0.0.8/src/hbasedriver/region.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6655 2024-02-21 14:08:38.000000 hbase-driver-0.0.8/src/hbasedriver/regionserver.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-10 15:01:32.000000 hbase-driver-0.0.8/src/hbasedriver/request.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      190 2024-02-15 04:47:05.000000 hbase-driver-0.0.8/src/hbasedriver/response.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.869742 hbase-driver-0.0.8/src/hbasedriver/util/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       22 2024-02-15 04:36:36.000000 hbase-driver-0.0.8/src/hbasedriver/util/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      211 2024-02-13 07:51:10.000000 hbase-driver-0.0.8/src/hbasedriver/util/bytes.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6044 2024-02-10 15:46:22.000000 hbase-driver-0.0.8/src/hbasedriver/util/varint.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3516 2024-02-15 04:47:30.000000 hbase-driver-0.0.8/src/hbasedriver/zk.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:13:09.871772 hbase-driver-0.0.8/test/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2024 2024-02-16 12:08:09.000000 hbase-driver-0.0.8/test/test_client.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      809 2024-02-15 09:31:21.000000 hbase-driver-0.0.8/test/test_master.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      444 2024-02-15 03:30:47.000000 hbase-driver-0.0.8/test/test_rs.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      853 2024-02-21 14:12:27.000000 hbase-driver-0.0.8/test/test_scan.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      207 2024-02-13 09:42:21.000000 hbase-driver-0.0.8/test/test_zk.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.457484 hbase-driver-0.0.9/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    11324 2024-02-09 09:08:07.000000 hbase-driver-0.0.9/LICENSE
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1239 2024-02-21 14:14:48.457263 hbase-driver-0.0.9/PKG-INFO
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      954 2024-02-21 14:14:33.000000 hbase-driver-0.0.9/README.md
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      515 2024-02-21 14:14:41.000000 hbase-driver-0.0.9/pyproject.toml
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-21 14:14:48.457526 hbase-driver-0.0.9/setup.cfg
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-15 05:54:23.000000 hbase-driver-0.0.9/setup.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.431149 hbase-driver-0.0.9/src/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:50.000000 hbase-driver-0.0.9/src/__init__.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.457007 hbase-driver-0.0.9/src/hbase_driver.egg-info/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1239 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/PKG-INFO
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4590 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        6 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/requires.txt
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       12 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/top_level.txt
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.434751 hbase-driver-0.0.9/src/hbasedriver/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     5564 2024-02-18 12:15:14.000000 hbase-driver-0.0.9/src/hbasedriver/Connection.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:42.000000 hbase-driver-0.0.9/src/hbasedriver/__init__.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.435557 hbase-driver-0.0.9/src/hbasedriver/client/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       27 2024-02-13 10:52:12.000000 hbase-driver-0.0.9/src/hbasedriver/client/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      875 2024-02-15 04:35:33.000000 hbase-driver-0.0.9/src/hbasedriver/client/client.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2549 2024-02-18 12:42:23.000000 hbase-driver-0.0.9/src/hbasedriver/client/table.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.436005 hbase-driver-0.0.9/src/hbasedriver/exceptions/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      208 2024-02-13 11:06:09.000000 hbase-driver-0.0.9/src/hbasedriver/exceptions/RemoteException.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-15 04:48:34.000000 hbase-driver-0.0.9/src/hbasedriver/exceptions/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-18 12:14:57.000000 hbase-driver-0.0.9/src/hbasedriver/master.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1092 2024-02-18 12:50:33.000000 hbase-driver-0.0.9/src/hbasedriver/meta_server.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.436806 hbase-driver-0.0.9/src/hbasedriver/model/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       39 2024-02-15 09:44:07.000000 hbase-driver-0.0.9/src/hbasedriver/model/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      560 2024-02-16 06:16:01.000000 hbase-driver-0.0.9/src/hbasedriver/model/cell.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1076 2024-02-21 14:09:31.000000 hbase-driver-0.0.9/src/hbasedriver/model/row.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.438344 hbase-driver-0.0.9/src/hbasedriver/operations/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       60 2024-02-15 09:36:12.000000 hbase-driver-0.0.9/src/hbasedriver/operations/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1403 2024-02-16 06:24:06.000000 hbase-driver-0.0.9/src/hbasedriver/operations/delete.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      579 2024-02-15 09:10:08.000000 hbase-driver-0.0.9/src/hbasedriver/operations/get.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      565 2024-02-16 11:15:48.000000 hbase-driver-0.0.9/src/hbasedriver/operations/put.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1651 2024-02-21 14:05:47.000000 hbase-driver-0.0.9/src/hbasedriver/operations/scan.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.454191 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6557 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     7736 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    16699 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    18884 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3927 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4557 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2239 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2408 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    18228 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    28375 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1271 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterId_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      408 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterId_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    10609 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    20630 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3727 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3765 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1474 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      896 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1942 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1671 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1057 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     8649 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    11171 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     9434 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    13837 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2376 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3041 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1317 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      411 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LoadBalancer_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4388 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     5485 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1666 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1232 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    32135 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    51191 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    52933 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    51311 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4819 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6880 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     7707 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     9897 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3846 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     5095 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1770 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1663 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1327 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      423 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     8348 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     9133 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4569 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2771 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6353 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     7628 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1345 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      466 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3910 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4966 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1597 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1009 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1321 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TestProcedure_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      420 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TestProcedure_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2142 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2530 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2052 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1028 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6485 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    10882 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3168 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3381 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      180 2024-02-15 08:37:54.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2070 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1164 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1837 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      164 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_rpc_service_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1290 2024-02-15 09:13:14.000000 hbase-driver-0.0.9/src/hbasedriver/region.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6655 2024-02-21 14:08:38.000000 hbase-driver-0.0.9/src/hbasedriver/regionserver.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-10 15:01:32.000000 hbase-driver-0.0.9/src/hbasedriver/request.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      190 2024-02-15 04:47:05.000000 hbase-driver-0.0.9/src/hbasedriver/response.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.454974 hbase-driver-0.0.9/src/hbasedriver/util/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       22 2024-02-15 04:36:36.000000 hbase-driver-0.0.9/src/hbasedriver/util/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      211 2024-02-13 07:51:10.000000 hbase-driver-0.0.9/src/hbasedriver/util/bytes.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6044 2024-02-10 15:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/util/varint.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3516 2024-02-15 04:47:30.000000 hbase-driver-0.0.9/src/hbasedriver/zk.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.456544 hbase-driver-0.0.9/test/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2024 2024-02-16 12:08:09.000000 hbase-driver-0.0.9/test/test_client.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      809 2024-02-15 09:31:21.000000 hbase-driver-0.0.9/test/test_master.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      444 2024-02-15 03:30:47.000000 hbase-driver-0.0.9/test/test_rs.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      853 2024-02-21 14:12:27.000000 hbase-driver-0.0.9/test/test_scan.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      207 2024-02-13 09:42:21.000000 hbase-driver-0.0.9/test/test_zk.py
```

### Comparing `hbase-driver-0.0.8/LICENSE` & `hbase-driver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/PKG-INFO` & `hbase-driver-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: hbase-driver
-Version: 0.0.8
-Project-URL: Homepage, https://github.com/innovationb1ue/hbase-driver
-Project-URL: Issues, https://github.com/innovationb1ue/hbase-driver/issues
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: kazoo
-
 # hbase-driver
 
 Native Hbase driver in Python. (No thrift)
 
 ### Introduction
 
 - written in pure Python
@@ -45,12 +36,13 @@
 
 ### Implemented
 
 - Create, Disable, Delete table
 - Put
 - Get
 - DELETE
+- Scan
 
 ### TODOs
 
-- Scan
 - Filters
+- More params in the operations.
```

### Comparing `hbase-driver-0.0.8/pyproject.toml` & `hbase-driver-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'hbase-driver'
-version = "0.0.8"
+version = "0.0.9"
 readme = "README.md"
 dependencies = ['kazoo']
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 packages = ["hbasedriver", "hbasedriver.protobuf_py", "hbasedriver.operations", "hbasedriver.model", "hbasedriver.exceptions", "hbasedriver.client"]
```

### Comparing `hbase-driver-0.0.8/src/hbase_driver.egg-info/PKG-INFO` & `hbase-driver-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbase-driver
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Homepage, https://github.com/innovationb1ue/hbase-driver
 Project-URL: Issues, https://github.com/innovationb1ue/hbase-driver/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kazoo
 
 # hbase-driver
@@ -45,12 +45,13 @@
 
 ### Implemented
 
 - Create, Disable, Delete table
 - Put
 - Get
 - DELETE
+- Scan
 
 ### TODOs
 
-- Scan
 - Filters
+- More params in the operations.
```

### Comparing `hbase-driver-0.0.8/src/hbase_driver.egg-info/SOURCES.txt` & `hbase-driver-0.0.9/src/hbase_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/Connection.py` & `hbase-driver-0.0.9/src/hbasedriver/Connection.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/client/client.py` & `hbase-driver-0.0.9/src/hbasedriver/client/client.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/client/table.py` & `hbase-driver-0.0.9/src/hbasedriver/client/table.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/master.py` & `hbase-driver-0.0.9/src/hbasedriver/master.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/meta_server.py` & `hbase-driver-0.0.9/src/hbasedriver/meta_server.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/model/cell.py` & `hbase-driver-0.0.9/src/hbasedriver/model/cell.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/model/row.py` & `hbase-driver-0.0.9/src/hbasedriver/model/row.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/operations/delete.py` & `hbase-driver-0.0.9/src/hbasedriver/operations/delete.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/operations/get.py` & `hbase-driver-0.0.9/src/hbasedriver/operations/get.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/operations/put.py` & `hbase-driver-0.0.9/src/hbasedriver/operations/put.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/operations/scan.py` & `hbase-driver-0.0.9/src/hbasedriver/operations/scan.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/AccessControl_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Admin_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Admin_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Cell_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Cell_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Client_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Client_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterId_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterId_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Comparator_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Comparator_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Encryption_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Encryption_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/FS_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/FS_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Filter_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Filter_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HBase_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HBase_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HFile_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/HFile_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LockService_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/LockService_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MapReduce_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Master_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Master_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Procedure_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Procedure_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Quota_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Quota_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RPC_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RPC_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RecentLogs_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Registry_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Registry_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Replication_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Replication_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Snapshot_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TestProcedure_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TestProcedure_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Tracing_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/Tracing_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/WAL_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/WAL_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_pb2.pyi` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py` & `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/region.py` & `hbase-driver-0.0.9/src/hbasedriver/region.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/regionserver.py` & `hbase-driver-0.0.9/src/hbasedriver/regionserver.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/util/varint.py` & `hbase-driver-0.0.9/src/hbasedriver/util/varint.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/src/hbasedriver/zk.py` & `hbase-driver-0.0.9/src/hbasedriver/zk.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/test/test_client.py` & `hbase-driver-0.0.9/test/test_client.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/test/test_master.py` & `hbase-driver-0.0.9/test/test_master.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.8/test/test_scan.py` & `hbase-driver-0.0.9/test/test_scan.py`

 * *Files identical despite different names*

