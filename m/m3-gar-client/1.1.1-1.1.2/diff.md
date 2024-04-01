# Comparing `tmp/m3-gar-client-1.1.1.tar.gz` & `tmp/m3-gar-client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-gar-client-1.1.1.tar", last modified: Sat Mar 30 11:52:07 2024, max compression
+gzip compressed data, was "m3-gar-client-1.1.2.tar", last modified: Mon Apr  1 09:35:07 2024, max compression
```

## Comparing `m3-gar-client-1.1.1.tar` & `m3-gar-client-1.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.164737 m3-gar-client-1.1.1/
--rw-r--r--   0 toor      (1000) toor      (1000)      565 2021-10-28 11:22:58.000000 m3-gar-client-1.1.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      153 2021-10-28 11:22:58.000000 m3-gar-client-1.1.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5486 2024-03-30 11:52:07.163737 m3-gar-client-1.1.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4056 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.146737 m3-gar-client-1.1.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)      497 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/requirements/_base.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2021-10-28 11:22:58.000000 m3-gar-client-1.1.1/requirements/prod.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-03-30 11:52:07.164737 m3-gar-client-1.1.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2619 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.143737 m3-gar-client-1.1.1/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.147737 m3-gar-client-1.1.1/src/m3_gar_client/
--rw-r--r--   0 toor      (1000) toor      (1000)     1163 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      446 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.150737 m3-gar-client-1.1.1/src/m3_gar_client/backends/
--rw-r--r--   0 toor      (1000) toor      (1000)       70 2021-10-28 11:22:58.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5336 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.151737 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/
--rw-r--r--   0 toor      (1000) toor      (1000)      127 2021-10-28 11:22:58.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4925 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.152737 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy/
--rw-r--r--   0 toor      (1000) toor      (1000)     2043 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4244 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.154737 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/
--rw-r--r--   0 toor      (1000) toor      (1000)     1762 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      480 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/authentication.py
--rw-r--r--   0 toor      (1000) toor      (1000)      198 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/const.py
--rw-r--r--   0 toor      (1000) toor      (1000)      694 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3310 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9941 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/server.py
--rw-r--r--   0 toor      (1000) toor      (1000)    34886 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)    24834 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/data.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.154737 m3-gar-client-1.1.1/src/m3_gar_client/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.1.1/src/m3_gar_client/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.155737 m3-gar-client-1.1.1/src/m3_gar_client/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.1.1/src/m3_gar_client/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      454 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/management/commands/clear_gar_cache.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.142737 m3-gar-client-1.1.1/src/m3_gar_client/static/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.143737 m3-gar-client-1.1.1/src/m3_gar_client/static/m3/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.143737 m3-gar-client-1.1.1/src/m3_gar_client/static/m3/js/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.156737 m3-gar-client-1.1.1/src/m3_gar_client/static/m3/js/gar/
--rw-r--r--   0 toor      (1000) toor      (1000)    37035 2024-03-18 09:04:10.000000 m3-gar-client-1.1.1/src/m3_gar_client/static/m3/js/gar/AddressPanel.js
--rw-r--r--   0 toor      (1000) toor      (1000)     6454 2024-03-18 09:04:10.000000 m3-gar-client-1.1.1/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js
--rw-r--r--   0 toor      (1000) toor      (1000)    27594 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12473 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/m3_gar_client/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.161737 m3-gar-client-1.1.1/src/m3_gar_client.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5486 2024-03-30 11:52:07.000000 m3-gar-client-1.1.1/src/m3_gar_client.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1636 2024-03-30 11:52:07.000000 m3-gar-client-1.1.1/src/m3_gar_client.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-03-30 11:52:07.000000 m3-gar-client-1.1.1/src/m3_gar_client.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      175 2024-03-30 11:52:07.000000 m3-gar-client-1.1.1/src/m3_gar_client.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2024-03-30 11:52:07.000000 m3-gar-client-1.1.1/src/m3_gar_client.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.159737 m3-gar-client-1.1.1/src/testapp/
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      399 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/asgi.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)      688 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/manage.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3498 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:07.160737 m3-gar-client-1.1.1/src/testapp/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/tests/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2090 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/tests/test_backend_responses.py
--rw-r--r--   0 toor      (1000) toor      (1000)      988 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/tests/test_defaults.py
--rw-r--r--   0 toor      (1000) toor      (1000)      768 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/urls.py
--rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-03-30 11:52:02.000000 m3-gar-client-1.1.1/src/testapp/wsgi.py
--rw-r--r--   0 toor      (1000) toor      (1000)      448 2024-03-30 11:52:07.000000 m3-gar-client-1.1.1/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.125061 m3-gar-client-1.1.2/
+-rw-r--r--   0 toor      (1000) toor      (1000)      565 2021-10-28 11:22:58.000000 m3-gar-client-1.1.2/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      153 2021-10-28 11:22:58.000000 m3-gar-client-1.1.2/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5666 2024-04-01 09:35:07.124061 m3-gar-client-1.1.2/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     4056 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.102061 m3-gar-client-1.1.2/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)      497 2024-04-01 09:35:01.000000 m3-gar-client-1.1.2/requirements/_base.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2021-10-28 11:22:58.000000 m3-gar-client-1.1.2/requirements/prod.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-01 09:35:07.125061 m3-gar-client-1.1.2/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2795 2024-04-01 09:35:01.000000 m3-gar-client-1.1.2/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.100061 m3-gar-client-1.1.2/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.104061 m3-gar-client-1.1.2/src/m3_gar_client/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1163 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      446 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.106061 m3-gar-client-1.1.2/src/m3_gar_client/backends/
+-rw-r--r--   0 toor      (1000) toor      (1000)       70 2021-10-28 11:22:58.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5336 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.109061 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/
+-rw-r--r--   0 toor      (1000) toor      (1000)      127 2021-10-28 11:22:58.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4925 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.110061 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2043 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4244 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.112061 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1762 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      480 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/authentication.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      198 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      694 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3310 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9941 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/server.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    34906 2024-04-01 09:35:01.000000 m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    24834 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/data.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.112061 m3-gar-client-1.1.2/src/m3_gar_client/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.1.2/src/m3_gar_client/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.113061 m3-gar-client-1.1.2/src/m3_gar_client/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 09:04:10.000000 m3-gar-client-1.1.2/src/m3_gar_client/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      454 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/management/commands/clear_gar_cache.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.099061 m3-gar-client-1.1.2/src/m3_gar_client/static/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.099061 m3-gar-client-1.1.2/src/m3_gar_client/static/m3/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.099061 m3-gar-client-1.1.2/src/m3_gar_client/static/m3/js/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.115061 m3-gar-client-1.1.2/src/m3_gar_client/static/m3/js/gar/
+-rw-r--r--   0 toor      (1000) toor      (1000)    37035 2024-03-18 09:04:10.000000 m3-gar-client-1.1.2/src/m3_gar_client/static/m3/js/gar/AddressPanel.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     6454 2024-03-18 09:04:10.000000 m3-gar-client-1.1.2/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js
+-rw-r--r--   0 toor      (1000) toor      (1000)    27594 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12473 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/m3_gar_client/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.121061 m3-gar-client-1.1.2/src/m3_gar_client.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5666 2024-04-01 09:35:07.000000 m3-gar-client-1.1.2/src/m3_gar_client.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1636 2024-04-01 09:35:07.000000 m3-gar-client-1.1.2/src/m3_gar_client.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-04-01 09:35:07.000000 m3-gar-client-1.1.2/src/m3_gar_client.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      177 2024-04-01 09:35:07.000000 m3-gar-client-1.1.2/src/m3_gar_client.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       14 2024-04-01 09:35:07.000000 m3-gar-client-1.1.2/src/m3_gar_client.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.119061 m3-gar-client-1.1.2/src/testapp/
+-rw-r--r--   0 toor      (1000) toor      (1000)       50 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      399 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/asgi.py
+-rwxr-xr-x   0 toor      (1000) toor      (1000)      688 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/manage.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3498 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-01 09:35:07.120061 m3-gar-client-1.1.2/src/testapp/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2090 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/tests/test_backend_responses.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      988 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/tests/test_defaults.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      768 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/urls.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      401 2024-03-30 11:52:02.000000 m3-gar-client-1.1.2/src/testapp/wsgi.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-04-01 09:35:07.000000 m3-gar-client-1.1.2/version.conf
```

### Comparing `m3-gar-client-1.1.1/LICENSE` & `m3-gar-client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/PKG-INFO` & `m3-gar-client-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: m3-gar-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: UI клиент для сервера ГАР m3-rest-gar
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-gar-client
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3,>=2
-Requires-Dist: django<5.1,>=3.2
+Requires-Dist: django<5.1,>=2.2
 Requires-Dist: m3-gar-constants>=1.0.3
 Provides-Extra: oauth2
