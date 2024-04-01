# Comparing `tmp/mkninja-0.2.0.tar.gz` & `tmp/mkninja-0.2.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkninja-0.2.0.tar", last modified: Sat Mar 30 13:13:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

