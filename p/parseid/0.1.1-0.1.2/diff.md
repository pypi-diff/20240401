# Comparing `tmp/parseid-0.1.1.tar.gz` & `tmp/parseid-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parseid-0.1.1.tar", last modified: Tue Mar 26 15:02:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

