# Comparing `tmp/mypy-boto3-datazone-1.34.31.tar.gz` & `tmp/mypy-boto3-datazone-1.34.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datazone-1.34.31.tar", last modified: Tue Jan 30 20:32:18 2024, max compression
+gzip compressed data, was "mypy-boto3-datazone-1.34.75.tar", last modified: Mon Apr  1 20:08:26 2024, max compression
```

## Comparing `mypy-boto3-datazone-1.34.31.tar` & `mypy-boto3-datazone-1.34.75.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 20:32:18.979390 mypy-boto3-datazone-1.34.31/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-01-30 20:32:18.979390 mypy-boto3-datazone-1.34.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 20:32:18.979390 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79244 2024-01-30 20:32:03.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    79241 2024-01-30 20:32:03.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-01-30 20:32:04.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-01-30 20:32:04.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28130 2024-01-30 20:32:04.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28108 2024-01-30 20:32:04.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   119584 2024-01-30 20:32:06.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   119584 2024-01-30 20:32:05.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 20:32:18.979390 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-01-30 20:32:18.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-30 20:32:18.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 20:32:18.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 20:32:18.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-30 20:32:18.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-30 20:32:18.000000 mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 20:32:18.979390 mypy-boto3-datazone-1.34.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-01-30 20:32:02.000000 mypy-boto3-datazone-1.34.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.581728 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82303 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82300 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18591 2024-04-01 20:07:59.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18591 2024-04-01 20:07:59.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-04-01 20:07:59.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29464 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   123413 2024-04-01 20:08:01.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123413 2024-04-01 20:08:01.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/setup.py
```

### Comparing `mypy-boto3-datazone-1.34.31/LICENSE` & `mypy-boto3-datazone-1.34.75/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datazone-1.34.31/PKG-INFO` & `mypy-boto3-datazone-1.34.75/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datazone
-Version: 1.34.31
-Summary: Type annotations for boto3.DataZone 1.34.31 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.75
+Summary: Type annotations for boto3.DataZone 1.34.75 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datazone.svg?color=blue)](https://pypi.org/project/mypy-boto3-datazone)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datazone)](https://pepy.tech/project/mypy-boto3-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataZone 1.34.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[boto3.DataZone 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datazone docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +289,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionTargetsPaginator,
     ListSubscriptionsPaginator,
@@ -328,14 +329,17 @@
 list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator(
     "list_environment_blueprints"
 )
 list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator(
     "list_environment_profiles"
 )
 list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator(
+    "list_metadata_generation_runs"
+)
 list_notifications_paginator: ListNotificationsPaginator = client.get_paginator(
     "list_notifications"
 )
 list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator(
     "list_project_memberships"
 )
 list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

### Comparing `mypy-boto3-datazone-1.34.31/README.md` & `mypy-boto3-datazone-1.34.75/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datazone.svg?color=blue)](https://pypi.org/project/mypy-boto3-datazone)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datazone)](https://pepy.tech/project/mypy-boto3-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataZone 1.34.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[boto3.DataZone 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datazone docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/).
 
 See how it helps to find and fix potential bugs:
 
@@ -256,14 +256,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionTargetsPaginator,
     ListSubscriptionsPaginator,
@@ -295,14 +296,17 @@
 list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator(
     "list_environment_blueprints"
 )
 list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator(
     "list_environment_profiles"
 )
 list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator(
+    "list_metadata_generation_runs"
+)
 list_notifications_paginator: ListNotificationsPaginator = client.get_paginator(
     "list_notifications"
 )
 list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator(
     "list_project_memberships"
 )
 list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/__init__.py` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         ListDataSourceRunsPaginator,
         ListDataSourcesPaginator,
         ListDomainsPaginator,
         ListEnvironmentBlueprintConfigurationsPaginator,
         ListEnvironmentBlueprintsPaginator,
         ListEnvironmentProfilesPaginator,
         ListEnvironmentsPaginator,
+        ListMetadataGenerationRunsPaginator,
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
@@ -39,14 +40,15 @@
     list_data_source_runs_paginator: ListDataSourceRunsPaginator = client.get_paginator("list_data_source_runs")
     list_data_sources_paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
     list_environment_blueprint_configurations_paginator: ListEnvironmentBlueprintConfigurationsPaginator = client.get_paginator("list_environment_blueprint_configurations")
     list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator("list_environment_blueprints")
     list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator("list_environment_profiles")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+    list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator("list_metadata_generation_runs")
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
@@ -65,14 +67,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
@@ -93,14 +96,15 @@
     "ListDataSourceRunsPaginator",
     "ListDataSourcesPaginator",
     "ListDomainsPaginator",
     "ListEnvironmentBlueprintConfigurationsPaginator",
     "ListEnvironmentBlueprintsPaginator",
     "ListEnvironmentProfilesPaginator",
     "ListEnvironmentsPaginator",
+    "ListMetadataGenerationRunsPaginator",
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/__init__.pyi` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         ListDataSourceRunsPaginator,
         ListDataSourcesPaginator,
         ListDomainsPaginator,
         ListEnvironmentBlueprintConfigurationsPaginator,
         ListEnvironmentBlueprintsPaginator,
         ListEnvironmentProfilesPaginator,
         ListEnvironmentsPaginator,
+        ListMetadataGenerationRunsPaginator,
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
@@ -39,14 +40,15 @@
     list_data_source_runs_paginator: ListDataSourceRunsPaginator = client.get_paginator("list_data_source_runs")
     list_data_sources_paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
     list_environment_blueprint_configurations_paginator: ListEnvironmentBlueprintConfigurationsPaginator = client.get_paginator("list_environment_blueprint_configurations")
     list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator("list_environment_blueprints")
     list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator("list_environment_profiles")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+    list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator("list_metadata_generation_runs")
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
@@ -65,14 +67,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
@@ -93,14 +96,15 @@
     "ListDataSourceRunsPaginator",
     "ListDataSourcesPaginator",
     "ListDomainsPaginator",
     "ListEnvironmentBlueprintConfigurationsPaginator",
     "ListEnvironmentBlueprintsPaginator",
     "ListEnvironmentProfilesPaginator",
     "ListEnvironmentsPaginator",
+    "ListMetadataGenerationRunsPaginator",
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/__main__.py` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataZone 1.34.31\n"
-        "Version:         1.34.31\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.DataZone 1.34.75\n"
+        "Version:         1.34.75\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.31")
+    print("1.34.75")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/client.py` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     EnvironmentStatusType,
     FormTypeStatusType,
     GlossaryStatusType,
     GlossaryTermStatusType,
     GroupProfileStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
+    MetadataGenerationRunStatusType,
     NotificationTypeType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantStatusType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
@@ -53,14 +54,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
@@ -115,14 +117,15 @@
     GetEnvironmentProfileOutputTypeDef,
     GetFormTypeOutputTypeDef,
     GetGlossaryOutputTypeDef,
     GetGlossaryTermOutputTypeDef,
     GetGroupProfileOutputTypeDef,
     GetIamPortalLoginUrlOutputTypeDef,
     GetListingOutputTypeDef,
+    GetMetadataGenerationRunOutputTypeDef,
     GetProjectOutputTypeDef,
     GetSubscriptionGrantOutputTypeDef,
     GetSubscriptionOutputTypeDef,
     GetSubscriptionRequestDetailsOutputTypeDef,
     GetSubscriptionTargetOutputTypeDef,
     GetUserProfileOutputTypeDef,
     GrantedEntityInputTypeDef,
@@ -131,23 +134,25 @@
     ListDataSourceRunsOutputTypeDef,
     ListDataSourcesOutputTypeDef,
     ListDomainsOutputTypeDef,
     ListEnvironmentBlueprintConfigurationsOutputTypeDef,
     ListEnvironmentBlueprintsOutputTypeDef,
     ListEnvironmentProfilesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListMetadataGenerationRunsOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberTypeDef,
+    MetadataGenerationRunTargetTypeDef,
     ModelTypeDef,
     PredictionConfigurationTypeDef,
     PutEnvironmentBlueprintConfigurationOutputTypeDef,
     RecommendationConfigurationTypeDef,
     RejectChoiceTypeDef,
     RejectPredictionsOutputTypeDef,
     RejectRuleTypeDef,
@@ -159,14 +164,15 @@
     SearchListingsOutputTypeDef,
     SearchOutputTypeDef,
     SearchSortTypeDef,
     SearchTypesOutputTypeDef,
     SearchUserProfilesOutputTypeDef,
     SingleSignOnTypeDef,
     StartDataSourceRunOutputTypeDef,
+    StartMetadataGenerationRunOutputTypeDef,
     SubscribedListingInputTypeDef,
     SubscribedPrincipalInputTypeDef,
     SubscriptionTargetFormTypeDef,
     TermRelationsTypeDef,
     TimestampTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateDomainOutputTypeDef,
@@ -260,14 +266,24 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#can_paginate)
         """
 
+    def cancel_metadata_generation_run(
+        self, *, domainIdentifier: str, identifier: str
+    ) -> Dict[str, Any]:
+        """
+        Cancels the metadata generation run.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.cancel_metadata_generation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#cancel_metadata_generation_run)
+        """
+
     def cancel_subscription(
         self, *, domainIdentifier: str, identifier: str
     ) -> CancelSubscriptionOutputTypeDef:
         """
         Cancels the subscription to the specified asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.cancel_subscription)
