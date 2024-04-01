# Comparing `tmp/gigalixir-1.9.1.tar.gz` & `tmp/gigalixir-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigalixir-1.9.1.tar", last modified: Tue Nov 21 12:46:54 2023, max compression
+gzip compressed data, was "gigalixir-1.9.3.tar", last modified: Thu Dec  7 03:14:03 2023, max compression
```

## Comparing `gigalixir-1.9.1.tar` & `gigalixir-1.9.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-11-21 12:46:54.573454 gigalixir-1.9.1/
--rw-rw-r--   0 tim       (1001) tim       (1001)     1081 2023-10-01 19:00:59.000000 gigalixir-1.9.1/LICENSE
--rw-r--r--   0 tim       (1001) tim       (1001)      724 2023-11-21 12:46:54.573454 gigalixir-1.9.1/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)      420 2023-10-01 19:00:59.000000 gigalixir-1.9.1/README.md
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-11-21 12:46:54.573454 gigalixir-1.9.1/gigalixir/
--rw-rw-r--   0 tim       (1001) tim       (1001)    40529 2023-10-14 03:38:21.000000 gigalixir-1.9.1/gigalixir/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      229 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/api_exception.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      858 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/api_key.py
--rw-rw-r--   0 tim       (1001) tim       (1001)    10764 2023-10-14 03:38:21.000000 gigalixir-1.9.1/gigalixir/app.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      538 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/app_activity.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      391 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/auth.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1560 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/canary.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1966 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/config.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     5314 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/database.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1633 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/domain.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      555 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/free_database.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      601 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/git.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      446 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/invoice.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1262 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/log_drain.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     2653 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/mfa.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     3084 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/netrc.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     7263 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/observer.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-11-21 12:46:54.573454 gigalixir-1.9.1/gigalixir/openers/
--rw-rw-r--   0 tim       (1001) tim       (1001)        0 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/openers/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      207 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/openers/darwin.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      214 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/openers/linux.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      210 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/openers/windows.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1172 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/payment_method.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1274 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/permission.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      347 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/presenter.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      538 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/release.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-11-21 12:46:54.573454 gigalixir-1.9.1/gigalixir/routers/
--rw-rw-r--   0 tim       (1001) tim       (1001)        0 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/routers/__init__.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1551 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/routers/darwin.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      902 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/routers/linux.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      618 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/routers/windows.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1490 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/shell.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     1234 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/ssh_key.py
--rw-rw-r--   0 tim       (1001) tim       (1001)      801 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/usage.py
--rw-rw-r--   0 tim       (1001) tim       (1001)     7549 2023-10-01 19:00:59.000000 gigalixir-1.9.1/gigalixir/user.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-11-21 12:46:54.573454 gigalixir-1.9.1/gigalixir.egg-info/
--rw-r--r--   0 tim       (1001) tim       (1001)      724 2023-11-21 12:46:54.000000 gigalixir-1.9.1/gigalixir.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1001) tim       (1001)     1019 2023-11-21 12:46:54.000000 gigalixir-1.9.1/gigalixir.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)        1 2023-11-21 12:46:54.000000 gigalixir-1.9.1/gigalixir.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       44 2023-11-21 12:46:54.000000 gigalixir-1.9.1/gigalixir.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)      197 2023-11-21 12:46:54.000000 gigalixir-1.9.1/gigalixir.egg-info/requires.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       10 2023-11-21 12:46:54.000000 gigalixir-1.9.1/gigalixir.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-11-21 12:46:54.573454 gigalixir-1.9.1/setup.cfg
--rw-rw-r--   0 tim       (1001) tim       (1001)      980 2023-11-21 12:43:53.000000 gigalixir-1.9.1/setup.py
-drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-11-21 12:46:54.573454 gigalixir-1.9.1/test/
--rw-rw-r--   0 tim       (1001) tim       (1001)    34868 2023-10-14 03:38:21.000000 gigalixir-1.9.1/test/test_gigalixir.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-12-07 03:14:03.801717 gigalixir-1.9.3/
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1081 2023-10-01 19:00:59.000000 gigalixir-1.9.3/LICENSE
+-rw-r--r--   0 tim       (1001) tim       (1001)      759 2023-12-07 03:14:03.801717 gigalixir-1.9.3/PKG-INFO
+-rw-rw-r--   0 tim       (1001) tim       (1001)      420 2023-10-01 19:00:59.000000 gigalixir-1.9.3/README.md
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-12-07 03:14:03.801717 gigalixir-1.9.3/gigalixir/
+-rw-rw-r--   0 tim       (1001) tim       (1001)    40529 2023-10-14 03:38:21.000000 gigalixir-1.9.3/gigalixir/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      229 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/api_exception.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      858 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/api_key.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)    10764 2023-10-14 03:38:21.000000 gigalixir-1.9.3/gigalixir/app.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      538 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/app_activity.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      391 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/auth.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1560 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/canary.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1966 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/config.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     5314 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/database.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1633 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/domain.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      555 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/free_database.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      601 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/git.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      446 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/invoice.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1262 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/log_drain.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     2653 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/mfa.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     3084 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/netrc.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     7263 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/observer.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-12-07 03:14:03.801717 gigalixir-1.9.3/gigalixir/openers/
+-rw-rw-r--   0 tim       (1001) tim       (1001)        0 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/openers/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      207 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/openers/darwin.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      214 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/openers/linux.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      210 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/openers/windows.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1172 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/payment_method.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1274 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/permission.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      347 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/presenter.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      538 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/release.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-12-07 03:14:03.801717 gigalixir-1.9.3/gigalixir/routers/
+-rw-rw-r--   0 tim       (1001) tim       (1001)        0 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/routers/__init__.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1551 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/routers/darwin.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      902 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/routers/linux.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      618 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/routers/windows.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1490 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/shell.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1234 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/ssh_key.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)      801 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/usage.py
+-rw-rw-r--   0 tim       (1001) tim       (1001)     7549 2023-10-01 19:00:59.000000 gigalixir-1.9.3/gigalixir/user.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-12-07 03:14:03.801717 gigalixir-1.9.3/gigalixir.egg-info/
+-rw-r--r--   0 tim       (1001) tim       (1001)      759 2023-12-07 03:14:03.000000 gigalixir-1.9.3/gigalixir.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1019 2023-12-07 03:14:03.000000 gigalixir-1.9.3/gigalixir.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)        1 2023-12-07 03:14:03.000000 gigalixir-1.9.3/gigalixir.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       44 2023-12-07 03:14:03.000000 gigalixir-1.9.3/gigalixir.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)      214 2023-12-07 03:14:03.000000 gigalixir-1.9.3/gigalixir.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       10 2023-12-07 03:14:03.000000 gigalixir-1.9.3/gigalixir.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1001) tim       (1001)       63 2023-12-07 03:14:03.801717 gigalixir-1.9.3/setup.cfg
+-rw-rw-r--   0 tim       (1001) tim       (1001)     1011 2023-12-07 03:12:52.000000 gigalixir-1.9.3/setup.py
+drwxrwxr-x   0 tim       (1001) tim       (1001)        0 2023-12-07 03:14:03.801717 gigalixir-1.9.3/test/
+-rw-rw-r--   0 tim       (1001) tim       (1001)    34868 2023-10-14 03:38:21.000000 gigalixir-1.9.3/test/test_gigalixir.py
```

### Comparing `gigalixir-1.9.1/LICENSE` & `gigalixir-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/PKG-INFO` & `gigalixir-1.9.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gigalixir
-Version: 1.9.1
+Version: 1.9.3
 Home-page: https://github.com/gigalixir/gigalixir-cli
