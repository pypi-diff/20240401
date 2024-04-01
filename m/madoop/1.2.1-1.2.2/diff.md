# Comparing `tmp/madoop-1.2.1.tar.gz` & `tmp/madoop-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madoop-1.2.1.tar", last modified: Fri Mar 29 13:54:01 2024, max compression
+gzip compressed data, was "madoop-1.2.2.tar", last modified: Mon Apr  1 15:16:42 2024, max compression
```

## Comparing `madoop-1.2.1.tar` & `madoop-1.2.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.515934 madoop-1.2.1/
--rw-rw-r--   0 awdeorio   (501) staff       (20)      222 2021-10-24 20:43:51.000000 madoop-1.2.1/.pylintrc
--rw-rw-r--   0 awdeorio   (501) staff       (20)     1671 2024-03-29 13:40:11.000000 madoop-1.2.1/CONTRIBUTING.md
--rw-rw-r--   0 awdeorio   (501) staff       (20)     1071 2021-10-21 18:56:55.000000 madoop-1.2.1/LICENSE
--rw-rw-r--   0 awdeorio   (501) staff       (20)      284 2024-03-29 13:36:41.000000 madoop-1.2.1/MANIFEST.in
--rw-r--r--   0 awdeorio   (501) staff       (20)     4971 2024-03-29 13:54:01.515750 madoop-1.2.1/PKG-INFO
--rw-rw-r--   0 awdeorio   (501) staff       (20)     2793 2022-11-07 15:29:19.000000 madoop-1.2.1/README.md
--rw-rw-r--   0 awdeorio   (501) staff       (20)     9617 2022-11-07 15:29:19.000000 madoop-1.2.1/README_Hadoop_Streaming.md
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.508775 madoop-1.2.1/madoop/
--rw-rw-r--   0 awdeorio   (501) staff       (20)      125 2021-11-30 21:07:41.000000 madoop-1.2.1/madoop/__init__.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     3649 2024-03-29 13:53:15.000000 madoop-1.2.1/madoop/__main__.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.509739 madoop-1.2.1/madoop/example/
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.509957 madoop-1.2.1/madoop/example/input/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2022-01-18 13:05:06.000000 madoop-1.2.1/madoop/example/input/input01.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2022-01-18 13:05:06.000000 madoop-1.2.1/madoop/example/input/input02.txt
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      160 2022-01-18 13:05:06.000000 madoop-1.2.1/madoop/example/map.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      619 2022-01-18 13:05:06.000000 madoop-1.2.1/madoop/example/reduce.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)      158 2021-11-30 21:07:41.000000 madoop-1.2.1/madoop/exceptions.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)    14569 2024-03-29 13:40:11.000000 madoop-1.2.1/madoop/mapreduce.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.515118 madoop-1.2.1/madoop.egg-info/
--rw-r--r--   0 awdeorio   (501) staff       (20)     4971 2024-03-29 13:54:01.000000 madoop-1.2.1/madoop.egg-info/PKG-INFO
--rw-rw-r--   0 awdeorio   (501) staff       (20)     2737 2024-03-29 13:54:01.000000 madoop-1.2.1/madoop.egg-info/SOURCES.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)        1 2024-03-29 13:54:01.000000 madoop-1.2.1/madoop.egg-info/dependency_links.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       48 2024-03-29 13:54:01.000000 madoop-1.2.1/madoop.egg-info/entry_points.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       96 2024-03-29 13:54:01.000000 madoop-1.2.1/madoop.egg-info/requires.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)        7 2024-03-29 13:54:01.000000 madoop-1.2.1/madoop.egg-info/top_level.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)      961 2024-03-29 13:53:15.000000 madoop-1.2.1/pyproject.toml
--rw-rw-r--   0 awdeorio   (501) staff       (20)       38 2024-03-29 13:54:01.515972 madoop-1.2.1/setup.cfg
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.510535 madoop-1.2.1/tests/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       97 2021-10-24 20:48:54.000000 madoop-1.2.1/tests/__init__.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     5973 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/test_api.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     4049 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/test_cli.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     2550 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/test_stages.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.506523 madoop-1.2.1/tests/testdata/
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.511649 madoop-1.2.1/tests/testdata/word_count/
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.507202 madoop-1.2.1/tests/testdata/word_count/correct/
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.512413 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2022-02-14 15:49:14.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)       40 2022-02-14 15:49:14.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output/part-00002
--rw-rw-r--   0 awdeorio   (501) staff       (20)       16 2022-02-14 15:49:14.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output/part-00003
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.512653 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output-2-reducers/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output-2-reducers/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)       16 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output-2-reducers/part-00001
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.512884 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output-custom-partitioner/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       16 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output-custom-partitioner/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count/correct/grouper-output-custom-partitioner/part-00001
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.513116 madoop-1.2.1/tests/testdata/word_count/correct/mapper-output/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       30 2022-02-10 14:53:20.000000 madoop-1.2.1/tests/testdata/word_count/correct/mapper-output/part-00001
--rw-rw-r--   0 awdeorio   (501) staff       (20)       36 2022-02-10 14:53:20.000000 madoop-1.2.1/tests/testdata/word_count/correct/mapper-output/part-00002
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.513456 madoop-1.2.1/tests/testdata/word_count/correct/output/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2022-02-14 15:48:21.000000 madoop-1.2.1/tests/testdata/word_count/correct/output/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2022-02-18 20:38:07.000000 madoop-1.2.1/tests/testdata/word_count/correct/output/part-00001
--rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2022-02-18 20:38:07.000000 madoop-1.2.1/tests/testdata/word_count/correct/output/part-00002
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.513670 madoop-1.2.1/tests/testdata/word_count/correct/output-2-reducers/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       33 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/correct/output-2-reducers/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/correct/output-2-reducers/part-00001
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.514024 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2022-02-14 15:49:32.000000 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2022-02-18 20:38:07.000000 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output/part-00001
--rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2022-02-18 20:38:07.000000 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output/part-00002
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.514234 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output-2-reducers/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       33 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output-2-reducers/part-00000
--rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/correct/reducer-output-2-reducers/part-00001
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.514456 madoop-1.2.1/tests/testdata/word_count/input/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2022-02-10 14:53:20.000000 madoop-1.2.1/tests/testdata/word_count/input/input01.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2022-02-10 14:53:20.000000 madoop-1.2.1/tests/testdata/word_count/input/input02.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/input-single-file.txt
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.514677 madoop-1.2.1/tests/testdata/word_count/input_empty/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2022-02-15 15:22:20.000000 madoop-1.2.1/tests/testdata/word_count/input_empty/input01.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)        0 2022-02-15 15:22:20.000000 madoop-1.2.1/tests/testdata/word_count/input_empty/input02.txt
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.514880 madoop-1.2.1/tests/testdata/word_count/input_with_subdir/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/input_with_subdir/input01.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/input_with_subdir/input02.txt
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.514985 madoop-1.2.1/tests/testdata/word_count/input_with_subdir/subdir/
--rw-rw-r--   0 awdeorio   (501) staff       (20)        0 2023-11-04 14:54:52.000000 madoop-1.2.1/tests/testdata/word_count/input_with_subdir/subdir/.gitkeep
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      160 2022-01-20 01:20:41.000000 madoop-1.2.1/tests/testdata/word_count/map.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      168 2022-02-10 14:53:20.000000 madoop-1.2.1/tests/testdata/word_count/map.sh
--rwxrwxr-x   0 awdeorio   (501) staff       (20)       95 2022-01-18 13:05:06.000000 madoop-1.2.1/tests/testdata/word_count/map_invalid.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      259 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count/partition.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      101 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count/partition_invalid.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      108 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count/partition_noninteger.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      619 2022-01-20 01:20:41.000000 madoop-1.2.1/tests/testdata/word_count/reduce.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      257 2022-01-18 13:05:06.000000 madoop-1.2.1/tests/testdata/word_count/reduce.sh
--rwxrwxr-x   0 awdeorio   (501) staff       (20)       75 2022-01-18 13:05:06.000000 madoop-1.2.1/tests/testdata/word_count/reduce_invalid.py
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.511866 madoop-1.2.1/tests/testdata/word_count SPACE/
-drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-03-29 13:54:01.512081 madoop-1.2.1/tests/testdata/word_count SPACE/input SPACE/
--rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count SPACE/input SPACE/input 01.txt
--rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count SPACE/input SPACE/input 02.txt
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      160 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count SPACE/map SPACE.py
--rwxrwxr-x   0 awdeorio   (501) staff       (20)      619 2024-03-29 13:40:11.000000 madoop-1.2.1/tests/testdata/word_count SPACE/reduce SPACE.py
--rw-rw-r--   0 awdeorio   (501) staff       (20)     1280 2022-01-18 13:05:06.000000 madoop-1.2.1/tests/utils.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.016397 madoop-1.2.2/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      222 2021-10-24 20:43:51.000000 madoop-1.2.2/.pylintrc
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1671 2024-03-29 13:40:11.000000 madoop-1.2.2/CONTRIBUTING.md
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1071 2021-10-21 18:56:55.000000 madoop-1.2.2/LICENSE
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      284 2024-03-29 13:36:41.000000 madoop-1.2.2/MANIFEST.in
+-rw-r--r--   0 awdeorio   (501) staff       (20)     4971 2024-04-01 15:16:42.016206 madoop-1.2.2/PKG-INFO
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     2793 2022-11-07 15:29:19.000000 madoop-1.2.2/README.md
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    11061 2024-04-01 15:15:39.000000 madoop-1.2.2/README_Hadoop_Streaming.md
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.008708 madoop-1.2.2/madoop/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      125 2021-11-30 21:07:41.000000 madoop-1.2.2/madoop/__init__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     3649 2024-03-29 13:53:15.000000 madoop-1.2.2/madoop/__main__.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.009702 madoop-1.2.2/madoop/example/
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.009972 madoop-1.2.2/madoop/example/input/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2022-01-18 13:05:06.000000 madoop-1.2.2/madoop/example/input/input01.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2022-01-18 13:05:06.000000 madoop-1.2.2/madoop/example/input/input02.txt
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      160 2022-01-18 13:05:06.000000 madoop-1.2.2/madoop/example/map.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      619 2022-01-18 13:05:06.000000 madoop-1.2.2/madoop/example/reduce.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      158 2021-11-30 21:07:41.000000 madoop-1.2.2/madoop/exceptions.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)    14569 2024-03-29 13:40:11.000000 madoop-1.2.2/madoop/mapreduce.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.015583 madoop-1.2.2/madoop.egg-info/
+-rw-r--r--   0 awdeorio   (501) staff       (20)     4971 2024-04-01 15:16:41.000000 madoop-1.2.2/madoop.egg-info/PKG-INFO
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     2737 2024-04-01 15:16:42.000000 madoop-1.2.2/madoop.egg-info/SOURCES.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        1 2024-04-01 15:16:42.000000 madoop-1.2.2/madoop.egg-info/dependency_links.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       48 2024-04-01 15:16:42.000000 madoop-1.2.2/madoop.egg-info/entry_points.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       96 2024-04-01 15:16:42.000000 madoop-1.2.2/madoop.egg-info/requires.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        7 2024-04-01 15:16:42.000000 madoop-1.2.2/madoop.egg-info/top_level.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)      961 2024-04-01 15:15:39.000000 madoop-1.2.2/pyproject.toml
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       38 2024-04-01 15:16:42.016439 madoop-1.2.2/setup.cfg
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.010644 madoop-1.2.2/tests/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       97 2021-10-24 20:48:54.000000 madoop-1.2.2/tests/__init__.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     5973 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/test_api.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     4049 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/test_cli.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     2550 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/test_stages.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.006523 madoop-1.2.2/tests/testdata/
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.011891 madoop-1.2.2/tests/testdata/word_count/
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.007130 madoop-1.2.2/tests/testdata/word_count/correct/
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.012734 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2022-02-14 15:49:14.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       40 2022-02-14 15:49:14.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output/part-00002
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       16 2022-02-14 15:49:14.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output/part-00003
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.012970 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output-2-reducers/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output-2-reducers/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       16 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output-2-reducers/part-00001
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.013219 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output-custom-partitioner/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       16 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output-custom-partitioner/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count/correct/grouper-output-custom-partitioner/part-00001
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.013455 madoop-1.2.2/tests/testdata/word_count/correct/mapper-output/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       30 2022-02-10 14:53:20.000000 madoop-1.2.2/tests/testdata/word_count/correct/mapper-output/part-00001
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       36 2022-02-10 14:53:20.000000 madoop-1.2.2/tests/testdata/word_count/correct/mapper-output/part-00002
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.013826 madoop-1.2.2/tests/testdata/word_count/correct/output/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2022-02-14 15:48:21.000000 madoop-1.2.2/tests/testdata/word_count/correct/output/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2022-02-18 20:38:07.000000 madoop-1.2.2/tests/testdata/word_count/correct/output/part-00001
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2022-02-18 20:38:07.000000 madoop-1.2.2/tests/testdata/word_count/correct/output/part-00002
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.014066 madoop-1.2.2/tests/testdata/word_count/correct/output-2-reducers/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       33 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/correct/output-2-reducers/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/correct/output-2-reducers/part-00001
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.014429 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       10 2022-02-14 15:49:32.000000 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       23 2022-02-18 20:38:07.000000 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output/part-00001
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2022-02-18 20:38:07.000000 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output/part-00002
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.014663 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output-2-reducers/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       33 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output-2-reducers/part-00000
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        8 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/correct/reducer-output-2-reducers/part-00001
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.014895 madoop-1.2.2/tests/testdata/word_count/input/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2022-02-10 14:53:20.000000 madoop-1.2.2/tests/testdata/word_count/input/input01.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2022-02-10 14:53:20.000000 madoop-1.2.2/tests/testdata/word_count/input/input02.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/input-single-file.txt
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.015130 madoop-1.2.2/tests/testdata/word_count/input_empty/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       50 2022-02-15 15:22:20.000000 madoop-1.2.2/tests/testdata/word_count/input_empty/input01.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        0 2022-02-15 15:22:20.000000 madoop-1.2.2/tests/testdata/word_count/input_empty/input02.txt
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.015335 madoop-1.2.2/tests/testdata/word_count/input_with_subdir/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/input_with_subdir/input01.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/input_with_subdir/input02.txt
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.015453 madoop-1.2.2/tests/testdata/word_count/input_with_subdir/subdir/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)        0 2023-11-04 14:54:52.000000 madoop-1.2.2/tests/testdata/word_count/input_with_subdir/subdir/.gitkeep
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      160 2022-01-20 01:20:41.000000 madoop-1.2.2/tests/testdata/word_count/map.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      168 2022-02-10 14:53:20.000000 madoop-1.2.2/tests/testdata/word_count/map.sh
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)       95 2022-01-18 13:05:06.000000 madoop-1.2.2/tests/testdata/word_count/map_invalid.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      259 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count/partition.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      101 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count/partition_invalid.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      108 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count/partition_noninteger.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      619 2022-01-20 01:20:41.000000 madoop-1.2.2/tests/testdata/word_count/reduce.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      257 2022-01-18 13:05:06.000000 madoop-1.2.2/tests/testdata/word_count/reduce.sh
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)       75 2022-01-18 13:05:06.000000 madoop-1.2.2/tests/testdata/word_count/reduce_invalid.py
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.012134 madoop-1.2.2/tests/testdata/word_count SPACE/
+drwxrwxr-x   0 awdeorio   (501) staff       (20)        0 2024-04-01 15:16:42.012384 madoop-1.2.2/tests/testdata/word_count SPACE/input SPACE/
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       22 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count SPACE/input SPACE/input 01.txt
+-rw-rw-r--   0 awdeorio   (501) staff       (20)       28 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count SPACE/input SPACE/input 02.txt
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      160 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count SPACE/map SPACE.py
+-rwxrwxr-x   0 awdeorio   (501) staff       (20)      619 2024-03-29 13:40:11.000000 madoop-1.2.2/tests/testdata/word_count SPACE/reduce SPACE.py
+-rw-rw-r--   0 awdeorio   (501) staff       (20)     1280 2022-01-18 13:05:06.000000 madoop-1.2.2/tests/utils.py
```

### Comparing `madoop-1.2.1/CONTRIBUTING.md` & `madoop-1.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/LICENSE` & `madoop-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/PKG-INFO` & `madoop-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madoop
-Version: 1.2.1
+Version: 1.2.2
 Summary: A light weight MapReduce framework for education.
 Author-email: Andrew DeOrio <awdeorio@umich.edu>
 License: MIT License
         
         Copyright (c) 2021 EECS 485 Staff
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `madoop-1.2.1/README.md` & `madoop-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/README_Hadoop_Streaming.md` & `madoop-1.2.2/README_Hadoop_Streaming.md`

 * *Files 10% similar despite different names*

