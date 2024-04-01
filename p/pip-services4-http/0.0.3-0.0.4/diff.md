# Comparing `tmp/pip_services4_http-0.0.3.tar.gz` & `tmp/pip_services4_http-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_http-0.0.3.tar", last modified: Wed Nov  8 17:27:14 2023, max compression
+gzip compressed data, was "pip_services4_http-0.0.4.tar", last modified: Mon Apr  1 19:30:17 2024, max compression
```

## Comparing `pip_services4_http-0.0.3.tar` & `pip_services4_http-0.0.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.701514 pip_services4_http-0.0.3/pip_services4_http/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.701514 pip_services4_http-0.0.3/pip_services4_http/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/auth/BasicAuthorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/auth/OwnerAuthorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/auth/RoleAuthorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.705514 pip_services4_http-0.0.3/pip_services4_http/build/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/build/DefaultRpcFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.705514 pip_services4_http-0.0.3/pip_services4_http/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/clients/CommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/clients/RestClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.705514 pip_services4_http-0.0.3/pip_services4_http/connect/
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/connect/HttpConnectionResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/pip_services4_http/controller/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/AboutOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/CommandableHttpController.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/CommandableSwaggerDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/HeartBeatOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/HeartbeatRestController.py
--rw-r--r--   0 runner    (1001) docker     (127)    17787 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/HttpEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/HttpRequestDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/HttpResponseSender.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/IRegisterable.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/ISwaggerController.py
--rw-r--r--   0 runner    (1001) docker     (127)    16444 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/RestController.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/RestOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/RestQueryParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/SSLCherryPyServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/StatusOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/StatusRestController.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/controller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/pip_services4_http/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/test/TestCommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/test/TestRestClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/pip_services4_http/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.701514 pip_services4_http-0.0.3/pip_services4_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-11-08 17:27:14.000000 pip_services4_http-0.0.3/pip_services4_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-11-08 17:27:14.000000 pip_services4_http-0.0.3/pip_services4_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 17:27:14.000000 pip_services4_http-0.0.3/pip_services4_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-08 17:27:14.000000 pip_services4_http-0.0.3/pip_services4_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-08 17:27:14.000000 pip_services4_http-0.0.3/pip_services4_http.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 17:27:14.000000 pip_services4_http-0.0.3/pip_services4_http.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-08 17:27:14.713514 pip_services4_http-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.701514 pip_services4_http-0.0.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/test/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/DummyClientFixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/DummyCommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/DummyRestClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/IDummyClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/test_DummyCommandableHttpClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/clients/test_DummyRestClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/test/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/connect/test_HttpConnectionResolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 17:27:14.709514 pip_services4_http-0.0.3/test/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/DummyCommandableHttpController.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/DummyRestController.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/DummyRestOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_DummyCommandableHttpController.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_DummyCredentialsRestController.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_DummyOperations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_DummyRestController.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_HeartbeatRestController.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_HttpEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-11-08 17:26:27.000000 pip_services4_http-0.0.3/test/controllers/test_StatusRestService.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.680409 pip_services4_http-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-01 19:30:17.680409 pip_services4_http-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.672409 pip_services4_http-0.0.4/pip_services4_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.672409 pip_services4_http-0.0.4/pip_services4_http/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/auth/BasicAuthorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/auth/OwnerAuthorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/auth/RoleAuthorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.672409 pip_services4_http-0.0.4/pip_services4_http/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/build/DefaultRpcFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.672409 pip_services4_http-0.0.4/pip_services4_http/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/clients/CommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/clients/RestClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.672409 pip_services4_http-0.0.4/pip_services4_http/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/connect/HttpConnectionResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.676409 pip_services4_http-0.0.4/pip_services4_http/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/AboutOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/CommandableHttpController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/CommandableSwaggerDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/HeartBeatOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/HeartbeatRestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/HttpEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/HttpRequestDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/HttpResponseSender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/IRegisterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/ISwaggerController.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/RestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/RestOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/RestQueryParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/SSLCherryPyServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/StatusOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/StatusRestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/controller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.676409 pip_services4_http-0.0.4/pip_services4_http/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/test/TestCommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/test/TestRestClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/pip_services4_http/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.680409 pip_services4_http-0.0.4/pip_services4_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-01 19:30:17.000000 pip_services4_http-0.0.4/pip_services4_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-01 19:30:17.000000 pip_services4_http-0.0.4/pip_services4_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:30:17.000000 pip_services4_http-0.0.4/pip_services4_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-01 19:30:17.000000 pip_services4_http-0.0.4/pip_services4_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 19:30:17.000000 pip_services4_http-0.0.4/pip_services4_http.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:30:17.000000 pip_services4_http-0.0.4/pip_services4_http.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 19:30:17.680409 pip_services4_http-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.668408 pip_services4_http-0.0.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.676409 pip_services4_http-0.0.4/test/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/DummyClientFixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/DummyCommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/DummyRestClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/IDummyClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/test_DummyCommandableHttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/clients/test_DummyRestClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.676409 pip_services4_http-0.0.4/test/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/connect/test_HttpConnectionResolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:30:17.680409 pip_services4_http-0.0.4/test/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/DummyCommandableHttpController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/DummyRestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/DummyRestOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_DummyCommandableHttpController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_DummyCredentialsRestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_DummyOperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_DummyRestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_HeartbeatRestController.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_HttpEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-01 19:29:32.000000 pip_services4_http-0.0.4/test/controllers/test_StatusRestService.py
```

### Comparing `pip_services4_http-0.0.3/LICENSE` & `pip_services4_http-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/PKG-INFO` & `pip_services4_http-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_http
-Version: 0.0.3
+Version: 0.0.4
 Summary: Communication components for Pip.Services in Python
 Home-page: http://github.com/pip-services4/pip-services4-python/tree/main/tree/main/pip-services4-http-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_http-0.0.3/README.md` & `pip_services4_http-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 <a name="links"></a> Quick links:
 
 * [Your first microservice in Node.js](https://www.pipservices.org/docs/quickstart/nodejs) 
 * [Data Microservice. Step 5](https://www.pipservices.org/docs/tutorials/data-microservice/service)
 * [Microservice Facade](https://www.pipservices.org/docs/tutorials/microservice-facade/microservice-facade-main) 
 * [Client Library. Step 2](https://www.pipservices.org/docs/tutorials/client-lib/direct-client)
 * [Client Library. Step 3](https://www.pipservices.org/docs/tutorials/client-lib/http-client)
-* [API Reference](https://pip-services3-python.github.io/pip-services4-http-python/index.html)
+* [API Reference](https://pip-services4-python.github.io/pip-services4-http-python/index.html)
 * [Change Log](CHANGELOG.md)
-* [Get Help](https://www.pipservices.org/community/help)
-* [Contribute](https://www.pipservices.org/community/contribute)
+* [Get Help](http://docs.pipservices.org/v4/get_help/)
+* [Contribute](http://docs.pipservices.org/v4/contribute/)
 
 ## Use
 
 Install the Python package as
 ```bash
 pip install pip_services4_http
 ```
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/auth/BasicAuthorizer.py` & `pip_services4_http-0.0.4/pip_services4_http/auth/BasicAuthorizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/auth/OwnerAuthorizer.py` & `pip_services4_http-0.0.4/pip_services4_http/auth/OwnerAuthorizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/auth/RoleAuthorizer.py` & `pip_services4_http-0.0.4/pip_services4_http/auth/RoleAuthorizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/build/DefaultRpcFactory.py` & `pip_services4_http-0.0.4/pip_services4_http/build/DefaultRpcFactory.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 
 class DefaultRpcFactory(Factory):
     """
     Creates RPC components by their descriptors.
     """
 
-    HttpEndpointDescriptor = Descriptor("pip-controller", "endpoint", "http", "*", "1.0")
-    StatusServiceDescriptor = Descriptor("pip-controller", "status-controller", "http", "*", "1.0")
-    HeartbeatServiceDescriptor = Descriptor("pip-controller", "heartbeat-controller", "http", "*", "1.0")
+    HttpEndpointDescriptor = Descriptor("pip-services", "endpoint", "http", "*", "1.0")
+    StatusServiceDescriptor = Descriptor("pip-services", "status-controller", "http", "*", "1.0")
+    HeartbeatServiceDescriptor = Descriptor("pip-services", "heartbeat-controller", "http", "*", "1.0")
 
     def __init__(self):
         """
         Create a new instance of the factory.
         """
         super(DefaultRpcFactory, self).__init__()
         self.register_as_type(self.HttpEndpointDescriptor, HttpEndpoint)
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/clients/CommandableHttpClient.py` & `pip_services4_http-0.0.4/pip_services4_http/clients/CommandableHttpClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             - uri:                   resource URI or connection string with all parameters in it
         - options:
             - retries:               number of retries (default: 3)
             - connect_timeout:       connection timeout in milliseconds (default: 10 sec)
             - timeout:               invocation timeout in milliseconds (default: 10 sec)
 
     ### References ###
-        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
 
     Example:
     
     .. code-block:: python
 
         class MyCommandableHttpClient(CommandableHttpClient, IMyClient):
             # ...
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/clients/RestClient.py` & `pip_services4_http-0.0.4/pip_services4_http/clients/RestClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,28 @@
 class RestClient(IOpenable, IConfigurable, IReferenceable):
     """
     Abstract client that calls remove endpoints using HTTP/REST protocol.
 
     ### Configuration parameters ###
         - base_route:              base route for remote URI
         - connection(s):
-            - discovery_key:         (optional) a key to retrieve the connection from :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>`
+            - discovery_key:         (optional) a key to retrieve the connection from :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>`
             - protocol:              connection protocol: http or https
             - host:                  host name or IP address
             - port:                  port number
             - uri:                   resource URI or connection string with all parameters in it
         - options:
             - retries:               number of retries (default: 3)
             - connect_timeout:       connection timeout in milliseconds (default: 10 sec)
             - timeout:               invocation timeout in milliseconds (default: 10 sec)
 
     ### References ###
-        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
 
     Example:
 
     .. code-block:: python
 
         class MyRestClient(RestClient, IMyClient):
             def get_data(self, context, id):
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/connect/HttpConnectionResolver.py` & `pip_services4_http-0.0.4/pip_services4_http/connect/HttpConnectionResolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         - connections:                   alternative to connection
             - [connection params 1]:       first connection parameters
             -  ...
             - [connection params N]:       Nth connection parameters
             -  ...
 
     ### References ###
-        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
 
     Example:
     
     .. code-block:: python
 
           config = ConfigParams.from_tuples("connection.host", "10.1.1.100","connection.port", 8080)
           connectionResolver = HttpConnectionResolver()
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/AboutOperations.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/AboutOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/CommandableHttpController.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/CommandableHttpController.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             - discovery_key:         (optional) a key to retrieve the connection from IDiscovery
             - protocol:              connection protocol: http or https
             - host:                  host name or IP address
             - port:                  port number
             - uri:                   resource URI or connection string with all parameters in it
 
     ### References ###
-        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
         - `*:endpoint:http:*:1.0`      (optional) :class:`HttpEndpoint <pip_services4_http.controller.HttpEndpoint` reference
 
     Example:
 
     .. code-block:: python
 
           class MyCommandableHttpController(CommandableHttpController):
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/CommandableSwaggerDocument.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/CommandableSwaggerDocument.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/HeartBeatOperations.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/HeartBeatOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/HeartbeatRestController.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/HeartbeatRestController.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    pip_services4_http.controller.HeartbeatRestService
+    pip_services4_http.controller.HeartbeatRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Heartbeat rest service implementation
 
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
@@ -29,17 +29,17 @@
         - discovery_key:         (optional) a key to retrieve the connection from IDiscovery
         - protocol:              connection protocol: http or https
         - host:                  host name or IP address
         - port:                  port number
         - uri:                   resource URI or connection string with all parameters in it
 
     ### References ###
-        - `*:logger:*:*:1.0`         (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-        - `*:counters:*:*:1.0`       (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-        - `*:discovery:*:*:1.0`      (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:logger:*:*:1.0`         (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - `*:counters:*:*:1.0`       (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - `*:discovery:*:*:1.0`      (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
         - `*:endpoint:http:*:1.0`    (optional) :class:`HttpEndpoint <pip_services4_http.controller.HttpEndpoint>` reference
 
     Example:
     
     .. code-block:: python
 
           controller = HeartbeatController()
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/HttpEndpoint.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/HttpEndpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,17 @@
             - "credential.ssl_key_file" - the SSL private key in PEM
             - "credential.ssl_crt_file" - the SSL certificate in PEM
             - "credential.ssl_ca_file" - the certificate authorities (root cerfiticates) in PEM
 
 
     ### References ###
         A logger, counters, and a connection resolver can be referenced by passing the following references to the object's :func:`set_references` method:
-            - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-            - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-            - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+            - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+            - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+            - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
 
     Example:
 
     .. code-block:: python
 
         def my_method(_config, _references):
             endpoint = HttpEndpoint()
@@ -145,17 +145,17 @@
                 self.__allowed_origins = list(filter(lambda h: h != origin, self.__allowed_origins))
                 self.__allowed_origins.append(origin)
 
     def set_references(self, references: IReferences):
         """
         Sets references to this endpoint's logger, counters, and connection resolver.
 
-        - *:logger:*:*:1.0           (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-        - *:counters:*:*:1.0         (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-        - *:discovery:*:*:1.0        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - *:logger:*:*:1.0           (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - *:counters:*:*:1.0         (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - *:discovery:*:*:1.0        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
 
         :param references: an IReferences object, containing references to a logger, counters, and a connection resolver.
         """
         self.__logger.set_references(references)
         self.__counters.set_references(references)
         self.__connection_resolver.set_references(references)
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/HttpRequestDetector.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/HttpRequestDetector.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/HttpResponseSender.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/HttpResponseSender.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/IRegisterable.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/IRegisterable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/RestController.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/RestController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    pip_services4_http.controller.RestService
+    pip_services4_http.controller.RestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     
     REST service implementation
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
@@ -38,36 +38,36 @@
 
     ### Configuration parameters ###
         - base_route:              base route for remote URI
         - dependencies:
             - endpoint:              override for HTTP Endpoint dependency
             - controller:            override for Controller dependency
         - connection(s):
-            - discovery_key:         (optional) a key to retrieve the connection from :class:`IDiscovery <pip_services4_components.connect.IDiscovery.IDiscovery>`
+            - discovery_key:         (optional) a key to retrieve the connection from :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>`
             - protocol:              connection protocol: http or https
             - host:                  host name or IP address
             - port:                  port number
             - uri:                   resource URI or connection string with all parameters in it
         - credential - the HTTPS credentials:
             - ssl_key_file:         the SSL private key in PEM
             - ssl_crt_file:         the SSL certificate in PEM
             - ssl_ca_file:          the certificate authorities (root cerfiticates) in PEM
 
     ### References ###
-        - `*:logger:*:*:1.0`         (optional) :class:`ILogger <pip_services4_components.log.ILogger.ILogger>` components to pass log messages
-        - `*:counters:*:*:1.0`       (optional) :class:`ICounters <pip_services4_components.count.ICounters.ICounters>` components to pass collected measurements
-        - `*:discovery:*:*:1.0`      (optional) :class:`IDiscovery <pip_services4_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:logger:*:*:1.0`         (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - `*:counters:*:*:1.0`       (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - `*:discovery:*:*:1.0`      (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
         - `*:endpoint:http:*:1.0`    (optional) :class:`HttpEndpoint <pip_services4_http.controller.HttpEndpoint>` reference
-        - `*:tracer:*:*:1.0`         (optional) :class:`ITracer <pip_services4_components.trace.ITracer.ITracer>` components to record traces
+        - `*:tracer:*:*:1.0`         (optional) :class:`ITracer <pip_services4_observability.trace.ITracer.ITracer>` components to record traces
 
     Example:
 
     .. code-block:: python
 
-        class RestController(RestService):
+        class RestController(RestController):
             _controller = None
             # ...
 
             def __init__(self):
                 super(RestController, self).__init__()
                 self._dependencyResolver.put("controller", Descriptor("mygroup","service","*","*","1.0"))
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/RestOperations.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/RestOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/RestQueryParams.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/RestQueryParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/SSLCherryPyServer.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/SSLCherryPyServer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/StatusOperations.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/StatusOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/StatusRestController.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/StatusRestController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    pip_services4_http.controller.StatusRestService
+    pip_services4_http.controller.StatusRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Status rest service implementation
 
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
@@ -45,17 +45,17 @@
             - discovery_key:         (optional) a key to retrieve the connection from IDiscovery
             - protocol:              connection protocol: http or https
             - host:                  host name or IP address
             - port:                  port number
             - uri:                   resource URI or connection string with all parameters in it
 
     ### References ###
-        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services3_components.log.ILogger.ILogger>` components to pass log messages
-        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services3_components.count.ICounters.ICounters>` components to pass collected measurements
-        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services3_components.connect.IDiscovery.IDiscovery>` controller to resolve connection
+        - `*:logger:*:*:1.0`           (optional) :class:`ILogger <pip_services4_observability.log.ILogger.ILogger>` components to pass log messages
+        - `*:counters:*:*:1.0`         (optional) :class:`ICounters <pip_services4_observability.count.ICounters.ICounters>` components to pass collected measurements
+        - `*:discovery:*:*:1.0`        (optional) :class:`IDiscovery <pip_services4_config.connect.IDiscovery.IDiscovery>` controller to resolve connection
         - `*:endpoint:http:*:1.0`      (optional) :class:`HttpEndpoint <pip_services4_http.controller.HttpEndpoint>` reference
 
     Example:
 
     .. code-block:: python
 
           controller = StatusRestController()
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http/controller/__init__.py` & `pip_services4_http-0.0.4/pip_services4_http/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/test/TestCommandableHttpClient.py` & `pip_services4_http-0.0.4/pip_services4_http/test/TestCommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http/test/TestRestClient.py` & `pip_services4_http-0.0.4/pip_services4_http/test/TestRestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/pip_services4_http.egg-info/PKG-INFO` & `pip_services4_http-0.0.4/pip_services4_http.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pip-services4-http
-Version: 0.0.3
+Name: pip_services4_http
+Version: 0.0.4
 Summary: Communication components for Pip.Services in Python
 Home-page: http://github.com/pip-services4/pip-services4-python/tree/main/tree/main/pip-services4-http-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_http-0.0.3/pip_services4_http.egg-info/SOURCES.txt` & `pip_services4_http-0.0.4/pip_services4_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/setup.py` & `pip_services4_http-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     readme = open('readme.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_http',
-    version='0.0.3',
+    version='0.0.4',
     url='http://github.com/pip-services4/pip-services4-python/tree/main/tree/main/pip-services4-http-python',
     license='MIT',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     description='Communication components for Pip.Services in Python',
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `pip_services4_http-0.0.3/test/clients/DummyClientFixture.py` & `pip_services4_http-0.0.4/test/clients/DummyClientFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/clients/DummyCommandableHttpClient.py` & `pip_services4_http-0.0.4/test/clients/DummyCommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/clients/DummyRestClient.py` & `pip_services4_http-0.0.4/test/clients/DummyRestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/clients/IDummyClient.py` & `pip_services4_http-0.0.4/test/clients/IDummyClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/clients/__init__.py` & `pip_services4_http-0.0.4/test/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/clients/test_DummyCommandableHttpClient.py` & `pip_services4_http-0.0.4/test/clients/test_DummyCommandableHttpClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/clients/test_DummyRestClient.py` & `pip_services4_http-0.0.4/test/clients/test_DummyRestClient.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/connect/test_HttpConnectionResolver.py` & `pip_services4_http-0.0.4/test/connect/test_HttpConnectionResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/controllers/DummyCommandableHttpController.py` & `pip_services4_http-0.0.4/test/controllers/DummyCommandableHttpController.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/controllers/DummyRestController.py` & `pip_services4_http-0.0.4/test/controllers/DummyRestController.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test.rest.DummyRestService
+    test.rest.DummyRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~
     
     Dummy REST service
     
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

### Comparing `pip_services4_http-0.0.3/test/controllers/DummyRestOperations.py` & `pip_services4_http-0.0.4/test/controllers/DummyRestOperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test.rest.DummyRestService
+    test.rest.DummyRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~
     
     Dummy REST service
     
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

### Comparing `pip_services4_http-0.0.3/test/controllers/__init__.py` & `pip_services4_http-0.0.4/test/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/controllers/test_DummyCommandableHttpController.py` & `pip_services4_http-0.0.4/test/controllers/test_DummyCommandableHttpController.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/controllers/test_DummyCredentialsRestController.py` & `pip_services4_http-0.0.4/test/controllers/test_DummyCredentialsRestController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test_DummyCredentialsRestService
+    test_DummyCredentialsRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Dummy commandable HTTP service test
 
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

### Comparing `pip_services4_http-0.0.3/test/controllers/test_DummyOperations.py` & `pip_services4_http-0.0.4/test/controllers/test_DummyOperations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test_DummyRestService
+    test_DummyRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Dummy commandable HTTP service test
 
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

### Comparing `pip_services4_http-0.0.3/test/controllers/test_DummyRestController.py` & `pip_services4_http-0.0.4/test/controllers/test_DummyRestController.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test_DummyRestService
+    test_DummyRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Dummy commandable HTTP service test
 
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

### Comparing `pip_services4_http-0.0.3/test/controllers/test_HeartbeatRestController.py` & `pip_services4_http-0.0.4/test/controllers/test_HeartbeatRestController.py`

 * *Files identical despite different names*

### Comparing `pip_services4_http-0.0.3/test/controllers/test_HttpEndpoint.py` & `pip_services4_http-0.0.4/test/controllers/test_HttpEndpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test_DummyRestService
+    test_DummyRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Dummy commandable HTTP service test
 
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

### Comparing `pip_services4_http-0.0.3/test/controllers/test_StatusRestService.py` & `pip_services4_http-0.0.4/test/controllers/test_StatusRestService.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    test_DummyRestService
+    test_DummyRestController
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Dummy commandable HTTP service test
 
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
```

