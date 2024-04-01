# Comparing `tmp/emailbob_twingate-0.0.7.tar.gz` & `tmp/emailbob_twingate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailbob_twingate-0.0.7.tar", last modified: Wed Mar 27 17:10:07 2024, max compression
+gzip compressed data, was "emailbob_twingate-0.0.9.tar", last modified: Mon Apr  1 15:44:39 2024, max compression
```

## Comparing `emailbob_twingate-0.0.7.tar` & `emailbob_twingate-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:10:07.932510 emailbob_twingate-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-27 17:10:07.932510 emailbob_twingate-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:10:07.928511 emailbob_twingate-0.0.7/emailbob_twingate/
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:10:07.932510 emailbob_twingate-0.0.7/emailbob_twingate/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_remote_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_security_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    25767 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_connector_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    30932 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_service_account_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate/twingate_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:10:07.932510 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/emailbob_twingate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 17:10:07.932510 emailbob_twingate-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-27 17:10:07.000000 emailbob_twingate-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:44:39.746895 emailbob_twingate-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-01 15:44:39.746895 emailbob_twingate-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:44:39.746895 emailbob_twingate-0.0.9/emailbob_twingate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:44:39.746895 emailbob_twingate-0.0.9/emailbob_twingate/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_remote_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25767 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_connector_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30932 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_service_account_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate/twingate_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:44:39.746895 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/emailbob_twingate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:44:39.746895 emailbob_twingate-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-01 15:44:39.000000 emailbob_twingate-0.0.9/setup.py
```

### Comparing `emailbob_twingate-0.0.7/PKG-INFO` & `emailbob_twingate-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailbob_twingate
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/emailbob/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `emailbob_twingate-0.0.7/README.md` & `emailbob_twingate-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/__init__.py` & `emailbob_twingate-0.0.9/emailbob_twingate/__init__.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/_inputs.py` & `emailbob_twingate-0.0.9/emailbob_twingate/_inputs.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/_utilities.py` & `emailbob_twingate-0.0.9/emailbob_twingate/_utilities.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/config/vars.py` & `emailbob_twingate-0.0.9/emailbob_twingate/config/vars.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_connector.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_connector.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_connectors.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_connectors.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_group.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_group.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_groups.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_groups.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_remote_network.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_remote_networks.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_remote_networks.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_resource.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_resource.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_resources.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_resources.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_security_policies.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_security_policies.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_security_policy.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_security_policy.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_service_accounts.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_service_accounts.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_user.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_user.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/get_twingate_users.py` & `emailbob_twingate-0.0.9/emailbob_twingate/get_twingate_users.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/outputs.py` & `emailbob_twingate-0.0.9/emailbob_twingate/outputs.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/provider.py` & `emailbob_twingate-0.0.9/emailbob_twingate/provider.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_connector.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_connector.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_connector_tokens.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_connector_tokens.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_group.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_group.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_remote_network.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_resource.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_resource.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_service_account.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_service_account.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_service_account_key.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_service_account_key.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate/twingate_user.py` & `emailbob_twingate-0.0.9/emailbob_twingate/twingate_user.py`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate.egg-info/PKG-INFO` & `emailbob_twingate-0.0.9/emailbob_twingate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailbob-twingate
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/emailbob/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `emailbob_twingate-0.0.7/emailbob_twingate.egg-info/SOURCES.txt` & `emailbob_twingate-0.0.9/emailbob_twingate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emailbob_twingate-0.0.7/setup.py` & `emailbob_twingate-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.7"
+VERSION = "0.0.9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "twingate Pulumi Package - Development Version"
```