@@ -489,16 +505,17 @@
         domainIdentifier: str,
         entityIdentifier: str,
         entityType: Literal["ASSET"],
         clientToken: str = ...,
         entityRevision: str = ...,
     ) -> CreateListingChangeSetOutputTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/CreateListingChangeSet).
+        Publishes a listing (a record of an asset at a given time) or removes a listing
+        from the
+        catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_listing_change_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#create_listing_change_set)
         """
 
     def create_project(
         self,
@@ -687,16 +704,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_glossary_term)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_glossary_term)
         """
 
     def delete_listing(self, *, domainIdentifier: str, identifier: str) -> Dict[str, Any]:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/DeleteListing).
+        Deletes a listing (a record of an asset at a given time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_listing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_listing)
         """
 
     def delete_project(
         self, *, domainIdentifier: str, identifier: str, skipDeletionCheck: bool = ...
@@ -898,21 +914,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_iam_portal_login_url)
         """
 
     def get_listing(
         self, *, domainIdentifier: str, identifier: str, listingRevision: str = ...
     ) -> GetListingOutputTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/GetListing).
+        Gets a listing (a record of an asset at a given time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_listing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_listing)
         """
 
+    def get_metadata_generation_run(
+        self, *, domainIdentifier: str, identifier: str
+    ) -> GetMetadataGenerationRunOutputTypeDef:
+        """
+        Gets a metadata generation run in Amazon DataZone.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_metadata_generation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_metadata_generation_run)
+        """
+
     def get_project(self, *, domainIdentifier: str, identifier: str) -> GetProjectOutputTypeDef:
         """
         Gets a project in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_project)
         """
@@ -1101,14 +1126,30 @@
         """
         Lists Amazon DataZone environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_environments)
         """
 
+    def list_metadata_generation_runs(
+        self,
+        *,
+        domainIdentifier: str,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        status: MetadataGenerationRunStatusType = ...,
+        type: Literal["BUSINESS_DESCRIPTIONS"] = ...,
+    ) -> ListMetadataGenerationRunsOutputTypeDef:
+        """
+        Lists all metadata generation runs.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_metadata_generation_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_metadata_generation_runs)
+        """
+
     def list_notifications(
         self,
         *,
         domainIdentifier: str,
         type: NotificationTypeType,
         afterTimestamp: TimestampTypeDef = ...,
         beforeTimestamp: TimestampTypeDef = ...,
@@ -1347,15 +1388,15 @@
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
     ) -> SearchListingsOutputTypeDef:
         """
-        Searches listings in Amazon DataZone.
+        Searches listings (records of an asset at a given time) in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_listings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#search_listings)
         """
 
     def search_types(
         self,
@@ -1399,14 +1440,30 @@
         """
         Start the run of the specified data source in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.start_data_source_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#start_data_source_run)
         """
 
+    def start_metadata_generation_run(
+        self,
+        *,
+        domainIdentifier: str,
+        owningProjectIdentifier: str,
+        target: MetadataGenerationRunTargetTypeDef,
+        type: Literal["BUSINESS_DESCRIPTIONS"],
+        clientToken: str = ...,
+    ) -> StartMetadataGenerationRunOutputTypeDef:
+        """
+        Starts the metadata generation run.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.start_metadata_generation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#start_metadata_generation_run)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#tag_resource)
         """
@@ -1693,14 +1750,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_metadata_generation_runs"]
+    ) -> ListMetadataGenerationRunsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_notifications"]
     ) -> ListNotificationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/client.pyi` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     EnvironmentStatusType,
     FormTypeStatusType,
     GlossaryStatusType,
     GlossaryTermStatusType,
     GroupProfileStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
+    MetadataGenerationRunStatusType,
     NotificationTypeType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantStatusType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
@@ -53,14 +54,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
@@ -115,14 +117,15 @@
     GetEnvironmentProfileOutputTypeDef,
     GetFormTypeOutputTypeDef,
     GetGlossaryOutputTypeDef,
     GetGlossaryTermOutputTypeDef,
     GetGroupProfileOutputTypeDef,
     GetIamPortalLoginUrlOutputTypeDef,
     GetListingOutputTypeDef,
+    GetMetadataGenerationRunOutputTypeDef,
     GetProjectOutputTypeDef,
     GetSubscriptionGrantOutputTypeDef,
     GetSubscriptionOutputTypeDef,
     GetSubscriptionRequestDetailsOutputTypeDef,
     GetSubscriptionTargetOutputTypeDef,
     GetUserProfileOutputTypeDef,
     GrantedEntityInputTypeDef,
@@ -131,23 +134,25 @@
     ListDataSourceRunsOutputTypeDef,
     ListDataSourcesOutputTypeDef,
     ListDomainsOutputTypeDef,
     ListEnvironmentBlueprintConfigurationsOutputTypeDef,
     ListEnvironmentBlueprintsOutputTypeDef,
     ListEnvironmentProfilesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListMetadataGenerationRunsOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberTypeDef,
+    MetadataGenerationRunTargetTypeDef,
     ModelTypeDef,
     PredictionConfigurationTypeDef,
     PutEnvironmentBlueprintConfigurationOutputTypeDef,
     RecommendationConfigurationTypeDef,
     RejectChoiceTypeDef,
     RejectPredictionsOutputTypeDef,
     RejectRuleTypeDef,
@@ -159,14 +164,15 @@
     SearchListingsOutputTypeDef,
     SearchOutputTypeDef,
     SearchSortTypeDef,
     SearchTypesOutputTypeDef,
     SearchUserProfilesOutputTypeDef,
     SingleSignOnTypeDef,
     StartDataSourceRunOutputTypeDef,
+    StartMetadataGenerationRunOutputTypeDef,
     SubscribedListingInputTypeDef,
     SubscribedPrincipalInputTypeDef,
     SubscriptionTargetFormTypeDef,
     TermRelationsTypeDef,
     TimestampTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateDomainOutputTypeDef,
@@ -257,14 +263,24 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#can_paginate)
         """
 
