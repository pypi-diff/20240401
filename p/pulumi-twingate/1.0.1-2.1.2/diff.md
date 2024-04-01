# Comparing `tmp/pulumi_twingate-1.0.1.tar.gz` & `tmp/pulumi_twingate-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_twingate-1.0.1.tar", last modified: Mon Apr  1 15:14:02 2024, max compression
+gzip compressed data, was "pulumi_twingate-2.1.2.tar", last modified: Tue Mar 26 21:53:43 2024, max compression
```

## Comparing `pulumi_twingate-1.0.1.tar` & `pulumi_twingate-2.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:02.029968 pulumi_twingate-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-01 15:14:02.029968 pulumi_twingate-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:02.029968 pulumi_twingate-1.0.1/pulumi_twingate/
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:02.029968 pulumi_twingate-1.0.1/pulumi_twingate/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_remote_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_security_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    25767 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_connector_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    30932 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_service_account_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate/twingate_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:14:02.029968 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-01 15:14:02.000000 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/pulumi_twingate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:14:02.029968 pulumi_twingate-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-01 15:14:01.000000 pulumi_twingate-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:53:43.363673 pulumi_twingate-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-26 21:53:43.363673 pulumi_twingate-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:53:43.359673 pulumi_twingate-2.1.2/pulumi_twingate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:53:43.363673 pulumi_twingate-2.1.2/pulumi_twingate/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_remote_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25767 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_connector_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30932 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_service_account_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate/twingate_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 21:53:43.359673 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/pulumi_twingate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 21:53:43.363673 pulumi_twingate-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-26 21:53:43.000000 pulumi_twingate-2.1.2/setup.py
```

### Comparing `pulumi_twingate-1.0.1/PKG-INFO` & `pulumi_twingate-2.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_twingate
-Version: 1.0.1
+Version: 2.1.2
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-1.0.1/README.md` & `pulumi_twingate-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/__init__.py` & `pulumi_twingate-2.1.2/pulumi_twingate/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/_inputs.py` & `pulumi_twingate-2.1.2/pulumi_twingate/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/_utilities.py` & `pulumi_twingate-2.1.2/pulumi_twingate/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/config/vars.py` & `pulumi_twingate-2.1.2/pulumi_twingate/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_connector.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_connectors.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_connectors.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_group.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_groups.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_remote_network.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_remote_networks.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_remote_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_resource.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_resources.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_security_policies.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_security_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_security_policy.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_service_accounts.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_service_accounts.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_user.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/get_twingate_users.py` & `pulumi_twingate-2.1.2/pulumi_twingate/get_twingate_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/outputs.py` & `pulumi_twingate-2.1.2/pulumi_twingate/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/provider.py` & `pulumi_twingate-2.1.2/pulumi_twingate/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_connector.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_connector_tokens.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_connector_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_group.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_remote_network.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_resource.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_service_account.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_service_account_key.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_service_account_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate/twingate_user.py` & `pulumi_twingate-2.1.2/pulumi_twingate/twingate_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate.egg-info/PKG-INFO` & `pulumi_twingate-2.1.2/pulumi_twingate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-twingate
-Version: 1.0.1
+Version: 2.1.2
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-1.0.1/pulumi_twingate.egg-info/SOURCES.txt` & `pulumi_twingate-2.1.2/pulumi_twingate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-1.0.1/setup.py` & `pulumi_twingate-2.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.1"
+VERSION = "2.1.2"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "twingate Pulumi Package - Development Version"
```

