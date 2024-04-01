# Comparing `tmp/enedis_data_connect-1.0.0.tar.gz` & `tmp/enedis_data_connect-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enedis_data_connect-1.0.0.tar", last modified: Sun Mar 31 08:57:24 2024, max compression
+gzip compressed data, was "enedis_data_connect-1.0.1.tar", last modified: Mon Apr  1 10:26:47 2024, max compression
```

## Comparing `enedis_data_connect-1.0.0.tar` & `enedis_data_connect-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:57:24.894068 enedis_data_connect-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-03-31 08:57:24.894068 enedis_data_connect-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:57:24.894068 enedis_data_connect-1.0.0/enedis_data_connect/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/enedis_data_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23696 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/enedis_data_connect/enedis_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/enedis_data_connect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:57:24.894068 enedis_data_connect-1.0.0/enedis_data_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-03-31 08:57:24.000000 enedis_data_connect-1.0.0/enedis_data_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-31 08:57:24.000000 enedis_data_connect-1.0.0/enedis_data_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 08:57:24.000000 enedis_data_connect-1.0.0/enedis_data_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 08:57:24.000000 enedis_data_connect-1.0.0/enedis_data_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 08:57:24.894068 enedis_data_connect-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:57:24.894068 enedis_data_connect-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18534 2024-03-31 08:57:21.000000 enedis_data_connect-1.0.0/tests/test_enedis_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:47.038746 enedis_data_connect-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23309 2024-04-01 10:26:47.038746 enedis_data_connect-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:47.038746 enedis_data_connect-1.0.1/enedis_data_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/enedis_data_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23696 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/enedis_data_connect/enedis_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/enedis_data_connect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:47.038746 enedis_data_connect-1.0.1/enedis_data_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23309 2024-04-01 10:26:47.000000 enedis_data_connect-1.0.1/enedis_data_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-01 10:26:47.000000 enedis_data_connect-1.0.1/enedis_data_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 10:26:47.000000 enedis_data_connect-1.0.1/enedis_data_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 10:26:47.000000 enedis_data_connect-1.0.1/enedis_data_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 10:26:47.038746 enedis_data_connect-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 10:26:47.038746 enedis_data_connect-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18534 2024-04-01 10:26:37.000000 enedis_data_connect-1.0.1/tests/test_enedis_client.py
```

### Comparing `enedis_data_connect-1.0.0/LICENSE` & `enedis_data_connect-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enedis_data_connect-1.0.0/PKG-INFO` & `enedis_data_connect-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enedis_data_connect
-Version: 1.0.0
+Version: 1.0.1
 Summary: Enedis data connect client
 Home-page: https://github.com/infodavide/enedis_data_connect
 Author: David R
 Author-email: contact@infodavid.org
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
@@ -346,7 +346,73 @@
         Public License instead of this License.
         
 License-File: LICENSE
 
 # Enedis data connect client
 
 Enedis data connect client is a client for the REST API of the Enedis company.
