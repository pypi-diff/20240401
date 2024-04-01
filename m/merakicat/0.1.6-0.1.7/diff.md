# Comparing `tmp/merakicat-0.1.6.tar.gz` & `tmp/merakicat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.1.6.tar", last modified: Tue Mar 26 22:12:28 2024, max compression
+gzip compressed data, was "merakicat-0.1.7.tar", last modified: Mon Apr  1 14:19:41 2024, max compression
```

## Comparing `merakicat-0.1.6.tar` & `merakicat-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.080020 merakicat-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.072020 merakicat-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.072020 merakicat-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-26 22:12:21.000000 merakicat-0.1.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-26 22:12:21.000000 merakicat-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-26 22:12:21.000000 merakicat-0.1.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-26 22:12:21.000000 merakicat-0.1.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-26 22:12:21.000000 merakicat-0.1.6/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-26 22:12:21.000000 merakicat-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-26 22:12:21.000000 merakicat-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-26 22:12:21.000000 merakicat-0.1.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-03-26 22:12:28.080020 merakicat-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-03-26 22:12:21.000000 merakicat-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.072020 merakicat-0.1.6/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-26 22:12:21.000000 merakicat-0.1.6/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.076020 merakicat-0.1.6/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-03-26 22:12:21.000000 merakicat-0.1.6/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 22:12:21.000000 merakicat-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-26 22:12:21.000000 merakicat-0.1.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:12:28.080020 merakicat-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-26 22:12:21.000000 merakicat-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.072020 merakicat-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.080020 merakicat-0.1.6/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.080020 merakicat-0.1.6/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_claim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1216 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_file_exists.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54782 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9240 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2217 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34004 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/mc_user_sample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77811 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 22:12:21.000000 merakicat-0.1.6/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:12:28.080020 merakicat-0.1.6/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-03-26 22:12:28.000000 merakicat-0.1.6/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-26 22:12:28.000000 merakicat-0.1.6/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:12:28.000000 merakicat-0.1.6/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:12:27.000000 merakicat-0.1.6/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 22:12:28.000000 merakicat-0.1.6/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 22:12:28.000000 merakicat-0.1.6/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-26 22:12:21.000000 merakicat-0.1.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.422526 merakicat-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 14:19:33.000000 merakicat-0.1.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-01 14:19:33.000000 merakicat-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 14:19:33.000000 merakicat-0.1.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-01 14:19:33.000000 merakicat-0.1.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-01 14:19:33.000000 merakicat-0.1.7/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 14:19:33.000000 merakicat-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 14:19:33.000000 merakicat-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-01 14:19:33.000000 merakicat-0.1.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-01 14:19:41.422526 merakicat-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-01 14:19:33.000000 merakicat-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 14:19:33.000000 merakicat-0.1.7/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.414526 merakicat-0.1.7/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-01 14:19:33.000000 merakicat-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-01 14:19:33.000000 merakicat-0.1.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:19:41.422526 merakicat-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-01 14:19:33.000000 merakicat-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.418526 merakicat-0.1.7/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.418526 merakicat-0.1.7/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_claim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54947 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8798 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34233 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_user_sample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84228 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.418526 merakicat-0.1.7/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-01 14:19:33.000000 merakicat-0.1.7/tox.ini
```

### Comparing `merakicat-0.1.6/.gitignore` & `merakicat-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/CONTRIBUTING.rst` & `merakicat-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/HISTORY.md` & `merakicat-0.1.7/HISTORY.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # History
 
+## 0.1.7 (04-01-2024)
+
+  - Added the ability to Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features.
+  - Included "with timing" and "with details" options on check drag-n-drop.
+  - Renamed some called functions in external modules.
+
 ## 0.1.6 (03-26-2024)
 
   - Updated encyclopedia.
-  - Migrated batch helper code.
+  - Migrated batch helper code for cleaner installation.
 
 ## 0.1.5 (03-23-2024)
 
   - Supports NM ports.
   - Merged nm-specifics into the encyclopedia.
 
 ## 0.1.4 (03-21-2024)
```

### Comparing `merakicat-0.1.6/LICENSE` & `merakicat-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/Makefile` & `merakicat-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/PKG-INFO` & `merakicat-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.1.6
+Version: 0.1.7
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -230,18 +230,24 @@
 
 The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
 
 
 
 # History
 
+## 0.1.7 (04-01-2024)
+
+  - Added the ability to Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features.
+  - Included "with timing" and "with details" options on check drag-n-drop.
+  - Renamed some called functions in external modules.
+
 ## 0.1.6 (03-26-2024)
 
   - Updated encyclopedia.
-  - Migrated batch helper code.
+  - Migrated batch helper code for cleaner installation.
 
 ## 0.1.5 (03-23-2024)
 
   - Supports NM ports.
   - Merged nm-specifics into the encyclopedia.
 
 ## 0.1.4 (03-21-2024)