-Requires-Dist: oauthlib<3,>=2; extra == "oauth2"
+Requires-Dist: oauthlib<3.3,>=2; extra == "oauth2"
 Requires-Dist: requests-oauthlib<=1.3.1; extra == "oauth2"
 Provides-Extra: m3
 Requires-Dist: m3-core<4,>=2.2.16; extra == "m3"
 Requires-Dist: m3-ui<3,>=2.0.8; extra == "m3"
 Provides-Extra: rest
 Requires-Dist: djangorestframework; extra == "rest"
```

### Comparing `m3-gar-client-1.1.1/README.rst` & `m3-gar-client-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/setup.py` & `m3-gar-client-1.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,29 +56,33 @@
     include_package_data=True,
     classifiers=[
         'Intended Audience :: Developers',
         'Environment :: Web Environment',
         'Natural Language :: Russian',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Development Status :: 5 - Production/Stable',
+        'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
         'Framework :: Django :: 4.2',
         'Framework :: Django :: 5.0',
     ],
     install_requires=tuple(_get_requirements('requirements/prod.txt')),
     extras_require={
         'oauth2': (
-            'oauthlib>=2,<3',
+            'oauthlib>=2,<3.3',
             'requests-oauthlib<=1.3.1',
         ),
         'm3': (
             'm3-core>=2.2.16,<4',
             'm3-ui>=2.0.8,<3'
         ),
         'rest': (
```

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/__init__.py` & `m3-gar-client-1.1.2/src/m3_gar_client/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/base.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/base.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/base.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy/actions.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/urls.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/proxy_rest/views.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/server.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/server.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/backends/m3_rest_gar/utils.py` & `m3-gar-client-1.1.2/src/m3_gar_client/backends/m3_rest_gar/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,18 +248,21 @@
 
     Предназначена для использования в UI.
     """
 
     @staticmethod
     def _get_display_name(drf_object_data):
         apartment_number = drf_object_data.get('number')
-        if apart_type := drf_object_data.get('aparttype__shortname'):
+        apart_type = drf_object_data.get('aparttype__shortname')
+
+        if apart_type:
             full_name = f'{apart_type} {apartment_number}'
         else:
             full_name = apartment_number
+
         return full_name
 
     fields_map = {
         'objectId': 'objectguid',
         'number': 'number',
         'apartType': 'aparttype__shortname',
         'displayName': _get_display_name,
```

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/data.py` & `m3-gar-client-1.1.2/src/m3_gar_client/data.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/static/m3/js/gar/AddressPanel.js` & `m3-gar-client-1.1.2/src/m3_gar_client/static/m3/js/gar/AddressPanel.js`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js` & `m3-gar-client-1.1.2/src/m3_gar_client/static/m3/js/gar/AddressPanelPatch.js`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/ui.py` & `m3-gar-client-1.1.2/src/m3_gar_client/ui.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client/utils.py` & `m3-gar-client-1.1.2/src/m3_gar_client/utils.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client.egg-info/PKG-INFO` & `m3-gar-client-1.1.2/src/m3_gar_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: m3-gar-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: UI клиент для сервера ГАР m3-rest-gar
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3-gar-client
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests<3,>=2
-Requires-Dist: django<5.1,>=3.2
+Requires-Dist: django<5.1,>=2.2
 Requires-Dist: m3-gar-constants>=1.0.3
 Provides-Extra: oauth2
-Requires-Dist: oauthlib<3,>=2; extra == "oauth2"
+Requires-Dist: oauthlib<3.3,>=2; extra == "oauth2"
 Requires-Dist: requests-oauthlib<=1.3.1; extra == "oauth2"
 Provides-Extra: m3
 Requires-Dist: m3-core<4,>=2.2.16; extra == "m3"
 Requires-Dist: m3-ui<3,>=2.0.8; extra == "m3"
 Provides-Extra: rest
 Requires-Dist: djangorestframework; extra == "rest"
```

### Comparing `m3-gar-client-1.1.1/src/m3_gar_client.egg-info/SOURCES.txt` & `m3-gar-client-1.1.2/src/m3_gar_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/testapp/manage.py` & `m3-gar-client-1.1.2/src/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/testapp/settings.py` & `m3-gar-client-1.1.2/src/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/testapp/tests/test_backend_responses.py` & `m3-gar-client-1.1.2/src/testapp/tests/test_backend_responses.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/testapp/tests/test_defaults.py` & `m3-gar-client-1.1.2/src/testapp/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `m3-gar-client-1.1.1/src/testapp/urls.py` & `m3-gar-client-1.1.2/src/testapp/urls.py`

 * *Files identical despite different names*

