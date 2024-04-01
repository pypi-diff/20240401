# Comparing `tmp/metasdk-1.7.6.tar.gz` & `tmp/metasdk-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasdk-1.7.6.tar", last modified: Thu Mar 28 15:09:28 2024, max compression
+gzip compressed data, was "metasdk-1.7.7.tar", last modified: Mon Apr  1 15:10:02 2024, max compression
```

## Comparing `metasdk-1.7.6.tar` & `metasdk-1.7.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-03-28 15:09:28.209778 metasdk-1.7.6/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.6/LICENSE
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.6/MANIFEST.in
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-03-28 15:09:28.209778 metasdk-1.7.6/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.6/README.md
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-03-28 15:09:28.205778 metasdk-1.7.6/metasdk/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-02-12 19:35:51.000000 metasdk-1.7.6/metasdk/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/__state.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/apiclient.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/event_bus.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/exceptions.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-03-28 15:08:27.000000 metasdk-1.7.6/metasdk/info.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/internal.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-03-28 15:09:28.205778 metasdk-1.7.6/metasdk/logger/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/logger/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/logger/bulk_logger.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.6/metasdk/logger/logger.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-03-28 15:09:28.209778 metasdk-1.7.6/metasdk/services/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/ApiProxyService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5353 2024-03-28 15:08:27.000000 metasdk-1.7.6/metasdk/services/AuthService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/CacheService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/DbQueryService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.6/metasdk/services/DbService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/DevService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/ExportService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/ExternalSystemService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    15701 2024-03-28 15:08:27.000000 metasdk-1.7.6/metasdk/services/FeedService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/IssueService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.6/metasdk/services/LockService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/MailService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/MediaService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/MetaqlService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/ObjectLogService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/SettingsService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8731 2023-12-07 09:05:36.000000 metasdk-1.7.6/metasdk/services/StarterService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/UserManagementService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/services/__init__.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-03-28 15:09:28.209778 metasdk-1.7.6/metasdk/tools/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/tools/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.6/metasdk/tools/extract_event_handlers.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/utils.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.6/metasdk/worker.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-03-28 15:09:28.205778 metasdk-1.7.6/metasdk.egg-info/
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-03-28 15:09:28.000000 metasdk-1.7.6/metasdk.egg-info/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-03-28 15:09:28.000000 metasdk-1.7.6/metasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-03-28 15:09:28.000000 metasdk-1.7.6/metasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-03-28 15:09:28.000000 metasdk-1.7.6/metasdk.egg-info/requires.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-03-28 15:09:28.000000 metasdk-1.7.6/metasdk.egg-info/top_level.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-03-28 15:09:28.209778 metasdk-1.7.6/setup.cfg
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.6/setup.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.7/LICENSE
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.7/MANIFEST.in
+-rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-01 15:10:02.145038 metasdk-1.7.7/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.7/README.md
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-02-12 19:35:51.000000 metasdk-1.7.7/metasdk/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/__state.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/apiclient.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/event_bus.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/exceptions.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-04-01 14:33:24.000000 metasdk-1.7.7/metasdk/info.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/internal.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/logger/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/logger/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/logger/bulk_logger.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/logger/logger.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/services/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ApiProxyService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5098 2024-04-01 14:33:24.000000 metasdk-1.7.7/metasdk/services/AuthService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/CacheService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/DbQueryService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/services/DbService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/DevService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ExportService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ExternalSystemService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    18707 2024-04-01 15:06:59.000000 metasdk-1.7.7/metasdk/services/FeedService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/IssueService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/services/LockService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/MailService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/MediaService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/MetaqlService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/ObjectLogService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/SettingsService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     8731 2023-12-07 09:05:36.000000 metasdk-1.7.7/metasdk/services/StarterService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/UserManagementService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/services/__init__.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk/tools/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/tools/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.7/metasdk/tools/extract_event_handlers.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/utils.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.7/metasdk/worker.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-01 15:10:02.145038 metasdk-1.7.7/metasdk.egg-info/
+-rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/requires.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-04-01 15:10:02.000000 metasdk-1.7.7/metasdk.egg-info/top_level.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-04-01 15:10:02.145038 metasdk-1.7.7/setup.cfg
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.7/setup.py
```

### Comparing `metasdk-1.7.6/LICENSE` & `metasdk-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/PKG-INFO` & `metasdk-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.7.6
+Version: 1.7.7
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `metasdk-1.7.6/README.md` & `metasdk-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/__init__.py` & `metasdk-1.7.7/metasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/apiclient.py` & `metasdk-1.7.7/metasdk/apiclient.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/event_bus.py` & `metasdk-1.7.7/metasdk/event_bus.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/exceptions.py` & `metasdk-1.7.7/metasdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/internal.py` & `metasdk-1.7.7/metasdk/internal.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/logger/__init__.py` & `metasdk-1.7.7/metasdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/logger/bulk_logger.py` & `metasdk-1.7.7/metasdk/logger/bulk_logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/logger/logger.py` & `metasdk-1.7.7/metasdk/logger/logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/ApiProxyService.py` & `metasdk-1.7.7/metasdk/services/ApiProxyService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/AuthService.py` & `metasdk-1.7.7/metasdk/services/AuthService.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-import functools
 import urllib.parse
-from typing import Dict, List
+from typing import Dict, List, TypedDict
 
 import requests
 
 from metasdk import UnexpectedError
 from metasdk.exceptions import ForbiddenError, RequestError
 
 
+class AuthUserInfo(TypedDict):
+    auth_user_id: int
+    company_id: int
+    is_admin: bool
+
+
 class AuthService:
     def __init__(self, app):
         """
         Класс проверяет авторизационный токен и определяет пользователя.
 
         :param app: metasdk.MetaApp
         """
@@ -97,33 +102,23 @@
         select company_id, roles from public.users where id = :user_id
         """
         result = self.__app.db("meta").one(query, {"user_id": int(user_id)})
         if not result:
             raise RequestError("Пользователь не найден")
         return result
 
-    def __set_permissions(self, auth_info: Dict) -> Dict:
+    def __set_permissions(self, auth_info: Dict) -> AuthUserInfo:
         """
         Дополняет информацию о владельце токена.
 
         :param auth_info: ответ от сервера верификации.
         :return: None.
         """
         auth_user_id = self._identify_user(token_user_id=int(auth_info["userId"]))
         user_info = self._get_user_info(auth_user_id)
         company_id = user_info["company_id"]
         is_admin = True if self.__admin_role_id in user_info["roles"] else False
-        # TODO добавить валидацию с pydantic
         return {
             "auth_user_id": int(auth_user_id),
             "company_id": int(company_id),
             "is_admin": is_admin,
         }
-
-
-def auth_required(func):
-    @functools.wraps(func)
-    def wrapper(self, *args, **kwargs):
-        user_info = self.auth_service.verify_access_token(self.token, self.required_scopes)
-        self.auth_user_info = user_info
-        return func(self, *args, **kwargs)
-    return wrapper
```

