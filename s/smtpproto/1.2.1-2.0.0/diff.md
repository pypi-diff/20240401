# Comparing `tmp/smtpproto-1.2.1.tar.gz` & `tmp/smtpproto-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smtpproto-1.2.1.tar", last modified: Tue Sep 19 08:32:49 2023, max compression
+gzip compressed data, was "smtpproto-2.0.0.tar", last modified: Mon Apr  1 13:08:06 2024, max compression
```

## Comparing `smtpproto-1.2.1.tar` & `smtpproto-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.025310 smtpproto-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.017310 smtpproto-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.017310 smtpproto-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-09-19 08:32:35.000000 smtpproto-1.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-09-19 08:32:35.000000 smtpproto-1.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-09-19 08:32:35.000000 smtpproto-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-09-19 08:32:35.000000 smtpproto-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-09-19 08:32:35.000000 smtpproto-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-19 08:32:35.000000 smtpproto-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2023-09-19 08:32:49.025310 smtpproto-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-09-19 08:32:35.000000 smtpproto-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.021310 smtpproto-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-09-19 08:32:35.000000 smtpproto-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-09-19 08:32:35.000000 smtpproto-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-09-19 08:32:35.000000 smtpproto-1.2.1/docs/devguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-09-19 08:32:35.000000 smtpproto-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2023-09-19 08:32:35.000000 smtpproto-1.2.1/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-09-19 08:32:35.000000 smtpproto-1.2.1/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-09-19 08:32:35.000000 smtpproto-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 08:32:49.025310 smtpproto-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.017310 smtpproto-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.021310 smtpproto-1.2.1/src/smtpproto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:35.000000 smtpproto-1.2.1/src/smtpproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2023-09-19 08:32:35.000000 smtpproto-1.2.1/src/smtpproto/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2023-09-19 08:32:35.000000 smtpproto-1.2.1/src/smtpproto/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2023-09-19 08:32:35.000000 smtpproto-1.2.1/src/smtpproto/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:35.000000 smtpproto-1.2.1/src/smtpproto/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.021310 smtpproto-1.2.1/src/smtpproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2023-09-19 08:32:48.000000 smtpproto-1.2.1/src/smtpproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-09-19 08:32:49.000000 smtpproto-1.2.1/src/smtpproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 08:32:48.000000 smtpproto-1.2.1/src/smtpproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-09-19 08:32:48.000000 smtpproto-1.2.1/src/smtpproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-19 08:32:48.000000 smtpproto-1.2.1/src/smtpproto.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 08:32:49.021310 smtpproto-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-09-19 08:32:35.000000 smtpproto-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2023-09-19 08:32:35.000000 smtpproto-1.2.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16890 2023-09-19 08:32:35.000000 smtpproto-1.2.1/tests/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.141371 smtpproto-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.133371 smtpproto-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.133371 smtpproto-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-01 13:07:59.000000 smtpproto-2.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-01 13:07:59.000000 smtpproto-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-01 13:07:59.000000 smtpproto-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 13:07:59.000000 smtpproto-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 13:07:59.000000 smtpproto-2.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 13:07:59.000000 smtpproto-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-01 13:08:06.141371 smtpproto-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-01 13:07:59.000000 smtpproto-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.137371 smtpproto-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 13:07:59.000000 smtpproto-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-01 13:07:59.000000 smtpproto-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-01 13:07:59.000000 smtpproto-2.0.0/docs/devguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 13:07:59.000000 smtpproto-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-01 13:07:59.000000 smtpproto-2.0.0/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-01 13:07:59.000000 smtpproto-2.0.0/docs/versionhistory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.137371 smtpproto-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-01 13:07:59.000000 smtpproto-2.0.0/examples/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 13:07:59.000000 smtpproto-2.0.0/examples/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-01 13:07:59.000000 smtpproto-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:08:06.141371 smtpproto-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.133371 smtpproto-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.137371 smtpproto-2.0.0/src/smtpproto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:07:59.000000 smtpproto-2.0.0/src/smtpproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-01 13:07:59.000000 smtpproto-2.0.0/src/smtpproto/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-01 13:07:59.000000 smtpproto-2.0.0/src/smtpproto/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-01 13:07:59.000000 smtpproto-2.0.0/src/smtpproto/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-04-01 13:07:59.000000 smtpproto-2.0.0/src/smtpproto/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:07:59.000000 smtpproto-2.0.0/src/smtpproto/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.137371 smtpproto-2.0.0/src/smtpproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-01 13:08:06.000000 smtpproto-2.0.0/src/smtpproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-01 13:08:06.000000 smtpproto-2.0.0/src/smtpproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:08:06.000000 smtpproto-2.0.0/src/smtpproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 13:08:06.000000 smtpproto-2.0.0/src/smtpproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 13:08:06.000000 smtpproto-2.0.0/src/smtpproto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:08:06.137371 smtpproto-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-01 13:07:59.000000 smtpproto-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-01 13:07:59.000000 smtpproto-2.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18171 2024-04-01 13:07:59.000000 smtpproto-2.0.0/tests/test_protocol.py
```

### Comparing `smtpproto-1.2.1/.github/workflows/publish.yml` & `smtpproto-2.0.0/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     environment: release
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
       run: python -m build
     - name: Archive packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: dist
         path: dist
 
   publish:
     needs: build
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
     steps:
     - name: Retrieve packages
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
     - name: Upload packages
       uses: pypa/gh-action-pypi-publish@release/v1
 
   release:
     name: Create a GitHub release
     needs: build
     runs-on: ubuntu-latest
```

### Comparing `smtpproto-1.2.1/.github/workflows/test.yml` & `smtpproto-2.0.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 
 jobs:
   pyright:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.x
-    - uses: actions/cache@v3
+    - uses: actions/cache@v4
       with:
         path: ~/.cache/pip
         key: pip-pyright
     - name: Install dependencies
       run: pip install -e . pyright pytest
     - name: Run pyright
       run: pyright --verifytypes smtpproto
 
   test:
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
         cache: pip
         cache-dependency-path: pyproject.toml
     - name: Install dependencies
       run: pip install .[test]
```

### Comparing `smtpproto-1.2.1/.pre-commit-config.yaml` & `smtpproto-2.0.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # This is the configuration file for pre-commit (https://pre-commit.com/).
 # To use:
 # * Install pre-commit (https://pre-commit.com/#installation)
 # * Copy this file as ".pre-commit-config.yaml"
 # * Run "pre-commit install".
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
-  - repo: https://github.com/psf/black
-    rev: 23.9.1
-    hooks:
-      - id: black
-
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.290
+    rev: v0.3.4
     hooks:
       - id: ruff
