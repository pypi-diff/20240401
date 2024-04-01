# Comparing `tmp/Quart-0.9.0.tar.gz` & `tmp/Quart-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Quart-0.9.0.tar", last modified: Mon Apr 22 12:23:41 2019, max compression
+gzip compressed data, was "dist/Quart-0.9.1.tar", last modified: Sun May 12 15:01:35 2019, max compression
```

## Comparing `Quart-0.9.0.tar` & `Quart-0.9.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11380 2019-04-22 12:23:36.000000 Quart-0.9.0/CHANGELOG.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2017-10-10 21:09:37.000000 Quart-0.9.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      402 2019-04-22 12:23:36.000000 Quart-0.9.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2019-04-22 12:23:41.000000 Quart-0.9.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/Quart.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6454 2019-04-22 12:23:40.000000 Quart-0.9.0/Quart.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1610 2019-04-22 12:23:40.000000 Quart-0.9.0/Quart.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2019-04-22 12:23:40.000000 Quart-0.9.0/Quart.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2019-04-22 12:23:40.000000 Quart-0.9.0/Quart.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      111 2019-04-22 12:23:40.000000 Quart-0.9.0/Quart.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2019-04-22 12:23:40.000000 Quart-0.9.0/Quart.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2019-04-22 12:23:36.000000 Quart-0.9.0/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/artwork/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      550 2018-01-14 10:51:34.000000 Quart-0.9.0/artwork/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14995 2018-01-14 10:51:34.000000 Quart-0.9.0/artwork/logo.png
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/quart/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/__about__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2018-01-14 10:51:34.000000 Quart-0.9.0/quart/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67485 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9155 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/asgi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27437 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/blueprints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7142 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8934 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12731 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/ctx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22533 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/datastructures.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/debug.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4623 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/quart/flask_patch/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2386 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/flask_patch/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4204 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/flask_patch/_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2018-06-24 21:06:01.000000 Quart-0.9.0/quart/flask_patch/_synchronise.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1549 2018-06-11 16:03:28.000000 Quart-0.9.0/quart/flask_patch/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2018-06-11 16:03:28.000000 Quart-0.9.0/quart/flask_patch/globals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      932 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/globals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8267 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/quart/json/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3175 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/json/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4848 2018-01-14 10:51:34.000000 Quart-0.9.0/quart/json/tag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7488 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/local.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1119 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/py.typed
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17723 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/routing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9338 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/sessions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4287 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/signals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7795 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/static.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/templating.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12133 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/testing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/typing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2563 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3607 2018-04-14 08:31:40.000000 Quart-0.9.0/quart/views.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/quart/wrappers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      222 2018-04-14 08:31:40.000000 Quart-0.9.0/quart/wrappers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11959 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/wrappers/_base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12112 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/wrappers/request.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21520 2019-04-22 12:23:36.000000 Quart-0.9.0/quart/wrappers/response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2019-04-22 12:23:41.000000 Quart-0.9.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1866 2019-04-22 12:23:36.000000 Quart-0.9.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/tests/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/tests/assets/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2017-10-10 21:09:37.000000 Quart-0.9.0/tests/assets/config.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2017-10-10 21:09:37.000000 Quart-0.9.0/tests/assets/config.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2017-10-10 21:09:37.000000 Quart-0.9.0/tests/assets/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11245 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_asgi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4580 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_basic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_blueprints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1603 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2147 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_ctx.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_datastructures.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_debug.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1043 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4902 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1172 2018-01-14 10:51:34.000000 Quart-0.9.0/tests/test_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2018-07-15 19:12:55.000000 Quart-0.9.0/tests/test_local.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10743 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_routing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4472 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_sessions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      775 2019-01-29 15:46:45.000000 Quart-0.9.0/tests/test_signals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3856 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_static.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3976 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_templating.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6086 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_testing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2018-12-16 20:09:19.000000 Quart-0.9.0/tests/test_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2028 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/test_views.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-04-22 12:23:41.000000 Quart-0.9.0/tests/wrappers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4033 2018-07-15 19:12:55.000000 Quart-0.9.0/tests/wrappers/test_base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/wrappers/test_request.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5445 2019-04-22 12:23:36.000000 Quart-0.9.0/tests/wrappers/test_response.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11592 2019-05-12 15:01:25.000000 Quart-0.9.1/CHANGELOG.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2017-10-10 21:09:37.000000 Quart-0.9.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      402 2019-04-22 12:23:36.000000 Quart-0.9.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6783 2019-05-12 15:01:35.000000 Quart-0.9.1/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6783 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1610 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      111 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2019-05-12 15:01:35.000000 Quart-0.9.1/Quart.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4733 2019-05-12 15:01:25.000000 Quart-0.9.1/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/artwork/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      550 2018-01-14 10:51:34.000000 Quart-0.9.1/artwork/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14995 2018-01-14 10:51:34.000000 Quart-0.9.1/artwork/logo.png
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/quart/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2019-05-12 15:01:25.000000 Quart-0.9.1/quart/__about__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2018-01-14 10:51:34.000000 Quart-0.9.1/quart/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67485 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9155 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/asgi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27437 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/blueprints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7142 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8934 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12731 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/ctx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22533 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/datastructures.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/debug.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4623 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/quart/flask_patch/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2386 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/flask_patch/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4204 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/flask_patch/_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2018-06-24 21:06:01.000000 Quart-0.9.1/quart/flask_patch/_synchronise.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1549 2018-06-11 16:03:28.000000 Quart-0.9.1/quart/flask_patch/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2018-06-11 16:03:28.000000 Quart-0.9.1/quart/flask_patch/globals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      932 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/globals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8267 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/helpers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/quart/json/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3175 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/json/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4848 2018-01-14 10:51:34.000000 Quart-0.9.1/quart/json/tag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7575 2019-05-12 15:01:25.000000 Quart-0.9.1/quart/local.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1119 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/py.typed
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17723 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/routing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9338 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/sessions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4287 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/signals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7793 2019-05-12 15:01:25.000000 Quart-0.9.1/quart/static.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/templating.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12151 2019-05-12 15:01:25.000000 Quart-0.9.1/quart/testing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/typing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2563 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3607 2018-04-14 08:31:40.000000 Quart-0.9.1/quart/views.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/quart/wrappers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      222 2018-04-14 08:31:40.000000 Quart-0.9.1/quart/wrappers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11959 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/wrappers/_base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12174 2019-05-12 15:01:25.000000 Quart-0.9.1/quart/wrappers/request.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21520 2019-04-22 12:23:36.000000 Quart-0.9.1/quart/wrappers/response.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      975 2019-05-12 15:01:35.000000 Quart-0.9.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1887 2019-05-12 15:01:25.000000 Quart-0.9.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/tests/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/tests/assets/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2017-10-10 21:09:37.000000 Quart-0.9.1/tests/assets/config.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2017-10-10 21:09:37.000000 Quart-0.9.1/tests/assets/config.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2017-10-10 21:09:37.000000 Quart-0.9.1/tests/assets/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11298 2019-05-12 15:01:25.000000 Quart-0.9.1/tests/test_app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5060 2019-05-12 15:01:25.000000 Quart-0.9.1/tests/test_asgi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4580 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_basic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_blueprints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1603 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2147 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8794 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_ctx.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_datastructures.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_debug.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1043 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4902 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1172 2018-01-14 10:51:34.000000 Quart-0.9.1/tests/test_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2018-07-15 19:12:55.000000 Quart-0.9.1/tests/test_local.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10743 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_routing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4472 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_sessions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      775 2019-01-29 15:46:45.000000 Quart-0.9.1/tests/test_signals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3856 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_static.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3976 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_templating.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6129 2019-05-12 15:01:25.000000 Quart-0.9.1/tests/test_testing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2018-12-16 20:09:19.000000 Quart-0.9.1/tests/test_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2028 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/test_views.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2019-05-12 15:01:35.000000 Quart-0.9.1/tests/wrappers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4033 2018-07-15 19:12:55.000000 Quart-0.9.1/tests/wrappers/test_base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/wrappers/test_request.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5445 2019-04-22 12:23:36.000000 Quart-0.9.1/tests/wrappers/test_response.py
```

### Comparing `Quart-0.9.0/CHANGELOG.rst` & `Quart-0.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.9.1 2019-05-12
+----------------
+
+* Bugfix unquote the path in the test client, following the ASGI
+  standard.
+* Bugfix follow Werkzeug LocalProxy name API.
+* Bugfix ensure multiple files are correctly loaded.
+
 0.9.0 2019-04-22
 ----------------
 
 *This contains all the Bugfixes in the 0.6 and 0.8 branches.*
 
 * Highlight the traceback line of code when using the debug system.
 * Bugfix ensure debug has an affect when passed to app run.
