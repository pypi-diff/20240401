# Comparing `tmp/djsm-0.1.5.tar.gz` & `tmp/djsm-0.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsm-0.1.5.tar", last modified: Mon Jan 29 20:04:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