```

### Comparing `merakicat-0.1.6/README.md` & `merakicat-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/botcongrats.jpg` & `merakicat-0.1.7/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/cisco_meraki.png` & `merakicat-0.1.7/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/createbot.jpg` & `merakicat-0.1.7/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/mc_quick.gif` & `merakicat-0.1.7/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/merakicat.png` & `merakicat-0.1.7/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/newapp.jpg` & `merakicat-0.1.7/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/images/newbot.jpg` & `merakicat-0.1.7/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/setup.py` & `merakicat-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/batch_helper/__init__.py` & `merakicat-0.1.7/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/batch_helper/config.py` & `merakicat-0.1.7/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.1.7/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/mc_cfg_check.py` & `merakicat-0.1.7/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/mc_claim.py` & `merakicat-0.1.7/src/merakicat/mc_claim.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/mc_file_exists.py` & `merakicat-0.1.7/src/merakicat/mc_file_exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from mc_user_info import DEBUG, DEBUG_FILE
 
 
-def File_exists(filespec):
+def FileExists(filespec):
     """
     Checks to see if a filespec can be found, and is a file.
     :param filespec: The incoming user text from Teams or the command line
     :return :The filespec (possibly modified) and True or False
     """
     debug = DEBUG or DEBUG_FILE
