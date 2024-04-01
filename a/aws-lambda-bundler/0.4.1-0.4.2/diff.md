# Comparing `tmp/aws_lambda_bundler-0.4.1.tar.gz` & `tmp/aws_lambda_bundler-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_bundler-0.4.1.tar", last modified: Fri Mar 29 22:37:39 2024, max compression
+gzip compressed data, was "aws_lambda_bundler-0.4.2.tar", last modified: Mon Apr  1 16:22:10 2024, max compression
```

## Comparing `aws_lambda_bundler-0.4.1.tar` & `aws_lambda_bundler-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:37:39.415381 aws_lambda_bundler-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-29 22:37:32.000000 aws_lambda_bundler-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-29 22:37:39.415381 aws_lambda_bundler-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 22:37:32.000000 aws_lambda_bundler-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:37:39.411381 aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-29 22:37:39.000000 aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-29 22:37:39.000000 aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:37:39.000000 aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-29 22:37:39.000000 aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 22:37:39.000000 aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-29 22:37:32.000000 aws_lambda_bundler-0.4.1/aws_lambda_bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-29 22:37:32.000000 aws_lambda_bundler-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 22:37:39.415381 aws_lambda_bundler-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:37:39.411381 aws_lambda_bundler-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-29 22:37:32.000000 aws_lambda_bundler-0.4.1/tests/test_aws_lambda_bundler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.799934 aws_lambda_bundler-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-01 16:22:10.000000 aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-01 16:22:10.000000 aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:22:10.000000 aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 16:22:10.000000 aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 16:22:10.000000 aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/aws_lambda_bundler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:10.803934 aws_lambda_bundler-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/tests/test_aws_lambda_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-01 16:22:01.000000 aws_lambda_bundler-0.4.2/tox.ini
```

### Comparing `aws_lambda_bundler-0.4.1/LICENSE.txt` & `aws_lambda_bundler-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_bundler-0.4.1/PKG-INFO` & `aws_lambda_bundler-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_bundler
-Version: 0.4.1
+Version: 0.4.2
 Summary: utility to build zip archives to run AWS Lambda functions
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 Project-URL: Documentation, https://github.com/unknown/aws-lambda-bundler#readme
 Project-URL: Issues, https://github.com/unknown/aws-lambda-bundler/issues
 Project-URL: Source, https://github.com/unknown/aws-lambda-bundler
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 # aws-lambda-bundler
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aws-lambda-bundler.svg)](https://pypi.org/project/aws-lambda-bundler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-lambda-bundler.svg)](https://pypi.org/project/aws-lambda-bundler)
 
 -----
 
-## What is it?
+## Rationale
 
 `aws-lambda-bundler` is a utility to build zip archives to run AWS Lambda functions from a list of dependencies.
 
 
 ## Installation
 
 ```console
```

### Comparing `aws_lambda_bundler-0.4.1/README.md` & `aws_lambda_bundler-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # aws-lambda-bundler
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aws-lambda-bundler.svg)](https://pypi.org/project/aws-lambda-bundler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-lambda-bundler.svg)](https://pypi.org/project/aws-lambda-bundler)
 
 -----
 
-## What is it?
+## Rationale
 
 `aws-lambda-bundler` is a utility to build zip archives to run AWS Lambda functions from a list of dependencies.
 
 
 ## Installation
 
 ```console
```

### Comparing `aws_lambda_bundler-0.4.1/aws_lambda_bundler.egg-info/PKG-INFO` & `aws_lambda_bundler-0.4.2/aws_lambda_bundler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_bundler
-Version: 0.4.1
+Version: 0.4.2
 Summary: utility to build zip archives to run AWS Lambda functions
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 Project-URL: Documentation, https://github.com/unknown/aws-lambda-bundler#readme
 Project-URL: Issues, https://github.com/unknown/aws-lambda-bundler/issues
 Project-URL: Source, https://github.com/unknown/aws-lambda-bundler
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 # aws-lambda-bundler
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aws-lambda-bundler.svg)](https://pypi.org/project/aws-lambda-bundler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aws-lambda-bundler.svg)](https://pypi.org/project/aws-lambda-bundler)
 
 -----
 
-## What is it?
+## Rationale
 
 `aws-lambda-bundler` is a utility to build zip archives to run AWS Lambda functions from a list of dependencies.
 
 
 ## Installation
 
 ```console
```

### Comparing `aws_lambda_bundler-0.4.1/aws_lambda_bundler.py` & `aws_lambda_bundler-0.4.2/aws_lambda_bundler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import subprocess
 import sys
 import hashlib
 from pathlib import Path
+from typing import Optional
 
 AWS_LAMBDA_BUNDLER_DEFAULT_APP = ".aws_lambda_bundler"
 
 
 def _install_to_dir(
     python: str, target_dir: Path, dependencies: list[str], index_url=None, platform=None, requirements=None
 ):
@@ -42,56 +43,60 @@
         f"zipping contents of {dir.absolute().as_posix()} to {output.absolute().as_posix()}",
         file=sys.stderr,
     )
     if not p.returncode == 0:
         print(p.stderr, file=sys.stderr)
         sys.exit(p.returncode)
 
