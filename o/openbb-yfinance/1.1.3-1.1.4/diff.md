# Comparing `tmp/openbb_yfinance-1.1.3.tar.gz` & `tmp/openbb_yfinance-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_yfinance-1.1.3.tar", max compression
+gzip compressed data, was "openbb_yfinance-1.1.4.tar", max compression
```

## Comparing `openbb_yfinance-1.1.3.tar` & `openbb_yfinance-1.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      450 2024-01-17 14:26:16.882592 openbb_yfinance-1.1.3/README.md
--rw-r--r--   0        0        0     4232 2024-03-11 10:41:33.417789 openbb_yfinance-1.1.3/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-01-17 14:26:16.882810 openbb_yfinance-1.1.3/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     2957 2024-02-23 17:14:57.547740 openbb_yfinance-1.1.3/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-02-23 17:14:57.547836 openbb_yfinance-1.1.3/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     1935 2024-01-17 14:26:16.883092 openbb_yfinance-1.1.3/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-02-23 17:14:57.549724 openbb_yfinance-1.1.3/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-02-23 17:14:57.549856 openbb_yfinance-1.1.3/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-02-26 09:54:05.510248 openbb_yfinance-1.1.3/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-03-11 10:41:33.417975 openbb_yfinance-1.1.3/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-03-11 10:41:33.418090 openbb_yfinance-1.1.3/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-03-11 10:41:33.418284 openbb_yfinance-1.1.3/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5722 2024-02-23 17:14:57.550490 openbb_yfinance-1.1.3/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-02-23 17:14:57.550610 openbb_yfinance-1.1.3/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-01-17 14:26:16.883741 openbb_yfinance-1.1.3/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0     9193 2024-02-23 17:14:57.550723 openbb_yfinance-1.1.3/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-01-26 17:52:27.973264 openbb_yfinance-1.1.3/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-03-11 10:41:33.418403 openbb_yfinance-1.1.3/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-02-23 17:14:57.550924 openbb_yfinance-1.1.3/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-02-23 17:14:57.551012 openbb_yfinance-1.1.3/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-02-23 17:14:57.551122 openbb_yfinance-1.1.3/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-02-23 17:14:57.551217 openbb_yfinance-1.1.3/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-03-11 10:41:33.418525 openbb_yfinance-1.1.3/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-02-23 17:14:57.551445 openbb_yfinance-1.1.3/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-02-26 14:49:06.441344 openbb_yfinance-1.1.3/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-02-23 17:14:57.551535 openbb_yfinance-1.1.3/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-02-23 17:14:57.551642 openbb_yfinance-1.1.3/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     3922 2024-02-23 17:14:57.551742 openbb_yfinance-1.1.3/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-02-23 17:14:57.551835 openbb_yfinance-1.1.3/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-02-23 17:14:57.551932 openbb_yfinance-1.1.3/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-02-23 17:14:57.552041 openbb_yfinance-1.1.3/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.884442 openbb_yfinance-1.1.3/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-01-17 14:26:16.884543 openbb_yfinance-1.1.3/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-01-17 14:26:16.884634 openbb_yfinance-1.1.3/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6639 2024-03-11 10:41:33.418638 openbb_yfinance-1.1.3/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-03-11 10:41:33.418776 openbb_yfinance-1.1.3/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0      484 2024-03-11 19:58:01.085343 openbb_yfinance-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 openbb_yfinance-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      450 2024-02-29 11:03:36.978859 openbb_yfinance-1.1.4/README.md
+-rw-r--r--   0        0        0     4232 2024-03-21 17:38:35.661543 openbb_yfinance-1.1.4/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.979066 openbb_yfinance-1.1.4/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-01 13:46:32.186015 openbb_yfinance-1.1.4/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-03-21 17:38:35.661819 openbb_yfinance-1.1.4/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     1935 2024-03-21 17:38:35.661928 openbb_yfinance-1.1.4/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-03-13 16:36:51.900644 openbb_yfinance-1.1.4/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-03-13 16:36:51.900730 openbb_yfinance-1.1.4/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-03-13 16:36:51.900846 openbb_yfinance-1.1.4/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-03-21 17:38:35.662100 openbb_yfinance-1.1.4/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-03-21 17:38:35.662226 openbb_yfinance-1.1.4/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-03-21 17:38:35.662401 openbb_yfinance-1.1.4/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5722 2024-03-13 16:36:51.901334 openbb_yfinance-1.1.4/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-03-13 16:36:51.901450 openbb_yfinance-1.1.4/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-02-29 11:03:36.979842 openbb_yfinance-1.1.4/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10040 2024-04-01 11:58:23.835972 openbb_yfinance-1.1.4/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-03-21 17:38:35.662520 openbb_yfinance-1.1.4/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-03-21 17:38:35.662638 openbb_yfinance-1.1.4/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-03-21 17:38:35.662730 openbb_yfinance-1.1.4/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-03-21 17:38:35.662848 openbb_yfinance-1.1.4/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-03-13 16:36:51.901953 openbb_yfinance-1.1.4/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-03-13 16:36:51.902047 openbb_yfinance-1.1.4/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-03-21 17:38:35.662968 openbb_yfinance-1.1.4/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-03-13 16:36:51.902309 openbb_yfinance-1.1.4/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-03-13 16:36:51.902559 openbb_yfinance-1.1.4/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-03-21 17:38:35.663075 openbb_yfinance-1.1.4/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-03-21 17:38:35.663197 openbb_yfinance-1.1.4/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     3922 2024-03-13 16:36:51.902853 openbb_yfinance-1.1.4/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-03-13 16:36:51.902907 openbb_yfinance-1.1.4/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-03-21 17:38:35.663370 openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-03-21 17:38:35.663509 openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.980652 openbb_yfinance-1.1.4/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-02-29 11:03:36.980745 openbb_yfinance-1.1.4/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-03-13 16:36:51.903317 openbb_yfinance-1.1.4/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6639 2024-03-21 17:38:35.663686 openbb_yfinance-1.1.4/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-03-13 16:36:51.903594 openbb_yfinance-1.1.4/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0      484 2024-04-01 14:19:31.712085 openbb_yfinance-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 openbb_yfinance-1.1.4/PKG-INFO
```

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/__init__.py` & `openbb_yfinance-1.1.4/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/active.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/active.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,17 +77,19 @@
     @staticmethod
     def transform_data(
         query: EquityPerformanceQueryParams,
         data: DataFrame,
         **kwargs: Any,
     ) -> List[YFActiveData]:
         """Transform data."""
-
         columns = ["Market Cap", "Avg Vol (3 month)", "Volume", "% Change"]
 
         data = df_transform_numbers(data, columns)
         data = data.fillna("N/A").replace("N/A", None)
 
+        # parse "Volume" column to float do avoid sorting issues
+        data["Volume"] = data["Volume"].astype(float)
+
         return [
             YFActiveData.model_validate(d)
             for d in data.sort_values(by="Volume", ascending=False).to_dict("records")
         ]
```

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/available_indices.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/balance_sheet.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/cash_flow.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/company_news.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/crypto_historical.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/currency_historical.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/equity_historical.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/equity_profile.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/equity_quote.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/etf_historical.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/etf_info.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/etf_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -186,15 +186,17 @@
         alias="previousClose",
     )
 
     @field_validator("inception_date", mode="before", check_fields=False)
     @classmethod
     def validate_date(cls, v):
         """Validate first stock price date."""