```diff
@@ -336,7 +336,41 @@
 def reduce_one_group(key, group):
     group = list(group)  # iterable to list
     for line in group:
         pass  # Do something
     for line in group:
         pass  # Do something
 ```
+
+## Custom partitioner
+If you need to specify which key-value pairs are sent to which reducers, you can create a custom partitioner. Here's a sample which works with our word count example.
+```python
+#!/usr/bin/env -S python3 -u
+"""Word count partitioner."""
+import sys
+
+
+num_reducers = int(sys.argv[1])
+
+
+for line in sys.stdin:
+    key, value = line.split("\t")
+    if key[0] <= "G":
+        print(0 % num_reducers)
+    else:
+        print(1 % num_reducers)
+```
+
+Each line of output from the mappers is streamed to this partition file, and the number of reducers is set to `sys.argv[1]`. For each line, the partitioner checks whether the first letter of the key is less than or greater than "G". If it's less than "G", the line is sent to the first reducer, and if it's greater, the line is sent to the second reducer. 
+
+Use the `-partitioner` command-line argument to tell Madoop to use this partitioner.
+
+```console
+$ madoop \
+  -input example/input \
+  -output example/output \
+  -mapper example/map.py \
+  -reducer example/reduce.py \
+  -partitioner example/partition.py
+```
+
+This feature is similar to Hadoop's [`Partitioner` class](https://hadoop.apache.org/docs/current/api/org/apache/hadoop/mapreduce/Partitioner.html), although it is not directly compatible with Hadoop. The main difference is that Hadoop only allows partitioners to be a Java class, while Madoop allows any executable that reads from `stdin` and writes to `stdout`.
```

### Comparing `madoop-1.2.1/madoop/__main__.py` & `madoop-1.2.2/madoop/__main__.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/madoop/example/reduce.py` & `madoop-1.2.2/madoop/example/reduce.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/madoop/mapreduce.py` & `madoop-1.2.2/madoop/mapreduce.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/madoop.egg-info/PKG-INFO` & `madoop-1.2.2/madoop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madoop
-Version: 1.2.1
+Version: 1.2.2
 Summary: A light weight MapReduce framework for education.
 Author-email: Andrew DeOrio <awdeorio@umich.edu>
 License: MIT License
         
         Copyright (c) 2021 EECS 485 Staff
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `madoop-1.2.1/madoop.egg-info/SOURCES.txt` & `madoop-1.2.2/madoop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/pyproject.toml` & `madoop-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "madoop"
-version = "1.2.1"
+version = "1.2.2"
 description="A light weight MapReduce framework for education."
 license = {file = "LICENSE"}
 authors = [
     {name = "Andrew DeOrio", email = "awdeorio@umich.edu"}
 ]
 readme = "README.md"
 keywords = [
```

### Comparing `madoop-1.2.1/tests/test_api.py` & `madoop-1.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/tests/test_cli.py` & `madoop-1.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/tests/test_stages.py` & `madoop-1.2.2/tests/test_stages.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/tests/testdata/word_count/reduce.py` & `madoop-1.2.2/tests/testdata/word_count/reduce.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/tests/testdata/word_count SPACE/reduce SPACE.py` & `madoop-1.2.2/tests/testdata/word_count SPACE/reduce SPACE.py`

 * *Files identical despite different names*

### Comparing `madoop-1.2.1/tests/utils.py` & `madoop-1.2.2/tests/utils.py`

 * *Files identical despite different names*

