# Comparing `tmp/pulumi_genesiscloud-0.0.8.tar.gz` & `tmp/pulumi_genesiscloud-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_genesiscloud-0.0.8.tar", last modified: Wed Mar 20 07:16:03 2024, max compression
+gzip compressed data, was "pulumi_genesiscloud-0.0.9.tar", last modified: Sun Mar 31 10:25:24 2024, max compression
```

## Comparing `pulumi_genesiscloud-0.0.8.tar` & `pulumi_genesiscloud-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 07:16:02.999727 pulumi_genesiscloud-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-20 07:16:02.999727 pulumi_genesiscloud-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 07:16:02.999727 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34917 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 07:16:02.999727 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    26357 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    21088 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    46192 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    33074 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17034 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 07:16:02.999727 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 07:16:02.999727 pulumi_genesiscloud-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-20 07:16:02.000000 pulumi_genesiscloud-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 10:25:24.335261 pulumi_genesiscloud-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-31 10:25:24.335261 pulumi_genesiscloud-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 10:25:24.331261 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34917 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 10:25:24.331261 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26357 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49608 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33074 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17034 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 10:25:24.331261 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 10:25:24.335261 pulumi_genesiscloud-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-31 10:25:24.000000 pulumi_genesiscloud-0.0.9/setup.py
```

### Comparing `pulumi_genesiscloud-0.0.8/PKG-INFO` & `pulumi_genesiscloud-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_genesiscloud
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing genesiscloud cloud resources.
 Home-page: https://www.pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/genesiscloud/pulumi-genesiscloud
 Keywords: pulumi genesiscloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_genesiscloud-0.0.8/README.md` & `pulumi_genesiscloud-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/__init__.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/_inputs.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/_utilities.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/config/vars.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/filesystem.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/filesystem.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/floating_ip.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/floating_ip.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                  timeouts: Optional[pulumi.Input['FloatingIpTimeoutsArgs']] = None):
         """
         The set of arguments for constructing a FloatingIp resource.
         :param pulumi.Input[str] region: The region identifier. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The
                value must be one of: ["ARC-IS-HAF-1" "EUC-DE-MUC-1" "NORD-NO-KRS-1"].
         :param pulumi.Input[str] version: The version of the floating IP. - If the value of this attribute changes, Terraform will destroy and recreate the
                resource. - The value must be one of: ["ipv4"].
-        :param pulumi.Input[str] description: The human-readable description set for the floating IP.
+        :param pulumi.Input[str] description: The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         :param pulumi.Input[str] name: The human-readable name for the floating IP.
         """
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "version", version)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
@@ -65,15 +65,15 @@
     def version(self, value: pulumi.Input[str]):
         pulumi.set(self, "version", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The human-readable description set for the floating IP.
+        The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -111,15 +111,15 @@
                  status: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input['FloatingIpTimeoutsArgs']] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering FloatingIp resources.
         :param pulumi.Input[str] created_at: The timestamp when this floating IP was created in RFC 3339.
-        :param pulumi.Input[str] description: The human-readable description set for the floating IP.
+        :param pulumi.Input[str] description: The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         :param pulumi.Input[str] ip_address: The IP address of the floating IP.
         :param pulumi.Input[bool] is_public: Whether the floating IP is public or private. - Sets the default value "true" if the attribute is not set.
         :param pulumi.Input[str] name: The human-readable name for the floating IP.
         :param pulumi.Input[str] region: The region identifier. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The
                value must be one of: ["ARC-IS-HAF-1" "EUC-DE-MUC-1" "NORD-NO-KRS-1"].
         :param pulumi.Input[str] status: The floating IP status.
         :param pulumi.Input[str] updated_at: The timestamp when this image was last updated in RFC 3339.
