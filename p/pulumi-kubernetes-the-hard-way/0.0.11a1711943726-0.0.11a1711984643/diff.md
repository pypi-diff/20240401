# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1711943726.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1711984643.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1711943726.tar", last modified: Mon Apr  1 03:57:14 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1711984643.tar", last modified: Mon Apr  1 15:19:23 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726.tar` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.658249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 03:57:14.654249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.650249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     2521 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)      334 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/_enums.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.654249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      318 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      463 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)     4859 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     4045 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)    11932 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/etcd.py
--rw-------   0 runner    (1001) docker     (127)     6520 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.654249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      295 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8177 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)     6927 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/remote/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.654249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      403 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)      942 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1401 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    18602 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    13757 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4166 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)    15417 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.654249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      369 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8252 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    10335 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    19738 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    10270 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    11452 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    12663 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:57:14.654249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 03:57:14.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-01 03:57:14.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 03:57:14.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 03:57:14.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 03:57:14.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      860 2024-04-01 03:57:07.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 03:57:14.658249 pulumi_kubernetes_the_hard_way-0.0.11a1711943726/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.222965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 15:19:23.222965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.218965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     2434 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      334 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.218965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      318 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      463 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     4567 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     2843 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    11932 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/etcd.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.218965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      295 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     8177 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)     6927 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/remote/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.222965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      403 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      942 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1401 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    18602 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    14904 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4166 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)    15417 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.222965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      369 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     8252 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    10335 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    19738 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    10270 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    11452 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    12663 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:23.222965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-01 15:19:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-01 15:19:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:19:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 15:19:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 15:19:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      860 2024-04-01 15:19:15.000000 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:19:23.222965 pulumi_kubernetes_the_hard_way-0.0.11a1711984643/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1711943726
+Version: 0.0.11a1711984643
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/README.md` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from ._enums import *
 from .etcd import *
-from .kubeconfig import *
 from .provider import *
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import pulumi_kubernetes_the_hard_way.config as __config
     config = __config
     import pulumi_kubernetes_the_hard_way.remote as __remote
@@ -30,16 +29,15 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "index",
   "fqn": "pulumi_kubernetes_the_hard_way",
   "classes": {
-   "kubernetes-the-hard-way:index:Etcd": "Etcd",
-   "kubernetes-the-hard-way:index:Kubeconfig": "Kubeconfig"
+   "kubernetes-the-hard-way:index:Etcd": "Etcd"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from .. import config as _config
 from ._enums import *
 from ._inputs import *
 from .certificate import Certificate
 from .root_ca import RootCa
 
 __all__ = ['ClusterPkiArgs', 'ClusterPki']
 
@@ -332,7 +333,27 @@
     @pulumi.getter(name="validityPeriodHours")
     def validity_period_hours(self) -> pulumi.Output[int]:
         """
         Number of hours, after initial issuing, that the certificate will remain valid.
         """
         return pulumi.get(self, "validity_period_hours")
 
+    @pulumi.output_type
+    class GetKubeconfigResult:
+        def __init__(__self__, result=None):
+            if result and not isinstance(result, dict):
+                raise TypeError("Expected argument 'result' to be a dict")
+            pulumi.set(__self__, "result", result)
+
+        @property
+        @pulumi.getter
+        def result(self) -> '_config.outputs.Kubeconfig':
+            return pulumi.get(self, "result")
+
+    def get_kubeconfig(__self__, *,
+                       options: Union[pulumi.Input['_config.KubeconfigAdminOptionsArgs'], pulumi.Input['_config.KubeconfigKubeControllerManagerOptionsArgs'], pulumi.Input['_config.KubeconfigKubeProxyOptionsArgs'], pulumi.Input['_config.KubeconfigKubeSchedulerOptionsArgs'], pulumi.Input['_config.KubeconfigWorkerOptionsArgs']]) -> pulumi.Output['dict']:
+        __args__ = dict()
+        __args__['__self__'] = __self__
+        __args__['options'] = options
+        __result__ = pulumi.runtime.call('kubernetes-the-hard-way:tls:ClusterPki/getKubeconfig', __args__, res=__self__, typ=ClusterPki.GetKubeconfigResult)
+        return __result__.result
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1711943726
+Version: 0.0.11a1711984643
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 README.md
 pyproject.toml
 pulumi_kubernetes_the_hard_way/__init__.py
 pulumi_kubernetes_the_hard_way/_enums.py
 pulumi_kubernetes_the_hard_way/_utilities.py
 pulumi_kubernetes_the_hard_way/etcd.py
-pulumi_kubernetes_the_hard_way/kubeconfig.py
 pulumi_kubernetes_the_hard_way/provider.py
 pulumi_kubernetes_the_hard_way/pulumi-plugin.json
 pulumi_kubernetes_the_hard_way/py.typed
 pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
 pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
 pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
 pulumi_kubernetes_the_hard_way.egg-info/requires.txt
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1711943726/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.11a1711984643/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-command>=0.9.0,<1.0.0", "pulumi-random>=4.0.0,<5.0.0", "pulumi-tls>=5.0.0,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.11a1711943726"
+  version = "0.0.11a1711984643"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

