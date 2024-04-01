# Comparing `tmp/apollo-orm-2.1.0.tar.gz` & `tmp/apollo-orm-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-orm-2.1.0.tar", last modified: Thu Mar 28 12:39:12 2024, max compression
+gzip compressed data, was "apollo-orm-2.1.1.tar", last modified: Mon Apr  1 20:58:37 2024, max compression
```

## Comparing `apollo-orm-2.1.0.tar` & `apollo-orm-2.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.508533 apollo-orm-2.1.0/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-03-28 12:39:12.507326 apollo-orm-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.477554 apollo-orm-2.1.0/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.0/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.482034 apollo-orm-2.1.0/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.0/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.482034 apollo-orm-2.1.0/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.0/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.483131 apollo-orm-2.1.0/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.484232 apollo-orm-2.1.0/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.485286 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.487382 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.488437 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.489473 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.491772 apollo-orm-2.1.0/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.493070 apollo-orm-2.1.0/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.495184 apollo-orm-2.1.0/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.0/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.496233 apollo-orm-2.1.0/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.0/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.498318 apollo-orm-2.1.0/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.0/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.0/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.0/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    20477 2024-03-28 12:37:10.000000 apollo-orm-2.1.0/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.501439 apollo-orm-2.1.0/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.0/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.0/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.0/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.0/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.501439 apollo-orm-2.1.0/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.0/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.503834 apollo-orm-2.1.0/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.0/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.0/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.504940 apollo-orm-2.1.0/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.0/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.0/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.506251 apollo-orm-2.1.0/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-03-28 12:39:12.000000 apollo-orm-2.1.0/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-03-28 12:39:12.000000 apollo-orm-2.1.0/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 12:39:12.000000 apollo-orm-2.1.0/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-28 12:39:12.000000 apollo-orm-2.1.0/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-03-28 12:37:10.000000 apollo-orm-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 12:39:12.508533 apollo-orm-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 12:39:12.506251 apollo-orm-2.1.0/tests/
--rw-rw-rw-   0        0        0    13745 2024-03-27 21:46:59.000000 apollo-orm-2.1.0/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.786523 apollo-orm-2.1.1/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo-orm-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-01 20:58:37.785087 apollo-orm-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo-orm-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.750048 apollo-orm-2.1.1/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo-orm-2.1.1/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.755054 apollo-orm-2.1.1/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo-orm-2.1.1/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.756049 apollo-orm-2.1.1/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo-orm-2.1.1/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.757049 apollo-orm-2.1.1/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.759106 apollo-orm-2.1.1/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.759106 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.761105 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.763145 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.764145 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.766146 apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.767150 apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.769524 apollo-orm-2.1.1/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo-orm-2.1.1/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.770797 apollo-orm-2.1.1/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo-orm-2.1.1/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.774352 apollo-orm-2.1.1/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo-orm-2.1.1/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo-orm-2.1.1/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo-orm-2.1.1/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    20501 2024-04-01 20:58:02.000000 apollo-orm-2.1.1/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.777684 apollo-orm-2.1.1/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo-orm-2.1.1/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.779685 apollo-orm-2.1.1/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo-orm-2.1.1/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.780683 apollo-orm-2.1.1/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo-orm-2.1.1/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo-orm-2.1.1/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.782686 apollo-orm-2.1.1/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo-orm-2.1.1/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo-orm-2.1.1/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.784079 apollo-orm-2.1.1/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-01 20:58:37.000000 apollo-orm-2.1.1/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-01 20:58:19.000000 apollo-orm-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:58:37.786523 apollo-orm-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 20:58:37.782686 apollo-orm-2.1.1/tests/
+-rw-rw-rw-   0        0        0    13745 2024-03-27 21:46:59.000000 apollo-orm-2.1.1/tests/test_full_process.py
```

### Comparing `apollo-orm-2.1.0/LICENSE` & `apollo-orm-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/PKG-INFO` & `apollo-orm-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.0
+Version: 2.1.1
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.0/README.md` & `apollo-orm-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo-orm-2.1.1/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo-orm-2.1.1/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo-orm-2.1.1/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/orm/abstracts/idatabase.py` & `apollo-orm-2.1.1/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/orm/core.py` & `apollo-orm-2.1.1/apollo_orm/orm/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 
 def _timestamp_validate(value: Any) -> datetime:
     if isinstance(value, datetime):
         return value
     elif isinstance(value, str):
         formats = ["%Y-%m-%d %H:%M:%S", "%Y-%m-%dT%H:%M:%S.%fZ", "%Y-%m-%dT%H:%M:%SZ", "%Y-%m-%dT%H:%M:%S.%f",
-                   "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d"]
+                   "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d", "%Y-%m-%d %H:%M:%S.%f"]
         for fmt in formats:
             try:
                 return datetime.strptime(value, fmt)
             except ValueError:
                 continue
     raise ValueError("No valid date format found")
```

### Comparing `apollo-orm-2.1.0/apollo_orm/orm/credentials/credential_service.py` & `apollo-orm-2.1.1/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/orm/credentials/json_credential_service.py` & `apollo-orm-2.1.1/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo-orm-2.1.1/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo-orm-2.1.1/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm/utils/logger/logger.py` & `apollo-orm-2.1.1/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/apollo_orm.egg-info/PKG-INFO` & `apollo-orm-2.1.1/apollo_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.0
+Version: 2.1.1
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-orm-2.1.0/apollo_orm.egg-info/SOURCES.txt` & `apollo-orm-2.1.1/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-orm-2.1.0/pyproject.toml` & `apollo-orm-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo-orm-2.1.0/tests/test_full_process.py` & `apollo-orm-2.1.1/tests/test_full_process.py`

 * *Files identical despite different names*

