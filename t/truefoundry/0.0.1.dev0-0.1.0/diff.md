# Comparing `tmp/truefoundry-0.0.1.dev0.tar.gz` & `tmp/truefoundry-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.0.1.dev0.tar", max compression
+gzip compressed data, was "truefoundry-0.1.0.tar", max compression
```

## Comparing `truefoundry-0.0.1.dev0.tar` & `truefoundry-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       17 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/README.md
--rw-r--r--   0        0        0      550 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      679 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       24 2024-03-22 14:30:14.356834 truefoundry-0.0.1.dev0/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 truefoundry-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-01 16:24:45.975400 truefoundry-0.1.0/README.md
+-rw-r--r--   0        0        0      654 2024-04-01 16:24:57.175420 truefoundry-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      794 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 truefoundry-0.1.0/PKG-INFO
```

### Comparing `truefoundry-0.0.1.dev0/pyproject.toml` & `truefoundry-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.0.1.dev"
+version = "0.1.0"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.1"
 mlfoundry = { version = "0.10.7", optional = true }
 
-
 [tool.poetry.extras]
 ml = ["mlfoundry"]
 
+[tool.poetry-dynamic-versioning]
+enable = false
+
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.plugins."console_scripts"]
 tfy = "truefoundry.cli.__main__:main"
 truefoundry = "truefoundry.cli.__main__:main"
```

### Comparing `truefoundry-0.0.1.dev0/truefoundry/cli/__main__.py` & `truefoundry-0.1.0/truefoundry/cli/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-import os
 import sys
 
 import click
-from mlfoundry.cli.commands import download
 from servicefoundry.cli import create_servicefoundry_cli
 
+MLFOUNDRY_INSTALLED = True
+try:
+    from mlfoundry.cli.commands import download
+except ImportError:
+    MLFOUNDRY_INSTALLED = False
+
 
 @click.group()
 def ml():
     """MlFoundry CLI"""
 
 
 def main():
     # Exit the interpreter by raising SystemExit(status).
     # If the status is omitted or None, it defaults to zero (i.e., success).
     # If the status is an integer, it will be used as the system exit status.
     # If it is another kind of object, it will be printed and the system exit status will be one (i.e., failure).
-    ml.add_command(download)
     cli = create_servicefoundry_cli()
-    cli.add_command(ml)
+    if MLFOUNDRY_INSTALLED:
+        ml.add_command(download)
+        cli.add_command(ml)
     sys.exit(cli())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `truefoundry-0.0.1.dev0/PKG-INFO` & `truefoundry-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.0.1.dev0
+Version: 0.1.0
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

