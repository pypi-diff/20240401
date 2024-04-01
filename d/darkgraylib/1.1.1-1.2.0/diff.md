# Comparing `tmp/darkgraylib-1.1.1.tar.gz` & `tmp/darkgraylib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darkgraylib-1.1.1.tar", last modified: Wed Mar 27 20:10:46 2024, max compression
+gzip compressed data, was "darkgraylib-1.2.0.tar", last modified: Mon Apr  1 18:31:28 2024, max compression
```

## Comparing `darkgraylib-1.1.1.tar` & `darkgraylib-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 20:10:46.210225 darkgraylib-1.1.1/
--rw-r--r--   0 akaihola  (1000) users      (100)     1554 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/LICENSE
--rw-r--r--   0 akaihola  (1000) users      (100)     5023 2024-03-27 20:10:46.210225 darkgraylib-1.1.1/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)    42690 2024-03-27 20:10:32.000000 darkgraylib-1.1.1/README.rst
--rw-r--r--   0 akaihola  (1000) users      (100)     1241 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/pyproject.toml
--rw-r--r--   0 akaihola  (1000) users      (100)     2331 2024-03-27 20:10:46.211225 darkgraylib-1.1.1/setup.cfg
--rw-r--r--   0 akaihola  (1000) users      (100)     1797 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/setup.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 20:10:46.206225 darkgraylib-1.1.1/src/
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 20:10:46.207225 darkgraylib-1.1.1/src/darkgraylib/
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7930 2024-03-27 20:05:20.000000 darkgraylib-1.1.1/src/darkgraylib/argparse_helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7144 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/command_line.py
--rw-r--r--   0 akaihola  (1000) users      (100)     8455 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/config.py
--rw-r--r--   0 akaihola  (1000) users      (100)     4431 2024-03-26 20:25:08.000000 darkgraylib-1.1.1/src/darkgraylib/diff.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1734 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/files.py
--rw-r--r--   0 akaihola  (1000) users      (100)    13484 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/git.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1573 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/help.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 20:10:46.208226 darkgraylib-1.1.1/src/darkgraylib/highlighting/
--rw-r--r--   0 akaihola  (1000) users      (100)     1869 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/highlighting/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3105 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/highlighting/lexers.py
--rw-r--r--   0 akaihola  (1000) users      (100)      367 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/log.py
--rw-r--r--   0 akaihola  (1000) users      (100)     1000 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/main.py
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/py.typed
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 20:10:46.208226 darkgraylib-1.1.1/src/darkgraylib/testtools/
--rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/__init__.py
--rw-r--r--   0 akaihola  (1000) users      (100)      642 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/clear_black_cache_plugin.py
--rw-r--r--   0 akaihola  (1000) users      (100)     2103 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/diff_helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7113 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/git_repo_plugin.py
--rw-r--r--   0 akaihola  (1000) users      (100)     3502 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)      213 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/highlighting_helpers.py
--rw-r--r--   0 akaihola  (1000) users      (100)      629 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/testtools/mock_argument_parser.py
--rw-r--r--   0 akaihola  (1000) users      (100)     7211 2024-03-16 12:59:04.000000 darkgraylib-1.1.1/src/darkgraylib/utils.py
--rw-r--r--   0 akaihola  (1000) users      (100)       90 2024-03-27 20:10:32.000000 darkgraylib-1.1.1/src/darkgraylib/version.py
-drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-03-27 20:10:46.208226 darkgraylib-1.1.1/src/darkgraylib.egg-info/
--rw-r--r--   0 akaihola  (1000) users      (100)     5023 2024-03-27 20:10:46.000000 darkgraylib-1.1.1/src/darkgraylib.egg-info/PKG-INFO
--rw-r--r--   0 akaihola  (1000) users      (100)     1026 2024-03-27 20:10:46.000000 darkgraylib-1.1.1/src/darkgraylib.egg-info/SOURCES.txt
--rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-03-27 20:10:46.000000 darkgraylib-1.1.1/src/darkgraylib.egg-info/dependency_links.txt
--rw-r--r--   0 akaihola  (1000) users      (100)      290 2024-03-27 20:10:46.000000 darkgraylib-1.1.1/src/darkgraylib.egg-info/entry_points.txt
--rw-r--r--   0 akaihola  (1000) users      (100)      441 2024-03-27 20:10:46.000000 darkgraylib-1.1.1/src/darkgraylib.egg-info/requires.txt
--rw-r--r--   0 akaihola  (1000) users      (100)       12 2024-03-27 20:10:46.000000 darkgraylib-1.1.1/src/darkgraylib.egg-info/top_level.txt
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.963186 darkgraylib-1.2.0/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1554 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/LICENSE
+-rw-r--r--   0 akaihola  (1000) users      (100)     4765 2024-04-01 18:31:28.963186 darkgraylib-1.2.0/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)    42637 2024-04-01 18:31:04.000000 darkgraylib-1.2.0/README.rst
+-rw-r--r--   0 akaihola  (1000) users      (100)     1241 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/pyproject.toml
+-rw-r--r--   0 akaihola  (1000) users      (100)     2262 2024-04-01 18:31:28.964186 darkgraylib-1.2.0/setup.cfg
+-rw-r--r--   0 akaihola  (1000) users      (100)     1797 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/setup.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.959186 darkgraylib-1.2.0/src/
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.960186 darkgraylib-1.2.0/src/darkgraylib/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7930 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/src/darkgraylib/argparse_helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7554 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/src/darkgraylib/command_line.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     8455 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/config.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     4431 2024-03-31 19:38:11.000000 darkgraylib-1.2.0/src/darkgraylib/diff.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1734 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/files.py
+-rw-r--r--   0 akaihola  (1000) users      (100)    13505 2024-04-01 18:27:39.000000 darkgraylib-1.2.0/src/darkgraylib/git.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1573 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/help.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.961186 darkgraylib-1.2.0/src/darkgraylib/highlighting/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1869 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/highlighting/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3105 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/highlighting/lexers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      367 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/log.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     1000 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/main.py
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/py.typed
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.961186 darkgraylib-1.2.0/src/darkgraylib/testtools/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      642 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/clear_black_cache_plugin.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2103 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/diff_helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7113 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/git_repo_plugin.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     3502 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      213 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/highlighting_helpers.py
+-rw-r--r--   0 akaihola  (1000) users      (100)      629 2024-03-16 12:59:04.000000 darkgraylib-1.2.0/src/darkgraylib/testtools/mock_argument_parser.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     7254 2024-04-01 18:27:39.000000 darkgraylib-1.2.0/src/darkgraylib/utils.py
+-rw-r--r--   0 akaihola  (1000) users      (100)       90 2024-04-01 18:31:04.000000 darkgraylib-1.2.0/src/darkgraylib/version.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-01 18:31:28.961186 darkgraylib-1.2.0/src/darkgraylib.egg-info/
+-rw-r--r--   0 akaihola  (1000) users      (100)     4765 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)     1026 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/SOURCES.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/dependency_links.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      290 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/entry_points.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      376 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/requires.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)       12 2024-04-01 18:31:28.000000 darkgraylib-1.2.0/src/darkgraylib.egg-info/top_level.txt
```

### Comparing `darkgraylib-1.1.1/LICENSE` & `darkgraylib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/PKG-INFO` & `darkgraylib-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkgraylib
-Version: 1.1.1
+Version: 1.2.0
 Summary: Common supporting code for Darker and Graylint
 Home-page: https://github.com/akaihola/darkgraylib
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darkgraylib
 Project-URL: Change Log, https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
