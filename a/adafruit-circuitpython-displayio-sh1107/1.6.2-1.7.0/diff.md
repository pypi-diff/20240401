# Comparing `tmp/adafruit-circuitpython-displayio-sh1107-1.6.2.tar.gz` & `tmp/adafruit-circuitpython-displayio-sh1107-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-sh1107-1.6.2.tar", last modified: Mon Mar 25 22:14:38 2024, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-sh1107-1.7.0.tar", last modified: Mon Apr  1 14:01:12 2024, max compression
```

## Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2.tar` & `adafruit-circuitpython-displayio-sh1107-1.7.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.201179 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.205179 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.205179 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.205179 adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-25 22:14:38.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-25 22:14:38.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 22:14:38.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 22:14:38.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-25 22:14:38.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-03-25 22:14:35.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_displayio_sh1107.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-03-25 22:14:35.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_game_of_life.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-25 22:14:35.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_mono_128x128_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-25 22:14:35.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_random_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-25 22:14:35.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-25 22:14:35.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-25 22:14:29.000000 adafruit-circuitpython-displayio-sh1107-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 22:14:38.209179 adafruit-circuitpython-displayio-sh1107-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.971779 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.975779 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.975779 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.975779 adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-01 14:01:12.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 14:01:12.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:01:12.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 14:01:12.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 14:01:12.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-01 14:01:10.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_displayio_sh1107.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-01 14:01:10.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_game_of_life.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-01 14:01:10.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_mono_128x128_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-01 14:01:10.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_random_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-01 14:01:10.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-01 14:01:10.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 14:01:03.000000 adafruit-circuitpython-displayio-sh1107-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:01:12.979779 adafruit-circuitpython-displayio-sh1107-1.7.0/setup.cfg
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-displayio-sh1107-1.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/.gitignore` & `adafruit-circuitpython-displayio-sh1107-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-sh1107-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/.pylintrc` & `adafruit-circuitpython-displayio-sh1107-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-sh1107-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSE` & `adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-sh1107-1.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/PKG-INFO` & `adafruit-circuitpython-displayio-sh1107-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-sh1107
-Version: 1.6.2
+Version: 1.7.0
 Summary: Support for the SH1107 OLED display driver IC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_sh1107,display,oled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
+Requires-Dist: Adafruit-Blinka-Displayio
 Provides-Extra: optional
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-displayio-sh1107/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/displayio-sh1107/en/latest/
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/README.rst` & `adafruit-circuitpython-displayio-sh1107-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-sh1107
-Version: 1.6.2
+Version: 1.7.0
 Summary: Support for the SH1107 OLED display driver IC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_sh1107,display,oled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
+Requires-Dist: Adafruit-Blinka-Displayio
 Provides-Extra: optional
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-displayio-sh1107/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/displayio-sh1107/en/latest/
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/adafruit_displayio_sh1107.py` & `adafruit-circuitpython-displayio-sh1107-1.7.0/adafruit_displayio_sh1107.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,23 +23,38 @@
 
 * Adafruit CircuitPython (version 6+) firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import sys
-import displayio
+
+
+try:
+    from busdisplay import BusDisplay as Display
+    from fourwire import FourWire
+except ImportError:
+    from displayio import Display
+    from displayio import FourWire
+
 from micropython import const
 
 try:
     from typing import Union
+
+    try:
+        from i2cdisplaybus import I2CDisplayBus
+    except ImportError:
+        # pylint: disable=ungrouped-imports
+        from displayio import I2CDisplay as I2CDisplayBus
+
 except ImportError:
     pass
 
-__version__ = "1.6.2"
+__version__ = "1.7.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107.git"
 
 
 DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650 = const(0x60)
 """
 The hardware display offset to use when configuring the SH1107 for the
 `Adafruit Featherwing 128x64 OLED <https://www.adafruit.com/product/4650>`_.
@@ -126,15 +141,15 @@
         b"\xa6\x00"  # normal (not reversed) display
         b"\xaf\x00"  # DISPLAY_ON
     )
     _PIXELS_IN_ROW = False
     _ROTATION_OFFSET = 90
 
 
-class SH1107(displayio.Display):
+class SH1107(Display):
     """
     SH1107 driver for use with DisplayIO
 
     :param bus: The bus that the display is connected to.
     :param int width: The width of the display. Maximum of 128
     :param int height: The height of the display. Maximum of 128
     :param int rotation: The rotation of the display. 0, 90, 180 or 270.
@@ -142,15 +157,15 @@
         This will be dependent on the OLED display and two displays with the
         same dimensions could have different offsets. This defaults to
         `DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650`
     """
 
     def __init__(
         self,
-        bus: Union[displayio.I2CDisplay, displayio.FourWire],
+        bus: Union[I2CDisplayBus, FourWire],
         display_offset: int = DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650,
         rotation: int = 0,
         **kwargs
     ) -> None:
         rotation = (rotation + _ROTATION_OFFSET) % 360
         if rotation in (0, 180):
             multiplex = kwargs["width"] - 1
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-sh1107-1.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/docs/conf.py` & `adafruit-circuitpython-displayio-sh1107-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/docs/index.rst` & `adafruit-circuitpython-displayio-sh1107-1.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_game_of_life.py` & `adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_game_of_life.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 
 import random
 import time
 
 import board
 import displayio