@@ -159,15 +159,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The human-readable description set for the floating IP.
+        The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -297,15 +297,15 @@
 
         ```sh
          $ pulumi import genesiscloud:index/floatingIp:FloatingIp example 18efeec8-94f0-4776-8ff2-5e9b49c74608
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: The human-readable description set for the floating IP.
+        :param pulumi.Input[str] description: The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         :param pulumi.Input[str] name: The human-readable name for the floating IP.
         :param pulumi.Input[str] region: The region identifier. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The
                value must be one of: ["ARC-IS-HAF-1" "EUC-DE-MUC-1" "NORD-NO-KRS-1"].
         :param pulumi.Input[str] version: The version of the floating IP. - If the value of this attribute changes, Terraform will destroy and recreate the
                resource. - The value must be one of: ["ipv4"].
         """
         ...
@@ -402,15 +402,15 @@
         Get an existing FloatingIp resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The timestamp when this floating IP was created in RFC 3339.
-        :param pulumi.Input[str] description: The human-readable description set for the floating IP.
+        :param pulumi.Input[str] description: The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         :param pulumi.Input[str] ip_address: The IP address of the floating IP.
         :param pulumi.Input[bool] is_public: Whether the floating IP is public or private. - Sets the default value "true" if the attribute is not set.
         :param pulumi.Input[str] name: The human-readable name for the floating IP.
         :param pulumi.Input[str] region: The region identifier. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The
                value must be one of: ["ARC-IS-HAF-1" "EUC-DE-MUC-1" "NORD-NO-KRS-1"].
         :param pulumi.Input[str] status: The floating IP status.
         :param pulumi.Input[str] updated_at: The timestamp when this image was last updated in RFC 3339.
@@ -439,17 +439,17 @@
         """
         The timestamp when this floating IP was created in RFC 3339.
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def description(self) -> pulumi.Output[str]:
         """
-        The human-readable description set for the floating IP.
+        The human-readable description set for the floating IP. - Sets the default value "" if the attribute is not set.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/images.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_genesiscloud as genesiscloud
 
-    base_os_images = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
-        type="base-os",
+    cloud_images = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
+        type="cloud-image",
     ))
     snapshots = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
         region="ARC-IS-HAF-1",
         type="snapshot",
     ))
     preconfigured_images = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
         type="preconfigured",
@@ -116,16 +116,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_genesiscloud as genesiscloud
 
-    base_os_images = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
-        type="base-os",
+    cloud_images = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
+        type="cloud-image",
     ))
     snapshots = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
         region="ARC-IS-HAF-1",
         type="snapshot",
     ))
     preconfigured_images = genesiscloud.images(filter=genesiscloud.ImagesFilterArgs(
         type="preconfigured",
```

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/instance.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 
 @pulumi.input_type
 class InstanceArgs:
     def __init__(__self__, *,
                  image: pulumi.Input[str],
                  region: pulumi.Input[str],
                  type: pulumi.Input[str],
+                 disk_size: Optional[pulumi.Input[int]] = None,
                  floating_ip_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input['InstanceMetadataArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  placement_option: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  timeouts: Optional[pulumi.Input['InstanceTimeoutsArgs']] = None,
                  volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Instance resource.
-        :param pulumi.Input[str] image: The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        :param pulumi.Input[str] image: The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+               image slug in this format `<image-slug>:<version>`. Learn more about images
+               [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
                recreate the resource.
         :param pulumi.Input[str] region: The region identifier. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The
                value must be one of: ["ARC-IS-HAF-1" "EUC-DE-MUC-1" "NORD-NO-KRS-1"].
         :param pulumi.Input[str] type: The instance type identifier. Learn more about instance types
                [here](https://developers.genesiscloud.com/instances#instance-types). - If the value of this attribute changes,
                Terraform will destroy and recreate the resource.
+        :param pulumi.Input[int] disk_size: The disk size of the instance in GB.
         :param pulumi.Input[str] floating_ip_id: The floating IP attached to the instance.
         :param pulumi.Input[str] hostname: The hostname of your instance. If not provided will be initially set to the `name` attribute. - If the value of this
                attribute is configured and changes, Terraform will destroy and recreate the resource.
         :param pulumi.Input['InstanceMetadataArgs'] metadata: Option to provide metadata. Currently supported is `startup_script`.
         :param pulumi.Input[str] name: The human-readable name for the instance.
         :param pulumi.Input[str] password: The password to access the instance. Your password must have upper and lower chars, digits and length between 8-72.
                **Please Note**: Only one of `ssh_keys` or `password` can be provided. Password is less secure - we recommend you use an
@@ -53,14 +57,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_key_ids: The ssh keys of the instance. - If the value of this attribute changes, Terraform will destroy and recreate the
                resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] volume_ids: The volumes of the instance.
         """
         pulumi.set(__self__, "image", image)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "type", type)
+        if disk_size is not None:
+            pulumi.set(__self__, "disk_size", disk_size)
         if floating_ip_id is not None:
             pulumi.set(__self__, "floating_ip_id", floating_ip_id)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if name is not None:
@@ -78,15 +84,17 @@
         if volume_ids is not None:
             pulumi.set(__self__, "volume_ids", volume_ids)
 
     @property
     @pulumi.getter
     def image(self) -> pulumi.Input[str]:
         """
-        The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+        image slug in this format `<image-slug>:<version>`. Learn more about images
+        [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
         recreate the resource.
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: pulumi.Input[str]):
         pulumi.set(self, "image", value)
@@ -115,14 +123,26 @@
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
+    @pulumi.getter(name="diskSize")
+    def disk_size(self) -> Optional[pulumi.Input[int]]:
+        """
+        The disk size of the instance in GB.
+        """
+        return pulumi.get(self, "disk_size")
+
+    @disk_size.setter
+    def disk_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "disk_size", value)
+
+    @property
     @pulumi.getter(name="floatingIpId")
     def floating_ip_id(self) -> Optional[pulumi.Input[str]]:
         """
         The floating IP attached to the instance.
         """
         return pulumi.get(self, "floating_ip_id")
 
@@ -242,14 +262,15 @@
         pulumi.set(self, "volume_ids", value)
 
 
 @pulumi.input_type
 class _InstanceState:
     def __init__(__self__, *,
                  created_at: Optional[pulumi.Input[str]] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
                  floating_ip_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  image_id: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input['InstanceMetadataArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
@@ -263,18 +284,21 @@
                  timeouts: Optional[pulumi.Input['InstanceTimeoutsArgs']] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
                  volume_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Instance resources.
         :param pulumi.Input[str] created_at: The timestamp when this image was created in RFC 3339.
+        :param pulumi.Input[int] disk_size: The disk size of the instance in GB.
         :param pulumi.Input[str] floating_ip_id: The floating IP attached to the instance.
         :param pulumi.Input[str] hostname: The hostname of your instance. If not provided will be initially set to the `name` attribute. - If the value of this
                attribute is configured and changes, Terraform will destroy and recreate the resource.
-        :param pulumi.Input[str] image: The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        :param pulumi.Input[str] image: The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+               image slug in this format `<image-slug>:<version>`. Learn more about images
+               [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
                recreate the resource.
         :param pulumi.Input[str] image_id: The resulting image ID of the instance.
         :param pulumi.Input['InstanceMetadataArgs'] metadata: Option to provide metadata. Currently supported is `startup_script`.
         :param pulumi.Input[str] name: The human-readable name for the instance.
         :param pulumi.Input[str] password: The password to access the instance. Your password must have upper and lower chars, digits and length between 8-72.
                **Please Note**: Only one of `ssh_keys` or `password` can be provided. Password is less secure - we recommend you use an
                SSH key-pair. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The string
@@ -293,14 +317,16 @@
                [here](https://developers.genesiscloud.com/instances#instance-types). - If the value of this attribute changes,
                Terraform will destroy and recreate the resource.
         :param pulumi.Input[str] updated_at: The timestamp when this image was last updated in RFC 3339.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] volume_ids: The volumes of the instance.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
+        if disk_size is not None:
+            pulumi.set(__self__, "disk_size", disk_size)
         if floating_ip_id is not None:
             pulumi.set(__self__, "floating_ip_id", floating_ip_id)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
         if image is not None:
             pulumi.set(__self__, "image", image)
         if image_id is not None:
@@ -343,14 +369,26 @@
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
+    @pulumi.getter(name="diskSize")
+    def disk_size(self) -> Optional[pulumi.Input[int]]:
+        """
+        The disk size of the instance in GB.
+        """
+        return pulumi.get(self, "disk_size")
+
+    @disk_size.setter
+    def disk_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "disk_size", value)
+
+    @property
     @pulumi.getter(name="floatingIpId")
     def floating_ip_id(self) -> Optional[pulumi.Input[str]]:
         """
         The floating IP attached to the instance.
         """
         return pulumi.get(self, "floating_ip_id")
 
@@ -371,15 +409,17 @@
     def hostname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hostname", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+        image slug in this format `<image-slug>:<version>`. Learn more about images
+        [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
         recreate the resource.
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
@@ -571,14 +611,15 @@
 
 
 class Instance(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
                  floating_ip_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[pulumi.InputType['InstanceMetadataArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  placement_option: Optional[pulumi.Input[str]] = None,
@@ -609,18 +650,21 @@
 
         ```sh
          $ pulumi import genesiscloud:index/instance:Instance example 18efeec8-94f0-4776-8ff2-5e9b49c74608
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[int] disk_size: The disk size of the instance in GB.
         :param pulumi.Input[str] floating_ip_id: The floating IP attached to the instance.
         :param pulumi.Input[str] hostname: The hostname of your instance. If not provided will be initially set to the `name` attribute. - If the value of this
                attribute is configured and changes, Terraform will destroy and recreate the resource.
-        :param pulumi.Input[str] image: The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        :param pulumi.Input[str] image: The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+               image slug in this format `<image-slug>:<version>`. Learn more about images
+               [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
                recreate the resource.
         :param pulumi.Input[pulumi.InputType['InstanceMetadataArgs']] metadata: Option to provide metadata. Currently supported is `startup_script`.
         :param pulumi.Input[str] name: The human-readable name for the instance.
         :param pulumi.Input[str] password: The password to access the instance. Your password must have upper and lower chars, digits and length between 8-72.
                **Please Note**: Only one of `ssh_keys` or `password` can be provided. Password is less secure - we recommend you use an
                SSH key-pair. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The string
                length must be at least 16.
@@ -675,14 +719,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 disk_size: Optional[pulumi.Input[int]] = None,
                  floating_ip_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  metadata: Optional[pulumi.Input[pulumi.InputType['InstanceMetadataArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  placement_option: Optional[pulumi.Input[str]] = None,
@@ -697,14 +742,15 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstanceArgs.__new__(InstanceArgs)
 
+            __props__.__dict__["disk_size"] = disk_size
             __props__.__dict__["floating_ip_id"] = floating_ip_id
             __props__.__dict__["hostname"] = hostname
             if image is None and not opts.urn:
                 raise TypeError("Missing required property 'image'")
             __props__.__dict__["image"] = image
             __props__.__dict__["metadata"] = metadata
             __props__.__dict__["name"] = name
@@ -735,14 +781,15 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             created_at: Optional[pulumi.Input[str]] = None,
+            disk_size: Optional[pulumi.Input[int]] = None,
             floating_ip_id: Optional[pulumi.Input[str]] = None,
             hostname: Optional[pulumi.Input[str]] = None,
             image: Optional[pulumi.Input[str]] = None,
             image_id: Optional[pulumi.Input[str]] = None,
             metadata: Optional[pulumi.Input[pulumi.InputType['InstanceMetadataArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             password: Optional[pulumi.Input[str]] = None,
@@ -761,18 +808,21 @@
         Get an existing Instance resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The timestamp when this image was created in RFC 3339.
+        :param pulumi.Input[int] disk_size: The disk size of the instance in GB.
         :param pulumi.Input[str] floating_ip_id: The floating IP attached to the instance.
         :param pulumi.Input[str] hostname: The hostname of your instance. If not provided will be initially set to the `name` attribute. - If the value of this
                attribute is configured and changes, Terraform will destroy and recreate the resource.
-        :param pulumi.Input[str] image: The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        :param pulumi.Input[str] image: The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+               image slug in this format `<image-slug>:<version>`. Learn more about images
+               [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
                recreate the resource.
         :param pulumi.Input[str] image_id: The resulting image ID of the instance.
         :param pulumi.Input[pulumi.InputType['InstanceMetadataArgs']] metadata: Option to provide metadata. Currently supported is `startup_script`.
         :param pulumi.Input[str] name: The human-readable name for the instance.
         :param pulumi.Input[str] password: The password to access the instance. Your password must have upper and lower chars, digits and length between 8-72.
                **Please Note**: Only one of `ssh_keys` or `password` can be provided. Password is less secure - we recommend you use an
                SSH key-pair. - If the value of this attribute changes, Terraform will destroy and recreate the resource. - The string
@@ -794,14 +844,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] volume_ids: The volumes of the instance.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstanceState.__new__(_InstanceState)
 
         __props__.__dict__["created_at"] = created_at
+        __props__.__dict__["disk_size"] = disk_size
         __props__.__dict__["floating_ip_id"] = floating_ip_id
         __props__.__dict__["hostname"] = hostname
         __props__.__dict__["image"] = image
         __props__.__dict__["image_id"] = image_id
         __props__.__dict__["metadata"] = metadata
         __props__.__dict__["name"] = name
         __props__.__dict__["password"] = password
@@ -823,14 +874,22 @@
     def created_at(self) -> pulumi.Output[str]:
         """
         The timestamp when this image was created in RFC 3339.
         """
         return pulumi.get(self, "created_at")
 
     @property
+    @pulumi.getter(name="diskSize")
+    def disk_size(self) -> pulumi.Output[int]:
+        """
+        The disk size of the instance in GB.
+        """
+        return pulumi.get(self, "disk_size")
+
+    @property
     @pulumi.getter(name="floatingIpId")
     def floating_ip_id(self) -> pulumi.Output[Optional[str]]:
         """
         The floating IP attached to the instance.
         """
         return pulumi.get(self, "floating_ip_id")
 
@@ -843,15 +902,17 @@
         """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def image(self) -> pulumi.Output[str]:
         """
-        The source image or snapshot of the instance. - If the value of this attribute changes, Terraform will destroy and
+        The source image id, image slug or snapshot id of the instance. The image version can also specified together with the
+        image slug in this format `<image-slug>:<version>`. Learn more about images
+        [here](https://developers.genesiscloud.com/images). - If the value of this attribute changes, Terraform will destroy and
         recreate the resource.
         """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="imageId")
     def image_id(self) -> pulumi.Output[str]:
```

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/outputs.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/provider.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/security_group.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/snapshot.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/ssh_key.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud/volume.py` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/PKG-INFO` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-genesiscloud
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing genesiscloud cloud resources.
 Home-page: https://www.pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/genesiscloud/pulumi-genesiscloud
 Keywords: pulumi genesiscloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_genesiscloud-0.0.8/pulumi_genesiscloud.egg-info/SOURCES.txt` & `pulumi_genesiscloud-0.0.9/pulumi_genesiscloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_genesiscloud-0.0.8/setup.py` & `pulumi_genesiscloud-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "genesiscloud Pulumi Package - Development Version"
```