```

### Comparing `merakicat-0.1.6/src/merakicat/mc_pedia.py` & `merakicat-0.1.7/src/merakicat/mc_pedia.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
 #####################################################################################
 '''
 
 
 mc_pedia = {
 
-    'version': "v0.1.2",
-    'dated': "03/26/2024",
+    'version': "v0.1.5",
+    'dated': "03/28/2024",
 
     'switch': {
         
         'switch_name': {
             'name': "Hostname",
             'support':"✓",
             'translatable':"✓",
@@ -291,23 +291,23 @@
                 'skip': True
             },
             'iosxe': "aaa = parse.find_objects('^aaa')\n",
             'url':"https://documentation.meraki.com/General_Administration/Managing_Dashboard_Access/Managing_Dashboard_Administrators_and_Permissions",
             'note':"Built in Meraki dashboard"
         },
         
-        '802.1x':{
+        'dot1x':{
             'name': "802.1x",
             'support': "✓",
             'translatable':"",
             'regex': '^aaa authentication dot1x',
             'meraki': {
                 'skip': True
             },
-            'iosxe': "802.1x = parse.find_objects('^aaa authentication dot1x')\n",
+            'iosxe': "dot1x = parse.find_objects('^aaa authentication dot1x')\n",
             'url':"https://documentation.meraki.com/MS/Access_Control/MS_Switch_Access_Policies_(802.1X)",
             'note':"Network-wide"
         },
         
         'netflow':{
             'name': "NetFlow",
             'support':"✓",
@@ -405,23 +405,23 @@
                 'skip': True
             },
             'iosxe': "vlan = parse.find_objects('^vlan')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Configured by default"
         },
         
-        'vpms':{
-            'name': "VPMS",
+        'vmps':{
+            'name': "VMPS",
             'support':"",
             'translatable':"",
             'regex': '^vpms',
             'meraki': {
                 'skip': True
             },
-            'iosxe': "vpms = parse.find_objects('^vpms')\n",
+            'iosxe': "vmps = parse.find_objects('^vmps')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported as it is dated technology"
         },
         
         'uplinkfast':{
             'name': "STP Uplinkfast",
             'support':"",
@@ -1566,35 +1566,38 @@
             blurb+="Supported & Translatable Items\n"
         else:
             blurb+="       Supported Items\n"
     elif "translatable" in index_args:
         blurb+="     Translatable Items\n"
     print(blurb+"==============================\n")
     for key,value in mc_pedia.items():
-        print(key+":\n")
-        for k,v in value.items():
-            skip = 0
-            if "translatable" in index_args:
-                if "translatable" not in v:
-                    skip = 1
-                elif not v['translatable'] == "✓":
-                    skip = 1
-            if "support" in index_args:
-                if "support" not in v:
-                    skip = 1
-                elif not v['support'] == "✓":
-                    skip = 1
-            if skip == 0:
-                if "name" in v:
-                    print(" - "+v['name']+"\n")
-                else:
-                    print(" - "+k+" (for Meraki)\n")
+        if key in ["version","dated"]:
+            print(key+": "+value+"\n")
+        else:
+            print(key+":\n")
+            for k,v in value.items():
+                skip = 0
+                if "translatable" in index_args:
+                    if "translatable" not in v:
+                        skip = 1
+                    elif not v['translatable'] == "✓":
+                        skip = 1
+                if "support" in index_args:
+                    if "support" not in v:
+                        skip = 1
+                    elif not v['support'] == "✓":
+                        skip = 1
+                if skip == 0:
+                    if "name" in v:
+                        print(" - "+v['name']+"\n")
+                    else:
+                        print(" - "+k+" (for Meraki)\n")
     if len(index_args) == 0:
         print("\n\nTo print the index based on either supported and translatable items or both, enter")
-        print("    python mc_pedia [support] [translatable]")
+        print("    python mc_pedia.py [support] [translatable]")
 
 if __name__ == '__main__':
     index_args = list()
     if len(sys.argv) > 1:
         args = sys.argv
         del args[0]
         for arg in args:
```

### Comparing `merakicat-0.1.6/src/merakicat/mc_ping.py` & `merakicat-0.1.7/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/mc_register.py` & `merakicat-0.1.7/src/merakicat/mc_register.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from netmiko import ConnectHandler
 from mc_user_info import DEBUG, DEBUG_REGISTER
+from mc_get_nms import GetNmList
 import re
 
 
 def Register(host_id, ios_username, ios_password, ios_port, ios_secret):
     """
     This function will check a Catalyst IOSXE switch for compatibility with
     Meraki management prior to registering the switch (or stack) to Dashboard.
@@ -49,30 +50,16 @@
     switch_name = switch_name[:len(switch_name) - 1]
 
     # Grab the switches in the stack
     r = net_connect.send_command('show switch')
     qty_switches = len(r.split("\n"))-8
 
     # Grab the uplink module in each switch
-    x = 1
-    while x <= qty_switches:
-        r = net_connect.send_command('show inventory "Switch ' +
-                                     str(x) + ' FRU Uplink Module 1"')
-        if debug:
-            print(f"For switch {x}, r = {r}")
-        if debug:
-            print(f"For switch {x}, len(r) = {len(r)}")
-        if not r[0] == "%":
-            nm_list.append(r.split("\n")[1].split()[1])
-        else:
-            nm_list.append("")
-        x += 1
-    if debug:
-        print(f"For the {qty_switches} switches in the stack, " +
-              f"the NM modules are {nm_list}")
+    nm_list = GetNmList(host_id, ios_username,
+                          ios_password, ios_port, ios_secret)
 
     # Check the version of IOSXE running on the switch
     r = net_connect.send_command('show version').split("\n")
     version = r[0].split("Version")[1].strip()[:8]
     if debug:
         print(f"In Register, version = {version}")
     v = list(map(int, version.split('.')))
```

### Comparing `merakicat-0.1.6/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.1.7/src/merakicat/mc_splitcheck_serials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from collections import Counter
 from mc_user_info import *
 
 
-def Split_check_serials(user_text,search_type):
+def SplitCheckSerials(user_text,search_type):
     """
     This function will accept of user's input or command line parms and find the serial
     numbers and split them out to a list to return.
     :param user_text: The incoming user text from Teams or the command line
     :param search_type: 'Claim' or 'Translate' based on the command line type to parse
     :return: A list of Meraki serial numbers and a string if there was an issue
     """
```

### Comparing `merakicat-0.1.6/src/merakicat/mc_translate.py` & `merakicat-0.1.7/src/merakicat/mc_translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             switch_dict[key] = ""
         if debug:
             print(f"switch_dict = {switch_dict}")
         # Parsing the Cisco Catalyst configuration
         if debug:
             print("-------- Reading <"+config_file+"> Configuration --------")
         parse = CiscoConfParse(config_file, syntax='ios', factory=True)
-
         # Try out our mc_pedia for the switch name
         for key, val in mc_pedia['switch'].items():
             newvals = {}
             exec(val.get('iosxe'), locals(), newvals)
             switch_dict[key] = newvals[key]
             if debug:
                 print(f"switch_dict['{key}'] = {switch_dict[key]}")
@@ -107,14 +106,17 @@
                         r'^interface\s\S+?thernet+(\d)')
                     if Switch_module == "":
                         Switch_module = intf_obj.re_match_typed(
                             r'^interface\s\S+?GigE+(\d)')
                 port, sub_module = check(intf_name)
                 if sub_module == "1":
                     intf_include = False
+                    if debug:
+                        print(f"Switch_module = {Switch_module}")
+                        print(f"nm_list = {nm_list}")
                     if not nm_list[int(Switch_module)-1] == "":
                         if nm_dict[
                               nm_list[int(Switch_module)-1]]['supported']:
                             for regex in nm_dict[
                               nm_list[int(Switch_module)-1]]['ports']:
                                 if re.match(regex,intf_name):
                                     # Make sure it has some settings,
@@ -295,15 +297,15 @@
     Interfaces, Others, port_dict, switch_name = read_Cisco_SW()
     if debug:
         print(f"\nInterfaces = {Interfaces}")
         print(f"\nOthers = {Others}")
     return Interfaces, Others, port_dict, switch_dict
 
 
-def Meraki_config(dashboard, organization_id, switch_path, sw_list, port_dict,
+def MerakiConfig(dashboard, organization_id, switch_path, sw_list, port_dict,
                   Intf_list, Other_list, switch_dict, nm_list):
     """
     This parent function will convert Catalyst switch config features to
     Meraki features and send them to Dashboard to program Meraki switches.
     :param dashboard: Active Meraki dashboard API session to use
     :param organization_id: Meraki Org ID used in batch configuration
     :param sw_list: List of Meraki switch serial numbers to configure
@@ -352,14 +354,16 @@
         # Configure the switch_name in the Dashboard
         if debug:
             print(f"switch_dict = {switch_dict}")
         for key, val in mc_pedia['switch'].items():
             if (val['translatable'] == "✓" and
                 val['meraki']['skip'] == "post_process") or \
                  val['meraki']['skip'] == "post_ports":
+                if debug:
+                    print(f"key = {key}, val = {val}")
                 if val['meraki']['skip'] == "post_ports":
                     post_ports_list.append([key, True])
                 newvals = {}
                 exec(val['meraki'].get('post_process'), locals(), newvals)
                 if debug:
                     print(f"newvals = {newvals}")
                 return_vals = newvals['return_vals']
```

### Comparing `merakicat-0.1.6/src/merakicat/mc_user_sample.py` & `merakicat-0.1.7/src/merakicat/mc_user_sample.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.6/src/merakicat/merakicat.py` & `merakicat-0.1.7/src/merakicat/merakicat.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 from netmiko import ConnectHandler
 from docx2pdf import convert
 from docx.enum.text import WD_ALIGN_PARAGRAPH
 from docx.shared import Inches
 from docx.oxml import OxmlElement
 from docx.oxml.ns import qn
 from mc_cfg_check import CheckFeatures
-from mc_translate import Evaluate, Meraki_config  # ,Meraki_config_up
+from mc_translate import Evaluate, MerakiConfig  # ,MerakiConfig_up
 from mc_claim import Claim
 from mc_register import Register
-from mc_splitcheck_serials import Split_check_serials
+from mc_get_nms import GetNmList
+from mc_splitcheck_serials import SplitCheckSerials
 from mc_ping import Ping
-from mc_file_exists import File_exists
+from mc_file_exists import FileExists
+from mc_get_config import GetConfig
 from mc_user_info import DEBUG, DEBUG_MAIN, PDF, NGROK_AUTHTOKEN
 from mc_user_info import IOS_USERNAME, IOS_PASSWORD, IOS_SECRET, IOS_PORT
 from mc_user_info import TEAMS_BOT_TOKEN, TEAMS_BOT_EMAIL
 from mc_user_info import TEAMS_BOT_APP_NAME, TEAMS_EMAILS, MERAKI_API_KEY
 from collections import defaultdict
 from functools import reduce
 from itertools import islice
@@ -286,50 +288,95 @@
     command = user_text.split()[0].lower()
 
     if BOT:
         # If first word from the user's input was Bot's first name, remove it
         if user_text.split()[0] == bot_fname:
             user_text = user_text.split(bot_fname + ' ', 1)[1]
 
-        # If the command is 'check' and the user attached any config files to
-        # the bot message, we will try to use them
-        if command == 'check' and (user_files is not None):
-            x = 0
-            while x < len(user_files) - 1:
-                config_file = save(user_files[x])
-                response.markdown = check_switch(
-                    incoming_msg,
-                    config=config_file)
-                create_message(user_roomId, response.markdown)
-                x += 1
-
     if debug:
         print(f"command = {command}")
 
-    # If the user asked for a report, we will try to give it to them
-    report = False
-    regex = r'\swith\sreports|\swith\sreports|\swith\sreporting'
-    if re.search(regex, user_text, re.IGNORECASE) is not None:
-        user_text = re.sub(regex, '', user_text, re.IGNORECASE)
-        report = True
-
     # If the user asked for timing, we will try to give it to them
     times = False
     regex = r'\swith\stimings|\swith\stiming|\swith\stime|\swith\stimes'
     if re.search(regex, user_text, re.IGNORECASE) is not None:
         user_text = re.sub(regex, '', user_text, re.IGNORECASE)
         times = True
 
     # If the user asked for detailed reports, we will try to give it to them
     detailed = False
     regex = r'\swith\sdetails|\swith\sdetail'
     if re.search(regex, user_text, re.IGNORECASE) is not None:
         user_text = re.sub(regex, '', user_text, re.IGNORECASE)
         detailed = True
 
+    # If the command is 'check' and the user attached any config files to
+    # the bot message, we will try to use them
+    if user_text.lower() == 'check' and (user_files is not None):
+        x = 0
+        while x < len(user_files) - 1:
+            config_file = save(user_files[x])
+            response.markdown = check_switch(
+                incoming_msg,
+                config=config_file)
+            create_message(user_roomId, response.markdown)
+            x += 1
+
+    # If the user asked for a report, we will try to give it to them
+    if user_text.lower().startswith('check network '):
+        # Now let's see if they specified target models...
+        targets = ['C9300']
+        regex = re.compile(r"\s*target\s *|\s*targets\s *", flags=re.I)
+        if len(regex.split(user_text)) > 1:
+            if not regex.split(user_text)[1] == "":
+                maybe_targets = regex.split(user_text)[1]
+                user_text = regex.split(user_text)[0].strip()
+                if not re.search(',', maybe_targets, re.IGNORECASE) == None:
+                    maybe_targets = maybe_targets.replace(" ", "")
+                if debug:
+                    print(f"maybe_targets = {maybe_targets}")
+                if not len(maybe_targets)==0:
+                    targets = re.split(';|,|\s',maybe_targets)
+                    print(f"regex.split(user_text)[0] = {regex.split(user_text)[0]}")
+        if debug:
+            print(f"targets = {targets}")
+        # Did they enter a network name after "network"?
+        dest_net = meraki_net
+        regex = re.compile(r"\s*network\s *", flags=re.I)
+        if not regex.split(user_text)[1] == "":
+            # They did, so register it!
+            dest_net_name = regex.split(user_text)[1]
+            dest_net = ""
+            test = [d['id'] for d in meraki_networks
+                    if d['name'] == dest_net_name]
+            if not len(test) == 0:
+                dest_net = test[0]
+                meraki_net_name = dest_net_name
+            if dest_net == "":
+                r = "I'm sorry, but {} is ".format(dest_net_name)
+                r += "not in your list of Meraki networks."
+                response.markdown = r
+            else:
+                if debug:
+                    print(f"dest_net = {dest_net}")
+        if dest_net == "":
+            r = "You need to enter a Meraki network to register into."
+            response.markdown = r
+        else:
+            response.markdown = check_network(incoming_msg,
+                                              dest_net,
+                                              targets=targets)
+
+    # If the user asked for a report, we will try to give it to them
+    report = False
+    regex = r'\swith\sreports|\swith\sreports|\swith\sreporting'
+    if re.search(regex, user_text, re.IGNORECASE) is not None:
+        user_text = re.sub(regex, '', user_text, re.IGNORECASE)
+        report = True
+
     serials = list()
 
     # Test if it is equivalent to a command.
     match command:
         case "demo":
             # If the only thing the user typed was "demo report""...
             if user_text.lower() == 'demo report':
@@ -389,20 +436,20 @@
                         else:
                             if debug:
                                 print(f"dest_net = {dest_net}")
                 if dest_net == "":
                     r = "You need to enter a Meraki network to register into."
                     response.markdown = r
                 host = host_id
-                # Did they type "translate host <something>" ?
+                # Did they type "migrate host <something>" ?
                 if re.search('host ', user_text, re.IGNORECASE):
                     if debug:
                         print("I made it to host...")
                     if not user_text.split("host ", 1)[1] == "":
-                        # They did, so translate it!
+                        # They did, so migrate it!
                         maybe_host = user_text.split("host ", 1)[1]
                         regex = re.compile(r"\s*to\s *", flags=re.I)
                         the_rest = regex.split(maybe_host)[0]
                         host = the_rest.strip()
                         if debug:
                             print(f"host = {host}")
                         if not Ping(host):
@@ -455,15 +502,15 @@
                 # after "to" ?
                 serials = meraki_serials
                 if re.search('to ', user_text, re.IGNORECASE):
                     if debug:
                         print("user_text.split('to ',1)[1] = " +
                               f"{user_text.split('to ',1)[1]}")
                     if not user_text.split("to ", 1)[1] == "":
-                        serials, r = Split_check_serials(user_text,
+                        serials, r = SplitCheckSerials(user_text,
                                                          "Translate")
                         if debug:
                             print(f"serials = {serials}")
                             print(f"r = {r}")
                             print(f"r=='' = {r==''}")
                         if not r == "":
                             response.markdown = r
@@ -471,15 +518,15 @@
                 # Did they type "translate file <something>" ?
                 if re.search('file ', user_text, re.IGNORECASE):
                     if not user_text.split("file ", 1)[1] == "":
                         # They did, so translate it!
                         maybe_file = user_text.split("file ", 1)[1].split()[0]
                         if debug:
                             print(f"maybe_file = {maybe_file}")
-                        maybe_file, exists = File_exists(maybe_file)
+                        maybe_file, exists = FileExists(maybe_file)
                         if not exists:
                             r = "I'm sorry, but I could not find that file."
                             response.markdown = r
                         else:
                             r = translate_switch(incoming_msg,
                                                  config=maybe_file,
                                                  serials=serials)
@@ -544,15 +591,15 @@
                 r = "Syntax is **check (host <_fqdn or ip address_> | "
                 r += "file <_filespec_>)**"
                 response.markdown = r
             elif user_text.lower().startswith('check'):
                 if re.search('file', user_text, re.IGNORECASE):
                     if not user_text.split("file ", 1)[1] == "":
                         maybe_file = user_text.split("file ", 1)[1].split()[0]
-                        maybe_file, exists = File_exists(maybe_file)
+                        maybe_file, exists = FileExists(maybe_file)
                         if not exists:
                             r = "I'm sorry, but I could not find that file."
                             response.markdown = r
                         else:
                             response.markdown = check_switch(incoming_msg,
                                                              config=maybe_file)
                     else:
@@ -666,17 +713,17 @@
                             r = "I'm sorry, but {} is ".format(dest_net_name)
                             r += "not in your list of Meraki networks."
                 # Set the list of serial numbers to the global stateful list in
                 # case nothing was entered by the user
                 serials = list()
                 # Did the user enter a list of serial numbers after "Claim" ?
                 if not user_text.lower() == 'claim':
-                    maybe_serials, r = Split_check_serials(user_text, "Claim")
+                    maybe_serials, r = SplitCheckSerials(user_text, "Claim")
                     if debug:
-                        print("In case: 'claim': after Split_check_serials, " +
+                        print("In case: 'claim': after SplitCheckSerials, " +
                               f"serials = {serials}, maybe_serials = " +
                               f"{maybe_serials}, r = {r}")
                     # If we didn't get back some kind of error response,
                     # use the returned list
                     if r == "":
                         serials = maybe_serials
                     else:
@@ -767,14 +814,131 @@
     return (f_path)
 
 
 # Create functions that will be linked to bot commands to add capabilities
 # ------------------------------------------------------------------------
 
 
+def check_network(incoming_msg, dest_net, targets=['C9300']):
+    """
+    This function will get a list of all switches in a Meraki network, parse
+    it for any cloud-monitored Catalyst switches that cold be cloud-managed.
+    It then grabs their configs one by one and sends them through the
+    check_switch function to generate a report for each.
+    :param incoming_msg: The incoming message object from Teams
+    :param dest_net: The Meraki network to check
+    :return: A text or markdown based reply
+    """
+
+    # Create a Response object to later craft a reply in Markdown.
+    response = Response()
+
+    # This will be our copy of the user input to work with
+    user_roomId = incoming_msg.roomId
+
+    # Grab the list of devices for that Network
+    try:
+        devices = dashboard.networks.getNetworkDevices(dest_net)
+    except meraki.exceptions.APIError:
+        r = "We were unable to get the list of devices for that network."
+        return (r)
+    if debug:
+        print(f"devices = {switches}")
+
+    # Loop through the devices searching for cloud monitored C9300s
+    success_list = list()
+    if targets == []:
+        targets = ['C9300']
+    if debug:
+        print(f"targets = {targets}")
+    x = 0
+    while x <= len(devices) - 1:
+        if debug:
+            print(f"\ndevice = {devices[x]}")
+        if devices[x]['firmware'].startswith('ios-xe'):
+            short_mod = devices[x]['model'][:5]
+            if debug:
+                print(f"short_mod = {short_mod}")
+            if short_mod in targets:
+                # Found one...
+                sw_name = devices[x]['name']
+
+                # Grab the list of config files archived for the switch
+                try:
+                    url = f"https://api.meraki.com/api/v1/devices/{devices[x]['serial']}/switch/configs"
+                    payload = {}
+                    headers = {
+                      'X-Cisco-Meraki-API-Key': meraki_api_key
+                    }
+                    response = requests.request("GET", url, headers=headers, data=payload)
+                except:
+                    print(f"ERROR getting the config list for {sw_name}")
+                    x += 1
+                conf_list = response.json()
+                # If the Python meraki SDK ever supports this it should look
+                # like this:
+                #
+                # conf_list = dashboard.devices.getSwitchConfigs(devices[x]['serial'])
+
+                if debug:
+                    print(f"conf_list = {conf_list}")
+                    print(f"len(conf_list) = {len(conf_list)}")
+                    print(f"conf_list[0] = {conf_list[0]}")
+
+                # Assuming there are and configs in the list, we will grab a copy
+                # of the first (latest) one.
+                if len(conf_list) > 0:
+                    url += "/" + conf_list[0]['id']
+                    if debug:
+                        print(f"url = {url}")
+                    try:
+                        response = requests.request("GET", url, headers=headers, data=payload)
+                    except:
+                        print(f"ERROR getting config for {sw_name}")
+                        x += 1
+                    c = response.json()
+                    # If the Python meraki SDK ever supports this it should look
+                    # like this:
+                    #
+                    # c = dashboard.devices.getSwitchConfigs(devices[x]['serial'],conf_list[0]['id'])
+
+                    # Now that we have the config, let's save a copy
+                    dir = os.path.join(os.getcwd(), "../../files")
+                    config_file = os.path.join(dir, sw_name + ".cfg")
+                    file = open(config_file, "w")
+                    file.writelines(c['config'])
+                    file.close()
+                    success_list.append(sw_name)
+
+                    # Run the Check report on that config file
+                    response.markdown = check_switch(
+                                                     incoming_msg,
+                                                     config=config_file)
+                    if BOT:
+                        create_message(user_roomId, response.markdown)
+                    else:
+                        print("\n\nFor switch "+sw_name+":"+response.markdown)
+        x += 1
+
+    # Prep the overall return status and pass it back
+    if len(success_list) > 0:
+        r = "We successfully downloaded the config file"
+        if len(success_list) == 1:
+            r += " for " + success_list[0] + "."
+        else:
+            r += "s for " + ','.join(success_list) + "."
+    else:
+        r = "We were unsuccessful locating cloud monitored switch model"
+        if len (targets) == 1:
+            r += ": " + ",".join(targets) + "."
+        else:
+            r += "s: " + ",".join(targets) + "."
+    return (r)
+
+
 def check_switch(incoming_msg, config="", host="", demo=False):
     """
     This function will check a Catalyst switch config for feature mapping to
     Meraki.
     :param incoming_msg: The incoming message object from Teams
     :param config: The incoming config filespec
     :param host: The incoming hostname or IP address
@@ -795,39 +959,20 @@
             if host == "":
                 return ("You need to enter either a host or a filename.")
 
             # We were passed a hostname or IP address...
             else:
                 host_id = host
 
-            # SSH to the switch with netmiko, read the config, grab the
-            # hostname, write the config out to a file using the hostname
-            # as part of the filespec
-            session_info = {
-                'device_type': 'cisco_xe',
-                'host': host_id,
-                'username': ios_username,
-                'password': ios_password,
-                'port': ios_port,          # optional, defaults to 22
-                'secret': ios_secret,      # optional, defaults to ''
-            }
-            net_connect = ConnectHandler(**session_info)
-            switch_name = net_connect.find_prompt()
-            net_connect.enable()
-            switch_name = net_connect.find_prompt()
-            switch_name = switch_name[:len(switch_name) - 1]
-            net_connect.send_command('term len 0')
-            config = net_connect.send_command('show running-config')
-            net_connect.send_command('term len 24')
-            net_connect.disconnect()
-            dir = os.path.join(os.getcwd(), "../../files")
-            file = open(os.path.join(dir, switch_name + ".cfg"), "w")
-            file.writelines(config)
-            file.close()
-            config = os.path.join(dir, switch_name + ".cfg")
+            # Get the config file from a switch/stack
+            switch_name, config = GetConfig(host_id,
+                                            ios_username,
+                                            ios_password,
+                                            ios_port,
+                                            ios_secret)
 
         # Update the global stateful variable for later
         config_file = config
 
         # Run the function in config_checker to get the list of
         # features configured on the switch (supported and not)
         host_name, the_list = CheckFeatures(config_file)
@@ -1215,21 +1360,21 @@
                 print(f"switch = {switch}")
                 print("switch['Migration Status'] = " +
                       f"{switch['migration_status']}")
     if debug:
         print(f"After registering switches, meraki_serials = {meraki_serials}")
     # Report back on what happened
     if called == "":
+        timing = ""
         if not len(registered_switches) == 0:
             vals = reduce(lambda x, y: x + y, [list(dic.values())
                           for dic in registered_switches])
             header = registered_switches[0].keys()
             rows = [x.values() for x in registered_switches]
             thing = tabulate(rows, header)
-            timing = ""
             if times:
                 t = "\n=== That registraion took "
                 t += "%s seconds" % str(round((time.time() - start_time), 2))
                 timing = t
             if BOT:
                 payload = "```\n%s" % thing + "\n```" + timing
                 r = f"We **{status}** registered **{vals.count('Registered')}"
@@ -1391,35 +1536,36 @@
                 'username': ios_username,
                 'password': ios_password,
                 'port': ios_port,          # optional, defaults to 22
                 'secret': ios_secret,     # optional, defaults to ''
             }
             if debug:
                 print(f"session_info = {session_info}")
-            net_connect = ConnectHandler(**session_info)
-            switch_name = net_connect.find_prompt()
-            net_connect.enable()
-            switch_name = net_connect.find_prompt()
-            switch_name = switch_name[:len(switch_name) - 1]
-            net_connect.send_command('term len 0')
-            config = net_connect.send_command('show running-config')
-            net_connect.send_command('term len 24')
-            net_connect.disconnect()
-            dir = os.path.join(os.getcwd(), "../../files")
-            file = open(os.path.join(dir, switch_name+".cfg"), "w")
-            file.writelines(config)
-            file.close()
-            config = os.path.join(dir, switch_name+".cfg")
+            # Get the config file from a switch/stack
+            switch_name, config = GetConfig(host_id,
+                                            ios_username,
+                                            ios_password,
+                                            ios_port,
+                                            ios_secret)
+
+            # Grab the uplink module in each switch
+            nm_list = GetNmList(host_id, ios_username,
+                                  ios_password, ios_port, ios_secret)
     else:
         if config == "":
             config = config_file
 
     # Update the global stateful variable for later
     config_file = config
 
+    # If we don't have an nm_list, create an empty list 9 switches long
+    # which is larger than a stack so we can test for this later
+    if nm_list == []:
+        nm_list = ["","","","","","","","",""]
+
     # Evaluate the Catalyst config and break it into lists we can work with
     Intf_list, Other_list, port_dict, switch_dict = \
         Evaluate(config_file, nm_list)
 
     # Creating a list of the downlink port configurations to push to Meraki
     ToBeConfigured = {}
     z = 0
@@ -1432,26 +1578,29 @@
     # Start the meraki config migration after confirmation from the user
     #
     blurb = "Evaluated the switch config based on encyclopedia "
     blurb += mc_pedia['version'] + ", published on " + mc_pedia['dated'] + "."
     if times:
         blurb += "\n--- That took "
         blurb += "%s seconds" % str(round((time.time() - start_time), 2))
+    if len(nm_list) == 9:
+        blurb += "\n\nSKIPPING NM MODULES, because we only had a config file"
+        blurb += " to work with..."
     blurb += "\n\nPushing the translated items to the Dashboard in a large"
     blurb += " batch.\nThis will take a while, but I'll message you"
     blurb += " when I'm done..."
     if BOT:
         create_message(incoming_msg.roomId, blurb)
     else:
         print(blurb)
 
     port_cfg_start_time = time.time()
 
     configured_ports, unconfigured_ports, port_dict, \
-        meraki_urls, meraki_net = Meraki_config(dashboard,
+        meraki_urls, meraki_net = MerakiConfig(dashboard,
                                                      meraki_org,
                                                      switch_name,
                                                      meraki_serials,
                                                      port_dict,
                                                      Intf_list,
                                                      Other_list,
                                                      switch_dict,
@@ -1569,39 +1718,21 @@
         # It was in the list of the user's Meraki networks, so save it
         meraki_net = dest_net
         test_net = [d['name'] for d in meraki_networks
                     if d['id'] == meraki_net]
         if not len(test_net) == 0:
             meraki_net_name = test_net[0]
 
-    # SSH to the switch with netmiko, read the config, grab the switch name,
-    # write the config out to a file using the switch name as part of the
-    # filespec
-    session_info = {
-        'device_type': 'cisco_xe',
-        'host': host_id,
-        'username': ios_username,
-        'password': ios_password,
-        'port': ios_port,          # optional, defaults to 22
-        'secret': ios_secret     # optional, defaults to ''
-    }
-    net_connect = ConnectHandler(**session_info)
-    switch_name = net_connect.find_prompt()
-    net_connect.enable()
-    switch_name = net_connect.find_prompt()
-    switch_name = switch_name[:len(switch_name) - 1]
-    net_connect.send_command('term len 0')
-    config = net_connect.send_command('show running-config')
-    net_connect.send_command('term len 24')
-    net_connect.disconnect()
-    dir = os.path.join(os.getcwd(), "../../files")
-    file = open(os.path.join(dir, switch_name+".cfg"), "w")
-    file.writelines(config)
-    file.close()
-    config = os.path.join(dir, switch_name+".cfg")
+    # Get the config file from a switch/stack
+    switch_name, config = GetConfig(host_id,
+                                    ios_username,
+                                    ios_password,
+                                    ios_port,
+                                    ios_secret)
+
     blurb = "Logged in to " + host_id + ", grabbed a copy of the running "
     blurb += "config and saved it as " + switch_name + ".cfg."
     if times:
         blurb += "\n--- That took "
         blurb += "%s seconds" % str(round((time.time() - start_time), 2))
     if BOT:
         create_message(incoming_msg.roomId, blurb)
@@ -1677,16 +1808,15 @@
     if debug:
         print("in migrate before translate, meraki_serials = " +
               f"{meraki_serials}")
     # Translate the switch stack to the Meraki switches we just claimed
     translate_start_time = time.time()
     r = "\n\n" + translate_switch(
         incoming_msg,
-        config="",
-        host=host_id,
+        config=config_file,
         serials=meraki_serials,
         verb="migrate")
     blurb = "\nTranslated " + switch_name+".cfg to Meraki switches "
     blurb += string_serials + " based on encyclopedia " + mc_pedia['version']
     blurb += ", published on " + mc_pedia['dated'] + ".\n"
     if times:
         t = "%s seconds" % str(round((time.time() - translate_start_time), 2))
@@ -1748,20 +1878,25 @@
     bot.set_greeting(greeting)
 
     # Add new commands to the bot.
     bot_commands = list(list())
     bot_commands.extend([
         ["* **help**", "Get help."],
 
-        ["* **check _drag-and-drop files_ [with timing]**",
+        ["* **check [network _Meraki network name_] [with timing] \
+[with details]**",
+         "Check the configs of cloud monitored Catalyst switches \
+for both translatable and possible Meraki features"],
+
+        ["* **check _drag-and-drop files_ [with timing] [with details]**",
          "Check one or more Catalyst switch config files for both \
 translatable and possible Meraki features"],
 
         ["* **check [host _FQDN or IP address_ | file _filespec_] \
-[with timing]**",
+[with timing] [with details]**",
          "Check a Catalyst switch config for both translatable \
 and possible Meraki features"],
 
         ["* **register [host _FQDN or IP address_] [with timing] \
 [with details]**",
          "Register a Catalyst switch to the Meraki Dashboard"],
 
@@ -1782,19 +1917,31 @@
         ["* **demo report**",
          "Create a demo report for all features currently in the feature \
 encyclopedia"]])
 
     bot.add_command("help", "This list of commands", greeting)
 
     bot.add_command("check [host _FQDN or IP address_ | file _filespec_] \
-[with timing]",
+[with timing] [with details]",
                     "Check a Catalyst switch config for both translatable \
 and possible Meraki features",
                     greeting)
 
+    bot.add_command("check _drag-and-drop files_ [with timing] [with details]\
+",
+                    "Check one or more Catalyst switch config files for both \
+translatable and possible Meraki features",
+                    greeting)
+
+    bot.add_command("check [network _Meraki network_] [with timing] \
+[with details]",
+                    "Check the configs of cloud monitored Catalyst switches \
+for both translatable and possible Meraki features",
+                    greeting)
+
     bot.add_command("register [host _FQDN or IP address_] [with timing]",
                     "Register a Catalyst switch to the Meraki Dashboard",
                     greeting)
 
     bot.add_command("claim [_Meraki serial numbers_] [to _Meraki network \
 name_] [with timing]",
                     "Claim Catalyst switches to a Meraki Network",
@@ -1821,14 +1968,18 @@
     # other command with the remove_command(command) method.
     bot.remove_command("/echo")
 else:
     command_list = list(list())
     command_list.extend([
         ["help", "This list of commands"],
 
+        ["check network <Meraki network name> [with timing] [with details]",
+         "Check the configs of cloud monitored Catalyst switches for both \
+translatable and possible Meraki features"],
+
         ["check host <FQDN or IP address> | file <filespec> [with timing] \
 [with details]",
          "Check a Catalyst switch config for both translatable and possible \
 Meraki features"],
 
         ["register host <FQDN or IP address> [with timing]",
          "Register a Catalyst switch to the Meraki Dashboard"],
```

### Comparing `merakicat-0.1.6/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.1.7/src/merakicat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.1.6
+Version: 0.1.7
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -230,18 +230,24 @@
 
 The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
 
 
 
 # History
 
+## 0.1.7 (04-01-2024)
+
+  - Added the ability to Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features.
+  - Included "with timing" and "with details" options on check drag-n-drop.
+  - Renamed some called functions in external modules.
+
 ## 0.1.6 (03-26-2024)
 
   - Updated encyclopedia.
-  - Migrated batch helper code.
+  - Migrated batch helper code for cleaner installation.
 
 ## 0.1.5 (03-23-2024)
 
   - Supports NM ports.
   - Merged nm-specifics into the encyclopedia.
 
 ## 0.1.4 (03-21-2024)
```

### Comparing `merakicat-0.1.6/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.1.7/src/merakicat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 images/newbot.jpg
 src/merakicat/__init__.py
 src/merakicat/bulk_check.sh
 src/merakicat/bulk_migrate.sh
 src/merakicat/mc_cfg_check.py
 src/merakicat/mc_claim.py
 src/merakicat/mc_file_exists.py
+src/merakicat/mc_get_config.py
+src/merakicat/mc_get_nms.py
 src/merakicat/mc_pedia.py
 src/merakicat/mc_ping.py
 src/merakicat/mc_register.py
 src/merakicat/mc_splitcheck_serials.py
 src/merakicat/mc_translate.py
 src/merakicat/mc_user_sample.py
 src/merakicat/merakicat.py
```

### Comparing `merakicat-0.1.6/tox.ini` & `merakicat-0.1.7/tox.ini`

 * *Files identical despite different names*

