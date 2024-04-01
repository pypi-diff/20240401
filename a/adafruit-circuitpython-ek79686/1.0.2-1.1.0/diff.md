# Comparing `tmp/adafruit-circuitpython-ek79686-1.0.2.tar.gz` & `tmp/adafruit-circuitpython-ek79686-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ek79686-1.0.2.tar", last modified: Sat Dec  9 17:21:07 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ek79686-1.1.0.tar", last modified: Mon Apr  1 14:50:51 2024, max compression
```

## Comparing `adafruit-circuitpython-ek79686-1.0.2.tar` & `adafruit-circuitpython-ek79686-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.447080 adafruit-circuitpython-ek79686-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.439081 adafruit-circuitpython-ek79686-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.443081 adafruit-circuitpython-ek79686-1.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.443081 adafruit-circuitpython-ek79686-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.443081 adafruit-circuitpython-ek79686-1.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-12-09 17:21:07.447080 adafruit-circuitpython-ek79686-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.447080 adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-12-09 17:21:07.000000 adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-12-09 17:21:07.000000 adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:21:07.000000 adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-09 17:21:07.000000 adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-09 17:21:07.000000 adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2264 2023-12-09 17:21:01.000000 adafruit-circuitpython-ek79686-1.0.2/adafruit_ek79686.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.443081 adafruit-circuitpython-ek79686-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.447080 adafruit-circuitpython-ek79686-1.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:21:07.447080 adafruit-circuitpython-ek79686-1.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   360122 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-09 17:21:01.000000 adafruit-circuitpython-ek79686-1.0.2/examples/ek79686_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-12-09 17:21:01.000000 adafruit-circuitpython-ek79686-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-09 17:20:54.000000 adafruit-circuitpython-ek79686-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:21:07.447080 adafruit-circuitpython-ek79686-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.686000 adafruit-circuitpython-ek79686-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.678000 adafruit-circuitpython-ek79686-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.682000 adafruit-circuitpython-ek79686-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.682000 adafruit-circuitpython-ek79686-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.682000 adafruit-circuitpython-ek79686-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-01 14:50:51.686000 adafruit-circuitpython-ek79686-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.686000 adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-01 14:50:51.000000 adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-01 14:50:51.000000 adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:50:51.000000 adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 14:50:51.000000 adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 14:50:51.000000 adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2493 2024-04-01 14:50:49.000000 adafruit-circuitpython-ek79686-1.1.0/adafruit_ek79686.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.682000 adafruit-circuitpython-ek79686-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.682000 adafruit-circuitpython-ek79686-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:50:51.686000 adafruit-circuitpython-ek79686-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   360122 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-01 14:50:49.000000 adafruit-circuitpython-ek79686-1.1.0/examples/ek79686_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-01 14:50:49.000000 adafruit-circuitpython-ek79686-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-01 14:50:39.000000 adafruit-circuitpython-ek79686-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:50:51.686000 adafruit-circuitpython-ek79686-1.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ek79686-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ek79686-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/.gitignore` & `adafruit-circuitpython-ek79686-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/.pre-commit-config.yaml` & `adafruit-circuitpython-ek79686-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/.pylintrc` & `adafruit-circuitpython-ek79686-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ek79686-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/LICENSE` & `adafruit-circuitpython-ek79686-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ek79686-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/LICENSES/MIT.txt` & `adafruit-circuitpython-ek79686-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ek79686-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/PKG-INFO` & `adafruit-circuitpython-ek79686-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ek79686
-Version: 1.0.2
+Version: 1.1.0
 Summary: CircuitPython `displayio` driver for EK79686-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_EK79686
 Keywords: adafruit,blinka,circuitpython,micropython,ek79686,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ek79686-1.0.2/README.rst` & `adafruit-circuitpython-ek79686-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/PKG-INFO` & `adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ek79686
