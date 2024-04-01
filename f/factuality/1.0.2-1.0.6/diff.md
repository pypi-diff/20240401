# Comparing `tmp/factuality-1.0.2.tar.gz` & `tmp/factuality-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factuality-1.0.2.tar", max compression
+gzip compressed data, was "factuality-1.0.6.tar", max compression
```

## Comparing `factuality-1.0.2.tar` & `factuality-1.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1075 2024-03-29 09:58:59.579427 factuality-1.0.2/LICENSE
--rw-r--r--   0        0        0    12474 2024-03-31 10:21:17.722778 factuality-1.0.2/README.md
--rw-r--r--   0        0        0      485 2024-03-31 16:16:01.492226 factuality-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2411 2024-03-31 15:37:57.041979 factuality-1.0.2/src/factuality.py
--rw-r--r--   0        0        0    13158 1970-01-01 00:00:00.000000 factuality-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-31 16:43:03.077513 factuality-1.0.6/LICENSE
+-rw-r--r--   0        0        0    12474 2024-03-31 16:43:03.077513 factuality-1.0.6/README.md
+-rw-r--r--   0        0        0      485 2024-03-31 16:43:03.085513 factuality-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2411 2024-03-31 16:43:03.085513 factuality-1.0.6/src/factuality.py
+-rw-r--r--   0        0        0    13158 1970-01-01 00:00:00.000000 factuality-1.0.6/PKG-INFO
```

### Comparing `factuality-1.0.2/LICENSE` & `factuality-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `factuality-1.0.2/README.md` & `factuality-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `factuality-1.0.2/src/factuality.py` & `factuality-1.0.6/src/factuality.py`

 * *Files identical despite different names*

### Comparing `factuality-1.0.2/PKG-INFO` & `factuality-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factuality
-Version: 1.0.2
+Version: 1.0.6
 Summary: 
 License: MIT
 Author: Felix Mönckemeyer
 Author-email: felix.moenckemeyer@rwth-aachen.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