-        args:
-          - --fix
+        args: [--fix, --show-fixes]
+      - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.1
+    rev: v1.9.0
     hooks:
       - id: mypy
-        additional_dependencies: [ "pytest", "packaging" ]
+        additional_dependencies:
+          - aiosmtpd
+          - anyio
+          - pytest
+          - trustme
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-eval
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
+
+ci:
+  autoupdate_schedule: quarterly
```

### Comparing `smtpproto-1.2.1/LICENSE` & `smtpproto-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smtpproto-1.2.1/PKG-INFO` & `smtpproto-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: smtpproto
-Version: 1.2.1
+Version: 2.0.0
 Summary: Sans-io SMTP client with an AnyIO based async I/O implementation
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://smtpproto.readthedocs.io/en/latest/
 Project-URL: Source code, https://github.com/agronholm/smtpproto
 Project-URL: Issue tracker, https://github.com/agronholm/smtpproto/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Classifier: Framework :: AnyIO
+Classifier: Topic :: Communications :: Email
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: anyio>=3.0
+Requires-Dist: anyio~=4.2
 Provides-Extra: test
 Requires-Dist: anyio[trio]>=3.0; extra == "test"
 Requires-Dist: aiosmtpd>=1.4.4; extra == "test"
 Requires-Dist: coverage>=7; extra == "test"
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: trustme; extra == "test"
 Provides-Extra: doc
```

### Comparing `smtpproto-1.2.1/README.rst` & `smtpproto-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `smtpproto-1.2.1/docs/conf.py` & `smtpproto-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smtpproto-1.2.1/docs/devguide.rst` & `smtpproto-2.0.0/docs/devguide.rst`

 * *Files identical despite different names*

### Comparing `smtpproto-1.2.1/pyproject.toml` & `smtpproto-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 readme = "README.rst"
 authors = [{name = "Alex Grönholm", email = "alex.gronholm@nextday.fi"}]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
+    "Typing :: Typed",
     "Framework :: AnyIO",
+    "Topic :: Communications :: Email",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-requires-python = ">= 3.7"
-dependencies = [ "anyio >= 3.0" ]
+requires-python = ">= 3.8"
+dependencies = [ "anyio ~= 4.2" ]
 dynamic = [ "version" ]
 
 [project.urls]
 Documentation = "https://smtpproto.readthedocs.io/en/latest/"
 "Source code" = "https://github.com/agronholm/smtpproto"
 "Issue tracker" = "https://github.com/agronholm/smtpproto/issues"
 
@@ -48,49 +49,61 @@
     "sphinx-autodoc-typehints >= 1.2.0",
 ]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
