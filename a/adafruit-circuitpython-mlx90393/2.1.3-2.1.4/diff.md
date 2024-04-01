# Comparing `tmp/adafruit-circuitpython-mlx90393-2.1.3.tar.gz` & `tmp/adafruit-circuitpython-mlx90393-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mlx90393-2.1.3.tar", last modified: Sat Dec  9 17:28:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-mlx90393-2.1.4.tar", last modified: Mon Apr  1 14:57:11 2024, max compression
```

## Comparing `adafruit-circuitpython-mlx90393-2.1.3.tar` & `adafruit-circuitpython-mlx90393-2.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.751302 adafruit-circuitpython-mlx90393-2.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.755302 adafruit-circuitpython-mlx90393-2.1.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.755302 adafruit-circuitpython-mlx90393-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.755302 adafruit-circuitpython-mlx90393-2.1.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-12-09 17:28:25.000000 adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-09 17:28:25.000000 adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:28:25.000000 adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-09 17:28:25.000000 adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-09 17:28:25.000000 adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    18430 2023-12-09 17:28:18.000000 adafruit-circuitpython-mlx90393-2.1.3/adafruit_mlx90393.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      717 2023-12-09 17:28:18.000000 adafruit-circuitpython-mlx90393-2.1.3/examples/mlx90393_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-09 17:28:18.000000 adafruit-circuitpython-mlx90393-2.1.3/examples/mlx90393_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-09 17:28:18.000000 adafruit-circuitpython-mlx90393-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-09 17:28:12.000000 adafruit-circuitpython-mlx90393-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:28:25.759302 adafruit-circuitpython-mlx90393-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.687458 adafruit-circuitpython-mlx90393-2.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.679458 adafruit-circuitpython-mlx90393-2.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.683458 adafruit-circuitpython-mlx90393-2.1.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.683458 adafruit-circuitpython-mlx90393-2.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.683458 adafruit-circuitpython-mlx90393-2.1.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-01 14:57:11.687458 adafruit-circuitpython-mlx90393-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.687458 adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-01 14:57:11.000000 adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 14:57:11.000000 adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:57:11.000000 adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 14:57:11.000000 adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 14:57:11.000000 adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18281 2024-04-01 14:57:08.000000 adafruit-circuitpython-mlx90393-2.1.4/adafruit_mlx90393.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.683458 adafruit-circuitpython-mlx90393-2.1.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.683458 adafruit-circuitpython-mlx90393-2.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:57:11.687458 adafruit-circuitpython-mlx90393-2.1.4/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-04-01 14:57:08.000000 adafruit-circuitpython-mlx90393-2.1.4/examples/mlx90393_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-01 14:57:08.000000 adafruit-circuitpython-mlx90393-2.1.4/examples/mlx90393_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-01 14:57:08.000000 adafruit-circuitpython-mlx90393-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 14:57:00.000000 adafruit-circuitpython-mlx90393-2.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:57:11.687458 adafruit-circuitpython-mlx90393-2.1.4/setup.cfg
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mlx90393-2.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/.gitignore` & `adafruit-circuitpython-mlx90393-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/.pre-commit-config.yaml` & `adafruit-circuitpython-mlx90393-2.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/.pylintrc` & `adafruit-circuitpython-mlx90393-2.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mlx90393-2.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/LICENSE` & `adafruit-circuitpython-mlx90393-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mlx90393-2.1.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/LICENSES/MIT.txt` & `adafruit-circuitpython-mlx90393-2.1.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mlx90393-2.1.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/PKG-INFO` & `adafruit-circuitpython-mlx90393-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mlx90393
-Version: 2.1.3
+Version: 2.1.4
 Summary: CircuitPython driver for the MLX90393 3-axis magnetometer.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MLX90393
 Keywords: adafruit,three-axis,magnetometer,magnet,mlx90393,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/README.rst` & `adafruit-circuitpython-mlx90393-2.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO` & `adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mlx90393
-Version: 2.1.3
+Version: 2.1.4
 Summary: CircuitPython driver for the MLX90393 3-axis magnetometer.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MLX90393
 Keywords: adafruit,three-axis,magnetometer,magnet,mlx90393,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt` & `adafruit-circuitpython-mlx90393-2.1.4/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/adafruit_mlx90393.py` & `adafruit-circuitpython-mlx90393-2.1.4/adafruit_mlx90393.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 try:
     from typing import Tuple
     from circuitpython_typing import ReadableBuffer
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.1.3"
+__version__ = "2.1.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MLX90393.git"
 
 _CMD_SB = const(0b00010000)  # Start burst mode
 _CMD_SW = const(0b00100000)  # Start wakeup on change mode
 _CMD_SM = const(0b00110000)  # Start single-measurement mode
 _CMD_RM = const(0b01000000)  # Read measurement
 _CMD_RR = const(0b01010000)  # Read register
@@ -402,23 +402,20 @@
 
     def read_reg(self, reg: int) -> int:
         """
         Gets the current value of the specified register.
 
         :param int reg: The register to read
         """
-        # Write 'value' to the specified register
+        # Read register
         payload = bytes([_CMD_RR, reg << 2])
-        with self.i2c_device as i2c:
-            i2c.write(payload)
-
-        # Read the response (+1 to account for the mandatory status byte!)
         data = bytearray(3)
         with self.i2c_device as i2c:
-            i2c.readinto(data)
+            i2c.write_then_readinto(payload, data)
+
         # Unpack data (status byte, big-endian 16-bit register value)
         self._status_last, val = struct.unpack(">BH", data)
         if self._debug:
             print("\t[{}]".format(time.monotonic()))
             print("\t Writing :", [hex(b) for b in payload])
             print("\tResponse :", [hex(b) for b in data])
             print("\t  Status :", hex(data[0]))
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/docs/_static/favicon.ico` & `adafruit-circuitpython-mlx90393-2.1.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/docs/conf.py` & `adafruit-circuitpython-mlx90393-2.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/docs/index.rst` & `adafruit-circuitpython-mlx90393-2.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/examples/mlx90393_simpletest.py` & `adafruit-circuitpython-mlx90393-2.1.4/examples/mlx90393_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/examples/mlx90393_temperature.py` & `adafruit-circuitpython-mlx90393-2.1.4/examples/mlx90393_temperature.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.3/pyproject.toml` & `adafruit-circuitpython-mlx90393-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mlx90393"
 description = "CircuitPython driver for the MLX90393 3-axis magnetometer."
-version = "2.1.3"
+version = "2.1.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MLX90393"}
 keywords = [
     "adafruit",
```

