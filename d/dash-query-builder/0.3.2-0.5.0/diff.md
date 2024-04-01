# Comparing `tmp/dash-query-builder-0.3.2.tar.gz` & `tmp/dash_query_builder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-query-builder-0.3.2.tar", max compression
+gzip compressed data, was "dash_query_builder-0.5.0.tar", max compression
```

## Comparing `dash-query-builder-0.3.2.tar` & `dash_query_builder-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,10 @@
--rw-r--r--   0        0        0        0 2022-02-25 17:09:44.690159 dash-query-builder-0.3.2/LICENSE
--rw-r--r--   0        0        0     4540 2022-02-25 17:12:34.596859 dash-query-builder-0.3.2/dash_query_builder/DashQueryBuilder.py
--rw-r--r--   0        0        0     2662 2022-02-25 17:09:44.690159 dash-query-builder-0.3.2/dash_query_builder/__init__.py
--rw-r--r--   0        0        0       84 2022-02-25 17:12:34.596859 dash-query-builder-0.3.2/dash_query_builder/_imports_.py
--rw-r--r--   0        0        0  4001679 2022-02-25 17:09:44.706159 dash-query-builder-0.3.2/dash_query_builder/async-antd.min.js
--rw-r--r--   0        0        0      246 2022-02-25 17:09:44.706159 dash-query-builder-0.3.2/dash_query_builder/async-antd.min.js.LICENSE.txt
--rw-r--r--   0        0        0  8059445 2022-02-25 17:09:44.738160 dash-query-builder-0.3.2/dash_query_builder/async-antd.min.js.map
--rw-r--r--   0        0        0     3342 2022-02-25 17:09:44.738160 dash-query-builder-0.3.2/dash_query_builder/async-basic.min.js
--rw-r--r--   0        0        0     1478 2022-02-25 17:09:44.738160 dash-query-builder-0.3.2/dash_query_builder/async-basic.min.js.map
--rw-r--r--   0        0        0  1883336 2022-02-25 17:09:44.750160 dash-query-builder-0.3.2/dash_query_builder/async-bootstrap.min.js
--rw-r--r--   0        0        0      219 2022-02-25 17:09:44.750160 dash-query-builder-0.3.2/dash_query_builder/async-bootstrap.min.js.LICENSE.txt
--rw-r--r--   0        0        0  2730206 2022-02-25 17:09:44.762160 dash-query-builder-0.3.2/dash_query_builder/async-bootstrap.min.js.map
--rw-r--r--   0        0        0   342264 2022-02-25 17:09:44.766160 dash-query-builder-0.3.2/dash_query_builder/async-material.min.js
--rw-r--r--   0        0        0      165 2022-02-25 17:09:44.766160 dash-query-builder-0.3.2/dash_query_builder/async-material.min.js.LICENSE.txt
--rw-r--r--   0        0        0  1590128 2022-02-25 17:09:44.770160 dash-query-builder-0.3.2/dash_query_builder/async-material.min.js.map
--rw-r--r--   0        0        0   426528 2022-02-25 17:09:44.774160 dash-query-builder-0.3.2/dash_query_builder/async-mui.min.js
--rw-r--r--   0        0        0      464 2022-02-25 17:09:44.774160 dash-query-builder-0.3.2/dash_query_builder/async-mui.min.js.LICENSE.txt
--rw-r--r--   0        0        0  2025437 2022-02-25 17:09:44.782160 dash-query-builder-0.3.2/dash_query_builder/async-mui.min.js.map
--rw-r--r--   0        0        0   816710 2022-02-25 17:12:32.780779 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.min.js
--rw-r--r--   0        0        0      668 2022-02-25 17:09:44.786160 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.min.js.LICENSE.txt
--rw-r--r--   0        0        0  3101029 2022-02-25 17:12:32.720776 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.min.js.map
--rw-r--r--   0        0        0    19881 2022-02-25 17:09:44.798160 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.shared.js
--rw-r--r--   0        0        0     9854 2022-02-25 17:09:44.798160 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.shared.js.map
--rw-r--r--   0        0        0     3889 2022-02-25 17:09:44.798160 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.shared.min.js
--rw-r--r--   0        0        0    12678 2022-02-25 17:09:44.798160 dash-query-builder-0.3.2/dash_query_builder/dash_query_builder.shared.min.js.map
--rw-r--r--   0        0        0     5559 2022-02-25 17:12:34.596859 dash-query-builder-0.3.2/dash_query_builder/metadata.json
--rw-r--r--   0        0        0     3080 2022-02-25 17:12:34.164840 dash-query-builder-0.3.2/dash_query_builder/package-info.json
--rw-r--r--   0        0        0      836 2022-02-25 17:09:44.922162 dash-query-builder-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      658 2022-02-25 17:12:37.758068 dash-query-builder-0.3.2/setup.py
--rw-r--r--   0        0        0      728 2022-02-25 17:12:37.758358 dash-query-builder-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1053 2024-04-01 16:21:49.619114 dash_query_builder-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2687 2024-04-01 16:21:49.883113 dash_query_builder-0.5.0/dash_query_builder/__init__.py
+-rw-r--r--   0        0        0       84 2024-04-01 16:21:49.879113 dash_query_builder-0.5.0/dash_query_builder/_imports_.py
+-rw-r--r--   0        0        0     1880 2024-04-01 16:21:50.611109 dash_query_builder-0.5.0/dash_query_builder/where_parser/__init__.py
+-rw-r--r--   0        0        0    16126 2024-04-01 16:21:50.623109 dash_query_builder-0.5.0/dash_query_builder/where_parser/actions.py
+-rw-r--r--   0        0        0     6389 2024-04-01 16:21:50.659109 dash_query_builder-0.5.0/dash_query_builder/where_parser/constants.py
+-rw-r--r--   0        0        0     1659 2024-04-01 16:21:50.671109 dash_query_builder-0.5.0/dash_query_builder/where_parser/operators.py
+-rw-r--r--   0        0        0     3141 2024-04-01 16:21:50.703109 dash_query_builder-0.5.0/dash_query_builder/where_parser/parser_.py
+-rw-r--r--   0        0        0     1150 2024-04-01 16:21:49.619114 dash_query_builder-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 dash_query_builder-0.5.0/PKG-INFO
```

### Comparing `dash-query-builder-0.3.2/dash_query_builder/__init__.py` & `dash_query_builder-0.5.0/dash_query_builder/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 from __future__ import print_function as _
 
