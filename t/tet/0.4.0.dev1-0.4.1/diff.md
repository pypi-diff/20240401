# Comparing `tmp/tet-0.4.0.dev1.tar.gz` & `tmp/tet-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tet-0.4.0.dev1.tar", last modified: Fri Mar 19 14:33:07 2021, max compression
+gzip compressed data, was "tet-0.4.1.tar", last modified: Mon Apr  1 12:46:05 2024, max compression
```

## Comparing `tet-0.4.0.dev1.tar` & `tet-0.4.1.tar`

### file list

```diff
@@ -1,60 +1,58 @@
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/
--rw-r--r--   0 ztane     (1000) ztane     (1000)      470 2021-03-19 14:30:37.000000 tet-0.4.0.dev1/CHANGES.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)       60 2017-08-29 07:23:25.000000 tet-0.4.0.dev1/MANIFEST.in
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2525 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/PKG-INFO
--rw-r--r--   0 ztane     (1000) ztane     (1000)      494 2017-08-29 07:23:25.000000 tet-0.4.0.dev1/README.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)       38 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/setup.cfg
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1919 2021-03-19 14:32:59.000000 tet-0.4.0.dev1/setup.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.600541 tet-0.4.0.dev1/tet/
--rw-r--r--   0 ztane     (1000) ztane     (1000)       77 2017-08-29 07:27:44.000000 tet-0.4.0.dev1/tet/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/config/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     8526 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/config/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/decorators/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1620 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/decorators/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/i18n/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2028 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/i18n/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/interface/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1560 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/interface/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/renderers/
--rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/renderers/__init__.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1812 2017-08-29 07:24:56.000000 tet-0.4.0.dev1/tet/renderers/json.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      278 2017-08-29 07:27:58.000000 tet-0.4.0.dev1/tet/renderers/tonnikala.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)       31 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/request.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)       32 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/response.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/security/
--rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/security/__init__.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2248 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/security/authorization.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      141 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/security/csrf.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/services/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     4507 2021-03-19 14:29:29.000000 tet-0.4.0.dev1/tet/services/__init__.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      298 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/session.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/sqlalchemy/
--rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/sqlalchemy/__init__.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      397 2017-08-29 07:26:17.000000 tet-0.4.0.dev1/tet/sqlalchemy/factory.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      801 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/sqlalchemy/password.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)     4968 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/sqlalchemy/simple.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/static/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1934 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/static/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet/util/
--rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/util/__init__.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2112 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/base64.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      445 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/collections.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      539 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/crypt.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      262 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/export.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      356 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/util/json.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      737 2017-08-29 07:25:11.000000 tet-0.4.0.dev1/tet/util/path.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1355 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/util/pshell.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/tet/view/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2245 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/view/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/tet/viewlet/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     1401 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/viewlet/__init__.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.608541 tet-0.4.0.dev1/tet/zodb/
--rw-r--r--   0 ztane     (1000) ztane     (1000)        0 2017-08-28 17:32:26.000000 tet-0.4.0.dev1/tet/zodb/__init__.py
--rw-r--r--   0 ztane     (1000) ztane     (1000)      413 2021-03-19 14:29:27.000000 tet-0.4.0.dev1/tet/zodb/password.py
-drwxr-xr-x   0 ztane     (1000) ztane     (1000)        0 2021-03-19 14:33:07.604541 tet-0.4.0.dev1/tet.egg-info/
--rw-r--r--   0 ztane     (1000) ztane     (1000)     2525 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/PKG-INFO
--rw-r--r--   0 ztane     (1000) ztane     (1000)      907 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/SOURCES.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)        1 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/dependency_links.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)        1 2017-08-29 07:32:39.000000 tet-0.4.0.dev1/tet.egg-info/not-zip-safe
--rw-r--r--   0 ztane     (1000) ztane     (1000)       49 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/requires.txt
--rw-r--r--   0 ztane     (1000) ztane     (1000)        4 2021-03-19 14:33:07.000000 tet-0.4.0.dev1/tet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 12:45:59.000000 tet-0.4.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-01 12:45:59.000000 tet-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 12:45:59.000000 tet-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-01 12:46:05.047245 tet-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 12:45:59.000000 tet-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 12:46:05.051245 tet-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-01 12:45:59.000000 tet-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.043244 tet-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 12:45:59.000000 tet-0.4.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.043244 tet-0.4.1/tet/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 12:45:59.000000 tet-0.4.1/tet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-04-01 12:45:59.000000 tet-0.4.1/tet/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-01 12:45:59.000000 tet-0.4.1/tet/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-01 12:45:59.000000 tet-0.4.1/tet/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 12:45:59.000000 tet-0.4.1/tet/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 12:45:59.000000 tet-0.4.1/tet/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-01 12:45:59.000000 tet-0.4.1/tet/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 12:45:59.000000 tet-0.4.1/tet/renderers/tonnikala.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 12:45:59.000000 tet-0.4.1/tet/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 12:45:59.000000 tet-0.4.1/tet/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 12:45:59.000000 tet-0.4.1/tet/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-01 12:45:59.000000 tet-0.4.1/tet/security/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 12:45:59.000000 tet-0.4.1/tet/security/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 12:45:59.000000 tet-0.4.1/tet/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 12:45:59.000000 tet-0.4.1/tet/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 12:45:59.000000 tet-0.4.1/tet/sqlalchemy/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 12:45:59.000000 tet-0.4.1/tet/sqlalchemy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-01 12:45:59.000000 tet-0.4.1/tet/sqlalchemy/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-01 12:45:59.000000 tet-0.4.1/tet/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-01 12:45:59.000000 tet-0.4.1/tet/util/pshell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-01 12:45:59.000000 tet-0.4.1/tet/view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet/viewlet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-01 12:45:59.000000 tet-0.4.1/tet/viewlet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:46:05.047245 tet-0.4.1/tet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-01 12:46:05.000000 tet-0.4.1/tet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 12:46:05.000000 tet-0.4.1/tet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:46:05.000000 tet-0.4.1/tet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:46:04.000000 tet-0.4.1/tet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 12:46:05.000000 tet-0.4.1/tet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 12:46:05.000000 tet-0.4.1/tet.egg-info/top_level.txt
```

### Comparing `tet-0.4.0.dev1/PKG-INFO` & `tet-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tet
-Version: 0.4.0.dev1
+Version: 0.4.1
 Summary: Unearthly intelligent batteries-included application framework built on Pyramid
 Home-page: http://www.anttipatterns.com
 Author: Antti Haapala
 Author-email: antti.haapala@anttipatterns.com