@@ -38,47 +38,43 @@
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: airium>=0.2.3; extra == "release"
-Requires-Dist: click>=8.0.0; extra == "release"
-Requires-Dist: darkgray-dev-tools~=0.0.1; extra == "release"
-Requires-Dist: defusedxml>=0.7.1; extra == "release"
-Requires-Dist: requests_cache>=0.7; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
 
 =============
  darkgraylib
 =============
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml/badge.svg
    :alt: main branch build status
-.. _build-badge: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml?query=branch%3Amain
+   :target: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml?query=branch%3Amain
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/darkgraylib/blob/main/LICENSE
+   :target: https://github.com/akaihola/darkgraylib/blob/main/LICENSE
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/darkgraylib
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/darkgraylib/
+   :target: https://pypi.org/project/darkgraylib/
 .. |downloads-badge| image:: https://pepy.tech/badge/darkgraylib
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/darkgraylib
+   :target: https://pepy.tech/project/darkgraylib
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/4?color=red&label=release%201.2.0
+   :target: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/6?color=red&label=release%201.2.1
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darkgraylib/milestone/4
+   :target: https://github.com/akaihola/darkgraylib/milestone/4
 
 
 What?
 =====
 
 This package is a placeholder for common supporting code for Darker_ and Graylint_.