```

### Comparing `Quart-0.9.0/LICENSE` & `Quart-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/PKG-INFO` & `Quart-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quart
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python ASGI web microframework with the same API as Flask
 Home-page: https://gitlab.com/pgjones/quart/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Description: Quart
         =====
@@ -86,36 +86,41 @@
         Note that not all ASGI servers support these features, for this reason
         the recommended server is `Hypercorn
         <https://gitlab.com/pgjones/hypercorn>`_.
         
         Contributing
         ------------
         
-        Quart is developed on `GitLab
-        <https://gitlab.com/pgjones/quart>`_. You are very welcome to open
-        `issues <https://gitlab.com/pgjones/quart/issues>`_ or propose `merge
-        requests <https://gitlab.com/pgjones/quart/merge_requests>`_.
+        Quart is developed on `GitLab <https://gitlab.com/pgjones/quart>`_. If
+        you come across an issue, or have a feature request please open an
+        `issue <https://gitlab.com/pgjones/quart/issues>`_.  If you want to
+        contribute a fix or the feature-implementation please do (typo fixes
+        welcome), by proposing a `merge request
+        <https://gitlab.com/pgjones/quart/merge_requests>`_.
         
         Testing
         ~~~~~~~
         
-        The best way to test Quart is with Tox,
+        The best way to test Quart is with `Tox
+        <https://tox.readthedocs.io>`_,
         
         .. code-block:: console
         
             $ pipenv install tox
             $ tox
         
         this will check the code style and run the tests.
         
         Help
         ----
         
         The Quart `documentation <https://pgjones.gitlab.io/quart/>`_ is the
