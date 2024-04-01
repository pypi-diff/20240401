# Comparing `tmp/cyipopt-1.3.0.tar.gz` & `tmp/cyipopt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyipopt-1.3.0.tar", last modified: Sat Sep 23 10:40:20 2023, max compression
+gzip compressed data, was "cyipopt-1.4.0.tar", last modified: Mon Apr  1 15:17:26 2024, max compression
```

## Comparing `cyipopt-1.3.0.tar` & `cyipopt-1.4.0.tar`

### file list

```diff
@@ -1,57 +1,64 @@
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      903 2023-09-23 09:45:24.000000 cyipopt-1.3.0/AUTHORS
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7394 2023-09-23 10:40:17.000000 cyipopt-1.3.0/CHANGELOG.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    14199 2023-09-15 20:17:16.000000 cyipopt-1.3.0/LICENSE
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      324 2023-09-23 09:45:24.000000 cyipopt-1.3.0/MANIFEST.in
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3899 2023-09-23 10:40:20.262858 cyipopt-1.3.0/PKG-INFO
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3082 2023-09-15 20:17:16.000000 cyipopt-1.3.0/README.rst
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.258859 cyipopt-1.3.0/cyipopt/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      399 2023-09-15 20:17:21.000000 cyipopt-1.3.0/cyipopt/__init__.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/cyipopt/cython/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8683 2023-09-15 20:17:16.000000 cyipopt-1.3.0/cyipopt/cython/ipopt.pxd
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    44653 2023-09-23 08:41:55.000000 cyipopt-1.3.0/cyipopt/cython/ipopt_wrapper.pyx
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1356 2023-09-15 20:17:21.000000 cyipopt-1.3.0/cyipopt/exceptions.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2548 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/ipopt_wrapper.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    26638 2023-09-23 07:13:09.000000 cyipopt-1.3.0/cyipopt/scipy_interface.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/cyipopt/tests/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     6366 2023-09-15 20:17:16.000000 cyipopt-1.3.0/cyipopt/tests/conftest.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/cyipopt/tests/integration/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/integration/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8459 2023-09-15 20:17:21.000000 cyipopt-1.3.0/cyipopt/tests/integration/test_hs071.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/integration/test_lasso.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/integration/test_rosen.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/cyipopt/tests/unit/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/unit/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_defaults.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4604 2023-09-15 20:17:16.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_deprecations.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7024 2023-09-23 08:41:55.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_deriv_errors.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_errors.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_exceptions.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    12436 2023-09-15 20:17:16.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_ipopt_funcs.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2023-04-07 05:45:28.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_options.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    20621 2023-09-23 07:13:09.000000 cyipopt-1.3.0/cyipopt/tests/unit/test_scipy_optional.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2854 2021-01-06 21:14:53.000000 cyipopt-1.3.0/cyipopt/utils.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      274 2023-09-23 10:40:17.000000 cyipopt-1.3.0/cyipopt/version.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.258859 cyipopt-1.3.0/cyipopt.egg-info/
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3899 2023-09-23 10:40:20.000000 cyipopt-1.3.0/cyipopt.egg-info/PKG-INFO
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1184 2023-09-23 10:40:20.000000 cyipopt-1.3.0/cyipopt.egg-info/SOURCES.txt
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2023-09-23 10:40:20.000000 cyipopt-1.3.0/cyipopt.egg-info/dependency_links.txt
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2023-09-23 10:40:00.000000 cyipopt-1.3.0/cyipopt.egg-info/not-zip-safe
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       14 2023-09-23 10:40:20.000000 cyipopt-1.3.0/cyipopt.egg-info/requires.txt
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2023-09-23 10:40:20.000000 cyipopt-1.3.0/cyipopt.egg-info/top_level.txt
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/docs/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5577 2021-01-06 21:14:53.000000 cyipopt-1.3.0/docs/Makefile
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5107 2021-01-06 21:14:53.000000 cyipopt-1.3.0/docs/make.bat
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/docs/source/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8540 2023-09-23 09:45:24.000000 cyipopt-1.3.0/docs/source/conf.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1083 2021-04-06 11:42:04.000000 cyipopt-1.3.0/docs/source/development.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1433 2023-09-15 20:17:16.000000 cyipopt-1.3.0/docs/source/index.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18642 2023-09-23 08:41:55.000000 cyipopt-1.3.0/docs/source/install.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      514 2023-09-15 20:17:21.000000 cyipopt-1.3.0/docs/source/reference.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18618 2023-09-15 20:17:16.000000 cyipopt-1.3.0/docs/source/tutorial.rst
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2023-09-23 10:40:20.262858 cyipopt-1.3.0/ipopt/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      486 2021-01-06 21:14:53.000000 cyipopt-1.3.0/ipopt/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      136 2023-09-23 08:41:55.000000 cyipopt-1.3.0/pyproject.toml
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       38 2023-09-23 10:40:20.262858 cyipopt-1.3.0/setup.cfg
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8243 2023-09-23 08:41:55.000000 cyipopt-1.3.0/setup.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      962 2024-04-01 15:14:42.000000 cyipopt-1.4.0/AUTHORS
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7849 2024-04-01 15:14:42.000000 cyipopt-1.4.0/CHANGELOG.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    14199 2023-02-19 14:17:20.000000 cyipopt-1.4.0/LICENSE
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      373 2023-11-28 14:15:09.000000 cyipopt-1.4.0/MANIFEST.in
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3950 2024-04-01 15:17:26.098451 cyipopt-1.4.0/PKG-INFO
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3082 2023-09-15 17:50:42.000000 cyipopt-1.4.0/README.rst
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      399 2024-04-01 15:14:42.000000 cyipopt-1.4.0/cyipopt/__init__.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/cython/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8683 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/cython/ipopt.pxd
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    46828 2024-04-01 14:32:00.000000 cyipopt-1.4.0/cyipopt/cython/ipopt_wrapper.pyx
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1356 2024-04-01 15:14:42.000000 cyipopt-1.4.0/cyipopt/exceptions.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2548 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/ipopt_wrapper.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    27367 2024-04-01 15:14:42.000000 cyipopt-1.4.0/cyipopt/scipy_interface.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/tests/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     6366 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/tests/conftest.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/tests/integration/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/integration/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8459 2023-09-15 18:27:54.000000 cyipopt-1.4.0/cyipopt/tests/integration/test_hs071.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/integration/test_lasso.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/integration/test_rosen.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/cyipopt/tests/unit/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_defaults.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4604 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_deprecations.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7024 2023-11-28 14:15:09.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_deriv_errors.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_errors.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_exceptions.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    12436 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_ipopt_funcs.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_options.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    21685 2023-11-28 14:15:09.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_scipy_optional.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2854 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/utils.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      274 2024-04-01 15:15:05.000000 cyipopt-1.4.0/cyipopt/version.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt.egg-info/
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3950 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/PKG-INFO
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1319 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/not-zip-safe
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       14 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/requires.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/top_level.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/docs/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5577 2020-12-22 10:59:03.000000 cyipopt-1.4.0/docs/Makefile
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5107 2020-12-22 10:59:03.000000 cyipopt-1.4.0/docs/make.bat
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2023-11-28 14:15:09.000000 cyipopt-1.4.0/docs/requirements.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/docs/source/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8540 2024-04-01 15:14:42.000000 cyipopt-1.4.0/docs/source/conf.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1083 2021-07-18 06:03:56.000000 cyipopt-1.4.0/docs/source/development.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1433 2024-04-01 15:14:42.000000 cyipopt-1.4.0/docs/source/index.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18639 2023-11-28 14:15:09.000000 cyipopt-1.4.0/docs/source/install.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      514 2023-09-15 18:27:54.000000 cyipopt-1.4.0/docs/source/reference.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18795 2024-04-01 14:35:21.000000 cyipopt-1.4.0/docs/source/tutorial.rst
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/examples/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4237 2024-04-01 15:14:42.000000 cyipopt-1.4.0/examples/exception_handling.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3912 2024-04-01 15:14:42.000000 cyipopt-1.4.0/examples/hs071.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1996 2022-11-28 12:13:07.000000 cyipopt-1.4.0/examples/hs071_scipy_jax.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5051 2024-04-01 15:14:42.000000 cyipopt-1.4.0/examples/lasso.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      168 2024-04-01 14:39:01.000000 cyipopt-1.4.0/examples/rosen.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/ipopt/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      486 2020-12-22 10:59:03.000000 cyipopt-1.4.0/ipopt/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      133 2023-11-28 14:15:09.000000 cyipopt-1.4.0/pyproject.toml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       38 2024-04-01 15:17:26.098451 cyipopt-1.4.0/setup.cfg
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8286 2024-04-01 15:14:42.000000 cyipopt-1.4.0/setup.py
```

### Comparing `cyipopt-1.3.0/AUTHORS` & `cyipopt-1.4.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 John Siirola <jsiirola@users.noreply.github.com>
 Nikitas Rontsis <nrontsis@gmail.com>
 Robert Parker <robbybparker@gmail.com>
 Matt Haberland <mhaberla@calpoly.edu>
 Benjamin A. Beasley <code@musicinmybrain.net>
 Polina Lakrisenko <p.lakrisenko@gmail.com>
 Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>
