# Comparing `tmp/adafruit-circuitpython-hx8357-1.4.2.tar.gz` & `tmp/adafruit-circuitpython-hx8357-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-hx8357-1.4.2.tar", last modified: Mon Mar 25 13:46:56 2024, max compression
+gzip compressed data, was "adafruit-circuitpython-hx8357-1.4.3.tar", last modified: Mon Apr  1 15:23:35 2024, max compression
```

## Comparing `adafruit-circuitpython-hx8357-1.4.2.tar` & `adafruit-circuitpython-hx8357-1.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.045238 adafruit-circuitpython-hx8357-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.049238 adafruit-circuitpython-hx8357-1.4.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.049238 adafruit-circuitpython-hx8357-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.049238 adafruit-circuitpython-hx8357-1.4.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-25 13:46:56.000000 adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-25 13:46:56.000000 adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:46:56.000000 adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-25 13:46:56.000000 adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-25 13:46:56.000000 adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2531 2024-03-25 13:46:53.000000 adafruit-circuitpython-hx8357-1.4.2/adafruit_hx8357.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-25 13:46:53.000000 adafruit-circuitpython-hx8357-1.4.2/examples/hx8357_pitft_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-25 13:46:53.000000 adafruit-circuitpython-hx8357-1.4.2/examples/hx8357_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-25 13:46:53.000000 adafruit-circuitpython-hx8357-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-25 13:46:46.000000 adafruit-circuitpython-hx8357-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:46:56.053238 adafruit-circuitpython-hx8357-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.871945 adafruit-circuitpython-hx8357-1.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.875945 adafruit-circuitpython-hx8357-1.4.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.875945 adafruit-circuitpython-hx8357-1.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.875945 adafruit-circuitpython-hx8357-1.4.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-01 15:23:35.000000 adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 15:23:35.000000 adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:23:35.000000 adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 15:23:35.000000 adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 15:23:35.000000 adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-04-01 15:23:32.000000 adafruit-circuitpython-hx8357-1.4.3/adafruit_hx8357.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-01 15:23:32.000000 adafruit-circuitpython-hx8357-1.4.3/examples/hx8357_pitft_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-01 15:23:32.000000 adafruit-circuitpython-hx8357-1.4.3/examples/hx8357_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-01 15:23:32.000000 adafruit-circuitpython-hx8357-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 15:23:23.000000 adafruit-circuitpython-hx8357-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:23:35.879945 adafruit-circuitpython-hx8357-1.4.3/setup.cfg
```

### Comparing `adafruit-circuitpython-hx8357-1.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-hx8357-1.4.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/.gitignore` & `adafruit-circuitpython-hx8357-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/.pre-commit-config.yaml` & `adafruit-circuitpython-hx8357-1.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/.pylintrc` & `adafruit-circuitpython-hx8357-1.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-hx8357-1.4.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/LICENSE` & `adafruit-circuitpython-hx8357-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-hx8357-1.4.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/LICENSES/MIT.txt` & `adafruit-circuitpython-hx8357-1.4.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-hx8357-1.4.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/PKG-INFO` & `adafruit-circuitpython-hx8357-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hx8357
-Version: 1.4.2
+Version: 1.4.3
 Summary: displayio driver for hx8357 and ILI9340 TFT-LCD displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_hx8357
 Keywords: adafruit,blinka,circuitpython,micropython,hx8357,display,tft,lcd,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hx8357-1.4.2/README.rst` & `adafruit-circuitpython-hx8357-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/PKG-INFO` & `adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hx8357
-Version: 1.4.2
+Version: 1.4.3
 Summary: displayio driver for hx8357 and ILI9340 TFT-LCD displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_hx8357
 Keywords: adafruit,blinka,circuitpython,micropython,hx8357,display,tft,lcd,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hx8357-1.4.2/adafruit_circuitpython_hx8357.egg-info/SOURCES.txt` & `adafruit-circuitpython-hx8357-1.4.3/adafruit_circuitpython_hx8357.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/adafruit_hx8357.py` & `adafruit-circuitpython-hx8357-1.4.3/adafruit_hx8357.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,34 +22,37 @@
 * Adafruit TFT FeatherWing - 3.5" 480x320 Touchscreen for Feathers:
   <https://www.adafruit.com/product/3651>
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
+
+** Datasheet:**
+  https://cdn-shop.adafruit.com/datasheets/HX8357-D_DS_April2012.pdf
 """
 
 # imports
 # Support both 8.x.x and 9.x.x. Remove 8.x method when discontinued.
 try:
     from fourwire import FourWire  # 9.x method
     from busdisplay import BusDisplay
 except ImportError:
     from displayio import FourWire  # 8.x method
     from displayio import Display as BusDisplay
 
-__version__ = "1.4.2"
+__version__ = "1.4.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HX8357.git"
 
 _INIT_SEQUENCE = (
     b"\x01\x80\x64"  # _SWRESET and Delay 100ms
     b"\xB9\x83\xFF\x83\x57\xFF"  # _SETC and delay 500ms
     b"\xB3\x04\x80\x00\x06\x06"  # _SETRGB 0x80 enables SDO pin (0x00 disables)
     b"\xB6\x01\x25"  # _SETCOM -1.52V
-    b"\xB0\x01\x68"  # _SETOSC Normal mode 70Hz, Idle mode 55 Hz
+    b"\xB0\x01\x66"  # _SETOSC Normal mode 60Hz, Idle mode 60 Hz
     b"\xCC\x01\x05"  # _SETPANEL BGR, Gate direction swapped
     b"\xB1\x06\x00\x15\x1C\x1C\x83\xAA"  # _SETPWR1 Not deep standby BT VSPR VSNR AP
     b"\xC0\x06\x50\x50\x01\x3C\x1E\x08"  # _SETSTBA OPON normal OPON idle STBA GEN
     b"\xB4\x07\x02\x40\x00\x2A\x2A\x0D\x78"  # _SETCYC NW 0x02 RTN DIV DUM DUM GDON GDOFF
     b"\xE0\x22\x02\x0A\x11\x1d\x23\x35\x41\x4b\x4b\x42\x3A\x27\x1B\x08\x09\x03\x02\x0A"
     b"\x11\x1d\x23\x35\x41\x4b\x4b\x42\x3A\x27\x1B\x08\x09\x03\x00\x01"  # _SETGAMMA
     b"\x3A\x01\x55"  # _COLMOD 16 bit
```

### Comparing `adafruit-circuitpython-hx8357-1.4.2/docs/_static/favicon.ico` & `adafruit-circuitpython-hx8357-1.4.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/docs/conf.py` & `adafruit-circuitpython-hx8357-1.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/docs/index.rst` & `adafruit-circuitpython-hx8357-1.4.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/examples/hx8357_pitft_simpletest.py` & `adafruit-circuitpython-hx8357-1.4.3/examples/hx8357_pitft_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/examples/hx8357_simpletest.py` & `adafruit-circuitpython-hx8357-1.4.3/examples/hx8357_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hx8357-1.4.2/pyproject.toml` & `adafruit-circuitpython-hx8357-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-hx8357"
 description = "displayio driver for hx8357 and ILI9340 TFT-LCD displays."
-version = "1.4.2"
+version = "1.4.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_hx8357"}
 keywords = [
     "adafruit",
```

