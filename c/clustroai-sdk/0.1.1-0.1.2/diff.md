# Comparing `tmp/clustroai_sdk-0.1.1-py3-none-any.whl.zip` & `tmp/clustroai_sdk-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5535 bytes, number of entries: 7
+Zip file size: 8424 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       34 b- defN 23-Nov-22 23:57 clustroai_sdk/__init__.py
--rw-r--r--  2.0 unx    12986 b- defN 24-Jan-16 14:24 clustroai_sdk/clustro_sdk.py
+-rw-r--r--  2.0 unx    13328 b- defN 24-Apr-01 13:57 clustroai_sdk/async_clustro_adk.py
+-rw-r--r--  2.0 unx    12986 b- defN 24-Feb-23 14:21 clustroai_sdk/clustro_sdk.py
 -rw-r--r--  2.0 unx      563 b- defN 23-Nov-22 23:57 clustroai_sdk/logger.py
--rw-r--r--  2.0 unx     2138 b- defN 24-Jan-16 14:26 clustroai_sdk-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-16 14:26 clustroai_sdk-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Jan-16 14:26 clustroai_sdk-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      567 b- defN 24-Jan-16 14:26 clustroai_sdk-0.1.1.dist-info/RECORD
-7 files, 16394 bytes uncompressed, 4525 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx     2159 b- defN 24-Apr-01 13:59 clustroai_sdk-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 13:59 clustroai_sdk-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-01 13:59 clustroai_sdk-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      659 b- defN 24-Apr-01 13:59 clustroai_sdk-0.1.2.dist-info/RECORD
+8 files, 29835 bytes uncompressed, 7270 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: clustroai_sdk/__init__.py
 Comment: 
 
+Filename: clustroai_sdk/async_clustro_adk.py
+Comment: 
+
 Filename: clustroai_sdk/clustro_sdk.py
 Comment: 
 
 Filename: clustroai_sdk/logger.py
 Comment: 
 
-Filename: clustroai_sdk-0.1.1.dist-info/METADATA
+Filename: clustroai_sdk-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: clustroai_sdk-0.1.1.dist-info/WHEEL
+Filename: clustroai_sdk-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: clustroai_sdk-0.1.1.dist-info/top_level.txt
+Filename: clustroai_sdk-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: clustroai_sdk-0.1.1.dist-info/RECORD
+Filename: clustroai_sdk-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `clustroai_sdk-0.1.1.dist-info/METADATA` & `clustroai_sdk-0.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: clustroai-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: clustroai-sdk
 Home-page: https://www.clustro.ai/
 Author: clustro ai
 Author-email: clustro@clustro.ai
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: httpx
 
 # ClustroAI SDK
 
 ClustroAI SDK is a powerful toolkit designed to harness idle computing resources for AI applications. It provides a comprehensive platform for AI enthusiasts and developers to utilize and monetize computing power efficiently.
 
 ## Key Features
 - **Resource Utilization**: ClustroAI SDK helps in tapping into underutilized computing resources, turning them into valuable assets for AI computation.
```

## Comparing `clustroai_sdk-0.1.1.dist-info/RECORD` & `clustroai_sdk-0.1.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 clustroai_sdk/__init__.py,sha256=qO_lUh2UumteabfhQZgpuVJ4j5CYCeAf5_NvkZ2JX8I,34
+clustroai_sdk/async_clustro_adk.py,sha256=jGaoEYb3DoyWddByIL_cNF6VB26rpVMwigJcvCVUUGo,13328
 clustroai_sdk/clustro_sdk.py,sha256=4VZsViXU3_2GapdM1jWJLihAlF-d5PAz3TambfVcaNY,12986
 clustroai_sdk/logger.py,sha256=F6GWo2s3SUnQVeTot6F92xXc5Vq_TZNH3dQaD2wAlfk,563
-clustroai_sdk-0.1.1.dist-info/METADATA,sha256=NI6M0YU1v1KT1VWMFJ9NT2e7-1TVeA7wmmuCRhTomNY,2138
-clustroai_sdk-0.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-clustroai_sdk-0.1.1.dist-info/top_level.txt,sha256=JYIbzOfN2Fnvio9raYcD7kOyKfLlteCHJHw2gDRfaiI,14
-clustroai_sdk-0.1.1.dist-info/RECORD,,
+clustroai_sdk-0.1.2.dist-info/METADATA,sha256=T_GmvFPA0hM2SVYkKrDgQYF_P8DOe1Xotxg_o04APOY,2159
+clustroai_sdk-0.1.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+clustroai_sdk-0.1.2.dist-info/top_level.txt,sha256=JYIbzOfN2Fnvio9raYcD7kOyKfLlteCHJHw2gDRfaiI,14
+clustroai_sdk-0.1.2.dist-info/RECORD,,
```

