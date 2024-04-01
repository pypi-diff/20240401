# Comparing `tmp/optidata-core-1.8.0.tar.gz` & `tmp/optidata-core-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optidata-core-1.8.0.tar", last modified: Fri Mar 29 03:10:16 2024, max compression
+gzip compressed data, was "optidata-core-1.9.0.tar", last modified: Mon Apr  1 12:24:43 2024, max compression
```

## Comparing `optidata-core-1.8.0.tar` & `optidata-core-1.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.060418 optidata-core-1.8.0/
--rw-r--r--   0 gtorres    (501) staff       (20)     1073 2024-03-22 14:30:04.000000 optidata-core-1.8.0/LICENSE
--rw-r--r--   0 gtorres    (501) staff       (20)      537 2024-03-29 03:10:16.060034 optidata-core-1.8.0/PKG-INFO
--rw-r--r--   0 gtorres    (501) staff       (20)      401 2024-03-26 15:11:40.000000 optidata-core-1.8.0/README.md
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.030608 optidata-core-1.8.0/app/
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.032577 optidata-core-1.8.0/app/optidata/
--rw-r--r--   0 gtorres    (501) staff       (20)       22 2024-03-25 16:27:18.000000 optidata-core-1.8.0/app/optidata/__init__.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.033296 optidata-core-1.8.0/app/optidata/core/
--rw-r--r--   0 gtorres    (501) staff       (20)       98 2024-03-25 20:34:03.000000 optidata-core-1.8.0/app/optidata/core/__init__.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.033913 optidata-core-1.8.0/app/optidata/core/src/
--rw-r--r--   0 gtorres    (501) staff       (20)      444 2024-03-25 20:39:07.000000 optidata-core-1.8.0/app/optidata/core/src/__init__.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.039249 optidata-core-1.8.0/app/optidata/core/src/config/
--rw-r--r--   0 gtorres    (501) staff       (20)      197 2024-03-25 18:56:53.000000 optidata-core-1.8.0/app/optidata/core/src/config/__init__.py
--rw-r--r--   0 gtorres    (501) staff       (20)     1424 2024-03-25 17:13:31.000000 optidata-core-1.8.0/app/optidata/core/src/config/api_rest.py
--rw-r--r--   0 gtorres    (501) staff       (20)     4745 2024-03-25 16:43:16.000000 optidata-core-1.8.0/app/optidata/core/src/config/constantes.py
--rw-r--r--   0 gtorres    (501) staff       (20)       97 2024-03-25 17:11:02.000000 optidata-core-1.8.0/app/optidata/core/src/config/error_handling.py
--rw-r--r--   0 gtorres    (501) staff       (20)     2466 2024-03-25 16:41:22.000000 optidata-core-1.8.0/app/optidata/core/src/config/kafka_config.py
--rw-r--r--   0 gtorres    (501) staff       (20)     5510 2024-03-29 03:07:49.000000 optidata-core-1.8.0/app/optidata/core/src/config/settings.py
--rw-r--r--   0 gtorres    (501) staff       (20)     4182 2024-03-25 16:45:58.000000 optidata-core-1.8.0/app/optidata/core/src/config/sftp.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.041118 optidata-core-1.8.0/app/optidata/core/src/database/
--rw-r--r--   0 gtorres    (501) staff       (20)       92 2024-03-25 18:57:13.000000 optidata-core-1.8.0/app/optidata/core/src/database/__init__.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.042717 optidata-core-1.8.0/app/optidata/core/src/database/entities/
--rw-r--r--   0 gtorres    (501) staff       (20)        1 2024-03-25 18:57:22.000000 optidata-core-1.8.0/app/optidata/core/src/database/entities/__init__.py
--rw-r--r--   0 gtorres    (501) staff       (20)     6002 2024-03-14 17:35:25.000000 optidata-core-1.8.0/app/optidata/core/src/database/entities/tb_oracle.py
--rw-r--r--   0 gtorres    (501) staff       (20)     7057 2024-03-25 19:44:36.000000 optidata-core-1.8.0/app/optidata/core/src/database/mongodb.py
--rw-r--r--   0 gtorres    (501) staff       (20)      879 2024-03-25 16:48:11.000000 optidata-core-1.8.0/app/optidata/core/src/database/oracle.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.043584 optidata-core-1.8.0/app/optidata/core/src/enums/
--rw-r--r--   0 gtorres    (501) staff       (20)       53 2024-03-25 17:15:51.000000 optidata-core-1.8.0/app/optidata/core/src/enums/__init__.py
--rw-r--r--   0 gtorres    (501) staff       (20)      380 2024-03-22 13:52:10.000000 optidata-core-1.8.0/app/optidata/core/src/enums/enums.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.044545 optidata-core-1.8.0/app/optidata/core/src/messages/
--rw-r--r--   0 gtorres    (501) staff       (20)       31 2024-03-25 16:50:26.000000 optidata-core-1.8.0/app/optidata/core/src/messages/__init__.py
--rw-r--r--   0 gtorres    (501) staff       (20)      662 2024-03-25 16:50:49.000000 optidata-core-1.8.0/app/optidata/core/src/messages/messages.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.050491 optidata-core-1.8.0/app/optidata/core/src/services/
--rw-r--r--   0 gtorres    (501) staff       (20)     1615 2024-03-25 17:16:42.000000 optidata-core-1.8.0/app/optidata/core/src/services/__init__.py
--rw-r--r--   0 gtorres    (501) staff       (20)    54138 2024-03-25 15:22:22.000000 optidata-core-1.8.0/app/optidata/core/src/services/conciliation.py
--rw-r--r--   0 gtorres    (501) staff       (20)    26480 2024-03-25 15:22:47.000000 optidata-core-1.8.0/app/optidata/core/src/services/config_rules.py
--rw-r--r--   0 gtorres    (501) staff       (20)     4253 2024-03-25 15:23:17.000000 optidata-core-1.8.0/app/optidata/core/src/services/cycles.py
--rw-r--r--   0 gtorres    (501) staff       (20)      300 2024-03-25 17:06:37.000000 optidata-core-1.8.0/app/optidata/core/src/services/messages.py
--rw-r--r--   0 gtorres    (501) staff       (20)     3875 2024-03-25 15:23:33.000000 optidata-core-1.8.0/app/optidata/core/src/services/partner.py
--rw-r--r--   0 gtorres    (501) staff       (20)     3774 2024-03-25 15:23:56.000000 optidata-core-1.8.0/app/optidata/core/src/services/role.py
--rw-r--r--   0 gtorres    (501) staff       (20)     3834 2024-03-25 15:24:12.000000 optidata-core-1.8.0/app/optidata/core/src/services/type_cycles.py
--rw-r--r--   0 gtorres    (501) staff       (20)     5381 2024-03-25 15:24:26.000000 optidata-core-1.8.0/app/optidata/core/src/services/users.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.056005 optidata-core-1.8.0/app/optidata/core/src/utility/
--rw-r--r--   0 gtorres    (501) staff       (20)      509 2024-03-29 03:02:04.000000 optidata-core-1.8.0/app/optidata/core/src/utility/__init__.py
--rw-r--r--   0 gtorres    (501) staff       (20)     2405 2024-03-29 00:45:13.000000 optidata-core-1.8.0/app/optidata/core/src/utility/utils.py
--rw-r--r--   0 gtorres    (501) staff       (20)    28603 2024-03-25 15:29:15.000000 optidata-core-1.8.0/app/optidata/core/src/utility/utils_file.py
--rw-r--r--   0 gtorres    (501) staff       (20)      795 2024-03-25 20:33:57.000000 optidata-core-1.8.0/app/optidata/core/src/utility/utils_messages.py
-drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-03-29 03:10:16.059316 optidata-core-1.8.0/app/optidata_core.egg-info/
--rw-r--r--   0 gtorres    (501) staff       (20)      537 2024-03-29 03:10:15.000000 optidata-core-1.8.0/app/optidata_core.egg-info/PKG-INFO
--rw-r--r--   0 gtorres    (501) staff       (20)     1569 2024-03-29 03:10:15.000000 optidata-core-1.8.0/app/optidata_core.egg-info/SOURCES.txt
--rw-r--r--   0 gtorres    (501) staff       (20)        1 2024-03-29 03:10:15.000000 optidata-core-1.8.0/app/optidata_core.egg-info/dependency_links.txt
--rw-r--r--   0 gtorres    (501) staff       (20)      257 2024-03-29 03:10:15.000000 optidata-core-1.8.0/app/optidata_core.egg-info/requires.txt
--rw-r--r--   0 gtorres    (501) staff       (20)        9 2024-03-29 03:10:15.000000 optidata-core-1.8.0/app/optidata_core.egg-info/top_level.txt
--rw-r--r--   0 gtorres    (501) staff       (20)       38 2024-03-29 03:10:16.060566 optidata-core-1.8.0/setup.cfg
--rw-r--r--   0 gtorres    (501) staff       (20)     1262 2024-03-29 03:02:36.000000 optidata-core-1.8.0/setup.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.818474 optidata-core-1.9.0/
+-rw-r--r--   0 gtorres    (501) staff       (20)     1073 2024-03-22 14:30:04.000000 optidata-core-1.9.0/LICENSE
+-rw-r--r--   0 gtorres    (501) staff       (20)      537 2024-04-01 12:24:43.818132 optidata-core-1.9.0/PKG-INFO
+-rw-r--r--   0 gtorres    (501) staff       (20)      401 2024-03-26 15:11:40.000000 optidata-core-1.9.0/README.md
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.794285 optidata-core-1.9.0/app/
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.798282 optidata-core-1.9.0/app/optidata/
+-rw-r--r--   0 gtorres    (501) staff       (20)       22 2024-03-25 16:27:18.000000 optidata-core-1.9.0/app/optidata/__init__.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.798689 optidata-core-1.9.0/app/optidata/core/
+-rw-r--r--   0 gtorres    (501) staff       (20)       98 2024-03-25 20:34:03.000000 optidata-core-1.9.0/app/optidata/core/__init__.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.799048 optidata-core-1.9.0/app/optidata/core/src/
+-rw-r--r--   0 gtorres    (501) staff       (20)      444 2024-03-25 20:39:07.000000 optidata-core-1.9.0/app/optidata/core/src/__init__.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.802267 optidata-core-1.9.0/app/optidata/core/src/config/
+-rw-r--r--   0 gtorres    (501) staff       (20)      197 2024-03-25 18:56:53.000000 optidata-core-1.9.0/app/optidata/core/src/config/__init__.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     1424 2024-03-25 17:13:31.000000 optidata-core-1.9.0/app/optidata/core/src/config/api_rest.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     4745 2024-03-25 16:43:16.000000 optidata-core-1.9.0/app/optidata/core/src/config/constantes.py
+-rw-r--r--   0 gtorres    (501) staff       (20)       97 2024-03-25 17:11:02.000000 optidata-core-1.9.0/app/optidata/core/src/config/error_handling.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     2466 2024-03-25 16:41:22.000000 optidata-core-1.9.0/app/optidata/core/src/config/kafka_config.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     5510 2024-04-01 11:48:44.000000 optidata-core-1.9.0/app/optidata/core/src/config/settings.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     4182 2024-03-25 16:45:58.000000 optidata-core-1.9.0/app/optidata/core/src/config/sftp.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.804204 optidata-core-1.9.0/app/optidata/core/src/database/
+-rw-r--r--   0 gtorres    (501) staff       (20)       92 2024-03-25 18:57:13.000000 optidata-core-1.9.0/app/optidata/core/src/database/__init__.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.805414 optidata-core-1.9.0/app/optidata/core/src/database/entities/
+-rw-r--r--   0 gtorres    (501) staff       (20)        1 2024-03-25 18:57:22.000000 optidata-core-1.9.0/app/optidata/core/src/database/entities/__init__.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     6002 2024-03-14 17:35:25.000000 optidata-core-1.9.0/app/optidata/core/src/database/entities/tb_oracle.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     7057 2024-03-25 19:44:36.000000 optidata-core-1.9.0/app/optidata/core/src/database/mongodb.py
+-rw-r--r--   0 gtorres    (501) staff       (20)      879 2024-03-25 16:48:11.000000 optidata-core-1.9.0/app/optidata/core/src/database/oracle.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.807023 optidata-core-1.9.0/app/optidata/core/src/enums/
+-rw-r--r--   0 gtorres    (501) staff       (20)       53 2024-03-25 17:15:51.000000 optidata-core-1.9.0/app/optidata/core/src/enums/__init__.py
+-rw-r--r--   0 gtorres    (501) staff       (20)      380 2024-03-22 13:52:10.000000 optidata-core-1.9.0/app/optidata/core/src/enums/enums.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.808221 optidata-core-1.9.0/app/optidata/core/src/messages/
+-rw-r--r--   0 gtorres    (501) staff       (20)       31 2024-03-25 16:50:26.000000 optidata-core-1.9.0/app/optidata/core/src/messages/__init__.py
+-rw-r--r--   0 gtorres    (501) staff       (20)      662 2024-03-25 16:50:49.000000 optidata-core-1.9.0/app/optidata/core/src/messages/messages.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.813737 optidata-core-1.9.0/app/optidata/core/src/services/
+-rw-r--r--   0 gtorres    (501) staff       (20)     1615 2024-03-25 17:16:42.000000 optidata-core-1.9.0/app/optidata/core/src/services/__init__.py
+-rw-r--r--   0 gtorres    (501) staff       (20)    54138 2024-03-25 15:22:22.000000 optidata-core-1.9.0/app/optidata/core/src/services/conciliation.py
+-rw-r--r--   0 gtorres    (501) staff       (20)    26480 2024-03-25 15:22:47.000000 optidata-core-1.9.0/app/optidata/core/src/services/config_rules.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     4253 2024-03-25 15:23:17.000000 optidata-core-1.9.0/app/optidata/core/src/services/cycles.py
+-rw-r--r--   0 gtorres    (501) staff       (20)      300 2024-03-25 17:06:37.000000 optidata-core-1.9.0/app/optidata/core/src/services/messages.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     3875 2024-03-25 15:23:33.000000 optidata-core-1.9.0/app/optidata/core/src/services/partner.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     3774 2024-03-25 15:23:56.000000 optidata-core-1.9.0/app/optidata/core/src/services/role.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     3834 2024-03-25 15:24:12.000000 optidata-core-1.9.0/app/optidata/core/src/services/type_cycles.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     5381 2024-03-25 15:24:26.000000 optidata-core-1.9.0/app/optidata/core/src/services/users.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.815492 optidata-core-1.9.0/app/optidata/core/src/utility/
+-rw-r--r--   0 gtorres    (501) staff       (20)      509 2024-03-29 03:02:04.000000 optidata-core-1.9.0/app/optidata/core/src/utility/__init__.py
+-rw-r--r--   0 gtorres    (501) staff       (20)     2469 2024-04-01 12:12:43.000000 optidata-core-1.9.0/app/optidata/core/src/utility/utils.py
+-rw-r--r--   0 gtorres    (501) staff       (20)    28603 2024-03-25 15:29:15.000000 optidata-core-1.9.0/app/optidata/core/src/utility/utils_file.py
+-rw-r--r--   0 gtorres    (501) staff       (20)      795 2024-03-25 20:33:57.000000 optidata-core-1.9.0/app/optidata/core/src/utility/utils_messages.py
+drwxr-xr-x   0 gtorres    (501) staff       (20)        0 2024-04-01 12:24:43.817578 optidata-core-1.9.0/app/optidata_core.egg-info/
+-rw-r--r--   0 gtorres    (501) staff       (20)      537 2024-04-01 12:24:43.000000 optidata-core-1.9.0/app/optidata_core.egg-info/PKG-INFO
+-rw-r--r--   0 gtorres    (501) staff       (20)     1569 2024-04-01 12:24:43.000000 optidata-core-1.9.0/app/optidata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 gtorres    (501) staff       (20)        1 2024-04-01 12:24:43.000000 optidata-core-1.9.0/app/optidata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 gtorres    (501) staff       (20)      257 2024-04-01 12:24:43.000000 optidata-core-1.9.0/app/optidata_core.egg-info/requires.txt
+-rw-r--r--   0 gtorres    (501) staff       (20)        9 2024-04-01 12:24:43.000000 optidata-core-1.9.0/app/optidata_core.egg-info/top_level.txt
+-rw-r--r--   0 gtorres    (501) staff       (20)       38 2024-04-01 12:24:43.818579 optidata-core-1.9.0/setup.cfg
+-rw-r--r--   0 gtorres    (501) staff       (20)     1262 2024-04-01 11:48:21.000000 optidata-core-1.9.0/setup.py
```

### Comparing `optidata-core-1.8.0/LICENSE` & `optidata-core-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/PKG-INFO` & `optidata-core-1.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optidata-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: Paquete de Python para OptiData
 Home-page: UNKNOWN
 Author: Gonzalo Torres Moya
 Author-email: <gtorres@optimisa.cl>
 License: MIT
 Keywords: python,optidata-core
 Platform: UNKNOWN
