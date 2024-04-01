# Comparing `tmp/m9s_nereid-7.0.8.tar.gz` & `tmp/m9s_nereid-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid-7.0.8.tar", last modified: Thu Mar 14 08:29:32 2024, max compression
+gzip compressed data, was "m9s_nereid-7.0.9.tar", last modified: Wed Mar 27 09:31:48 2024, max compression
```

## Comparing `m9s_nereid-7.0.8.tar` & `m9s_nereid-7.0.9.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       72 2024-01-22 10:58:44.000000 m9s_nereid-7.0.8/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid-7.0.8/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/.gitignore
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2022-11-26 15:16:29.000000 m9s_nereid-7.0.8/.gitmodules
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      283 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/.travis.yml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.420534 m9s_nereid-7.0.8/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2122 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      832 2024-01-22 10:59:23.000000 m9s_nereid-7.0.8/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1577 2020-03-16 09:24:46.000000 m9s_nereid-7.0.8/LICENSE.BSD
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-16 09:24:46.000000 m9s_nereid-7.0.8/LICENSE.GPL3
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      519 2024-02-02 16:34:56.000000 m9s_nereid-7.0.8/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1599 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/MIGRATION
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      638 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/Makefile
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3700 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1527 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4235 2024-03-13 17:32:50.000000 m9s_nereid-7.0.8/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      298 2024-02-02 17:08:52.000000 m9s_nereid-7.0.8/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.420534 m9s_nereid-7.0.8/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.420534 m9s_nereid-7.0.8/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4235 2024-03-13 17:32:50.000000 m9s_nereid-7.0.8/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.424534 m9s_nereid-7.0.8/docs/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5564 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/Makefile
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.424534 m9s_nereid-7.0.8/docs/_static/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     3593 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/_static/favicon.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    71979 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/_static/logo.png
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.424534 m9s_nereid-7.0.8/docs/_templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      768 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/_templates/sidebarintro.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      667 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/api.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10358 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/docs/conf.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10187 2016-10-03 10:42:45.000000 m9s_nereid-7.0.8/docs/conf.py.bak
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      739 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/contents.rst.inc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2278 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/foreword.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1707 2023-06-01 08:37:00.000000 m9s_nereid-7.0.8/docs/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3688 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/installation.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1789 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/installation_windows.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    33942 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/license.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3173 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/locale.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5096 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/make.bat
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5908 2022-11-26 15:16:47.000000 m9s_nereid-7.0.8/docs/quickstart.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/tryton_module_api.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2652 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/docs/versionmanagement.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.424534 m9s_nereid-7.0.8/m9s_nereid.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3700 2024-03-14 08:29:32.000000 m9s_nereid-7.0.8/m9s_nereid.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2418 2024-03-14 08:29:32.000000 m9s_nereid-7.0.8/m9s_nereid.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-03-14 08:29:32.000000 m9s_nereid-7.0.8/m9s_nereid.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-22 10:03:37.000000 m9s_nereid-7.0.8/m9s_nereid.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      209 2024-03-14 08:29:32.000000 m9s_nereid-7.0.8/m9s_nereid.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2024-03-14 08:29:32.000000 m9s_nereid-7.0.8/m9s_nereid.egg-info/top_level.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.428534 m9s_nereid-7.0.8/nereid/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      935 2024-03-06 07:04:54.000000 m9s_nereid-7.0.8/nereid/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21542 2024-03-06 07:03:42.000000 m9s_nereid-7.0.8/nereid/application.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6146 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/caching.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1135 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/config.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.428534 m9s_nereid-7.0.8/nereid/contrib/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/contrib/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6765 2024-02-05 10:13:04.000000 m9s_nereid-7.0.8/nereid/contrib/locale.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11470 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/contrib/pagination.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11178 2024-01-23 15:47:24.000000 m9s_nereid-7.0.8/nereid/contrib/sitemap.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2157 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/csrf.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1019 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid/ctx.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/exceptions.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1376 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid/globals.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17350 2024-03-14 08:29:26.000000 m9s_nereid-7.0.8/nereid/helpers.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      170 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/logging.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3044 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/routing.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3709 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid/sessions.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      936 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid/signals.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14527 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid/templating.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5620 2024-03-03 11:57:52.000000 m9s_nereid-7.0.8/nereid/testing.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4197 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid/wrappers.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.432534 m9s_nereid-7.0.8/nereid_test_module/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       81 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      680 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1780 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1019 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      346 2024-01-22 10:56:08.000000 m9s_nereid-7.0.8/nereid_test_module/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/dev_requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2002 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/model.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/requirements.txt
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4395 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.432534 m9s_nereid-7.0.8/nereid_test_module/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       73 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/nereid_test_module/templates/registration.jinja
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/nereid_test_module/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       24 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/nereid_test_module/templates/tests/from-module.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2020-03-16 09:24:45.000000 m9s_nereid-7.0.8/nereid_test_module/templates/tests/test-changing-context.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      904 2021-02-12 20:10:26.000000 m9s_nereid-7.0.8/nereid_test_module/templates/tests/translation-test.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      162 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/nereid_test_module/tryton.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      448 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4232 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      934 2024-03-06 07:02:55.000000 m9s_nereid-7.0.8/tests/__init__.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/tests/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       18 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tests/templates/from-local.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        6 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tests/templates/home.jinja
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/tests/templates/localhost/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tests/templates/localhost/site-specific-template.html
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-14 08:29:32.436534 m9s_nereid-7.0.8/tests/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       19 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tests/templates/tests/exists-both.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3637 2024-03-05 16:12:30.000000 m9s_nereid-7.0.8/tests/test_dispatch.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3545 2024-03-03 11:57:52.000000 m9s_nereid-7.0.8/tests/test_helpers.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5267 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tests/test_pagination.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6336 2024-03-03 13:02:26.000000 m9s_nereid-7.0.8/tests/test_signals.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17658 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tests/test_templates.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-02-02 16:35:15.000000 m9s_nereid-7.0.8/tox.ini
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       72 2024-01-22 10:58:44.000000 m9s_nereid-7.0.9/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid-7.0.9/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/.gitignore
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1905 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2022-11-26 15:16:29.000000 m9s_nereid-7.0.9/.gitmodules
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      283 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/.travis.yml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.442234 m9s_nereid-7.0.9/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2122 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      832 2024-01-22 10:59:23.000000 m9s_nereid-7.0.9/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1577 2020-03-16 09:24:46.000000 m9s_nereid-7.0.9/LICENSE.BSD
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-16 09:24:46.000000 m9s_nereid-7.0.9/LICENSE.GPL3
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      519 2024-02-02 16:34:56.000000 m9s_nereid-7.0.9/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1599 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/MIGRATION
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      638 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/Makefile
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3700 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1527 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4235 2024-03-13 17:32:50.000000 m9s_nereid-7.0.9/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      298 2024-02-02 17:08:52.000000 m9s_nereid-7.0.9/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.442234 m9s_nereid-7.0.9/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.442234 m9s_nereid-7.0.9/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4235 2024-03-13 17:32:50.000000 m9s_nereid-7.0.9/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.446234 m9s_nereid-7.0.9/docs/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5564 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/Makefile
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.450234 m9s_nereid-7.0.9/docs/_static/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     3593 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/_static/favicon.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    71979 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/_static/logo.png
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.450234 m9s_nereid-7.0.9/docs/_templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      768 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/_templates/sidebarintro.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      667 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/api.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10358 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/docs/conf.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10187 2016-10-03 10:42:45.000000 m9s_nereid-7.0.9/docs/conf.py.bak
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      739 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/contents.rst.inc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2278 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/foreword.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1707 2023-06-01 08:37:00.000000 m9s_nereid-7.0.9/docs/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3688 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/installation.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1789 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/installation_windows.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    33942 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/license.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3173 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/locale.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5096 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/make.bat
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5908 2022-11-26 15:16:47.000000 m9s_nereid-7.0.9/docs/quickstart.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/tryton_module_api.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2652 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/docs/versionmanagement.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.450234 m9s_nereid-7.0.9/m9s_nereid.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3700 2024-03-27 09:31:48.000000 m9s_nereid-7.0.9/m9s_nereid.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2418 2024-03-27 09:31:48.000000 m9s_nereid-7.0.9/m9s_nereid.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-03-27 09:31:48.000000 m9s_nereid-7.0.9/m9s_nereid.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-22 10:03:37.000000 m9s_nereid-7.0.9/m9s_nereid.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      209 2024-03-27 09:31:48.000000 m9s_nereid-7.0.9/m9s_nereid.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2024-03-27 09:31:48.000000 m9s_nereid-7.0.9/m9s_nereid.egg-info/top_level.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.454234 m9s_nereid-7.0.9/nereid/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      935 2024-03-14 08:29:38.000000 m9s_nereid-7.0.9/nereid/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    21805 2024-03-27 09:31:28.000000 m9s_nereid-7.0.9/nereid/application.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6146 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/caching.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1135 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/config.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.454234 m9s_nereid-7.0.9/nereid/contrib/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/contrib/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6765 2024-02-05 10:13:04.000000 m9s_nereid-7.0.9/nereid/contrib/locale.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11470 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/contrib/pagination.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    11130 2024-03-27 09:31:28.000000 m9s_nereid-7.0.9/nereid/contrib/sitemap.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     2282 2024-03-27 09:31:28.000000 m9s_nereid-7.0.9/nereid/csrf.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1019 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid/ctx.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/exceptions.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1376 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid/globals.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17350 2024-03-14 08:29:26.000000 m9s_nereid-7.0.9/nereid/helpers.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      170 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/logging.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3044 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/routing.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3709 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid/sessions.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      936 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid/signals.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14527 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid/templating.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5620 2024-03-03 11:57:52.000000 m9s_nereid-7.0.9/nereid/testing.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4197 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid/wrappers.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.458234 m9s_nereid-7.0.9/nereid_test_module/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       81 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      680 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1780 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1019 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      346 2024-01-22 10:56:08.000000 m9s_nereid-7.0.9/nereid_test_module/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/dev_requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2002 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/model.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/requirements.txt
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4395 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.458234 m9s_nereid-7.0.9/nereid_test_module/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       73 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/nereid_test_module/templates/registration.jinja
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.458234 m9s_nereid-7.0.9/nereid_test_module/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       24 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/nereid_test_module/templates/tests/from-module.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2020-03-16 09:24:45.000000 m9s_nereid-7.0.9/nereid_test_module/templates/tests/test-changing-context.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      904 2021-02-12 20:10:26.000000 m9s_nereid-7.0.9/nereid_test_module/templates/tests/translation-test.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      162 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/nereid_test_module/tryton.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      448 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4232 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      934 2024-03-06 07:02:55.000000 m9s_nereid-7.0.9/tests/__init__.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/tests/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       18 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tests/templates/from-local.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        6 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tests/templates/home.jinja
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/tests/templates/localhost/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tests/templates/localhost/site-specific-template.html
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-27 09:31:48.462234 m9s_nereid-7.0.9/tests/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       19 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tests/templates/tests/exists-both.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3637 2024-03-05 16:12:30.000000 m9s_nereid-7.0.9/tests/test_dispatch.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3545 2024-03-03 11:57:52.000000 m9s_nereid-7.0.9/tests/test_helpers.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5267 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tests/test_pagination.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6336 2024-03-03 13:02:26.000000 m9s_nereid-7.0.9/tests/test_signals.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17658 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tests/test_templates.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-02-02 16:35:15.000000 m9s_nereid-7.0.9/tox.ini
```

### Comparing `m9s_nereid-7.0.8/.drone.yml` & `m9s_nereid-7.0.9/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/.gitlab-ci.yml` & `m9s_nereid-7.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/.woodpecker/mail_curl.sh` & `m9s_nereid-7.0.9/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/.woodpecker/report.yml` & `m9s_nereid-7.0.9/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/.woodpecker/test.yml` & `m9s_nereid-7.0.9/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/CHANGELOG` & `m9s_nereid-7.0.9/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/COPYRIGHT` & `m9s_nereid-7.0.9/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/INSTALL` & `m9s_nereid-7.0.9/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/LICENSE.BSD` & `m9s_nereid-7.0.9/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/LICENSE.GPL3` & `m9s_nereid-7.0.9/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/MANIFEST.in` & `m9s_nereid-7.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/MIGRATION` & `m9s_nereid-7.0.9/MIGRATION`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/Makefile` & `m9s_nereid-7.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/PKG-INFO` & `m9s_nereid-7.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_nereid
-Version: 7.0.8
+Version: 7.0.9
 Summary: Tryton Nereid Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_nereid-7.0.8/README.md` & `m9s_nereid-7.0.9/README.md`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/README.rst` & `m9s_nereid-7.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/doc/index.rst` & `m9s_nereid-7.0.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/Makefile` & `m9s_nereid-7.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/_static/favicon.png` & `m9s_nereid-7.0.9/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/_static/logo.png` & `m9s_nereid-7.0.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/_templates/sidebarintro.html` & `m9s_nereid-7.0.9/docs/_templates/sidebarintro.html`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/api.rst` & `m9s_nereid-7.0.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/conf.py` & `m9s_nereid-7.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/conf.py.bak` & `m9s_nereid-7.0.9/docs/conf.py.bak`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/contents.rst.inc` & `m9s_nereid-7.0.9/docs/contents.rst.inc`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/foreword.rst` & `m9s_nereid-7.0.9/docs/foreword.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/index.rst` & `m9s_nereid-7.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/installation.rst` & `m9s_nereid-7.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/installation_windows.rst` & `m9s_nereid-7.0.9/docs/installation_windows.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/license.rst` & `m9s_nereid-7.0.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/locale.rst` & `m9s_nereid-7.0.9/docs/locale.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/make.bat` & `m9s_nereid-7.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/quickstart.rst` & `m9s_nereid-7.0.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/docs/versionmanagement.rst` & `m9s_nereid-7.0.9/docs/versionmanagement.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/m9s_nereid.egg-info/PKG-INFO` & `m9s_nereid-7.0.9/m9s_nereid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-nereid
-Version: 7.0.8
+Version: 7.0.9
 Summary: Tryton Nereid Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_nereid-7.0.8/m9s_nereid.egg-info/SOURCES.txt` & `m9s_nereid-7.0.9/m9s_nereid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/__init__.py` & `m9s_nereid-7.0.9/nereid/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from .globals import cache, current_locale, current_user, current_website
 from .helpers import (
     context_processor, flash, get_version, login_required, route,
     template_filter, url_for)
 from .sessions import Session
 from .templating import LazyRenderer, render_email, render_template
 
-__version__ = "7.0.8"
+__version__ = "7.0.9"
```

