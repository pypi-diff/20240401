# Comparing `tmp/openbb_government_us-1.1.3.tar.gz` & `tmp/openbb_government_us-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_government_us-1.1.3.tar", max compression
+gzip compressed data, was "openbb_government_us-1.1.4.tar", max compression
```

## Comparing `openbb_government_us-1.1.3.tar` & `openbb_government_us-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      445 2024-01-17 14:26:16.764486 openbb_government_us-1.1.3/README.md
--rw-r--r--   0        0        0      988 2024-01-17 14:26:16.764618 openbb_government_us-1.1.3/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-01-17 14:26:16.764705 openbb_government_us-1.1.3/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-02-23 17:14:57.465228 openbb_government_us-1.1.3/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5221 2024-03-11 10:41:33.407719 openbb_government_us-1.1.3/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.764907 openbb_government_us-1.1.3/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-01-17 14:26:16.764981 openbb_government_us-1.1.3/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0      522 2024-03-11 19:59:14.507347 openbb_government_us-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 openbb_government_us-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      445 2024-02-29 11:03:36.873075 openbb_government_us-1.1.4/README.md
+-rw-r--r--   0        0        0      988 2024-03-21 17:38:35.647065 openbb_government_us-1.1.4/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-02-29 11:03:36.873377 openbb_government_us-1.1.4/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-03-13 16:36:51.740330 openbb_government_us-1.1.4/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5221 2024-03-21 17:38:35.647219 openbb_government_us-1.1.4/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.873541 openbb_government_us-1.1.4/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-03-13 16:36:51.740949 openbb_government_us-1.1.4/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0      522 2024-04-01 14:20:27.742856 openbb_government_us-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 openbb_government_us-1.1.4/PKG-INFO
```

### Comparing `openbb_government_us-1.1.3/openbb_government_us/__init__.py` & `openbb_government_us-1.1.4/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.1.3/openbb_government_us/models/treasury_auctions.py` & `openbb_government_us-1.1.4/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.1.3/openbb_government_us/models/treasury_prices.py` & `openbb_government_us-1.1.4/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.1.3/pyproject.toml` & `openbb_government_us-1.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "openbb-government-us"
-version = "1.1.3"
+version = "1.1.4"
 description = "US Government Data Extension for OpenBB"
 authors = ["OpenBB <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_government_us" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 random-user-agent = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
```

### Comparing `openbb_government_us-1.1.3/PKG-INFO` & `openbb_government_us-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-government-us
-Version: 1.1.3
+Version: 1.1.4
 Summary: US Government Data Extension for OpenBB
 Author: OpenBB
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
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Government US Provider
 
 This extension integrates the [US Government](https://data.gov) data provider into the OpenBB Platform.
```

