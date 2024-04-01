# Comparing `tmp/tiledbsoma-1.9.2.tar.gz` & `tmp/tiledbsoma-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.9.2.tar", last modified: Thu Mar 28 16:03:50 2024, max compression
+gzip compressed data, was "tiledbsoma-1.9.3.tar", last modified: Mon Apr  1 15:14:50 2024, max compression
```

## Comparing `tiledbsoma-1.9.2.tar` & `tiledbsoma-1.9.3.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.184400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.188400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/khash/
--rw-r--r--   0 runner    (1001) docker     (127)    32575 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/khash/khash.h
--rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/khash/khashl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.184400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.192400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.192400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/reindexer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/reindexer.h
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.192400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/array_buffers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/enums.h
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (127)    19394 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_collection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_collection.h
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_context.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_context.h
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_experiment.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_experiment.h
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_group.h
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_measurement.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_measurement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_object.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_object.h
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.192400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.196400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/carrow.h
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.196400 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/test_indexer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_collection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.196400 tiledbsoma-1.9.2/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     3300 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/scripts/bld
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/scripts/bld.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1403 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.184400 tiledbsoma-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.200400 tiledbsoma-1.9.2/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    27774 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    37350 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (127)    24423 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    19480 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/common.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/ambient_label_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/id_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)   101038 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/io/outgest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/query_condition.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/reindexer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28814 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_collection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_context.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_dense_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_object.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-28 16:03:47.000000 tiledbsoma-1.9.2/src/tiledbsoma/soma_sparse_ndarray.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:03:50.204400 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-28 16:03:50.000000 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-28 16:03:50.000000 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:03:50.000000 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:03:50.000000 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-28 16:03:50.000000 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 16:03:50.000000 tiledbsoma-1.9.2/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-28 16:03:48.000000 tiledbsoma-1.9.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-01 15:14:47.000000 tiledbsoma-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-01 15:14:47.000000 tiledbsoma-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 15:14:49.000000 tiledbsoma-1.9.3/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.211971 tiledbsoma-1.9.3/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-01 15:14:47.000000 tiledbsoma-1.9.3/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.211971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.211971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.211971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/khash/
+-rw-r--r--   0 runner    (1001) docker     (127)    32575 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/khash/khash.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/khash/khashl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.211971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.215971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/reindexer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/reindexer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.219971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/array_buffers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19394 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_collection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_context.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_context.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_experiment.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_experiment.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_group.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_measurement.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_measurement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_object.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_object.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.219971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.219971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.223971 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/test_indexer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.223971 tiledbsoma-1.9.3/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3300 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/scripts/bld
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/scripts/bld.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1403 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:14:50.231971 tiledbsoma-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.211971 tiledbsoma-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28478 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37350 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24423 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/common.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/ambient_label_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/id_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101038 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/io/outgest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/query_condition.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/reindexer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28814 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_context.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_object.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/src/tiledbsoma/soma_sparse_ndarray.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:50.227971 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-01 15:14:50.000000 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-01 15:14:50.000000 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:14:50.000000 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:14:50.000000 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 15:14:50.000000 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 15:14:50.000000 tiledbsoma-1.9.3/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-01 15:14:48.000000 tiledbsoma-1.9.3/version.py
```

### Comparing `tiledbsoma-1.9.2/PKG-INFO` & `tiledbsoma-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.9.2
+Version: 1.9.3
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.9.2/README.md` & `tiledbsoma-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/khash/khash.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/khash/khash.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/khash/khashl.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/khash/khashl.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/example.py` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/example.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/reindexer.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/reindexer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/reindexer.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/reindexer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/array_buffers.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/array_buffers.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/array_buffers.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/array_buffers.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/column_buffer.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/column_buffer.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/column_buffer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/enums.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/enums.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/logger_public.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_collection.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_collection.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_collection.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_collection.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_context.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_context.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_context.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_context.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dataframe.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dataframe.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_experiment.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_experiment.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_experiment.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_experiment.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_group.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_group.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_group.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_measurement.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_measurement.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_measurement.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_measurement.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_object.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_object.cc`

 * *Files 23% similar despite different names*