### Comparing `m9s_nereid-7.0.8/nereid/application.py` & `m9s_nereid-7.0.9/nereid/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,19 @@
         #: exception since it is required
         assert self.secret_key, 'Secret Key is not defined in config'
 
         #: Load the cache
         self.load_cache()
 
         #: Initialise the CSRF handling
+
+        #: CSRF tokens expire with the session and no more after the default
+        #: timeout of flask_wtf (3600)
+        #:
+        #: .. versionchanged:: 7.0.9
         self.csrf_protection = NereidCsrfProtect()
         self.csrf_protection.init_app(self)
 
         self.view_functions['static'] = self.send_static_file
 
         # Backend initialisation
         self.load_backend()
@@ -460,17 +465,19 @@
                     # Raise BadRequest on Tryton exceptions
                     # and all sort of SMTP Errors (that could
                     # be caused by sendmail_transactional on
                     # txn.commmit()
                     if isinstance(e, (
                                 UserError,
                                 UserWarning,
-                                ConcurrencyException,
-                                SMTPException)):
+                                ConcurrencyException)):
                         raise BadRequest(e.message)
+                    elif isinstance(e, (
+                                SMTPException)):
+                        raise BadRequest(e.smtp_error)
                     raise
                 else:
                     while txn.tasks:
                         task_id = txn.tasks.pop()
                         run_task(nereid.pool, task_id)
                     return rv
                 finally:
```

### Comparing `m9s_nereid-7.0.8/nereid/caching.py` & `m9s_nereid-7.0.9/nereid/caching.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/config.py` & `m9s_nereid-7.0.9/nereid/config.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/contrib/locale.py` & `m9s_nereid-7.0.9/nereid/contrib/locale.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/contrib/pagination.py` & `m9s_nereid-7.0.9/nereid/contrib/pagination.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/contrib/sitemap.py` & `m9s_nereid-7.0.9/nereid/contrib/sitemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,30 @@
             return url_for('product.product.render',
                 uri=self.uri, **kwargs)
     """
     #: Batch Size: The number of URLs per sitemap page
     batch_size = 1000
 
     def __init__(self, model, domain, priorities=[0.5],
-            cache_timeout=60 * 60 * 24):
+            max_age=60 * 60 * 24):
         """
         A collection of SitemapSection objects which are automatically
         generated based on the
 
         :param collection: An iterable of tuples with the name of the model
                            and the domain. Example
 
         ...>>> product_obj = pool.get('product.product')
         ...>>> sitemap = Sitemap(
         ...        product_obj, [('displayed_on_eshop', '=', True)])
         """
         self.model = model
         self.domain = domain
         self.priorities = priorities
-        self.cache_timeout = cache_timeout
+        self.max_age = max_age
 
     def render(self):
         with io.BytesIO() as tmp_file:
             data = '<?xml version="1.0" encoding="UTF-8"?>\n'
             data += '<sitemapindex '
             data += 'xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">\n'
             method = '%s.sitemap' % self.model.__name__
@@ -79,15 +79,15 @@
             tmp_file.write(data.encode())
             mimetype = 'application/xml'
             # Workaround to avoid closed file error
             # https://stackoverflow.com/questions/58197454/using-bytesio-and-flask-send-file
             # Remove with flask 2.0
             tmp_file.seek(0)
             return send_file(io.BytesIO(tmp_file.read()),
-                cache_timeout=self.cache_timeout,
+                max_age=self.max_age,
                 mimetype=mimetype)
 
     @cached_property
     def count(self):
         """
         Returns the number of items of the object
         """
@@ -156,15 +156,15 @@
     :param domain: The domain expression which should be searched against in
                    the model
     :param page: The page of the sitemap.
     """
 
     #: The timeout in seconds for the headers, which would be respceted by
     #: intermediate cache servers.