-License: UNKNOWN
-Description: tet
-        ===
-        
-        Unearthly intelligent batteries-included application framework built on Pyramid
-        
-        
-        How to install
-        --------------
-        
-            git clone https://github.com/ztane/tet.git
-            cd tet
-            python setup.py develop
-        
-        
-        What do you get out of the box
-        ------------------------------
-        
-        1. Awesome scaffold(s):
-        
-                pcreate -s basictet MyProject
-                cd MyProject
-                python setup.py develop
-                initialize_myproject_db development.ini
-                # go to http://localhost://6543 and feel awesome
-        
-        
-        2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-        
-            * The tet.di request scoped services are now truly instantiated per request!
-        
-        2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-        
-            * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
-              fixed backports.typing to greater than or equal to 1.1.
-        
-        2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
-        
-            * renamed the package to `tet`
-        
-        
 Keywords: web wsgi bfg pylons pyramid
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE
+Requires-Dist: pyramid>=1.9
+Requires-Dist: passlib
+Requires-Dist: sqlalchemy
+Requires-Dist: pyramid_di
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+
+# tet
+
+Unearthly intelligent batteries-included application framework built on Pyramid
+
+
+## How to install
+
+```
+pip install tet
+```
+
+
+# Changes
+
+
+2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+
+    * The tet.di request scoped services are now truly instantiated per request!
+
+2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+
+    * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
+      fixed backports.typing to greater than or equal to 1.1.
+
+2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
+
+    * renamed the package to `tet`
+
```

### Comparing `tet-0.4.0.dev1/setup.py` & `tet-0.4.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-import os, sys
+from pathlib import Path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-here = os.path.abspath(os.path.dirname(__file__))
+here = Path(__file__).parent
+README = (here / "README.md").read_text()
+CHANGES = (here / "CHANGES.md").read_text()
 
