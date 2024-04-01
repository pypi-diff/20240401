# Comparing `tmp/adafruit-circuitpython-displayio-ssd1306-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-displayio-ssd1306-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-ssd1306-2.0.0.tar", last modified: Tue Mar 19 22:29:23 2024, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-ssd1306-2.0.1.tar", last modified: Mon Apr  1 13:53:23 2024, max compression
```

## Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0.tar` & `adafruit-circuitpython-displayio-ssd1306-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.746940 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.750941 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.750941 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.750941 adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-19 22:29:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-19 22:29:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 22:29:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-19 22:29:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 22:29:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-03-19 22:29:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_displayio_ssd1306.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-19 22:29:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_64x32_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-19 22:29:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-19 22:29:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_picowbell_tempsensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-19 22:29:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-19 22:29:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-19 22:29:12.000000 adafruit-circuitpython-displayio-ssd1306-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 22:29:23.754941 adafruit-circuitpython-displayio-ssd1306-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.284380 adafruit-circuitpython-displayio-ssd1306-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.276380 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.280380 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.280380 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.280380 adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-01 13:53:23.284380 adafruit-circuitpython-displayio-ssd1306-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.284380 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-01 13:53:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 13:53:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:53:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 13:53:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 13:53:23.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-01 13:53:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_displayio_ssd1306.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.280380 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.284380 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:53:23.284380 adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-01 13:53:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_64x32_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-01 13:53:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-01 13:53:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_picowbell_tempsensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-01 13:53:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-01 13:53:21.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 13:53:14.000000 adafruit-circuitpython-displayio-ssd1306-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:53:23.284380 adafruit-circuitpython-displayio-ssd1306-2.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/.gitignore` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/.pylintrc` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSE` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/PKG-INFO` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-ssd1306
-Version: 2.0.0
+Version: 2.0.1
 Summary: DisplayIO driver for SSD1306 monochrome displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_ssd1306,displayio,ssd1306,oled
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-displayio-ssd1306/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/displayio_ssd1306/en/latest/
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/README.rst` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-ssd1306
-Version: 2.0.0
+Version: 2.0.1
 Summary: DisplayIO driver for SSD1306 monochrome displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_ssd1306,displayio,ssd1306,oled
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-displayio-ssd1306/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/displayio_ssd1306/en/latest/
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/adafruit_displayio_ssd1306.py` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/adafruit_displayio_ssd1306.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     from fourwire import FourWire
     from i2cdisplaybus import I2CDisplayBus
 except ImportError:
     from displayio import FourWire
     from displayio import I2CDisplay as I2CDisplayBus
     from displayio import Display as BusDisplay
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306.git"
 
 # Sequence from page 19 here: https://cdn-shop.adafruit.com/datasheets/UG-2864HSWEG01+user+guide.pdf
 _INIT_SEQUENCE = (
     b"\xAE\x00"  # DISPLAY_OFF
     b"\x20\x01\x00"  # Set memory addressing to horizontal mode.
     b"\x81\x01\xcf"  # set contrast control
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/conf.py` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/docs/index.rst` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_64x32_simpletest.py` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_64x32_simpletest.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,24 +5,32 @@
 This test will initialize the display using displayio and draw a solid white
 background, a smaller black rectangle, and some white text.
 Customized version of displayio_ssd1306_simpletest.py for 64x32
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
 from adafruit_display_text import label
 import adafruit_displayio_ssd1306
 
 displayio.release_displays()
 
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3C)
+display_bus = I2CDisplayBus(i2c, device_address=0x3C)
 display = adafruit_displayio_ssd1306.SSD1306(display_bus, width=64, height=32)
 
 # Make the display context
 splash = displayio.Group()
 display.root_group = splash
 
 color_bitmap = displayio.Bitmap(64, 32, 1)
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_featherwing.py` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_featherwing.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 """
 This test will initialize the display using displayio and draw a solid white
 background, a smaller black rectangle, and some white text.
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
 from adafruit_display_text import label
 import adafruit_displayio_ssd1306
 
 displayio.release_displays()
 
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3C)
+display_bus = I2CDisplayBus(i2c, device_address=0x3C)
 display = adafruit_displayio_ssd1306.SSD1306(display_bus, width=128, height=32)
 
 # Make the display context
 splash = displayio.Group()
 display.root_group = splash
 
 color_bitmap = displayio.Bitmap(128, 32, 1)
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_picowbell_tempsensor.py` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_picowbell_tempsensor.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 # SPDX-License-Identifier: MIT
 # Pi Pico & Picowbell with SSD1306 display & BME280 sensor
 # Coded for Circuit Python 8.1
 
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
 import busio
 import terminalio
 from adafruit_display_text import label
 from adafruit_bme280 import basic as adafruit_bme280
 import adafruit_displayio_ssd1306 as ssd1306
 
 # Reinitalizes display upon any soft reboot or hard reset
@@ -25,15 +33,15 @@
 bme280 = adafruit_bme280.Adafruit_BME280_I2C(i2c1)
 
 # Configure display size
 ssd_width = 128
 ssd_height = 32
 
 # Ensure the physical address of your SSD1306 is set here:
-ssd_bus = displayio.I2CDisplay(i2c0, device_address=0x3C)
+ssd_bus = I2CDisplayBus(i2c0, device_address=0x3C)
 display = ssd1306.SSD1306(ssd_bus, width=ssd_width, height=ssd_height)
 
 # Manually set your sea_level_pressure to your area
 # This can change houly, lookup NOAA data or automate it.
 # On a normal sunny day it's generally 1013-1015
 bme280.sea_level_pressure = 1013.4
 # If you live at 0 sea level this is a nice workaround
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/examples/displayio_ssd1306_simpletest.py` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/examples/displayio_ssd1306_simpletest.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,32 +4,44 @@
 """
 This test will initialize the display using displayio and draw a solid white
 background, a smaller black rectangle, and some white text.
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
 from adafruit_display_text import label
 import adafruit_displayio_ssd1306
 
 displayio.release_displays()
 
 oled_reset = board.D9
 
 # Use for I2C
 i2c = board.I2C()  # uses board.SCL and board.SDA
 # i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
-display_bus = displayio.I2CDisplay(i2c, device_address=0x3C, reset=oled_reset)
+display_bus = I2CDisplayBus(i2c, device_address=0x3C, reset=oled_reset)
 
 # Use for SPI
 # spi = board.SPI()
 # oled_cs = board.D5
 # oled_dc = board.D6
-# display_bus = displayio.FourWire(spi, command=oled_dc, chip_select=oled_cs,
+# display_bus = FourWire(spi, command=oled_dc, chip_select=oled_cs,
 #                                 reset=oled_reset, baudrate=1000000)
 
 WIDTH = 128
 HEIGHT = 32  # Change to 64 if needed
 BORDER = 5
 
 display = adafruit_displayio_ssd1306.SSD1306(display_bus, width=WIDTH, height=HEIGHT)
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-2.0.0/pyproject.toml` & `adafruit-circuitpython-displayio-ssd1306-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-displayio-ssd1306"
 description = "DisplayIO driver for SSD1306 monochrome displays"
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306"}
 keywords = [
     "adafruit",
```