+def _generate_dirname(app_dir: Path, dependencies: list[str], requirements: Optional[str] = None) -> Path:
+    key = hashlib.md5("".join(dependencies).encode())
+    if requirements:
+        with open(requirements,"rb") as handle:
+            key.update(handle.read())
+
+    return  app_dir / key.hexdigest()
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--app-dir", default=AWS_LAMBDA_BUNDLER_DEFAULT_APP)
     parser.add_argument("--output", required=True)
     parser.add_argument("--interpreter", required=False, default=sys.executable, help="path to the python interpreter")
     parser.add_argument("--index-url", required=False, help="index url to pass on to pip")
     parser.add_argument("--platform", required=False, help="install only wheel compatible with <platform>")
     parser.add_argument("--requirements", "-r", required=False, help="requirements file passed on to pip")
     parser.add_argument("dependencies", nargs="*")
     args = parser.parse_args()
 
-    python = args.interpreter
     app_dir = Path(args.app_dir)
     if not app_dir.is_dir():
         app_dir.mkdir(parents=True)
-    output: Path = Path(args.output)
-    if not output.is_absolute():
-        output = Path.cwd().joinpath(output)
+
+    python = args.interpreter
     dependencies: list[str] = args.dependencies
     platform = args.platform
     index_url = args.index_url
     requirements = args.requirements
 
     if not requirements and not dependencies:
         print("must at least specify one of --requirements or dependencies", file=sys.stderr)
 
-    key = hashlib.md5("".join(args.dependencies).encode())
-    if args.requirements:
-        with open(args.requirements,"rb") as handle:
-            key.update(handle.read())
+    target_dir = _generate_dirname(app_dir, dependencies, requirements)
 
-    target_dir = app_dir / key.hexdigest()
     if not target_dir.is_dir():
         _install_to_dir(
             python=python,
             target_dir=target_dir,
             dependencies=dependencies,
             index_url=index_url,
             platform=platform,
             requirements=requirements,
         )
+
+
+    output = Path(args.output)
     _zip_dir(output=output, dir=target_dir)
 
     sys.stdout.write(f"{output.absolute().as_posix()}\n")
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `aws_lambda_bundler-0.4.1/pyproject.toml` & `aws_lambda_bundler-0.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = [
+    "setuptools>=61.0",
+    "setuptools-scm>=8.0"
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_lambda_bundler"
-version = "0.4.1"
+dynamic = ["version"]
 description = 'utility to build zip archives to run AWS Lambda functions'
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "MIT"}
 keywords = []
 authors = [
   { name = "Felix Scherz", email = "felixwscherz@gmail.com" },
@@ -29,7 +32,15 @@
 [project.urls]
 Documentation = "https://github.com/unknown/aws-lambda-bundler#readme"
 Issues = "https://github.com/unknown/aws-lambda-bundler/issues"
 Source = "https://github.com/unknown/aws-lambda-bundler"
 
 [project.scripts]
 aws-lambda-bundler = "aws_lambda_bundler:main"
+
+[tool.towncrier]
+name = "aws-lambda-bundler"
+package = "aws_lambda_bundler"
+directory = "changes"
+filename = "CHANGELOG.md"
+
+[tool.setuptools_scm]
```

### Comparing `aws_lambda_bundler-0.4.1/tests/test_aws_lambda_bundler.py` & `aws_lambda_bundler-0.4.2/tests/test_aws_lambda_bundler.py`

 * *Files identical despite different names*

