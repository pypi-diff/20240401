# Comparing `tmp/ambition-utils-3.1.8.tar.gz` & `tmp/ambition-utils-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambition-utils-3.1.8.tar", last modified: Thu Aug  3 15:09:45 2023, max compression
+gzip compressed data, was "ambition-utils-3.1.9.tar", last modified: Fri Aug  4 12:42:41 2023, max compression
```

## Comparing `ambition-utils-3.1.8.tar` & `ambition-utils-3.1.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.609560 ambition-utils-3.1.8/
--rw-r--r--   0 tneu       (501) staff       (20)     1075 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/LICENSE
--rw-r--r--   0 tneu       (501) staff       (20)       68 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/MANIFEST.in
--rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-08-03 15:09:45.609631 ambition-utils-3.1.8/PKG-INFO
--rw-r--r--   0 tneu       (501) staff       (20)     1114 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/README.rst
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.597344 ambition-utils-3.1.8/ambition_utils/
--rw-r--r--   0 tneu       (501) staff       (20)       48 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/__init__.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.598469 ambition-utils-3.1.8/ambition_utils/activity/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/__init__.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.599104 ambition-utils-3.1.8/ambition_utils/activity/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)     2231 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)     1656 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     4446 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/activity/models.py
--rw-r--r--   0 tneu       (501) staff       (20)     2737 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/tasks.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.599475 ambition-utils-3.1.8/ambition_utils/activity/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      229 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/activity/tests/model_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     2794 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/activity/tests/task_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.599738 ambition-utils-3.1.8/ambition_utils/anomaly/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/anomaly/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     9762 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/anomaly/models.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.600468 ambition-utils-3.1.8/ambition_utils/anomaly/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     6036 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/anomaly_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)      202 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/apps.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.600787 ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)     2644 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      928 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/anomaly/tests/models.py
--rw-r--r--   0 tneu       (501) staff       (20)      138 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)     2545 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/fields.py
--rw-r--r--   0 tneu       (501) staff       (20)    13636 2023-01-26 16:48:58.000000 ambition-utils-3.1.8/ambition_utils/forms.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.601279 ambition-utils-3.1.8/ambition_utils/postgres_lock/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     3782 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/lock.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.602014 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)      487 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)      434 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
--rw-r--r--   0 tneu       (501) staff       (20)      581 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      875 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/models.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.602235 ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     4399 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/lock_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.603343 ambition-utils-3.1.8/ambition_utils/rrule/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      162 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)      127 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/rrule/constants.py
--rw-r--r--   0 tneu       (501) staff       (20)     9900 2023-07-20 18:18:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/forms.py
--rw-r--r--   0 tneu       (501) staff       (20)      389 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/rrule/handler.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.604541 ambition-utils-3.1.8/ambition_utils/rrule/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)      927 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)      415 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
--rw-r--r--   0 tneu       (501) staff       (20)      936 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
--rw-r--r--   0 tneu       (501) staff       (20)      486 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
--rw-r--r--   0 tneu       (501) staff       (20)      412 2023-08-03 14:04:44.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/0005_auto_20230802_1548.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/rrule/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)    18906 2023-08-03 14:04:44.000000 ambition-utils-3.1.8/ambition_utils/rrule/models.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.605796 ambition-utils-3.1.8/ambition_utils/rrule/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      200 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)    18459 2023-07-20 18:18:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/form_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.606192 ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)     1005 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)    60914 2023-08-03 14:04:44.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/model_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)      713 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/rrule/tests/models.py
--rw-r--r--   0 tneu       (501) staff       (20)     7349 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/sql.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.607418 ambition-utils-3.1.8/ambition_utils/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      190 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/apps.py
--rw-r--r--   0 tneu       (501) staff       (20)     2556 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/field_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)    16249 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/form_tests.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.607987 ambition-utils-3.1.8/ambition_utils/tests/migrations/
--rw-r--r--   0 tneu       (501) staff       (20)      489 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/migrations/0001_initial.py
--rw-r--r--   0 tneu       (501) staff       (20)      685 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
--rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/migrations/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)      364 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/models.py
--rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-07-20 17:55:28.000000 ambition-utils-3.1.8/ambition_utils/tests/sql_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     3435 2022-11-29 21:40:08.000000 ambition-utils-3.1.8/ambition_utils/tests/time_helper_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     4765 2022-11-29 21:40:08.000000 ambition-utils-3.1.8/ambition_utils/time_helpers.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.608487 ambition-utils-3.1.8/ambition_utils/transaction/
--rw-r--r--   0 tneu       (501) staff       (20)       46 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     2261 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/decorators.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.608780 ambition-utils-3.1.8/ambition_utils/transaction/tests/
--rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/tests/__init__.py
--rw-r--r--   0 tneu       (501) staff       (20)     2032 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/ambition_utils/transaction/tests/durable_tests.py
--rw-r--r--   0 tneu       (501) staff       (20)     2666 2022-08-25 21:39:28.000000 ambition-utils-3.1.8/ambition_utils/transaction/utils.py
--rw-r--r--   0 tneu       (501) staff       (20)       38 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/ambition_utils/urls.py
--rw-r--r--   0 tneu       (501) staff       (20)       22 2023-08-03 14:06:21.000000 ambition-utils-3.1.8/ambition_utils/version.py
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.597983 ambition-utils-3.1.8/ambition_utils.egg-info/
--rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/PKG-INFO
--rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/SOURCES.txt
--rw-r--r--   0 tneu       (501) staff       (20)        1 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/dependency_links.txt
--rw-r--r--   0 tneu       (501) staff       (20)      262 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/requires.txt
--rw-r--r--   0 tneu       (501) staff       (20)       15 2023-08-03 15:09:45.000000 ambition-utils-3.1.8/ambition_utils.egg-info/top_level.txt
-drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-03 15:09:45.609433 ambition-utils-3.1.8/requirements/
--rw-r--r--   0 tneu       (501) staff       (20)       31 2022-08-25 20:38:52.000000 ambition-utils-3.1.8/requirements/docs.txt
--rw-r--r--   0 tneu       (501) staff       (20)       96 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/requirements/requirements-testing.txt
--rw-r--r--   0 tneu       (501) staff       (20)      160 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/requirements/requirements.txt
--rw-r--r--   0 tneu       (501) staff       (20)      252 2023-08-03 15:09:45.610101 ambition-utils-3.1.8/setup.cfg
--rw-r--r--   0 tneu       (501) staff       (20)     1914 2023-07-20 17:58:01.000000 ambition-utils-3.1.8/setup.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.611253 ambition-utils-3.1.9/
+-rw-r--r--   0 tneu       (501) staff       (20)     1075 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/LICENSE
+-rw-r--r--   0 tneu       (501) staff       (20)       68 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/MANIFEST.in
+-rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-08-04 12:42:41.611328 ambition-utils-3.1.9/PKG-INFO
+-rw-r--r--   0 tneu       (501) staff       (20)     1114 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/README.rst
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.598138 ambition-utils-3.1.9/ambition_utils/
+-rw-r--r--   0 tneu       (501) staff       (20)       48 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/__init__.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.599345 ambition-utils-3.1.9/ambition_utils/activity/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/activity/__init__.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.599956 ambition-utils-3.1.9/ambition_utils/activity/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     2231 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/activity/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)     1656 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/activity/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4446 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/activity/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2737 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/activity/tasks.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.600462 ambition-utils-3.1.9/ambition_utils/activity/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/activity/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      229 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/activity/tests/model_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2794 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/activity/tests/task_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.600718 ambition-utils-3.1.9/ambition_utils/anomaly/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/anomaly/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     9762 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/anomaly/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.601421 ambition-utils-3.1.9/ambition_utils/anomaly/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/anomaly/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     6036 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/anomaly/tests/anomaly_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)      202 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/anomaly/tests/apps.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.601758 ambition-utils-3.1.9/ambition_utils/anomaly/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     2644 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/anomaly/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/anomaly/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      928 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/anomaly/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)      138 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2545 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/fields.py
+-rw-r--r--   0 tneu       (501) staff       (20)    13636 2023-01-26 16:48:58.000000 ambition-utils-3.1.9/ambition_utils/forms.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.602215 ambition-utils-3.1.9/ambition_utils/postgres_lock/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3782 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/lock.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.602956 ambition-utils-3.1.9/ambition_utils/postgres_lock/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      487 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      434 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
+-rw-r--r--   0 tneu       (501) staff       (20)      581 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      875 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.603160 ambition-utils-3.1.9/ambition_utils/postgres_lock/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4399 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/postgres_lock/tests/lock_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.604260 ambition-utils-3.1.9/ambition_utils/rrule/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/rrule/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      162 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)      127 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/rrule/constants.py
+-rw-r--r--   0 tneu       (501) staff       (20)     9900 2023-07-20 18:18:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/forms.py
+-rw-r--r--   0 tneu       (501) staff       (20)      389 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/rrule/handler.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.605835 ambition-utils-3.1.9/ambition_utils/rrule/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      927 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/rrule/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      415 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
+-rw-r--r--   0 tneu       (501) staff       (20)      936 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+-rw-r--r--   0 tneu       (501) staff       (20)      486 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
+-rw-r--r--   0 tneu       (501) staff       (20)      412 2023-08-03 14:04:44.000000 ambition-utils-3.1.9/ambition_utils/rrule/migrations/0005_auto_20230802_1548.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/rrule/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)    19037 2023-08-03 21:29:37.000000 ambition-utils-3.1.9/ambition_utils/rrule/models.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.607206 ambition-utils-3.1.9/ambition_utils/rrule/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      200 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)    18459 2023-07-20 18:18:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/form_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.607715 ambition-utils-3.1.9/ambition_utils/rrule/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)     1005 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)    60914 2023-08-03 18:23:43.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/model_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)      713 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/rrule/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     7349 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/sql.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.609105 ambition-utils-3.1.9/ambition_utils/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      190 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/tests/apps.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2556 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/tests/field_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)    16249 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/tests/form_tests.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.609719 ambition-utils-3.1.9/ambition_utils/tests/migrations/
+-rw-r--r--   0 tneu       (501) staff       (20)      489 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/tests/migrations/0001_initial.py
+-rw-r--r--   0 tneu       (501) staff       (20)      685 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/tests/migrations/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)      364 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/tests/models.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-07-20 17:55:28.000000 ambition-utils-3.1.9/ambition_utils/tests/sql_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     3435 2022-11-29 21:40:08.000000 ambition-utils-3.1.9/ambition_utils/tests/time_helper_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     4765 2022-11-29 21:40:08.000000 ambition-utils-3.1.9/ambition_utils/time_helpers.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.610429 ambition-utils-3.1.9/ambition_utils/transaction/
+-rw-r--r--   0 tneu       (501) staff       (20)       46 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/transaction/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2261 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/transaction/decorators.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.610669 ambition-utils-3.1.9/ambition_utils/transaction/tests/
+-rw-r--r--   0 tneu       (501) staff       (20)        0 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/transaction/tests/__init__.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2032 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/ambition_utils/transaction/tests/durable_tests.py
+-rw-r--r--   0 tneu       (501) staff       (20)     2666 2022-08-25 21:39:28.000000 ambition-utils-3.1.9/ambition_utils/transaction/utils.py
+-rw-r--r--   0 tneu       (501) staff       (20)       38 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/ambition_utils/urls.py
+-rw-r--r--   0 tneu       (501) staff       (20)       22 2023-08-03 21:57:37.000000 ambition-utils-3.1.9/ambition_utils/version.py
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.598867 ambition-utils-3.1.9/ambition_utils.egg-info/
+-rw-r--r--   0 tneu       (501) staff       (20)     1995 2023-08-04 12:42:41.000000 ambition-utils-3.1.9/ambition_utils.egg-info/PKG-INFO
+-rw-r--r--   0 tneu       (501) staff       (20)     3144 2023-08-04 12:42:41.000000 ambition-utils-3.1.9/ambition_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 tneu       (501) staff       (20)        1 2023-08-04 12:42:41.000000 ambition-utils-3.1.9/ambition_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      262 2023-08-04 12:42:41.000000 ambition-utils-3.1.9/ambition_utils.egg-info/requires.txt
+-rw-r--r--   0 tneu       (501) staff       (20)       15 2023-08-04 12:42:41.000000 ambition-utils-3.1.9/ambition_utils.egg-info/top_level.txt
+drwxr-xr-x   0 tneu       (501) staff       (20)        0 2023-08-04 12:42:41.611142 ambition-utils-3.1.9/requirements/
+-rw-r--r--   0 tneu       (501) staff       (20)       31 2022-08-25 20:38:52.000000 ambition-utils-3.1.9/requirements/docs.txt
+-rw-r--r--   0 tneu       (501) staff       (20)       96 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/requirements/requirements-testing.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      160 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/requirements/requirements.txt
+-rw-r--r--   0 tneu       (501) staff       (20)      252 2023-08-04 12:42:41.611573 ambition-utils-3.1.9/setup.cfg
+-rw-r--r--   0 tneu       (501) staff       (20)     1914 2023-07-20 17:58:01.000000 ambition-utils-3.1.9/setup.py
```

### Comparing `ambition-utils-3.1.8/LICENSE` & `ambition-utils-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/PKG-INFO` & `ambition-utils-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.8
+Version: 3.1.9
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
 Platform: UNKNOWN