```

### Comparing `optidata-core-1.8.0/app/optidata/core/src/config/api_rest.py` & `optidata-core-1.9.0/app/optidata/core/src/config/api_rest.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/config/constantes.py` & `optidata-core-1.9.0/app/optidata/core/src/config/constantes.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/config/kafka_config.py` & `optidata-core-1.9.0/app/optidata/core/src/config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/config/settings.py` & `optidata-core-1.9.0/app/optidata/core/src/config/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Version liberación - Release ddmmyyyy
 import os
 
 from ..utility.utils import get_value_env
 
-APP_VERSION = '1.8.0'
+APP_VERSION = '1.9.0'
 # Flask Settings
 FLASK_SECRET_KEY = '0pt1m1$42560-$3cr3t4'
 FLASK_SERVER_NAME_API = get_value_env(os.environ['SERVER_API_BE'])
 FLASK_SERVER_PORT_API = get_value_env(os.environ['SERVER_BE_PORT'])
 
 FLASK_SERVER_NAME_SCH = get_value_env(os.environ['SERVER_API_SCHED'])
 FLASK_SERVER_PORT_SCH = get_value_env(os.environ['SERVER_SCHED_PORT'])
```

### Comparing `optidata-core-1.8.0/app/optidata/core/src/config/sftp.py` & `optidata-core-1.9.0/app/optidata/core/src/config/sftp.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/database/entities/tb_oracle.py` & `optidata-core-1.9.0/app/optidata/core/src/database/entities/tb_oracle.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/database/mongodb.py` & `optidata-core-1.9.0/app/optidata/core/src/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/database/oracle.py` & `optidata-core-1.9.0/app/optidata/core/src/database/oracle.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/messages/messages.py` & `optidata-core-1.9.0/app/optidata/core/src/messages/messages.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/__init__.py` & `optidata-core-1.9.0/app/optidata/core/src/services/__init__.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/conciliation.py` & `optidata-core-1.9.0/app/optidata/core/src/services/conciliation.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/config_rules.py` & `optidata-core-1.9.0/app/optidata/core/src/services/config_rules.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/cycles.py` & `optidata-core-1.9.0/app/optidata/core/src/services/cycles.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/partner.py` & `optidata-core-1.9.0/app/optidata/core/src/services/partner.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/role.py` & `optidata-core-1.9.0/app/optidata/core/src/services/role.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/type_cycles.py` & `optidata-core-1.9.0/app/optidata/core/src/services/type_cycles.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/services/users.py` & `optidata-core-1.9.0/app/optidata/core/src/services/users.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/utility/utils.py` & `optidata-core-1.9.0/app/optidata/core/src/utility/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,21 +86,24 @@
         return data[pos_ini:total]
     elif pos_ini:
         return data[pos_ini:]
     else:
         return data[:total]
 
 
