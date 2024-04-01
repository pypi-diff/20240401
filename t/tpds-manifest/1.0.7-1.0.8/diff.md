# Comparing `tmp/tpds_manifest-1.0.7-py3-none-any.whl.zip` & `tmp/tpds_manifest-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4508 bytes, number of entries: 8
--rw-r--r--  2.0 unx       65 b- defN 24-Mar-09 17:22 tpds/__init__.py
--rw-r--r--  2.0 unx      145 b- defN 24-Mar-09 17:22 tpds/packages/__init__.py
--rw-r--r--  2.0 unx     4158 b- defN 24-Mar-09 17:22 tpds/packages/packages.yaml
--rw-r--r--  2.0 unx     1322 b- defN 24-Mar-09 17:23 tpds_manifest-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2428 b- defN 24-Mar-09 17:23 tpds_manifest-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-09 17:23 tpds_manifest-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-09 17:23 tpds_manifest-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 24-Mar-09 17:23 tpds_manifest-1.0.7.dist-info/RECORD
-8 files, 8866 bytes uncompressed, 3364 bytes compressed:  62.1%
+Zip file size: 4531 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-01 16:17 tpds/__init__.py
+-rw-r--r--  2.0 unx      145 b- defN 24-Apr-01 16:17 tpds/packages/__init__.py
+-rw-r--r--  2.0 unx     4339 b- defN 24-Apr-01 16:17 tpds/packages/packages.yaml
+-rw-r--r--  2.0 unx     1322 b- defN 24-Apr-01 16:17 tpds_manifest-1.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2428 b- defN 24-Apr-01 16:17 tpds_manifest-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 16:17 tpds_manifest-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-01 16:17 tpds_manifest-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 24-Apr-01 16:17 tpds_manifest-1.0.8.dist-info/RECORD
+8 files, 9047 bytes uncompressed, 3387 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: tpds/packages/__init__.py
 Comment: 
 
 Filename: tpds/packages/packages.yaml
 Comment: 
 
-Filename: tpds_manifest-1.0.7.dist-info/LICENSE
+Filename: tpds_manifest-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: tpds_manifest-1.0.7.dist-info/METADATA
+Filename: tpds_manifest-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: tpds_manifest-1.0.7.dist-info/WHEEL
+Filename: tpds_manifest-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: tpds_manifest-1.0.7.dist-info/top_level.txt
+Filename: tpds_manifest-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: tpds_manifest-1.0.7.dist-info/RECORD
+Filename: tpds_manifest-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpds/packages/packages.yaml

```diff
@@ -147,7 +147,13 @@
         - tpds-extension-aes-message-encryption
 
   tpds-extension-dspic33-support:
     description: "Microchip(SPG) Trust Platform - dsPIC33 extension"
     source:
       pypi:
         - tpds-extension-dspic33-support
+
+  tpds-extension-keystream-connect:
+    description: "Microchip(SPG) Trust Platform - Keystream connect Usecase"
+    source:
+      pypi:
+        - tpds-extension-keystream-connect
```

## Comparing `tpds_manifest-1.0.7.dist-info/LICENSE` & `tpds_manifest-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tpds_manifest-1.0.7.dist-info/METADATA` & `tpds_manifest-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpds-manifest
-Version: 1.0.7
+Version: 1.0.8
 Summary: Microchip(SPG) Trust Platform Approved Package List
 Maintainer-email: Microchip Technology <SPG.Tools@microchip.com>
 License: (c) 2015-2023 Microchip Technology Inc. and its subsidiaries.
         
         Subject to your compliance with these terms, you may use the Microchip Software
         and any derivatives exclusively with Microchip products. It is your
         responsibility to comply with third party license terms applicable to your
```