-    cache_timeout = 60 * 60 * 24
+    max_age = 60 * 60 * 24
 
     #: Indicates how frequently the page is likely to change. This value
     #: provides general information to search engines and may not correlate
     #: exactly to how often they crawl the page. Valid values are:
     #:
     #:     always
     #:     hourly
@@ -249,15 +249,15 @@
             tmp_file.write(data.encode())
             mimetype = 'application/xml'
             # Workaround to avoid closed file error
             # https://stackoverflow.com/questions/58197454/using-bytesio-and-flask-send-file
             # Remove with flask 2.0
             tmp_file.seek(0)
             return send_file(io.BytesIO(tmp_file.read()),
-                cache_timeout=self.cache_timeout,
+                max_age=self.max_age,
                 mimetype=mimetype)
 
     def get_url_xml(self, item):
         """
         Returns the etree node for the specific item
         """
         return E(
```

### Comparing `m9s_nereid-7.0.8/nereid/csrf.py` & `m9s_nereid-7.0.9/nereid/csrf.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,17 @@
         app.config['WTF_CSRF_METHODS'] = set(app.config.get(
             'WTF_CSRF_METHODS', ['POST', 'PUT', 'PATCH', 'DELETE']
         ))
         app.config.setdefault('WTF_CSRF_FIELD_NAME', 'csrf_token')
         app.config.setdefault(
             'WTF_CSRF_HEADERS', ['X-CSRFToken', 'X-CSRF-Token']
         )
-        app.config.setdefault('WTF_CSRF_TIME_LIMIT', 3600)
+        # expire with the session instead of the default timeout
+        # https://flask-wtf.readthedocs.io/en/1.2.x/config/
+        app.config.setdefault('WTF_CSRF_TIME_LIMIT', None)
         app.config.setdefault('WTF_CSRF_SSL_STRICT', True)
 
         # expose csrf_token as a helper in all templates
         @app.context_processor
         def csrf_token():
             return dict(csrf_token=generate_csrf)
```

### Comparing `m9s_nereid-7.0.8/nereid/ctx.py` & `m9s_nereid-7.0.9/nereid/ctx.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/globals.py` & `m9s_nereid-7.0.9/nereid/globals.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/helpers.py` & `m9s_nereid-7.0.9/nereid/helpers.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/routing.py` & `m9s_nereid-7.0.9/nereid/routing.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/sessions.py` & `m9s_nereid-7.0.9/nereid/sessions.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/signals.py` & `m9s_nereid-7.0.9/nereid/signals.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/templating.py` & `m9s_nereid-7.0.9/nereid/templating.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/testing.py` & `m9s_nereid-7.0.9/nereid/testing.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid/wrappers.py` & `m9s_nereid-7.0.9/nereid/wrappers.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/.gitlab-ci.yml` & `m9s_nereid-7.0.9/nereid_test_module/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/COPYRIGHT` & `m9s_nereid-7.0.9/nereid_test_module/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/INSTALL` & `m9s_nereid-7.0.9/nereid_test_module/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/LICENSE` & `m9s_nereid-7.0.9/nereid_test_module/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/README.md` & `m9s_nereid-7.0.9/nereid_test_module/README.md`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/README.rst` & `m9s_nereid-7.0.9/nereid_test_module/README.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/model.py` & `m9s_nereid-7.0.9/nereid_test_module/model.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/setup.py` & `m9s_nereid-7.0.9/nereid_test_module/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/templates/tests/translation-test.html` & `m9s_nereid-7.0.9/nereid_test_module/templates/tests/translation-test.html`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/nereid_test_module/tox.ini` & `m9s_nereid-7.0.9/nereid_test_module/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/setup.py` & `m9s_nereid-7.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tests/__init__.py` & `m9s_nereid-7.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tests/test_dispatch.py` & `m9s_nereid-7.0.9/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tests/test_helpers.py` & `m9s_nereid-7.0.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tests/test_pagination.py` & `m9s_nereid-7.0.9/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tests/test_signals.py` & `m9s_nereid-7.0.9/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tests/test_templates.py` & `m9s_nereid-7.0.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-7.0.8/tox.ini` & `m9s_nereid-7.0.9/tox.ini`

 * *Files identical despite different names*

