# Comparing `tmp/mypy-boto3-lightsail-1.34.41.tar.gz` & `tmp/mypy-boto3-lightsail-1.34.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.34.41.tar", last modified: Tue Feb 13 20:32:22 2024, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.34.75.tar", last modified: Mon Apr  1 20:08:27 2024, max compression
```

## Comparing `mypy-boto3-lightsail-1.34.41.tar` & `mypy-boto3-lightsail-1.34.75.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 20:32:22.728881 mypy-boto3-lightsail-1.34.41/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-02-13 20:32:22.728881 mypy-boto3-lightsail-1.34.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 20:32:22.728881 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   115525 2024-02-13 20:32:05.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   115522 2024-02-13 20:32:05.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-02-13 20:32:06.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    26040 2024-02-13 20:32:06.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22982 2024-02-13 20:32:05.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-02-13 20:32:05.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   141456 2024-02-13 20:32:09.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   141456 2024-02-13 20:32:08.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 20:32:22.728881 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-02-13 20:32:22.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-13 20:32:22.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 20:32:22.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 20:32:22.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-13 20:32:22.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-13 20:32:22.000000 mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 20:32:22.728881 mypy-boto3-lightsail-1.34.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-13 20:32:04.000000 mypy-boto3-lightsail-1.34.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:27.633744 mypy-boto3-lightsail-1.34.75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-04-01 20:08:27.629743 mypy-boto3-lightsail-1.34.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:27.629743 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115861 2024-04-01 20:08:12.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115858 2024-04-01 20:08:12.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-04-01 20:08:12.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26282 2024-04-01 20:08:12.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22982 2024-04-01 20:08:12.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-01 20:08:12.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   142001 2024-04-01 20:08:15.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   142001 2024-04-01 20:08:15.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:27.629743 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-04-01 20:08:27.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-01 20:08:27.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:27.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:27.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:08:27.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 20:08:27.000000 mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:08:27.633744 mypy-boto3-lightsail-1.34.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-01 20:08:11.000000 mypy-boto3-lightsail-1.34.75/setup.py
```

### Comparing `mypy-boto3-lightsail-1.34.41/LICENSE` & `mypy-boto3-lightsail-1.34.75/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.34.41/PKG-INFO` & `mypy-boto3-lightsail-1.34.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.34.41
-Summary: Type annotations for boto3.Lightsail 1.34.41 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.75
+Summary: Type annotations for boto3.Lightsail 1.34.75 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.34.41](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lightsail-1.34.41/README.md` & `mypy-boto3-lightsail-1.34.75/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.34.41](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.34.41\n"
-        "Version:         1.34.41\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.Lightsail 1.34.75\n"
+        "Version:         1.34.75\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.41")
+    print("1.34.75")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     MetricUnitType,
     RegionNameType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     ResourceBucketAccessType,
     ResourceTypeType,
     TreatMissingDataType,
+    ViewerMinimumTlsProtocolVersionEnumType,
 )
 from .paginator import (
     GetActiveNamesPaginator,
     GetBlueprintsPaginator,
     GetBundlesPaginator,
     GetCloudFormationStackRecordsPaginator,
     GetDiskSnapshotsPaginator,
@@ -566,14 +567,16 @@
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...,
+        certificateName: str = ...,
+        viewerMinimumTlsProtocolVersion: ViewerMinimumTlsProtocolVersionEnumType = ...,
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_distribution)
         """
@@ -2104,14 +2107,17 @@
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...,
+        viewerMinimumTlsProtocolVersion: ViewerMinimumTlsProtocolVersionEnumType = ...,
+        certificateName: str = ...,
+        useDefaultCertificate: bool = ...,
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_distribution)
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     MetricUnitType,
     RegionNameType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     ResourceBucketAccessType,
     ResourceTypeType,
     TreatMissingDataType,
+    ViewerMinimumTlsProtocolVersionEnumType,
 )
 from .paginator import (
     GetActiveNamesPaginator,
     GetBlueprintsPaginator,
     GetBundlesPaginator,
     GetCloudFormationStackRecordsPaginator,
     GetDiskSnapshotsPaginator,
@@ -563,14 +564,16 @@
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...,
+        certificateName: str = ...,
+        viewerMinimumTlsProtocolVersion: ViewerMinimumTlsProtocolVersionEnumType = ...,
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_distribution)
         """
@@ -2101,14 +2104,17 @@
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
         cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...,
+        viewerMinimumTlsProtocolVersion: ViewerMinimumTlsProtocolVersionEnumType = ...,
+        certificateName: str = ...,
+        useDefaultCertificate: bool = ...,
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_distribution)
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     "RenewalStatusType",
     "ResourceBucketAccessType",
     "ResourceTypeType",
     "SetupStatusType",
     "StatusType",
     "StatusTypeType",
     "TreatMissingDataType",