-        best place to start, after that try opening an `issue
+        best place to start, after that try searching `stack overflow
+        <https://stackoverflow.com/questions/tagged/quart>`_, if you still
+        can't find an answer please `open an issue
         <https://gitlab.com/pgjones/quart/issues>`_.
         
         API Compatibility with Flask
         ----------------------------
         
         The Flask API can be described as consisting of the Flask public and
         private APIs and Werkzeug upon which Flask is based. Quart is designed
```

### Comparing `Quart-0.9.0/Quart.egg-info/PKG-INFO` & `Quart-0.9.1/Quart.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quart
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python ASGI web microframework with the same API as Flask
 Home-page: https://gitlab.com/pgjones/quart/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Description: Quart
         =====
@@ -86,36 +86,41 @@
         Note that not all ASGI servers support these features, for this reason
         the recommended server is `Hypercorn
         <https://gitlab.com/pgjones/hypercorn>`_.
         
         Contributing
         ------------
         
-        Quart is developed on `GitLab
-        <https://gitlab.com/pgjones/quart>`_. You are very welcome to open
-        `issues <https://gitlab.com/pgjones/quart/issues>`_ or propose `merge
-        requests <https://gitlab.com/pgjones/quart/merge_requests>`_.
+        Quart is developed on `GitLab <https://gitlab.com/pgjones/quart>`_. If
+        you come across an issue, or have a feature request please open an
+        `issue <https://gitlab.com/pgjones/quart/issues>`_.  If you want to
+        contribute a fix or the feature-implementation please do (typo fixes
+        welcome), by proposing a `merge request
+        <https://gitlab.com/pgjones/quart/merge_requests>`_.
         
         Testing
         ~~~~~~~
         
