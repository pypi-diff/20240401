# Comparing `tmp/composabl_dev-0.8.0.dev1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/composabl_dev-0.8.0.dev6-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 106028 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 21:39 composabl_dev-0.8.0.dev1.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 21:39 composabl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 21:39 composabl_dev.libs/
--rw-rw-r--  2.0 unx      772 b- defN 24-Mar-27 21:39 composabl_dev-0.8.0.dev1.dist-info/RECORD
--rw-r--r--  2.0 unx       56 b- defN 24-Mar-27 21:39 composabl_dev-0.8.0.dev1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1825 b- defN 24-Mar-27 21:39 composabl_dev-0.8.0.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx      225 b- defN 24-Mar-27 21:39 composabl_dev-0.8.0.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-27 21:39 composabl_dev-0.8.0.dev1.dist-info/top_level.txt
--rwxr-xr-x  2.0 unx    93456 b- defN 24-Mar-27 21:39 composabl/ray.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    93456 b- defN 24-Mar-27 21:39 composabl/core.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    94456 b- defN 24-Mar-27 21:39 composabl/__init__.cpython-311-x86_64-linux-gnu.so
-11 files, 284256 bytes uncompressed, 104314 bytes compressed:  63.3%
+Zip file size: 25196 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      742 b- defN 24-Apr-01 17:28 composabl_dev-0.8.0.dev6.dist-info/RECORD
+-rw-r--r--  2.0 unx      111 b- defN 24-Apr-01 17:28 composabl_dev-0.8.0.dev6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-01 17:28 composabl_dev-0.8.0.dev6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-01 17:28 composabl_dev-0.8.0.dev6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1825 b- defN 24-Apr-01 17:28 composabl_dev-0.8.0.dev6.dist-info/METADATA
+-rwxr-xr-x  2.0 unx    39912 b- defN 24-Apr-01 17:28 composabl/__init__.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    39648 b- defN 24-Apr-01 17:28 composabl/ray.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    39656 b- defN 24-Apr-01 17:28 composabl/core.cpython-310-darwin.so
+8 files, 121960 bytes uncompressed, 23898 bytes compressed:  80.4%
```

## zipnote {}

```diff
@@ -1,34 +1,25 @@
-Filename: composabl_dev-0.8.0.dev1.dist-info/
+Filename: composabl_dev-0.8.0.dev6.dist-info/RECORD
 Comment: 
 
-Filename: composabl/
+Filename: composabl_dev-0.8.0.dev6.dist-info/WHEEL
 Comment: 
 
-Filename: composabl_dev.libs/
+Filename: composabl_dev-0.8.0.dev6.dist-info/entry_points.txt
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev1.dist-info/RECORD
+Filename: composabl_dev-0.8.0.dev6.dist-info/top_level.txt
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev1.dist-info/entry_points.txt
+Filename: composabl_dev-0.8.0.dev6.dist-info/METADATA
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev1.dist-info/METADATA
+Filename: composabl/__init__.cpython-310-darwin.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev1.dist-info/WHEEL
+Filename: composabl/ray.cpython-310-darwin.so
 Comment: 
 
-Filename: composabl_dev-0.8.0.dev1.dist-info/top_level.txt
-Comment: 
-
-Filename: composabl/ray.cpython-311-x86_64-linux-gnu.so
-Comment: 
-
-Filename: composabl/core.cpython-311-x86_64-linux-gnu.so
-Comment: 
-
-Filename: composabl/__init__.cpython-311-x86_64-linux-gnu.so
+Filename: composabl/core.cpython-310-darwin.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `composabl_dev-0.8.0.dev1.dist-info/RECORD` & `composabl_dev-0.8.0.dev6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-composabl_dev-0.8.0.dev1.dist-info/RECORD,,
-composabl_dev-0.8.0.dev1.dist-info/entry_points.txt,sha256=WrLVbw0dPbDvkgFcNa275XoyuBvDoP-453FEPMn_cG8,56
-composabl_dev-0.8.0.dev1.dist-info/METADATA,sha256=9GjyGIhob4WeKxTiTkvd2bnyR3xnLMdd6eU1apKYitw,1825
-composabl_dev-0.8.0.dev1.dist-info/WHEEL,sha256=xKUA0gyukCdKmxzOYBswqPPCMi4WQuuKA4Va6I5EzV0,225
-composabl_dev-0.8.0.dev1.dist-info/top_level.txt,sha256=u1D_14CTd3ryfSJBYuAR0PfjwHJ5_4NGQts7rZy2xks,10
-composabl/ray.cpython-311-x86_64-linux-gnu.so,sha256=lqwclMP1rCdO1e-VDr8fE5PCnTUIHurPchEutuWswNs,93456
-composabl/core.cpython-311-x86_64-linux-gnu.so,sha256=N8ljnym6tvGS2lrJRrbhaqsk6CILhgy1JKf5TKzyNh8,93456
-composabl/__init__.cpython-311-x86_64-linux-gnu.so,sha256=K046OMhSeiaYRy5CiObRgwon3uoW_O5GYFNu8CQUi7Q,94456
+composabl_dev-0.8.0.dev6.dist-info/RECORD,,
+composabl_dev-0.8.0.dev6.dist-info/WHEEL,sha256=5gVbVe_w8vFuKIeI1RffqCqgT_cNTJucal8EyR-41SQ,111
+composabl_dev-0.8.0.dev6.dist-info/entry_points.txt,sha256=WrLVbw0dPbDvkgFcNa275XoyuBvDoP-453FEPMn_cG8,56
+composabl_dev-0.8.0.dev6.dist-info/top_level.txt,sha256=u1D_14CTd3ryfSJBYuAR0PfjwHJ5_4NGQts7rZy2xks,10
+composabl_dev-0.8.0.dev6.dist-info/METADATA,sha256=e-jHkjXKCSS_Lja9Tpx2syFO5dHVYk9SNugEcQ8aCN0,1825
+composabl/__init__.cpython-310-darwin.so,sha256=CpRt_OBj-v9Epctz8zQ-rdVIcHfoRZ-IH49-fgEKKxw,39912
+composabl/ray.cpython-310-darwin.so,sha256=LHRDSdu8YbtW3WHw6CS6R3-16fHjwRcEFk_8AczeBP0,39648
+composabl/core.cpython-310-darwin.so,sha256=c87s48UvRIcDiRymfpoT0S1tuR71CVeo77nBlfShC6s,39656
```

## Comparing `composabl_dev-0.8.0.dev1.dist-info/METADATA` & `composabl_dev-0.8.0.dev6.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: composabl-dev
-Version: 0.8.0.dev1
+Version: 0.8.0.dev6
 Summary: a distributed runtime to be able to train agents across a cluster of machines
 Author-email: Xavier Geerinck <xavier@composabl.io>, Hunter Park <hunter@composabl.io>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: composabl-core-dev >=0.8.0.dev1
-Requires-Dist: composabl-train-dev >=0.8.0.dev1
-Requires-Dist: composabl-cli-dev >=0.8.0.dev1
+Requires-Dist: composabl-core-dev >=0.8.0.dev6
+Requires-Dist: composabl-train-dev >=0.8.0.dev6
+Requires-Dist: composabl-cli-dev >=0.8.0.dev6
 
 # Composabl
 
 Composabl helps you build Autonomous Agents! Through an easy SDK you get access to outscaled simulator training tools.
 
 ## Licenses / Seats
```