```

### Comparing `darkgraylib-1.1.1/README.rst` & `darkgraylib-1.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 =============
  darkgraylib
 =============
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml/badge.svg
    :alt: main branch build status
-.. _build-badge: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml?query=branch%3Amain
+   :target: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml?query=branch%3Amain
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/darkgraylib/blob/main/LICENSE
+   :target: https://github.com/akaihola/darkgraylib/blob/main/LICENSE
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/darkgraylib
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/darkgraylib/
+   :target: https://pypi.org/project/darkgraylib/
 .. |downloads-badge| image:: https://pepy.tech/badge/darkgraylib
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/darkgraylib
+   :target: https://pepy.tech/project/darkgraylib
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/4?color=red&label=release%201.2.0
+   :target: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/6?color=red&label=release%201.2.1
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darkgraylib/milestone/4
+   :target: https://github.com/akaihola/darkgraylib/milestone/4
 
 
 What?
 =====
 
 This package is a placeholder for common supporting code for Darker_ and Graylint_.
 
@@ -37,15 +37,15 @@
 .. _Darker: https://pypi.org/project/darker
 .. _Graylint: https://pypi.org/project/graylint
 
 +------------------------------------------------+--------------------------------+
 | |you-can-help|                                 | |support|                      |
 +================================================+================================+
 | We're asking the community kindly for help to  | We have a                      |
-| review pull requests for |next-milestone|_ .   | `community support channel`_   |
+| review pull requests for |next-milestone|.     | `community support channel`_   |
 | If you have a moment to spare, please take a   | on GitHub Discussions. Welcome |
 | look at one of them and shoot us a comment!    | to ask for help and advice!    |
 +------------------------------------------------+--------------------------------+
 
 .. |you-can-help| image:: https://img.shields.io/badge/-You%20can%20help-green?style=for-the-badge
    :alt: You can help
 .. |support| image:: https://img.shields.io/badge/-Support-green?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,39 +1,38 @@
-============= darkgraylib ============= |build-badge|_ |license-badge|_ |pypi-
-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_ .. |build-badge|
+============= darkgraylib ============= |build-badge| |license-badge| |pypi-
+badge| |downloads-badge| |black-badge| |changelog-badge| .. |build-badge|
 image:: https://github.com/akaihola/darkgraylib/actions/workflows/python-
-package.yml/badge.svg :alt: main branch build status .. _build-badge: https://
+package.yml/badge.svg :alt: main branch build status :target: https://
 github.com/akaihola/darkgraylib/actions/workflows/python-
 package.yml?query=branch%3Amain .. |license-badge| image:: https://
 img.shields.io/badge/License-BSD%203--Clause-blue.svg :alt: BSD 3 Clause
