# Comparing `tmp/adafruit-circuitpython-httpserver-4.5.6.tar.gz` & `tmp/adafruit-circuitpython-httpserver-4.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-4.5.6.tar", last modified: Sat Feb 24 16:24:38 2024, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-4.5.7.tar", last modified: Mon Apr  1 15:19:35 2024, max compression
```

## Comparing `adafruit-circuitpython-httpserver-4.5.6.tar` & `adafruit-circuitpython-httpserver-4.5.7.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.269729 adafruit-circuitpython-httpserver-4.5.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.253729 adafruit-circuitpython-httpserver-4.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.257729 adafruit-circuitpython-httpserver-4.5.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.257729 adafruit-circuitpython-httpserver-4.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.257729 adafruit-circuitpython-httpserver-4.5.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-02-24 16:24:38.269729 adafruit-circuitpython-httpserver-4.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.269729 adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-02-24 16:24:38.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-24 16:24:38.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 16:24:38.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-24 16:24:38.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-24 16:24:38.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.261729 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    28371 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.261729 adafruit-circuitpython-httpserver-4.5.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.261729 adafruit-circuitpython-httpserver-4.5.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:24:38.269729 adafruit-circuitpython-httpserver-4.5.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/examples/directory_listing.tpl.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/examples/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_authentication_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_authentication_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_ethernet_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_form_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_handler_serves_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_multiple_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_simpletest_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_simpletest_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_start_and_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_start_and_poll_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_static_files_serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/examples/settings.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-02-24 16:24:32.000000 adafruit-circuitpython-httpserver-4.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-24 16:24:25.000000 adafruit-circuitpython-httpserver-4.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 16:24:38.269729 adafruit-circuitpython-httpserver-4.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.083020 adafruit-circuitpython-httpserver-4.5.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.087020 adafruit-circuitpython-httpserver-4.5.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.087020 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.087020 adafruit-circuitpython-httpserver-4.5.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.091020 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28371 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.095020 adafruit-circuitpython-httpserver-4.5.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.095020 adafruit-circuitpython-httpserver-4.5.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/examples/directory_listing.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/examples/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_ethernet_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_form_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_handler_serves_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_multiple_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_connectionmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_static_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-4.5.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-4.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/.gitignore` & `adafruit-circuitpython-httpserver-4.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-4.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/.pylintrc` & `adafruit-circuitpython-httpserver-4.5.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-4.5.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/LICENSE` & `adafruit-circuitpython-httpserver-4.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-4.5.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-4.5.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-4.5.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/PKG-INFO` & `adafruit-circuitpython-httpserver-4.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.5.6
+Version: 4.5.7
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-4.5.6/README.rst` & `adafruit-circuitpython-httpserver-4.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.5.6
+Version: 4.5.7
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 examples/httpserver_handler_serves_file.py
 examples/httpserver_mdns.py
 examples/httpserver_methods.py
 examples/httpserver_multiple_servers.py
 examples/httpserver_neopixel.py
 examples/httpserver_redirects.py
 examples/httpserver_simpletest_auto.py
+examples/httpserver_simpletest_connectionmanager.py
 examples/httpserver_simpletest_manual.py
 examples/httpserver_sse.py
 examples/httpserver_start_and_poll.py
 examples/httpserver_start_and_poll_asyncio.py
 examples/httpserver_static_files_serving.py
 examples/httpserver_templates.py
 examples/httpserver_url_parameters.py
```

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/__init__.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "4.5.6"
+__version__ = "4.5.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
 
 
 from .authentication import (
     Basic,
     Token,
     Bearer,
```

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/authentication.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/authentication.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/exceptions.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/headers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/interfaces.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/interfaces.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/mime_types.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/mime_types.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/request.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/response.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/response.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/route.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/route.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/server.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/status.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-4.5.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/docs/api.rst` & `adafruit-circuitpython-httpserver-4.5.7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/docs/conf.py` & `adafruit-circuitpython-httpserver-4.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/docs/examples.rst` & `adafruit-circuitpython-httpserver-4.5.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/docs/index.rst` & `adafruit-circuitpython-httpserver-4.5.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/directory_listing.tpl.html` & `adafruit-circuitpython-httpserver-4.5.7/examples/directory_listing.tpl.html`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_authentication_handlers.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_handlers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_authentication_server.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_chunked.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_chunked.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_cookies.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_cpu_information.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpu_information.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_cpython.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_ethernet_simpletest.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_ethernet_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_form_data.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_form_data.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_handler_serves_file.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_handler_serves_file.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_mdns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_methods.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_methods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_multiple_servers.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_multiple_servers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_neopixel.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_redirects.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_redirects.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_simpletest_auto.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_auto.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_simpletest_manual.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_manual.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_sse.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_sse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_start_and_poll.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_start_and_poll_asyncio.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll_asyncio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_static_files_serving.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_static_files_serving.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_templates.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_templates.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_url_parameters.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_url_parameters.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/examples/httpserver_websocket.py` & `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_websocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.6/pyproject.toml` & `adafruit-circuitpython-httpserver-4.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "4.5.6"
+version = "4.5.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```