-        The best way to test Quart is with Tox,
+        The best way to test Quart is with `Tox
+        <https://tox.readthedocs.io>`_,
         
         .. code-block:: console
         
             $ pipenv install tox
             $ tox
         
         this will check the code style and run the tests.
         
         Help
         ----
         
         The Quart `documentation <https://pgjones.gitlab.io/quart/>`_ is the
-        best place to start, after that try opening an `issue
+        best place to start, after that try searching `stack overflow
+        <https://stackoverflow.com/questions/tagged/quart>`_, if you still
+        can't find an answer please `open an issue
         <https://gitlab.com/pgjones/quart/issues>`_.
         
         API Compatibility with Flask
         ----------------------------
         
         The Flask API can be described as consisting of the Flask public and
         private APIs and Werkzeug upon which Flask is based. Quart is designed
```

### Comparing `Quart-0.9.0/Quart.egg-info/SOURCES.txt` & `Quart-0.9.1/Quart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/README.rst` & `Quart-0.9.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -78,36 +78,41 @@
 Note that not all ASGI servers support these features, for this reason
 the recommended server is `Hypercorn
 <https://gitlab.com/pgjones/hypercorn>`_.
 
 Contributing
 ------------
 
-Quart is developed on `GitLab
-<https://gitlab.com/pgjones/quart>`_. You are very welcome to open
-`issues <https://gitlab.com/pgjones/quart/issues>`_ or propose `merge
-requests <https://gitlab.com/pgjones/quart/merge_requests>`_.
+Quart is developed on `GitLab <https://gitlab.com/pgjones/quart>`_. If
+you come across an issue, or have a feature request please open an
+`issue <https://gitlab.com/pgjones/quart/issues>`_.  If you want to
+contribute a fix or the feature-implementation please do (typo fixes
+welcome), by proposing a `merge request
+<https://gitlab.com/pgjones/quart/merge_requests>`_.
 
 Testing
 ~~~~~~~
 
-The best way to test Quart is with Tox,
+The best way to test Quart is with `Tox
+<https://tox.readthedocs.io>`_,
 
 .. code-block:: console
 
     $ pipenv install tox
     $ tox
 
 this will check the code style and run the tests.
 
 Help
 ----
 
 The Quart `documentation <https://pgjones.gitlab.io/quart/>`_ is the
-best place to start, after that try opening an `issue
+best place to start, after that try searching `stack overflow
+<https://stackoverflow.com/questions/tagged/quart>`_, if you still
+can't find an answer please `open an issue
 <https://gitlab.com/pgjones/quart/issues>`_.
 
 API Compatibility with Flask
 ----------------------------
 
 The Flask API can be described as consisting of the Flask public and
 private APIs and Werkzeug upon which Flask is based. Quart is designed