-license .. _license-badge: https://github.com/akaihola/darkgraylib/blob/main/
-LICENSE .. |pypi-badge| image:: https://img.shields.io/pypi/v/darkgraylib :alt:
-Latest release on PyPI .. _pypi-badge: https://pypi.org/project/darkgraylib/ ..
-|downloads-badge| image:: https://pepy.tech/badge/darkgraylib :alt: Number of
-downloads .. _downloads-badge: https://pepy.tech/project/darkgraylib .. |black-
-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg :alt:
-Source code formatted using Black .. _black-badge: https://github.com/psf/black
-.. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
-:alt: Change log .. _changelog-badge: https://github.com/akaihola/darkgraylib/
-blob/main/CHANGES.rst .. |next-milestone| image:: https://img.shields.io/
-github/milestones/progress/akaihola/darkgraylib/
-4?color=red&label=release%201.2.0 :alt: Next milestone .. _next-milestone:
+license :target: https://github.com/akaihola/darkgraylib/blob/main/LICENSE ..
+|pypi-badge| image:: https://img.shields.io/pypi/v/darkgraylib :alt: Latest
+release on PyPI :target: https://pypi.org/project/darkgraylib/ .. |downloads-
+badge| image:: https://pepy.tech/badge/darkgraylib :alt: Number of downloads :
+target: https://pepy.tech/project/darkgraylib .. |black-badge| image:: https://
+img.shields.io/badge/code%20style-black-000000.svg :alt: Source code formatted
+using Black :target: https://github.com/psf/black .. |changelog-badge| image::
+https://img.shields.io/badge/-change%20log-purple :alt: Change log :target:
+https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst .. |next-
+milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/
+darkgraylib/6?color=red&label=release%201.2.1 :alt: Next milestone :target:
 https://github.com/akaihola/darkgraylib/milestone/4 What? ===== This package is
 a placeholder for common supporting code for Darker_ and Graylint_. Such pieces
 of code have been moved from Darker_ to this new package. .. _Darker: https://
 pypi.org/project/darker .. _Graylint: https://pypi.org/project/graylint +------
 ------------------------------------------+--------------------------------+ |
 |you-can-help| | |support| |
 +================================================+================================+
 | We're asking the community kindly for help to | We have a | | review pull
-requests for |next-milestone|_ . | `community support channel`_ | | If you have
-a moment to spare, please take a | on GitHub Discussions. Welcome | | look at
-one of them and shoot us a comment! | to ask for help and advice! | +----------
---------------------------------------+--------------------------------+ ..
-|you-can-help| image:: https://img.shields.io/badge/-You%20can%20help-
+requests for |next-milestone|. | `community support channel`_ | | If you have a
+moment to spare, please take a | on GitHub Discussions. Welcome | | look at one
+of them and shoot us a comment! | to ask for help and advice! | +--------------
+----------------------------------+--------------------------------+ .. |you-
+can-help| image:: https://img.shields.io/badge/-You%20can%20help-
 green?style=for-the-badge :alt: You can help .. |support| image:: https://
 img.shields.io/badge/-Support-green?style=for-the-badge :alt: Support .. _#151:
 https://github.com/akaihola/darker/issues/151 .. _community support channel:
 https://github.com/akaihola/darker/discussions Why? ==== Darker_ and Graylint_
 originate from the same original Darker_ code base. In February 2023, linter
 support was decided to be moved out from Darker_. Obviously, the two tools are
 still very similar and share a lot of under-the-hood functionality. For
```

### Comparing `darkgraylib-1.1.1/pyproject.toml` & `darkgraylib-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/setup.cfg` & `darkgraylib-1.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -65,19 +65,15 @@
 	ruff>=0.0.292
 	twine>=2.0.0
 	types-requests>=2.27.9
 	types-toml>=0.10.4
 	urllib3>=1.25.9  # through requests-cache and twine, fixes CVE-2020-26137
 	wheel>=0.21.0
 release = 