+    "ViewerMinimumTlsProtocolVersionEnumType",
     "LightsailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -537,14 +538,17 @@
     "started",
     "starting",
     "stopped",
     "stopping",
 ]
 StatusTypeType = Literal["Active", "Inactive"]
 TreatMissingDataType = Literal["breaching", "ignore", "missing", "notBreaching"]
+ViewerMinimumTlsProtocolVersionEnumType = Literal[
+    "TLSv1.1_2016", "TLSv1.2_2018", "TLSv1.2_2019", "TLSv1.2_2021"
+]
 LightsailServiceName = Literal["lightsail"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -564,14 +568,15 @@
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
@@ -582,14 +587,15 @@
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
@@ -607,14 +613,15 @@
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
@@ -637,14 +644,15 @@
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
@@ -705,15 +713,14 @@
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
@@ -893,14 +900,15 @@
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
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     "RenewalStatusType",
     "ResourceBucketAccessType",
     "ResourceTypeType",
     "SetupStatusType",
     "StatusType",
     "StatusTypeType",
     "TreatMissingDataType",
+    "ViewerMinimumTlsProtocolVersionEnumType",
     "LightsailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -537,14 +538,17 @@
     "started",
     "starting",
     "stopped",
     "stopping",
 ]
 StatusTypeType = Literal["Active", "Inactive"]
 TreatMissingDataType = Literal["breaching", "ignore", "missing", "notBreaching"]