```

### Comparing `Quart-0.9.0/artwork/LICENSE` & `Quart-0.9.1/artwork/LICENSE`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/artwork/logo.png` & `Quart-0.9.1/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/__init__.py` & `Quart-0.9.1/quart/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/app.py` & `Quart-0.9.1/quart/app.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/asgi.py` & `Quart-0.9.1/quart/asgi.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/blueprints.py` & `Quart-0.9.1/quart/blueprints.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/cli.py` & `Quart-0.9.1/quart/cli.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/config.py` & `Quart-0.9.1/quart/config.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/ctx.py` & `Quart-0.9.1/quart/ctx.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/datastructures.py` & `Quart-0.9.1/quart/datastructures.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/debug.py` & `Quart-0.9.1/quart/debug.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/exceptions.py` & `Quart-0.9.1/quart/exceptions.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/flask_patch/__init__.py` & `Quart-0.9.1/quart/flask_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/flask_patch/_patch.py` & `Quart-0.9.1/quart/flask_patch/_patch.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/flask_patch/_synchronise.py` & `Quart-0.9.1/quart/flask_patch/_synchronise.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/flask_patch/app.py` & `Quart-0.9.1/quart/flask_patch/app.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/flask_patch/globals.py` & `Quart-0.9.1/quart/flask_patch/globals.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/globals.py` & `Quart-0.9.1/quart/globals.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/helpers.py` & `Quart-0.9.1/quart/helpers.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/json/__init__.py` & `Quart-0.9.1/quart/json/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/json/tag.py` & `Quart-0.9.1/quart/json/tag.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/local.py` & `Quart-0.9.1/quart/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import copy
 from contextvars import ContextVar  # noqa # contextvars not understood as stdlib
-from typing import Any, Callable, Dict  # noqa # contextvars not understood as stdlib
+from typing import Any, Callable, Dict, Optional  # noqa # contextvars not understood as stdlib
 
 
 class TaskLocal:
     """An object local to the current task."""
 
     __slots__ = ('_storage',)
 
@@ -70,18 +70,19 @@
             return None
 
 
 class LocalProxy:
     """Proxy to a task local object."""
     __slots__ = ('__dict__', '__local', '__wrapped__')
 
-    def __init__(self, local: Callable) -> None:
+    def __init__(self, local: Callable, name: Optional[str]=None) -> None:
         # Note as __setattr__ is overidden below, use the object __setattr__
         object.__setattr__(self, '__LocalProxy_local', local)
         object.__setattr__(self, '__wrapped__', local)
+        object.__setattr__(self, "__name__", name)
 
     def _get_current_object(self) -> Any:
         return object.__getattribute__(self, '__LocalProxy_local')()
 
     @property
     def __dict__(self) -> Dict[str, Any]:  # type: ignore
         try:
```

