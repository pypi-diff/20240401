# Comparing `tmp/databento_dbn-0.8.3-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.9.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 651837 bytes, number of entries: 8
--rw-r--r--  4.6 unx     3052 b- defN 23-Aug-15 20:24 databento_dbn-0.8.3.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Aug-15 20:24 databento_dbn-0.8.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     9868 b- defN 23-Aug-15 20:24 databento_dbn-0.8.3.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-Aug-15 20:24 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    50547 b- defN 23-Aug-15 20:24 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Aug-15 20:24 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1948672 b- defN 23-Aug-15 20:24 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      679 b- defN 23-Aug-15 20:24 databento_dbn-0.8.3.dist-info/RECORD
-8 files, 2013047 bytes uncompressed, 650649 bytes compressed:  67.7%
+Zip file size: 652921 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     3052 b- defN 23-Aug-24 20:36 databento_dbn-0.9.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Aug-24 20:36 databento_dbn-0.9.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-Aug-24 20:36 databento_dbn-0.9.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-Aug-24 20:36 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    50621 b- defN 23-Aug-24 20:36 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Aug-24 20:36 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1950720 b- defN 23-Aug-24 20:36 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-Aug-24 20:36 databento_dbn-0.9.0.dist-info/RECORD
+8 files, 2015169 bytes uncompressed, 651733 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: databento_dbn-0.8.3.dist-info/METADATA
+Filename: databento_dbn-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.8.3.dist-info/WHEEL
+Filename: databento_dbn-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: databento_dbn-0.8.3.dist-info/license_files/LICENSE
+Filename: databento_dbn-0.9.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.8.3.dist-info/RECORD
+Filename: databento_dbn-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databento_dbn/__init__.pyi

```diff
@@ -366,15 +366,15 @@
         -------
         int
 
         """
     @property
     def publisher_id(self) -> int:
         """
-        The publisher ID assigned by Databento.
+        The publisher ID assigned by Databento, which denotes the dataset and venue.
 
         Returns
         -------
         int
 
         """
     @property
@@ -447,15 +447,15 @@
         -------
         int
 
         """
     @property
     def publisher_id(self) -> int:
         """
-        The publisher ID assigned by Databento.
+        The publisher ID assigned by Databento, which denotes the dataset and venue.
 
         Returns
         -------
         int
 
         """
     @property
```

## Comparing `databento_dbn-0.8.3.dist-info/METADATA` & `databento_dbn-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.8.3
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for encoding and decoding Databento Binary Encoding (DBN)
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
```

## Comparing `databento_dbn-0.8.3.dist-info/license_files/LICENSE` & `databento_dbn-0.9.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

