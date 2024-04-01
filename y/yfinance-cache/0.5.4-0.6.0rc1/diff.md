# Comparing `tmp/yfinance-cache-0.5.4.tar.gz` & `tmp/yfinance-cache-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfinance-cache-0.5.4.tar", last modified: Sun Mar 31 21:29:36 2024, max compression
+gzip compressed data, was "yfinance-cache-0.6.0rc1.tar", last modified: Mon Apr  1 19:50:05 2024, max compression
```

## Comparing `yfinance-cache-0.5.4.tar` & `yfinance-cache-0.6.0rc1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-03-31 21:29:36.541783 yfinance-cache-0.5.4/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/LICENSE
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5658 2024-03-31 21:29:36.541783 yfinance-cache-0.5.4/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4966 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/README.md
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/pyproject.toml
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      829 2024-03-31 21:29:36.541783 yfinance-cache-0.5.4/setup.cfg
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-03-31 21:29:36.540783 yfinance-cache-0.5.4/tests/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1651 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/context.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_cache.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_datetime-assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_schedules_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_schedules_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_schedules_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_market_schedules_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_missing_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_missing_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_missing_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_missing_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_price_data_aging_1d.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_price_data_aging_1h.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_price_data_aging_1w.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_time_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_yf_assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_yfc_adjust.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_yfc_backend.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_yfc_interface.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/test_yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4477 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/tests/utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-03-31 21:29:36.534783 yfinance-cache-0.5.4/yfinance_cache/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      324 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/yfinance_cache/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    15998 2024-02-10 20:27:27.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_cache_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    14671 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_dat.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_logging.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-02-10 20:27:47.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_multi.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-02-10 13:35:58.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_options.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-02-10 20:34:05.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_prices_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    42429 2024-03-31 21:28:46.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-02-10 20:32:55.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_time.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-02-10 20:32:31.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_upgrade.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24742 2024-02-10 20:32:02.000000 yfinance-cache-0.5.4/yfinance_cache/yfc_utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-03-31 21:29:36.541783 yfinance-cache-0.5.4/yfinance_cache.egg-info/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5658 2024-03-31 21:29:36.000000 yfinance-cache-0.5.4/yfinance_cache.egg-info/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2213 2024-03-31 21:29:36.000000 yfinance-cache-0.5.4/yfinance_cache.egg-info/SOURCES.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-03-31 21:29:36.000000 yfinance-cache-0.5.4/yfinance_cache.egg-info/dependency_links.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-03-31 21:29:36.000000 yfinance-cache-0.5.4/yfinance_cache.egg-info/requires.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-03-31 21:29:36.000000 yfinance-cache-0.5.4/yfinance_cache.egg-info/top_level.txt
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/LICENSE
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5294 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/README.md
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      832 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.166226 yfinance-cache-0.6.0rc1/tests/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc1/tests/context.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_cache.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_datetime-assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1d.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1h.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1w.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_time_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yf_assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_adjust.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_backend.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_financials.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_interface.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc1/tests/utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.160226 yfinance-cache-0.6.0rc1/yfinance_cache/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_cache_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_dat.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    87870 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_financials_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_logging.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_multi.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_options.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_prices_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39045 2024-03-31 21:41:16.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_time.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-02-25 13:22:49.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_upgrade.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25378 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/requires.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/top_level.txt
```

### Comparing `yfinance-cache-0.5.4/LICENSE` & `yfinance-cache-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/PKG-INFO` & `yfinance-cache-0.6.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.5.4
+Version: 0.6.0rc1
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,20 +20,20 @@
 
 # yfinance-cache
 
 Persistent caching wrapper for `yfinance` module. Intelligent caching, not dumb caching of web requests - only update cache where missing/outdated and new data expected. Idea is to minimise fetch frequency and quantity - Yahoo API officially only cares about frequency, but I'm guessing they also care about server load from scrapers.
 
 Cache auto-update implemented for:
 - prices
-- calendar
+- financials
+- calendar & earnings_dates
 - shares
 - info
 
 Everything else cached once but never updated (unless you delete their files).
-Financials auto-update will be implemented soon ...
 
 Persistent cache stored in your user cache folder:
 - Windows = C:/Users/\<USER\>/AppData/Local/py-yfinance-cache
 - Linux = /home/\<USER\>/.cache/py-yfinance-cache
 - MacOS = /Users/\<USER\>/Library/Caches/py-yfinance-cache
 
 ## Interface