```

### Comparing `ambition-utils-3.1.8/README.rst` & `ambition-utils-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/activity/migrations/0001_initial.py` & `ambition-utils-3.1.9/ambition_utils/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/activity/migrations/0002_auto_20180427_1819.py` & `ambition-utils-3.1.9/ambition_utils/activity/migrations/0002_auto_20180427_1819.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/activity/models.py` & `ambition-utils-3.1.9/ambition_utils/activity/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/activity/tasks.py` & `ambition-utils-3.1.9/ambition_utils/activity/tasks.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/activity/tests/task_tests.py` & `ambition-utils-3.1.9/ambition_utils/activity/tests/task_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/anomaly/models.py` & `ambition-utils-3.1.9/ambition_utils/anomaly/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/anomaly/tests/anomaly_tests.py` & `ambition-utils-3.1.9/ambition_utils/anomaly/tests/anomaly_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/anomaly/tests/migrations/0001_initial.py` & `ambition-utils-3.1.9/ambition_utils/anomaly/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/anomaly/tests/models.py` & `ambition-utils-3.1.9/ambition_utils/anomaly/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/fields.py` & `ambition-utils-3.1.9/ambition_utils/fields.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/forms.py` & `ambition-utils-3.1.9/ambition_utils/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/postgres_lock/lock.py` & `ambition-utils-3.1.9/ambition_utils/postgres_lock/lock.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py` & `ambition-utils-3.1.9/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/postgres_lock/models.py` & `ambition-utils-3.1.9/ambition_utils/postgres_lock/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/postgres_lock/tests/lock_tests.py` & `ambition-utils-3.1.9/ambition_utils/postgres_lock/tests/lock_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/forms.py` & `ambition-utils-3.1.9/ambition_utils/rrule/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/migrations/0001_initial.py` & `ambition-utils-3.1.9/ambition_utils/rrule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py` & `ambition-utils-3.1.9/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/models.py` & `ambition-utils-3.1.9/ambition_utils/rrule/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,16 +360,16 @@
         if is_new:
             # Get the first scheduled time according to the rrule (this converts from utc back to local time)
             self.next_occurrence = self.get_rrule_set()[0]
 
             # Convert back to utc before saving
             self.next_occurrence = self.convert_to_utc(self.next_occurrence)
 