-	airium>=0.2.3
-	click>=8.0.0
-	darkgray-dev-tools~=0.0.1
-	defusedxml>=0.7.1
-	requests_cache>=0.7
+	darkgray-dev-tools~=0.0.2
 
 [flake8]
 max-line-length = 88
 ignore = 
 	C408
 	D400
 	D415
```

### Comparing `darkgraylib-1.1.1/setup.py` & `darkgraylib-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/argparse_helpers.py` & `darkgraylib-1.2.0/src/darkgraylib/argparse_helpers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/command_line.py` & `darkgraylib-1.2.0/src/darkgraylib/command_line.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Command line parsing for the ``darker`` and ``graylint`` binaries."""
 
+from __future__ import annotations
+
 import sys
 from argparse import SUPPRESS, ArgumentParser, Namespace
 from functools import partial
-from typing import Any, List, Optional, Tuple, Type, TypeVar, Protocol
+from typing import Any, Callable, Protocol, TypeVar
 
 from darkgraylib import help as hlp
 from darkgraylib.argparse_helpers import (
     LogLevelAction,
     NewlinePreservingFormatter,
-    OptionsForReadmeAction, UpdateReadmeAction, VerifyReadmeAction,
+    OptionsForReadmeAction,
+    UpdateReadmeAction,
+    VerifyReadmeAction,
 )
 from darkgraylib.config import (
     BaseConfig,
     get_effective_config,
     get_modified_config,
     load_config,
     override_color_with_environment,
@@ -79,15 +83,18 @@
     add_arg(SUPPRESS, "--options-for-readme", action=OptionsForReadmeAction)
     add_arg(SUPPRESS, "--verify-readme", action=VerifyReadmeAction)
     add_arg(SUPPRESS, "--update-readme", action=UpdateReadmeAction)
     return parser
 
 
 def add_parser_argument(
-    parser: ArgumentParser, help_text: Optional[str], *name_or_flags: str, **kwargs: Any
+    parser: ArgumentParser,
+    help_text: str | None,
+    *name_or_flags: str,
+    **kwargs: Any,  # noqa: ANN401
 ) -> None:
     """Add an argument to the parser
 
     :parser: The parser to add the argument to
     :help_text: The help text for the argument
     :name_or_flags: The name of the positional argument or the alternative flags for the
                     option
@@ -106,18 +113,19 @@
 
     def __call__(self, require_src: bool) -> ArgumentParser:
         ...
 
 
 def parse_command_line(
     argument_parser_factory: ArgumentParserFactory,
-    argv: Optional[List[str]],
+    argv: list[str] | None,
     section_name: str,
-    config_type: Type[T],
-) -> Tuple[Namespace, T, T]:
+    config_type: type[T],
+    load_config_hook: Callable[[T], None] | None = None,
+) -> tuple[Namespace, T, T]:
     """Return the parsed command line, using defaults from a configuration file
 
     Also return the effective configuration which combines defaults, the configuration
     read from ``pyproject.toml`` (or the path given in ``--config``), environment
     variables, and command line arguments.
 
     Finally, also return the set of configuration options which differ from defaults.
@@ -125,14 +133,17 @@
     :param argument_parser_factory: A function that creates an argument parser object.
     :param argv: Command line arguments to parse (excluding the path of the script). If
                  ``None``, use ``sys.argv``.
     :param section_name: The name of the section in the configuration file to read
     :param config_type: The type of the configuration object to be returned. For Darker,
                         this should be ``DarkerConfig``, for Graylint
                         ``GraylintConfig``.
+    :param load_config_hook: A hook to call after loading the configuration file. This
+                             is used to warn about configuration options which are
+                             deprecated in the configuration file.
     :return: A tuple of the parsed command line, the effective configuration, and the
              set of modified configuration options from the defaults.
 
     """
     if argv is None:
         argv = sys.argv[1:]
 
@@ -142,14 +153,16 @@
     args = parser_for_srcs.parse_args(argv)
 
     # 2. Locate `pyproject.toml` based on the `-c`/`--config` command line option, or
     #    if it's not provided, based on the paths to process, or in the current
     #    directory if no paths were given. Load Darker or Graylint configuration from
     #    it.
     pyproject_config = load_config(args.config, args.src, section_name, config_type)