+import json
 import os as _os
 import sys as _sys
-import json
 
 import dash as _dash
 
-# noinspection PyUnresolvedReferences
-from ._imports_ import *
+# noinspection PyUnresolvedReferences'
+from ._imports_ import *  # noqa
 from ._imports_ import __all__
+from .where_parser import WhereParser  # noqa
 
 if not hasattr(_dash, "__plotly_dash") and not hasattr(_dash, "development"):
     print(
         "Dash was not successfully imported. "
         "Make sure you don't have a file "
         'named \n"dash.py" in your current directory.',
         file=_sys.stderr,
     )
     _sys.exit(1)
 
 _basepath = _os.path.dirname(__file__)
-_filepath = _os.path.abspath(_os.path.join(_basepath, "package-info.json"))
+_filepath = _os.path.abspath(_os.path.join(_basepath, "package.json"))
 with open(_filepath) as f:
     package = json.load(f)
 
 package_name = package["name"].replace(" ", "_").replace("-", "_")
 __version__ = package["version"]
 
 _current_path = _os.path.dirname(_os.path.abspath(__file__))
 
 _this_module = _sys.modules[__name__]
 
 dev_mode = False
 mode_suffix = "dev" if dev_mode else "min"
-async_resources = ["material", "mui", "antd", "bootstrap", "basic"]
+async_resources = ["mui", "antd", "bootstrap", "basic"]
 _shared = "shared." + mode_suffix
 
-shared_resources = [mode_suffix, _shared]
+shared_resources = [mode_suffix]
 
 _js_dist = []
 
 _js_dist.extend(
     [
         {
-            "relative_package_path": "async-{0}.{1}.js".format(
+            "relative_package_path": "async-{}.{}.js".format(
                 async_resource, mode_suffix
             ),
             "external_url": ("https://unpkg.com/{0}@{2}" "/{1}/async-{3}.js").format(
                 package_name, __name__, __version__, async_resource
             ),
             "namespace": package_name,
             "async": True,
@@ -56,15 +57,15 @@
     ]
 )
 
 # TODO: Figure out if unpkg link works
 _js_dist.extend(
     [
         {
-            "relative_package_path": "async-{0}.{1}.js.map".format(
+            "relative_package_path": "async-{}.{}.js.map".format(
                 async_resource, mode_suffix
             ),
             "external_url": (
                 "https://unpkg.com/{0}@{2}" "/{1}/async-{3}.js.map"
             ).format(package_name, __name__, __version__, async_resource),
             "namespace": package_name,
             "dynamic": True,
```

### Comparing `dash-query-builder-0.3.2/pyproject.toml` & `dash_query_builder-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 [tool.poetry]
 name = "dash-query-builder"
-version = "0.3.2"
+version = "0.5.0"
 description = "Dash Component based on react-awesome-query-builder"
 authors = ["Tyler Baur <baur.tyler@protonmail.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Dash",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "License :: OSI Approved :: MIT License"
 ]
 
 [tool.poetry.urls]
-"Bug Tracker"="https://github.com/baurt/dash_query_builder/issues"
-"Homepage"="https://github.com/baurt/dash_query_builder"
+"Bug Tracker"="https://github.com/baurt/dash-query-builder/issues"
+"Homepage"="https://github.com/baurt/dash-query-builder"
 
 
+[tool.ruff]
+ignore = []
+line-length = 88
+select = [
+  'E',
+  'F',
+  'W',
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dash="^2.0.0"
+pyparsing = "^3.0.9"
+rich = "^13.3.1"
+shortuuid = "^1.0.11"
 
-
-[tool.poetry.dev-dependencies]
-black = "^21.6b0"
-flake8 = "^3.9.2"
+[tool.poetry.group.dev.dependencies]
 dash = {version = "^2.0.0", extras = ["dev","testing"]}
-
+mypy = "^1.0.0"
+pre-commit = "^3.0.4"
+shed = "^0.10.9"
+ruff = "^0.0.246"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