+    def cancel_metadata_generation_run(
+        self, *, domainIdentifier: str, identifier: str
+    ) -> Dict[str, Any]:
+        """
+        Cancels the metadata generation run.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.cancel_metadata_generation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#cancel_metadata_generation_run)
+        """
+
     def cancel_subscription(
         self, *, domainIdentifier: str, identifier: str
     ) -> CancelSubscriptionOutputTypeDef:
         """
         Cancels the subscription to the specified asset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.cancel_subscription)
@@ -486,16 +502,17 @@
         domainIdentifier: str,
         entityIdentifier: str,
         entityType: Literal["ASSET"],
         clientToken: str = ...,
         entityRevision: str = ...,
     ) -> CreateListingChangeSetOutputTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/CreateListingChangeSet).
+        Publishes a listing (a record of an asset at a given time) or removes a listing
+        from the
+        catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.create_listing_change_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#create_listing_change_set)
         """
 
     def create_project(
         self,
@@ -684,16 +701,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_glossary_term)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_glossary_term)
         """
 
     def delete_listing(self, *, domainIdentifier: str, identifier: str) -> Dict[str, Any]:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/DeleteListing).
+        Deletes a listing (a record of an asset at a given time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_listing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_listing)
         """
 
     def delete_project(
         self, *, domainIdentifier: str, identifier: str, skipDeletionCheck: bool = ...
@@ -895,21 +911,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_iam_portal_login_url)
         """
 
     def get_listing(
         self, *, domainIdentifier: str, identifier: str, listingRevision: str = ...
     ) -> GetListingOutputTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/datazone-2018-05-10/GetListing).
+        Gets a listing (a record of an asset at a given time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_listing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_listing)
         """
 
+    def get_metadata_generation_run(
+        self, *, domainIdentifier: str, identifier: str
+    ) -> GetMetadataGenerationRunOutputTypeDef:
+        """
+        Gets a metadata generation run in Amazon DataZone.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_metadata_generation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_metadata_generation_run)
+        """
+
     def get_project(self, *, domainIdentifier: str, identifier: str) -> GetProjectOutputTypeDef:
         """
         Gets a project in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_project)
         """
@@ -1098,14 +1123,30 @@
         """
         Lists Amazon DataZone environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_environments)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_environments)
         """
 
+    def list_metadata_generation_runs(
+        self,
+        *,
+        domainIdentifier: str,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        status: MetadataGenerationRunStatusType = ...,
+        type: Literal["BUSINESS_DESCRIPTIONS"] = ...,
+    ) -> ListMetadataGenerationRunsOutputTypeDef:
+        """
+        Lists all metadata generation runs.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_metadata_generation_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_metadata_generation_runs)
+        """
+
     def list_notifications(
         self,
         *,
         domainIdentifier: str,
         type: NotificationTypeType,
         afterTimestamp: TimestampTypeDef = ...,
         beforeTimestamp: TimestampTypeDef = ...,
@@ -1344,15 +1385,15 @@
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
     ) -> SearchListingsOutputTypeDef:
         """
-        Searches listings in Amazon DataZone.
+        Searches listings (records of an asset at a given time) in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.search_listings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#search_listings)
         """
 
     def search_types(
         self,
@@ -1396,14 +1437,30 @@
         """
         Start the run of the specified data source in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.start_data_source_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#start_data_source_run)
         """
 
+    def start_metadata_generation_run(
+        self,
+        *,
+        domainIdentifier: str,
+        owningProjectIdentifier: str,
+        target: MetadataGenerationRunTargetTypeDef,
+        type: Literal["BUSINESS_DESCRIPTIONS"],
+        clientToken: str = ...,
+    ) -> StartMetadataGenerationRunOutputTypeDef:
+        """
+        Starts the metadata generation run.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.start_metadata_generation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#start_metadata_generation_run)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#tag_resource)
         """
@@ -1690,14 +1747,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_metadata_generation_runs"]
+    ) -> ListMetadataGenerationRunsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_notifications"]
     ) -> ListNotificationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/literals.py` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,26 @@
     "ListDataSourceRunsPaginatorName",
     "ListDataSourcesPaginatorName",
     "ListDomainsPaginatorName",
     "ListEnvironmentBlueprintConfigurationsPaginatorName",
     "ListEnvironmentBlueprintsPaginatorName",
     "ListEnvironmentProfilesPaginatorName",
     "ListEnvironmentsPaginatorName",
+    "ListMetadataGenerationRunsPaginatorName",
     "ListNotificationsPaginatorName",
     "ListProjectMembershipsPaginatorName",
     "ListProjectsPaginatorName",
     "ListSubscriptionGrantsPaginatorName",
     "ListSubscriptionRequestsPaginatorName",
     "ListSubscriptionTargetsPaginatorName",
     "ListSubscriptionsPaginatorName",
     "ListingStatusType",
+    "MetadataGenerationRunStatusType",
+    "MetadataGenerationRunTypeType",
+    "MetadataGenerationTargetTypeType",
     "NotificationResourceTypeType",
     "NotificationRoleType",
     "NotificationTypeType",
     "ProjectStatusType",
     "RejectRuleBehaviorType",
     "SearchGroupProfilesPaginatorName",
     "SearchListingsPaginatorName",
@@ -166,22 +170,28 @@
 ListDomainsPaginatorName = Literal["list_domains"]
 ListEnvironmentBlueprintConfigurationsPaginatorName = Literal[
     "list_environment_blueprint_configurations"
 ]
 ListEnvironmentBlueprintsPaginatorName = Literal["list_environment_blueprints"]
 ListEnvironmentProfilesPaginatorName = Literal["list_environment_profiles"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
+ListMetadataGenerationRunsPaginatorName = Literal["list_metadata_generation_runs"]
 ListNotificationsPaginatorName = Literal["list_notifications"]
 ListProjectMembershipsPaginatorName = Literal["list_project_memberships"]
 ListProjectsPaginatorName = Literal["list_projects"]
 ListSubscriptionGrantsPaginatorName = Literal["list_subscription_grants"]
 ListSubscriptionRequestsPaginatorName = Literal["list_subscription_requests"]
 ListSubscriptionTargetsPaginatorName = Literal["list_subscription_targets"]
 ListSubscriptionsPaginatorName = Literal["list_subscriptions"]
 ListingStatusType = Literal["ACTIVE", "CREATING", "INACTIVE"]
+MetadataGenerationRunStatusType = Literal[
+    "CANCELED", "FAILED", "IN_PROGRESS", "SUBMITTED", "SUCCEEDED"
+]
+MetadataGenerationRunTypeType = Literal["BUSINESS_DESCRIPTIONS"]
+MetadataGenerationTargetTypeType = Literal["ASSET"]
 NotificationResourceTypeType = Literal["PROJECT"]
 NotificationRoleType = Literal[
     "DOMAIN_OWNER", "PROJECT_CONTRIBUTOR", "PROJECT_OWNER", "PROJECT_SUBSCRIBER", "PROJECT_VIEWER"
 ]
 NotificationTypeType = Literal["EVENT", "TASK"]
 ProjectStatusType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 RejectRuleBehaviorType = Literal["ALL", "NONE"]
@@ -312,14 +322,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -330,14 +341,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -355,14 +367,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -385,14 +398,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -453,15 +467,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -641,14 +654,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -687,14 +701,15 @@
     "list_data_source_runs",
     "list_data_sources",
     "list_domains",
     "list_environment_blueprint_configurations",
     "list_environment_blueprints",
     "list_environment_profiles",
     "list_environments",
+    "list_metadata_generation_runs",
     "list_notifications",
     "list_project_memberships",
     "list_projects",
     "list_subscription_grants",
     "list_subscription_requests",
     "list_subscription_targets",
     "list_subscriptions",
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/literals.pyi` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,26 @@
     "ListDataSourceRunsPaginatorName",
     "ListDataSourcesPaginatorName",
     "ListDomainsPaginatorName",
     "ListEnvironmentBlueprintConfigurationsPaginatorName",
     "ListEnvironmentBlueprintsPaginatorName",
     "ListEnvironmentProfilesPaginatorName",
     "ListEnvironmentsPaginatorName",