+ViewerMinimumTlsProtocolVersionEnumType = Literal[
+    "TLSv1.1_2016", "TLSv1.2_2018", "TLSv1.2_2019", "TLSv1.2_2021"
+]
 LightsailServiceName = Literal["lightsail"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -564,14 +568,15 @@
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
@@ -582,14 +587,15 @@
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
@@ -607,14 +613,15 @@
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
@@ -637,14 +644,15 @@
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
@@ -705,15 +713,14 @@
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
@@ -893,14 +900,15 @@
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
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
     SetupStatusType,
     StatusType,
     StatusTypeType,
     TreatMissingDataType,
+    ViewerMinimumTlsProtocolVersionEnumType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -635,18 +636,18 @@
         "staticIpName": str,
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
 AttachCertificateToDistributionRequestRequestTypeDef = TypedDict(
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
@@ -943,14 +944,15 @@
 )
 InputOriginTypeDef = TypedDict(
     "InputOriginTypeDef",
     {
         "name": NotRequired[str],
         "regionName": NotRequired[RegionNameType],
         "protocolPolicy": NotRequired[OriginProtocolPolicyEnumType],
+        "responseTimeout": NotRequired[int],
     },
 )
 DomainEntryTypeDef = TypedDict(
     "DomainEntryTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -1720,14 +1722,15 @@
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "name": NotRequired[str],
         "resourceType": NotRequired[ResourceTypeType],
         "regionName": NotRequired[RegionNameType],
         "protocolPolicy": NotRequired[OriginProtocolPolicyEnumType],
+        "responseTimeout": NotRequired[int],
     },
 )
 LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef = TypedDict(
     "LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef",
     {
         "code": NotRequired[LoadBalancerTlsCertificateDnsRecordCreationStateCodeType],
         "message": NotRequired[str],
@@ -3903,14 +3906,16 @@
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
         "cacheBehaviorSettings": NotRequired[CacheSettingsTypeDef],
         "cacheBehaviors": NotRequired[Sequence[CacheBehaviorPerPathTypeDef]],
         "ipAddressType": NotRequired[IpAddressTypeType],
         "tags": NotRequired[Sequence[TagTypeDef]],
+        "certificateName": NotRequired[str],
+        "viewerMinimumTlsProtocolVersion": NotRequired[ViewerMinimumTlsProtocolVersionEnumType],
     },
 )
 LightsailDistributionTypeDef = TypedDict(
     "LightsailDistributionTypeDef",
     {
         "name": NotRequired[str],
         "arn": NotRequired[str],
@@ -3928,25 +3933,29 @@
         "originPublicDNS": NotRequired[str],
         "defaultCacheBehavior": NotRequired[CacheBehaviorTypeDef],
         "cacheBehaviorSettings": NotRequired[CacheSettingsTypeDef],
         "cacheBehaviors": NotRequired[List[CacheBehaviorPerPathTypeDef]],
         "ableToUpdateBundle": NotRequired[bool],
         "ipAddressType": NotRequired[IpAddressTypeType],
         "tags": NotRequired[List[TagTypeDef]],
+        "viewerMinimumTlsProtocolVersion": NotRequired[str],
     },
 )
 UpdateDistributionRequestRequestTypeDef = TypedDict(
     "UpdateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": NotRequired[InputOriginTypeDef],
         "defaultCacheBehavior": NotRequired[CacheBehaviorTypeDef],
         "cacheBehaviorSettings": NotRequired[CacheSettingsTypeDef],
         "cacheBehaviors": NotRequired[Sequence[CacheBehaviorPerPathTypeDef]],
         "isEnabled": NotRequired[bool],
+        "viewerMinimumTlsProtocolVersion": NotRequired[ViewerMinimumTlsProtocolVersionEnumType],
+        "certificateName": NotRequired[str],
+        "useDefaultCertificate": NotRequired[bool],
     },
 )
 GetCloudFormationStackRecordsResultTypeDef = TypedDict(
     "GetCloudFormationStackRecordsResultTypeDef",
     {
         "cloudFormationStackRecords": List[CloudFormationStackRecordTypeDef],
         "nextPageToken": str,
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
     SetupStatusType,
     StatusType,
     StatusTypeType,
     TreatMissingDataType,
+    ViewerMinimumTlsProtocolVersionEnumType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -635,18 +636,18 @@
         "staticIpName": str,
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
 AttachCertificateToDistributionRequestRequestTypeDef = TypedDict(
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
@@ -943,14 +944,15 @@
 )
 InputOriginTypeDef = TypedDict(
     "InputOriginTypeDef",
     {
         "name": NotRequired[str],
         "regionName": NotRequired[RegionNameType],
         "protocolPolicy": NotRequired[OriginProtocolPolicyEnumType],
+        "responseTimeout": NotRequired[int],
     },
 )
 DomainEntryTypeDef = TypedDict(
     "DomainEntryTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -1720,14 +1722,15 @@
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "name": NotRequired[str],
         "resourceType": NotRequired[ResourceTypeType],
         "regionName": NotRequired[RegionNameType],
         "protocolPolicy": NotRequired[OriginProtocolPolicyEnumType],
+        "responseTimeout": NotRequired[int],
     },
 )
 LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef = TypedDict(
     "LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef",
     {
         "code": NotRequired[LoadBalancerTlsCertificateDnsRecordCreationStateCodeType],
         "message": NotRequired[str],
@@ -3903,14 +3906,16 @@
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
         "cacheBehaviorSettings": NotRequired[CacheSettingsTypeDef],
         "cacheBehaviors": NotRequired[Sequence[CacheBehaviorPerPathTypeDef]],
         "ipAddressType": NotRequired[IpAddressTypeType],
         "tags": NotRequired[Sequence[TagTypeDef]],
+        "certificateName": NotRequired[str],
+        "viewerMinimumTlsProtocolVersion": NotRequired[ViewerMinimumTlsProtocolVersionEnumType],
     },
 )
 LightsailDistributionTypeDef = TypedDict(
     "LightsailDistributionTypeDef",
     {
         "name": NotRequired[str],
         "arn": NotRequired[str],
@@ -3928,25 +3933,29 @@
         "originPublicDNS": NotRequired[str],
         "defaultCacheBehavior": NotRequired[CacheBehaviorTypeDef],
         "cacheBehaviorSettings": NotRequired[CacheSettingsTypeDef],
         "cacheBehaviors": NotRequired[List[CacheBehaviorPerPathTypeDef]],
         "ableToUpdateBundle": NotRequired[bool],
         "ipAddressType": NotRequired[IpAddressTypeType],
         "tags": NotRequired[List[TagTypeDef]],
+        "viewerMinimumTlsProtocolVersion": NotRequired[str],
     },
 )
 UpdateDistributionRequestRequestTypeDef = TypedDict(
     "UpdateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": NotRequired[InputOriginTypeDef],
         "defaultCacheBehavior": NotRequired[CacheBehaviorTypeDef],
         "cacheBehaviorSettings": NotRequired[CacheSettingsTypeDef],
         "cacheBehaviors": NotRequired[Sequence[CacheBehaviorPerPathTypeDef]],
         "isEnabled": NotRequired[bool],
+        "viewerMinimumTlsProtocolVersion": NotRequired[ViewerMinimumTlsProtocolVersionEnumType],
+        "certificateName": NotRequired[str],
+        "useDefaultCertificate": NotRequired[bool],
     },
 )
 GetCloudFormationStackRecordsResultTypeDef = TypedDict(
     "GetCloudFormationStackRecordsResultTypeDef",
     {
         "cloudFormationStackRecords": List[CloudFormationStackRecordTypeDef],
         "nextPageToken": str,
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.34.41
-Summary: Type annotations for boto3.Lightsail 1.34.41 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.75
+Summary: Type annotations for boto3.Lightsail 1.34.75 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.34.41](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lightsail-1.34.41/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.34.75/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.34.41/setup.py` & `mypy-boto3-lightsail-1.34.75/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.34.41",
+    version="1.34.75",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Lightsail 1.34.41 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.Lightsail 1.34.75 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