-[tool.ruff]
-select = [
-    "E", "F", "W",  # default flake-8
+[tool.ruff.lint]
+extend-select = [
+    "B0",           # flake8-bugbear
+    "G",            # flake8-logging-format
     "I",            # isort
+    "ISC",          # flake8-implicit-str-concat
     "PGH",          # pygrep-hooks
+    "RUF100",       # unused noqa (yesqa)
     "UP",           # pyupgrade
-    "B0",           # flake8-bugbear
+    "W",            # pycodestyle warnings
 ]
 
+[tool.mypy]
+python_version = "3.8"
+strict = true
+
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short"
 testpaths = "tests"
 filterwarnings = "always"
 
 [tool.coverage.run]
 source = ["smtpproto"]
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = lint, py37, py38, py39, py310, py311, py312, pypy3
+envlist = lint, py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = true
 minversion = 4.0
 
 [testenv]
 depends = lint
+package = editable
 commands = pytest {posargs}
 extras = test
 
-[testenv:lint]
+[testenv:pre-commit]
 depends =
+package = skip
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
-skip_install = true
+
+[testenv:pyright]
+deps = pyright
+commands = pyright --verifytypes smtpproto
 
 [testenv:docs]
 extras = doc
 commands = sphinx-build -W -n docs build/sphinx
 """
```

### Comparing `smtpproto-1.2.1/src/smtpproto/client.py` & `smtpproto-2.0.0/tests/test_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,311 +1,323 @@
 from __future__ import annotations
 
-import logging
-import socket
-import sys
-from collections.abc import Callable, Iterable
-from dataclasses import dataclass, field
+import ssl
+from collections import defaultdict
+from collections.abc import Callable, Generator
+from concurrent.futures import ThreadPoolExecutor
+from contextlib import ExitStack, closing, contextmanager
 from email.headerregistry import Address
 from email.message import EmailMessage
-from email.utils import getaddresses, parseaddr
-from functools import partial
-from ssl import SSLContext
-from types import TracebackType
-from typing import Any, ContextManager, TypeVar
-from warnings import warn
-
-from anyio import (
-    BrokenResourceError,
-    aclose_forcefully,
-    connect_tcp,
-    fail_after,
-)
-from anyio.abc import AsyncResource, BlockingPortal, SocketStream
-from anyio.from_thread import start_blocking_portal
-from anyio.streams.tls import TLSStream
-
-from .auth import SMTPAuthenticator
-from .protocol import ClientState, SMTPClientProtocol, SMTPException, SMTPResponse
-
-logger: logging.Logger = logging.getLogger(__name__)
-TAsync = TypeVar("TAsync", bound="AsyncSMTPClient")
-TSync = TypeVar("TSync", bound="SyncSMTPClient")
-
-
-@dataclass
-class AsyncSMTPClient(AsyncResource):
-    """
-    An asynchronous SMTP client.
-
-    This runs on asyncio or any other backend supported by AnyIO.
-
-    It is recommended that this client is used as an async context manager instead of
-    manually calling :meth:`~connect` and :meth:`aclose`, if possible.
-
-    :param host: host name or IP address of the SMTP server
-    :param port: port on the SMTP server to connect to
-    :param connect_timeout: connection timeout (in seconds)
-    :param timeout: timeout for sending requests and reading responses (in seconds)
-    :param domain: domain name to send to the server as part of the greeting message
-    :param ssl_context: SSL context to use for establishing TLS encrypted sessions
-    :param authenticator: authenticator to use for authenticating with the SMTP server
-    """
-
-    host: str
-    port: int = 587
-    connect_timeout: float = 30
-    timeout: float = 60
-    domain: str = field(default_factory=socket.gethostname)
-    ssl_context: SSLContext | None = None
-    authenticator: SMTPAuthenticator | None = None
-    _protocol: SMTPClientProtocol = field(
-        init=False, default_factory=SMTPClientProtocol
-    )
-    _stream: TLSStream | SocketStream | None = field(init=False, default=None)
+from socket import socket
+from typing import Any
 
-    async def __aenter__(self: TAsync) -> TAsync:
-        await self.connect()
-        return self
+import pytest
+from aiosmtpd.controller import Controller
+from aiosmtpd.handlers import Sink
+from aiosmtpd.smtp import SMTP, AuthResult, Envelope, Session
+from anyio import create_task_group
+from smtpproto.auth import PlainAuthenticator
+from smtpproto.client import AsyncSMTPClient, SyncSMTPClient
+from smtpproto.protocol import SMTPException
 
-    async def __aexit__(
-        self,
-        exc_type: type[BaseException] | None,
-        exc_val: BaseException | None,
-        exc_tb: TracebackType | None,
-    ) -> None:
-        await self.aclose()
+pytestmark = pytest.mark.anyio
 
-    def __del__(self) -> None:
-        if self._stream:
-            warn(
-                f"unclosed {self.__class__.__name__}",
-                ResourceWarning,
-                stacklevel=1,
-                source=self._stream,
-            )
 
-    async def connect(self) -> None:
-        """Connect to the SMTP server."""
-        if not self._stream:
-            with fail_after(self.connect_timeout):
-                self._stream = await connect_tcp(self.host, self.port)
-
-            try:
-                await self._wait_response()
-                await self._send_command(self._protocol.send_greeting, self.domain)
-
-                # Do the TLS handshake if supported by the server
-                if "STARTTLS" in self._protocol.extensions:
-                    await self._send_command(self._protocol.start_tls)
-                    self._stream = await TLSStream.wrap(
-                        self._stream,
-                        hostname=self.host,
-                        ssl_context=self.ssl_context,
-                        standard_compatible=False,
-                    )
-
-                    # Send a new EHLO command to determine new capabilities
-                    await self._send_command(self._protocol.send_greeting, self.domain)
-
-                # Use the authenticator if one was provided
-                if self.authenticator:
-                    auth_gen = self.authenticator.authenticate()
-                    try:
-                        auth_data = await auth_gen.__anext__()
-                        response = await self._send_command(
-                            self._protocol.authenticate,
-                            self.authenticator.mechanism,
-                            auth_data,
-                        )
-                        while self._protocol.state is ClientState.authenticating:
-                            auth_data = await auth_gen.asend(response.message)
-                            self._protocol.send_authentication_data(auth_data)
-                            await self._flush_output()
-                    except StopAsyncIteration:
-                        pass
-                    finally:
-                        await auth_gen.aclose()
-            except BaseException:
-                await aclose_forcefully(self)
-                self._stream = None
-                raise
-
-    async def aclose(self) -> None:
-        """Close the connection, if connected."""
-        if self._stream:
-            try:
-                if self._protocol.state is not ClientState.finished:
-                    await self._send_command(self._protocol.quit)
-            finally:
-                await self._stream.aclose()
-                self._stream = None
-
-    async def _wait_response(self) -> SMTPResponse:
-        while True:
-            if not self._stream:
-                raise SMTPException("Not connected")
-
-            if self._protocol.needs_incoming_data:
-                try:
-                    with fail_after(self.timeout):
-                        data = await self._stream.receive()
-                except (BrokenResourceError, TimeoutError):
-                    await aclose_forcefully(self._stream)
-                    self._stream = None
-                    raise
-
-                logger.debug("Received: %s", data)
-                response = self._protocol.feed_bytes(data)
-                if response:
-                    if response.is_error():
-                        response.raise_as_exception()
-                    else:
-                        return response
-
-                await self._flush_output()
-
-    async def _flush_output(self) -> None:
-        if not self._stream:
-            raise SMTPException("Not connected")
-
-        data = self._protocol.get_outgoing_data()
-        if data:
-            logger.debug("Sent: %s", data)
-            try:
-                with fail_after(self.timeout):
-                    await self._stream.send(data)
-            except (BrokenResourceError, TimeoutError):
-                await aclose_forcefully(self._stream)
-                self._stream = None
-                raise
-
-    async def _send_command(self, command: Callable, *args) -> SMTPResponse:
-        if not self._stream:
-            raise SMTPException("Not connected")
-
-        command(*args)
-        await self._flush_output()
-        return await self._wait_response()
-
-    async def send_message(
+class DummyController(Controller):
+    def __init__(
         self,
-        message: EmailMessage,
+        handler: Any,
+        factory: Callable[..., SMTP] = SMTP,
+        hostname: str | None = None,
+        port: int = 0,
         *,
-        sender: str | Address | None = None,
-        recipients: Iterable[str] | None = None,
-    ) -> SMTPResponse:
-        sender = sender or parseaddr(message.get("From"))[1]
-        await self._send_command(self._protocol.mail, sender)
-
-        if not recipients:
-            tos: list[str] = message.get_all("to", [])
-            ccs: list[str] = message.get_all("cc", [])
-            resent_tos: list[str] = message.get_all("resent-to", [])
-            resent_ccs: list[str] = message.get_all("resent-cc", [])
-            recipients = [
-                email
-                for name, email in getaddresses(tos + ccs + resent_tos + resent_ccs)
-            ]
-
-        for recipient in recipients:
-            await self._send_command(self._protocol.recipient, recipient)
-
-        await self._send_command(self._protocol.start_data)
-        return await self._send_command(self._protocol.data, message)
-
-
-class SyncSMTPClient:
-    """
-    A synchronous (blocking) SMTP client.
-
-    It is recommended that this client is used as a context manager instead of manually
-    calling :meth:`~connect` and :meth:`close`, if possible.
-
-    :param host: host name or IP address of the SMTP server
-    :param port: port on the SMTP server to connect to
-    :param connect_timeout: connection timeout (in seconds)
-    :param timeout: timeout for sending requests and reading responses (in seconds)
-    :param domain: domain name to send to the server as part of the greeting message
-    :param ssl_context: SSL context to use for establishing TLS encrypted sessions
-    :param authenticator: authenticator to use for authenticating with the SMTP server
-    :param async_backend: name of the AnyIO-supported asynchronous backend
-    :param async_backend_options: dictionary of keyword arguments passed to
-        :func:`anyio.from_thread.start_blocking_portal`
-    """
+        ready_timeout: float = 1.0,
+        ssl_context: ssl.SSLContext | None = None,
+    ):
+        super().__init__(
+            handler,
+            hostname=hostname,
+            port=port,
+            ready_timeout=ready_timeout,
+            ssl_context=None,
+        )
+        self.__factory = factory
+        self.__ssl_context = ssl_context
 
-    _portal_cm: ContextManager[BlockingPortal] | None = None
-    _portal: BlockingPortal | None = None
+    def factory(self) -> SMTP:
+        return self.__factory(
+            self.handler, hostname=self.hostname, tls_context=self.__ssl_context
+        )
 
-    def __init__(
+
+@contextmanager
+def start_server(
+    *,
+    ssl_context: ssl.SSLContext | None = None,
+    factory: Callable[..., SMTP] = SMTP,
+    handler: Any = Sink,
+) -> Generator[tuple[str, int], Any, None]:
+    with closing(socket()) as sock:
+        sock.bind(("localhost", 0))
+        port = sock.getsockname()[1]
+
+    controller = DummyController(
+        handler,
+        factory=factory,
+        hostname="localhost",
+        port=port,
+        ssl_context=ssl_context,
+    )
+    controller.start()  # type: ignore[no-untyped-call]
+    yield controller.hostname, port
+    controller.stop()
+
+
+@pytest.fixture
+def message() -> EmailMessage:
+    message = EmailMessage()
+    message["From"] = Address("Foo Bar", "foo.bar", "baz.com")  # type: ignore[assignment]
+    message["To"] = ["test1@example.org"]  # type: ignore[assignment]
+    message["Cc"] = ["test2@example.org"]  # type: ignore[assignment]
+    message["Bcc"] = ["test3@example.org"]  # type: ignore[assignment]
+    message["Resent-To"] = ["test4@example.org"]  # type: ignore[assignment]
+    message["Resent-Cc"] = ["test5@example.org"]  # type: ignore[assignment]
+    message["Resent-Bcc"] = ["test6@example.org"]  # type: ignore[assignment]
+    message["Subject"] = "Unicöde string"
+    return message
+
+
+class TestAsyncClient:
+    @pytest.mark.parametrize("use_tls", [False, True], ids=["notls", "tls"])
+    async def test_send_mail(
         self,
-        *args: Any,
-        async_backend: str = "asyncio",
-        async_backend_options: dict[str, Any] | None = None,
-        **kwargs: Any,
-    ):
-        self._async_backend = async_backend
-        self._async_backend_options = async_backend_options
-        self._async_client = AsyncSMTPClient(*args, **kwargs)
-
-    def __enter__(self: TSync) -> TSync:
-        self.connect()
-        return self
+        client_context: ssl.SSLContext,
+        server_context: ssl.SSLContext,
+        use_tls: bool,
+        message: EmailMessage,
+    ) -> None:
+        received_recipients = []
+        received_content = b""
 
-    def __exit__(
+        class Handler:
+            async def handle_RCPT(
+                self,
+                server: SMTP,
+                session: Session,
+                envelope: Envelope,
+                address: str,
+                rcpt_options: list[str],
+            ) -> str:
+                received_recipients.append(address)
+                envelope.rcpt_tos.append(address)
+                envelope.rcpt_options.extend(rcpt_options)
+                return "250 OK"
+
+            async def handle_DATA(
+                self, server: SMTP, session: Session, envelope: Envelope
+            ) -> str:
+                nonlocal received_content
+                received_content = envelope.original_content or b""
+                return "250 OK"
+
+        with start_server(
+            ssl_context=server_context if use_tls else None, handler=Handler()
+        ) as (host, port):
+            client = AsyncSMTPClient(host=host, port=port, ssl_context=client_context)
+            await client.send_message(message)
+
+        assert received_recipients == [
+            f"test{index}@example.org" for index in range(1, 7)
+        ]
+        assert b"To: test1@example.org" in received_content
+        assert b"Cc: test2@example.org" in received_content
+        assert b"Resent-To: test4@example.org" in received_content
+        assert b"Resent-Cc: test5@example.org" in received_content
+        assert b"Bcc:" not in received_content
+        assert b"Resent-Bcc:" not in received_content
+
+    async def test_concurrency(self, message: EmailMessage) -> None:
+        received_recipients: dict[str, int] = defaultdict(lambda: 0)
+        received_contents: list[bytes] = []
+
+        class Handler:
+            async def handle_RCPT(
+                self,
+                server: SMTP,
+                session: Session,
+                envelope: Envelope,
+                address: str,
+                rcpt_options: list[str],
+            ) -> str:
+                received_recipients[address] += 1
+                envelope.rcpt_tos.append(address)
+                envelope.rcpt_options.extend(rcpt_options)
+                return "250 OK"
+
+            async def handle_DATA(
+                self, server: SMTP, session: Session, envelope: Envelope
+            ) -> str:
+                received_contents.append(envelope.original_content or b"")
+                return "250 OK"
+
+        with start_server(handler=Handler()) as (host, port):
+            client = AsyncSMTPClient(host=host, port=port)
+
+            async def send_multiple_messages(count: int) -> None:
+                async with client.connect() as session:
+                    for _ in range(count):
+                        await session.send_message(message)
+
+            async with create_task_group() as tg:
+                for _ in range(10):
+                    tg.start_soon(send_multiple_messages, 10)
+
+        for index in range(1, 7):
+            assert received_recipients[f"test{index}@example.org"] == 100
+
+        assert len(received_contents) == 100
+
+    async def test_no_esmtp_support(self) -> None:
+        class NoESMTP(SMTP):
+            async def smtp_EHLO(self, hostname: str) -> None:
+                await self.push("500 Unknown command")
+
+        with start_server(factory=NoESMTP) as (host, port):
+            client = AsyncSMTPClient(host=host, port=port)
+            async with client.connect():
+                pass
+
+    @pytest.mark.parametrize("success", [True, False], ids=["success", "failure"])
+    async def test_auth_plain(
         self,
-        exc_type: type[BaseException] | None,
-        exc_val: BaseException | None,
-        exc_tb: TracebackType | None,
+        client_context: ssl.SSLContext,
+        server_context: ssl.SSLContext,
+        success: bool,
     ) -> None:
-        self.close()
+        class AuthCapableSMTP(SMTP):
+            async def auth_PLAIN(self, _: Any, args: list[str]) -> AuthResult:
+                expected = "AHVzZXJuYW1lAHBhc3N3b3Jk"
+                if args[1] == expected and success:
+                    return AuthResult(success=True)
+                else:
+                    return AuthResult(success=False, handled=False)
+
+        with ExitStack() as stack:
+            host, port = stack.enter_context(
+                start_server(ssl_context=server_context, factory=AuthCapableSMTP)
+            )
+            if not success:
+                stack.enter_context(pytest.raises(SMTPException))
 
-    def __del__(self) -> None:
-        if self._portal:
-            warn(
-                f"unclosed {self.__class__.__name__}",
-                ResourceWarning,
-                stacklevel=1,
-                source=self._portal,
+            authenticator = PlainAuthenticator("username", "password")
+            client = AsyncSMTPClient(
+                host=host,
+                port=port,
+                ssl_context=client_context,
+                authenticator=authenticator,
             )
-            self.close()
+            async with client.connect():
+                pass
 
-    def connect(self) -> None:
-        """Connect to the SMTP server."""
-        portal_cm = start_blocking_portal(
-            self._async_backend, self._async_backend_options
-        )
-        portal = portal_cm.__enter__()
-        try:
-            portal.call(self._async_client.connect)
-        except BaseException:
-            portal_cm.__exit__(*sys.exc_info())
-            raise
-
-        self._portal_cm = portal_cm
-        self._portal = portal
-
-    def close(self) -> None:
-        """Close the connection, if connected."""
-        if self._portal:
-            try:
-                self._portal.call(self._async_client.aclose)
-            finally:
-                del self._portal
-                if self._portal_cm:
-                    self._portal_cm.__exit__(None, None, None)
-                    del self._portal_cm
 
-    def send_message(
+class TestSyncClient:
+    @pytest.mark.parametrize("use_tls", [False, True], ids=["notls", "tls"])
+    def test_send_mail(
         self,
-        message: EmailMessage,
-        *,
-        sender: str | Address | None = None,
-        recipients: Iterable[str] | None = None,
-    ) -> SMTPResponse:
-        if not self._portal:
-            raise SMTPException("Not connected")
+        client_context: ssl.SSLContext,
+        server_context: ssl.SSLContext,
+        use_tls: bool,
+    ) -> None:
+        message = EmailMessage()
+        message["From"] = Address("Foo Bar", "foo.bar", "baz.com")  # type: ignore[assignment]
+        message["To"] = ["test@example.org"]  # type: ignore[assignment]
+        message["Cc"] = ["test2@example.org"]  # type: ignore[assignment]
+        message["Subject"] = "Unicöde string"
+        with start_server(ssl_context=server_context if use_tls else None) as (
+            host,
+            port,
+        ):
+            client = SyncSMTPClient(host=host, port=port, ssl_context=client_context)
+            client.send_message(message)
+
+    def test_concurrency(self, message: EmailMessage) -> None:
+        received_recipients: dict[str, int] = defaultdict(lambda: 0)
+        received_contents: list[bytes] = []
+
+        class Handler:
+            async def handle_RCPT(
+                self,
+                server: SMTP,
+                session: Session,
+                envelope: Envelope,
+                address: str,
+                rcpt_options: list[str],
+            ) -> str:
+                received_recipients[address] += 1
+                envelope.rcpt_tos.append(address)
+                envelope.rcpt_options.extend(rcpt_options)
+                return "250 OK"
+
+            async def handle_DATA(
+                self, server: SMTP, session: Session, envelope: Envelope
+            ) -> str:
+                received_contents.append(envelope.original_content or b"")
+                return "250 OK"
+
+        with start_server(handler=Handler()) as (host, port):
+            client = SyncSMTPClient(host=host, port=port)
+
+            def send_multiple_messages(count: int) -> None:
+                with client.connect() as session:
+                    for _ in range(count):
+                        session.send_message(message)
+
+            with ThreadPoolExecutor() as executor:
+                for _ in range(10):
+                    executor.submit(send_multiple_messages, 10)
+
+        for index in range(1, 7):
+            assert received_recipients[f"test{index}@example.org"] == 100
+
+        assert len(received_contents) == 100
+
+    def test_no_esmtp_support(self) -> None:
+        class NoESMTP(SMTP):
+            async def smtp_EHLO(self, hostname: str) -> None:
+                await self.push("500 Unknown command")
+
+        with start_server(factory=NoESMTP) as (host, port):
+            client = SyncSMTPClient(host=host, port=port)
+            with client.connect():
+                pass
 
-        func = partial(
-            self._async_client.send_message, sender=sender, recipients=recipients
-        )
-        return self._portal.call(func, message)
+    @pytest.mark.parametrize("success", [True, False], ids=["success", "failure"])
+    def test_auth_plain(
+        self,
+        client_context: ssl.SSLContext,
+        server_context: ssl.SSLContext,
+        success: bool,
+    ) -> None:
+        class AuthCapableSMTP(SMTP):
+            async def auth_PLAIN(self, _: Any, args: list[str]) -> AuthResult:
+                expected = "AHVzZXJuYW1lAHBhc3N3b3Jk"
+                if args[1] == expected and success:
+                    return AuthResult(success=True)
+                else:
+                    return AuthResult(success=False, handled=False)
+
+        with ExitStack() as stack:
+            host, port = stack.enter_context(
+                start_server(ssl_context=server_context, factory=AuthCapableSMTP)
+            )
+            if not success:
+                stack.enter_context(pytest.raises(SMTPException))
+
+            authenticator = PlainAuthenticator("username", "password")
+            client = SyncSMTPClient(
+                host=host,
+                port=port,
+                ssl_context=client_context,
+                authenticator=authenticator,
+            )
+            with client.connect():
+                pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smtpproto-1.2.1/src/smtpproto/protocol.py` & `smtpproto-2.0.0/src/smtpproto/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import re
 from collections.abc import Iterable, Sequence
+from copy import copy
 from dataclasses import dataclass, field
 from email.headerregistry import Address
 from email.message import EmailMessage
 from email.policy import SMTP, SMTPUTF8, Policy
 from enum import Enum, auto
 from re import Pattern
 from typing import NoReturn
@@ -91,15 +92,15 @@
     def _require_extension(self, extension: str) -> None:
         if extension not in self._extensions:
             raise SMTPMissingExtension(
                 f"This operation requires the {extension} extension but "
                 f"the server does not support it"
             )
 
-    def _require_auth_mechanism(self, mechanism) -> None:
+    def _require_auth_mechanism(self, mechanism: str) -> None:
         if mechanism not in self._auth_mechanisms:
             raise SMTPUnsupportedAuthMechanism(
                 f"{mechanism} is not a supported authentication mechanism on this "
                 f"server"
             )
 
     def _encode_address(self, address: str | Address) -> bytes:
@@ -125,15 +126,15 @@
                     f"The address {address_str!r} requires UTF-8 encoding but the "
                     f"server does not support the SMTPUTF8 extension"
                 )
 
     def _send_command(self, command: str, *args: str | bytes) -> None:
         if self._command_sent is not None:
             raise SMTPProtocolViolation(
-                "Tried to send a command before the previous one received " "a response"
+                "Tried to send a command before the previous one received a response"
             )
 
         line = command.encode("ascii")
         args_encoded = tuple(
             arg.encode("ascii") if isinstance(arg, str) else arg for arg in args
         )
         if args_encoded:
@@ -386,14 +387,20 @@
         self._require_state(ClientState.send_data)
         policy: Policy = SMTPUTF8 if self._smtputf8_message else SMTP
         policy = (
             policy.clone(cte_type="7bit")
             if "8BITMIME" not in self._extensions
             else policy
         )
+
+        if "bcc" in message or "resent-bcc" in message:
+            message = copy(message)
+            del message["bcc"]
+            del message["resent-bcc"]
+
         self._out_buffer += message.as_bytes(policy=policy).replace(b"\r\n.", b"\r\n..")
         self._out_buffer += b".\r\n"
         self._state = ClientState.data_sent
 
     def reset(self) -> None:
         """Send the RSET command (cancel the active mail transaction)."""
         self._require_state(
```

### Comparing `smtpproto-1.2.1/src/smtpproto.egg-info/PKG-INFO` & `smtpproto-2.0.0/src/smtpproto.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: smtpproto
-Version: 1.2.1
+Version: 2.0.0
 Summary: Sans-io SMTP client with an AnyIO based async I/O implementation
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://smtpproto.readthedocs.io/en/latest/
 Project-URL: Source code, https://github.com/agronholm/smtpproto
 Project-URL: Issue tracker, https://github.com/agronholm/smtpproto/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Classifier: Framework :: AnyIO
+Classifier: Topic :: Communications :: Email
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: anyio>=3.0
+Requires-Dist: anyio~=4.2
 Provides-Extra: test
 Requires-Dist: anyio[trio]>=3.0; extra == "test"
 Requires-Dist: aiosmtpd>=1.4.4; extra == "test"
 Requires-Dist: coverage>=7; extra == "test"
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: trustme; extra == "test"
 Provides-Extra: doc
```

### Comparing `smtpproto-1.2.1/src/smtpproto.egg-info/SOURCES.txt` & `smtpproto-2.0.0/src/smtpproto.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 .github/workflows/test.yml
 docs/api.rst
 docs/conf.py
 docs/devguide.rst
 docs/index.rst
 docs/userguide.rst
 docs/versionhistory.rst
+examples/gmail.py
+examples/local.py
 src/smtpproto/__init__.py
+src/smtpproto/_utils.py
 src/smtpproto/auth.py
 src/smtpproto/client.py
 src/smtpproto/protocol.py
 src/smtpproto/py.typed
 src/smtpproto.egg-info/PKG-INFO
 src/smtpproto.egg-info/SOURCES.txt
 src/smtpproto.egg-info/dependency_links.txt
```

### Comparing `smtpproto-1.2.1/tests/conftest.py` & `smtpproto-2.0.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import ssl
 
 import pytest
 import trustme
 
 
 @pytest.fixture(scope="session")
-def ca():
+def ca() -> trustme.CA:
     return trustme.CA()
 
 
 @pytest.fixture(scope="session")
-def server_context(ca):
+def server_context(ca: trustme.CA) -> ssl.SSLContext:
     server_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
     ca.issue_cert("localhost").configure_cert(server_context)
     return server_context
 
 
 @pytest.fixture(scope="session")
-def client_context(ca):
+def client_context(ca: trustme.CA) -> ssl.SSLContext:
     client_context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
     ca.configure_trust(client_context)
     return client_context
```

### Comparing `smtpproto-1.2.1/tests/test_protocol.py` & `smtpproto-2.0.0/tests/test_protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from email.headerregistry import Address
 from email.message import EmailMessage
+from typing import Any, cast
 
 import pytest
+from _pytest.fixtures import SubRequest
 from smtpproto.protocol import (
     ClientState,
     SMTPClientProtocol,
     SMTPMissingExtension,
     SMTPProtocolViolation,
     SMTPUnsupportedAuthMechanism,
 )
 
 
 def call_protocol_method(
-    protocol: SMTPClientProtocol, func: Callable, expected_outgoing_data: bytes
-):
+    protocol: SMTPClientProtocol, func: Callable[[], Any], expected_outgoing_data: bytes
+) -> None:
     assert not protocol.needs_incoming_data
     func()
     assert protocol.get_outgoing_data() == expected_outgoing_data
 
 
 def feed_bytes(
     protocol: SMTPClientProtocol,
     data: bytes,
     expected_code: int | None = None,
     expected_message: str | None = None,
     expected_state: ClientState | None = None,
-):
+) -> None:
     assert protocol.needs_incoming_data
     response = protocol.feed_bytes(data)
     if expected_code:
         assert response
         assert response.code == expected_code
         assert not protocol.needs_incoming_data
     else:
@@ -42,15 +44,15 @@
     if expected_message:
         assert response
         assert response.message == expected_message
     if expected_state:
         assert protocol.state is expected_state
 
 
-def exchange_greetings(protocol, esmtp=True):
+def exchange_greetings(protocol: SMTPClientProtocol, esmtp: bool = True) -> None:
     # Server sends a greeting message
     feed_bytes(
         protocol,
         b"220 foo.bar SMTP service ready\r\n",
         220,
         "foo.bar SMTP service ready",
         ClientState.greeting_received,
@@ -91,15 +93,15 @@
             protocol, b"250 foo.bar ready\r\n", 250, "foo.bar ready", ClientState.ready
         )
         assert protocol.extensions == frozenset()
         assert protocol.auth_mechanisms == frozenset()
         assert protocol.max_message_size is None
 
 
-def start_mail_tx(protocol, smtputf8=True):
+def start_mail_tx(protocol: SMTPClientProtocol, smtputf8: bool = True) -> None:
     # Start a mail transaction
     extra_args = b""
     if "8BITMIME" in protocol.extensions:
         extra_args += b" BODY=8BITMIME"
     if smtputf8 and "SMTPUTF8" in protocol.extensions:
         extra_args += b" SMTPUTF8"
 
@@ -135,23 +137,25 @@
         354,
         "Start mail input; end with <CRLF>.<CRLF>",
         ClientState.send_data,
     )
 
 
 @pytest.fixture(
-    params=["héllö@example.org", Address("Héllö World", "héllö", "example.org")],
-    ids=["str", "object"],
+    params=[
+        pytest.param("héllö@example.org", id="str"),
+        pytest.param(Address("Héllö World", "héllö", "example.org"), id="object"),
+    ],
 )
-def unicode_address(request):
-    return request.param
+def unicode_address(request: SubRequest) -> str | Address:
+    return cast("str | Address", request.param)
 
 
 @pytest.fixture
-def protocol():
+def protocol() -> SMTPClientProtocol:
     proto = SMTPClientProtocol()
     assert proto.state is ClientState.greeting_expected
     assert proto.needs_incoming_data
     return proto
 
 
 @pytest.mark.parametrize(
@@ -180,16 +184,21 @@
             "This is a =?utf-8?q?subj=C3=ABct?=",
             "This is ä test message.",
             id="smtputf8_opt_out",
         ),
     ],
 )
 def test_send_mail_utf8_content(
-    protocol, esmtp, smtputf8, expected_cte, expected_subject, expected_body
-):
+    protocol: SMTPClientProtocol,
+    esmtp: bool,
+    smtputf8: bool,
+    expected_cte: str,
+    expected_subject: str,
+    expected_body: str,
+) -> None:
     exchange_greetings(protocol, esmtp=esmtp)
     start_mail_tx(protocol, smtputf8=smtputf8)
 
     message = EmailMessage()
     message["Subject"] = "This is a subjëct"
     message.set_content("This is ä test message.")
     call_protocol_method(
@@ -200,63 +209,71 @@
         f"Content-Transfer-Encoding: {expected_cte}\r\n"
         f"MIME-Version: 1.0\r\n\r\n"
         f"{expected_body}\r\n.\r\n".encode(),
     )
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.ready)
 
 
-def test_send_mail_utf8_addresses(protocol, unicode_address):
+def test_send_mail_utf8_addresses(
+    protocol: SMTPClientProtocol, unicode_address: str | Address
+) -> None:
     exchange_greetings(protocol)
     protocol.mail(unicode_address)
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.mailtx)
     protocol.recipient(unicode_address)
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.recipient_sent)
 
 
-def test_send_mail_unicode_sender_encoding_error(protocol, unicode_address):
+def test_send_mail_unicode_sender_encoding_error(
+    protocol: SMTPClientProtocol, unicode_address: str | Address
+) -> None:
     exchange_greetings(protocol, esmtp=False)
     exc = pytest.raises(SMTPProtocolViolation, protocol.mail, unicode_address)
     exc.match(
         "^The address 'héllö@example.org' requires UTF-8 encoding but the server does "
         "not support the SMTPUTF8 extension"
     )
 
 
-def test_send_mail_unicode_sender_no_smtputf8_encoding_error(protocol, unicode_address):
+def test_send_mail_unicode_sender_no_smtputf8_encoding_error(
+    protocol: SMTPClientProtocol, unicode_address: str | Address
+) -> None:
     exchange_greetings(protocol, esmtp=True)
     exc = pytest.raises(
         SMTPProtocolViolation, protocol.mail, unicode_address, smtputf8=False
     )
     exc.match(
         "^The address 'héllö@example.org' requires UTF-8 encoding but `smtputf8` was "
         "not specified"
     )
 
 
-def test_send_mail_unicode_recipient_encoding_error(protocol, unicode_address):
+def test_send_mail_unicode_recipient_encoding_error(
+    protocol: SMTPClientProtocol, unicode_address: str | Address
+) -> None:
     exchange_greetings(protocol, esmtp=False)
     protocol.mail("hello@example.org")
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.mailtx)
 
     exc = pytest.raises(SMTPProtocolViolation, protocol.recipient, unicode_address)
     exc.match("^The address 'héllö@example.org' requires UTF-8")
 
 
 def test_send_mail_unicode_recipient_no_smtputf8_encoding_error(
-    protocol, unicode_address
-):
+    protocol: SMTPClientProtocol, unicode_address: str | Address
+) -> None:
     exchange_greetings(protocol, esmtp=True)
     protocol.mail("hello@example.org", smtputf8=False)
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.mailtx)
 
     exc = pytest.raises(SMTPProtocolViolation, protocol.recipient, unicode_address)
     exc.match("^The address 'héllö@example.org' requires UTF-8")
 
 
-def test_send_mail_escape_dots(protocol):
+def test_send_mail_escape_dots(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     start_mail_tx(protocol)
 
     message = EmailMessage()
     message.set_content("The following lines might trip the protocol:\n.test\n.")
     call_protocol_method(
         protocol,
@@ -268,84 +285,84 @@
         b"..test\r\n"
         b"..\r\n"
         b".\r\n",
     )
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.ready)
 
 
-def test_reset_mail_tx(protocol):
+def test_reset_mail_tx(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     start_mail_tx(protocol)
     call_protocol_method(protocol, protocol.reset, b"RSET\r\n")
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.ready)
 
 
-def test_bad_greeting(protocol):
+def test_bad_greeting(protocol: SMTPClientProtocol) -> None:
     feed_bytes(protocol, b"554 Go away\r\n", 554, "Go away")
 
 
-def test_premature_greeting(protocol):
+def test_premature_greeting(protocol: SMTPClientProtocol) -> None:
     pytest.raises(SMTPProtocolViolation, protocol.send_greeting, "foo.bar").match(
         "Required state: one of: greeting_received; current state: greeting_expected"
     )
 
 
-def test_double_command(protocol):
+def test_double_command(protocol: SMTPClientProtocol) -> None:
     protocol.noop()
     pytest.raises(SMTPProtocolViolation, protocol.noop).match(
         "Tried to send a command before the previous one received a response"
     )
 
 
-def test_authentication_required(protocol):
+def test_authentication_required(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     call_protocol_method(
         protocol,
         lambda: protocol.mail("foo@bar.com"),
         b"MAIL FROM:<foo@bar.com> BODY=8BITMIME SMTPUTF8\r\n",
     )
     feed_bytes(
         protocol, b"530 Authentication required\r\n", 530, "Authentication required"
     )
 
 
-def test_noop(protocol):
+def test_noop(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     call_protocol_method(protocol, protocol.noop, b"NOOP\r\n")
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK", ClientState.ready)
 
 
-def test_start_tls(protocol):
+def test_start_tls(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     call_protocol_method(protocol, protocol.start_tls, b"STARTTLS\r\n")
     feed_bytes(protocol, b"220 OK\r\n", 220, "OK", ClientState.greeting_received)
 
 
-def test_start_tls_missing_extension(protocol):
+def test_start_tls_missing_extension(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol, esmtp=False)
     pytest.raises(SMTPMissingExtension, protocol.start_tls).match(
         "This operation requires the STARTTLS extension but the server does not "
         "support it"
     )
 
 
-def test_quit(protocol):
+def test_quit(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     call_protocol_method(protocol, protocol.quit, b"QUIT\r\n")
     feed_bytes(protocol, b"221 OK\r\n", 221, "OK", ClientState.finished)
 
 
-def test_auth_with_unsupported_mechanism(protocol):
+def test_auth_with_unsupported_mechanism(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
     pytest.raises(
         SMTPUnsupportedAuthMechanism, lambda: protocol.authenticate("XOAUTH2")
     ).match("XOAUTH2 is not a supported authentication mechanism on this server")
 
 
-def test_auth_plain(protocol):
+def test_auth_plain(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
 
     call_protocol_method(
         protocol,
         lambda: protocol.authenticate("PLAIN", "AHRlc3QAcGFzcw=="),
         b"AUTH PLAIN AHRlc3QAcGFzcw==\r\n",
     )
@@ -355,15 +372,15 @@
         235,
         "Authentication successful",
         ClientState.authenticated,
     )
 
 
 @pytest.mark.parametrize("error_code", [432, 454, 500, 534, 535, 538])
-def test_auth_plain_failure(protocol, error_code):
+def test_auth_plain_failure(protocol: SMTPClientProtocol, error_code: int) -> None:
     exchange_greetings(protocol)
     call_protocol_method(
         protocol,
         lambda: protocol.authenticate("PLAIN", "dummy"),
         b"AUTH PLAIN dummy\r\n",
     )
     feed_bytes(
@@ -371,15 +388,15 @@
         f"{error_code} Error\r\n".encode(),
         error_code,
         "Error",
         ClientState.ready,
     )
 
 
-def test_auth_login(protocol):
+def test_auth_login(protocol: SMTPClientProtocol) -> None:
     exchange_greetings(protocol)
 
     call_protocol_method(
         protocol, lambda: protocol.authenticate("LOGIN"), b"AUTH LOGIN\r\n"
     )
     feed_bytes(
         protocol,
@@ -407,15 +424,15 @@
         235,
         "Authentication successful",
         ClientState.authenticated,
     )
 
 
 @pytest.mark.parametrize("error_code", [432, 454, 500, 534, 535, 538])
-def test_auth_login_failure(protocol, error_code):
+def test_auth_login_failure(protocol: SMTPClientProtocol, error_code: int) -> None:
     exchange_greetings(protocol)
 
     call_protocol_method(
         protocol, lambda: protocol.authenticate("LOGIN"), b"AUTH LOGIN\r\n"
     )
     feed_bytes(
         protocol,
@@ -442,47 +459,47 @@
         f"{error_code} Error\r\n".encode(),
         error_code,
         "Error",
         ClientState.ready,
     )
 
 
-def test_server_invalid_input(protocol):
+def test_server_invalid_input(protocol: SMTPClientProtocol) -> None:
     exc = pytest.raises(SMTPProtocolViolation, feed_bytes, protocol, b"BLAH foobar\r\n")
     exc.match("Invalid input: BLAH foobar")
 
 
-def test_server_invalid_continuation(protocol):
+def test_server_invalid_continuation(protocol: SMTPClientProtocol) -> None:
     feed_bytes(protocol, b"220-hello\r\n")
     exc = pytest.raises(SMTPProtocolViolation, feed_bytes, protocol, b"230 hello\r\n")
     exc.match("Expected code 220, got 230 instead")
 
 
-def test_server_invalid_status_code(protocol):
+def test_server_invalid_status_code(protocol: SMTPClientProtocol) -> None:
     exc = pytest.raises(SMTPProtocolViolation, feed_bytes, protocol, b"600 hello\r\n")
     exc.match("Unexpected response: 600 hello")
 
 
 @pytest.mark.parametrize("error_code", [504, 550])
-def test_ehlo_error(protocol, error_code):
+def test_ehlo_error(protocol: SMTPClientProtocol, error_code: int) -> None:
     feed_bytes(
         protocol,
         b"220 foo.bar SMTP service ready\r\n",
         220,
         "foo.bar SMTP service ready",
         ClientState.greeting_received,
     )
     call_protocol_method(
         protocol, lambda: protocol.send_greeting("foo.bar"), b"EHLO foo.bar\r\n"
     )
     feed_bytes(protocol, f"{error_code} Error\r\n".encode(), error_code, "Error")
 
 
 @pytest.mark.parametrize("error_code", [502, 504, 550])
-def test_helo_error(protocol, error_code):
+def test_helo_error(protocol: SMTPClientProtocol, error_code: int) -> None:
     feed_bytes(
         protocol,
         b"220 foo.bar SMTP service ready\r\n",
         220,
         "foo.bar SMTP service ready",
         ClientState.greeting_received,
     )
@@ -491,43 +508,43 @@
     )
     feed_bytes(protocol, b"500 unrecognized command\r\n")
     assert protocol.get_outgoing_data() == b"HELO foo.bar\r\n"
     feed_bytes(protocol, f"{error_code} Error\r\n".encode(), error_code, "Error")
 
 
 @pytest.mark.parametrize("error_code", [451, 452, 455, 503, 550, 553, 552, 555])
-def test_mail_error(protocol, error_code):
+def test_mail_error(protocol: SMTPClientProtocol, error_code: int) -> None:
     exchange_greetings(protocol)
     call_protocol_method(
         protocol,
         lambda: protocol.mail("foo@bar"),
         b"MAIL FROM:<foo@bar> BODY=8BITMIME SMTPUTF8\r\n",
     )
     feed_bytes(protocol, f"{error_code} Error\r\n".encode(), error_code, "Error")
 
 
 @pytest.mark.parametrize(
     "error_code", [450, 451, 452, 455, 503, 550, 551, 552, 553, 555]
 )
-def test_rcpt_error(protocol, error_code):
+def test_rcpt_error(protocol: SMTPClientProtocol, error_code: int) -> None:
     exchange_greetings(protocol)
     call_protocol_method(
         protocol,
         lambda: protocol.mail("foo@bar"),
         b"MAIL FROM:<foo@bar> BODY=8BITMIME SMTPUTF8\r\n",
     )
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK")
     call_protocol_method(
         protocol, lambda: protocol.recipient("foo@bar"), b"RCPT TO:<foo@bar>\r\n"
     )
     feed_bytes(protocol, f"{error_code} Error\r\n".encode(), error_code, "Error")
 
 
 @pytest.mark.parametrize("error_code", [450, 451, 452, 503, 550, 552, 554])
-def test_start_data_error(protocol, error_code):
+def test_start_data_error(protocol: SMTPClientProtocol, error_code: int) -> None:
     exchange_greetings(protocol)
     call_protocol_method(
         protocol,
         lambda: protocol.mail("foo@bar"),
         b"MAIL FROM:<foo@bar> BODY=8BITMIME SMTPUTF8\r\n",
     )
     feed_bytes(protocol, b"250 OK\r\n", 250, "OK")
```

