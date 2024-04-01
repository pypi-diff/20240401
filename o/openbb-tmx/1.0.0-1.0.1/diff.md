# Comparing `tmp/openbb_tmx-1.0.0.tar.gz` & `tmp/openbb_tmx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tmx-1.0.0.tar", max compression
+gzip compressed data, was "openbb_tmx-1.0.1.tar", max compression
```

## Comparing `openbb_tmx-1.0.0.tar` & `openbb_tmx-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2369 2024-02-23 17:14:57.473845 openbb_tmx-1.0.0/README.md
--rw-r--r--   0        0        0     3319 2024-03-11 10:41:33.417548 openbb_tmx-1.0.0/openbb_tmx/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 17:14:57.474266 openbb_tmx-1.0.0/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-02-23 17:14:57.474373 openbb_tmx-1.0.0/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-02-23 17:14:57.474439 openbb_tmx-1.0.0/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5170 2024-02-23 17:14:57.474513 openbb_tmx-1.0.0/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-02-23 17:14:57.474607 openbb_tmx-1.0.0/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4373 2024-02-23 17:14:57.474686 openbb_tmx-1.0.0/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8830 2024-03-11 19:09:39.080054 openbb_tmx-1.0.0/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5446 2024-02-23 17:14:57.474862 openbb_tmx-1.0.0/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12441 2024-02-23 17:14:57.474935 openbb_tmx-1.0.0/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-02-23 17:14:57.476031 openbb_tmx-1.0.0/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-02-23 17:14:57.476130 openbb_tmx-1.0.0/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-02-23 17:14:57.476261 openbb_tmx-1.0.0/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-02-28 09:43:45.472471 openbb_tmx-1.0.0/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-02-23 17:14:57.476463 openbb_tmx-1.0.0/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-02-23 17:14:57.476536 openbb_tmx-1.0.0/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4439 2024-02-23 17:14:57.476616 openbb_tmx-1.0.0/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-02-23 17:14:57.476707 openbb_tmx-1.0.0/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3055 2024-02-23 17:14:57.476781 openbb_tmx-1.0.0/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-02-23 17:14:57.476870 openbb_tmx-1.0.0/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10268 2024-02-23 17:14:57.476943 openbb_tmx-1.0.0/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6055 2024-02-23 17:14:57.477019 openbb_tmx-1.0.0/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-02-23 17:14:57.477104 openbb_tmx-1.0.0/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5688 2024-02-23 17:14:57.477177 openbb_tmx-1.0.0/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-02-23 17:14:57.477244 openbb_tmx-1.0.0/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-02-23 17:14:57.477270 openbb_tmx-1.0.0/openbb_tmx/py.typed
--rw-r--r--   0        0        0        0 2024-02-23 17:14:57.477354 openbb_tmx-1.0.0/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-02-23 17:14:57.477458 openbb_tmx-1.0.0/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38297 2024-02-23 17:14:57.477577 openbb_tmx-1.0.0/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0      636 2024-03-11 20:00:20.577643 openbb_tmx-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 openbb_tmx-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2369 2024-03-13 16:36:51.803442 openbb_tmx-1.0.1/README.md
+-rw-r--r--   0        0        0     3319 2024-03-21 17:38:35.656878 openbb_tmx-1.0.1/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.804121 openbb_tmx-1.0.1/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-03-21 17:38:35.657064 openbb_tmx-1.0.1/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-03-21 17:38:35.657217 openbb_tmx-1.0.1/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5170 2024-03-21 17:38:35.657345 openbb_tmx-1.0.1/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-03-21 17:38:35.657496 openbb_tmx-1.0.1/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4373 2024-03-21 17:38:35.657642 openbb_tmx-1.0.1/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8830 2024-03-21 17:38:35.657823 openbb_tmx-1.0.1/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5446 2024-03-21 17:38:35.658001 openbb_tmx-1.0.1/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12441 2024-03-21 17:38:35.658160 openbb_tmx-1.0.1/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-03-21 17:38:35.658331 openbb_tmx-1.0.1/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-03-21 17:38:35.658468 openbb_tmx-1.0.1/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-03-21 17:38:35.658625 openbb_tmx-1.0.1/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-03-21 17:38:35.658764 openbb_tmx-1.0.1/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-03-21 17:38:35.658932 openbb_tmx-1.0.1/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-03-21 17:38:35.659035 openbb_tmx-1.0.1/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4439 2024-03-21 17:38:35.659165 openbb_tmx-1.0.1/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-03-21 17:38:35.659289 openbb_tmx-1.0.1/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3055 2024-03-21 17:38:35.659409 openbb_tmx-1.0.1/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-03-21 17:38:35.659521 openbb_tmx-1.0.1/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10268 2024-03-21 17:38:35.659626 openbb_tmx-1.0.1/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6055 2024-03-21 17:38:35.659773 openbb_tmx-1.0.1/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-03-21 17:38:35.659904 openbb_tmx-1.0.1/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5688 2024-03-21 17:38:35.660009 openbb_tmx-1.0.1/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5133 2024-03-21 17:38:35.660112 openbb_tmx-1.0.1/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.806449 openbb_tmx-1.0.1/openbb_tmx/py.typed
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.806502 openbb_tmx-1.0.1/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-03-13 16:36:51.806596 openbb_tmx-1.0.1/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38297 2024-03-21 17:38:35.660407 openbb_tmx-1.0.1/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0      636 2024-04-01 14:21:26.089284 openbb_tmx-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 openbb_tmx-1.0.1/PKG-INFO
```

### Comparing `openbb_tmx-1.0.0/README.md` & `openbb_tmx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/__init__.py` & `openbb_tmx-1.0.1/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/available_indices.py` & `openbb_tmx-1.0.1/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/bond_prices.py` & `openbb_tmx-1.0.1/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/calendar_earnings.py` & `openbb_tmx-1.0.1/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/company_filings.py` & `openbb_tmx-1.0.1/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/company_news.py` & `openbb_tmx-1.0.1/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/equity_historical.py` & `openbb_tmx-1.0.1/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/equity_profile.py` & `openbb_tmx-1.0.1/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/equity_quote.py` & `openbb_tmx-1.0.1/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/equity_search.py` & `openbb_tmx-1.0.1/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/etf_countries.py` & `openbb_tmx-1.0.1/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/etf_holdings.py` & `openbb_tmx-1.0.1/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/etf_info.py` & `openbb_tmx-1.0.1/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/etf_search.py` & `openbb_tmx-1.0.1/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/etf_sectors.py` & `openbb_tmx-1.0.1/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/gainers.py` & `openbb_tmx-1.0.1/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/historical_dividends.py` & `openbb_tmx-1.0.1/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/index_constituents.py` & `openbb_tmx-1.0.1/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/index_sectors.py` & `openbb_tmx-1.0.1/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/index_snapshots.py` & `openbb_tmx-1.0.1/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/insider_trading.py` & `openbb_tmx-1.0.1/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/options_chains.py` & `openbb_tmx-1.0.1/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/price_target_consensus.py` & `openbb_tmx-1.0.1/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/models/treasury_prices.py` & `openbb_tmx-1.0.1/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/utils/gql.py` & `openbb_tmx-1.0.1/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/openbb_tmx/utils/helpers.py` & `openbb_tmx-1.0.1/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.0/pyproject.toml` & `openbb_tmx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-tmx"
-version = "1.0.0"
+version = "1.0.1"
 description = "Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API."
 authors = ["OpenBB <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb_tmx" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp-client-cache = "^0.10.0"
 aiosqlite = "^0.19.0"
 random-user-agent = "^1.0.1"
 exchange-calendars = "^4.2.8"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tmx = "openbb_tmx:tmx_provider"
```

### Comparing `openbb_tmx-1.0.0/PKG-INFO` & `openbb_tmx-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-tmx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API.
 Author: OpenBB
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp-client-cache (>=0.10.0,<0.11.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: exchange-calendars (>=4.2.8,<5.0.0)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # openbb-tmx: A Community Data Provider Extension
 
 `openbb-tmx` is an unofficial, community, data provider extension for the OpenBB Platform.
```