+    "ListMetadataGenerationRunsPaginatorName",
     "ListNotificationsPaginatorName",
     "ListProjectMembershipsPaginatorName",
     "ListProjectsPaginatorName",
     "ListSubscriptionGrantsPaginatorName",
     "ListSubscriptionRequestsPaginatorName",
     "ListSubscriptionTargetsPaginatorName",
     "ListSubscriptionsPaginatorName",
     "ListingStatusType",
+    "MetadataGenerationRunStatusType",
+    "MetadataGenerationRunTypeType",
+    "MetadataGenerationTargetTypeType",
     "NotificationResourceTypeType",
     "NotificationRoleType",
     "NotificationTypeType",
     "ProjectStatusType",
     "RejectRuleBehaviorType",
     "SearchGroupProfilesPaginatorName",
     "SearchListingsPaginatorName",
@@ -166,22 +170,28 @@
 ListDomainsPaginatorName = Literal["list_domains"]
 ListEnvironmentBlueprintConfigurationsPaginatorName = Literal[
     "list_environment_blueprint_configurations"
 ]
 ListEnvironmentBlueprintsPaginatorName = Literal["list_environment_blueprints"]
 ListEnvironmentProfilesPaginatorName = Literal["list_environment_profiles"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
+ListMetadataGenerationRunsPaginatorName = Literal["list_metadata_generation_runs"]
 ListNotificationsPaginatorName = Literal["list_notifications"]
 ListProjectMembershipsPaginatorName = Literal["list_project_memberships"]
 ListProjectsPaginatorName = Literal["list_projects"]
 ListSubscriptionGrantsPaginatorName = Literal["list_subscription_grants"]
 ListSubscriptionRequestsPaginatorName = Literal["list_subscription_requests"]
 ListSubscriptionTargetsPaginatorName = Literal["list_subscription_targets"]
 ListSubscriptionsPaginatorName = Literal["list_subscriptions"]
 ListingStatusType = Literal["ACTIVE", "CREATING", "INACTIVE"]
+MetadataGenerationRunStatusType = Literal[
+    "CANCELED", "FAILED", "IN_PROGRESS", "SUBMITTED", "SUCCEEDED"
+]
+MetadataGenerationRunTypeType = Literal["BUSINESS_DESCRIPTIONS"]
+MetadataGenerationTargetTypeType = Literal["ASSET"]
 NotificationResourceTypeType = Literal["PROJECT"]
 NotificationRoleType = Literal[
     "DOMAIN_OWNER", "PROJECT_CONTRIBUTOR", "PROJECT_OWNER", "PROJECT_SUBSCRIBER", "PROJECT_VIEWER"
 ]
 NotificationTypeType = Literal["EVENT", "TASK"]
 ProjectStatusType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 RejectRuleBehaviorType = Literal["ALL", "NONE"]
@@ -312,14 +322,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -330,14 +341,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -355,14 +367,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -385,14 +398,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -453,15 +467,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -641,14 +654,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -687,14 +701,15 @@
     "list_data_source_runs",
     "list_data_sources",
     "list_domains",
     "list_environment_blueprint_configurations",
     "list_environment_blueprints",
     "list_environment_profiles",
     "list_environments",
+    "list_metadata_generation_runs",
     "list_notifications",
     "list_project_memberships",
     "list_projects",
     "list_subscription_grants",
     "list_subscription_requests",
     "list_subscription_targets",
     "list_subscriptions",
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/paginator.py` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         ListDataSourceRunsPaginator,
         ListDataSourcesPaginator,
         ListDomainsPaginator,
         ListEnvironmentBlueprintConfigurationsPaginator,
         ListEnvironmentBlueprintsPaginator,
         ListEnvironmentProfilesPaginator,
         ListEnvironmentsPaginator,
+        ListMetadataGenerationRunsPaginator,
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
@@ -41,14 +42,15 @@
     list_data_source_runs_paginator: ListDataSourceRunsPaginator = client.get_paginator("list_data_source_runs")
     list_data_sources_paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
     list_environment_blueprint_configurations_paginator: ListEnvironmentBlueprintConfigurationsPaginator = client.get_paginator("list_environment_blueprint_configurations")
     list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator("list_environment_blueprints")
     list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator("list_environment_profiles")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+    list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator("list_metadata_generation_runs")
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
@@ -69,14 +71,15 @@
     DataAssetActivityStatusType,
     DataSourceRunStatusType,
     DataSourceStatusType,
     DomainStatusType,
     EnvironmentStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
+    MetadataGenerationRunStatusType,
     NotificationTypeType,
     SortKeyType,
     SortOrderType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
     TypesSearchScopeType,
@@ -89,14 +92,15 @@
     ListDataSourceRunsOutputTypeDef,
     ListDataSourcesOutputTypeDef,
     ListDomainsOutputTypeDef,
     ListEnvironmentBlueprintConfigurationsOutputTypeDef,
     ListEnvironmentBlueprintsOutputTypeDef,
     ListEnvironmentProfilesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListMetadataGenerationRunsOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
@@ -122,14 +126,15 @@
     "ListDataSourceRunsPaginator",
     "ListDataSourcesPaginator",
     "ListDomainsPaginator",
     "ListEnvironmentBlueprintConfigurationsPaginator",
     "ListEnvironmentBlueprintsPaginator",
     "ListEnvironmentProfilesPaginator",
     "ListEnvironmentsPaginator",
+    "ListMetadataGenerationRunsPaginator",
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
@@ -327,14 +332,34 @@
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listenvironmentspaginator)
         """
 
 
+class ListMetadataGenerationRunsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListMetadataGenerationRuns)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listmetadatagenerationrunspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domainIdentifier: str,
+        status: MetadataGenerationRunStatusType = ...,
+        type: Literal["BUSINESS_DESCRIPTIONS"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListMetadataGenerationRunsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListMetadataGenerationRuns.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listmetadatagenerationrunspaginator)
+        """
+
+
 class ListNotificationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListNotifications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listnotificationspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/paginator.pyi` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         ListDataSourceRunsPaginator,
         ListDataSourcesPaginator,
         ListDomainsPaginator,
         ListEnvironmentBlueprintConfigurationsPaginator,
         ListEnvironmentBlueprintsPaginator,
         ListEnvironmentProfilesPaginator,
         ListEnvironmentsPaginator,
+        ListMetadataGenerationRunsPaginator,
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
@@ -41,14 +42,15 @@
     list_data_source_runs_paginator: ListDataSourceRunsPaginator = client.get_paginator("list_data_source_runs")
     list_data_sources_paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
     list_environment_blueprint_configurations_paginator: ListEnvironmentBlueprintConfigurationsPaginator = client.get_paginator("list_environment_blueprint_configurations")
     list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator("list_environment_blueprints")
     list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator("list_environment_profiles")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+    list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator("list_metadata_generation_runs")
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
@@ -69,14 +71,15 @@
     DataAssetActivityStatusType,
     DataSourceRunStatusType,
     DataSourceStatusType,
     DomainStatusType,
     EnvironmentStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
+    MetadataGenerationRunStatusType,
     NotificationTypeType,
     SortKeyType,
     SortOrderType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
     TypesSearchScopeType,
@@ -89,14 +92,15 @@
     ListDataSourceRunsOutputTypeDef,
     ListDataSourcesOutputTypeDef,
     ListDomainsOutputTypeDef,
     ListEnvironmentBlueprintConfigurationsOutputTypeDef,
     ListEnvironmentBlueprintsOutputTypeDef,
     ListEnvironmentProfilesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
+    ListMetadataGenerationRunsOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
@@ -122,14 +126,15 @@
     "ListDataSourceRunsPaginator",
     "ListDataSourcesPaginator",
     "ListDomainsPaginator",
     "ListEnvironmentBlueprintConfigurationsPaginator",
     "ListEnvironmentBlueprintsPaginator",
     "ListEnvironmentProfilesPaginator",
     "ListEnvironmentsPaginator",
+    "ListMetadataGenerationRunsPaginator",
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
@@ -316,14 +321,33 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listenvironmentspaginator)
         """
 
+class ListMetadataGenerationRunsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListMetadataGenerationRuns)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listmetadatagenerationrunspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domainIdentifier: str,
+        status: MetadataGenerationRunStatusType = ...,
+        type: Literal["BUSINESS_DESCRIPTIONS"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListMetadataGenerationRunsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListMetadataGenerationRuns.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listmetadatagenerationrunspaginator)
+        """
+
 class ListNotificationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListNotifications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listnotificationspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/type_defs.py` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     FormTypeStatusType,
     GlossaryStatusType,
     GlossaryTermStatusType,
     GroupProfileStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
     ListingStatusType,
+    MetadataGenerationRunStatusType,
     NotificationRoleType,
     NotificationTypeType,
     ProjectStatusType,
     RejectRuleBehaviorType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantOverallStatusType,
@@ -82,14 +83,15 @@
     "AssetListingDetailsTypeDef",
     "AssetListingItemAdditionalAttributesTypeDef",
     "DetailedGlossaryTermTypeDef",
     "AssetRevisionTypeDef",
     "AssetTargetNameMapTypeDef",
     "FormEntryOutputTypeDef",
     "BusinessNameGenerationConfigurationTypeDef",
+    "CancelMetadataGenerationRunInputRequestTypeDef",
     "CancelSubscriptionInputRequestTypeDef",
     "CloudFormationPropertiesTypeDef",
     "ConfigurableActionParameterTypeDef",
     "FormInputTypeDef",
     "FormEntryInputTypeDef",
     "RecommendationConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
@@ -147,14 +149,16 @@
     "GetEnvironmentProfileInputRequestTypeDef",
     "GetFormTypeInputRequestTypeDef",
     "GetGlossaryInputRequestTypeDef",
     "GetGlossaryTermInputRequestTypeDef",
     "GetGroupProfileInputRequestTypeDef",
     "GetIamPortalLoginUrlInputRequestTypeDef",
     "GetListingInputRequestTypeDef",
+    "GetMetadataGenerationRunInputRequestTypeDef",
+    "MetadataGenerationRunTargetTypeDef",
     "GetProjectInputRequestTypeDef",
     "GetSubscriptionGrantInputRequestTypeDef",
     "GetSubscriptionInputRequestTypeDef",
     "GetSubscriptionRequestDetailsInputRequestTypeDef",
     "GetSubscriptionTargetInputRequestTypeDef",
     "GetUserProfileInputRequestTypeDef",
     "GlossaryItemTypeDef",
@@ -170,14 +174,15 @@
     "ListDataSourceRunsInputRequestTypeDef",
     "ListDataSourcesInputRequestTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListEnvironmentBlueprintConfigurationsInputRequestTypeDef",
     "ListEnvironmentBlueprintsInputRequestTypeDef",
     "ListEnvironmentProfilesInputRequestTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
+    "ListMetadataGenerationRunsInputRequestTypeDef",
     "TimestampTypeDef",
     "ListProjectMembershipsInputRequestTypeDef",
     "ListProjectsInputRequestTypeDef",
     "ListSubscriptionGrantsInputRequestTypeDef",
     "ListSubscriptionRequestsInputRequestTypeDef",
     "ListSubscriptionTargetsInputRequestTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
@@ -219,14 +224,15 @@
     "GetEnvironmentBlueprintConfigurationOutputTypeDef",
     "GetGlossaryOutputTypeDef",
     "GetGroupProfileOutputTypeDef",
     "GetIamPortalLoginUrlOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutEnvironmentBlueprintConfigurationOutputTypeDef",
     "RejectPredictionsOutputTypeDef",
+    "StartMetadataGenerationRunOutputTypeDef",
     "UpdateGlossaryOutputTypeDef",
     "UpdateGroupProfileOutputTypeDef",
     "AssetItemAdditionalAttributesTypeDef",
     "GetAssetOutputTypeDef",
     "AssetListingItemTypeDef",
     "AssetListingTypeDef",
     "SubscribedAssetListingTypeDef",
@@ -281,27 +287,31 @@
     "ListEnvironmentsOutputTypeDef",
     "SubscribedAssetTypeDef",
     "UpdateSubscriptionGrantStatusInputRequestTypeDef",
     "FilterClauseTypeDef",
     "RelationalFilterConfigurationTypeDef",
     "FormTypeDataTypeDef",
     "GetFormTypeOutputTypeDef",
+    "GetMetadataGenerationRunOutputTypeDef",
+    "MetadataGenerationRunItemTypeDef",
+    "StartMetadataGenerationRunInputRequestTypeDef",
     "GlossaryTermItemPaginatorTypeDef",
     "GrantedEntityInputTypeDef",
     "GrantedEntityTypeDef",
     "SearchGroupProfilesOutputTypeDef",
     "ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef",
     "ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef",
     "ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef",
     "ListDataSourcesInputListDataSourcesPaginateTypeDef",
     "ListDomainsInputListDomainsPaginateTypeDef",
     "ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef",
     "ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef",
     "ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    "ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef",
     "ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef",
     "ListProjectsInputListProjectsPaginateTypeDef",
     "ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef",
     "ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef",
     "ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef",
     "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef",
@@ -338,14 +348,15 @@
     "UpdateEnvironmentOutputTypeDef",
     "SearchInputSearchPaginateTypeDef",
     "SearchListingsInputSearchListingsPaginateTypeDef",
     "SearchTypesInputSearchTypesPaginateTypeDef",
     "GlueRunConfigurationInputTypeDef",
     "GlueRunConfigurationOutputTypeDef",
     "SearchTypesResultItemTypeDef",
+    "ListMetadataGenerationRunsOutputTypeDef",
     "CreateSubscriptionGrantInputRequestTypeDef",
     "CreateSubscriptionGrantOutputTypeDef",
     "DeleteSubscriptionGrantOutputTypeDef",
     "GetSubscriptionGrantOutputTypeDef",
     "SubscriptionGrantSummaryTypeDef",
     "UpdateSubscriptionGrantStatusOutputTypeDef",
     "ProjectMemberTypeDef",
@@ -391,33 +402,34 @@
     "ListSubscriptionRequestsOutputTypeDef",
     "ListSubscriptionsOutputTypeDef",
 )
 
 AcceptChoiceTypeDef = TypedDict(
     "AcceptChoiceTypeDef",
     {
+        "predictionTarget": str,
+        "editedValue": NotRequired[str],
         "predictionChoice": NotRequired[int],
-        "predictionTarget": NotRequired[str],
     },
 )
 AcceptRuleTypeDef = TypedDict(
     "AcceptRuleTypeDef",
     {
         "rule": NotRequired[AcceptRuleBehaviorType],
         "threshold": NotRequired[float],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 AcceptSubscriptionRequestInputRequestTypeDef = TypedDict(
     "AcceptSubscriptionRequestInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
@@ -480,14 +492,21 @@
 )
 BusinessNameGenerationConfigurationTypeDef = TypedDict(
     "BusinessNameGenerationConfigurationTypeDef",
     {
         "enabled": NotRequired[bool],
     },
 )
+CancelMetadataGenerationRunInputRequestTypeDef = TypedDict(
+    "CancelMetadataGenerationRunInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "identifier": str,
+    },
+)
 CancelSubscriptionInputRequestTypeDef = TypedDict(
     "CancelSubscriptionInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
     },
 )
@@ -994,14 +1013,29 @@
     "GetListingInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
         "listingRevision": NotRequired[str],
     },
 )
+GetMetadataGenerationRunInputRequestTypeDef = TypedDict(
+    "GetMetadataGenerationRunInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "identifier": str,
+    },
+)
+MetadataGenerationRunTargetTypeDef = TypedDict(
+    "MetadataGenerationRunTargetTypeDef",
+    {
+        "identifier": str,
+        "type": Literal["ASSET"],
+        "revision": NotRequired[str],
+    },
+)
 GetProjectInputRequestTypeDef = TypedDict(
     "GetProjectInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
     },
 )
@@ -1200,14 +1234,24 @@
         "maxResults": NotRequired[int],
         "name": NotRequired[str],
         "nextToken": NotRequired[str],
         "provider": NotRequired[str],
         "status": NotRequired[EnvironmentStatusType],
     },
 )
+ListMetadataGenerationRunsInputRequestTypeDef = TypedDict(
+    "ListMetadataGenerationRunsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "status": NotRequired[MetadataGenerationRunStatusType],
+        "type": NotRequired[Literal["BUSINESS_DESCRIPTIONS"]],
+    },
+)
 TimestampTypeDef = Union[datetime, str]
 ListProjectMembershipsInputRequestTypeDef = TypedDict(
     "ListProjectMembershipsInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "projectIdentifier": str,
         "maxResults": NotRequired[int],
@@ -1329,16 +1373,16 @@
     {
         "workgroupName": str,
     },
 )
 RejectChoiceTypeDef = TypedDict(
     "RejectChoiceTypeDef",
     {
+        "predictionTarget": str,
         "predictionChoices": NotRequired[Sequence[int]],
-        "predictionTarget": NotRequired[str],
     },
 )
 RejectRuleTypeDef = TypedDict(
     "RejectRuleTypeDef",
     {
         "rule": NotRequired[RejectRuleBehaviorType],
         "threshold": NotRequired[float],
@@ -1643,14 +1687,27 @@
     {
         "assetId": str,
         "assetRevision": str,
         "domainId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartMetadataGenerationRunOutputTypeDef = TypedDict(
+    "StartMetadataGenerationRunOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "createdBy": str,
+        "domainId": str,
+        "id": str,
+        "owningProjectId": str,
+        "status": MetadataGenerationRunStatusType,
+        "type": Literal["BUSINESS_DESCRIPTIONS"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateGlossaryOutputTypeDef = TypedDict(
     "UpdateGlossaryOutputTypeDef",
     {
         "description": str,
         "domainId": str,
         "id": str,
         "name": str,
@@ -2498,14 +2555,51 @@
         "originProjectId": str,
         "owningProjectId": str,
         "revision": str,
         "status": FormTypeStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetMetadataGenerationRunOutputTypeDef = TypedDict(
+    "GetMetadataGenerationRunOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "createdBy": str,
+        "domainId": str,
+        "id": str,
+        "owningProjectId": str,
+        "status": MetadataGenerationRunStatusType,
+        "target": MetadataGenerationRunTargetTypeDef,
+        "type": Literal["BUSINESS_DESCRIPTIONS"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+MetadataGenerationRunItemTypeDef = TypedDict(
+    "MetadataGenerationRunItemTypeDef",
+    {
+        "domainId": str,
+        "id": str,
+        "owningProjectId": str,
+        "createdAt": NotRequired[datetime],
+        "createdBy": NotRequired[str],
+        "status": NotRequired[MetadataGenerationRunStatusType],
+        "target": NotRequired[MetadataGenerationRunTargetTypeDef],
+        "type": NotRequired[Literal["BUSINESS_DESCRIPTIONS"]],
+    },
+)
+StartMetadataGenerationRunInputRequestTypeDef = TypedDict(
+    "StartMetadataGenerationRunInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "owningProjectIdentifier": str,
+        "target": MetadataGenerationRunTargetTypeDef,
+        "type": Literal["BUSINESS_DESCRIPTIONS"],
+        "clientToken": NotRequired[str],
+    },
+)
 GlossaryTermItemPaginatorTypeDef = TypedDict(
     "GlossaryTermItemPaginatorTypeDef",
     {
         "domainId": str,
         "glossaryId": str,
         "id": str,
         "name": str,
@@ -2623,14 +2717,23 @@
         "environmentProfileIdentifier": NotRequired[str],
         "name": NotRequired[str],
         "provider": NotRequired[str],
         "status": NotRequired[EnvironmentStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef = TypedDict(
+    "ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef",
+    {
+        "domainIdentifier": str,
+        "status": NotRequired[MetadataGenerationRunStatusType],
+        "type": NotRequired[Literal["BUSINESS_DESCRIPTIONS"]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef = TypedDict(
     "ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef",
     {
         "domainIdentifier": str,
         "projectIdentifier": str,
         "sortBy": NotRequired[Literal["NAME"]],
         "sortOrder": NotRequired[SortOrderType],
@@ -3156,14 +3259,22 @@
 SearchTypesResultItemTypeDef = TypedDict(
     "SearchTypesResultItemTypeDef",
     {
         "assetTypeItem": NotRequired[AssetTypeItemTypeDef],
         "formTypeItem": NotRequired[FormTypeDataTypeDef],
     },
 )
+ListMetadataGenerationRunsOutputTypeDef = TypedDict(
+    "ListMetadataGenerationRunsOutputTypeDef",
+    {
+        "items": List[MetadataGenerationRunItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateSubscriptionGrantInputRequestTypeDef = TypedDict(
     "CreateSubscriptionGrantInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "environmentIdentifier": str,
         "grantedEntity": GrantedEntityInputTypeDef,
         "subscriptionTargetIdentifier": str,
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone/type_defs.pyi` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     FormTypeStatusType,
     GlossaryStatusType,
     GlossaryTermStatusType,
     GroupProfileStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
     ListingStatusType,
