# Comparing `tmp/girder-audit-logs-3.2.3.dev5.tar.gz` & `tmp/girder-audit-logs-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-audit-logs-3.2.3.dev5.tar", last modified: Wed Feb 14 15:48:43 2024, max compression
+gzip compressed data, was "girder-audit-logs-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:06 2024, max compression
```

## Comparing `girder-audit-logs-3.2.3.dev5.tar` & `girder-audit-logs-3.2.3.dev7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:43.046965 girder-audit-logs-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-02-14 15:48:43.046965 girder-audit-logs-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:43.046965 girder-audit-logs-3.2.3.dev5/girder_audit_logs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2024-02-14 15:48:26.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2024-02-14 15:48:26.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs/cleanup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2024-02-14 15:48:26.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs/report.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:43.046965 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-02-14 15:48:42.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2024-02-14 15:48:43.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:42.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-02-14 15:48:42.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:42.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:48:42.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-02-14 15:48:42.000000 girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:48:43.046965 girder-audit-logs-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1710 2024-02-14 15:48:26.000000 girder-audit-logs-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:06.433266 girder-audit-logs-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-02-14 18:47:06.433266 girder-audit-logs-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:06.429267 girder-audit-logs-3.2.3.dev7/girder_audit_logs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2024-02-14 18:46:47.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      838 2024-02-14 18:46:47.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs/cleanup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2024-02-14 18:46:47.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs/report.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:06.433266 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-02-14 18:47:06.000000 girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:06.433266 girder-audit-logs-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1710 2024-02-14 18:46:47.000000 girder-audit-logs-3.2.3.dev7/setup.py
```

### Comparing `girder-audit-logs-3.2.3.dev5/PKG-INFO` & `girder-audit-logs-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-audit-logs
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Keeps detailed logs of every REST request and low-level file download event.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-audit-logs-3.2.3.dev5/girder_audit_logs/__init__.py` & `girder-audit-logs-3.2.3.dev7/girder_audit_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.2.3.dev5/girder_audit_logs/cleanup.py` & `girder-audit-logs-3.2.3.dev7/girder_audit_logs/cleanup.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.2.3.dev5/girder_audit_logs/report.py` & `girder-audit-logs-3.2.3.dev7/girder_audit_logs/report.py`

 * *Files identical despite different names*

### Comparing `girder-audit-logs-3.2.3.dev5/girder_audit_logs.egg-info/PKG-INFO` & `girder-audit-logs-3.2.3.dev7/girder_audit_logs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-audit-logs
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Keeps detailed logs of every REST request and low-level file download event.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-audit-logs-3.2.3.dev5/setup.py` & `girder-audit-logs-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

