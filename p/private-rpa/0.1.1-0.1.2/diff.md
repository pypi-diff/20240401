# Comparing `tmp/private_rpa-0.1.1.tar.gz` & `tmp/private_rpa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "private_rpa-0.1.1.tar", last modified: Mon Apr  1 08:50:43 2024, max compression
+gzip compressed data, was "private_rpa-0.1.2.tar", last modified: Mon Apr  1 14:51:49 2024, max compression
```

## Comparing `private_rpa-0.1.1.tar` & `private_rpa-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.750996 private_rpa-0.1.1/
--rw-rw-rw-   0        0        0      163 2024-04-01 08:50:43.746991 private_rpa-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-01 07:55:30.000000 private_rpa-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.627999 private_rpa-0.1.1/private_rpa/
--rw-rw-rw-   0        0        0       61 2024-03-19 11:57:37.000000 private_rpa-0.1.1/private_rpa/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.643001 private_rpa-0.1.1/private_rpa/libraries/
--rw-rw-rw-   0        0        0       62 2024-03-19 11:57:37.000000 private_rpa-0.1.1/private_rpa/libraries/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.711018 private_rpa-0.1.1/private_rpa/libraries/cloud/
--rw-rw-rw-   0        0        0      179 2024-04-01 06:34:28.000000 private_rpa-0.1.1/private_rpa/libraries/cloud/__init__.py
--rw-rw-rw-   0        0        0    10001 2024-04-01 06:34:28.000000 private_rpa-0.1.1/private_rpa/libraries/cloud/pre_defined_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.737996 private_rpa-0.1.1/private_rpa/libraries/common/
--rw-rw-rw-   0        0        0       80 2024-04-01 06:35:01.000000 private_rpa-0.1.1/private_rpa/libraries/common/__init__.py
--rw-rw-rw-   0        0        0    10196 2024-03-25 16:01:45.000000 private_rpa-0.1.1/private_rpa/libraries/common/common_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.746011 private_rpa-0.1.1/private_rpa/libraries/device/
--rw-rw-rw-   0        0        0       64 2024-03-25 10:29:00.000000 private_rpa-0.1.1/private_rpa/libraries/device/__init__.py
--rw-rw-rw-   0        0        0       93 2024-03-25 10:29:00.000000 private_rpa-0.1.1/private_rpa/libraries/device/execute_powershell_script.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:50:43.639013 private_rpa-0.1.1/private_rpa.egg-info/
--rw-rw-rw-   0        0        0      163 2024-04-01 08:50:43.000000 private_rpa-0.1.1/private_rpa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-04-01 08:50:43.000000 private_rpa-0.1.1/private_rpa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 08:50:43.000000 private_rpa-0.1.1/private_rpa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 08:50:43.000000 private_rpa-0.1.1/private_rpa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 08:50:43.751995 private_rpa-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      312 2024-04-01 08:50:21.000000 private_rpa-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.370083 private_rpa-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2024-04-01 14:47:11.000000 private_rpa-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      204 2024-04-01 14:51:49.369008 private_rpa-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-01 07:55:30.000000 private_rpa-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.321001 private_rpa-0.1.2/private_rpa/
+-rw-rw-rw-   0        0        0       61 2024-03-19 11:57:37.000000 private_rpa-0.1.2/private_rpa/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.343025 private_rpa-0.1.2/private_rpa/libraries/
+-rw-rw-rw-   0        0        0       62 2024-03-19 11:57:37.000000 private_rpa-0.1.2/private_rpa/libraries/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.355013 private_rpa-0.1.2/private_rpa/libraries/cloud/
+-rw-rw-rw-   0        0        0      179 2024-04-01 06:34:28.000000 private_rpa-0.1.2/private_rpa/libraries/cloud/__init__.py
+-rw-rw-rw-   0        0        0    10001 2024-04-01 06:34:28.000000 private_rpa-0.1.2/private_rpa/libraries/cloud/pre_defined_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.361006 private_rpa-0.1.2/private_rpa/libraries/common/
+-rw-rw-rw-   0        0        0       80 2024-04-01 06:35:01.000000 private_rpa-0.1.2/private_rpa/libraries/common/__init__.py
+-rw-rw-rw-   0        0        0    10196 2024-03-25 16:01:45.000000 private_rpa-0.1.2/private_rpa/libraries/common/common_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.365999 private_rpa-0.1.2/private_rpa/libraries/device/
+-rw-rw-rw-   0        0        0       64 2024-03-25 10:29:00.000000 private_rpa-0.1.2/private_rpa/libraries/device/__init__.py
+-rw-rw-rw-   0        0        0       93 2024-03-25 10:29:00.000000 private_rpa-0.1.2/private_rpa/libraries/device/execute_powershell_script.py
+drwxrwxrwx   0        0        0        0 2024-04-01 14:51:49.339014 private_rpa-0.1.2/private_rpa.egg-info/
+-rw-rw-rw-   0        0        0      204 2024-04-01 14:51:49.000000 private_rpa-0.1.2/private_rpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2024-04-01 14:51:49.000000 private_rpa-0.1.2/private_rpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 14:51:49.000000 private_rpa-0.1.2/private_rpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-01 14:51:49.000000 private_rpa-0.1.2/private_rpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 14:51:49.370999 private_rpa-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      330 2024-04-01 14:51:30.000000 private_rpa-0.1.2/setup.py
```

### Comparing `private_rpa-0.1.1/private_rpa/libraries/cloud/pre_defined_functions.py` & `private_rpa-0.1.2/private_rpa/libraries/cloud/pre_defined_functions.py`

 * *Files identical despite different names*

### Comparing `private_rpa-0.1.1/private_rpa/libraries/common/common_functions.py` & `private_rpa-0.1.2/private_rpa/libraries/common/common_functions.py`

 * *Files identical despite different names*