### Comparing `Quart-0.9.0/quart/logging.py` & `Quart-0.9.1/quart/logging.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/routing.py` & `Quart-0.9.1/quart/routing.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/sessions.py` & `Quart-0.9.1/quart/sessions.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/signals.py` & `Quart-0.9.1/quart/signals.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/static.py` & `Quart-0.9.1/quart/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,16 @@
     """Send a file from a given directory.
 
     Arguments:
        directory: Directory that when combined with file_name gives
            the file path.
        file_name: File name that when combined with directory gives
            the file path.
-       See :func:`send_file` for the other arguments.
+
+    See :func:`send_file` for the other arguments.
     """
     file_path = safe_join(directory, file_name)
     if not file_path.is_file():
         raise NotFound()
     return await send_file(
         file_path,
         mimetype=mimetype,
```

### Comparing `Quart-0.9.0/quart/templating.py` & `Quart-0.9.1/quart/templating.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/testing.py` & `Quart-0.9.1/quart/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from contextlib import asynccontextmanager
 from datetime import datetime, timedelta
 from http.cookies import SimpleCookie
 from json import dumps
 from typing import Any, AnyStr, AsyncGenerator, List, Optional, Tuple, TYPE_CHECKING, Union
-from urllib.parse import urlencode
+from urllib.parse import unquote, urlencode
 
 from .datastructures import CIMultiDict, Headers
 from .exceptions import BadRequest
 from .utils import create_cookie
 from .wrappers import Request, Response
 
 if TYPE_CHECKING:
@@ -80,15 +80,15 @@
     if '?' in path and query_string is not None:
         raise ValueError('Query string is defined in the path and as an argument')
     if query_string is None:
         path, _, query_string_raw = path.partition('?')
     else:
         query_string_raw = urlencode(query_string, doseq=True)
     query_string_bytes = query_string_raw.encode('ascii')
-    return headers, path, query_string_bytes
+    return headers, unquote(path), query_string_bytes
 
 
 async def no_op_push(path: str, headers: Headers) -> None:
     """A push promise sender that does nothing.
 
     This is best used when creating Request instances for testing
     outside of the QuartClient. The Request instance must know what to
```

### Comparing `Quart-0.9.0/quart/typing.py` & `Quart-0.9.1/quart/typing.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/utils.py` & `Quart-0.9.1/quart/utils.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/views.py` & `Quart-0.9.1/quart/views.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/wrappers/_base.py` & `Quart-0.9.1/quart/wrappers/_base.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/quart/wrappers/request.py` & `Quart-0.9.1/quart/wrappers/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -226,25 +226,28 @@
                 io.BytesIO(raw_data), headers=self.headers,
                 environ={'REQUEST_METHOD': 'POST'}, limit=len(raw_data),
             )
             for key in field_storage:  # type: ignore
                 field_storage_key = field_storage[key]
                 if isinstance(field_storage_key, list):
                     for item in field_storage_key:
-                        self._form.add(key, item.value)
-                elif (
-                        isinstance(field_storage_key, FieldStorage) and
-                        field_storage_key.filename is not None
-                ):
-                    self._files[key] = FileStorage(  # type: ignore
-                        io.BytesIO(field_storage_key.file.read()), field_storage_key.filename,
-                        field_storage_key.name, field_storage_key.type, field_storage_key.headers,  # type: ignore # noqa: E501
-                    )
-                elif key:
-                    self._form.add(key, field_storage_key.value)
+                        self._load_field_storage(key, item)
+                else:
+                    self._load_field_storage(key, field_storage_key)
+
+    def _load_field_storage(self, key: str, field_storage: FieldStorage) -> None:
+        if isinstance(field_storage, FieldStorage) and field_storage.filename is not None:
+            self._files.add(
+                key, FileStorage(  # type: ignore
+                    io.BytesIO(field_storage.file.read()), field_storage.filename,
+                    field_storage.name, field_storage.type, field_storage.headers,  # type: ignore # noqa: E501
+                ),
+            )
+        else:
+            self._form.add(key, field_storage.value)
 
     @property
     def content_encoding(self) -> Optional[str]:
         return self.headers.get('Content-Encoding')
 
     @property
     def content_length(self) -> Optional[int]:
```

### Comparing `Quart-0.9.0/quart/wrappers/response.py` & `Quart-0.9.1/quart/wrappers/response.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/setup.cfg` & `Quart-0.9.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 [mypy-_pytest.*]
 ignore_missing_imports = True
 
 [mypy-aiofiles.*]
 ignore_missing_imports = True
 
+[mypy-asynctest.*]
+ignore_missing_imports = True
+
 [mypy-blinker.*]
 ignore_missing_imports = True
 
 [mypy-dotenv.*]
 ignore_missing_imports = True
 
 [mypy-flask.*]
```

### Comparing `Quart-0.9.0/setup.py` & `Quart-0.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open(os.path.join(PROJECT_ROOT, 'README.rst')) as file_:
     long_description = file_.read()
 
 INSTALL_REQUIRES = [
     'aiofiles',
     'blinker',
     'click',
-    'hypercorn >= 0.5.0',
+    'hypercorn >= 0.6.0',
     'itsdangerous',
     'jinja2',
     'multidict',
     'sortedcontainers',
 ]
 
 setup(
@@ -48,14 +48,15 @@
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     packages=find_packages(exclude=["tests", "tests.*"]),
     py_modules=['quart'],
     install_requires=INSTALL_REQUIRES,
     tests_require=INSTALL_REQUIRES + [
+        'asynctest',
         'hypothesis',
         'pytest',
         'pytest-asyncio',
     ],
     extras_require={
         'dotenv': ['python-dotenv'],
     },
```

### Comparing `Quart-0.9.0/tests/test_app.py` & `Quart-0.9.1/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 import os
 from typing import NoReturn, Optional, Set
-from unittest.mock import Mock
 
 import pytest
+from asynctest import Mock as AsyncMock
 
 from quart.app import Quart
 from quart.datastructures import CIMultiDict
 from quart.globals import session, websocket
-from quart.sessions import SecureCookieSession
+from quart.sessions import SecureCookieSession, SessionInterface
 from quart.testing import no_op_push, WebsocketResponse
 from quart.typing import ResponseReturnValue
 from quart.wrappers import Response
 
 TEST_RESPONSE = Response('')
 
 
@@ -306,15 +306,15 @@
     with pytest.raises(asyncio.CancelledError):
         await app.handle_websocket(websocket)
 
 
 @pytest.fixture(name='session_app', scope="function")
 def _session_app() -> Quart:
     app = Quart(__name__)
-    app.session_interface = Mock()
+    app.session_interface = AsyncMock(spec=SessionInterface)
     app.session_interface.open_session.return_value = SecureCookieSession()  # type: ignore
     app.session_interface.is_null_session.return_value = False  # type: ignore
 
     @app.route('/')
     async def route() -> str:
         session["a"] = "b"
         return ''
```

### Comparing `Quart-0.9.0/tests/test_asgi.py` & `Quart-0.9.1/tests/test_asgi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 from typing import Optional
 
 import pytest
+from asynctest.mock import CoroutineMock
 
 from quart import Quart
 from quart.asgi import (
     _convert_version, _encode_headers, ASGIHTTPConnection, ASGIWebsocketConnection,
 )
 from quart.datastructures import Headers
 
@@ -130,26 +131,28 @@
         ({"asgi": {"spec_version": "2.1.1"}}, Headers({"a": "b"}), None, True),
     ],
 )
 async def test_websocket_accept_connection(
         scope: dict, headers: Headers, subprotocol: Optional[str], has_headers: bool,
 ) -> None:
     connection = ASGIWebsocketConnection(Quart(__name__), scope)
-    sent_message = None
-
-    async def mock_send(message: dict) -> None:
-        nonlocal sent_message
-        sent_message = message
-
+    mock_send = CoroutineMock()
     await connection.accept_connection(mock_send, headers, subprotocol)
 
     if has_headers:
-        assert sent_message["headers"]
-    if subprotocol is not None:
-        assert sent_message["subprotocol"] == subprotocol
+        mock_send.assert_called_with({
+            "subprotocol": subprotocol,
+            "type": "websocket.accept",
+            "headers": _encode_headers(headers),
+        })
+    else:
+        mock_send.assert_called_with({
+            "subprotocol": subprotocol,
+            "type": "websocket.accept",
+        })
 
 
 @pytest.mark.asyncio
 async def test_websocket_accept_connection_warns() -> None:
     connection = ASGIWebsocketConnection(Quart(__name__), {})
 
     async def mock_send(message: dict) -> None:
```

### Comparing `Quart-0.9.0/tests/test_basic.py` & `Quart-0.9.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_blueprints.py` & `Quart-0.9.1/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_cli.py` & `Quart-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_config.py` & `Quart-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_ctx.py` & `Quart-0.9.1/tests/test_ctx.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_datastructures.py` & `Quart-0.9.1/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_debug.py` & `Quart-0.9.1/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_exceptions.py` & `Quart-0.9.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_helpers.py` & `Quart-0.9.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_json.py` & `Quart-0.9.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_local.py` & `Quart-0.9.1/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_routing.py` & `Quart-0.9.1/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_sessions.py` & `Quart-0.9.1/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_signals.py` & `Quart-0.9.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_static.py` & `Quart-0.9.1/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_templating.py` & `Quart-0.9.1/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_testing.py` & `Quart-0.9.1/tests/test_testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 @pytest.mark.parametrize(
     'path, query_string, expected_path, expected_query_string',
     [
         ('/path', {'a': 'b'}, '/path', b'a=b'),
         ('/path', {'a': ['b', 'c']}, '/path', b'a=b&a=c'),
         ('/path?b=c', None, '/path', b'b=c'),
+        ('/path%20', None, '/path ', b''),
     ],
 )
 def test_build_headers_path_and_query_string(
         path: str,
         query_string: Optional[dict],
         expected_path: str,
         expected_query_string: bytes,
```

### Comparing `Quart-0.9.0/tests/test_utils.py` & `Quart-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/test_views.py` & `Quart-0.9.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/wrappers/test_base.py` & `Quart-0.9.1/tests/wrappers/test_base.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/wrappers/test_request.py` & `Quart-0.9.1/tests/wrappers/test_request.py`

 * *Files identical despite different names*

### Comparing `Quart-0.9.0/tests/wrappers/test_response.py` & `Quart-0.9.1/tests/wrappers/test_response.py`

 * *Files identical despite different names*

