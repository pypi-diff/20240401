# Comparing `tmp/pulumi_spotinst-3.9.0.tar.gz` & `tmp/pulumi_spotinst-3.9.0a1633346805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_spotinst-3.9.0.tar", last modified: Mon Oct  4 11:58:03 2021, max compression
+gzip compressed data, was "dist/pulumi_spotinst-3.9.0a1633346805.tar", last modified: Mon Oct  4 11:33:18 2021, max compression
```

## Comparing `pulumi_spotinst-3.9.0.tar` & `pulumi_spotinst-3.9.0a1633346805.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24427 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   390544 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    36294 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/beanstalk.py
--rw-r--r--   0 runner    (1001) docker     (121)   214056 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/elastigroup.py
--rw-r--r--   0 runner    (1001) docker     (121)   110597 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/managed_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)   174251 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/mr_scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)    78159 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/ocean.py
--rw-r--r--   0 runner    (1001) docker     (121)    67122 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/ocean_launch_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)   374298 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10178 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/aws/suspension.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   107520 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    70119 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/elastigroup.py
--rw-r--r--   0 runner    (1001) docker     (121)    50526 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/ocean.py
--rw-r--r--   0 runner    (1001) docker     (121)    25539 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/ocean_virtual_node_group.py
--rw-r--r--   0 runner    (1001) docker     (121)   104651 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/config/
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    48394 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    74093 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/ocean.py
--rw-r--r--   0 runner    (1001) docker     (121)    45153 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/ocean_launch_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    49362 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    38721 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/elastigroup_azure_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/
--rw-r--r--   0 runner    (1001) docker     (121)      984 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    57852 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    91014 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/elastigroup.py
--rw-r--r--   0 runner    (1001) docker     (121)    52969 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    78695 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    60628 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/elastigroup.py
--rw-r--r--   0 runner    (1001) docker     (121)    30360 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/ocean_import.py
--rw-r--r--   0 runner    (1001) docker     (121)    45293 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/ocean_launch_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     8943 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/ocean_launch_spec_import.py
--rw-r--r--   0 runner    (1001) docker     (121)    75758 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/gke/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13289 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/health_check.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10318 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11437 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)    10834 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     8180 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    15408 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    12844 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/target.py
--rw-r--r--   0 runner    (1001) docker     (121)    14795 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/multai/target_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    23790 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5873 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    26472 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-10-04 11:58:03.000000 pulumi_spotinst-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/
+-rw-r--r--   0 runner    (1001) docker     (121)     2994 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/
+-rw-r--r--   0 runner    (1001) docker     (121)     2215 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24427 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4152 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)     2516 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   390544 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36294 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/beanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (121)   214056 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/elastigroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)   110597 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/managed_instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)   174251 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/mr_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78159 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67122 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/ocean_launch_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)   374298 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10178 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/suspension.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/
+-rw-r--r--   0 runner    (1001) docker     (121)     1535 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   107520 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    70119 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/elastigroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50526 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25539 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/ocean_virtual_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)   104651 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48394 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74093 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45153 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/ocean_launch_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49362 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38721 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/elastigroup_azure_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57852 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    91014 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/elastigroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52969 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78695 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60628 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/elastigroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30360 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/ocean_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45293 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/ocean_launch_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8943 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/ocean_launch_spec_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75758 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13289 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/health_check.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10318 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11437 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4939 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10834 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8180 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15408 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12844 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/target.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14795 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/target_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23790 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5873 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    26472 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2994 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2021-10-04 11:33:18.000000 pulumi_spotinst-3.9.0a1633346805/setup.py
```

### Comparing `pulumi_spotinst-3.9.0/PKG-INFO` & `pulumi_spotinst-3.9.0a1633346805/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_spotinst
-Version: 3.9.0
+Version: 3.9.0a1633346805
 Summary: A Pulumi package for creating and managing spotinst cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-spotinst
 Description: [![Actions Status](https://github.com/pulumi/pulumi-spotinst/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-spotinst/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fspotinst.svg)](https://www.npmjs.com/package/@pulumi/spotinst)
```

### Comparing `pulumi_spotinst-3.9.0/README.md` & `pulumi_spotinst-3.9.0a1633346805/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/_utilities.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/beanstalk.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/beanstalk.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/elastigroup.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/elastigroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/managed_instance.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/managed_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/mr_scalar.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/mr_scalar.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/ocean.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/ocean.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/ocean_launch_spec.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/ocean_launch_spec.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/aws/suspension.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/aws/suspension.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/azure/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/azure/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/azure/elastigroup.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/elastigroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/azure/ocean.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/ocean.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/azure/ocean_virtual_node_group.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/ocean_virtual_node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/azure/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/config/vars.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/ocean.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/ocean.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/ocean_launch_spec.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/ocean_launch_spec.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/ecs/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/ecs/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/elastigroup_azure_v3.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/elastigroup_azure_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/elastigroup.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/elastigroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gcp/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/elastigroup.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/elastigroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/ocean_import.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/ocean_import.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/ocean_launch_spec.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/ocean_launch_spec.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/ocean_launch_spec_import.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/ocean_launch_spec_import.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/gke/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/gke/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/health_check.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/health_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/__init__.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/_inputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/balancer.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/deployment.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/listener.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/listener.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/routing_rule.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/target.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/target.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/multai/target_set.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/multai/target_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/outputs.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/provider.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst/subscription.py` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/PKG-INFO` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-spotinst
-Version: 3.9.0
+Version: 3.9.0a1633346805
 Summary: A Pulumi package for creating and managing spotinst cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-spotinst
 Description: [![Actions Status](https://github.com/pulumi/pulumi-spotinst/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-spotinst/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fspotinst.svg)](https://www.npmjs.com/package/@pulumi/spotinst)
```

### Comparing `pulumi_spotinst-3.9.0/pulumi_spotinst.egg-info/SOURCES.txt` & `pulumi_spotinst-3.9.0a1633346805/pulumi_spotinst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_spotinst-3.9.0/setup.py` & `pulumi_spotinst-3.9.0a1633346805/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 from subprocess import check_call
 
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'spotinst', '3.9.0'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'spotinst', '3.9.0-alpha.1633346805+e6a7a7e8'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print("""
                 There was an error installing the spotinst resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
-                `pulumi plugin install resource spotinst 3.9.0`
+                `pulumi plugin install resource spotinst 3.9.0-alpha.1633346805+e6a7a7e8`
                 """)
             else:
                 raise
 
 
 def readme():
     with open('README.md', encoding='utf-8') as f:
         return f.read()
 
 
 setup(name='pulumi_spotinst',
-      version='3.9.0',
+      version='3.9.0a1633346805',
       description="A Pulumi package for creating and managing spotinst cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi spotinst',
```

