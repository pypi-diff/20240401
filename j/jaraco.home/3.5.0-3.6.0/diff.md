# Comparing `tmp/jaraco.home-3.5.0.tar.gz` & `tmp/jaraco.home-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.home-3.5.0.tar", last modified: Sun Jul 30 00:40:29 2023, max compression
+gzip compressed data, was "jaraco.home-3.6.0.tar", last modified: Mon Apr  1 16:18:02 2024, max compression
```

## Comparing `jaraco.home-3.5.0.tar` & `jaraco.home-3.6.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.778366 jaraco.home-3.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.778366 jaraco.home-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.782366 jaraco.home-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.774366 jaraco.home-3.5.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/jaraco/home/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/Gather HDHomeRun Stats.plist
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/mock hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/jaraco/home/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:40:29.782366 jaraco.home-3.5.0/jaraco.home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 00:40:29.000000 jaraco.home-3.5.0/jaraco.home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-30 00:40:29.786366 jaraco.home-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-30 00:40:01.000000 jaraco.home-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.123748 jaraco.home-3.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.123748 jaraco.home-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.123748 jaraco.home-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.119748 jaraco.home-3.6.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/jaraco/home/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/Gather HDHomeRun Stats.plist
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/mock hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/report-spam-call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/jaraco/home/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:18:02.127748 jaraco.home-3.6.0/jaraco.home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 16:18:02.000000 jaraco.home-3.6.0/jaraco.home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-01 16:18:02.131748 jaraco.home-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-01 16:17:43.000000 jaraco.home-3.6.0/tox.ini
```

### Comparing `jaraco.home-3.5.0/.github/workflows/main.yml` & `jaraco.home-3.6.0/.github/workflows/main.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,103 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient. For tox, it must be one of
-  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
-  # in common is "1".
+  # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
-  # MyPy's color enforcement (must be a non-zero number)
-  MYPY_FORCE_COLOR: -42
-  # Recognized by the `py` package, dependency of `pytest` (must be "1")
-  PY_COLORS: 1
-  # Make tox-wrapped tools see color requests
-  TOX_TESTENV_PASSENV: >-
-    FORCE_COLOR
-    MYPY_FORCE_COLOR
-    NO_COLOR
-    PY_COLORS
-    PYTEST_THEME
-    PYTEST_THEME_MODE
 
   # Suppress noisy pip warnings
   PIP_DISABLE_PIP_VERSION_CHECK: 'true'
   PIP_NO_PYTHON_VERSION_WARNING: 'true'
   PIP_NO_WARN_SCRIPT_LOCATION: 'true'
 
-  # Disable the spinner, noise in GHA; TODO(webknjaz): Fix this upstream
-  # Must be "1".
-  TOX_PARALLEL_NO_SPINNER: 1
+  # Ensure tests can sense settings about the environment
+  TOX_OVERRIDE: >-
+    testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
         - "3.9"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
         exclude:
         # lxml fails to build on Windows
         # https://bugs.launchpad.net/lxml/+bug/1977998
         - platform: windows-latest
           python: '3.11'
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox
 
-  docs:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
@@ -110,20 +108,19 @@
       contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.home-3.5.0/LICENSE` & `jaraco.home-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.5.0/NEWS.rst` & `jaraco.home-3.6.0/NEWS.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+v3.6.0
+======
+
+Features
+--------
+
+- Add routine to quickly report spam calls to FTC.
+
+
+v3.5.1
+======
+
+Bugfixes
+--------
+
+- Removed workaround in tests.
+
+
 v3.5.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `jaraco.home-3.5.0/README.rst` & `jaraco.home-3.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.home.svg
    :target: https://pypi.org/project/jaraco.home
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.home.svg
 
-.. image:: https://github.com/jaraco/jaraco.home/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.home/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.home/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.home-3.5.0/conftest.py` & `jaraco.home-3.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.5.0/docs/conf.py` & `jaraco.home-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.5.0/jaraco/home/Gather HDHomeRun Stats.plist` & `jaraco.home-3.6.0/jaraco/home/Gather HDHomeRun Stats.plist`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.5.0/jaraco/home/hdhomerun.py` & `jaraco.home-3.6.0/jaraco/home/hdhomerun.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,18 @@
 def shuffled(items):
     ordered = list(items)
     random.shuffle(ordered)
     return ordered
 
 
 def find_idle_tuner():
-    for id in shuffled(range(4)):
-        status = get_status(id)
-        if not status['ch']:
-            return id
-    raise RuntimeError("Could not find idle tuner")
+    try:
+        return next(id for id in shuffled(range(4)) if not get_status(id)['ch'])
+    except StopIteration:
+        raise RuntimeError("Could not find idle tuner")
 
 
 def _combine(*dicts):
     return dict(DictStack(dicts))
 
 
 def gather_status():
```

### Comparing `jaraco.home-3.5.0/jaraco/home/relay.py` & `jaraco.home-3.6.0/jaraco/home/relay.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.5.0/jaraco/home/thermostat.py` & `jaraco.home-3.6.0/jaraco/home/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.5.0/jaraco.home.egg-info/SOURCES.txt` & `jaraco.home-3.6.0/jaraco.home.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 LICENSE
 NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
+ruff.toml
 setup.cfg
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
@@ -23,8 +24,9 @@
 jaraco.home.egg-info/requires.txt
 jaraco.home.egg-info/top_level.txt
 jaraco/home/Gather HDHomeRun Stats.plist
 jaraco/home/__init__.py
 jaraco/home/hdhomerun.py
 jaraco/home/mock hdhomerun.py
 jaraco/home/relay.py
+jaraco/home/report-spam-call.py
 jaraco/home/thermostat.py
```

### Comparing `jaraco.home-3.5.0/setup.cfg` & `jaraco.home-3.6.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -9,45 +9,36 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
 	requests
 	lxml>=4.2.6
 	pymongo
 	jaraco.functools
 	jaraco.mongodb
 	dnspython
 	keyring
 	jaraco.collections
-
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
+	splinter[selenium]
+	autocommand
 
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
+	pytest-mypy
 	pytest-enabler >= 2.2
-	pytest-ruff
+	pytest-ruff >= 0.2.1
 	
 	types-requests
 	mockproc
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
```