-def readfile(name):
-    with open(os.path.join(here, name)) as f:
-        return f.read()
-
-README = readfile('README.txt')
-CHANGES = readfile('CHANGES.txt')
 
 requires = """
     pyramid>=1.9
     passlib
     sqlalchemy
-    pyramid_services
+    pyramid_di
 """.split()
 
-if sys.version_info < (3, 5, 2):
-    requires.append('backports.typing>=1.1,<1.2')
-
+dev_requires = ["pytest"]
 
-setup(name='tet',
-      version='0.4.0.dev1',
-      description='Unearthly intelligent batteries-included application framework built on Pyramid',
-      long_description=README + '\n\n' + CHANGES,
-      classifiers=[
-          "Development Status :: 4 - Beta",
-          "Framework :: Pyramid",
-          "Intended Audience :: Developers",
-          "License :: OSI Approved :: Python Software Foundation License",
-          "Programming Language :: Python :: 3.3",
-          "Programming Language :: Python :: 3.4",
-          "Programming Language :: Python :: 3.5",
-          "Programming Language :: Python :: 3.6",
-          "Programming Language :: Python :: 3.7",
-          "Programming Language :: Python :: 3.8",
-          "Programming Language :: Python :: 3.9",
-          "Programming Language :: Python :: 3.10",
-          "Programming Language :: Python :: 3 :: Only",
-          "Topic :: Internet :: WWW/HTTP :: WSGI",
-          "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
-          "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
-          "Topic :: Software Development :: Libraries :: Application Frameworks"
-      ],
-      author='Antti Haapala',
-      author_email='antti.haapala@anttipatterns.com',
-      url='http://www.anttipatterns.com',
-      keywords='web wsgi bfg pylons pyramid',
-      packages=find_packages(),
-      include_package_data=True,
-      zip_safe=False,
-      test_suite='tet',
-      install_requires=requires,
+setup(
+    name="tet",
+    version="0.4.1",
+    description="Unearthly intelligent batteries-included application framework built on Pyramid",
+    long_description=README + "\n\n" + CHANGES,
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Framework :: Pyramid",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Python Software Foundation License",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Internet :: WWW/HTTP :: WSGI",
+        "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
+        "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+    ],
+    author="Antti Haapala",
+    author_email="antti.haapala@anttipatterns.com",
+    url="http://www.anttipatterns.com",
+    keywords="web wsgi bfg pylons pyramid",
+    packages=find_packages(),
+    include_package_data=True,
+    zip_safe=False,
+    test_suite="tet",
+    install_requires=requires,
+    extras_require={"dev": dev_requires},
 )
```

### Comparing `tet-0.4.0.dev1/tet/config/__init__.py` & `tet-0.4.1/tet/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Callable, Any
-
 import sys
-
 from collections import ChainMap
 from collections.abc import Mapping
 from functools import wraps
-from pyramid.config import *
+from typing import Any, Callable
 
+from pyramid.config import *
 from pyramid.config import Configurator
+
 from tet.decorators import deprecated
 from tet.i18n import configure_i18n
 from tet.util.collections import flatten
 from tet.util.path import caller_package
 
 
 class TetAppFactory(object):
@@ -27,18 +26,15 @@
     i18n = True
     default_i18n_domain = None
     settings = {}
     global_config = None
 
     # :type config: Configurator
     config = None
-    default_includes = [
-        'tet.services',
-        'tet.renderers.json'
-    ]
+    default_includes = ["tet.renderers.json"]
 
     @deprecated
     def __new__(cls, global_config, **settings_kw):
         instance = cls.instantiate()
         instance.init_app_factory(global_config, settings_kw)
         return instance.construct_app()
 
@@ -116,86 +112,87 @@
     @classmethod
     @deprecated
     def main(cls, global_config, **settings):
         return cls(global_config, **settings)
 
 
 ALL_FEATURES = [
-    'services',
-    'i18n',
-    'renderers.json',
-    'renderers.tonnikala',
-    'renderers.tonnikala.i18n',
-    'security.authorization',
-    'security.csrf'
+    "services",
+    "i18n",
+    "renderers.json",
+    "renderers.tonnikala",
+    "renderers.tonnikala.i18n",
+    "security.authorization",
+    "security.csrf",
 ]
 
 MINIMAL_FEATURES = []
 
 
-def create_configurator(*,
-                        global_config=None,
-                        settings=None,
-                        merge_global_config=True,
-                        configurator_class=Configurator,
-                        included_features=(),
-                        excluded_features=(),
-                        package=None,
-                        **kw) -> Configurator:
-
+def create_configurator(
+    *,
+    global_config=None,
+    settings=None,
+    merge_global_config=True,
+    configurator_class=Configurator,
+    included_features=(),
+    excluded_features=(),
+    package=None,
+    **kw
+) -> Configurator:
     defaults = {}
     if merge_global_config and isinstance(global_config, Mapping):
         settings = ChainMap(settings, global_config, defaults)
 
     extracted_settings = {}
 
     if package is None:
         package = caller_package(ignored_modules=[__name__])
 
-    for name in ['default_i18n_domain']:
+    for name in ["default_i18n_domain"]:
         if name in kw:
             extracted_settings[name] = kw.pop(name)
 
-    if hasattr(package, '__name__'):
+    if hasattr(package, "__name__"):
         package_name = package.__name__
     else:
         package_name = package
 
-    defaults['default_i18n_domain'] = package_name
+    defaults["default_i18n_domain"] = package_name
 
-    config = configurator_class(settings=settings,
-                                package=package,
-                                **kw)
+    config = configurator_class(settings=settings, package=package, **kw)
     config.add_settings(extracted_settings)
     included_features = list(flatten(included_features))
     excluded_features = set(flatten(excluded_features))
 
     feature_set = set(included_features) - set(excluded_features)
     config.registry.tet_features = feature_set
 
     for feature_name in included_features:
         if feature_name in feature_set:
             try:
-                config.include('tet.' + feature_name)
+                config.include("tet." + feature_name)
             except Exception as e:
-                print('Unable to include feature {}: {}'.format(
-                    feature_name,
-                    e
-                ), file=sys.stderr)
+                print(
+                    "Unable to include feature {}: {}".format(feature_name, e),
+                    file=sys.stderr,
+                )
                 raise
 
     return config
 
 
-def application_factory(factory_function: Callable[[Configurator], Any]=None,
-                        configure_only=False,
-                        included_features=ALL_FEATURES,
-                        excluded_features=(),
-                        package=None,
-                        **extra_parameters):
+def application_factory(
+    factory_function: Callable[[Configurator], Any] = None,
+    configure_only=False,
+    included_features=MINIMAL_FEATURES,
+    excluded_features=(),
+    package=None,
+    **extra_parameters
+):
     """
     A decorator for main method / application configurator for Tet. The
     wrapped function must accept a single argument - the Configurator. The
     wrapper itself accepts arguments (global_config, **settings) like an
     ordinary Pyramid/Paster application entry point does.
 
     If configure_only=False (the default), then the return value is a
@@ -232,25 +229,29 @@
     if package is None:
         package = caller_package(ignored_modules=[__name__])
 
     def decorator(function):
         @wraps(function)
         def wrapper(*a, **kw):
             if len(a) > 1:
-                raise TypeError('application_factory wrapped function '
-                                'called with more than 1 positional argument')
+                raise TypeError(
+                    "application_factory wrapped function "
+                    "called with more than 1 positional argument"
+                )
 
             global_config = a[0] if a else None
             settings = kw
-            config = create_configurator(global_config=global_config,
-                                         settings=settings,
-                                         included_features=included_features,
-                                         excluded_features=excluded_features,
-                                         package=package,
-                                         **extra_parameters)
+            config = create_configurator(
+                global_config=global_config,
+                settings=settings,
+                included_features=included_features,
+                excluded_features=excluded_features,
+                package=package,
+                **extra_parameters
+            )
 
             returned = function(config)
             if isinstance(returned, Configurator):
                 config = returned
 
             if not configure_only:
                 return config.make_wsgi_app()
```

### Comparing `tet-0.4.0.dev1/tet/decorators/__init__.py` & `tet-0.4.1/tet/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/i18n/__init__.py` & `tet-0.4.1/tet/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/interface/__init__.py` & `tet-0.4.1/tet/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/renderers/json.py` & `tet-0.4.1/tet/renderers/json.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/security/authorization.py` & `tet-0.4.1/tet/security/authorization.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/sqlalchemy/password.py` & `tet-0.4.1/tet/sqlalchemy/password.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/sqlalchemy/simple.py` & `tet-0.4.1/tet/sqlalchemy/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from typing import Type, Any, Optional
+from typing import Any, Optional
 
-import tet.services
 from pyramid.config import Configurator
+from pyramid.request import Request
+from zope.interface import Interface
 
 # Recommended naming convention used by Alembic, as various different database
 # providers will autogenerate vastly different names making migrations more
 # difficult. See: http://alembic.zzzcomputing.com/en/latest/naming.html
-from pyramid.request import Request
-from zope.interface import Interface
-
 DEFAULT_NAMING_CONVENTION = {
-    "ix": 'ix_%(column_0_label)s',
+    "ix": "ix_%(column_0_label)s",
     "uq": "uq_%(table_name)s_%(column_0_name)s",
     "ck": "ck_%(table_name)s_%(constraint_name)s",
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
-    "pk": "pk_%(table_name)s"
+    "pk": "pk_%(table_name)s",
 }
 
 _NOT_SET = object()
 
 
-def declarative_base(*,
-                     metadata=_NOT_SET,
-                     naming_convention=_NOT_SET) -> Any:
+def declarative_base(*, metadata=_NOT_SET, naming_convention=_NOT_SET) -> Any:
     """
     Create a declarative base, using the given naming convention, defaulting
     to the DEFAULT_NAMING_CONVENTION of this module
 
     :return: the newly created declarative_base
     """
     from sqlalchemy.ext.declarative import declarative_base
@@ -53,89 +49,89 @@
           import transaction
           engine = get_engine(settings)
           session_factory = get_session_factory(engine)
           with transaction.manager:
               dbsession = get_tm_session(session_factory, transaction.manager)
     """
     import zope.sqlalchemy
+
     dbsession = session_factory()
-    zope.sqlalchemy.register(
-        dbsession, transaction_manager=transaction_manager)
+    zope.sqlalchemy.register(dbsession, transaction_manager=transaction_manager)
     return dbsession
 
 
-def setup_sqlalchemy(config: Configurator,
-                     *,
-                     settings: Optional[dict] =_NOT_SET,
-                     prefix: str ='sqlalchemy.',
-                     engine: Optional['sqlalchemy.Engine'] =_NOT_SET,
-                     name: str='') -> None:
-
+def setup_sqlalchemy(
+    config: Configurator,
+    *,
+    settings: Optional[dict] = _NOT_SET,
+    prefix: str = "sqlalchemy.",
+    engine: Optional["sqlalchemy.Engine"] = _NOT_SET,
+    name: str = ""
+) -> None:
     """
     Sets up SQLAlchemy, creating a request scoped service for the ORM session.
     Include all models before calling this configurator.
 
     :param config: the configurator
     :param base: The declarative base class. Required
     :param settings: Optional settings dictionary for the engine creation
     :param prefix: Optional settings prefix for the engine settings
     :param engine: The engine to use - if specified, settings must not be
                 given, or vice versa
     :param name: the alternate name for which to bind the session service
     """
 
     from sqlalchemy import engine_from_config
-    from sqlalchemy.orm import sessionmaker, Session, configure_mappers, scoped_session
+    from sqlalchemy.orm import Session, configure_mappers, scoped_session, sessionmaker
 
     if settings is not _NOT_SET:
         if engine is not _NOT_SET:
-            raise ValueError('Only one of settings, '
-                             'engine may be specified')
+            raise ValueError("Only one of settings, engine may be specified")
     else:
         settings = config.registry.settings
 
     if engine is _NOT_SET:
         engine = engine_from_config(settings, prefix)
 
     session_factory = sessionmaker()
     session_factory.configure(bind=engine)
 
-    if 'tet.sqlalchemy.simple.factories' not in config.registry:
-        config.registry['tet.sqlalchemy.simple.factories' ] = {}
+    if "tet.sqlalchemy.simple.factories" not in config.registry:
+        config.registry["tet.sqlalchemy.simple.factories"] = {}
 
-    config.registry['tet.sqlalchemy.simple.factories'][name] = session_factory
+    config.registry["tet.sqlalchemy.simple.factories"][name] = session_factory
 
     def _session_service(context: Any, request: Request):
         return get_tm_session(session_factory, request.tm)
 
-    config.register_service_factory(
-        _session_service, Session, Interface, name=name)
+    config.register_service_factory(_session_service, Session, Interface, name=name)
 
     config.register_service(
         scoped_session(session_factory),
-        name='scoped_session' + (':' + name if name else '')
+        name="scoped_session" + (":" + name if name else ""),
     )
 
-    config.action('tet.sqlalchemy.simple.configure_mappers', configure_mappers)
+    config.action("tet.sqlalchemy.simple.configure_mappers", configure_mappers)
 
 
 def includeme(config: Configurator) -> None:
     """
     Include the simple SQLAlchemy configuration with reasonable defaults.
 
     :param config: the configurator
     """
     try:
         import sqlalchemy
     except ImportError as e:
-        raise RuntimeError('sqlalchemy cannot be imported, '
-                           'unable to include tet.sqlalchemy.simple') from e
+        raise RuntimeError(
+            "sqlalchemy cannot be imported, unable to include tet.sqlalchemy.simple"
+        ) from e
 
-    config.include('pyramid_services')
+    config.include("pyramid_di")
 
     settings = config.get_settings()
-    settings['tm.manager_hook'] = 'pyramid_tm.explicit_manager'
+    settings["tm.manager_hook"] = "pyramid_tm.explicit_manager"
 
     # use pyramid_tm to hook the transaction lifecycle to the request
-    config.include('pyramid_tm')
+    config.include("pyramid_tm")
 
-    config.add_directive('setup_sqlalchemy', setup_sqlalchemy)
+    config.add_directive("setup_sqlalchemy", setup_sqlalchemy)
```

### Comparing `tet-0.4.0.dev1/tet/static/__init__.py` & `tet-0.4.1/tet/static/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/util/base64.py` & `tet-0.4.1/tet/util/base64.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/util/crypt.py` & `tet-0.4.1/tet/util/crypt.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/util/path.py` & `tet-0.4.1/tet/util/path.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/util/pshell.py` & `tet-0.4.1/tet/util/pshell.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet/view/__init__.py` & `tet-0.4.1/tet/view/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 from inspect import isclass
 
 from pyramid.request import Request
 from pyramid.view import *
 from pyramid.view import view_config as _pyramid_view_config
-from tet.services import RequestScopedBaseService
+from pyramid_di import RequestScopedBaseService
 
 
 class view_config(_pyramid_view_config):
     def __init__(self, **settings):
         super(view_config, self).__init__(**settings)
 
 
 class expose(object):
-    """
-    """
+    """ """
 
     venusian = venusian
 
     def __init__(self, **settings):
         self.__dict__.update(settings)
 
     def __call__(self, wrapped):
         settings = self.__dict__.copy()
 
         def callback(context, name, ob):
             config = context.config.with_package(info.module)
 
             name = attr_name
-            if name == 'index':
-                name = ''
+            if name == "index":
+                name = ""
 
             def view_wrapper(request):
                 # TODO: should we stack the request?
                 return getattr(request.context, attr_name)()
 
             config.add_view(view=view_wrapper, name=name, context=ob, **settings)
 
-        info = self.venusian.attach(wrapped, callback, category='pyramid')
+        info = self.venusian.attach(wrapped, callback, category="pyramid")
 
-        if info.scope != 'class':
+        if info.scope != "class":
             # if the decorator was attached to a method in a class, or
             # otherwise executed at class scope, we need to set an
             # 'attr' into the settings if one isn't already in there
             raise ValueError("expose can be only applied to instance methods!")
 
         attr_name = wrapped.__name__
 
-        settings['_info'] = info.codeinfo # fbo "action_method"
+        settings["_info"] = info.codeinfo  # fbo "action_method"
         return wrapped
 
 
 class BaseController(object):
     def __getitem__(self, name):
-        if hasattr(self, '_lookup'):
+        if hasattr(self, "_lookup"):
             try:
                 return self._lookup(name)
             except KeyError:
                 pass
 
         child_controller = getattr(self, name, None)
         if isclass(child_controller) and issubclass(child_controller, BaseController):
@@ -67,8 +66,8 @@
 
         raise KeyError("Child not found: %s" % name)
 
 
 class ServiceViews(RequestScopedBaseService):
     def __init__(self, request: Request):
         super().__init__(request=request)
-        self.context = getattr(request, 'context', None)
+        self.context = getattr(request, "context", None)
```

### Comparing `tet-0.4.0.dev1/tet/viewlet/__init__.py` & `tet-0.4.1/tet/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `tet-0.4.0.dev1/tet.egg-info/PKG-INFO` & `tet-0.4.1/tet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tet
-Version: 0.4.0.dev1
+Version: 0.4.1
 Summary: Unearthly intelligent batteries-included application framework built on Pyramid
 Home-page: http://www.anttipatterns.com
 Author: Antti Haapala
 Author-email: antti.haapala@anttipatterns.com
-License: UNKNOWN
-Description: tet
-        ===
-        
-        Unearthly intelligent batteries-included application framework built on Pyramid
-        
-        
-        How to install
-        --------------
-        
-            git clone https://github.com/ztane/tet.git
-            cd tet
-            python setup.py develop
-        
-        
-        What do you get out of the box
-        ------------------------------
-        
-        1. Awesome scaffold(s):
-        
-                pcreate -s basictet MyProject
-                cd MyProject
-                python setup.py develop
-                initialize_myproject_db development.ini
-                # go to http://localhost://6543 and feel awesome
-        
-        
-        2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-        
-            * The tet.di request scoped services are now truly instantiated per request!
-        
-        2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
-        
-            * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
-              fixed backports.typing to greater than or equal to 1.1.
-        
-        2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
-        
-            * renamed the package to `tet`
-        
-        
 Keywords: web wsgi bfg pylons pyramid
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE
+Requires-Dist: pyramid>=1.9
+Requires-Dist: passlib
+Requires-Dist: sqlalchemy
+Requires-Dist: pyramid_di
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+
+# tet
+
+Unearthly intelligent batteries-included application framework built on Pyramid
+
+
+## How to install
+
+```
+pip install tet
+```
+
+
+# Changes
+
+
+2021-03-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+
+    * The tet.di request scoped services are now truly instantiated per request!
+
+2016-08-19  Antti Haapala  <antti.haapala@anttipatterns.com>
+
+    * SQLAlchemy root factory now gives NotFound on DataError; made into a implicit-namespace package;
+      fixed backports.typing to greater than or equal to 1.1.
+
+2013-09-07  Antti Haapala  <antti.haapala@anttipatterns.com>
+
+    * renamed the package to `tet`
+
```