+
+The client is used to retrieve the consumption and production data, refer to the documentation provided by the Enedis API on https://datahub-enedis.fr/services-api/data-connect/documentation.
+
+## Connecting the client to authenticate and get the token
+
+To connect you need to provide the PDL identifier described in the contract.
+
+You have to pass the client identifier and the secret key generated by the Enedis portal.
+
+    client = EnedisClient(pdl, id, secret)
+    client.connect()
+
+If the authentication fails, an InvalidAccess exception is thrown otherwise the token data will be stored internally.
+
+## Closing or deleting token data
+
+To clear the token data, you just have to use:
+
+    client.close()
+
+## Other methods
+
+The client has some getters to access counters and basic data.
+
+    client.get_pdl()
+
+    client.get_client_id()
+
+    client.get_token_data()
+
+    client.get_requests_count()
+
+    client.get_errors_count()
+
+    client.is_connected()
+
+## The helper
+
+The module provides a helper class useful for retrieving data from the API.
+
+To instantiate the helper, you just need to pass the client instance.
+
+    helper = EnedisApiHelper(client)
+
+To use the helper, it is not necessary to authenticate first. The helper will manage the authentication process (with retry on token expiration)
+
+### Get the maximum consumed power per day
+
+The maximum consumed power per day is returned as a dictionary of integers indexed by the datetime.
+To request the API you have to pass a start date and a end date.
+
+    data: dict[datetime, int] = helper.get_max_daily_consumed_power(start_time, end_time)
+
+### Get the consumption per day
+
+The consumption per day is returned as a dictionary of integers indexed by the date.
+To request the API you have to pass a start date and a end date.
+
+    data: dict[date, int] = helper.get_daily_consumption(start_time, end_time)
+
+### Get the consumption per half an hour
+
+The consumption is returned as a dictionary of integers indexed by the datetime.
+To request the API you have to pass a start date and a end date.
+
+    data: dict[datetime, int] = helper.get_consumption_load_curve(start_time, end_time)
```

### Comparing `enedis_data_connect-1.0.0/enedis_data_connect/enedis_client.py` & `enedis_data_connect-1.0.1/enedis_data_connect/enedis_client.py`

 * *Files identical despite different names*

### Comparing `enedis_data_connect-1.0.0/enedis_data_connect.egg-info/PKG-INFO` & `enedis_data_connect-1.0.1/enedis_data_connect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enedis_data_connect
-Version: 1.0.0
+Version: 1.0.1
 Summary: Enedis data connect client
 Home-page: https://github.com/infodavide/enedis_data_connect
 Author: David R
 Author-email: contact@infodavid.org
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
@@ -346,7 +346,73 @@
         Public License instead of this License.
         
 License-File: LICENSE
 
 # Enedis data connect client
 
 Enedis data connect client is a client for the REST API of the Enedis company.
+
+The client is used to retrieve the consumption and production data, refer to the documentation provided by the Enedis API on https://datahub-enedis.fr/services-api/data-connect/documentation.
+
+## Connecting the client to authenticate and get the token
+
+To connect you need to provide the PDL identifier described in the contract.
+
+You have to pass the client identifier and the secret key generated by the Enedis portal.
+
+    client = EnedisClient(pdl, id, secret)
+    client.connect()
+
+If the authentication fails, an InvalidAccess exception is thrown otherwise the token data will be stored internally.
+
+## Closing or deleting token data
+
+To clear the token data, you just have to use:
+
+    client.close()
+
+## Other methods
+
+The client has some getters to access counters and basic data.
+
+    client.get_pdl()
+
+    client.get_client_id()
+
+    client.get_token_data()
+
+    client.get_requests_count()
+
+    client.get_errors_count()
+
+    client.is_connected()
+
+## The helper
+
+The module provides a helper class useful for retrieving data from the API.
+
+To instantiate the helper, you just need to pass the client instance.
+
+    helper = EnedisApiHelper(client)
+
+To use the helper, it is not necessary to authenticate first. The helper will manage the authentication process (with retry on token expiration)
+
+### Get the maximum consumed power per day
+
+The maximum consumed power per day is returned as a dictionary of integers indexed by the datetime.
+To request the API you have to pass a start date and a end date.
+
+    data: dict[datetime, int] = helper.get_max_daily_consumed_power(start_time, end_time)
+
+### Get the consumption per day
+
+The consumption per day is returned as a dictionary of integers indexed by the date.
+To request the API you have to pass a start date and a end date.
+
+    data: dict[date, int] = helper.get_daily_consumption(start_time, end_time)
+
+### Get the consumption per half an hour
+
+The consumption is returned as a dictionary of integers indexed by the datetime.
+To request the API you have to pass a start date and a end date.
+
+    data: dict[datetime, int] = helper.get_consumption_load_curve(start_time, end_time)
```

### Comparing `enedis_data_connect-1.0.0/setup.py` & `enedis_data_connect-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme_content = f.read()
 
 with open('LICENSE', encoding='utf-8') as f:
     license_content = f.read()
 
 setup(
     name='enedis_data_connect',
-    version='1.0.0',
+    version='1.0.1',
     description='Enedis data connect client',
     long_description=readme_content,
     author='David R', 
     author_email='contact@infodavid.org',
     url='https://github.com/infodavide/enedis_data_connect',
     license=license_content,
     packages=find_packages(exclude=('tests', 'docs'))
```

### Comparing `enedis_data_connect-1.0.0/tests/test_enedis_client.py` & `enedis_data_connect-1.0.1/tests/test_enedis_client.py`

 * *Files identical despite different names*