+    MetadataGenerationRunStatusType,
     NotificationRoleType,
     NotificationTypeType,
     ProjectStatusType,
     RejectRuleBehaviorType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantOverallStatusType,
@@ -82,14 +83,15 @@
     "AssetListingDetailsTypeDef",
     "AssetListingItemAdditionalAttributesTypeDef",
     "DetailedGlossaryTermTypeDef",
     "AssetRevisionTypeDef",
     "AssetTargetNameMapTypeDef",
     "FormEntryOutputTypeDef",
     "BusinessNameGenerationConfigurationTypeDef",
+    "CancelMetadataGenerationRunInputRequestTypeDef",
     "CancelSubscriptionInputRequestTypeDef",
     "CloudFormationPropertiesTypeDef",
     "ConfigurableActionParameterTypeDef",
     "FormInputTypeDef",
     "FormEntryInputTypeDef",
     "RecommendationConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
@@ -147,14 +149,16 @@
     "GetEnvironmentProfileInputRequestTypeDef",
     "GetFormTypeInputRequestTypeDef",
     "GetGlossaryInputRequestTypeDef",
     "GetGlossaryTermInputRequestTypeDef",
     "GetGroupProfileInputRequestTypeDef",
     "GetIamPortalLoginUrlInputRequestTypeDef",
     "GetListingInputRequestTypeDef",