-Author: Tim Day
+Author: Tim Knight
 Author-email: tim@gigalixir.com
 License-File: LICENSE
 Requires-Dist: click>=8.1
-Requires-Dist: requests>=2.28
-Requires-Dist: stripe>=4.1
-Requires-Dist: rollbar>=0.16
+Requires-Dist: cryptography>=38.0
 Requires-Dist: pygments>=2.13
-Requires-Dist: qrcode>=7.3
 Requires-Dist: pyOpenSSL>=22.1
-Requires-Dist: cryptography>=38.0
+Requires-Dist: qrcode>=7.3
+Requires-Dist: requests>=2.28
+Requires-Dist: rollbar>=0.16
+Requires-Dist: setuptools>=69.0
 Requires-Dist: six>=1.16
+Requires-Dist: stripe>=4.1
 Provides-Extra: dev
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: sphinx-tabs; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: HTTPretty; extra == "test"
```

### Comparing `gigalixir-1.9.1/gigalixir/__init__.py` & `gigalixir-1.9.3/gigalixir/__init__.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/api_key.py` & `gigalixir-1.9.3/gigalixir/api_key.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/app.py` & `gigalixir-1.9.3/gigalixir/app.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/app_activity.py` & `gigalixir-1.9.3/gigalixir/app_activity.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/canary.py` & `gigalixir-1.9.3/gigalixir/canary.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/config.py` & `gigalixir-1.9.3/gigalixir/config.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/database.py` & `gigalixir-1.9.3/gigalixir/database.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/domain.py` & `gigalixir-1.9.3/gigalixir/domain.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/free_database.py` & `gigalixir-1.9.3/gigalixir/free_database.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/git.py` & `gigalixir-1.9.3/gigalixir/git.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/log_drain.py` & `gigalixir-1.9.3/gigalixir/log_drain.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/mfa.py` & `gigalixir-1.9.3/gigalixir/mfa.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/netrc.py` & `gigalixir-1.9.3/gigalixir/netrc.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/observer.py` & `gigalixir-1.9.3/gigalixir/observer.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/payment_method.py` & `gigalixir-1.9.3/gigalixir/payment_method.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/permission.py` & `gigalixir-1.9.3/gigalixir/permission.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/release.py` & `gigalixir-1.9.3/gigalixir/release.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/routers/darwin.py` & `gigalixir-1.9.3/gigalixir/routers/darwin.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/routers/linux.py` & `gigalixir-1.9.3/gigalixir/routers/linux.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/routers/windows.py` & `gigalixir-1.9.3/gigalixir/routers/windows.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/shell.py` & `gigalixir-1.9.3/gigalixir/shell.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/ssh_key.py` & `gigalixir-1.9.3/gigalixir/ssh_key.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/usage.py` & `gigalixir-1.9.3/gigalixir/usage.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir/user.py` & `gigalixir-1.9.3/gigalixir/user.py`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/gigalixir.egg-info/PKG-INFO` & `gigalixir-1.9.3/gigalixir.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gigalixir
-Version: 1.9.1
+Version: 1.9.3
 Home-page: https://github.com/gigalixir/gigalixir-cli
-Author: Tim Day
+Author: Tim Knight
 Author-email: tim@gigalixir.com
 License-File: LICENSE
 Requires-Dist: click>=8.1
-Requires-Dist: requests>=2.28
-Requires-Dist: stripe>=4.1
-Requires-Dist: rollbar>=0.16
+Requires-Dist: cryptography>=38.0
 Requires-Dist: pygments>=2.13
-Requires-Dist: qrcode>=7.3
 Requires-Dist: pyOpenSSL>=22.1
-Requires-Dist: cryptography>=38.0
+Requires-Dist: qrcode>=7.3
+Requires-Dist: requests>=2.28
+Requires-Dist: rollbar>=0.16
+Requires-Dist: setuptools>=69.0
 Requires-Dist: six>=1.16
+Requires-Dist: stripe>=4.1
 Provides-Extra: dev
 Requires-Dist: Sphinx; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: sphinx-tabs; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: HTTPretty; extra == "test"
```

### Comparing `gigalixir-1.9.1/gigalixir.egg-info/SOURCES.txt` & `gigalixir-1.9.3/gigalixir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gigalixir-1.9.1/setup.py` & `gigalixir-1.9.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gigalixir',
     url='https://github.com/gigalixir/gigalixir-cli',
-    author='Tim Day',
+    author='Tim Knight',
     author_email='tim@gigalixir.com',
-    version='1.9.1',
+    version='1.9.3',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'click>=8.1',
-        'requests>=2.28',
-        'stripe>=4.1',
-        'rollbar>=0.16',
+        'cryptography>=38.0',
         'pygments>=2.13',
-        'qrcode>=7.3',
         'pyOpenSSL>=22.1',
-        'cryptography>=38.0',
+        'qrcode>=7.3',
+        'requests>=2.28',
+        'rollbar>=0.16',
+        'setuptools>=69.0',
         'six>=1.16',
+        'stripe>=4.1',
     ],
     entry_points='''
         [console_scripts]
         gigalixir=gigalixir:cli
     ''',
     setup_requires=[
         'pytest-runner',
```

### Comparing `gigalixir-1.9.1/test/test_gigalixir.py` & `gigalixir-1.9.3/test/test_gigalixir.py`

 * *Files identical despite different names*