+Markus Zimmer <none>
+Thomas Lynn <lynn.thomas.f@gmail.com>
```

### Comparing `cyipopt-1.3.0/CHANGELOG.rst` & `cyipopt-1.4.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,32 @@
 - Removed - for now removed features.
 - Fixed - for any bug fixes.
 - Security - in case of vulnerabilities.
 
 Version History
 ---------------
 
+[1.4.0] - 2024-04-01
+~~~~~~~~~~~~~~~~~~~~
+
+Added
++++++
+
+- Support for building with Cython 3. #227, #240
+- Exposed the ``eps`` kwarg in the SciPy interface. #228
+- Added the examples to the source tarball. #242
+- Documentation improvements on specifics of Jacobian and Hessian inputs.  #247
+- Support for Python 3.12.
+
+Fixed
++++++
+
+- Ensure ``tol`` is always a float in the SciPy interface. #236
+- ``print_level`` allows integers other than 0 or 1. #244
+
 [1.3.0] - 2023-09-23
 ~~~~~~~~~~~~~~~~~~~~
 
 Added
 +++++
 
 - Added a ``pyproject.toml`` file with build dependencies. #162
```

### Comparing `cyipopt-1.3.0/LICENSE` & `cyipopt-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/PKG-INFO` & `cyipopt-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cyipopt
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Cython wrapper to the IPOPT optimization package
 Home-page: https://github.com/mechmotum/cyipopt
 Author: Jason K. Moore
 Author-email: moorepants@gmail.com
 License: EPL-2.0
 Keywords: coin-or,interior-point,ipopt,nlp,nonlinear programming,optimization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: numpy>=1.21.5
 
 ==================
 README for cyipopt
 ==================