@@ -42,19 +42,19 @@
 
 ```python
 import yfinance_cache as yfc
 
 msft = yfc.Ticker("MSFT")
 msft.info
 msft.calendar
+msft.cashflow ; msft.quarterly_cashflow  # or: balance_sheet, financials
+msft.get_earnings_dates(4)
 msft.get_shares(start='2024-01-01')
 msft.history(period="1wk")
 yfc.download("MSFT AMZN", period="1wk")
-
-# See yfinance documentation for full API
 ```
 
 ### Price data differences
 
 Other people have implemented price caches, but none adjust cached data for new stock splits or dividends.
 YFC does. Price can be adjusted for stock splits, dividends, or both:
 
@@ -114,15 +114,22 @@
     "max_ages": {
         "calendar": "30d",
         "info": "180d"
     }
 }
 ```
 
-#### Verifying cache
+## Financials
+
+Financials updates are handled different because they don't age.
+Instead, YFC analyses earnings dates to determine exactly when next earnings will be, 
+or if Yahoo data is incomplete then YFC will predict.
+You can inspect this schedule in new function `dat.get_release_dates()`.
+
+## Verifying cache
 
 Cached prices can be compared against latest Yahoo Finance data, and correct differences:
 ```python
 # Verify prices of one ticker symbol
 msft.verify_cached_prices(
 	rtol=0.0001,  # relative tolerance for differences
 	vol_rtol=0.005,  # relative tolerance specifically for Volume
```

### Comparing `yfinance-cache-0.5.4/README.md` & `yfinance-cache-0.6.0rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # yfinance-cache
 
 Persistent caching wrapper for `yfinance` module. Intelligent caching, not dumb caching of web requests - only update cache where missing/outdated and new data expected. Idea is to minimise fetch frequency and quantity - Yahoo API officially only cares about frequency, but I'm guessing they also care about server load from scrapers.
 
 Cache auto-update implemented for:
 - prices
-- calendar
+- financials
+- calendar & earnings_dates
 - shares
 - info
 
 Everything else cached once but never updated (unless you delete their files).
-Financials auto-update will be implemented soon ...
 
 Persistent cache stored in your user cache folder:
 - Windows = C:/Users/\<USER\>/AppData/Local/py-yfinance-cache
 - Linux = /home/\<USER\>/.cache/py-yfinance-cache
 - MacOS = /Users/\<USER\>/Library/Caches/py-yfinance-cache
 
 ## Interface
@@ -22,19 +22,19 @@
 
 ```python
 import yfinance_cache as yfc
 
 msft = yfc.Ticker("MSFT")
 msft.info
 msft.calendar
+msft.cashflow ; msft.quarterly_cashflow  # or: balance_sheet, financials
+msft.get_earnings_dates(4)
 msft.get_shares(start='2024-01-01')
 msft.history(period="1wk")
 yfc.download("MSFT AMZN", period="1wk")
-
-# See yfinance documentation for full API
 ```
 
 ### Price data differences
 
 Other people have implemented price caches, but none adjust cached data for new stock splits or dividends.
 YFC does. Price can be adjusted for stock splits, dividends, or both:
 
@@ -94,15 +94,22 @@
     "max_ages": {
         "calendar": "30d",
         "info": "180d"
     }
 }
 ```
 
-#### Verifying cache
+## Financials
+
+Financials updates are handled different because they don't age.
+Instead, YFC analyses earnings dates to determine exactly when next earnings will be, 
+or if Yahoo data is incomplete then YFC will predict.
+You can inspect this schedule in new function `dat.get_release_dates()`.
+
+## Verifying cache
 
 Cached prices can be compared against latest Yahoo Finance data, and correct differences:
 ```python
 # Verify prices of one ticker symbol
 msft.verify_cached_prices(
 	rtol=0.0001,  # relative tolerance for differences
 	vol_rtol=0.005,  # relative tolerance specifically for Volume
```

### Comparing `yfinance-cache-0.5.4/setup.cfg` & `yfinance-cache-0.6.0rc1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yfinance-cache
-version = 0.5.4
+version = 0.6.0rc1
 author = ValueRaider
 author_email = ValueRaider@protonmail.com
 description = Smart caching wrapper for 'yfinance' module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ValueRaider/yfinance-cache
 project_urls =
```

### Comparing `yfinance-cache-0.5.4/tests/context.py` & `yfinance-cache-0.6.0rc1/tests/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 _parent_dp = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 # _src_dp = os.path.join(_parent_dp, "src")
 _src_dp = _parent_dp
 sys.path.insert(0, _src_dp)
 
 # import yfinance_cache
-from yfinance_cache import yfc_cache_manager, yfc_dat, yfc_prices_manager, yfc_ticker, yfc_time, yfc_utils, yfc_logging, yfc_options
+from yfinance_cache import yfc_cache_manager, yfc_dat, yfc_prices_manager, yfc_financials_manager, yfc_ticker, yfc_time, yfc_utils, yfc_logging, yfc_options
 
 
 import numpy as np ; np.seterr(divide='raise', over='raise', under='raise', invalid='raise')
 
 
 # Setup a session to rate-limit and cache persistently:
 import datetime as _dt
```

### Comparing `yfinance-cache-0.5.4/tests/test_cache.py` & `yfinance-cache-0.6.0rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_datetime-assumptions.py` & `yfinance-cache-0.6.0rc1/tests/test_datetime-assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_intervals_asx.py` & `yfinance-cache-0.6.0rc1/tests/test_market_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_intervals_nze.py` & `yfinance-cache-0.6.0rc1/tests/test_market_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_intervals_tlv.py` & `yfinance-cache-0.6.0rc1/tests/test_market_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_intervals_usa.py` & `yfinance-cache-0.6.0rc1/tests/test_market_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_schedules_asx.py` & `yfinance-cache-0.6.0rc1/tests/test_market_schedules_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_schedules_nze.py` & `yfinance-cache-0.6.0rc1/tests/test_market_schedules_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_schedules_tlv.py` & `yfinance-cache-0.6.0rc1/tests/test_market_schedules_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_market_schedules_usa.py` & `yfinance-cache-0.6.0rc1/tests/test_market_schedules_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_missing_intervals_asx.py` & `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_missing_intervals_nze.py` & `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_missing_intervals_tlv.py` & `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_missing_intervals_usa.py` & `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_price_data_aging_1d.py` & `yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1d.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_price_data_aging_1h.py` & `yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1h.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_price_data_aging_1w.py` & `yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1w.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_time_utils.py` & `yfinance-cache-0.6.0rc1/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_utils.py` & `yfinance-cache-0.6.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_yf_assumptions.py` & `yfinance-cache-0.6.0rc1/tests/test_yf_assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_yfc_adjust.py` & `yfinance-cache-0.6.0rc1/tests/test_yfc_adjust.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_yfc_backend.py` & `yfinance-cache-0.6.0rc1/tests/test_yfc_backend.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_yfc_interface.py` & `yfinance-cache-0.6.0rc1/tests/test_yfc_interface.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/test_yfc_ticker.py` & `yfinance-cache-0.6.0rc1/tests/test_yfc_ticker.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/tests/utils.py` & `yfinance-cache-0.6.0rc1/tests/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 import numpy as np
 import unittest
 from pprint import pprint
 
+import os
+import time
+def take_directory_snapshot(directory_path):
+    snapshot = {}
+    for root, dirs, files in os.walk(directory_path):
+        for file in files:
+            file_path = os.path.join(root, file)
+            try:
+                stats = os.stat(file_path)
+                snapshot[file_path] = {
+                    'size': stats.st_size,
+                    'modification_time': time.ctime(stats.st_mtime)
+                }
+            except FileNotFoundError:
+                # The file might have been deleted between os.walk and os.stat
+                continue
+    return snapshot
+
+
 class Test_Base(unittest.TestCase):
     def verify_df(self, df, answer, rtol=None, different=False):
         if (df is None or df.shape[0]==0) and (answer is None or answer.shape[0]==0):
             return
 
         if df is None:
             print("df is None but answer is:")
```

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_cache_manager.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_cache_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from zoneinfo import ZoneInfo
 
 from . import yfc_dat as yfcd
 from . import yfc_utils as yfcu
 
 # To reduce #files in cache, store some YF objects together into same file (including metadata)
 packed_data_cats = {}
-packed_data_cats["quarterlys"] = ["quarterly_balance_sheet", "quarterly_cashflow", "quarterly_earnings", "quarterly_financials"]
-packed_data_cats["annuals"]    = ["balance_sheet", "cashflow", "earnings", "financials"]
+packed_data_cats["quarterlys"] = ["quarterly_balance_sheet", "quarterly_cashflow", "quarterly_earnings", "quarterly_financials", "quarterly_income_stmt"]
+packed_data_cats["annuals"]    = ["balance_sheet", "cashflow", "earnings", "financials", "income_stmt"]
 
 quarterly_objects = packed_data_cats["quarterlys"]
 annual_objects    = packed_data_cats["annuals"]
 
 verbose = False
 # verbose = True
 
@@ -62,37 +62,42 @@
 
 def GetFilepath(ticker, objectName, obj=None, prune=False):
     if IsObjectInPackedData(objectName):
         return GetFilepathPacked(ticker, objectName)
 
     fp = None
     if obj is not None:
-        if isinstance(obj, (list, int, float, str, datetime, date, timedelta)):
+        if isinstance(obj, list) and (len(obj)==0 or isinstance(obj[0], (int, float, str, datetime, date, timedelta))):
             ext = "json"
-            ext2 = "pkl"
+            ext_bad = "pkl"
+        elif isinstance(obj, (int, float, str, datetime, date, timedelta)):
+            ext = "json"
+            ext_bad = "pkl"
         else:
             ext = "pkl"
-            ext2 = "json"
+            ext_bad = "json"
         fp = os.path.join(GetCacheDirpath(), ticker, objectName) + "."+ext
-        fp2 = os.path.join(GetCacheDirpath(), ticker, objectName) + "."+ext2
-        if os.path.isfile(fp2):
+        fp_bad = os.path.join(GetCacheDirpath(), ticker, objectName) + "."+ext_bad
+        if os.path.isfile(fp_bad):
             if prune:
-                os.remove(fp2)
+                os.remove(fp_bad)
             else:
-                raise Exception("For {} object {}/{}, a {} file already exists".format(ext, ticker, objectName, ext2))
+                raise Exception("For {} object {}/{}, a {} file already exists".format(ext, ticker, objectName, ext_bad))
     else:
         fp_base = os.path.join(GetCacheDirpath(), ticker, objectName)
         json_exists = os.path.isfile(fp_base+".json")
         pkl_exists = os.path.isfile(fp_base+".pkl")
         if json_exists and pkl_exists:
             raise Exception("For cached datum '{0}', both a .json and .pkl file exist. Should only be one.".format(objectName))
         elif json_exists:
             fp = fp_base + ".json"
         elif pkl_exists:
             fp = fp_base + ".pkl"
+        elif "release-dates" in objectName or "earnings_dates" in objectName:
+            fp = fp_base + ".pkl"
     return fp
 def GetFilepathPacked(ticker, objectName):
     if not IsObjectInPackedData(objectName):
         return GetFilepath(ticker, objectName)
     pkg = GetPackedDataCat(objectName)
     fp = os.path.join(GetCacheDirpath(), ticker, pkg) + ".pkl"
     return fp
@@ -359,15 +364,15 @@
     if IsObjectInPackedData(objectName):
         pkData = _ReadPackedData(ticker, objectName)
         if (pkData is not None) and (objectName in pkData):
             objData = pkData[objectName]
             md      = objData["metadata"] if "metadata" in objData else None
     else:
         d = _ReadData(ticker, objectName)
-        if "metadata" not in d:
+        if d is None or "metadata" not in d:
             return None
         md = d["metadata"]
         if verbose:
             print("ReadCacheMetadata() read md as:")
             print(md)
     if md is None:
         return None
@@ -385,19 +390,20 @@
         if value is None:
             print(f"WriteCacheMetadata({ticker}, {objectName}, {key}) deleting")
         else:
             print(f"WriteCacheMetadata({ticker}, {objectName}, {key}) storing")
 
     d = _ReadData(ticker, objectName)
     if d is None:
-        raise Exception("'{}/{}' not in cache, cannot add metadata".format(ticker, objectName))
+        d = {"data":None}
 
     if "metadata" in d:
         if value is None:
-            del d["metadata"][key]
+            if key in d["metadata"]:
+                del d["metadata"][key]
         else:
             d["metadata"][key] = value
     elif value is not None:
         d["metadata"] = {key: value}
 
     if verbose:
         print("WriteCacheMetadata() updated md to:")
```

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_logging.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_logging.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_multi.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_multi.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_options.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_options.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_prices_manager.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_prices_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_ticker.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_ticker.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from . import yfc_cache_manager as yfcm
 from . import yfc_dat as yfcd
 from . import yfc_utils as yfcu
 from . import yfc_logging as yfcl
 from . import yfc_time as yfct
 from . import yfc_prices_manager as yfcp
+from . import yfc_financials_manager as yfcf
 
 import numpy as np
 import pandas as pd
 import datetime
 from dateutil.relativedelta import relativedelta
 from zoneinfo import ZoneInfo
 import os
@@ -33,30 +34,18 @@
         self._info = None
         self._fast_info = None
 
         self._splits = None
 
         self._shares = None
 
-        self._financials = None
-        self._quarterly_financials = None
-
         self._major_holders = None
 
         self._institutional_holders = None
 
-        self._balance_sheet = None
-        self._quarterly_balance_sheet = None
-
-        self._cashflow = None
-        self._quarterly_cashflow = None
-
-        self._earnings = None
-        self._quarterly_earnings = None
-
         self._sustainability = None
 
         self._recommendations = None
 
         self._calendar = None
 
         self._isin = None
@@ -67,14 +56,17 @@
 
         self._debug = False
         # self._debug = True
 
         self._tz = None
         self._exchange = None
 
+        exchange, tz_name = self._getExchangeAndTz()
+        self._financials_manager = yfcf.FinancialsManager(ticker, exchange, tz_name, session=self.session)
+
     def history(self,
                 interval="1d",
                 max_age=None,  # defaults to half of interval
                 period=None,
                 start=None, end=None, prepost=False, actions=True,
                 adjust_splits=True, adjust_divs=True,
                 keepna=False,
@@ -474,31 +466,16 @@
 
         v = self._histories_manager.GetHistory(interval)._verifyCachedPrices(rtol, vol_rtol, correct, discard_old, quiet, debug)
 
         yfcl.TraceExit(f"Ticker::_verify_cached_prices_interval() returning {v}")
         return v
 
     def _process_user_dt(self, dt):
-        d = None
         exchange, tz_name = self._getExchangeAndTz()
-        tz_exchange = ZoneInfo(tz_name)
-        if isinstance(dt, str):
-            d = datetime.datetime.strptime(dt, "%Y-%m-%d").date()
-            dt = datetime.datetime.combine(d, datetime.time(0), tz_exchange)
-        elif isinstance(dt, datetime.date) and not isinstance(dt, datetime.datetime):
-            d = dt
-            dt = datetime.datetime.combine(dt, datetime.time(0), tz_exchange)
-        elif not isinstance(dt, datetime.datetime):
-            raise Exception("Argument 'dt' must be str, date or datetime")
-        dt = dt.replace(tzinfo=tz_exchange) if dt.tzinfo is None else dt.astimezone(tz_exchange)
-
-        if d is None and dt.time() == datetime.time(0):
-            d = dt.date()
-
-        return dt, d
+        return yfcu.ProcessUserDt(dt, tz_name)
 
     @property
     def info(self):
         return self.get_info()
 
     def get_info(self, max_age=None):
         if self._info is not None:
@@ -724,40 +701,14 @@
         df = df.sort_index()
 
         df['FetchDate'] = fetch_dt
 
         return df
 
     @property
-    def financials(self):
-        if self._financials is not None:
-            return self._financials
-
-        if yfcm.IsDatumCached(self.ticker, "financials"):
-            self._financials = yfcm.ReadCacheDatum(self.ticker, "financials")
-            return self._financials
-
-        self._financials = self.dat.financials
-        yfcm.StoreCacheDatum(self.ticker, "financials", self._financials)
-        return self._financials
-
-    @property
-    def quarterly_financials(self):
-        if self._quarterly_financials is not None:
-            return self._quarterly_financials
-
-        if yfcm.IsDatumCached(self.ticker, "quarterly_financials"):
-            self._quarterly_financials = yfcm.ReadCacheDatum(self.ticker, "quarterly_financials")
-            return self._quarterly_financials
-
-        self._quarterly_financials = self.dat.quarterly_financials
-        yfcm.StoreCacheDatum(self.ticker, "quarterly_financials", self._quarterly_financials)
-        return self._quarterly_financials
-
-    @property
     def major_holders(self):
         if self._major_holders is not None:
             return self._major_holders
 
         if yfcm.IsDatumCached(self.ticker, "major_holders"):
             self._major_holders = yfcm.ReadCacheDatum(self.ticker, "major_holders")
             return self._major_holders
@@ -776,90 +727,91 @@
             return self._institutional_holders
 
         self._institutional_holders = self.dat.institutional_holders
         yfcm.StoreCacheDatum(self.ticker, "institutional_holders", self._institutional_holders)
         return self._institutional_holders
 
     @property
-    def balance_sheet(self):
-        if self._balance_sheet is not None:
-            return self._balance_sheet
-
-        if yfcm.IsDatumCached(self.ticker, "balance_sheet"):
-            self._balance_sheet = yfcm.ReadCacheDatum(self.ticker, "balance_sheet")
-            return self._balance_sheet
-
-        self._balance_sheet = self.dat.balance_sheet
-        yfcm.StoreCacheDatum(self.ticker, "balance_sheet", self._balance_sheet)
-        return self._balance_sheet
+    def earnings(self):
+        return self._financials_manager.get_earnings()
 
     @property
-    def quarterly_balance_sheet(self):
-        if self._quarterly_balance_sheet is not None:
-            return self._quarterly_balance_sheet
+    def quarterly_earnings(self):
+        return self._financials_manager.get_quarterly_earnings()
 
-        if yfcm.IsDatumCached(self.ticker, "quarterly_balance_sheet"):
-            self._quarterly_balance_sheet = yfcm.ReadCacheDatum(self.ticker, "quarterly_balance_sheet")
-            return self._quarterly_balance_sheet
-
-        self._quarterly_balance_sheet = self.dat.quarterly_balance_sheet
-        yfcm.StoreCacheDatum(self.ticker, "quarterly_balance_sheet", self._quarterly_balance_sheet)
-        return self._quarterly_balance_sheet
+    @property
+    def income_stmt(self):
+        return self._financials_manager.get_income_stmt()
 
     @property
-    def cashflow(self):
-        if self._cashflow is not None:
-            return self._cashflow
+    def quarterly_income_stmt(self):
+        return self._financials_manager.get_quarterly_income_stmt()
 
-        if yfcm.IsDatumCached(self.ticker, "cashflow"):
-            self._cashflow = yfcm.ReadCacheDatum(self.ticker, "cashflow")
-            return self._cashflow
-
-        self._cashflow = self.dat.cashflow
-        yfcm.StoreCacheDatum(self.ticker, "cashflow", self._cashflow)
-        return self._cashflow
+    @property
+    def financials(self):
+        return self._financials_manager.get_income_stmt()
 
     @property
-    def quarterly_cashflow(self):
-        if self._quarterly_cashflow is not None:
-            return self._quarterly_cashflow
+    def quarterly_financials(self):
+        return self._financials_manager.get_quarterly_income_stmt()
 
-        if yfcm.IsDatumCached(self.ticker, "quarterly_cashflow"):
-            self._quarterly_cashflow = yfcm.ReadCacheDatum(self.ticker, "quarterly_cashflow")
-            return self._quarterly_cashflow
-
-        self._quarterly_cashflow = self.dat.quarterly_cashflow
-        yfcm.StoreCacheDatum(self.ticker, "quarterly_cashflow", self._quarterly_cashflow)
-        return self._quarterly_cashflow
+    @property
+    def balance_sheet(self):
+        return self._financials_manager.get_balance_sheet()
 
     @property
-    def earnings(self):
-        if self._earnings is not None:
-            return self._earnings
+    def quarterly_balance_sheet(self):
+        return self._financials_manager.get_quarterly_balance_sheet()
 
-        if yfcm.IsDatumCached(self.ticker, "earnings"):
-            self._earnings = yfcm.ReadCacheDatum(self.ticker, "earnings")
-            return self._earnings
-
-        self._earnings = self.dat.earnings
-        yfcm.StoreCacheDatum(self.ticker, "earnings", self._earnings)
-        return self._earnings
+    @property
+    def cashflow(self):
+        return self._financials_manager.get_cashflow()
 
     @property
-    def quarterly_earnings(self):
-        if self._quarterly_earnings is not None:
-            return self._quarterly_earnings
+    def quarterly_cashflow(self):
+        return self._financials_manager.get_quarterly_cashflow()
+
+    def get_earnings_dates(self, limit=12):
+        return self._financials_manager.get_earnings_dates(limit)
 
-        if yfcm.IsDatumCached(self.ticker, "quarterly_earnings"):
-            self._quarterly_earnings = yfcm.ReadCacheDatum(self.ticker, "quarterly_earnings")
-            return self._quarterly_earnings
-
-        self._quarterly_earnings = self.dat.quarterly_earnings
-        yfcm.StoreCacheDatum(self.ticker, "quarterly_earnings", self._quarterly_earnings)
-        return self._quarterly_earnings
+    def get_release_dates(self, period='quarterly', as_df=False, check=True):
+        if not period in ['annual', 'quarterly']:
+            raise ValueError(f'period argument must be "annual" or "quarterly", not "{period}"')
+        if period == 'annual':
+            period = yfcd.ReportingPeriod.Full
+        else:
+            period = yfcd.ReportingPeriod.Interim
+
+        releases = self._financials_manager.get_release_dates(period, as_df, refresh=True, check=check)
+        if releases is None:
+            return releases
+
+        if as_df:
+            # Format:
+            releases['Period end uncertainty'] = '0d'
+            f = releases['PE confidence'] == yfcd.Confidence.Medium
+            if f.any():
+                releases.loc[f, 'Period end uncertainty'] = '+-7d'
+            f = releases['PE confidence'] == yfcd.Confidence.Low
+            if f.any():
+                releases.loc[f, 'Period end uncertainty'] = '+-45d'
+            releases = releases.drop('PE confidence', axis=1)
+
+            releases['Release date uncertainty'] = '0d'
+            f = releases['RD confidence'] == yfcd.Confidence.Medium
+            if f.any():
+                releases.loc[f, 'Release date uncertainty'] = '+/-7d'
+            f = releases['RD confidence'] == yfcd.Confidence.Low
+            if f.any():
+                releases.loc[f, 'Release date uncertainty'] = '+/-45d'
+            releases = releases.drop('RD confidence', axis=1)
+
+            releases = releases.drop('Delay', axis=1)
+
+        return releases
 
     @property
     def sustainability(self):
         if self._sustainability is not None:
             return self._sustainability
 
         if yfcm.IsDatumCached(self.ticker, "sustainability"):
@@ -881,45 +833,15 @@
 
         self._recommendations = self.dat.recommendations
         yfcm.StoreCacheDatum(self.ticker, "recommendations", self._recommendations)
         return self._recommendations
 
     @property
     def calendar(self):
-        max_age = pd.Timedelta(yfcm._option_manager.max_ages.calendar)
-
-        if self._calendar is None:
-            if yfcm.IsDatumCached(self.ticker, "calendar"):
-                self._calendar = yfcm.ReadCacheDatum(self.ticker, "calendar")
-                if 'FetchDate' not in self._calendar.keys():
-                    fp = yfcm.GetFilepath(self.ticker, 'info')
-                    mod_dt = datetime.datetime.fromtimestamp(os.path.getmtime(fp))
-                    self._calendar['FetchDate'] = mod_dt
-
-        if (self._calendar is not None) and (self._calendar['FetchDate'] + max_age) > pd.Timestamp.now():
-            return self._calendar
-
-        c = self.dat.calendar
-        c['FetchDate'] = pd.Timestamp.now()
-        
-        if self._calendar is not None:
-            # Check calendar info is not downgrade
-            diff = len(c) - len(self._calendar)
-            if diff < -1:
-                # More than 1 element disappeared
-                msg = 'When fetching new calendar, data has disappeared\n'
-                msg += '- cached calendar:\n'
-                msg += f'{self._calendar}' + '\n'
-                msg += '- new calendar:\n'
-                msg += f'{c}' + '\n'
-                raise Exception(msg)
-
-        yfcm.StoreCacheDatum(self.ticker, "calendar", c)
-        self._calendar = c
-        return self._calendar
+        return self._financials_manager.get_calendar()
 
     @property
     def inin(self):
         if self._inin is not None:
             return self._inin
 
         if yfcm.IsDatumCached(self.ticker, "inin"):
```

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_time.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_time.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_upgrade.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_upgrade.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.5.4/yfinance_cache/yfc_utils.py` & `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, date, timedelta
+from datetime import datetime, date, timedelta, time
 from dateutil.relativedelta import relativedelta
 from zoneinfo import ZoneInfo
 import re
 from pprint import pprint
 import numpy as np
 import math
 import pandas as pd
@@ -44,15 +44,15 @@
 def TypeCheckBool(var, varName):
     if not isinstance(var, (bool, np.bool_)):
         raise TypeError(f"'{varName}' must be bool not {type(var)}")
 def TypeCheckFloat(var, varName):
     if not isinstance(var, (float, np.float32, np.float64)):
         raise TypeError(f"'{varName}' must be float not {type(var)}")
 def TypeCheckInt(var, varName):
-    if not isinstance(var, (int, np.int32, np.int64)):
+    if isinstance(var, bool) or not isinstance(var, (int, np.int32, np.int64)):
         raise TypeError(f"'{varName}' must be int not {type(var)}")
 def TypeCheckIterable(var, varName):
     if not isinstance(var, (list, set, np.ndarray, pd.Series)):
         raise TypeError(f"'{varName}' must be iterable not {type(var)}")
 
 def TypeCheckDateEasy(var, varName):
     if not (isinstance(var, date) or isinstance(var, datetime)):
@@ -180,14 +180,33 @@
 def CalculateRounding(n, sigfigs):
     if GetSigFigs(round(n)) >= sigfigs:
         return 0
     else:
         return sigfigs - GetSigFigs(round(n))
 
 
+def ProcessUserDt(dt, tz_name):
+    d = None
+    tz = ZoneInfo(tz_name)
+    if isinstance(dt, str):
+        d = datetime.strptime(dt, "%Y-%m-%d").date()
+        dt = datetime.combine(d, time(0), tz)
+    elif isinstance(dt, date) and not isinstance(dt, datetime):
+        d = dt
+        dt = datetime.combine(dt, time(0), tz)
+    elif not isinstance(dt, datetime):
+        raise Exception("Argument 'dt' must be str, date or datetime")
+    dt = dt.replace(tzinfo=tz) if dt.tzinfo is None else dt.astimezone(tz)
+
+    if d is None and dt.time() == datetime.time(0):
+        d = dt.date()
+
+    return dt, d
+
+
 def GetCSF0(df):
     if "Stock Splits" not in df:
         raise Exception("DataFrame does not contain column 'Stock Splits")
     if df.shape[0] == 0:
         raise Exception("DataFrame is empty")
 
     ss = df["Stock Splits"].copy()
```

### Comparing `yfinance-cache-0.5.4/yfinance_cache.egg-info/PKG-INFO` & `yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.5.4
+Version: 0.6.0rc1
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,20 +20,20 @@
 
 # yfinance-cache
 
 Persistent caching wrapper for `yfinance` module. Intelligent caching, not dumb caching of web requests - only update cache where missing/outdated and new data expected. Idea is to minimise fetch frequency and quantity - Yahoo API officially only cares about frequency, but I'm guessing they also care about server load from scrapers.
 
 Cache auto-update implemented for:
 - prices
-- calendar
+- financials
+- calendar & earnings_dates
 - shares
 - info
 
 Everything else cached once but never updated (unless you delete their files).
-Financials auto-update will be implemented soon ...
 
 Persistent cache stored in your user cache folder:
 - Windows = C:/Users/\<USER\>/AppData/Local/py-yfinance-cache
 - Linux = /home/\<USER\>/.cache/py-yfinance-cache
 - MacOS = /Users/\<USER\>/Library/Caches/py-yfinance-cache
 
 ## Interface
@@ -42,19 +42,19 @@
 
 ```python
 import yfinance_cache as yfc
 
 msft = yfc.Ticker("MSFT")
 msft.info
 msft.calendar
+msft.cashflow ; msft.quarterly_cashflow  # or: balance_sheet, financials
+msft.get_earnings_dates(4)
 msft.get_shares(start='2024-01-01')
 msft.history(period="1wk")
 yfc.download("MSFT AMZN", period="1wk")
-
-# See yfinance documentation for full API
 ```
 
 ### Price data differences
 
 Other people have implemented price caches, but none adjust cached data for new stock splits or dividends.
 YFC does. Price can be adjusted for stock splits, dividends, or both:
 
@@ -114,15 +114,22 @@
     "max_ages": {
         "calendar": "30d",
         "info": "180d"
     }
 }
 ```
 
-#### Verifying cache
+## Financials
+
+Financials updates are handled different because they don't age.
+Instead, YFC analyses earnings dates to determine exactly when next earnings will be, 
+or if Yahoo data is incomplete then YFC will predict.
+You can inspect this schedule in new function `dat.get_release_dates()`.
+
+## Verifying cache
 
 Cached prices can be compared against latest Yahoo Finance data, and correct differences:
 ```python
 # Verify prices of one ticker symbol
 msft.verify_cached_prices(
 	rtol=0.0001,  # relative tolerance for differences
 	vol_rtol=0.005,  # relative tolerance specifically for Volume
```

### Comparing `yfinance-cache-0.5.4/yfinance_cache.egg-info/SOURCES.txt` & `yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 ./tests/test_price_data_aging_1h.py
 ./tests/test_price_data_aging_1w.py
 ./tests/test_time_utils.py
 ./tests/test_utils.py
 ./tests/test_yf_assumptions.py
 ./tests/test_yfc_adjust.py
 ./tests/test_yfc_backend.py
+./tests/test_yfc_financials.py
 ./tests/test_yfc_interface.py
 ./tests/test_yfc_ticker.py
 ./tests/utils.py
 ./yfinance_cache/__init__.py
 ./yfinance_cache/yfc_cache_manager.py
 ./yfinance_cache/yfc_dat.py
+./yfinance_cache/yfc_financials_manager.py
 ./yfinance_cache/yfc_logging.py
 ./yfinance_cache/yfc_multi.py
 ./yfinance_cache/yfc_options.py
 ./yfinance_cache/yfc_prices_manager.py
 ./yfinance_cache/yfc_ticker.py
 ./yfinance_cache/yfc_time.py
 ./yfinance_cache/yfc_upgrade.py
@@ -63,9 +65,10 @@
 tests/test_price_data_aging_1h.py
 tests/test_price_data_aging_1w.py
 tests/test_time_utils.py
 tests/test_utils.py
 tests/test_yf_assumptions.py
 tests/test_yfc_adjust.py
 tests/test_yfc_backend.py
+tests/test_yfc_financials.py
 tests/test_yfc_interface.py
 tests/test_yfc_ticker.py
```