+    if load_config_hook:
+        load_config_hook(pyproject_config)
 
     # 3. The PY_COLORS, NO_COLOR and FORCE_COLOR environment variables override the
     #    `--color` command line option.
     config = override_color_with_environment(pyproject_config)
 
     # 4. Re-run the parser with configuration defaults. This way we get combined values
     #    based on the configuration file and the command line options for all options
```

### Comparing `darkgraylib-1.1.1/src/darkgraylib/config.py` & `darkgraylib-1.2.0/src/darkgraylib/config.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/diff.py` & `darkgraylib-1.2.0/src/darkgraylib/diff.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/files.py` & `darkgraylib-1.2.0/src/darkgraylib/files.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/git.py` & `darkgraylib-1.2.0/src/darkgraylib/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 import re
 import shlex
 import sys
 from contextlib import contextmanager
 from dataclasses import dataclass
-from datetime import datetime
+from datetime import datetime, timezone
 from functools import lru_cache
 from pathlib import Path
 from subprocess import PIPE, CalledProcessError, check_output  # nosec
 from typing import Dict, Iterator, List, Match, Optional, Tuple, Union, cast, overload
 
 from darkgraylib.utils import GIT_DATEFORMAT, TextDocument
 
@@ -74,15 +74,15 @@
     :param path: The relative path of the file in the Git repository
     :param revision: The Git revision for which to get the file modification time
     :param cwd: The root of the Git repository
 
     """
     cmd = ["log", "-1", "--format=%ct", revision, "--", path.as_posix()]
     lines = git_check_output_lines(cmd, cwd)
-    return datetime.utcfromtimestamp(int(lines[0])).strftime(GIT_DATEFORMAT)
+    return datetime.fromtimestamp(int(lines[0]), timezone.utc).strftime(GIT_DATEFORMAT)
 
 
 def git_get_content_at_revision(path: Path, revision: str, cwd: Path) -> TextDocument:
     """Get unmodified text lines of a file at a Git revision
 
     :param path: The relative path of the file in the Git repository
     :param revision: The Git revision for which to get the file content, or ``WORKTREE``
