# Comparing `tmp/edx-django-release-util-1.3.0.tar.gz` & `tmp/edx-django-release-util-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-release-util-1.3.0.tar", last modified: Tue Jul 25 08:45:35 2023, max compression
+gzip compressed data, was "edx-django-release-util-1.4.0.tar", last modified: Mon Apr  1 14:32:07 2024, max compression
```

## Comparing `edx-django-release-util-1.3.0.tar` & `edx-django-release-util-1.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/release_util/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/release_util/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)    12964 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/check_reserved_keywords.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/default_reserved_keywords.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/detect_missing_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5770 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/generate_history.py
--rw-r--r--   0 runner    (1001) docker     (122)     3044 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/run_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/run_specific_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/show_unapplied_migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/release_util/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0002_second.py
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0003_third.py
--rw-r--r--   0 runner    (1001) docker     (122)      733 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0004_fourth.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2930 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     8165 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2506 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/edx_django_release_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-01 14:32:07.000000 edx-django-release-util-1.4.0/edx_django_release_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-01 14:32:07.000000 edx-django-release-util-1.4.0/edx_django_release_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:32:07.000000 edx-django-release-util-1.4.0/edx_django_release_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 14:32:07.000000 edx-django-release-util-1.4.0/edx_django_release_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 14:32:07.000000 edx-django-release-util-1.4.0/edx_django_release_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.785091 edx-django-release-util-1.4.0/release_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.785091 edx-django-release-util-1.4.0/release_util/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.785091 edx-django-release-util-1.4.0/release_util/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/check_reserved_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/default_reserved_keywords.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/detect_missing_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/generate_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/run_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/run_specific_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/management/commands/show_unapplied_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.785091 edx-django-release-util-1.4.0/release_util/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.785091 edx-django-release-util-1.4.0/release_util/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0002_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0003_third.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0004_fourth.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-01 14:32:07.789091 edx-django-release-util-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-01 14:32:03.000000 edx-django-release-util-1.4.0/setup.py
```

### Comparing `edx-django-release-util-1.3.0/LICENSE` & `edx-django-release-util-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/PKG-INFO` & `edx-django-release-util-1.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: edx-django-release-util
-Version: 1.3.0
+Version: 1.4.0
 Summary: edx-django-release-util
 Home-page: http://github.com/openedx/edx-django-release-util
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Internet
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
+Requires-Dist: PyYAML
+Requires-Dist: Django
+Requires-Dist: six
 
 Part of `edX code`__.
 
 __ http://code.edx.org/
 
 edX Django Release Utilities  |Travis|_ 
 =======================================
@@ -62,18 +65,16 @@
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code in the `edx-code Google Group`__ or in the ``#edx-code`` IRC channel on Freenode.
 
 __ https://groups.google.com/forum/#!forum/edx-code
-
-
```

### Comparing `edx-django-release-util-1.3.0/README.rst` & `edx-django-release-util-1.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code in the `edx-code Google Group`__ or in the ``#edx-code`` IRC channel on Freenode.
```

### Comparing `edx-django-release-util-1.3.0/edx_django_release_util.egg-info/PKG-INFO` & `edx-django-release-util-1.4.0/edx_django_release_util.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: edx-django-release-util
-Version: 1.3.0
+Version: 1.4.0
 Summary: edx-django-release-util
 Home-page: http://github.com/openedx/edx-django-release-util
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Internet
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
+Requires-Dist: PyYAML
+Requires-Dist: Django
+Requires-Dist: six
 
 Part of `edX code`__.
 
 __ http://code.edx.org/
 
 edX Django Release Utilities  |Travis|_ 
 =======================================
@@ -62,18 +65,16 @@
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code in the `edx-code Google Group`__ or in the ``#edx-code`` IRC channel on Freenode.
 
 __ https://groups.google.com/forum/#!forum/edx-code
-
-
```

### Comparing `edx-django-release-util-1.3.0/edx_django_release_util.egg-info/SOURCES.txt` & `edx-django-release-util-1.4.0/edx_django_release_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/__init__.py` & `edx-django-release-util-1.4.0/release_util/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/check_reserved_keywords.py` & `edx-django-release-util-1.4.0/release_util/management/commands/check_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/default_reserved_keywords.yml` & `edx-django-release-util-1.4.0/release_util/management/commands/default_reserved_keywords.yml`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/detect_missing_migrations.py` & `edx-django-release-util-1.4.0/release_util/management/commands/detect_missing_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/generate_history.py` & `edx-django-release-util-1.4.0/release_util/management/commands/generate_history.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/run_migrations.py` & `edx-django-release-util-1.4.0/release_util/management/commands/run_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/run_specific_migrations.py` & `edx-django-release-util-1.4.0/release_util/management/commands/run_specific_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/management/commands/show_unapplied_migrations.py` & `edx-django-release-util-1.4.0/release_util/management/commands/show_unapplied_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0001_initial.py` & `edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0002_second.py` & `edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0002_second.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0003_third.py` & `edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0003_third.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0004_fourth.py` & `edx-django-release-util-1.4.0/release_util/tests/migrations/test_migrations/0004_fourth.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py` & `edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py` & `edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py` & `edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py` & `edx-django-release-util-1.4.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.3.0/setup.py` & `edx-django-release-util-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,12 +70,13 @@
         'Environment :: Web Environment',
         'Topic :: Internet',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
     ],
 )
```

