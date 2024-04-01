# Comparing `tmp/bertagent-1.0.7.tar.gz` & `tmp/bertagent-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bertagent-1.0.7.tar", last modified: Tue Jun 27 09:40:13 2023, max compression
+gzip compressed data, was "bertagent-1.1.0.tar", last modified: Mon Apr  1 21:37:14 2024, max compression
```

## Comparing `bertagent-1.0.7.tar` & `bertagent-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.0.7/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.0.7/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.0.7/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.0.7/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      126 2023-06-16 10:58:03.000000 bertagent-1.0.7/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.0.7/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.0.7/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.0.7/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.0.7/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-1.0.7/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:40:13.157870 bertagent-1.0.7/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1472 2023-06-27 09:02:11.000000 bertagent-1.0.7/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/
--rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.0.7/bertagent/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/_version.py
--rw-------   0 jiko      (1000) jiko      (1000)     9444 2023-06-06 04:18:16.000000 bertagent-1.0.7/bertagent/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/cli/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/cli/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/cli/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/tests/test_bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1547 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/top_level.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.0.7/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-1.0.7/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-1.0.7/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-1.0.7/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-1.0.7/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.7/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.7/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.0.7/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/authors.rst
--rw-------   0 jiko      (1000) jiko      (1000)      394 2023-06-27 09:39:04.000000 bertagent-1.0.7/docs/source/bertagent.rst
--rw-------   0 jiko      (1000) jiko      (1000)      372 2023-06-27 09:39:04.000000 bertagent-1.0.7/docs/source/bertagent.tests.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.0.7/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1001 2023-06-27 08:28:30.000000 bertagent-1.0.7/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.0.7/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       64 2023-06-27 09:39:04.000000 bertagent-1.0.7/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1343 2023-06-27 08:35:15.000000 bertagent-1.0.7/docs/source/tutorial-01-input.csv
--rw-------   0 jiko      (1000) jiko      (1000)     2468 2023-06-27 08:48:33.000000 bertagent-1.0.7/docs/source/tutorial-02-output.csv
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     3142 2023-06-27 09:38:36.000000 bertagent-1.0.7/docs/source/tutorial.rst
--rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.0.7/docs/source/usage.rst
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.0.7/pyproject.toml
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.0.7/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-27 09:40:13.157870 bertagent-1.0.7/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-1.0.7/setup.py
--rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.0.7/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.0.7/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.008741 bertagent-1.1.0/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.1.0/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.1.0/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.1.0/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.1.0/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.1.0/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      126 2023-06-16 10:58:03.000000 bertagent-1.1.0/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.1.0/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.1.0/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.1.0/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.1.0/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3215 2024-02-29 00:27:18.000000 bertagent-1.1.0/Makefile
+-rw-r--r--   0 jiko      (1000) jiko      (1000)     5499 2024-04-01 21:37:14.008741 bertagent-1.1.0/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1472 2023-06-27 09:02:11.000000 bertagent-1.1.0/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/bertagent/
+-rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.1.0/bertagent/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2024-04-01 21:37:14.008741 bertagent-1.1.0/bertagent/_version.py
+-rw-------   0 jiko      (1000) jiko      (1000)    10688 2024-03-21 13:49:06.000000 bertagent-1.1.0/bertagent/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/bertagent/cli/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/cli/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/cli/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/bertagent/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/bertagent/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/bertagent/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/tests/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.1.0/bertagent/tests/test_bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.004741 bertagent-1.1.0/bertagent.egg-info/
+-rw-r--r--   0 jiko      (1000) jiko      (1000)     5499 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1547 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       59 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1137 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       10 2024-04-01 21:37:13.000000 bertagent-1.1.0/bertagent.egg-info/top_level.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.1.0/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.004741 bertagent-1.1.0/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2024-02-29 04:26:48.000000 bertagent-1.1.0/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2024-02-29 04:26:48.000000 bertagent-1.1.0/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.000741 bertagent-1.1.0/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.004741 bertagent-1.1.0/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2024-02-29 04:27:04.000000 bertagent-1.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2024-03-21 13:08:42.000000 bertagent-1.1.0/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2024-03-21 13:08:42.000000 bertagent-1.1.0/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2024-03-21 13:08:42.000000 bertagent-1.1.0/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.1.0/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.004741 bertagent-1.1.0/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2024-04-01 21:37:14.004741 bertagent-1.1.0/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.1.0/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.1.0/docs/source/authors.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      394 2024-03-21 13:39:42.000000 bertagent-1.1.0/docs/source/bertagent.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      372 2024-03-21 13:39:42.000000 bertagent-1.1.0/docs/source/bertagent.tests.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.1.0/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.1.0/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.1.0/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1001 2023-06-27 08:28:30.000000 bertagent-1.1.0/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.1.0/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       64 2024-03-21 13:39:42.000000 bertagent-1.1.0/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.1.0/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1343 2023-06-27 08:35:15.000000 bertagent-1.1.0/docs/source/tutorial-01-input.csv
+-rw-------   0 jiko      (1000) jiko      (1000)     2468 2023-06-27 08:48:33.000000 bertagent-1.1.0/docs/source/tutorial-02-output.csv
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5006 2024-04-01 21:27:48.000000 bertagent-1.1.0/docs/source/tutorial.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.1.0/docs/source/usage.rst
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.1.0/pyproject.toml
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.1.0/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2024-04-01 21:37:14.008741 bertagent-1.1.0/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2747 2024-03-07 19:38:54.000000 bertagent-1.1.0/setup.py
+-rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.1.0/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.1.0/versioneer.py
```

### Comparing `bertagent-1.0.7/.github/workflows/build-main.yml` & `bertagent-1.1.0/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/.gitignore` & `bertagent-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/.readthedocs.yaml` & `bertagent-1.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/CONTRIBUTING.rst` & `bertagent-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/LICENSE` & `bertagent-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/Makefile` & `bertagent-1.1.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -102,10 +102,10 @@
 
 prep: clean lint test docs dist check install-editable
 
 release: dist ## package and upload a release
 	twine upload dist/*
 
 version-check: ## display git versioning tags and the actual current version from versioneer
-	@git tag | grep "bertagent-v" | sed -e "s|bertagent-v||g"
+	@git tag | grep "bertagent-v" | sed -e "s|bertagent-v||g" | sort -V
 	@echo "----------------"
 	@python -c "import bertagent; print(bertagent.__version__+' [← current]')"
```

### Comparing `bertagent-1.0.7/README.rst` & `bertagent-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/bertagent/bertagent.py` & `bertagent-1.1.0/bertagent/bertagent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """BERTAgent main module."""
 
+import re
 import torch
 import logging
 import pathlib
 import pandas as pd
 import numpy as np
 
 from typing import (
@@ -17,75 +18,96 @@
     Optional,
 )
 
 from transformers import AutoModelForSequenceClassification
 from transformers import AutoTokenizer
 
 EXAMPLE_SENTENCES = [
+    "He is a hard working individual",
     "She is a hard working individual",
+    "He is a hardly working individual",
     "She is a hardly working individual",
     "This thing was made of lead",
     "This is a car, it runs on gas",
-    "This is a Karen, she runs for office",
     "This is a Jane, she runs for office",
     "Striving to achieve my goals",
     "Struggling to achieve my goals",
     "Striving to make it",
     "Struggling to make it",
-    "Striving to survive",
     "Struggling to survive",
     "Well planned and well executed",
     "Coordinated activity",
     "Uncoordinated activity",
     "Not coordinated activity",
     "Everything is messy and uncoordinated",
     "A bad decisionmaker",
     "A marvelous decisionmaker",
     "They are submissive",
-    "They submitted to his will",
     "They submitted a paper",
     "They submitted a request",
+    "They requested a submission",
     "We are winners",
     "We are losers",
-    "motivated",
-    "We are motivated",
-    "We are not motivated",
-    "We are unmotivated",
     "Lazy and unmotivated",
     "I want to give up",
     "lost all hope",
     "We'll lose anyway",
+    "motivated",
+    "We are motivated",
+    "We are unmotivated",
+    "We are not motivated",
+    "I'm not motivated.",
+    "I'm in no way motivated.",
+    "I'm way more motivated.",
+    "I'm quite motivated.",
+    "I'm motivated.",
+    "I'm absolutely motivated.",
+    "I'm not lazy.",
+    "I'm not  lazy.",
+    "I'm in no way lazy.",
+    "I'm not at all lazy.",
+    "I'm anything but lazy.",
+    "I'm one of the least lazy people you'll ever meet.",
     "We should give up and say nothing",
     "We must win",
     "We will lead our way out of trouble",
     "We must fight for our rights",
     "We should take control and assert our position",
     "We should take control",
-    "We shoud take controll",
-    "Hard working individual. Hardly working individual",
+    "I sat on the couch and watched funny comedies all day",
+    "I sat on the couch and watched educational documentaries all day",
+    "I hate soup!",
+    "I hate soup.",
+    "I love soup!",
+    "I love soup.",
+    "I make my own decisions.",
+    "I make my own decisions I make my own decisions I make my own decisions",
+    "She was able to decide without any permission from others.",
+    "She was able to decide only after she was given permission to do so.",
 ]
 
 MAX_LENGTH = 128
 TOKENIZER_PARAMS = dict(
     add_special_tokens=True,
     max_length=MAX_LENGTH,
     padding="max_length",
     truncation=True,
     return_attention_mask=True,
 )
 
 
 class BERTAgent:
-    """Evaluates agency in a list of sentences.
+    """
+    Evaluates agency in a list of sentences.
 
     Parameters
     ----------
     model_path : Union[str, pathlib.Path]
         path to huggingface repository or a local directory
-        containing fine-tuned model (e.g., BERTAgent)
+        containing the fine-tuned model (e.g., BERTAgent)
 
     tokenizer_path : Union[str, pathlib.Path]
         path to text tokenizer
 
     tokenizer_params : Dict
         tokenizer parameters dictionary, see examples below
         (``TOKENIZER_PARAMS``)
@@ -176,36 +198,43 @@
     >>> # Check example rows.
     >>> df0[cols0].tail(n=8)
 
     """
 
     def __init__(
         self,
-        model_path: Union[str, pathlib.Path] = None,
+        model_path: Union[str, pathlib.Path, None] = None,
         tokenizer_path: Union[str, pathlib.Path, None] = None,
         tokenizer_params: Dict = TOKENIZER_PARAMS,
         device: Union[str, torch.device] = "cuda",  # TODO checkup
         # device: str = "cuda",
+        revision: Union[str, None] = None,
         factor: float = 1.0,
         bias: float = 0.0,
         log0: logging.Logger = logging.getLogger("dummy"),
     ):
         if model_path is None:
             model_path = "EnchantedStardust/bertagent-best"
 
+        if revision is None:
+            revision = "09044f6c38c4af0d9ddf1d9eea13a98bb932e7f6" # version 1.0.22
+            revision = "5bae55efbd95dd51759d275410cea36c81109227" # version 1.0.24 (added negation training)
+
         if tokenizer_path is None:
             tokenizer_path = model_path
 
         self.model = AutoModelForSequenceClassification.from_pretrained(
             str(model_path),
             num_labels=1,
+            revision=revision,
         )
         self.tokenizer = AutoTokenizer.from_pretrained(
             str(tokenizer_path),
             do_lower_case=True,
+            revision=revision,
         )
         self.tokenizer_params = tokenizer_params
         self.device = device
         self.factor = factor
         self.bias = bias
         self.log0 = log0
 
@@ -216,32 +245,32 @@
         self.log0.debug(f"{self.model.training = }")
         self.log0.debug(f"{self.tokenizer = }")
         self.log0.debug(f"{self.tokenizer_params = }")
 
     def predict(self, sentences: List[str]) -> List[float]:
         """Predict agency for a list of texts.
 
+        .. _BA-ref:
+
         Parameters
         ----------
         sentences : List[str]
             a list of texts (e.g., sentences).
 
         Returns
         -------
         List[float]
             List of scores.
 
-
         .. note::
             See doc for the BERTAgent class for usage examples.
 
-
-
-
         """
+        # Remove repeated whitespace characters.
+        sentences = [re.sub(r"\s\s+", " ", sent).strip() for sent in sentences]
         batch_encodings = self.tokenizer(
             list(sentences),
             None,
             **self.tokenizer_params,
             return_tensors="pt",
         )
         self.model.eval()  # CHECKUP
```

### Comparing `bertagent-1.0.7/bertagent/data/emacs-logo/emacs-128x128.png` & `bertagent-1.1.0/bertagent/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/bertagent/data/emacs-logo/emacs.svg` & `bertagent-1.1.0/bertagent/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/bertagent/tests/test_bertagent.py` & `bertagent-1.1.0/bertagent/tests/test_bertagent.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/bertagent.egg-info/SOURCES.txt` & `bertagent-1.1.0/bertagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/bertagent.egg-info/requires.txt` & `bertagent-1.1.0/bertagent.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 GitPython>=3.1.31
 blessed>=1.20.0
 srsly>=2.4.0
-pandas>=1.4.0
+pandas>=2.0.3
 pytz>=2022.1
 tzlocal>=4.2
 humanfriendly>=10.0
 contexttimer>=0.3.3
+transformers>=4.38.1
+huggingface-hub>=0.21.2
+datasets>=2.17.1
 
 [all]
 GitPython>=3.1.31
 blessed>=1.20.0
 srsly>=2.4.0
-pandas>=1.4.0
+pandas>=2.0.3
 pytz>=2022.1
 tzlocal>=4.2
 humanfriendly>=10.0
 contexttimer>=0.3.3
+transformers>=4.38.1
+huggingface-hub>=0.21.2
+datasets>=2.17.1
 pytest-runner>=5.2
 build>=0.10.0
 black==23.3.0
 codecov==2.1.13
 flake8==6.0.0
 flake8-debugger==4.1.2
 pytest==5.4.3
```

### Comparing `bertagent-1.0.7/docs/Makefile` & `bertagent-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `bertagent-1.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/requirements.txt` & `bertagent-1.1.0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/source/conf.py` & `bertagent-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/source/index.rst` & `bertagent-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/source/installation.rst` & `bertagent-1.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/source/tutorial-01-input.csv` & `bertagent-1.1.0/docs/source/tutorial-01-input.csv`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/docs/source/tutorial-02-output.csv` & `bertagent-1.1.0/docs/source/tutorial-02-output.csv`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/pyproject.toml` & `bertagent-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/requirements_dev.txt` & `bertagent-1.1.0/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/setup.cfg` & `bertagent-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/setup.py` & `bertagent-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,22 @@
     "wheel>=0.34.2",
 ]
 
 requirements = [
     "GitPython>=3.1.31",
     "blessed>=1.20.0",
     "srsly>=2.4.0",
-    "pandas>=1.4.0",
+    "pandas>=2.0.3",
     "pytz>=2022.1",
     "tzlocal>=4.2",
     "humanfriendly>=10.0",
     "contexttimer>=0.3.3",
+    "transformers>=4.38.1",
+    "huggingface-hub>=0.21.2",
+    "datasets>=2.17.1",
 ]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [
```

### Comparing `bertagent-1.0.7/tox.ini` & `bertagent-1.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.7/versioneer.py` & `bertagent-1.1.0/versioneer.py`

 * *Files identical despite different names*

