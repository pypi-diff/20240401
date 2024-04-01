# Comparing `tmp/adafruit-circuitpython-il91874-1.3.1.tar.gz` & `tmp/adafruit-circuitpython-il91874-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-il91874-1.3.1.tar", last modified: Sat Dec  9 17:22:53 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-il91874-1.4.0.tar", last modified: Mon Apr  1 14:29:33 2024, max compression
```

## Comparing `adafruit-circuitpython-il91874-1.3.1.tar` & `adafruit-circuitpython-il91874-1.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.859139 adafruit-circuitpython-il91874-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.851139 adafruit-circuitpython-il91874-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.855139 adafruit-circuitpython-il91874-1.3.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.855139 adafruit-circuitpython-il91874-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.855139 adafruit-circuitpython-il91874-1.3.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2023-12-09 17:22:53.859139 adafruit-circuitpython-il91874-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.859139 adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2023-12-09 17:22:53.000000 adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-12-09 17:22:53.000000 adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:22:53.000000 adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-09 17:22:53.000000 adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-09 17:22:53.000000 adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2023-12-09 17:22:47.000000 adafruit-circuitpython-il91874-1.3.1/adafruit_il91874.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.855139 adafruit-circuitpython-il91874-1.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.855139 adafruit-circuitpython-il91874-1.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:22:53.859139 adafruit-circuitpython-il91874-1.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   360122 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-12-09 17:22:47.000000 adafruit-circuitpython-il91874-1.3.1/examples/il91874_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-09 17:22:47.000000 adafruit-circuitpython-il91874-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-09 17:22:41.000000 adafruit-circuitpython-il91874-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:22:53.859139 adafruit-circuitpython-il91874-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.445633 adafruit-circuitpython-il91874-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.437633 adafruit-circuitpython-il91874-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.437633 adafruit-circuitpython-il91874-1.4.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.441633 adafruit-circuitpython-il91874-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.441633 adafruit-circuitpython-il91874-1.4.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-01 14:29:33.445633 adafruit-circuitpython-il91874-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.445633 adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-01 14:29:33.000000 adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-01 14:29:33.000000 adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:29:33.000000 adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 14:29:33.000000 adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 14:29:33.000000 adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-01 14:29:31.000000 adafruit-circuitpython-il91874-1.4.0/adafruit_il91874.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.441633 adafruit-circuitpython-il91874-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.441633 adafruit-circuitpython-il91874-1.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:33.445633 adafruit-circuitpython-il91874-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   360122 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-01 14:29:31.000000 adafruit-circuitpython-il91874-1.4.0/examples/il91874_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-01 14:29:31.000000 adafruit-circuitpython-il91874-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 14:29:22.000000 adafruit-circuitpython-il91874-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:29:33.445633 adafruit-circuitpython-il91874-1.4.0/setup.cfg
```

### Comparing `adafruit-circuitpython-il91874-1.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-il91874-1.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/.gitignore` & `adafruit-circuitpython-il91874-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/.pre-commit-config.yaml` & `adafruit-circuitpython-il91874-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/.pylintrc` & `adafruit-circuitpython-il91874-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-il91874-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/LICENSE` & `adafruit-circuitpython-il91874-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-il91874-1.4.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/LICENSES/MIT.txt` & `adafruit-circuitpython-il91874-1.4.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-il91874-1.4.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/PKG-INFO` & `adafruit-circuitpython-il91874-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-il91874
-Version: 1.3.1
+Version: 1.4.0
 Summary: CircuitPython `displayio` driver for IL91874-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IL91874
 Keywords: adafruit,blinka,circuitpython,micropython,il91874,displayio,epd,epaper
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-il91874/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/il91874/en/latest/
```

### Comparing `adafruit-circuitpython-il91874-1.3.1/README.rst` & `adafruit-circuitpython-il91874-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/PKG-INFO` & `adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-il91874
-Version: 1.3.1
+Version: 1.4.0
 Summary: CircuitPython `displayio` driver for IL91874-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IL91874
 Keywords: adafruit,blinka,circuitpython,micropython,il91874,displayio,epd,epaper
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-il91874/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/il91874/en/latest/
```

### Comparing `adafruit-circuitpython-il91874-1.3.1/adafruit_circuitpython_il91874.egg-info/SOURCES.txt` & `adafruit-circuitpython-il91874-1.4.0/adafruit_circuitpython_il91874.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/adafruit_il91874.py` & `adafruit-circuitpython-il91874-1.4.0/adafruit_il91874.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,17 +21,23 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-import displayio
+# Compatibility with both CircuitPython 8.x.x and 9.x.x.
+# Remove after 8.x.x is no longer a supported release.
+try:
+    from epaperdisplay import EPaperDisplay
+    from fourwire import FourWire
+except ImportError:
+    from displayio import EPaperDisplay, FourWire
 
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IL91874.git"
 
 _START_SEQUENCE = (
     b"\x04\x00"  # Power on
     b"\x00\x01\xaf"  # panel setting
     b"\x30\x01\x3a"  # PLL
     b"\x01\x05\x03\x00\x2b\x2b\x09"  # power setting
@@ -63,18 +69,18 @@
     b"\x16\x80\x00"  # PDRF
 )
 
 _STOP_SEQUENCE = b"\x02\x01\x17"  # Power off
 
 
 # pylint: disable=too-few-public-methods
-class IL91874(displayio.EPaperDisplay):
+class IL91874(EPaperDisplay):
     """IL91874 display driver"""
 
-    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
+    def __init__(self, bus: FourWire, **kwargs) -> None:
         start_sequence = bytearray(_START_SEQUENCE)
 
         width = kwargs["width"]
         height = kwargs["height"]
         if "rotation" in kwargs and kwargs["rotation"] % 180 != 0:
             width, height = height, width
         start_sequence[-7] = (width >> 8) & 0xFF
```

### Comparing `adafruit-circuitpython-il91874-1.3.1/docs/_static/favicon.ico` & `adafruit-circuitpython-il91874-1.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/docs/conf.py` & `adafruit-circuitpython-il91874-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/docs/index.rst` & `adafruit-circuitpython-il91874-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/examples/display-ruler.bmp` & `adafruit-circuitpython-il91874-1.4.0/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.3.1/examples/il91874_simpletest.py` & `adafruit-circuitpython-il91874-1.4.0/examples/il91874_simpletest.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,37 @@
   This program only requires the adafruit_il91874 library in /lib
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
+    # pylint: disable=ungrouped-imports
+    from displayio import FourWire
+
 import adafruit_il91874
 
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
 display = adafruit_il91874.IL91874(
     display_bus,
```

### Comparing `adafruit-circuitpython-il91874-1.3.1/pyproject.toml` & `adafruit-circuitpython-il91874-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-il91874"
 description = "CircuitPython `displayio` driver for IL91874-based ePaper displays"
-version = "1.3.1"
+version = "1.4.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IL91874"}
 keywords = [
     "adafruit",
```