### Comparing `metasdk-1.7.6/metasdk/services/CacheService.py` & `metasdk-1.7.7/metasdk/services/CacheService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/DbQueryService.py` & `metasdk-1.7.7/metasdk/services/DbQueryService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/DbService.py` & `metasdk-1.7.7/metasdk/services/DbService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/DevService.py` & `metasdk-1.7.7/metasdk/services/DevService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/ExportService.py` & `metasdk-1.7.7/metasdk/services/ExportService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/ExternalSystemService.py` & `metasdk-1.7.7/metasdk/services/ExternalSystemService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/FeedService.py` & `metasdk-1.7.7/metasdk/services/FeedService.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,36 @@
+import functools
 import json
 import re
 from tempfile import NamedTemporaryFile
-from typing import List, Dict
 
 import sqlparse
 
-from metasdk.services.AuthService import auth_required
+from metasdk.exceptions import BadParametersError, ForbiddenError
+from metasdk.services.AuthService import AuthUserInfo
 
 SOURCE_FORMAT_EXTENSION = {
     'CSV': '.csv',
     'TSV': '.tsv',
     'JSON_NEWLINE': '.json'
 }
 
 
+def auth_required(func):
+    @functools.wraps(func)
+    def wrapper(self, *args, **kwargs):
+        user_info = self.auth_service.verify_access_token(self.token, self.required_scopes)
+        self.auth_user_info = user_info
+
+        if kwargs.get("feed_id"):
+            self.check_feed_permissions(feed_id=kwargs["feed_id"], auth_user_info=user_info)
+        return func(self, *args, **kwargs)
+    return wrapper
+
+
 class FeedService:
     def __init__(self, app, token: str = ""):
         """
         :type app: metasdk.MetaApp
         """
         self.__app = app
         self.__options = {}