-Version: 1.0.2
+Version: 1.1.0
 Summary: CircuitPython `displayio` driver for EK79686-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_EK79686
 Keywords: adafruit,blinka,circuitpython,micropython,ek79686,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ek79686-1.0.2/adafruit_circuitpython_ek79686.egg-info/SOURCES.txt` & `adafruit-circuitpython-ek79686-1.1.0/adafruit_circuitpython_ek79686.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/adafruit_ek79686.py` & `adafruit-circuitpython-ek79686-1.1.0/adafruit_ek79686.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,24 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
 import math
-import displayio
 
-__version__ = "1.0.2"
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from epaperdisplay import EPaperDisplay
+    from fourwire import FourWire
+except ImportError:
+    from displayio import EPaperDisplay, FourWire
+
+__version__ = "1.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_EK79686.git"
 
 _START_SEQUENCE = (
     b"\x00\x01\x0F"  # LUT from OTP 176x264
     b"\x4D\x01\xAA"  # FITI cmd (???)
     b"\x87\x01\x28"
     b"\x84\x01\x00"
@@ -50,18 +57,18 @@
     b"\x04\x00"  # Power on
 )
 
 _STOP_SEQUENCE = b"\x02\x01\xff" b"\x07\x01\xa5"  # Power off  # Deep sleep
 
 
 # pylint: disable=too-few-public-methods
-class EK79686(displayio.EPaperDisplay):
+class EK79686(EPaperDisplay):
     """EK79686 display driver"""
 
-    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
+    def __init__(self, bus: FourWire, **kwargs) -> None:
         start_sequence = bytearray(_START_SEQUENCE)
 
         width = 8 * math.ceil(kwargs["width"] / 8)
         height = 8 * math.ceil(kwargs["height"] / 8)
         if "rotation" in kwargs and kwargs["rotation"] % 180 == 0:
             width, height = height, width
             kwargs["width"] = width
```

### Comparing `adafruit-circuitpython-ek79686-1.0.2/docs/_static/favicon.ico` & `adafruit-circuitpython-ek79686-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/docs/conf.py` & `adafruit-circuitpython-ek79686-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/docs/index.rst` & `adafruit-circuitpython-ek79686-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/examples/display-ruler.bmp` & `adafruit-circuitpython-ek79686-1.1.0/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ek79686-1.0.2/examples/ek79686_simpletest.py` & `adafruit-circuitpython-ek79686-1.1.0/examples/ek79686_simpletest.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,28 +11,36 @@
   This program only requires the adafruit_ek79686 library in /lib
   for CircuitPython 5.0 and above which has displayio support.
 """
 
 import time
 import board
 import displayio
+
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from fourwire import FourWire
+except ImportError:
+    from displayio import FourWire
+
 import adafruit_ek79686
 
 # Used to ensure the display is free in CircuitPython
 displayio.release_displays()
 
 # Define the pins needed for display use on the Metro
 spi = board.SPI()
 epd_cs = board.D10
 epd_dc = board.D9
 epd_reset = board.D5
 epd_busy = board.D6
 
 # Create the displayio connection to the display pins
-display_bus = displayio.FourWire(
+display_bus = FourWire(
     spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset, baudrate=1000000
 )
 time.sleep(1)  # Wait a bit
 
 # Create the display object - the third color is red (0xff0000)
 display = adafruit_ek79686.EK79686(
     display_bus,
@@ -56,15 +64,15 @@
         pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
     )
     # CircuitPython 7 compatible only
     # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     # Place the display group on the screen (does not refresh)
-    display.show(g)
+    display.root_group = g
 
     # Show the image on the display
     display.refresh()
 
     print("refreshed")
 
     # Do Not refresh the screen more often than every 180 seconds
```

### Comparing `adafruit-circuitpython-ek79686-1.0.2/pyproject.toml` & `adafruit-circuitpython-ek79686-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ek79686"
 description = "CircuitPython `displayio` driver for EK79686-based ePaper displays"
-version = "1.0.2"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_EK79686"}
 keywords = [
     "adafruit",
```

