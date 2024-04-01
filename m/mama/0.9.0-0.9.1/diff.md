# Comparing `tmp/mama-0.9.0.tar.gz` & `tmp/mama-0.9.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.9.0.tar", last modified: Tue Mar 26 13:18:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