```

### Comparing `cyipopt-1.3.0/README.rst` & `cyipopt-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/cython/ipopt.pxd` & `cyipopt-1.4.0/cyipopt/cython/ipopt.pxd`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/cython/ipopt_wrapper.pyx` & `cyipopt-1.4.0/cyipopt/cython/ipopt_wrapper.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -361,15 +361,15 @@
                    "defined.")
             raise ValueError(msg)
 
         #
         # Verify that the constraints and jacobian callbacks are defined
         #
         if m > 0 and (self.__constraints is None or self.__jacobian is None):
-            msg = ("Both the \"constrains\" and \"jacobian\" callbacks must "
+            msg = ("Both the \"constraints\" and \"jacobian\" callbacks must "
                    "be defined.")
             raise ValueError(msg)
 
         cdef Index nele_jac = self.__m * self.__n
         cdef Index nele_hess = <Index>(<long>self.__n * (<long>self.__n + 1) / 2)
 
         if self.__jacobianstructure:
@@ -854,195 +854,339 @@
 # Callback functions
 #
 cdef Bool objective_cb(Index n,
                        Number* x,
                        Bool new_x,
                        Number* obj_value,
                        UserDataPtr user_data
-                       ):
-
-    log(b"objective_cb", logging.INFO)
-
-    cdef object self = <object>user_data
+                       ) noexcept:
+    cdef Problem self
     cdef Index i
-    cdef np.ndarray[DTYPEd_t, ndim=1] _x = np.zeros((n,), dtype=DTYPEd)
-    for i in range(n):
-        _x[i] = x[i]
+    cdef np.ndarray[DTYPEd_t, ndim=1] _x
+
     try:
+        log(b"objective_cb", logging.INFO)
+
+        self = <Problem>user_data
+        _x = np.zeros((n,), dtype=DTYPEd)
+
+        for i in range(n):
+            _x[i] = x[i]
+
         obj_value[0] = self.__objective(_x)
     except CyIpoptEvaluationError:
         return False
     except:
         self.__exception = sys.exc_info()
     return True
 
 
 cdef Bool gradient_cb(Index n,
                       Number* x,
                       Bool new_x,
                       Number* grad_f,
                       UserDataPtr user_data
-                      ):
+                      ) noexcept:
 
-    log(b"gradient_cb", logging.INFO)
-
-    cdef object self = <object>user_data
+    cdef Problem self
     cdef Index i
-    cdef np.ndarray[DTYPEd_t, ndim=1] _x = np.zeros((n,), dtype=DTYPEd)
+    cdef np.ndarray[DTYPEd_t, ndim=1] _x
     cdef np.ndarray[DTYPEd_t, ndim=1] np_grad_f
 
-    for i in range(n):
-        _x[i] = x[i]
-
     try:
+        log(b"gradient_cb", logging.INFO)
+
+        self = <Problem>user_data
+        _x = np.zeros((n,), dtype=DTYPEd)
+
+        for i in range(n):
+            _x[i] = x[i]
+
         ret_val = self.__gradient(_x)
+
+        np_grad_f = np.array(ret_val, dtype=DTYPEd).flatten()
+
+        for i in range(n):
+            grad_f[i] = np_grad_f[i]
+
     except CyIpoptEvaluationError:
         return False
     except:
         self.__exception = sys.exc_info()
         return True
 
-    np_grad_f = np.array(ret_val, dtype=DTYPEd).flatten()
-
-    for i in range(n):
-        grad_f[i] = np_grad_f[i]
-
     return True
 
 
 cdef Bool constraints_cb(Index n,
                          Number* x,
                          Bool new_x,
                          Index m,
                          Number* g,
                          UserDataPtr user_data
-                         ):
+                         ) noexcept:
+    cdef Problem self
+    cdef Index i
+    cdef np.ndarray[DTYPEd_t, ndim=1] _x
+    cdef np.ndarray[DTYPEd_t, ndim=1] np_g
+
+    try:
+        log(b"constraints_cb", logging.INFO)
+
+        self = <Problem>user_data
+        _x = np.zeros((n,), dtype=DTYPEd)
 
-    log(b"constraints_cb", logging.INFO)
+        if not self.__constraints:
+            log(b"Constraints callback not defined", logging.DEBUG)
+            return True
+
+        for i in range(n):
+            _x[i] = x[i]
+
+        ret_val = self.__constraints(_x)
 
-    cdef object self = <object>user_data
+        np_g = np.array(ret_val, dtype=DTYPEd).flatten()
+
+        for i in range(m):
+            g[i] = np_g[i]
+
+    except CyIpoptEvaluationError:
+        return False
+    except:
+        self.__exception = sys.exc_info()
+        return True
+
+    return True
+
+
+cdef Bool jacobian_struct_cb(Index n,
+                             Index m,
+                             Index nele_jac,
+                             Index *iRow,
+                             Index *jCol,
+                             UserDataPtr user_data):
+    cdef Problem self = <Problem>user_data
+    cdef Index i
+
+    if not self.__jacobianstructure:
+        msg = b"Jacobian callback not defined. assuming a dense jacobian"
+        log(msg, logging.INFO)
+
+        #
+        # Assuming a dense Jacobian
+        #
+        s = np.unravel_index(np.arange(self.__m * self.__n),
+                             (self.__m, self.__n))
+        np_iRow = np.array(s[0], dtype=DTYPEi)
+        np_jCol = np.array(s[1], dtype=DTYPEi)
+    else:
+        #
+        # Sparse Jacobian
+        #
+        ret_val = self.__jacobianstructure()
+
+        np_iRow = np.array(ret_val[0], dtype=DTYPEi).flatten()
+        np_jCol = np.array(ret_val[1], dtype=DTYPEi).flatten()
+
+        if (np_iRow.size != nele_jac) or (np_jCol.size != nele_jac):
+            msg = b"Invalid number of indices returned from jacobianstructure"
+            log(msg, logging.ERROR)
+            return False
+
+        if (np_iRow < 0).any() or (np_iRow >= m).any():
+            msg = b"Invalid row indices returned from jacobianstructure"
+            log(msg, logging.ERROR)
+            return False
+
+        if (np_jCol < 0).any() or (np_jCol >= n).any():
+            msg = b"Invalid column indices returned from jacobianstructure"
+            log(msg, logging.ERROR)
+            return False
+
+    for i in range(nele_jac):
+        iRow[i] = np_iRow[i]
+        jCol[i] = np_jCol[i]
+
+    return True
+
+
+cdef Bool jacobian_value_cb(Index n,
+                            Number* x,
+                            Bool new_x,
+                            Index m,
+                            Index nele_jac,
+                            Number *values,
+                            UserDataPtr user_data
+                            ):
+    cdef Problem self = <Problem>user_data
     cdef Index i
     cdef np.ndarray[DTYPEd_t, ndim=1] _x = np.zeros((n,), dtype=DTYPEd)
-    cdef np.ndarray[DTYPEd_t, ndim=1] np_g
 
-    if not self.__constraints:
-        log(b"Constraints callback not defined", logging.DEBUG)
+    if not self.__jacobian:
+        log(b"Jacobian callback not defined", logging.DEBUG)
         return True
 
     for i in range(n):
         _x[i] = x[i]
 
     try:
-        ret_val = self.__constraints(_x)
+        ret_val = self.__jacobian(_x)
     except CyIpoptEvaluationError:
-        return False
-    except:
-        self.__exception = sys.exc_info()
-        return True
+            return False
 
-    np_g = np.array(ret_val, dtype=DTYPEd).flatten()
+    np_jac_g = np.array(ret_val, dtype=DTYPEd).flatten()
 
-    for i in range(m):
-        g[i] = np_g[i]
+    if (np_jac_g.size != nele_jac):
+        msg = b"Invalid number of indices returned from jacobian"
+        log(msg, logging.ERROR)
+        return False
+
+    for i in range(nele_jac):
+        values[i] = np_jac_g[i]
 
     return True
 
 
 cdef Bool jacobian_cb(Index n,
                       Number* x,
                       Bool new_x,
                       Index m,
                       Index nele_jac,
                       Index *iRow,
                       Index *jCol,
                       Number *values,
                       UserDataPtr user_data
-                      ):
+                      ) noexcept:
+    cdef Problem self
+    cdef object ret_val
+
+    try:
+        log(b"jacobian_cb", logging.INFO)
+        ret_val = True
+        self = <Problem>user_data
+        if values == NULL:
+            log(b"Querying for iRow/jCol indices of the jacobian", logging.INFO)
+            ret_val = jacobian_struct_cb(n, m, nele_jac, iRow, jCol, user_data)
+        else:
+            log(b"Querying for jacobian", logging.INFO)
+            ret_val = jacobian_value_cb(n, x, new_x, m, nele_jac, values, user_data)
+
+    except:
+        self.__exception = sys.exc_info()
+    finally:
+        return ret_val
 
-    log(b"jacobian_cb", logging.INFO)
 
-    cdef object self = <object>user_data
+cdef Bool hessian_struct_cb(Index n,
+                            Index m,
+                            Index nele_hess,
+                            Index *iRow,
+                            Index *jCol,
+                            UserDataPtr user_data
+                            ):
+    cdef Problem self = <Problem>user_data
     cdef Index i
-    cdef np.ndarray[DTYPEd_t, ndim=1] _x = np.zeros((n,), dtype=DTYPEd)
     cdef np.ndarray[DTYPEi_t, ndim=1] np_iRow
     cdef np.ndarray[DTYPEi_t, ndim=1] np_jCol
-    cdef np.ndarray[DTYPEd_t, ndim=1] np_jac_g
 
-    if values == NULL:
-        log(b"Querying for iRow/jCol indices of the jacobian", logging.INFO)
+    msg = b"Querying for iRow/jCol indices of the Hessian"
+    log(msg, logging.INFO)
 
-        if not self.__jacobianstructure:
-            msg = b"Jacobian callback not defined. assuming a dense jacobian"
-            log(msg, logging.INFO)
+    if not self.__hessianstructure:
+        msg = (b"Hessian callback not defined. assuming a lower triangle "
+               b"Hessian")
+        log(msg, logging.INFO)
 
-            #
-            # Assuming a dense Jacobian
-            #
-            s = np.unravel_index(np.arange(self.__m * self.__n),
-                                 (self.__m, self.__n))
-            np_iRow = np.array(s[0], dtype=DTYPEi)
-            np_jCol = np.array(s[1], dtype=DTYPEi)
-        else:
-            #
-            # Sparse Jacobian
-            #
-            try:
-                ret_val = self.__jacobianstructure()
-            except:
-                self.__exception = sys.exc_info()
-                return True
-
-            np_iRow = np.array(ret_val[0], dtype=DTYPEi).flatten()
-            np_jCol = np.array(ret_val[1], dtype=DTYPEi).flatten()
-
-            if (np_iRow.size != nele_jac) or (np_jCol.size != nele_jac):
-                msg = b"Invalid number of indices returned from jacobianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-            if (np_iRow < 0).any() or (np_iRow >= m).any():
-                msg = b"Invalid row indices returned from jacobianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-            if (np_jCol < 0).any() or (np_jCol >= n).any():
-                msg = b"Invalid column indices returned from jacobianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-        for i in range(nele_jac):
-            iRow[i] = np_iRow[i]
-            jCol[i] = np_jCol[i]
+        #
+        # Assuming a lower triangle Hessian
+        # Note:
+        # There is a need to reconvert the s.col and s.row to arrays
+        # because they have the wrong stride
+        #
+        row, col = np.nonzero(np.tril(np.ones((self.__n, self.__n))))
+        np_iRow = np.array(col, dtype=DTYPEi)
+        np_jCol = np.array(row, dtype=DTYPEi)
     else:
-        log(b"Querying for jacobian", logging.INFO)
+        #
+        # Sparse Hessian
+        #
+        ret_val = self.__hessianstructure()
 
-        if not self.__jacobian:
-            log(b"Jacobian callback not defined", logging.DEBUG)
-            return True
+        np_iRow = np.array(ret_val[0], dtype=DTYPEi).flatten()
+        np_jCol = np.array(ret_val[1], dtype=DTYPEi).flatten()
 
-        for i in range(n):
-            _x[i] = x[i]
+        if (np_iRow.size != nele_hess) or (np_jCol.size != nele_hess):
+            msg = b"Invalid number of indices returned from hessianstructure"
+            log(msg, logging.ERROR)
+            return False
 
-        try:
-            ret_val = self.__jacobian(_x)
-        except CyIpoptEvaluationError:
+        if not(np_iRow >= np_jCol).all():
+            msg = b"Indices are not lower triangular in hessianstructure"
+            log(msg, logging.ERROR)
             return False
-        except:
-            self.__exception = sys.exc_info()
-            return True
 
-        np_jac_g = np.array(ret_val, dtype=DTYPEd).flatten()
+        if (np_jCol < 0).any():
+            msg = b"Invalid column indices returned from hessianstructure"
+            log(msg, logging.ERROR)
+            return False
 
-        if (np_jac_g.size != nele_jac):
-            msg = b"Invalid number of indices returned from jacobian"
+        if (np_iRow >= n).any():
+            msg = b"Invalid row indices returned from hessianstructure"
             log(msg, logging.ERROR)
             return False
 
-        for i in range(nele_jac):
-            values[i] = np_jac_g[i]
+    for i in range(nele_hess):
+        iRow[i] = np_iRow[i]
+        jCol[i] = np_jCol[i]
+
+    return True
+
+
+cdef Bool hessian_value_cb(Index n,
+                           Number* x,
+                           Bool new_x,
+                           Number obj_factor,
+                           Index m,
+                           Number *lambd,
+                           Bool new_lambda,
+                           Index nele_hess,
+                           Number *values,
+                           UserDataPtr user_data
+                           ):
+    cdef Index i
+    cdef Problem self = <Problem>user_data
+    cdef np.ndarray[DTYPEd_t, ndim=1] _x = np.zeros((n,), dtype=DTYPEd)
+    cdef np.ndarray[DTYPEd_t, ndim=1] _lambda = np.zeros((m,), dtype=DTYPEd)
+
+    if not self.__hessian:
+        msg = (b"Hessian callback not defined but called by the Ipopt "
+               b"algorithm")
+        log(msg, logging.ERROR)
+        return False
+
+    for i in range(n):
+        _x[i] = x[i]
+
+    for i in range(m):
+        _lambda[i] = lambd[i]
+
+    try:
+        ret_val = self.__hessian(_x, _lambda, obj_factor)
+    except CyIpoptEvaluationError:
+        return False
+
+    np_h = np.array(ret_val, dtype=DTYPEd).flatten()
+
+    if (np_h.size != nele_hess):
+        msg = b"Invalid number of indices returned from hessian"
+        log(msg, logging.ERROR)
+        return False
+
+    for i in range(nele_hess):
+        values[i] = np_h[i]
 
     return True
 
 
 cdef Bool hessian_cb(Index n,
                      Number* x,
                      Bool new_x,
@@ -1051,155 +1195,94 @@
                      Number *lambd,
                      Bool new_lambda,
                      Index nele_hess,
                      Index *iRow,
                      Index *jCol,
                      Number *values,
                      UserDataPtr user_data
-                     ):
+                     ) noexcept:
+    cdef object self
+    cdef object ret_val
 
-    log(b"hessian_cb", logging.INFO)
-
-    cdef object self = <object>user_data
-    cdef Index i
-    cdef np.ndarray[DTYPEd_t, ndim=1] _x = np.zeros((n,), dtype=DTYPEd)
-    cdef np.ndarray[DTYPEd_t, ndim=1] _lambda = np.zeros((m,), dtype=DTYPEd)
-    cdef np.ndarray[DTYPEi_t, ndim=1] np_iRow
-    cdef np.ndarray[DTYPEi_t, ndim=1] np_jCol
-    cdef np.ndarray[DTYPEd_t, ndim=1] np_h
-
-    if values == NULL:
-        msg = b"Querying for iRow/jCol indices of the Hessian"
-        log(msg, logging.INFO)
-
-        if not self.__hessianstructure:
-            msg = (b"Hessian callback not defined. assuming a lower triangle "
-                   b"Hessian")
-            log(msg, logging.INFO)
+    try:
+        log(b"hessian_cb", logging.INFO)
+        ret_val = True
+        self = <object>user_data
+
+        if values == NULL:
+            ret_val = hessian_struct_cb(n,
+                                        m,
+                                        nele_hess,
+                                        iRow,
+                                        jCol,
+                                        user_data)
 
-            #
-            # Assuming a lower triangle Hessian
-            # Note:
-            # There is a need to reconvert the s.col and s.row to arrays
-            # because they have the wrong stride
-            #
-            row, col = np.nonzero(np.tril(np.ones((self.__n, self.__n))))
-            np_iRow = np.array(col, dtype=DTYPEi)
-            np_jCol = np.array(row, dtype=DTYPEi)
         else:
-            #
-            # Sparse Hessian
-            #
-            try:
-                ret_val = self.__hessianstructure()
-            except:
-                self.__exception = sys.exc_info()
-                return True
-
-            np_iRow = np.array(ret_val[0], dtype=DTYPEi).flatten()
-            np_jCol = np.array(ret_val[1], dtype=DTYPEi).flatten()
-
-            if (np_iRow.size != nele_hess) or (np_jCol.size != nele_hess):
-                msg = b"Invalid number of indices returned from hessianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-            if not(np_iRow >= np_jCol).all():
-                msg = b"Indices are not lower triangular in hessianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-            if (np_jCol < 0).any():
-                msg = b"Invalid column indices returned from hessianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-            if (np_iRow >= n).any():
-                msg = b"Invalid row indices returned from hessianstructure"
-                log(msg, logging.ERROR)
-                return False
-
-        for i in range(nele_hess):
-            iRow[i] = np_iRow[i]
-            jCol[i] = np_jCol[i]
-    else:
-        if not self.__hessian:
-            msg = (b"Hessian callback not defined but called by the Ipopt "
-                   b"algorithm")
-            log(msg, logging.ERROR)
-            return False
-
-        for i in range(n):
-            _x[i] = x[i]
-
-        for i in range(m):
-            _lambda[i] = lambd[i]
-
-        try:
-            ret_val = self.__hessian(_x, _lambda, obj_factor)
-        except CyIpoptEvaluationError:
-            return False
-        except:
-            self.__exception = sys.exc_info()
-            return True
-
-        np_h = np.array(ret_val, dtype=DTYPEd).flatten()
-
-        if (np_h.size != nele_hess):
-            msg = b"Invalid number of indices returned from hessian"
-            log(msg, logging.ERROR)
-            return False
-
-        for i in range(nele_hess):
-            values[i] = np_h[i]
-
-    return True
+            ret_val = hessian_value_cb(n,
+                                       x,
+                                       new_x,
+                                       obj_factor,
+                                       m,
+                                       lambd,
+                                       new_lambda,
+                                       nele_hess,
+                                       values,
+                                       user_data)
+    except:
+        self.__exception = sys.exc_info()
+    finally:
+        return ret_val
 
 
 cdef Bool intermediate_cb(Index alg_mod,
                           Index iter_count,
                           Number obj_value,
                           Number inf_pr,
                           Number inf_du,
                           Number mu,
                           Number d_norm,
                           Number regularization_size,
                           Number alpha_du,
                           Number alpha_pr,
                           Index ls_trials,
                           UserDataPtr user_data
-                          ):
+                          ) noexcept:
+    cdef Problem self
 
-    log(b"intermediate_cb", logging.INFO)
+    try:
+        log(b"intermediate_cb", logging.INFO)
 
-    cdef object self = <object>user_data
+        self = <Problem>user_data
 
-    if self.__exception:
-        return False
+        if self.__exception:
+            return False
 
-    if not self.__intermediate:
-        return True
+        if not self.__intermediate:
+            return True
 
-    ret_val = self.__intermediate(alg_mod,
+        ret_val = self.__intermediate(alg_mod,
                                   iter_count,
-                                  obj_value,
-                                  inf_pr,
-                                  inf_du,
-                                  mu,
-                                  d_norm,
-                                  regularization_size,
-                                  alpha_du,
-                                  alpha_pr,
-                                  ls_trials
-                                  )
+                                      obj_value,
+                                      inf_pr,
+                                      inf_du,
+                                      mu,
+                                      d_norm,
+                                      regularization_size,
+                                      alpha_du,
+                                      alpha_pr,
+                                      ls_trials
+                                      )
 
-    if ret_val is None:
+        if ret_val is None:
+            return True
+    except:
+        self.__exception = sys.exc_info()
         return True
 
-    return ret_val
+    return True
 
 
 class problem(Problem):
     """Class to continue support for old API.
 
     .. deprecated:: 1.0.0
        :class:`problem` will be removed in CyIpopt 1.1.0, it is replaced by
```