+    "GetMetadataGenerationRunInputRequestTypeDef",
+    "MetadataGenerationRunTargetTypeDef",
     "GetProjectInputRequestTypeDef",
     "GetSubscriptionGrantInputRequestTypeDef",
     "GetSubscriptionInputRequestTypeDef",
     "GetSubscriptionRequestDetailsInputRequestTypeDef",
     "GetSubscriptionTargetInputRequestTypeDef",
     "GetUserProfileInputRequestTypeDef",
     "GlossaryItemTypeDef",
@@ -170,14 +174,15 @@
     "ListDataSourceRunsInputRequestTypeDef",
     "ListDataSourcesInputRequestTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListEnvironmentBlueprintConfigurationsInputRequestTypeDef",
     "ListEnvironmentBlueprintsInputRequestTypeDef",
     "ListEnvironmentProfilesInputRequestTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
+    "ListMetadataGenerationRunsInputRequestTypeDef",
     "TimestampTypeDef",
     "ListProjectMembershipsInputRequestTypeDef",
     "ListProjectsInputRequestTypeDef",
     "ListSubscriptionGrantsInputRequestTypeDef",
     "ListSubscriptionRequestsInputRequestTypeDef",
     "ListSubscriptionTargetsInputRequestTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
@@ -219,14 +224,15 @@
     "GetEnvironmentBlueprintConfigurationOutputTypeDef",
     "GetGlossaryOutputTypeDef",
     "GetGroupProfileOutputTypeDef",
     "GetIamPortalLoginUrlOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutEnvironmentBlueprintConfigurationOutputTypeDef",
     "RejectPredictionsOutputTypeDef",