@@ -27,14 +40,44 @@
         self.__media = app.MediaService
         self.__starter = app.StarterService
         self.auth_service = app.AuthService
         self.token = token
         self.required_scopes = ["datahub"]
         self.auth_user_info = None
 
+    def check_feed_permissions(self, feed_id: str, auth_user_info: AuthUserInfo) -> bool:
+        """
+        Проверяет права доступа к фиду.
+
+        :param feed_id: ID фида.
+        :param auth_user_info: данные о пользователе, предоставившем валидный токен.
+        :return: True, если есть доступ к фиду, иначе - исключение PermissionError.
+        """
+        company_id = auth_user_info["company_id"]
+        author_user_id = auth_user_info["auth_user_id"]
+        query_params = {"feed_id": feed_id, "company_id": company_id, "author_user_id": author_user_id}
+
+        base_query = """
+        SELECT
+            fd.id AS feed_id
+        FROM meta.feed_datasource fd
+        LEFT JOIN public.users us ON fd.author_user_id =us.id
+        WHERE fd.id = :feed_id::uuid
+        """
+        if auth_user_info["is_admin"]:
+            query = f"{base_query} AND us.company_id = :company_id::int4"
+        else:
+            query = f"{base_query} AND fd.author_user_id = :author_user_id::int8"
+
+        result = self.__metadb.one(query, query_params)
+        if result and result["feed_id"]:
+            return True
+        else:
+            raise ForbiddenError("Do not have permissions to access this feed")
+
     def get_feed(self, datasource_id: str):
         """
         Получение настроек для фида
         :param datasource_id: идентификатор фида
         :return: FeedDataSource
         """
         info = self.__metadb.one(
@@ -105,36 +148,31 @@
         # TODO Выпилить потом класс используется для другого
         # TODO без applicationId не выбираются поля сущностей. Подумать на сколько это НЕ нормально
         response = self.__app.native_api_call('feed', 'datasource/' + datasource_id + '/process?applicationId=1', {},
                                               self.__options, False, None, False, http_method="POST")
         return json.loads(response.text)
 
     @auth_required
-    def list_feeds(self, filters: Dict) -> List[Dict]:
+    def list_feeds(self, filters: dict) -> list[dict]:
         """
         Получает список фидов юзера.
 
         :param filters: поля для фильтрации запроса. Формат '{column_name: filter_value}'.
         :param token: токен авторизации.
         :return: список фидов.
         """
         if not isinstance(filters, dict):
             msg = "filters должен быть словарём, в котором key - это название столбца, а value значение фильтрации"
             raise TypeError(msg)
-
-        if self.auth_user_info["is_admin"]:
-            query_params = {"company_id": self.auth_user_info["company_id"], **filters}
-        else:
-            query_params = {"author_user_id": self.auth_user_info["auth_user_id"], **filters}
-
         query = self._generate_list_feeds_query(filters=filters, is_admin=self.auth_user_info["is_admin"])
-        feeds = self.__metadb.all(query, query_params)
+        query_params = {**filters, **self.auth_user_info}
+        feeds = self.__metadb.all(command=query, params=query_params)
         return feeds
 
-    def _generate_list_feeds_query(self, filters: Dict = None, is_admin: bool = False) -> str:
+    def _generate_list_feeds_query(self, filters: dict = None, is_admin: bool = False) -> str:
         """
         Генерирует SQL запрос для получения списка фидов.
 
         :param filters: поля для фильтрации запроса. Формат '{column_name: filter_value}'.
         :return: SQL запрос.
         """
         base_query = """
@@ -149,20 +187,20 @@
             us.company_id 
         FROM meta.feed_datasource AS fd
         LEFT JOIN public.users AS us ON fd.author_user_id =us.id
         """
         if is_admin:
             base_query = f"{base_query} WHERE company_id = :company_id::int4"
         else:
-            base_query = f"{base_query} WHERE author_user_id = :author_user_id::int8"
+            base_query = f"{base_query} WHERE author_user_id = :auth_user_id::int8"
         filters_query = self._generate_filters_query(filters=filters)
         final_query = f"{base_query} {filters_query}"
         return sqlparse.format(final_query, reindent=True)
 
-    def _generate_tags_query(self, tags: List[str]) -> str:
+    def _generate_tags_query(self, tags: list[str]) -> str:
         """
         Гененрирует SQL запрос для фильтрации по полю tags.
 
         :param tags: список тэгов фида.
         :return: часть SQL запроса с фильтрацией по тэгам.
         """
         if not isinstance(tags, list):
@@ -175,15 +213,15 @@
         for tag in tags:
             # обработка спец символов
             tag_escaped = re.escape(tag)
             tag = f"""tags @> array['{tag_escaped}']"""
             tags_expr.append(tag)
         return " OR ".join(tags_expr)
 
-    def _generate_filters_query(self, filters: Dict = None) -> str:
+    def _generate_filters_query(self, filters: dict = None) -> str:
         """
         Гененирует SQL запрос со значениями фильтров.
 
         :param filters: поля для фильтрации запроса. Формат '{column_name: filter_value}'.
         :return: часть SQL запроса с фильтрами для вставки в WHERE.
         """
         if not filters:
@@ -203,37 +241,32 @@
                     filter_expr = f"AND {key} = :{key}::{special_types[key]}"
                 else:
                     filter_expr = f"AND {key} = :{key}"
             filters_sql.append(filter_expr)
         return " ".join(filters_sql)
 
     @auth_required
-    def get_feed_by_id(self, feed_id: str, last_tasks: bool = False) -> Dict:
+    def get_feed_by_id(self, feed_id: str, last_tasks: bool = False) -> dict:
         """
         Получает данные о конкретном фиде.
 
         :param feed_id: ID фида.
         :param token: токен авторизации.
         :param last_tasks: если True, то возвращает ID последних тасков фида в поле last_tasks.
         :return: данные о фиде.
         """
         if not feed_id:
             raise ValueError("'feed_id' is required")
 
         query_params = {"feed_id": feed_id}
-        if self.auth_user_info["is_admin"]:
-            query_params.update({"company_id": self.auth_user_info["company_id"]})
-        else:
-            query_params.update({"author_user_id": self.auth_user_info["auth_user_id"]})
-
-        query = self._generate_feed_by_id_query(last_tasks=last_tasks, is_admin=self.auth_user_info["is_admin"])
+        query = self._generate_feed_by_id_query(last_tasks=last_tasks)
         feed = self.__metadb.one(query, query_params)
         return feed
 
-    def _generate_feed_by_id_query(self, last_tasks: bool = False, is_admin: bool = False) -> str:
+    def _generate_feed_by_id_query(self, last_tasks: bool = False) -> str:
         """
         Генерирует SQL запрос для получения данных о фиде.
 
         Запрос дополнитено фильтруется по author_user_id, а не только по feed_id,
         чтобы ограничить доступ юзеров не к своим фидам.
 
         Для получения списка последних тасков дополнительно обращается к таблице 'job.task'.
@@ -259,19 +292,14 @@
         LEFT JOIN meta.feed_connector_type fct ON fct.id=fd.connector_type_id
         LEFT JOIN meta.feed_share_type fst ON fst.id = fd.share_type_id
         LEFT JOIN meta.feed_connector_type_preset ctp ON ctp.id = fd.connector_type_preset_id
         LEFT JOIN public.users us ON fd.author_user_id =us.id
         WHERE fd.id = :feed_id::uuid
         """
 
-        if is_admin:
-            base_query = f"{base_query} AND us.company_id = :company_id::int4"
-        else:
-            base_query = f"{base_query} AND fd.author_user_id = :author_user_id::int8"
-
         if last_tasks:
             last_tasks_query = self._generate_last_tasks_query()
             base_query = f"""
             WITH feed_data AS (
             {base_query}
             ),
             {last_tasks_query}
@@ -280,15 +308,14 @@
                 fd.connector_type_name,
                 fd.connector_type_preset_name,
                 fd.share_type_name,
                 aggt.last_tasks
             FROM feed_data fd
             LEFT JOIN agg_tasks aggt ON aggt.ds_id = fd.id
             """
-
         return sqlparse.format(base_query, reindent=True)
 
     def _generate_last_tasks_query(self) -> str:
         """
         Генерирет SQL запрос для получения последних тасков фида.
 
         Таски сортируются по 'creation_time'.
@@ -309,35 +336,30 @@
         ), agg_tasks AS (
             SELECT array_agg(id) AS last_tasks, ds_id FROM last_tasks GROUP BY ds_id
         )
         """
         return sqlparse.format(base_query, reindent=True)
 
     @auth_required
-    def get_tasks(self, feed_id: str) -> List[Dict]:
+    def get_tasks(self, feed_id: str) -> list[dict]:
         """
         Получает список тасков фида.
 
         :param feed_id: ID фида.
         :param token: токен авторизации.
         :return: данные о таске. '{id: status}'
         """
         if not feed_id:
             raise ValueError("'feed_id' обязательный параметр")
 
         query_params = {"feed_id": feed_id}
-        if self.auth_user_info["is_admin"]:
-            query_params.update({"company_id": self.auth_user_info["company_id"]})
-        else:
-            query_params.update({"author_user_id": self.auth_user_info["auth_user_id"]})
-
-        query = self._generate_tasks_query(is_admin=self.auth_user_info["is_admin"])
+        query = self._generate_tasks_query()
         return self.__metadb.all(query, query_params)
 
-    def _generate_tasks_query(self, is_admin: bool = False) -> str:
+    def _generate_tasks_query(self) -> str:
         """
         Генерирует SQL запрос для получения списка фидов.
 
         Таблица 'job.task' переодически очищается, поэтому там будут таски только за последние несколько дней.
         Фильтрация по 'service_id' ускоряет запрос.
         :param is_admin: флаг админа компании.
         :return: SQL запрос для получения списка тасков фида.
@@ -345,20 +367,68 @@
         base_query = """
         SELECT ta.id, ta.status 
         FROM job.task ta
         LEFT JOIN meta.feed_datasource fd ON (ta.data ->> 'ds_id')::uuid = fd.id
         LEFT JOIN public.users us ON fd.author_user_id =us.id 
         WHERE service_id = 'meta.datasource_share' AND data->>'ds_id' = :feed_id::text
         """
-        if is_admin:
-            base_query = f"{base_query} AND us.company_id = :company_id::int4"
-        else:
-            base_query = f"{base_query} AND fd.author_user_id = :author_user_id::int8"
         return sqlparse.format(base_query, reindent=True)
 
+    @auth_required
+    def update_feed(self, feed_id: str, update_values: dict) -> dict:
+        """
+        Обновляет данные о фиде.
+
+        Для обновления доступны колонки ["name", "user_status", "tags"].
+        Для обновления tags нужно передать строку вида "tag1, tag2, tag3".
+        :param feed_id: ID фида.
+        :param update_values: данные для обвноления в формате {col_name: value}
+        :return: результаты выполнения запроса от Meta API.
+        """
+        allowed_cols = ["name", "user_status", "tags"]
+
+        allowed_updates = {}
+        allowed_update_col_names = []
+        for col_name, coi_value in update_values.items():
+            if col_name in allowed_cols:
+                allowed_updates.update({col_name: coi_value})
+                allowed_update_col_names.append(col_name)
+            else:
+                raise BadParametersError(f"Column '{col_name}' is not allowed for update")
+
+        if allowed_updates.get("tags"):
+            allowed_updates["tags"] = f"{{{allowed_updates['tags']}}}"  # получится строка вида '{tag1, tag2}'
+
+        query_params = {"feed_id": feed_id, **allowed_updates}
+        query = self._generate_update_feed_query(allowed_update_col_names)
+        return self.__metadb.update(query, query_params)
+
+    def _generate_update_feed_query(self, col_names: list[str]) -> str:
+        """
+        Формирует SQL запрс для обновления данных фида.
+
+        :param col_names: список колонок для обновления.
+        :return: строка SQL запроса.
+        """
+        special_types = {
+            "user_status": "meta.user_status_type",
+            "tags": "_text",
+        }
+        col_updates = []
+        for col_name in col_names:
+            if special_types.get(col_name):
+                col_upd_expr = f"{col_name} = :{col_name}::{special_types[col_name]}"
+            else:
+                col_upd_expr = f"{col_name} = :{col_name}"
+            col_updates.append(col_upd_expr)
+        col_updates_expr = ", ".join(col_updates)
+
+        query = f"UPDATE meta.feed_datasource SET {col_updates_expr} WHERE id = :feed_id::uuid"
+        return sqlparse.format(query, reindent=True)
+
 
 class FeedDataSource:
     """
     Класс хранения данных по коннектору
     """
 
     def __init__(
```

### Comparing `metasdk-1.7.6/metasdk/services/IssueService.py` & `metasdk-1.7.7/metasdk/services/IssueService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/LockService.py` & `metasdk-1.7.7/metasdk/services/LockService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/MailService.py` & `metasdk-1.7.7/metasdk/services/MailService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/MediaService.py` & `metasdk-1.7.7/metasdk/services/MediaService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/MetaqlService.py` & `metasdk-1.7.7/metasdk/services/MetaqlService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/ObjectLogService.py` & `metasdk-1.7.7/metasdk/services/ObjectLogService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/SettingsService.py` & `metasdk-1.7.7/metasdk/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/StarterService.py` & `metasdk-1.7.7/metasdk/services/StarterService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/UserManagementService.py` & `metasdk-1.7.7/metasdk/services/UserManagementService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/services/__init__.py` & `metasdk-1.7.7/metasdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/tools/extract_event_handlers.py` & `metasdk-1.7.7/metasdk/tools/extract_event_handlers.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/utils.py` & `metasdk-1.7.7/metasdk/utils.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk/worker.py` & `metasdk-1.7.7/metasdk/worker.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/metasdk.egg-info/PKG-INFO` & `metasdk-1.7.7/metasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.7.6
+Version: 1.7.7
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `metasdk-1.7.6/metasdk.egg-info/SOURCES.txt` & `metasdk-1.7.7/metasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.6/setup.py` & `metasdk-1.7.7/setup.py`

 * *Files identical despite different names*

