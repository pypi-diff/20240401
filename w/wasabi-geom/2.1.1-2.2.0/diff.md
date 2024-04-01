# Comparing `tmp/wasabi-geom-2.1.1.tar.gz` & `tmp/wasabi_geom-2.2.0-cp36-cp36m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasabi-geom-2.1.1.tar", last modified: Wed Apr 20 22:55:52 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