+
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from i2cdisplaybus import I2CDisplayBus
+except ImportError:
+    from displayio import I2CDisplay as I2CDisplayBus
+
 import adafruit_displayio_sh1107
 
 displayio.release_displays()
 
 
 def apply_life_rule(old, new):
     """
@@ -89,15 +97,15 @@
         y = output.height - len(conway_data) - 2 + i
         for j, cj in enumerate(si):
             output[(output.width - 8) // 2 + j, y] = cj & 1
 
 
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3C)
+display_bus = I2CDisplayBus(i2c, device_address=0x3C)
 
 # SH1107 is vertically oriented 64x128
 WIDTH = 128
 HEIGHT = 64
 display = adafruit_displayio_sh1107.SH1107(display_bus, width=WIDTH, height=HEIGHT)
 
 SCALE = 2  # scale up for the small OLED pixels!
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_mono_128x128_test.py` & `adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_mono_128x128_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,41 @@
 Based on example by Mark Roberts (mdroberts1243).
 
 This example writes text to the display, and draws a series of squares and a rectangle.
 """
 
 import board
 import displayio
+
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from i2cdisplaybus import I2CDisplayBus
+
+    # from fourwire import FourWire
+except ImportError:
+    from displayio import I2CDisplay as I2CDisplayBus
+
+    # from displayio import FourWire
+
 import terminalio
 from adafruit_display_text import bitmap_label as label
 from adafruit_displayio_sh1107 import SH1107, DISPLAY_OFFSET_ADAFRUIT_128x128_OLED_5297
 
 displayio.release_displays()
 
 # For I2C
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3D)
+display_bus = I2CDisplayBus(i2c, device_address=0x3D)
 
 # For SPI:
 # import busio
 # spi_bus = busio.SPI(board.SCK, board.MOSI)
-# display_bus = displayio.FourWire(spi_bus, command=board.D6, chip_select=board.D5, reset=board.D9)
+# display_bus = FourWire(spi_bus, command=board.D6, chip_select=board.D5, reset=board.D9)
 
 # Width, height and rotation for Monochrome 1.12" 128x128 OLED
 WIDTH = 128
 HEIGHT = 128
 ROTATION = 90
 
 # Border width
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_random_motion.py` & `adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_random_motion.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 
 """
 
 import random
 import time
 import board
 import displayio
+
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from i2cdisplaybus import I2CDisplayBus
+except ImportError:
+    from displayio import I2CDisplay as I2CDisplayBus
+
 import terminalio
 
 # can try import bitmap_label below for alternative
 from adafruit_display_text import label
 import adafruit_displayio_sh1107
 
 displayio.release_displays()
 # oled_reset = board.D9
 
 # Use for I2C
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3C)
+display_bus = I2CDisplayBus(i2c, device_address=0x3C)
 
 # SH1107 is vertically oriented 64x128
 WIDTH = 128
 HEIGHT = 64
 BORDER = 2
 
 display = adafruit_displayio_sh1107.SH1107(display_bus, width=WIDTH, height=HEIGHT)
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/examples/displayio_sh1107_simpletest.py` & `adafruit-circuitpython-displayio-sh1107-1.7.0/examples/displayio_sh1107_simpletest.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,27 +7,35 @@
 background, a smaller black rectangle, miscellaneous stuff and some white text.
 
 """
 
 
 import board
 import displayio
+
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from i2cdisplaybus import I2CDisplayBus
+except ImportError:
+    from displayio import I2CDisplay as I2CDisplayBus
+
 import terminalio
 
 # can try import bitmap_label below for alternative
 from adafruit_display_text import label
 import adafruit_displayio_sh1107
 
 displayio.release_displays()
 # oled_reset = board.D9
 
 # Use for I2C
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3C)
+display_bus = I2CDisplayBus(i2c, device_address=0x3C)
 
 # SH1107 is vertically oriented 64x128
 WIDTH = 128
 HEIGHT = 64
 BORDER = 2
 
 display = adafruit_displayio_sh1107.SH1107(
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.6.2/pyproject.toml` & `adafruit-circuitpython-displayio-sh1107-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-displayio-sh1107"
 description = "Support for the SH1107 OLED display driver IC"
-version = "1.6.2"
+version = "1.7.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107"}
 keywords = [
     "adafruit",
```

