# Comparing `tmp/givapi-0.1.2b0.tar.gz` & `tmp/givapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "givapi-0.1.2b0.tar", max compression
+gzip compressed data, was "givapi-0.2.0.tar", max compression
```

## Comparing `givapi-0.1.2b0.tar` & `givapi-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    35149 2024-03-31 08:35:27.610759 givapi-0.1.2b0/LICENSE
--rw-r--r--   0        0        0     2460 2024-03-31 08:35:27.610759 givapi-0.1.2b0/givapi.py
--rw-r--r--   0        0        0      397 2024-03-31 08:35:27.610759 givapi-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 givapi-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-01 16:32:19.487008 givapi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3515 2024-04-01 16:32:19.487008 givapi-0.2.0/givapi.py
+-rw-r--r--   0        0        0      396 2024-04-01 16:32:19.487008 givapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 givapi-0.2.0/PKG-INFO
```

### Comparing `givapi-0.1.2b0/LICENSE` & `givapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `givapi-0.1.2b0/PKG-INFO` & `givapi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GivAPI
-Version: 0.1.2b0
+Version: 0.2.0
 Summary: Pulls data from the GivEnergy API
 License: GPL-3.0
 Author: Wilbur Williams
 Author-email: contact@wilburwilliams.uk
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