### Comparing `cyipopt-1.3.0/cyipopt/exceptions.py` & `cyipopt-1.4.0/cyipopt/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 cyipopt: Python wrapper for the Ipopt optimization package, written in Cython.
 
 Copyright (C) 2012-2015 Amit Aides
 Copyright (C) 2015-2017 Matthias Kümmerer
-Copyright (C) 2017-2023 cyipopt developers
+Copyright (C) 2017-2024 cyipopt developers
 
 License: EPL 2.0
 """
 
 class CyIpoptEvaluationError(ArithmeticError):
     """An exception that should be raised in evaluation callbacks to signal
     to CyIpopt that a numerical error occured during function evaluation.
```

### Comparing `cyipopt-1.3.0/cyipopt/ipopt_wrapper.py` & `cyipopt-1.4.0/cyipopt/ipopt_wrapper.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/scipy_interface.py` & `cyipopt-1.4.0/cyipopt/scipy_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 cyipopt: Python wrapper for the Ipopt optimization package, written in Cython.
 
 Copyright (C) 2012-2015 Amit Aides
 Copyright (C) 2015-2017 Matthias Kümmerer
-Copyright (C) 2017-2023 cyipopt developers
+Copyright (C) 2017-2024 cyipopt developers
 
 License: EPL 2.0
 """
 
 import sys
 
 import numpy as np
@@ -53,16 +53,17 @@
     args : tuple, optional
         Extra arguments passed to the objective function and its derivatives
         (``fun``, ``jac``, ``hess``).
     kwargs : dictionary, optional
         Extra keyword arguments passed to the objective function and its
         derivatives (``fun``, ``jac``, ``hess``).
     jac : callable, optional
-        The Jacobian of the objective function: ``jac(x, *args, **kwargs) ->
-        ndarray, shape(n, )``. If ``None``, SciPy's ``approx_fprime`` is used.
+        The Jacobian (gradient) of the objective function:
+        ``jac(x, *args, **kwargs) -> ndarray, shape(n, )``.
+        If ``None``, SciPy's ``approx_fprime`` is used.
     hess : callable, optional
         If ``None``, the Hessian is computed using IPOPT's numerical methods.
         Explicitly defined Hessians are not yet supported for this class.
     hessp : callable, optional
         If ``None``, the Hessian is computed using IPOPT's numerical methods.
         Explicitly defined Hessians are not yet supported for this class.
     constraints : {Constraint, dict} or List of {Constraint, dict}, optional
@@ -70,15 +71,16 @@
         the jacobian of each constraint corresponds to the `'jac'` key and must
         be a callable function with signature ``jac(x) -> {ndarray,
         coo_array}``. If the constraint's value of `'jac'` is a boolean and
         True, the constraint function `fun` is expected to return a tuple
         `(con_val, con_jac)` consisting of the evaluated constraint `con_val`
         and the evaluated jacobian `con_jac`.
     eps : float, optional
-        Epsilon used in finite differences.
+        Step size used in finite difference approximations of the objective
+        function gradient and constraint Jacobian.
     con_dims : array_like, optional
         Dimensions p_1, ..., p_m of the m constraint functions
         g_1, ..., g_m : R^n -> R^(p_i).
     sparse_jacs: array_like, optional
         If sparse_jacs[i] = True, the i-th constraint's jacobian is sparse.
         Otherwise, the i-th constraint jacobian is assumed to be dense.
     jac_nnz_row: array_like, optional
@@ -432,16 +434,17 @@
     kwargs : dictionary, optional
         Extra keyword arguments passed to the objective function and its
         derivatives (``fun``, ``jac``, ``hess``).
     method : str, optional
         If unspecified (default), Ipopt is used.
         :py:func:`scipy.optimize.minimize` methods can also be used.
     jac : callable, optional
-        The Jacobian of the objective function: ``jac(x, *args, **kwargs) ->
-        ndarray, shape(n, )``. If ``None``, SciPy's ``approx_fprime`` is used.
+        The Jacobian (gradient) of the objective function:
+        ``jac(x, *args, **kwargs) -> ndarray, shape(n, )``.
+        If ``None``, SciPy's ``approx_fprime`` is used.
     hess : callable, optional
         The Hessian of the objective function:
         ``hess(x) -> ndarray, shape(n, )``.
         If ``None``, the Hessian is computed using IPOPT's numerical methods.
     hessp : callable, optional
         If `method` is one of the SciPy methods, this is a callable that
         produces the inner product of the Hessian and a vector. Otherwise, an
@@ -465,26 +468,36 @@
         constraint function ``fun`` must return a tuple ``(con_val, con_jac)``
         consisting of the evaluated constraint ``con_val`` and the evaluated
         Jacobian ``con_jac``.
     tol : float, optional (default=1e-8)
         The desired relative convergence tolerance, passed as an option to
         Ipopt. See [1]_ for details.
     options : dict, optional
-        A dictionary of solver options. The options ``disp`` and ``maxiter``
-        are automatically mapped to their Ipopt equivalents ``print_level``
-        and ``max_iter``. All other options are passed directly to Ipopt. See
-        [1]_ for details.
+        A dictionary of solver options.
+
+        When `method` is unspecified (default: Ipopt), the options
+        ``disp`` and ``maxiter`` are automatically mapped to their Ipopt
+        equivalents ``print_level`` and ``max_iter``, and ``eps`` is used to
+        control the step size of finite difference gradient and constraint
+        Jacobian approximations. All other options are passed directly
+        to Ipopt. See [1]_ for details.
+
+        For other values of `method`, `options` is passed to the SciPy solver.
+        See [2]_ for details.
     callback : callable, optional
-        This parameter is ignored unless `method` is one of the SciPy
-        methods.
+        This argument is ignored by the default `method` (Ipopt).
+        If `method` is one of the SciPy methods, this is a callable that is
+        called once per iteration. See [2]_ for details.
 
     References
     ----------
     .. [1] COIN-OR Project. "Ipopt: Ipopt Options".
            https://coin-or.github.io/Ipopt/OPTIONS.html
+    .. [2] The SciPy Developers. "scipy.optimize.minimize".
+           https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html
 
     Examples
     --------
     Consider the problem of minimizing the Rosenbrock function. The Rosenbrock
     function and its derivatives are implemented in
     :py:func:`scipy.optimize.rosen`, :py:func:`scipy.optimize.rosen_der`, and
     :py:func:`scipy.optimize.rosen_hess`.
@@ -548,48 +561,47 @@
 
     lb, ub = bounds
     cl, cu = get_constraint_bounds(constraints, _x0)
     con_dims = get_constraint_dimensions(constraints, _x0)
     sparse_jacs, jac_nnz_row, jac_nnz_col = _get_sparse_jacobian_structure(
         constraints, x0)
 
+    if options is None:
+        options = {}
+    eps = options.pop('eps', 1e-8)
+
     problem = IpoptProblemWrapper(fun,
                                   args=args,
                                   kwargs=kwargs,
                                   jac=jac,
                                   hess=hess,
                                   hessp=hessp,
                                   constraints=constraints,
-                                  eps=1e-8,
+                                  eps=eps,
                                   con_dims=con_dims,
                                   sparse_jacs=sparse_jacs,
                                   jac_nnz_row=jac_nnz_row,
                                   jac_nnz_col=jac_nnz_col)
 
-    if options is None:
-        options = {}
-
     nlp = cyipopt.Problem(n=len(x0),
                           m=len(cl),
                           problem_obj=problem,
                           lb=lb,
                           ub=ub,
                           cl=cl,
                           cu=cu)
 
     # python3 compatibility
     convert_to_bytes(options)
 
     # Rename some default scipy options
     replace_option(options, b'disp', b'print_level')
     replace_option(options, b'maxiter', b'max_iter')
-    if getattr(options, 'print_level', False) is True:
-        options[b'print_level'] = 1
-    else:
-        options[b'print_level'] = 0
+    options[b'print_level'] = int(options.get(b'print_level', 0))
+
     if b'tol' not in options:
         options[b'tol'] = tol or 1e-8
     if b'mu_strategy' not in options:
         options[b'mu_strategy'] = b'adaptive'
     if b'hessian_approximation' not in options:
         if hess is None and hessp is None:
             options[b'hessian_approximation'] = b'limited-memory'
@@ -664,14 +676,16 @@
     if method is None and callback is not None:
         raise NotImplementedError('`callback` is not yet supported by Ipopt.`')
 
     if tol is not None:
         tol = np.asarray(tol)[()]
         if tol.ndim != 0 or not np.issubdtype(tol.dtype, np.number) or tol <= 0:
             raise ValueError('`tol` must be a positive scalar.')
+        else:  # tol should be a float, not an array
+            tol = float(tol)
 
     options = dict() if options is None else options
     if not isinstance(options, dict):
         raise ValueError('`options` must be a dictionary.')
 
     return (fun, x0, args, kwargs, method, jac, hess, hessp,
             bounds, constraints, tol, callback, options)
```

### Comparing `cyipopt-1.3.0/cyipopt/tests/conftest.py` & `cyipopt-1.4.0/cyipopt/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/tests/integration/test_hs071.py` & `cyipopt-1.4.0/cyipopt/tests/integration/test_hs071.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/tests/unit/test_deprecations.py` & `cyipopt-1.4.0/cyipopt/tests/unit/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/tests/unit/test_deriv_errors.py` & `cyipopt-1.4.0/cyipopt/tests/unit/test_deriv_errors.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/tests/unit/test_ipopt_funcs.py` & `cyipopt-1.4.0/cyipopt/tests/unit/test_ipopt_funcs.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt/tests/unit/test_scipy_optional.py` & `cyipopt-1.4.0/cyipopt/tests/unit/test_scipy_optional.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,30 @@
                                    "`minimize_ipopt` function.")
     with pytest.raises(ImportError, match=expected_error_msg):
         cyipopt.minimize_ipopt(None, None)
 
 
 @pytest.mark.skipif("scipy" not in sys.modules,
                     reason="Test only valid if Scipy available.")
+def test_tol_type_issue_235():
+    # from: https://github.com/mechmotum/cyipopt/issues/235
+
+    def fun(x):
+        return np.sum(x ** 2)
+
+    # tol should not raise an error
+    cyipopt.minimize_ipopt(
+        fun=fun,
+        x0=np.zeros(2),
+        tol=1e-9,
+    )
+
+
+@pytest.mark.skipif("scipy" not in sys.modules,
+                    reason="Test only valid if Scipy available.")
 def test_minimize_ipopt_input_validation():
     from scipy import optimize
 
     x0 = 1
     def f(x):
         return x @ x
 
@@ -571,7 +587,29 @@
     bnds = ((0, None), (0, None))
 
     res = cyipopt.minimize_ipopt(fun, (2, 0), bounds=bnds, constraints=cons)
     ref = minimize(fun, (2, 0), bounds=bnds, constraints=cons)
     assert res.success
     np.testing.assert_allclose(res.x, ref.x)
     np.testing.assert_allclose(res.fun, ref.fun)
+
+
+@pytest.mark.skipif("scipy" not in sys.modules,
+                    reason="Test only valid if Scipy available.")
+def test_gh115_eps_option():
+    # gh-115 requested that the `eps` argument be exposed as an option. Verify
+    # that it is working as advertised (at least for the objective function).
+    def f(x):
+        if f.x is None:
+            f.x = x
+        elif f.dx is None:
+            f.dx = x - f.x
+        return x ** 2
+
+    f.x, f.dx = None, None
+    cyipopt.minimize_ipopt(f, x0=0)
+    np.testing.assert_equal(f.dx, 1e-8)
+
+    f.x, f.dx = None, None
+    eps = 1e-9
+    cyipopt.minimize_ipopt(f, x0=0, options={'eps': eps})
+    np.testing.assert_equal(f.dx, eps)
```

### Comparing `cyipopt-1.3.0/cyipopt/utils.py` & `cyipopt-1.4.0/cyipopt/utils.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/cyipopt.egg-info/PKG-INFO` & `cyipopt-1.4.0/cyipopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cyipopt
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Cython wrapper to the IPOPT optimization package
 Home-page: https://github.com/mechmotum/cyipopt
 Author: Jason K. Moore
 Author-email: moorepants@gmail.com
 License: EPL-2.0
 Keywords: coin-or,interior-point,ipopt,nlp,nonlinear programming,optimization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: numpy>=1.21.5
 
 ==================
 README for cyipopt
 ==================
```

### Comparing `cyipopt-1.3.0/cyipopt.egg-info/SOURCES.txt` & `cyipopt-1.4.0/cyipopt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 cyipopt/tests/unit/test_errors.py
 cyipopt/tests/unit/test_exceptions.py
 cyipopt/tests/unit/test_ipopt_funcs.py
 cyipopt/tests/unit/test_options.py
 cyipopt/tests/unit/test_scipy_optional.py
 docs/Makefile
 docs/make.bat
+docs/requirements.txt
 docs/source/conf.py
 docs/source/development.rst
 docs/source/index.rst
 docs/source/install.rst
 docs/source/reference.rst
 docs/source/tutorial.rst
+examples/exception_handling.py
+examples/hs071.py
+examples/hs071_scipy_jax.py
+examples/lasso.py
+examples/rosen.py
 ipopt/__init__.py
```

### Comparing `cyipopt-1.3.0/docs/Makefile` & `cyipopt-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/docs/make.bat` & `cyipopt-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/docs/source/conf.py` & `cyipopt-1.4.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'cyipopt'
-copyright = u'2023, cyipopt developers'
+copyright = u'2024, cyipopt developers'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = __version__
```

### Comparing `cyipopt-1.3.0/docs/source/development.rst` & `cyipopt-1.4.0/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/docs/source/index.rst` & `cyipopt-1.4.0/docs/source/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -49,9 +49,9 @@
 * :ref:`search`
 
 Copyright
 =========
 
 | Copyright (C) 2012-2015 Amit Aides
 | Copyright (C) 2015-2017 Matthias Kümmerer
-| Copyright (C) 2017-2023 cyipopt developers
+| Copyright (C) 2017-2024 cyipopt developers
 | License: EPL 2.0
```

### Comparing `cyipopt-1.3.0/docs/source/install.rst` & `cyipopt-1.4.0/docs/source/install.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 dependencies:
 
   * C/C++ compiler
   * pkg-config [only for Linux and Mac]
   * Ipopt >=3.12 [>= 3.13 on Windows]
   * Python 3.8+
   * setuptools >=44.1.1
-  * cython >=0.29.28,<3
+  * cython >=0.29.28
   * NumPy >=1.21.5
   * SciPy >=1.8 [optional]
 
 The binaries and header files of the Ipopt package can be obtained from
 http://www.coin-or.org/download/binary/Ipopt/. These include a version compiled
 against the MKL library. Or you can build Ipopt from source. The remaining
 dependencies can be installed with conda or other package managers.
```

### Comparing `cyipopt-1.3.0/docs/source/reference.rst` & `cyipopt-1.4.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.3.0/docs/source/tutorial.rst` & `cyipopt-1.4.0/docs/source/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -249,23 +249,26 @@
 - :func:`cyipopt.Problem.hessian`
 
 The :func:`cyipopt.Problem.jacobian` and :func:`cyipopt.Problem.hessian`
 methods should return the non-zero values of the respective matrices as
 flattened arrays. The hessian should return a flattened lower triangular
 matrix.
 
-The Jacobian and Hessian can be dense or sparse. If sparse, you must also
-define:
+The Jacobian and Hessian can be dense or sparse. If sparse,
+:func:`cyipopt.Problem.jacobian` and :func:`cyipopt.Problem.hessian` methods
+should return only the non-zero values of the respective matrices and you must
+also define:
 
 - :func:`cyipopt.Problem.jacobianstructure`
 - :func:`cyipopt.Problem.hessianstructure`
 
-which should return a tuple of indices that indicate the location of the
-non-zero values of the Jacobian and Hessian matrices, respectively. If not
-defined then these matrices are assumed to be dense.
+which should return a tuple of indices (row indices, column indices) that
+indicate the location of the non-zero values of the Jacobian and Hessian
+matrices, respectively. If not defined then these matrices are assumed to be
+dense.
 
 The :func:`cyipopt.Problem.intermediate` method is called every Ipopt iteration
 algorithm and can be used to perform any needed computation at each iteration.
 
 Define the problem class::
 
    class HS071():
```

### Comparing `cyipopt-1.3.0/setup.py` & `cyipopt-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 cyipopt: Python wrapper for the Ipopt optimization package, written in Cython.
 
 Copyright (C) 2012-2015 Amit Aides
 Copyright (C) 2015-2017 Matthias Kümmerer
-Copyright (C) 2017-2023 cyipopt developers
+Copyright (C) 2017-2024 cyipopt developers
 
 License: EPL 2.0
 """
 
 import sys
 import os.path
 from distutils.sysconfig import get_python_lib
@@ -16,15 +16,15 @@
 
 from setuptools import setup
 from setuptools.extension import Extension
 
 # install requirements before import
 from setuptools import dist
 SETUP_REQUIRES = [
-    "cython>=0.29.28,<3",
+    "cython>=0.29.28",
     "numpy>=1.21.5",
     "setuptools>=44.1.1",
 ]
 dist.Distribution().fetch_build_eggs(SETUP_REQUIRES)
 
 from Cython.Distutils import build_ext
 import numpy as np
@@ -57,14 +57,15 @@
     "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 
 def pkgconfig(*packages, **kw):
     """Returns a dictionary containing the include and library flags to pass to
     a Python extension that depends on the provided packages.
```