```diff
@@ -14,44 +14,60 @@
 
 using namespace tiledb;
 
 std::unique_ptr<SOMAObject> SOMAObject::open(
     std::string_view uri,
     OpenMode mode,
     std::shared_ptr<SOMAContext> ctx,
-    std::optional<std::pair<uint64_t, uint64_t>> timestamp) {
-    auto obj = tiledb::Object::object(*ctx->tiledb_ctx(), std::string(uri));
+    std::optional<std::pair<uint64_t, uint64_t>> timestamp,
+    std::optional<std::string> soma_type) {
+    if (soma_type == std::nullopt) {
+        auto tiledb_type = Object::object(*ctx->tiledb_ctx(), std::string(uri))
+                               .type();
+        switch (tiledb_type) {
+            case Object::Type::Array:
+                soma_type = "SOMAArray";
+                break;
+            case Object::Type::Group:
+                soma_type = "SOMAGroup";
+                break;
+            default:
+                throw TileDBSOMAError("Saw invalid TileDB type");
+        }
+    }
 
-    if (obj.type() == tiledb::Object::Type::Array) {
+    if (soma_type == "SOMAArray") {
         auto array_ = SOMAArray::open(
             mode, uri, ctx, "", {}, "auto", ResultOrder::automatic, timestamp);
+        auto array_type = array_->type();
 
-        if (!array_->type().has_value())
+        if (!array_type.has_value())
             throw TileDBSOMAError("SOMAArray has no type info");
 
-        if (array_->type() == "SOMADataFrame") {
+        if (array_type == "SOMADataFrame") {
             return std::make_unique<SOMADataFrame>(*array_);
-        } else if (array_->type() == "SOMASparseNDArray") {
+        } else if (array_type == "SOMASparseNDArray") {
             return std::make_unique<SOMASparseNDArray>(*array_);
-        } else if (array_->type() == "SOMADenseNDArray") {
+        } else if (array_type == "SOMADenseNDArray") {
             return std::make_unique<SOMADenseNDArray>(*array_);
         } else {
             throw TileDBSOMAError("Saw invalid SOMAArray type");
         }
-    } else if (obj.type() == tiledb::Object::Type::Group) {
+    } else if (soma_type == "SOMAGroup") {
         auto group_ = SOMAGroup::open(mode, uri, ctx, "", timestamp);
+        auto group_type = group_->type();
 
-        if (!group_->type().has_value())
+        if (!group_type.has_value())
             throw TileDBSOMAError("SOMAGroup has no type info");
 
-        if (group_->type() == "SOMACollection") {
+        if (group_type == "SOMACollection") {
             return std::make_unique<SOMACollection>(*group_);
-        } else if (group_->type() == "SOMAExperiment") {
+        } else if (group_type == "SOMAExperiment") {
             return std::make_unique<SOMAExperiment>(*group_);
-        } else if (group_->type() == "SOMAMeasurement") {
+        } else if (group_type == "SOMAMeasurement") {
             return std::make_unique<SOMAMeasurement>(*group_);
         } else {
             throw TileDBSOMAError("Saw invalid SOMAGroup type");
         }
     }
 
     throw TileDBSOMAError("Invalid TileDB object passed to SOMAObject::open");
```

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_object.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_object.h`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     //===================================================================
     virtual ~SOMAObject() = default;
 
     static std::unique_ptr<SOMAObject> open(
         std::string_view uri,
         OpenMode mode,
         std::shared_ptr<SOMAContext> ctx,
-        std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
+        std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt,
+        std::optional<std::string> soma_type = std::nullopt);
 
     /**
      * @brief Return a constant string describing the type of the object.
      */
     const std::optional<std::string> type();
 
     /**
```

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/carrow.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/src/utils/version.h` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/test_indexer.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/test_indexer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_collection.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_collection.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_group.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.9.3/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/scripts/bld` & `tiledbsoma-1.9.3/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/scripts/bld.ps1` & `tiledbsoma-1.9.3/dist_links/scripts/bld.ps1`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.9.3/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/scripts/show-versions.py` & `tiledbsoma-1.9.3/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.9.3/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/setup.py` & `tiledbsoma-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/__init__.py` & `tiledbsoma-1.9.3/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_collection.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,35 @@
         handle = cls._wrapper_type.open(uri, "w", context, tiledb_timestamp)
         cls._set_create_metadata(handle)
         return cls(
             handle,
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
 
+    @classmethod
+    def open(
+        cls,
+        uri: str,
+        mode: options.OpenMode = "r",
+        *,
+        tiledb_timestamp: Optional[OpenTimestamp] = None,
+        context: Optional[SOMATileDBContext] = None,
+        platform_config: Optional[options.PlatformConfig] = None,
+        clib_type: Optional[str] = None,
+    ) -> Self:
+        """Opens this specific type of SOMA object."""
+        return super().open(
+            uri,
+            mode,
+            tiledb_timestamp=tiledb_timestamp,
+            context=context,
+            platform_config=platform_config,
+            clib_type="SOMAGroup",
+        )
+
     # Subclass protocol to constrain which SOMA objects types  may be set on a
     # particular collection key. Used by Experiment and Measurement.
     _subclass_constrained_soma_types: ClassVar[Dict[str, Tuple[str, ...]]] = {}
     """A map limiting what types may be set to certain keys.
 
     Map keys are the key of the collection to constrain; values are the SOMA
     type names of the types that may be set to the key.  See :class:`Experiment` and
@@ -432,15 +453,16 @@
 
             uri = entry.entry.uri
             mode = self.mode
             context = self.context
             timestamp = self.tiledb_timestamp_ms
 
             try:
-                wrapper = _tdb_handles.open(uri, mode, context, timestamp)
+                clib_type = entry.entry.wrapper_type.clib_type
+                wrapper = _tdb_handles.open(uri, mode, context, timestamp, clib_type)
                 entry.soma = _factory.reify_handle(wrapper)
             except SOMAError:
                 entry.soma = _factory._open_internal(
                     entry.entry.wrapper_type.open, uri, mode, context, timestamp
                 )
             # Since we just opened this object, we own it and should close it.
             self._close_stack.enter_context(entry.soma)
```

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_common_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_exception.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_factory.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_indexer.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_indexer.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_sparse_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_tdb_handles.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,60 +50,77 @@
 
 
 def open(
     uri: str,
     mode: options.OpenMode,
     context: SOMATileDBContext,
     timestamp: Optional[OpenTimestamp],
+    clib_type: Optional[str] = None,
 ) -> "Wrapper[RawHandle]":
     """Determine whether the URI is an array or group, and open it."""
     open_mode = clib.OpenMode.read if mode == "r" else clib.OpenMode.write
+
+    # raise("WAMI")
+
+    # Traceback (most recent call last):
+    #   File "/home/ubuntu/Desktop/awol-perf/./aw3.py", line 20, in <module>
+    #     exp = tiledbsoma.Experiment.open(SOMA_URI)
+    #   File "/home/ubuntu/git/single-cell-data/TileDB-SOMA/apis/python/src/tiledbsoma/_tiledb_object.py", line 96, in open
+    #     handle = _tdb_handles.open(uri, mode, context, tiledb_timestamp)
+    #   File "/home/ubuntu/git/single-cell-data/TileDB-SOMA/apis/python/src/tiledbsoma/_tdb_handles.py", line 63, in open
+    #     raise("WAMI")
+    # TypeError: exceptions must derive from BaseException
+
     timestamp_ms = context._open_timestamp_ms(timestamp)
 
     # if there is not a valid SOMAObject at the given URI, this
     # returns None
     soma_object = clib.SOMAObject.open(
-        uri, open_mode, context.native_context, timestamp=(0, timestamp_ms)
+        uri=uri,
+        mode=open_mode,
+        context=context.native_context,
+        timestamp=(0, timestamp_ms),
+        clib_type=clib_type,
     )
 
     # Avoid creating a TileDB-Py Ctx unless necessary
-    obj_type = (
+    soma_type = (
         soma_object.type
         if soma_object is not None
         else tiledb.object_type(uri, ctx=context.tiledb_ctx)
     )
 
-    if not obj_type:
+    if not soma_type:
         raise DoesNotExistError(f"{uri!r} does not exist")
 
-    if open_mode == clib.OpenMode.read and obj_type == "SOMADataFrame":
+    if open_mode == clib.OpenMode.read and soma_type == "SOMADataFrame":
         return DataFrameWrapper._from_soma_object(soma_object, context)
-    if open_mode == clib.OpenMode.read and obj_type == "SOMADenseNDArray":
+    if open_mode == clib.OpenMode.read and soma_type == "SOMADenseNDArray":
         return DenseNDArrayWrapper._from_soma_object(soma_object, context)
-    if open_mode == clib.OpenMode.read and obj_type == "SOMASparseNDArray":
+    if open_mode == clib.OpenMode.read and soma_type == "SOMASparseNDArray":
         return SparseNDArrayWrapper._from_soma_object(soma_object, context)
 
-    if obj_type in (
+    if soma_type in (
         "SOMADataFrame",
         "SOMADenseNDArray",
         "SOMASparseNDArray",
         "array",
     ):
         return ArrayWrapper.open(uri, mode, context, timestamp)
 
-    if obj_type in (
+    if soma_type in (
         "SOMACollection",
         "SOMAExperiment",
         "SOMAMeasurement",
         "group",
     ):
         return GroupWrapper.open(uri, mode, context, timestamp)
 
     # Invalid object
-    raise SOMAError(f"{uri!r} has unknown storage type {obj_type!r}")
+    raise SOMAError(f"{uri!r} has unknown storage type {soma_type!r}")
 
 
 @attrs.define(eq=False, hash=False, slots=False)
 class Wrapper(Generic[_RawHdl_co], metaclass=abc.ABCMeta):
     """Wrapper for TileDB handles to manage lifecycle and metadata.
 
     Callers may read and use (non-underscored) members but should never set
@@ -112,14 +129,15 @@
 
     uri: str
     mode: options.OpenMode
     context: SOMATileDBContext
     timestamp_ms: int
     _handle: _RawHdl_co
     closed: bool = attrs.field(default=False, init=False)
+    clib_type: Optional[str] = None
 
     @classmethod
     def open(
         cls,
         uri: str,
         mode: options.OpenMode,
         context: SOMATileDBContext,
@@ -238,14 +256,16 @@
 AnyWrapper = Wrapper[RawHandle]
 """Non-instantiable type representing any Handle."""
 
 
 class ArrayWrapper(Wrapper[tiledb.Array]):
     """Wrapper around a TileDB Array handle."""
 
+    clib_type = "SOMAArray"
+
     @classmethod
     def _opener(
         cls,
         uri: str,
         mode: options.OpenMode,
         context: SOMATileDBContext,
         timestamp: int,
@@ -303,14 +323,16 @@
             return GroupEntry(obj.uri, GroupWrapper)
         raise SOMAError(f"internal error: unknown object type {obj.type}")
 
 
 class GroupWrapper(Wrapper[tiledb.Group]):
     """Wrapper around a TileDB Group handle."""
 
+    clib_type = "SOMAGroup"
+
     @classmethod
     def _opener(
         cls,
         uri: str,
         mode: options.OpenMode,
         context: SOMATileDBContext,
         timestamp: int,
```

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_tiledb_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #
 # Licensed under the MIT License.
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import pyarrow as pa
 import tiledb
-from somacore.options import ResultOrder, ResultOrderStr
+from somacore import options
+from typing_extensions import Self
 
 from . import _tdb_handles, _util
 
 # This package's pybind11 code
 from . import pytiledbsoma as clib  # noqa: E402
 from ._arrow_types import tiledb_schema_to_arrow
 from ._tiledb_object import TileDBObject
@@ -28,14 +29,35 @@
         Experimental.
     """
 
     __slots__ = ()
 
     _wrapper_type = _tdb_handles.ArrayWrapper
 
+    @classmethod
+    def open(
+        cls,
+        uri: str,
+        mode: options.OpenMode = "r",
+        *,
+        tiledb_timestamp: Optional[OpenTimestamp] = None,
+        context: Optional[SOMATileDBContext] = None,
+        platform_config: Optional[options.PlatformConfig] = None,
+        clib_type: Optional[str] = None,
+    ) -> Self:
+        """Opens this specific type of SOMA object."""
+        return super().open(
+            uri,
+            mode,
+            tiledb_timestamp=tiledb_timestamp,
+            context=context,
+            platform_config=platform_config,
+            clib_type="SOMAArray",
+        )
+
     @property
     def schema(self) -> pa.Schema:
         """Returns data schema, in the form of an
         `Arrow Schema <https://arrow.apache.org/docs/python/generated/pyarrow.Schema.html>`_.
 
         Lifecycle:
             Experimental.
@@ -83,15 +105,15 @@
 
     def _soma_reader(
         self,
         *,
         schema: Optional[tiledb.ArraySchema] = None,
         column_names: Optional[Sequence[str]] = None,
         query_condition: Optional[tiledb.QueryCondition] = None,
-        result_order: Optional[ResultOrderStr] = None,
+        result_order: Optional[options.ResultOrderStr] = None,
     ) -> clib.SOMAArray:
         """Constructs a C++ SOMAArray using appropriate context/config/etc."""
         # Leave empty arguments out of kwargs to allow C++ constructor defaults to apply, as
         # they're not all wrapped in std::optional<>.
         kwargs: Dict[str, object] = {}
         # if schema:
         #     kwargs["schema"] = schema
@@ -99,15 +121,17 @@
             kwargs["column_names"] = column_names
         if result_order:
             result_order_map = {
                 "auto": clib.ResultOrder.automatic,
                 "row-major": clib.ResultOrder.rowmajor,
                 "column-major": clib.ResultOrder.colmajor,
             }
-            result_order_enum = result_order_map[ResultOrder(result_order).value]
+            result_order_enum = result_order_map[
+                options.ResultOrder(result_order).value
+            ]
             kwargs["result_order"] = result_order_enum
 
         soma_array = clib.SOMAArray(
             self.uri,
             name=f"{self} reader",
             platform_config=self._ctx.config().dict(),
             timestamp=(0, self.tiledb_timestamp_ms),
```

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_tiledb_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         cls,
         uri: str,
         mode: options.OpenMode = "r",
         *,
         tiledb_timestamp: Optional[OpenTimestamp] = None,
         context: Optional[SOMATileDBContext] = None,
         platform_config: Optional[options.PlatformConfig] = None,
+        clib_type: Optional[str] = None,
     ) -> Self:
         """Opens this specific type of SOMA object.
 
         Args:
             uri:
                 The URI to open.
             mode:
@@ -88,15 +89,17 @@
                 If the user-provided ``mode`` is invalid.
 
         Lifecycle:
             Experimental.
         """
         del platform_config  # unused
         context = _validate_soma_tiledb_context(context)
-        handle = _tdb_handles.open(uri, mode, context, tiledb_timestamp)
+        handle = _tdb_handles.open(
+            uri, mode, context, tiledb_timestamp, clib_type=clib_type
+        )
         if not isinstance(handle, cls._reader_wrapper_type):
             handle = cls._wrapper_type.open(uri, mode, context, tiledb_timestamp)
         return cls(
             handle,  # type: ignore[arg-type]
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
```

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_types.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/_util.py` & `tiledbsoma-1.9.3/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/common.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/common.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/common.h` & `tiledbsoma-1.9.3/src/tiledbsoma/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/eta.py` & `tiledbsoma-1.9.3/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.9.3/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/__init__.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/_common.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/_common.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/__init__.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/ambient_label_mappings.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/ambient_label_mappings.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/id_mappings.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/id_mappings.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/_registration/signatures.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/_registration/signatures.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/_util.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/ingest.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/io/outgest.py` & `tiledbsoma-1.9.3/src/tiledbsoma/io/outgest.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/logging.py` & `tiledbsoma-1.9.3/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.9.3/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.9.3/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/reindexer.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/reindexer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_array.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_collection.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_collection.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_context.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_context.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_dataframe.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_dataframe.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_dense_ndarray.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_dense_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_group.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_object.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_object.cc`

 * *Files 25% similar despite different names*

```diff
@@ -51,36 +51,45 @@
     py::class_<SOMAObject>(m, "SOMAObject")
 
         .def_static(
             "open",
             [](std::string_view uri,
                OpenMode mode,
                std::shared_ptr<SOMAContext> context,
-               std::optional<std::pair<uint64_t, uint64_t>> timestamp)
-                -> py::object {
+               std::optional<std::pair<uint64_t, uint64_t>> timestamp,
+               std::optional<std::string> clib_type) -> py::object {
                 try {
-                    auto obj = SOMAObject::open(uri, mode, context, timestamp);
-                    if (obj->type() == "SOMADataFrame")
-                        return py::cast(dynamic_cast<SOMADataFrame&>(*obj));
-                    else if (obj->type() == "SOMASparseNDArray")
-                        return py::cast(dynamic_cast<SOMASparseNDArray&>(*obj));
-                    else if (obj->type() == "SOMADenseNDArray")
-                        return py::cast(dynamic_cast<SOMADenseNDArray&>(*obj));
-                    else if (obj->type() == "SOMACollection")
-                        return py::cast(dynamic_cast<SOMACollection&>(*obj));
-                    else if (obj->type() == "SOMAExperiment")
-                        return py::cast(dynamic_cast<SOMAExperiment&>(*obj));
-                    else if (obj->type() == "SOMAMeasurement")
-                        return py::cast(dynamic_cast<SOMAMeasurement&>(*obj));
+                    auto soma_obj = SOMAObject::open(
+                        uri, mode, context, timestamp, clib_type);
+                    auto soma_obj_type = soma_obj->type();
+                    if (soma_obj_type == "SOMADataFrame")
+                        return py::cast(
+                            dynamic_cast<SOMADataFrame&>(*soma_obj));
+                    else if (soma_obj_type == "SOMASparseNDArray")
+                        return py::cast(
+                            dynamic_cast<SOMASparseNDArray&>(*soma_obj));
+                    else if (soma_obj_type == "SOMADenseNDArray")
+                        return py::cast(
+                            dynamic_cast<SOMADenseNDArray&>(*soma_obj));
+                    else if (soma_obj_type == "SOMACollection")
+                        return py::cast(
+                            dynamic_cast<SOMACollection&>(*soma_obj));
+                    else if (soma_obj_type == "SOMAExperiment")
+                        return py::cast(
+                            dynamic_cast<SOMAExperiment&>(*soma_obj));
+                    else if (soma_obj_type == "SOMAMeasurement")
+                        return py::cast(
+                            dynamic_cast<SOMAMeasurement&>(*soma_obj));
                     return py::none();
                 } catch (...) {
                     return py::none();
                 }
             },
             "uri"_a,
             "mode"_a,
             "context"_a,
             py::kw_only(),
-            "timestamp"_a = py::none())
+            "timestamp"_a = py::none(),
+            "clib_type"_a = py::none())
         .def_property_readonly("type", &SOMAObject::type);
 };
 }  // namespace libtiledbsomacpp
```

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma/soma_sparse_ndarray.cc` & `tiledbsoma-1.9.3/src/tiledbsoma/soma_sparse_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.9.3/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.9.2
+Version: 1.9.3
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.9.2/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.9.3/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.2/version.py` & `tiledbsoma-1.9.3/version.py`

 * *Files identical despite different names*

