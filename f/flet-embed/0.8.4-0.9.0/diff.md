# Comparing `tmp/flet_embed-0.8.4.tar.gz` & `tmp/flet_embed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_embed-0.8.4.tar", max compression
+gzip compressed data, was "flet_embed-0.9.0.tar", max compression
```

## Comparing `flet_embed-0.8.4.tar` & `flet_embed-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2023-07-25 02:24:11.320507 flet_embed-0.8.4/README.md
--rw-r--r--   0        0        0      742 2023-07-25 02:24:41.883711 flet_embed-0.8.4/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/__init__.py
--rw-r--r--   0        0        0       32 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/auth/__init__.py
--rw-r--r--   0        0        0       42 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/auth/providers/__init__.py
--rw-r--r--   0        0        0       31 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0       55 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/plotly_chart.py
--rw-r--r--   0        0        0       44 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/utils/__init__.py
--rw-r--r--   0        0        0      103 2023-07-25 02:24:11.320507 flet_embed-0.8.4/src/flet/version.py
--rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 flet_embed-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-08-04 19:28:31.527733 flet_embed-0.9.0/README.md
+-rw-r--r--   0        0        0      742 2023-08-04 19:29:04.812736 flet_embed-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/__init__.py
+-rw-r--r--   0        0        0       32 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/auth/__init__.py
+-rw-r--r--   0        0        0       42 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/auth/providers/__init__.py
+-rw-r--r--   0        0        0       31 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0       55 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0       44 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/utils/__init__.py
+-rw-r--r--   0        0        0      103 2023-08-04 19:28:31.527733 flet_embed-0.9.0/src/flet/version.py
+-rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 flet_embed-0.9.0/PKG-INFO
```

### Comparing `flet_embed-0.8.4/pyproject.toml` & `flet_embed-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-embed"
-version = "0.8.4"
+version = "0.9.0"
 description = "Flet Embed - embed Python into Flutter apps"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-runtime = "0.8.4"
+flet-runtime = "0.9.0"
 python = "^3.7"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.6"
 pytest = "^7.2.0"
```

### Comparing `flet_embed-0.8.4/PKG-INFO` & `flet_embed-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-embed
-Version: 0.8.4
+Version: 0.9.0
 Summary: Flet Embed - embed Python into Flutter apps
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-runtime (==0.8.4)
+Requires-Dist: flet-runtime (==0.9.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet embedded library
```