+    "StartMetadataGenerationRunOutputTypeDef",
     "UpdateGlossaryOutputTypeDef",
     "UpdateGroupProfileOutputTypeDef",
     "AssetItemAdditionalAttributesTypeDef",
     "GetAssetOutputTypeDef",
     "AssetListingItemTypeDef",
     "AssetListingTypeDef",
     "SubscribedAssetListingTypeDef",
@@ -281,27 +287,31 @@
     "ListEnvironmentsOutputTypeDef",
     "SubscribedAssetTypeDef",
     "UpdateSubscriptionGrantStatusInputRequestTypeDef",
     "FilterClauseTypeDef",
     "RelationalFilterConfigurationTypeDef",
     "FormTypeDataTypeDef",
     "GetFormTypeOutputTypeDef",
+    "GetMetadataGenerationRunOutputTypeDef",
+    "MetadataGenerationRunItemTypeDef",
+    "StartMetadataGenerationRunInputRequestTypeDef",
     "GlossaryTermItemPaginatorTypeDef",
     "GrantedEntityInputTypeDef",
     "GrantedEntityTypeDef",
     "SearchGroupProfilesOutputTypeDef",
     "ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef",
     "ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef",
     "ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef",
     "ListDataSourcesInputListDataSourcesPaginateTypeDef",
     "ListDomainsInputListDomainsPaginateTypeDef",
     "ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef",
     "ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef",
     "ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    "ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef",
     "ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef",
     "ListProjectsInputListProjectsPaginateTypeDef",
     "ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef",
     "ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef",
     "ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef",
     "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef",
@@ -338,14 +348,15 @@
     "UpdateEnvironmentOutputTypeDef",
     "SearchInputSearchPaginateTypeDef",
     "SearchListingsInputSearchListingsPaginateTypeDef",
     "SearchTypesInputSearchTypesPaginateTypeDef",
     "GlueRunConfigurationInputTypeDef",
     "GlueRunConfigurationOutputTypeDef",
     "SearchTypesResultItemTypeDef",
+    "ListMetadataGenerationRunsOutputTypeDef",
     "CreateSubscriptionGrantInputRequestTypeDef",
     "CreateSubscriptionGrantOutputTypeDef",
     "DeleteSubscriptionGrantOutputTypeDef",
     "GetSubscriptionGrantOutputTypeDef",
     "SubscriptionGrantSummaryTypeDef",
     "UpdateSubscriptionGrantStatusOutputTypeDef",
     "ProjectMemberTypeDef",
@@ -391,33 +402,34 @@
     "ListSubscriptionRequestsOutputTypeDef",
     "ListSubscriptionsOutputTypeDef",
 )
 
 AcceptChoiceTypeDef = TypedDict(
     "AcceptChoiceTypeDef",
     {
+        "predictionTarget": str,
+        "editedValue": NotRequired[str],
         "predictionChoice": NotRequired[int],
-        "predictionTarget": NotRequired[str],
     },
 )
 AcceptRuleTypeDef = TypedDict(
     "AcceptRuleTypeDef",
     {
         "rule": NotRequired[AcceptRuleBehaviorType],
         "threshold": NotRequired[float],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 AcceptSubscriptionRequestInputRequestTypeDef = TypedDict(
     "AcceptSubscriptionRequestInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
@@ -480,14 +492,21 @@
 )
 BusinessNameGenerationConfigurationTypeDef = TypedDict(
     "BusinessNameGenerationConfigurationTypeDef",
     {
         "enabled": NotRequired[bool],
     },
 )
+CancelMetadataGenerationRunInputRequestTypeDef = TypedDict(
+    "CancelMetadataGenerationRunInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "identifier": str,
+    },
+)
 CancelSubscriptionInputRequestTypeDef = TypedDict(
     "CancelSubscriptionInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
     },
 )
@@ -994,14 +1013,29 @@
     "GetListingInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
         "listingRevision": NotRequired[str],
     },
 )
