# Comparing `tmp/kcli-99.0.202404010855.tar.gz` & `tmp/kcli-99.0.202404011739-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcli-99.0.202404010855.tar", last modified: Mon Apr  1 08:55:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

