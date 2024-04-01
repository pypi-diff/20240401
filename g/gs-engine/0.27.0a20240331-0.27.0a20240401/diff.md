# Comparing `tmp/gs_engine-0.27.0a20240331-py2.py3-none-macosx_12_0_x86_64.whl.zip` & `tmp/gs_engine-0.27.0a20240401-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,11 @@
-Zip file size: 13150 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 graphscope_runtime/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 gs_engine-0.27.0a20240331.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 graphscope.runtime/
--rw-r--r--  2.0 unx      694 b- defN 24-Mar-31 19:45 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      840 b- defN 24-Mar-31 20:57 gs_engine-0.27.0a20240331.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 24-Mar-31 20:50 gs_engine-0.27.0a20240331.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Mar-31 20:50 gs_engine-0.27.0a20240331.dist-info/top_level.txt
--rw-r--r--  2.0 unx    23179 b- defN 24-Mar-31 20:50 gs_engine-0.27.0a20240331.dist-info/METADATA
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-31 20:57 graphscope.runtime/conf/
--rw-r--r--  2.0 unx     1573 b- defN 24-Mar-31 19:45 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 24-Mar-31 19:45 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      593 b- defN 24-Mar-31 19:45 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 24-Mar-31 19:45 graphscope.runtime/conf/log4rs.yml
-13 files, 27640 bytes uncompressed, 11188 bytes compressed:  59.5%
+Zip file size: 12626 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 24-Apr-01 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      593 b- defN 24-Apr-01 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 24-Apr-01 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-01 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-01 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    23179 b- defN 24-Apr-01 20:00 gs_engine-0.27.0a20240401.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-01 20:00 gs_engine-0.27.0a20240401.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-01 20:00 gs_engine-0.27.0a20240401.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-Apr-01 20:00 gs_engine-0.27.0a20240401.dist-info/RECORD
+9 files, 27601 bytes uncompressed, 11164 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,40 +1,28 @@
-Filename: graphscope_runtime/
-Comment: 
-
-Filename: gs_engine-0.27.0a20240331.dist-info/
-Comment: 
-
-Filename: graphscope.runtime/
-Comment: 
-
-Filename: graphscope_runtime/__init__.py
-Comment: 
-
-Filename: gs_engine-0.27.0a20240331.dist-info/RECORD
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.27.0a20240331.dist-info/WHEEL
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.27.0a20240331.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.27.0a20240331.dist-info/METADATA
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
-Filename: graphscope.runtime/conf/
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.27.0a20240401.dist-info/METADATA
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: gs_engine-0.27.0a20240401.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.27.0a20240401.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.27.0a20240401.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `gs_engine-0.27.0a20240331.dist-info/METADATA` & `gs_engine-0.27.0a20240401.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.27.0a20240331
+Version: 0.27.0a20240401
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

