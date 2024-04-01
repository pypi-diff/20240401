# Comparing `tmp/openbb_tradingeconomics-1.1.3.tar.gz` & `tmp/openbb_tradingeconomics-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradingeconomics-1.1.3.tar", max compression
+gzip compressed data, was "openbb_tradingeconomics-1.1.4.tar", max compression
```

## Comparing `openbb_tradingeconomics-1.1.3.tar` & `openbb_tradingeconomics-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      469 2024-01-17 14:26:16.878650 openbb_tradingeconomics-1.1.3/README.md
--rw-r--r--   0        0        0      440 2024-01-26 17:52:27.971180 openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4529 2024-02-28 12:51:01.931304 openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4567 2024-02-26 21:17:23.742232 openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3636 2024-02-23 17:14:57.546944 openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0      512 2024-03-11 20:00:41.545164 openbb_tradingeconomics-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      469 2024-02-29 11:03:36.974304 openbb_tradingeconomics-1.1.4/README.md
+-rw-r--r--   0        0        0      440 2024-03-21 17:38:35.661271 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     4529 2024-03-13 16:36:51.898559 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4567 2024-03-13 16:36:51.898679 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3636 2024-03-13 16:36:51.898787 openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0      512 2024-04-01 14:21:45.210039 openbb_tradingeconomics-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.1.4/PKG-INFO
```

### Comparing `openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/utils/countries.py` & `openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.1.3/openbb_tradingeconomics/utils/url_generator.py` & `openbb_tradingeconomics-1.1.4/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.1.3/pyproject.toml` & `openbb_tradingeconomics-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "openbb-tradingeconomics"
-version = "1.1.3"
+version = "1.1.4"
 description = "Trading Economics extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_tradingeconomics" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tradingeconomics = "openbb_tradingeconomics:tradingeconomics_provider"
```

### Comparing `openbb_tradingeconomics-1.1.3/PKG-INFO` & `openbb_tradingeconomics-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-tradingeconomics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Trading Economics extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Trading Economics Provider
 
 This extension integrates the [Trading Economics](https://docs.tradingeconomics.com/) data provider into the OpenBB SDK.
 
 ## Installation
```

