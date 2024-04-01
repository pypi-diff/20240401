# Comparing `tmp/adafruit-circuitpython-pybadger-3.8.1.tar.gz` & `tmp/adafruit-circuitpython-pybadger-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pybadger-3.8.1.tar", last modified: Sat Dec  9 17:46:38 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-pybadger-4.0.0.tar", last modified: Mon Apr  1 14:52:24 2024, max compression
```

## Comparing `adafruit-circuitpython-pybadger-3.8.1.tar` & `adafruit-circuitpython-pybadger-4.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.998659 adafruit-circuitpython-pybadger-3.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.986659 adafruit-circuitpython-pybadger-3.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.986659 adafruit-circuitpython-pybadger-3.8.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.990659 adafruit-circuitpython-pybadger-3.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.990659 adafruit-circuitpython-pybadger-3.8.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17967 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-12-09 17:46:37.998659 adafruit-circuitpython-pybadger-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.998659 adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-12-09 17:46:37.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-12-09 17:46:37.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:46:37.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-09 17:46:37.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-09 17:46:37.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.990659 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/clue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/cpb_gizmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/magtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pewpewm4.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pybadge.py
--rw-r--r--   0 runner    (1001) docker     (127)    31867 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pybadger_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pygamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pyportal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.994660 adafruit-circuitpython-pybadger-3.8.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.994660 adafruit-circuitpython-pybadger-3.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.994660 adafruit-circuitpython-pybadger-3.8.1/docs/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/mocks/keypad.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:46:37.998659 adafruit-circuitpython-pybadger-3.8.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)    61494 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (127)   115256 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_CLUE.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_CLUE.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)    38966 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_MagTag.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_MagTag.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_PewPewM4.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_PewPewM4.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)    42102 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_PyPortal.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_PyPortal.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)    38470 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/QR_Blinka_CircuitPythonOrg.bmp
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/examples/QR_Blinka_CircuitPythonOrg.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_button_debouncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_clue_custom_badge.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_clue_custom_image_badge.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_custom_badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_pewpewm4_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_pygamer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_pyportal_touchscreen.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-12-09 17:46:31.000000 adafruit-circuitpython-pybadger-3.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-09 17:46:25.000000 adafruit-circuitpython-pybadger-3.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:46:37.998659 adafruit-circuitpython-pybadger-3.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.770333 adafruit-circuitpython-pybadger-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.758333 adafruit-circuitpython-pybadger-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.762333 adafruit-circuitpython-pybadger-4.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.762333 adafruit-circuitpython-pybadger-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.762333 adafruit-circuitpython-pybadger-4.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17967 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-01 14:52:24.770333 adafruit-circuitpython-pybadger-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.770333 adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-01 14:52:24.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-01 14:52:24.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:52:24.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-01 14:52:24.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 14:52:24.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.766332 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/clue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/cpb_gizmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/magtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pewpewm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pybadge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32080 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pybadger_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pygamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pyportal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.766332 adafruit-circuitpython-pybadger-4.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.766332 adafruit-circuitpython-pybadger-4.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.766332 adafruit-circuitpython-pybadger-4.0.0/docs/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/mocks/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:52:24.770333 adafruit-circuitpython-pybadger-4.0.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61494 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)   115256 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_CLUE.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_CLUE.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)    38966 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_MagTag.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_MagTag.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_PewPewM4.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_PewPewM4.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)    42102 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_PyPortal.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_PyPortal.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)    38470 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/QR_Blinka_CircuitPythonOrg.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/examples/QR_Blinka_CircuitPythonOrg.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_button_debouncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_clue_custom_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_clue_custom_image_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_custom_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_pewpewm4_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_pygamer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_pyportal_touchscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-01 14:52:22.000000 adafruit-circuitpython-pybadger-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 14:52:16.000000 adafruit-circuitpython-pybadger-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:52:24.770333 adafruit-circuitpython-pybadger-4.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pybadger-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/.gitignore` & `adafruit-circuitpython-pybadger-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/.pre-commit-config.yaml` & `adafruit-circuitpython-pybadger-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/.pylintrc` & `adafruit-circuitpython-pybadger-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pybadger-4.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/LICENSE` & `adafruit-circuitpython-pybadger-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pybadger-4.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-pybadger-4.0.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/LICENSES/MIT.txt` & `adafruit-circuitpython-pybadger-4.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pybadger-4.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/PKG-INFO` & `adafruit-circuitpython-pybadger-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pybadger
-Version: 3.8.1
+Version: 4.0.0
 Summary: Badge-focused CircuitPython helper library for PyBadge, PyBadge LC, PyGamer and CLUE
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pybadge,pygamer,clue,display,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/README.rst` & `adafruit-circuitpython-pybadger-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/PKG-INFO` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pybadger
-Version: 3.8.1
+Version: 4.0.0
 Summary: Badge-focused CircuitPython helper library for PyBadge, PyBadge LC, PyGamer and CLUE
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pybadge,pygamer,clue,display,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/__init__.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/clue.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/clue.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import board
 import audiopwmio
 import keypad
 import adafruit_lsm6ds.lsm6ds33
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "a b")
 
 
 class Clue(PyBadgerBase):
     """Class that represents a single CLUE."""
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/cpb_gizmo.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/cpb_gizmo.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import keypad
 from adafruit_gizmo import tft_gizmo
 import adafruit_lis3dh
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "a b")
 
 
 class CPB_Gizmo(PyBadgerBase):
     """Class that represents a single Circuit Playground Bluefruit with TFT Gizmo."""
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/magtag.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/magtag.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from collections import namedtuple
 import board
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase
 
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "a b c d")
 
 
 class MagTag(PyBadgerBase):
     """Class that represents a single Mag Tag."""
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pewpewm4.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pewpewm4.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from collections import namedtuple
 import board
 import audioio
 import keypad
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", ("o", "x", "z", "right", "down", "up", "left"))
 
 
 class PewPewM4(PyBadgerBase):
     """Class that represents a single Pew Pew M4."""
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pybadge.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pybadge.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import audioio
 import keypad
 import adafruit_lis3dh
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "b a start select right down up left")
 
 
 class PyBadge(PyBadgerBase):
     """Class that represents a single PyBadge, PyBadge LC, or EdgeBadge."""
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pybadger_base.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pybadger_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     from adafruit_bitmap_font.bdf import BDF  # pylint: disable=ungrouped-imports
     from adafruit_bitmap_font.pcf import PCF  # pylint: disable=ungrouped-imports
     from fontio import BuiltinFont
     from keypad import Keys, ShiftRegisterKeys
     from neopixel import NeoPixel
 
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 
 def load_font(fontname: str, text: str) -> Union[BDF, PCF]:
     """Load a font and glyphs in the text string
 
     :param str fontname: The full path to the font file.
@@ -161,15 +161,15 @@
 
     def _create_badge_background(self) -> None:
         self._created_background = True
 
         if self._background_group is None:
             self._background_group = displayio.Group()
 
-        self.show(self._background_group)
+        self.root_group = self._background_group
 
         if self._background_image_filename:
             file_handle = open(  # pylint: disable=consider-using-with
                 self._background_image_filename, "rb"
             )
             on_disk_bitmap = displayio.OnDiskBitmap(file_handle)
             background_image = displayio.TileGrid(
@@ -355,15 +355,15 @@
     def show_custom_badge(self) -> None:
         """Call ``pybadger.show_custom_badge()`` to display the custom badge elements. If
         ``show_custom_badge()`` is not called, the custom badge elements will not be displayed.
         """
         if not self._created_background:
             self._create_badge_background()
 
-        self.show(self._background_group)
+        self.root_group = self._background_group
 
     # pylint: disable=too-many-arguments
     def _create_label_group(
         self,
         text: str,
         font: Union[BuiltinFont, BDF, PCF],
         scale: int,
@@ -557,15 +557,15 @@
         on_disk_bitmap = displayio.OnDiskBitmap(image_file)
         face_image = displayio.TileGrid(
             on_disk_bitmap, pixel_shader=on_disk_bitmap.pixel_shader
         )
         business_card_splash.append(face_image)
         for group in business_card_label_groups:
             business_card_splash.append(group)
-        self.show(business_card_splash)
+        self.root_group = business_card_splash
 
     # pylint: disable=too-many-locals
     def show_badge(
         self,
         *,
         background_color: Tuple[int, int, int] = RED,
         foreground_color: Tuple[int, int, int] = WHITE,
@@ -642,27 +642,33 @@
             self._badge_background(
                 background_color=background_color, rectangle_color=foreground_color
             )
         )
         group.append(hello_group)
         group.append(my_name_is_group)
         group.append(name_group)
-        self.show(group)
+        self.root_group = group
 
-    def show(self, group) -> None:
+    @property
+    def root_group(self):
+        """The currently showing Group"""
+        return self.display.root_group
+
+    @root_group.setter
+    def root_group(self, group):
         """Show the given group, refreshing the screen immediately"""
         self.activity()
         self.display.auto_refresh = False
         self.display.root_group = group
         self.display.refresh()
         self.display.auto_refresh = True
 
     def show_terminal(self) -> None:
         """Revert to terminalio screen."""
-        self.show(None)
+        self.root_group = displayio.CIRCUITPYTHON_TERMINAL
 
     @staticmethod
     def bitmap_qr(matrix: adafruit_miniqr.QRBitMatrix) -> displayio.Bitmap:
         """The QR code bitmap."""
         border_pixels = 2
         bitmap = displayio.Bitmap(
             matrix.width + 2 * border_pixels, matrix.height + 2 * border_pixels, 2
@@ -706,15 +712,15 @@
             ((self.display.height / qr_code_scale) - qr_bitmap.height) / 2
         )
         qr_img = displayio.TileGrid(
             qr_bitmap, pixel_shader=palette, x=qr_position_x, y=qr_position_y
         )
         qr_code = displayio.Group(scale=qr_code_scale)
         qr_code.append(qr_img)
-        self.show(qr_code)
+        self.root_group = qr_code
 
     @staticmethod
     def _sine_sample(length: int) -> Generator[int, None, None]:
         tone_volume = (2**15) - 1
         shift = 2**15
         for i in range(length):
             yield int(tone_volume * math.sin(2 * math.pi * (i / length)) + shift)
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pygamer.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pygamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "b a start select right down up left")
 
 
 class PyGamer(PyBadgerBase):
     """Class that represents a single PyGamer."""
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/adafruit_pybadger/pyportal.py` & `adafruit-circuitpython-pybadger-4.0.0/adafruit_pybadger/pyportal.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 import board
 import analogio
 import audioio
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase
 
-__version__ = "3.8.1"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 
 class PyPortal(PyBadgerBase):
     """Class that represents a single PyPortal."""
 
     _audio_out = audioio.AudioOut
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/docs/_static/favicon.ico` & `adafruit-circuitpython-pybadger-4.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/docs/api.rst` & `adafruit-circuitpython-pybadger-4.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/docs/conf.py` & `adafruit-circuitpython-pybadger-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/docs/index.rst` & `adafruit-circuitpython-pybadger-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/docs/mocks/keypad.py` & `adafruit-circuitpython-pybadger-4.0.0/docs/mocks/keypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/Blinka.bmp` & `adafruit-circuitpython-pybadger-4.0.0/examples/Blinka.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_CLUE.bmp` & `adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_CLUE.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_MagTag.bmp` & `adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_MagTag.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_PewPewM4.bmp` & `adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_PewPewM4.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/Blinka_PyPortal.bmp` & `adafruit-circuitpython-pybadger-4.0.0/examples/Blinka_PyPortal.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/QR_Blinka_CircuitPythonOrg.bmp` & `adafruit-circuitpython-pybadger-4.0.0/examples/QR_Blinka_CircuitPythonOrg.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_button_debouncing.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_button_debouncing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_clue_custom_badge.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_clue_custom_badge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_clue_custom_image_badge.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_clue_custom_image_badge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_custom_badge.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_custom_badge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_magtag_simpletest.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_pewpewm4_simpletest.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_pewpewm4_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_pygamer_asyncio.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_pygamer_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 image_name="Blinka.bmp",
                 name_string="Jeff Epler",
                 name_scale=2,
                 email_string_one="jeff@adafruit.com",
                 email_string_two=pronoun,
             )
         elif pybadger.button.b:
-            pybadger.show(qr_gp)
+            pybadger.root_group = qr_gp
         elif pybadger.button.start:
             pybadger.show_custom_badge()
         elif pybadger.button.select:
             pybadger.activity()
         else:
             pybadger.auto_dim_display(
                 delay=0.5
```

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_pyportal_touchscreen.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_pyportal_touchscreen.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/examples/pybadger_simpletest.py` & `adafruit-circuitpython-pybadger-4.0.0/examples/pybadger_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.8.1/pyproject.toml` & `adafruit-circuitpython-pybadger-4.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pybadger"
 description = "Badge-focused CircuitPython helper library for PyBadge, PyBadge LC, PyGamer and CLUE"
-version = "3.8.1"
+version = "4.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_REPLACE"}
 keywords = [
     "adafruit",
```

