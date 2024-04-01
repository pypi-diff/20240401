# Comparing `tmp/edx-celeryutils-1.2.5.tar.gz` & `tmp/edx-celeryutils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-celeryutils-1.2.5.tar", last modified: Thu Feb  1 09:52:52 2024, max compression
+gzip compressed data, was "edx-celeryutils-1.3.0.tar", last modified: Mon Apr  1 19:51:25 2024, max compression
```

## Comparing `edx-celeryutils-1.2.5.tar` & `edx-celeryutils-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.097196 edx-celeryutils-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-02-01 09:52:52.097196 edx-celeryutils-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.093196 edx-celeryutils-1.2.5/celery_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/logged_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.093196 edx-celeryutils-1.2.5/celery_utils/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.093196 edx-celeryutils-1.2.5/celery_utils/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/commands/cleanup_resolved_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/commands/reapply_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.093196 edx-celeryutils-1.2.5/celery_utils/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/management/commands/tests/test_reapply_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.093196 edx-celeryutils-1.2.5/celery_utils/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/migrations/0002_chordable_django_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/persist_on_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/celery_utils/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.097196 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-02-01 09:52:52.000000 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-01 09:52:52.000000 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 09:52:52.000000 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 09:52:52.000000 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-01 09:52:52.000000 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-01 09:52:52.000000 edx-celeryutils-1.2.5/edx_celeryutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.097196 edx-celeryutils-1.2.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-01 09:52:52.097196 edx-celeryutils-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:52:52.097196 edx-celeryutils-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/tests/test_logged_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-01 09:52:44.000000 edx-celeryutils-1.2.5/tests/test_persist_on_failure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.782978 edx-celeryutils-1.3.0/celery_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/logged_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.782978 edx-celeryutils-1.3.0/celery_utils/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/celery_utils/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/commands/cleanup_resolved_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/commands/reapply_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/celery_utils/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/management/commands/tests/test_reapply_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/celery_utils/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/migrations/0002_chordable_django_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/persist_on_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/celery_utils/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-01 19:51:25.000000 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 19:51:25.000000 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:51:25.000000 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:51:25.000000 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 19:51:25.000000 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 19:51:25.000000 edx-celeryutils-1.3.0/edx_celeryutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:25.786978 edx-celeryutils-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/tests/test_logged_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-01 19:51:22.000000 edx-celeryutils-1.3.0/tests/test_persist_on_failure.py
```

### Comparing `edx-celeryutils-1.2.5/CHANGELOG.rst` & `edx-celeryutils-1.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[1.3.0] - 2024-03-31
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
 [1.2.5] - 2024-02-01
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Ran django-upgrade tool to add support for Django 4.2 in missing files.
 
 [1.2.3] - 2023-06-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support added for Django 4.2.
```

### Comparing `edx-celeryutils-1.2.5/LICENSE.txt` & `edx-celeryutils-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/PKG-INFO` & `edx-celeryutils-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: edx-celeryutils
-Version: 1.2.5
+Version: 1.3.0
 Summary: Code to support working with celery
 Home-page: https://github.com/openedx/edx-celeryutils
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: Django
 Requires-Dist: celery<6.0
 Requires-Dist: django-model-utils
 Requires-Dist: jsonfield
 
@@ -120,14 +119,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[1.3.0] - 2024-03-31
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
 [1.2.5] - 2024-02-01
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Ran django-upgrade tool to add support for Django 4.2 in missing files.
 
 [1.2.3] - 2023-06-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support added for Django 4.2.
```

### Comparing `edx-celeryutils-1.2.5/README.rst` & `edx-celeryutils-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/logged_task.py` & `edx-celeryutils-1.3.0/celery_utils/logged_task.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/management/commands/cleanup_resolved_tasks.py` & `edx-celeryutils-1.3.0/celery_utils/management/commands/cleanup_resolved_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/management/commands/reapply_tasks.py` & `edx-celeryutils-1.3.0/celery_utils/management/commands/reapply_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py` & `edx-celeryutils-1.3.0/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/management/commands/tests/test_reapply_tasks.py` & `edx-celeryutils-1.3.0/celery_utils/management/commands/tests/test_reapply_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/migrations/0001_initial.py` & `edx-celeryutils-1.3.0/celery_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/models.py` & `edx-celeryutils-1.3.0/celery_utils/models.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/persist_on_failure.py` & `edx-celeryutils-1.3.0/celery_utils/persist_on_failure.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/celery_utils/tasks.py` & `edx-celeryutils-1.3.0/celery_utils/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/edx_celeryutils.egg-info/PKG-INFO` & `edx-celeryutils-1.3.0/edx_celeryutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: edx-celeryutils
-Version: 1.2.5
+Version: 1.3.0
 Summary: Code to support working with celery
 Home-page: https://github.com/openedx/edx-celeryutils
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: Django
 Requires-Dist: celery<6.0
 Requires-Dist: django-model-utils
 Requires-Dist: jsonfield
 
@@ -120,14 +119,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[1.3.0] - 2024-03-31
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added python3.11 and 3.12 support. Dropped django32 support.
+
 [1.2.5] - 2024-02-01
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Ran django-upgrade tool to add support for Django 4.2 in missing files.
 
 [1.2.3] - 2023-06-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support added for Django 4.2.
```

### Comparing `edx-celeryutils-1.2.5/edx_celeryutils.egg-info/SOURCES.txt` & `edx-celeryutils-1.3.0/edx_celeryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/requirements/constraints.txt` & `edx-celeryutils-1.3.0/requirements/constraints.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 # linking to it here is good.
 
 # This file contains all common constraints for edx-repos
 -c common_constraints.txt
 
 # pinning it to latest release.
 celery<6.0
+
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `edx-celeryutils-1.2.5/setup.py` & `edx-celeryutils-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,18 +114,17 @@
     install_requires=load_requirements('requirements/base.in'),
     license="Apache 2.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
-        'Framework :: Django :: 4.1',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `edx-celeryutils-1.2.5/tests/test_logged_task.py` & `edx-celeryutils-1.3.0/tests/test_logged_task.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.5/tests/test_persist_on_failure.py` & `edx-celeryutils-1.3.0/tests/test_persist_on_failure.py`

 * *Files identical despite different names*

