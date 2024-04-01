# Comparing `tmp/adafruit-circuitpython-tca8418-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-tca8418-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tca8418-1.0.8.tar", last modified: Mon Aug 28 14:38:58 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-tca8418-1.0.9.tar", last modified: Mon Sep 25 15:52:53 2023, max compression
```

## Comparing `adafruit-circuitpython-tca8418-1.0.8.tar` & `adafruit-circuitpython-tca8418-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.812270 adafruit-circuitpython-tca8418-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.804271 adafruit-circuitpython-tca8418-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.808271 adafruit-circuitpython-tca8418-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (999)      880 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.808271 adafruit-circuitpython-tca8418-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      303 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (999)      479 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (999)      482 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1654 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     1253 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    13078 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     6753 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (999)     1098 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.808271 adafruit-circuitpython-tca8418-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (999)    16814 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1108 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (999)     4194 2023-08-28 14:38:58.812270 adafruit-circuitpython-tca8418-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3419 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.808271 adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4194 2023-08-28 14:38:58.000000 adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1185 2023-08-28 14:38:58.000000 adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 14:38:58.000000 adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-28 14:38:58.000000 adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       17 2023-08-28 14:38:58.000000 adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)    12767 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/adafruit_tca8418.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.808271 adafruit-circuitpython-tca8418-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.808271 adafruit-circuitpython-tca8418-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)     4414 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (999)      105 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (999)      267 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (999)      183 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (999)     6094 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)      196 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (999)      183 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (999)     1114 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      183 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (999)      144 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 14:38:58.812270 adafruit-circuitpython-tca8418-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (999)     2651 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_3x4_OLED.py
--rw-r--r--   0 runner    (1001) docker     (999)     1738 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_3x4_noOLED.py
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_digitalio_blink.py
--rw-r--r--   0 runner    (1001) docker     (999)      719 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_digitalio_button.py
--rw-r--r--   0 runner    (1001) docker     (999)     1702 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_gpio_fifo.py
--rw-r--r--   0 runner    (1001) docker     (999)      734 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_gpiobutton.py
--rw-r--r--   0 runner    (1001) docker     (999)     1395 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_keypad.py
--rw-r--r--   0 runner    (1001) docker     (999)      594 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1236 2023-08-28 14:38:51.000000 adafruit-circuitpython-tca8418-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      272 2023-08-28 14:38:42.000000 adafruit-circuitpython-tca8418-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 14:38:58.812270 adafruit-circuitpython-tca8418-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.824149 adafruit-circuitpython-tca8418-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.812149 adafruit-circuitpython-tca8418-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.816149 adafruit-circuitpython-tca8418-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.816149 adafruit-circuitpython-tca8418-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.816149 adafruit-circuitpython-tca8418-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2023-09-25 15:52:53.824149 adafruit-circuitpython-tca8418-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.816149 adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2023-09-25 15:52:53.000000 adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-09-25 15:52:53.000000 adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 15:52:53.000000 adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-09-25 15:52:53.000000 adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-25 15:52:53.000000 adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/adafruit_tca8418.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.820149 adafruit-circuitpython-tca8418-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.820149 adafruit-circuitpython-tca8418-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 15:52:53.820149 adafruit-circuitpython-tca8418-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_3x4_OLED.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_3x4_noOLED.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_digitalio_blink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_digitalio_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_gpio_fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_gpiobutton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_keypad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-09-25 15:52:44.000000 adafruit-circuitpython-tca8418-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-09-25 15:52:33.000000 adafruit-circuitpython-tca8418-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 15:52:53.824149 adafruit-circuitpython-tca8418-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-tca8418-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tca8418-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/.gitignore` & `adafruit-circuitpython-tca8418-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tca8418-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/.pylintrc` & `adafruit-circuitpython-tca8418-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tca8418-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/LICENSE` & `adafruit-circuitpython-tca8418-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tca8418-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tca8418-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tca8418-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/PKG-INFO` & `adafruit-circuitpython-tca8418-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tca8418
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython / Python library for TCA8418 Keyboard Multiplexor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TCA8418.git
 Keywords: adafruit,blinka,circuitpython,micropython,tca8418,python,keyboard,keeb
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-busdevice
+Requires-Dist: adafruit-circuitpython-register
+Provides-Extra: optional
+Requires-Dist: adafruit-circuitpython-debug-i2c; extra == "optional"
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-tca8418/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/tca8418/en/latest/
```

### Comparing `adafruit-circuitpython-tca8418-1.0.8/README.rst` & `adafruit-circuitpython-tca8418-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/PKG-INFO` & `adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tca8418
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython / Python library for TCA8418 Keyboard Multiplexor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TCA8418.git
 Keywords: adafruit,blinka,circuitpython,micropython,tca8418,python,keyboard,keeb
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-busdevice
+Requires-Dist: adafruit-circuitpython-register
+Provides-Extra: optional
+Requires-Dist: adafruit-circuitpython-debug-i2c; extra == "optional"
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-tca8418/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/tca8418/en/latest/
```

### Comparing `adafruit-circuitpython-tca8418-1.0.8/adafruit_circuitpython_tca8418.egg-info/SOURCES.txt` & `adafruit-circuitpython-tca8418-1.0.9/adafruit_circuitpython_tca8418.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/adafruit_tca8418.py` & `adafruit-circuitpython-tca8418-1.0.9/adafruit_tca8418.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tca8418-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/docs/conf.py` & `adafruit-circuitpython-tca8418-1.0.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,27 +108,18 @@
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import sphinx_rtd_theme
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme = "sphinx_rtd_theme"
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to use as a favicon of
```

### Comparing `adafruit-circuitpython-tca8418-1.0.8/docs/index.rst` & `adafruit-circuitpython-tca8418-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_3x4_OLED.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_3x4_OLED.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_3x4_noOLED.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_3x4_noOLED.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_digitalio_blink.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_digitalio_blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_digitalio_button.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_digitalio_button.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_gpio_fifo.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_gpio_fifo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_gpiobutton.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_gpiobutton.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_keypad.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_keypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/examples/tca8418_simpletest.py` & `adafruit-circuitpython-tca8418-1.0.9/examples/tca8418_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca8418-1.0.8/pyproject.toml` & `adafruit-circuitpython-tca8418-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-tca8418"
 description = "CircuitPython / Python library for TCA8418 Keyboard Multiplexor"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TCA8418.git"}
 keywords = [
     "adafruit",
```

