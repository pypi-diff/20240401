# Comparing `tmp/girder-jobs-3.2.3.dev5.tar.gz` & `tmp/girder-jobs-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-jobs-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:23 2024, max compression
+gzip compressed data, was "girder-jobs-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:46 2024, max compression
```

## Comparing `girder-jobs-3.2.3.dev5.tar` & `girder-jobs-3.2.3.dev7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.691181 girder-jobs-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-02-14 15:49:23.691181 girder-jobs-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.683181 girder-jobs-3.2.3.dev5/girder_jobs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/job_rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.683181 girder-jobs-3.2.3.dev5/girder_jobs/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23250 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/models/job.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/girder_jobs/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/JobStatus.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/girder_jobs/web_client/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/collections/JobCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/girder_jobs/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/models/JobModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/girder_jobs/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/stylesheets/jobListWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/adminViewMenuItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/headerUserViewMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobCheckBoxContent.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2232 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobDetailsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobListWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobsGraphWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/CheckBoxMenu.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4906 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8414 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/JobGraphWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12083 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/JobListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/timeChartConfig.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/timingHistoryChartConfig.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.691181 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1802 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 15:49:23.000000 girder-jobs-3.2.3.dev5/girder_jobs.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:23.687181 girder-jobs-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21567 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/plugin_tests/jobsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/plugin_tests/jobs_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/plugin_tests/local_job_impl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:23.691181 girder-jobs-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-02-14 15:48:27.000000 girder-jobs-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.149327 girder-jobs-3.2.3.dev7/girder_jobs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/job_rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.149327 girder-jobs-3.2.3.dev7/girder_jobs/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23250 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/models/job.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.149327 girder-jobs-3.2.3.dev7/girder_jobs/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/JobStatus.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.149327 girder-jobs-3.2.3.dev7/girder_jobs/web_client/collections/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/collections/JobCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/collections/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.149327 girder-jobs-3.2.3.dev7/girder_jobs/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/models/JobModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/models/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.149327 girder-jobs-3.2.3.dev7/girder_jobs/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/stylesheets/jobListWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/adminViewMenuItem.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/headerUserViewMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobCheckBoxContent.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2232 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobDetailsWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobListWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobsGraphWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/AdminView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/CheckBoxMenu.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/HeaderUserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4906 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/JobDetailsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8414 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/JobGraphWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12083 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/JobListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/timeChartConfig.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/timingHistoryChartConfig.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1802 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 18:47:46.000000 girder-jobs-3.2.3.dev7/girder_jobs.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21567 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/plugin_tests/jobsSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/plugin_tests/jobs_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/plugin_tests/local_job_impl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:46.153327 girder-jobs-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-02-14 18:46:47.000000 girder-jobs-3.2.3.dev7/setup.py
```

### Comparing `girder-jobs-3.2.3.dev5/PKG-INFO` & `girder-jobs-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-jobs
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: A general purpose plugin for managing offline jobs.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#jobs
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/__init__.py` & `girder-jobs-3.2.3.dev7/girder_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/constants.py` & `girder-jobs-3.2.3.dev7/girder_jobs/constants.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/job_rest.py` & `girder-jobs-3.2.3.dev7/girder_jobs/job_rest.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/models/job.py` & `girder-jobs-3.2.3.dev7/girder_jobs/models/job.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/JobStatus.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/JobStatus.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/models/JobModel.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/models/JobModel.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/package.json` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/routes.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/stylesheets/jobListWidget.styl` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/stylesheets/jobListWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobDetailsWidget.pug` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobDetailsWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobList.pug` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobList.pug`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/templates/jobListWidget.pug` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/templates/jobListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/CheckBoxMenu.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/CheckBoxMenu.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/HeaderUserView.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/JobDetailsWidget.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/JobDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/JobGraphWidget.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/JobGraphWidget.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/JobListWidget.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/JobListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/timeChartConfig.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/timeChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs/web_client/views/timingHistoryChartConfig.js` & `girder-jobs-3.2.3.dev7/girder_jobs/web_client/views/timingHistoryChartConfig.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs.egg-info/PKG-INFO` & `girder-jobs-3.2.3.dev7/girder_jobs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-jobs
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: A general purpose plugin for managing offline jobs.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#jobs
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-jobs-3.2.3.dev5/girder_jobs.egg-info/SOURCES.txt` & `girder-jobs-3.2.3.dev7/girder_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/plugin_tests/jobsSpec.js` & `girder-jobs-3.2.3.dev7/plugin_tests/jobsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/plugin_tests/jobs_test.py` & `girder-jobs-3.2.3.dev7/plugin_tests/jobs_test.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.3.dev5/setup.py` & `girder-jobs-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

