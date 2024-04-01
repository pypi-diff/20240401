# Comparing `tmp/biomedicus_client-3.4.1.tar.gz` & `tmp/biomedicus_client-3.4.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedicus_client-3.4.1.tar", last modified: Wed Mar 20 19:33:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