-        return datetime.utcfromtimestamp(v).date().strftime("%Y-%m-%d") if v else None
+        if isinstance(v, datetime):
+            return v.date().strftime("%Y-%m-%d")
+        return datetime.fromtimestamp(v).date().strftime("%Y-%m-%d") if v else None
 
 
 class YFinanceEtfInfoFetcher(
     Fetcher[YFinanceEtfInfoQueryParams, List[YFinanceEtfInfoData]]
 ):
     """YFinance ETF Info fetcher."""
 
@@ -245,30 +247,44 @@
             "fiftyDayAverage",
             "twoHundredDayAverage",
             "ytdReturn",
             "threeYearAverageReturn",
             "fiveYearAverageReturn",
             "beta3Year",
             "longBusinessSummary",
+            "firstTradeDateEpochUtc",
         ]
 
         async def get_one(symbol):
             """Get the data for one ticker symbol."""
             result = {}
             ticker = {}
             try:
                 ticker = Ticker(symbol).get_info()
             except Exception as e:
                 _warn(f"Error getting data for {symbol}: {e}")
             if ticker:
                 quote_type = ticker.pop("quoteType", "")
                 if quote_type == "ETF":
-                    for field in fields:
-                        if field in ticker:
-                            result[field] = ticker.get(field, None)
+                    try:
+                        for field in fields:
+                            if field in ticker and ticker.get(field) is not None:
+                                result[field] = ticker.get(field, None)
+                        if "firstTradeDateEpochUtc" in result:
+                            _first_trade = result.pop("firstTradeDateEpochUtc")
+                            if (
+                                "fundInceptionDate" not in result
+                                and _first_trade is not None
+                            ):
+                                result["fundInceptionDate"] = datetime.fromtimestamp(
+                                    _first_trade
+                                )
+                    except Exception as e:
+                        _warn(f"Error processing data for {symbol}: {e}")
+                        result = {}
                 if quote_type != "ETF":
                     _warn(f"{symbol} is not an ETF.")
                 if result:
                     results.append(result)
 
         tasks = [get_one(symbol) for symbol in symbols]
```

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/futures_curve.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/futures_historical.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/gainers.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/growth_tech_equities.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/historical_dividends.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/income_statement.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/index_historical.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/key_executives.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/key_metrics.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/losers.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/market_indices.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/price_target_consensus.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/share_statistics.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_yfinance-1.1.4/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/utils/futures.csv` & `openbb_yfinance-1.1.4/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/utils/helpers.py` & `openbb_yfinance-1.1.4/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/openbb_yfinance/utils/references.py` & `openbb_yfinance-1.1.4/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.3/PKG-INFO` & `openbb_yfinance-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-yfinance
-Version: 1.1.3
+Version: 1.1.4
 Summary: yfinance extension for OpenBB
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
 Requires-Dist: yfinance (>=0.2.27,<0.3.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Yahoo!Finance Provider
 
 This extension integrates the [Yahoo!Finance](https://finance.yahoo.com/) data provider into the OpenBB Platform.
```