-def get_value_env(v):
+def get_value_env(v, enc=False):
     # Generation of a key
     # key = Fernet.generate_key()
-    cipher_suite = Fernet(os.environ['OPTIDATA_KEY'])
+    if enc:
+        cipher_suite = Fernet(bytes(os.environ['OPTIDATA_KEY'], "utf8"))
 
-    response = cipher_suite.decrypt(v)
-    return response.decode()
+        response = cipher_suite.decrypt(v)
+        return response.decode()
+
+    return v
 
 
 class DateTimeEncoder(json.JSONEncoder):
     def default(self, z):
         if isinstance(z, datetime):
             return str(z)
         else:
```

### Comparing `optidata-core-1.8.0/app/optidata/core/src/utility/utils_file.py` & `optidata-core-1.9.0/app/optidata/core/src/utility/utils_file.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata/core/src/utility/utils_messages.py` & `optidata-core-1.9.0/app/optidata/core/src/utility/utils_messages.py`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/app/optidata_core.egg-info/PKG-INFO` & `optidata-core-1.9.0/app/optidata_core.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optidata-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: Paquete de Python para OptiData
 Home-page: UNKNOWN
 Author: Gonzalo Torres Moya
 Author-email: <gtorres@optimisa.cl>
 License: MIT
 Keywords: python,optidata-core
 Platform: UNKNOWN
```

### Comparing `optidata-core-1.8.0/app/optidata_core.egg-info/SOURCES.txt` & `optidata-core-1.9.0/app/optidata_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optidata-core-1.8.0/setup.py` & `optidata-core-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.8.0'  # settings.APP_VERSION
+VERSION = '1.9.0'  # settings.APP_VERSION
 DESCRIPTION = 'Paquete de Python para OptiData'
 LONG_DESCRIPTION = 'Paquete para OptiData que contiene funcionalidades para realizar una Conciliación con Pandas y Vaex'
 
 # Configurando
 setup(
     name="optidata-core",
     version=VERSION,
```