```

### Comparing `darkgraylib-1.1.1/src/darkgraylib/help.py` & `darkgraylib-1.2.0/src/darkgraylib/help.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/highlighting/__init__.py` & `darkgraylib-1.2.0/src/darkgraylib/highlighting/__init__.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/highlighting/lexers.py` & `darkgraylib-1.2.0/src/darkgraylib/highlighting/lexers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/main.py` & `darkgraylib-1.2.0/src/darkgraylib/main.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/testtools/clear_black_cache_plugin.py` & `darkgraylib-1.2.0/src/darkgraylib/testtools/clear_black_cache_plugin.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/testtools/diff_helpers.py` & `darkgraylib-1.2.0/src/darkgraylib/testtools/diff_helpers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/testtools/git_repo_plugin.py` & `darkgraylib-1.2.0/src/darkgraylib/testtools/git_repo_plugin.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/testtools/helpers.py` & `darkgraylib-1.2.0/src/darkgraylib/testtools/helpers.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/testtools/mock_argument_parser.py` & `darkgraylib-1.2.0/src/darkgraylib/testtools/mock_argument_parser.py`

 * *Files identical despite different names*

### Comparing `darkgraylib-1.1.1/src/darkgraylib/utils.py` & `darkgraylib-1.2.0/src/darkgraylib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Miscellaneous utility functions"""
 
 import io
 import sys
 import tokenize
-from datetime import datetime
+from datetime import datetime, timezone
 from itertools import chain
 from pathlib import Path
 from typing import Iterable, Tuple
 
 TextLines = Tuple[str, ...]
 
 WINDOWS = sys.platform.startswith("win")
@@ -121,15 +121,17 @@
     @classmethod
     def from_file(cls, path: Path) -> "TextDocument":
         """Create a document object by reading a text file
 
         Also store the last modification time of the file.
 
         """
-        mtime = datetime.utcfromtimestamp(path.stat().st_mtime).strftime(GIT_DATEFORMAT)
+        mtime = datetime.fromtimestamp(path.stat().st_mtime, timezone.utc).strftime(
+            GIT_DATEFORMAT
+        )
         with path.open("rb") as srcbuf:
             return cls.from_bytes(srcbuf.read(), mtime)
 
     @classmethod
     def from_lines(
         cls,
         lines: Iterable[str],
```

### Comparing `darkgraylib-1.1.1/src/darkgraylib.egg-info/PKG-INFO` & `darkgraylib-1.2.0/src/darkgraylib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkgraylib
-Version: 1.1.1
+Version: 1.2.0
 Summary: Common supporting code for Darker and Graylint
 Home-page: https://github.com/akaihola/darkgraylib
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darkgraylib
 Project-URL: Change Log, https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
@@ -38,47 +38,43 @@
 Requires-Dist: ruff>=0.0.292; extra == "test"
 Requires-Dist: twine>=2.0.0; extra == "test"
 Requires-Dist: types-requests>=2.27.9; extra == "test"
 Requires-Dist: types-toml>=0.10.4; extra == "test"
 Requires-Dist: urllib3>=1.25.9; extra == "test"
 Requires-Dist: wheel>=0.21.0; extra == "test"
 Provides-Extra: release
-Requires-Dist: airium>=0.2.3; extra == "release"
-Requires-Dist: click>=8.0.0; extra == "release"
-Requires-Dist: darkgray-dev-tools~=0.0.1; extra == "release"
-Requires-Dist: defusedxml>=0.7.1; extra == "release"
-Requires-Dist: requests_cache>=0.7; extra == "release"
+Requires-Dist: darkgray-dev-tools~=0.0.2; extra == "release"
 
 =============
  darkgraylib
 =============
 
-|build-badge|_ |license-badge|_ |pypi-badge|_ |downloads-badge|_ |black-badge|_ |changelog-badge|_
+|build-badge| |license-badge| |pypi-badge| |downloads-badge| |black-badge| |changelog-badge|
 
 .. |build-badge| image:: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml/badge.svg
    :alt: main branch build status
-.. _build-badge: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml?query=branch%3Amain
+   :target: https://github.com/akaihola/darkgraylib/actions/workflows/python-package.yml?query=branch%3Amain
 .. |license-badge| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
    :alt: BSD 3 Clause license
-.. _license-badge: https://github.com/akaihola/darkgraylib/blob/main/LICENSE
+   :target: https://github.com/akaihola/darkgraylib/blob/main/LICENSE
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/darkgraylib
    :alt: Latest release on PyPI
-.. _pypi-badge: https://pypi.org/project/darkgraylib/
+   :target: https://pypi.org/project/darkgraylib/
 .. |downloads-badge| image:: https://pepy.tech/badge/darkgraylib
    :alt: Number of downloads
-.. _downloads-badge: https://pepy.tech/project/darkgraylib
+   :target: https://pepy.tech/project/darkgraylib
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
-.. _black-badge: https://github.com/psf/black
+   :target: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
-.. _changelog-badge: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/4?color=red&label=release%201.2.0
+   :target: https://github.com/akaihola/darkgraylib/blob/main/CHANGES.rst
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darkgraylib/6?color=red&label=release%201.2.1
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darkgraylib/milestone/4
+   :target: https://github.com/akaihola/darkgraylib/milestone/4
 
 
 What?
 =====
 
 This package is a placeholder for common supporting code for Darker_ and Graylint_.
```

### Comparing `darkgraylib-1.1.1/src/darkgraylib.egg-info/SOURCES.txt` & `darkgraylib-1.2.0/src/darkgraylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