-        # Offset, if applicable, for old and new.
-        self.next_occurrence = self.offset(self.next_occurrence)
+            # Offset, if applicable, for new objects.
+            self.next_occurrence = self.offset(self.next_occurrence)
 
     def set_date_objects_for_params(self, params, is_new=False):
         """
         Give an rrule params object, ensure that the date keys are properly set and properly converted to strings
         """
         # Check for no params
         if not params:
@@ -464,17 +464,19 @@
         clone.id = None
         clone.save()
         return clone
 
     def clone_with_day_offset(self, day_offset: int) -> RRule:
         """
         Creates a clone of a passed RRule object with day_offset set.
+        clone() is not called to ensure .id is not set before .save() so offset is applied.
         :param day_offset: The number of days to offset the clone's start date. Can be negative.
         """
-        clone = self.clone()
+        clone = copy.deepcopy(self)
+        clone.id = None
         clone.day_offset = day_offset
         clone.save()
         return clone
 
     @classmethod
     def get_dates_from_params(cls, rrule_params, time_zone=None, num_dates=20, start_date=None):
         time_zone = time_zone or pytz.utc
```

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/tests/form_tests.py` & `ambition-utils-3.1.9/ambition_utils/rrule/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/tests/migrations/0001_initial.py` & `ambition-utils-3.1.9/ambition_utils/rrule/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/tests/model_tests.py` & `ambition-utils-3.1.9/ambition_utils/rrule/tests/model_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/rrule/tests/models.py` & `ambition-utils-3.1.9/ambition_utils/rrule/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/sql.py` & `ambition-utils-3.1.9/ambition_utils/sql.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/tests/field_tests.py` & `ambition-utils-3.1.9/ambition_utils/tests/field_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/tests/form_tests.py` & `ambition-utils-3.1.9/ambition_utils/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/tests/migrations/0002_auto_20230124_1754.py` & `ambition-utils-3.1.9/ambition_utils/tests/migrations/0002_auto_20230124_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/tests/sql_tests.py` & `ambition-utils-3.1.9/ambition_utils/tests/sql_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/tests/time_helper_tests.py` & `ambition-utils-3.1.9/ambition_utils/tests/time_helper_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/time_helpers.py` & `ambition-utils-3.1.9/ambition_utils/time_helpers.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/transaction/decorators.py` & `ambition-utils-3.1.9/ambition_utils/transaction/decorators.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/transaction/tests/durable_tests.py` & `ambition-utils-3.1.9/ambition_utils/transaction/tests/durable_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils/transaction/utils.py` & `ambition-utils-3.1.9/ambition_utils/transaction/utils.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/ambition_utils.egg-info/PKG-INFO` & `ambition-utils-3.1.9/ambition_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.1.8
+Version: 3.1.9
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Keywords: django,database,query,sql,postgres,upsert
 Platform: UNKNOWN
```

### Comparing `ambition-utils-3.1.8/ambition_utils.egg-info/SOURCES.txt` & `ambition-utils-3.1.9/ambition_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.1.8/setup.py` & `ambition-utils-3.1.9/setup.py`

 * *Files identical despite different names*

