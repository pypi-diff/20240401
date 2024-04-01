# Comparing `tmp/openbb_devtools-1.1.4.tar.gz` & `tmp/openbb_devtools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_devtools-1.1.4.tar", max compression
+gzip compressed data, was "openbb_devtools-1.1.5.tar", max compression
```

## Comparing `openbb_devtools-1.1.4.tar` & `openbb_devtools-1.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      604 2024-01-17 14:26:16.634331 openbb_devtools-1.1.4/README.md
--rw-r--r--   0        0        0       39 2024-01-17 14:26:16.634527 openbb_devtools-1.1.4/openbb_devtools/__init__.py
--rw-r--r--   0        0        0      711 2024-03-11 19:57:07.317142 openbb_devtools-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 openbb_devtools-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-29 11:03:36.732430 openbb_devtools-1.1.5/README.md
+-rw-r--r--   0        0        0       39 2024-02-29 11:03:36.732586 openbb_devtools-1.1.5/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-01 14:18:45.492574 openbb_devtools-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 openbb_devtools-1.1.5/PKG-INFO
```

### Comparing `openbb_devtools-1.1.4/README.md` & `openbb_devtools-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openbb_devtools-1.1.4/pyproject.toml` & `openbb_devtools-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-devtools"
-version = "1.1.4"
+version = "1.1.5"
 description = "Tools for OpenBB Platform Developers"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_devtools" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"               # scipy forces <4.0 explicitly
```

### Comparing `openbb_devtools-1.1.4/PKG-INFO` & `openbb_devtools-1.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-devtools
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tools for OpenBB Platform Developers
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