+GetMetadataGenerationRunInputRequestTypeDef = TypedDict(
+    "GetMetadataGenerationRunInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "identifier": str,
+    },
+)
+MetadataGenerationRunTargetTypeDef = TypedDict(
+    "MetadataGenerationRunTargetTypeDef",
+    {
+        "identifier": str,
+        "type": Literal["ASSET"],
+        "revision": NotRequired[str],
+    },
+)
 GetProjectInputRequestTypeDef = TypedDict(
     "GetProjectInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "identifier": str,
     },
 )
@@ -1200,14 +1234,24 @@
         "maxResults": NotRequired[int],
         "name": NotRequired[str],
         "nextToken": NotRequired[str],
         "provider": NotRequired[str],
         "status": NotRequired[EnvironmentStatusType],
     },
 )
+ListMetadataGenerationRunsInputRequestTypeDef = TypedDict(
+    "ListMetadataGenerationRunsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "status": NotRequired[MetadataGenerationRunStatusType],
+        "type": NotRequired[Literal["BUSINESS_DESCRIPTIONS"]],
+    },
+)
 TimestampTypeDef = Union[datetime, str]
 ListProjectMembershipsInputRequestTypeDef = TypedDict(
     "ListProjectMembershipsInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "projectIdentifier": str,
         "maxResults": NotRequired[int],
@@ -1329,16 +1373,16 @@
     {
         "workgroupName": str,
     },
 )
 RejectChoiceTypeDef = TypedDict(
     "RejectChoiceTypeDef",
     {
+        "predictionTarget": str,
         "predictionChoices": NotRequired[Sequence[int]],
-        "predictionTarget": NotRequired[str],
     },
 )
 RejectRuleTypeDef = TypedDict(
     "RejectRuleTypeDef",
     {
         "rule": NotRequired[RejectRuleBehaviorType],
         "threshold": NotRequired[float],
@@ -1643,14 +1687,27 @@
     {
         "assetId": str,
         "assetRevision": str,
         "domainId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartMetadataGenerationRunOutputTypeDef = TypedDict(
+    "StartMetadataGenerationRunOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "createdBy": str,
+        "domainId": str,
+        "id": str,
+        "owningProjectId": str,
+        "status": MetadataGenerationRunStatusType,
+        "type": Literal["BUSINESS_DESCRIPTIONS"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateGlossaryOutputTypeDef = TypedDict(
     "UpdateGlossaryOutputTypeDef",
     {
         "description": str,
         "domainId": str,
         "id": str,
         "name": str,
@@ -2498,14 +2555,51 @@
         "originProjectId": str,
         "owningProjectId": str,
         "revision": str,
         "status": FormTypeStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+GetMetadataGenerationRunOutputTypeDef = TypedDict(
+    "GetMetadataGenerationRunOutputTypeDef",
+    {
+        "createdAt": datetime,
+        "createdBy": str,
+        "domainId": str,
+        "id": str,
+        "owningProjectId": str,
+        "status": MetadataGenerationRunStatusType,
+        "target": MetadataGenerationRunTargetTypeDef,
+        "type": Literal["BUSINESS_DESCRIPTIONS"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+MetadataGenerationRunItemTypeDef = TypedDict(
+    "MetadataGenerationRunItemTypeDef",
+    {
+        "domainId": str,
+        "id": str,
+        "owningProjectId": str,
+        "createdAt": NotRequired[datetime],
+        "createdBy": NotRequired[str],
+        "status": NotRequired[MetadataGenerationRunStatusType],
+        "target": NotRequired[MetadataGenerationRunTargetTypeDef],
+        "type": NotRequired[Literal["BUSINESS_DESCRIPTIONS"]],
+    },
+)
+StartMetadataGenerationRunInputRequestTypeDef = TypedDict(
+    "StartMetadataGenerationRunInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "owningProjectIdentifier": str,
+        "target": MetadataGenerationRunTargetTypeDef,
+        "type": Literal["BUSINESS_DESCRIPTIONS"],
+        "clientToken": NotRequired[str],
+    },
+)
 GlossaryTermItemPaginatorTypeDef = TypedDict(
     "GlossaryTermItemPaginatorTypeDef",
     {
         "domainId": str,
         "glossaryId": str,
         "id": str,
         "name": str,
@@ -2623,14 +2717,23 @@
         "environmentProfileIdentifier": NotRequired[str],
         "name": NotRequired[str],
         "provider": NotRequired[str],
         "status": NotRequired[EnvironmentStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef = TypedDict(
+    "ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef",
+    {
+        "domainIdentifier": str,
+        "status": NotRequired[MetadataGenerationRunStatusType],
+        "type": NotRequired[Literal["BUSINESS_DESCRIPTIONS"]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef = TypedDict(
     "ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef",
     {
         "domainIdentifier": str,
         "projectIdentifier": str,
         "sortBy": NotRequired[Literal["NAME"]],
         "sortOrder": NotRequired[SortOrderType],
@@ -3156,14 +3259,22 @@
 SearchTypesResultItemTypeDef = TypedDict(
     "SearchTypesResultItemTypeDef",
     {
         "assetTypeItem": NotRequired[AssetTypeItemTypeDef],
         "formTypeItem": NotRequired[FormTypeDataTypeDef],
     },
 )
+ListMetadataGenerationRunsOutputTypeDef = TypedDict(
+    "ListMetadataGenerationRunsOutputTypeDef",
+    {
+        "items": List[MetadataGenerationRunItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateSubscriptionGrantInputRequestTypeDef = TypedDict(
     "CreateSubscriptionGrantInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "environmentIdentifier": str,
         "grantedEntity": GrantedEntityInputTypeDef,
         "subscriptionTargetIdentifier": str,
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/PKG-INFO` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datazone
-Version: 1.34.31
-Summary: Type annotations for boto3.DataZone 1.34.31 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.75
+Summary: Type annotations for boto3.DataZone 1.34.75 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datazone.svg?color=blue)](https://pypi.org/project/mypy-boto3-datazone)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datazone)](https://pepy.tech/project/mypy-boto3-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataZone 1.34.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[boto3.DataZone 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datazone docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +289,15 @@
     ListDataSourceRunsPaginator,
     ListDataSourcesPaginator,
     ListDomainsPaginator,
     ListEnvironmentBlueprintConfigurationsPaginator,
     ListEnvironmentBlueprintsPaginator,
     ListEnvironmentProfilesPaginator,
     ListEnvironmentsPaginator,
+    ListMetadataGenerationRunsPaginator,
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionTargetsPaginator,
     ListSubscriptionsPaginator,
@@ -328,14 +329,17 @@
 list_environment_blueprints_paginator: ListEnvironmentBlueprintsPaginator = client.get_paginator(
     "list_environment_blueprints"
 )
 list_environment_profiles_paginator: ListEnvironmentProfilesPaginator = client.get_paginator(
     "list_environment_profiles"
 )
 list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
+list_metadata_generation_runs_paginator: ListMetadataGenerationRunsPaginator = client.get_paginator(
+    "list_metadata_generation_runs"
+)
 list_notifications_paginator: ListNotificationsPaginator = client.get_paginator(
     "list_notifications"
 )
 list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator(
     "list_project_memberships"
 )
 list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

### Comparing `mypy-boto3-datazone-1.34.31/mypy_boto3_datazone.egg-info/SOURCES.txt` & `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datazone-1.34.31/setup.py` & `mypy-boto3-datazone-1.34.75/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datazone",
-    version="1.34.31",
+    version="1.34.75",
     packages=["mypy_boto3_datazone"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.DataZone 1.34.31 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.DataZone 1.34.75 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

