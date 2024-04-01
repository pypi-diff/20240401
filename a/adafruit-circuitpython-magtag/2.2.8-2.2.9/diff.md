# Comparing `tmp/adafruit-circuitpython-magtag-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-magtag-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-magtag-2.2.8.tar", last modified: Mon Oct  2 21:37:58 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-magtag-2.2.9.tar", last modified: Sat Dec  9 17:45:24 2023, max compression
```

## Comparing `adafruit-circuitpython-magtag-2.2.8.tar` & `adafruit-circuitpython-magtag-2.2.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.003310 adafruit-circuitpython-magtag-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.003310 adafruit-circuitpython-magtag-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.003310 adafruit-circuitpython-magtag-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.003310 adafruit-circuitpython-magtag-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-10-02 21:37:57.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-02 21:37:57.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 21:37:57.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-10-02 21:37:57.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-02 21:37:57.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3364 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7326 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/magtag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2595 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/network.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5897 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/examples/magtag_btn_sleep_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/examples/magtag_quote_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/examples/magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-10-02 21:37:50.000000 adafruit-circuitpython-magtag-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-10-02 21:37:42.000000 adafruit-circuitpython-magtag-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-02 21:37:58.007310 adafruit-circuitpython-magtag-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.639194 adafruit-circuitpython-magtag-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.639194 adafruit-circuitpython-magtag-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.643194 adafruit-circuitpython-magtag-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.643194 adafruit-circuitpython-magtag-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2023-12-09 17:45:24.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-12-09 17:45:24.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:45:24.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-09 17:45:24.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-09 17:45:24.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.643194 adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3364 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7326 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/magtag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2595 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5897 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/examples/magtag_btn_sleep_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/examples/magtag_quote_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/examples/magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-09 17:45:18.000000 adafruit-circuitpython-magtag-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-09 17:45:11.000000 adafruit-circuitpython-magtag-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:45:24.647194 adafruit-circuitpython-magtag-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-magtag-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/.gitignore` & `adafruit-circuitpython-magtag-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-magtag-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/.pylintrc` & `adafruit-circuitpython-magtag-2.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-magtag-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/LICENSE` & `adafruit-circuitpython-magtag-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-magtag-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-magtag-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-magtag-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/PKG-INFO` & `adafruit-circuitpython-magtag-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-magtag
-Version: 2.2.8
+Version: 2.2.9
 Summary: Helper library for the Adafruit MagTag
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MagTag
 Keywords: adafruit,magtag,eink,iot,esp32,espressif,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/README.rst` & `adafruit-circuitpython-magtag-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/PKG-INFO` & `adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-magtag
-Version: 2.2.8
+Version: 2.2.9
 Summary: Helper library for the Adafruit MagTag
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MagTag
 Keywords: adafruit,magtag,eink,iot,esp32,espressif,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/adafruit_circuitpython_magtag.egg-info/SOURCES.txt` & `adafruit-circuitpython-magtag-2.2.9/adafruit_circuitpython_magtag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/graphics.py` & `adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from adafruit_portalbase.graphics import GraphicsBase
 
 try:
     from typing import Union, Optional, Tuple
 except ImportError:
     pass
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the MagTag Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/magtag.py` & `adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/magtag.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 try:
     from typing import Optional, Union, Sequence, Dict, Callable, Any
     import microcontroller
     import neopixel
 except ImportError:
     pass
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class MagTag(PortalBase):
     """Class representing the Adafruit MagTag.
 
     :param url: The URL of your data source. Defaults to ``None``.
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/network.py` & `adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Optional, Union
     import microcontroller
 except ImportError:
     pass
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit MagTag.
 
     :param status_neopixel: The pin for the status NeoPixel. Use ``board.NEOPIXEL`` for the on-board
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/adafruit_magtag/peripherals.py` & `adafruit-circuitpython-magtag-2.2.9/adafruit_magtag/peripherals.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import board
 from digitalio import DigitalInOut, Direction, Pull
 from analogio import AnalogIn
 import neopixel
 import simpleio
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the MagTag Library"""
 
     # pylint: disable=too-many-instance-attributes, too-many-locals, too-many-branches, too-many-statements
```

### Comparing `adafruit-circuitpython-magtag-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-magtag-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/docs/conf.py` & `adafruit-circuitpython-magtag-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/docs/index.rst` & `adafruit-circuitpython-magtag-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/examples/magtag_btn_sleep_demo.py` & `adafruit-circuitpython-magtag-2.2.9/examples/magtag_btn_sleep_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/examples/magtag_quote_demo.py` & `adafruit-circuitpython-magtag-2.2.9/examples/magtag_quote_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/examples/magtag_simpletest.py` & `adafruit-circuitpython-magtag-2.2.9/examples/magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.8/pyproject.toml` & `adafruit-circuitpython-magtag-2.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-magtag"
 description = "Helper library for the Adafruit MagTag"
-version = "2.2.8"
+version = "2.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag"}
 keywords = [
     "adafruit",
```

