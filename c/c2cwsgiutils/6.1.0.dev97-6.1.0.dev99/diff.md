# Comparing `tmp/c2cwsgiutils-6.1.0.dev97.tar.gz` & `tmp/c2cwsgiutils-6.1.0.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2cwsgiutils-6.1.0.dev97.tar", max compression
+gzip compressed data, was "c2cwsgiutils-6.1.0.dev99.tar", max compression
```

## Comparing `c2cwsgiutils-6.1.0.dev97.tar` & `c2cwsgiutils-6.1.0.dev99.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1304 2024-03-03 11:39:25.704383 c2cwsgiutils-6.1.0.dev97/LICENSE
--rw-r--r--   0        0        0    30298 2024-03-03 11:39:25.704383 c2cwsgiutils-6.1.0.dev97/README.md
--rw-r--r--   0        0        0     3986 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/__init__.py
--rw-r--r--   0        0        0     1500 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/__init__.py
--rw-r--r--   0        0        0     9742 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/connection.py
--rw-r--r--   0        0        0     8769 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/image.py
--rw-r--r--   0        0        0    45501 2024-03-03 11:44:30.728159 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/package-lock.json
--rw-r--r--   0        0        0      101 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/package.json
--rw-r--r--   0        0        0     2323 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/print.py
--rw-r--r--   0        0        0     2041 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/screenshot.js
--rw-r--r--   0        0        0     1851 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/utils.py
--rw-r--r--   0        0        0     9453 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/auth.py
--rw-r--r--   0        0        0     4361 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/__init__.py
--rw-r--r--   0        0        0      636 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/interface.py
--rw-r--r--   0        0        0     1083 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/local.py
--rw-r--r--   0        0        0     5085 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/redis.py
--rw-r--r--   0        0        0      272 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/utils.py
--rw-r--r--   0        0        0     3028 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/client_info.py
--rw-r--r--   0        0        0     1524 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/config_utils.py
--rw-r--r--   0        0        0      839 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/coverage_setup.py
--rw-r--r--   0        0        0    16175 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/db.py
--rw-r--r--   0        0        0     3076 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/db_maintenance_view.py
--rw-r--r--   0        0        0     1239 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/__init__.py
--rw-r--r--   0        0        0     4378 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/_listeners.py
--rw-r--r--   0        0        0     7522 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/_views.py
--rw-r--r--   0        0        0     2311 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/utils.py
--rw-r--r--   0        0        0     6725 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/errors.py
--rw-r--r--   0        0        0    19978 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/health_check.py
--rw-r--r--   0        0        0    16707 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/index.py
--rw-r--r--   0        0        0      622 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/loader.py
--rw-r--r--   0        0        0     3357 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/logging_view.py
--rw-r--r--   0        0        0     2680 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/models_graph.py
--rw-r--r--   0        0        0     1698 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/pretty_json.py
--rw-r--r--   0        0        0      739 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/profiler.py
--rw-r--r--   0        0        0     6558 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/prometheus.py
--rw-r--r--   0        0        0        0 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/py.typed
--rw-r--r--   0        0        0     1388 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/pyramid.py
--rw-r--r--   0        0        0     3731 2024-03-03 11:39:25.708383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/pyramid_logging.py
--rw-r--r--   0        0        0     1545 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/redis_stats.py
--rw-r--r--   0        0        0     4615 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/redis_utils.py
--rw-r--r--   0        0        0     4040 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/request_tracking/__init__.py
--rw-r--r--   0        0        0      573 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/request_tracking/_sql.py
--rw-r--r--   0        0        0        0 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/__init__.py
--rwxr-xr-x   0        0        0     1985 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/genversion.py
--rwxr-xr-x   0        0        0    10317 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/stats_db.py
--rwxr-xr-x   0        0        0     2096 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/test_print.py
--rw-r--r--   0        0        0     5031 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sentry.py
--rw-r--r--   0        0        0     1567 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/services.py
--rw-r--r--   0        0        0     3427 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/setup_process.py
--rw-r--r--   0        0        0      877 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sql_profiler/__init__.py
--rw-r--r--   0        0        0     3703 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sql_profiler/_impl.py
--rw-r--r--   0        0        0     1552 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/README.md
--rw-r--r--   0        0        0        0 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/__init__.py
--rw-r--r--   0        0        0      752 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/_filters.py
--rw-r--r--   0        0        0     1471 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/_models.py
--rw-r--r--   0        0        0      460 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/examples/example.py
--rw-r--r--   0        0        0     4801 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/handlers.py
--rw-r--r--   0        0        0      887 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/static/favicon-16x16.png
--rw-r--r--   0        0        0     1216 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/static/favicon-32x32.png
--rw-r--r--   0        0        0      747 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/stats_pyramid/__init__.py
--rw-r--r--   0        0        0     2917 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/stats_pyramid/_db_spy.py
--rw-r--r--   0        0        0     3209 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
--rw-r--r--   0        0        0     1362 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/templates/index.html.mako
--rw-r--r--   0        0        0     2870 2024-03-03 11:39:25.712383 c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/version.py
--rw-r--r--   0        0        0     5849 2024-03-03 11:47:40.343995 c2cwsgiutils-6.1.0.dev97/pyproject.toml
--rw-r--r--   0        0        0    33515 1970-01-01 00:00:00.000000 c2cwsgiutils-6.1.0.dev97/PKG-INFO
+-rw-r--r--   0        0        0     1304 2024-03-03 11:50:47.566347 c2cwsgiutils-6.1.0.dev99/LICENSE
+-rw-r--r--   0        0        0    30298 2024-03-03 11:50:47.566347 c2cwsgiutils-6.1.0.dev99/README.md
+-rw-r--r--   0        0        0     3986 2024-03-03 11:50:47.570347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/__init__.py
+-rw-r--r--   0        0        0     1500 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/__init__.py
+-rw-r--r--   0        0        0     9742 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/connection.py
+-rw-r--r--   0        0        0     8769 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/image.py
+-rw-r--r--   0        0        0    45501 2024-03-03 11:55:39.524985 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/package-lock.json
+-rw-r--r--   0        0        0      101 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/package.json
+-rw-r--r--   0        0        0     2323 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/print.py
+-rw-r--r--   0        0        0     2041 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/screenshot.js
+-rw-r--r--   0        0        0     1851 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/utils.py
+-rw-r--r--   0        0        0     9453 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/auth.py
+-rw-r--r--   0        0        0     4361 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/__init__.py
+-rw-r--r--   0        0        0      636 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/interface.py
+-rw-r--r--   0        0        0     1083 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/local.py
+-rw-r--r--   0        0        0     5085 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/redis.py
+-rw-r--r--   0        0        0      272 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/utils.py
+-rw-r--r--   0        0        0     3028 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/client_info.py
+-rw-r--r--   0        0        0     1524 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/config_utils.py
+-rw-r--r--   0        0        0      839 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/coverage_setup.py
+-rw-r--r--   0        0        0    16175 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/db.py
+-rw-r--r--   0        0        0     3076 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/db_maintenance_view.py
+-rw-r--r--   0        0        0     1239 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/__init__.py
+-rw-r--r--   0        0        0     4378 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/_listeners.py
+-rw-r--r--   0        0        0     7522 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/_views.py
+-rw-r--r--   0        0        0     2311 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/utils.py
+-rw-r--r--   0        0        0     6725 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/errors.py
+-rw-r--r--   0        0        0    19978 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/health_check.py
+-rw-r--r--   0        0        0    16707 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/index.py
+-rw-r--r--   0        0        0      622 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/loader.py
+-rw-r--r--   0        0        0     3357 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/logging_view.py
+-rw-r--r--   0        0        0     2680 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/models_graph.py
+-rw-r--r--   0        0        0     1698 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/pretty_json.py
+-rw-r--r--   0        0        0      739 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/profiler.py
+-rw-r--r--   0        0        0     6558 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/prometheus.py
+-rw-r--r--   0        0        0        0 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/py.typed
+-rw-r--r--   0        0        0     1388 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/pyramid.py
+-rw-r--r--   0        0        0     3731 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/pyramid_logging.py
+-rw-r--r--   0        0        0     1545 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/redis_stats.py
+-rw-r--r--   0        0        0     4615 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/redis_utils.py
+-rw-r--r--   0        0        0     4040 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/request_tracking/__init__.py
+-rw-r--r--   0        0        0      573 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/request_tracking/_sql.py
+-rw-r--r--   0        0        0        0 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/__init__.py
+-rwxr-xr-x   0        0        0     1985 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/genversion.py
+-rwxr-xr-x   0        0        0    10317 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/stats_db.py
+-rwxr-xr-x   0        0        0     2096 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/test_print.py
+-rw-r--r--   0        0        0     5031 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sentry.py
+-rw-r--r--   0        0        0     1567 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/services.py
+-rw-r--r--   0        0        0     3427 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/setup_process.py
+-rw-r--r--   0        0        0      877 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sql_profiler/__init__.py
+-rw-r--r--   0        0        0     3703 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sql_profiler/_impl.py
+-rw-r--r--   0        0        0     1552 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/__init__.py
+-rw-r--r--   0        0        0      752 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/_filters.py
+-rw-r--r--   0        0        0     1471 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/_models.py
+-rw-r--r--   0        0        0      460 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/examples/example.py
+-rw-r--r--   0        0        0     4801 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/handlers.py
+-rw-r--r--   0        0        0      887 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/static/favicon-16x16.png
+-rw-r--r--   0        0        0     1216 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/static/favicon-32x32.png
+-rw-r--r--   0        0        0      747 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/stats_pyramid/__init__.py
+-rw-r--r--   0        0        0     2917 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/stats_pyramid/_db_spy.py
+-rw-r--r--   0        0        0     3209 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
+-rw-r--r--   0        0        0     1362 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/templates/index.html.mako
+-rw-r--r--   0        0        0     2870 2024-03-03 11:50:47.574347 c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/version.py
+-rw-r--r--   0        0        0     5849 2024-03-03 11:58:50.267792 c2cwsgiutils-6.1.0.dev99/pyproject.toml
+-rw-r--r--   0        0        0    33515 1970-01-01 00:00:00.000000 c2cwsgiutils-6.1.0.dev99/PKG-INFO
```

### Comparing `c2cwsgiutils-6.1.0.dev97/LICENSE` & `c2cwsgiutils-6.1.0.dev99/LICENSE`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/README.md` & `c2cwsgiutils-6.1.0.dev99/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/connection.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/connection.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/image.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/image.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/package-lock.json` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99970703125%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'commander': '12.0.0'}}, 'node_modules/commander': "*

 * *               "{'version': '12.0.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/commander/-/commander-12.0.0.tgz', 'integrity': "*

 * *               "'sha512-MwVNWlYjDTtOjX5PiD7o5pK0UrFU/OYgcJfjjK4RaHZETNtjJqrZa9Y9ds88+A+f+d5lv+561eZ+yCKoS3gbAA==', "*

 * *               "'engines': {'node': '>=18'}}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "lockfileVersion": 3,
     "name": "acceptance",
     "packages": {
         "": {
             "dependencies": {
-                "commander": "11.1.0",
+                "commander": "12.0.0",
                 "puppeteer": "22.3.0"
             }
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
                 "@babel/highlight": "^7.23.4",
                 "chalk": "^2.4.2"
@@ -284,19 +284,19 @@
         "node_modules/color-name": {
             "integrity": "sha512-72fSenhMw2HZMTVHeCA9KCmpEIbzWiQsjN+BHcBbS9vr1mtt+vJjPdksIBNUmKAW8TFUDPJK5SUU3QhE9NEXDw==",
             "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.3.tgz",
             "version": "1.1.3"
         },
         "node_modules/commander": {
             "engines": {
-                "node": ">=16"
+                "node": ">=18"
             },
-            "integrity": "sha512-yPVavfyCcRhmorC7rWlkHn15b4wDVgVmBA7kV4QVBsF7kv/9TKJAbAXVTxvTnwP8HHKjRCJDClKbciiYS7p0DQ==",
-            "resolved": "https://registry.npmjs.org/commander/-/commander-11.1.0.tgz",
-            "version": "11.1.0"
+            "integrity": "sha512-MwVNWlYjDTtOjX5PiD7o5pK0UrFU/OYgcJfjjK4RaHZETNtjJqrZa9Y9ds88+A+f+d5lv+561eZ+yCKoS3gbAA==",
+            "resolved": "https://registry.npmjs.org/commander/-/commander-12.0.0.tgz",
+            "version": "12.0.0"
         },
         "node_modules/cosmiconfig": {
             "dependencies": {
                 "env-paths": "^2.2.1",
                 "import-fresh": "^3.3.0",
                 "js-yaml": "^4.1.0",
                 "parse-json": "^5.2.0"
```

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/print.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/screenshot.js` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/screenshot.js`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/acceptance/utils.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/acceptance/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/auth.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/auth.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/interface.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/interface.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/local.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/local.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/broadcast/redis.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/broadcast/redis.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/client_info.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/client_info.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/config_utils.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/coverage_setup.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/coverage_setup.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/db.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/db.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/db_maintenance_view.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/db_maintenance_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/_listeners.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/_listeners.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/_views.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/_views.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/debug/utils.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/debug/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/errors.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/errors.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/health_check.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/health_check.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/index.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/index.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/loader.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/loader.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/logging_view.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/logging_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/models_graph.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/models_graph.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/pretty_json.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/pretty_json.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/profiler.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/profiler.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/prometheus.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/prometheus.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/pyramid.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/pyramid.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/pyramid_logging.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/pyramid_logging.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/redis_stats.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/redis_stats.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/redis_utils.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/request_tracking/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/request_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/request_tracking/_sql.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/request_tracking/_sql.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/genversion.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/genversion.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/stats_db.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/stats_db.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/scripts/test_print.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/scripts/test_print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sentry.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sentry.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/services.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/services.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/setup_process.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/setup_process.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sql_profiler/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sql_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sql_profiler/_impl.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sql_profiler/_impl.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/README.md` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/_filters.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/_filters.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/_models.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/_models.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/sqlalchemylogger/handlers.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/sqlalchemylogger/handlers.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/static/favicon-16x16.png` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/static/favicon-32x32.png` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/stats_pyramid/__init__.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/stats_pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/stats_pyramid/_db_spy.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/stats_pyramid/_db_spy.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/stats_pyramid/_pyramid_spy.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/stats_pyramid/_pyramid_spy.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/templates/index.html.mako` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/templates/index.html.mako`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/c2cwsgiutils/version.py` & `c2cwsgiutils-6.1.0.dev99/c2cwsgiutils/version.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.1.0.dev97/pyproject.toml` & `c2cwsgiutils-6.1.0.dev99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "c2cwsgiutils"
-version = "6.1.0.dev97"
+version = "6.1.0.dev99"
 description = "Common utilities for Camptocamp WSGI applications"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 keywords = ["geo", "gis", "sqlalchemy", "orm", "wsgi"]
 repository = "https://github.com/camptocamp/c2cwsgiutils"
 license = "BSD-2-Clause"
 classifiers = [
```

### Comparing `c2cwsgiutils-6.1.0.dev97/PKG-INFO` & `c2cwsgiutils-6.1.0.dev99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2cwsgiutils
-Version: 6.1.0.dev97
+Version: 6.1.0.dev99
 Summary: Common utilities for Camptocamp WSGI applications
 Home-page: https://github.com/camptocamp/c2cwsgiutils
 License: BSD-2-Clause
 Keywords: geo,gis,sqlalchemy,orm,wsgi
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.9
```

