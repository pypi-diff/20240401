# Comparing `tmp/openbb-4.1.5.tar.gz` & `tmp/openbb-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb-4.1.5.tar", max compression
+gzip compressed data, was "openbb-4.1.6.tar", max compression
```

## Comparing `openbb-4.1.5.tar` & `openbb-4.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     6818 2024-03-11 19:21:16.058801 openbb-4.1.5/README.md
--rw-r--r--   0        0        0     1324 2024-01-26 17:52:27.958818 openbb-4.1.5/openbb/__init__.py
--rw-r--r--   0        0        0      638 2024-03-11 21:07:34.481061 openbb-4.1.5/openbb/assets/extension_map.json
--rw-r--r--   0        0        0     8699 2024-03-11 21:07:34.481830 openbb-4.1.5/openbb/assets/module_map.json
--rw-r--r--   0        0        0     2794 2024-03-11 21:07:34.566028 openbb-4.1.5/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-03-11 21:07:34.540380 openbb-4.1.5/openbb/package/__init__.py
--rw-r--r--   0        0        0     3340 2024-03-11 21:07:34.822894 openbb-4.1.5/openbb/package/crypto.py
--rw-r--r--   0        0        0     6563 2024-03-11 21:07:34.842386 openbb-4.1.5/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    11751 2024-03-11 21:07:34.868028 openbb-4.1.5/openbb/package/currency.py
--rw-r--r--   0        0        0     6455 2024-03-11 21:07:34.859511 openbb-4.1.5/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-03-11 21:07:34.842041 openbb-4.1.5/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12160 2024-03-11 21:07:34.865426 openbb-4.1.5/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    53519 2024-03-11 21:07:34.979144 openbb-4.1.5/openbb/package/economy.py
--rw-r--r--   0        0        0    12674 2024-03-11 21:07:34.900691 openbb-4.1.5/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    26227 2024-03-11 21:07:34.915271 openbb-4.1.5/openbb/package/equity.py
--rw-r--r--   0        0        0    19402 2024-03-11 21:07:34.906792 openbb-4.1.5/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2869 2024-03-11 21:07:34.859698 openbb-4.1.5/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    26106 2024-03-11 21:07:34.933060 openbb-4.1.5/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    26394 2024-03-11 21:07:34.898433 openbb-4.1.5/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   169275 2024-03-11 21:07:35.141679 openbb-4.1.5/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30641 2024-03-11 21:07:34.922080 openbb-4.1.5/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    27081 2024-03-11 21:07:34.929968 openbb-4.1.5/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3567 2024-03-11 21:07:34.887839 openbb-4.1.5/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    48531 2024-03-11 21:07:34.974868 openbb-4.1.5/openbb/package/etf.py
--rw-r--r--   0        0        0     4649 2024-03-11 21:07:34.892329 openbb-4.1.5/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    19969 2024-03-11 21:07:34.969639 openbb-4.1.5/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7155 2024-03-11 21:07:34.933100 openbb-4.1.5/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26900 2024-03-11 21:07:34.985632 openbb-4.1.5/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    11204 2024-03-11 21:07:34.961573 openbb-4.1.5/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11893 2024-03-11 21:07:34.962973 openbb-4.1.5/openbb/package/index.py
--rw-r--r--   0        0        0    15672 2024-03-11 21:07:34.951896 openbb-4.1.5/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-03-11 21:07:34.558200 openbb-4.1.5/openbb/package/regulators.py
--rw-r--r--   0        0        0    16562 2024-03-11 21:07:34.987309 openbb-4.1.5/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.654769 openbb-4.1.5/openbb/py.typed
--rw-r--r--   0        0        0     2862 2024-03-11 21:07:10.820234 openbb-4.1.5/pyproject.toml
--rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 openbb-4.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-03-13 16:36:51.521524 openbb-4.1.6/README.md
+-rw-r--r--   0        0        0     1440 2024-03-26 20:18:41.103946 openbb-4.1.6/openbb/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-01 14:32:42.894066 openbb-4.1.6/openbb/assets/extension_map.json
+-rw-r--r--   0        0        0  1053853 2024-04-01 14:32:46.283202 openbb-4.1.6/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2794 2024-04-01 14:32:46.440038 openbb-4.1.6/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0       50 2024-04-01 14:32:46.232307 openbb-4.1.6/openbb/package/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-01 14:32:47.372844 openbb-4.1.6/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6589 2024-04-01 14:32:47.385805 openbb-4.1.6/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    11777 2024-04-01 14:32:47.428143 openbb-4.1.6/openbb/package/currency.py
+-rw-r--r--   0        0        0     6481 2024-04-01 14:32:47.399407 openbb-4.1.6/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-04-01 14:32:47.372358 openbb-4.1.6/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12160 2024-04-01 14:32:47.398980 openbb-4.1.6/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    53423 2024-04-01 14:32:47.650745 openbb-4.1.6/openbb/package/economy.py
+-rw-r--r--   0        0        0    12674 2024-04-01 14:32:47.462113 openbb-4.1.6/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27673 2024-04-01 14:32:47.484070 openbb-4.1.6/openbb/package/equity.py
+-rw-r--r--   0        0        0    18754 2024-04-01 14:32:47.513789 openbb-4.1.6/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2869 2024-04-01 14:32:47.415091 openbb-4.1.6/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    26106 2024-04-01 14:32:47.538838 openbb-4.1.6/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    27199 2024-04-01 14:32:47.498714 openbb-4.1.6/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   169108 2024-04-01 14:32:47.847511 openbb-4.1.6/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30667 2024-04-01 14:32:47.539373 openbb-4.1.6/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26819 2024-04-01 14:32:47.536280 openbb-4.1.6/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3567 2024-04-01 14:32:47.450524 openbb-4.1.6/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    74985 2024-04-01 14:32:47.634556 openbb-4.1.6/openbb/package/etf.py
+-rw-r--r--   0        0        0     4649 2024-04-01 14:32:47.520201 openbb-4.1.6/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    20027 2024-04-01 14:32:47.621255 openbb-4.1.6/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7155 2024-04-01 14:32:47.560838 openbb-4.1.6/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26900 2024-04-01 14:32:47.652572 openbb-4.1.6/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    11204 2024-04-01 14:32:47.611377 openbb-4.1.6/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11919 2024-04-01 14:32:47.592563 openbb-4.1.6/openbb/package/index.py
+-rw-r--r--   0        0        0    15535 2024-04-01 14:32:47.599940 openbb-4.1.6/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-04-01 14:32:46.425844 openbb-4.1.6/openbb/package/regulators.py
+-rw-r--r--   0        0        0    16562 2024-04-01 14:32:47.634630 openbb-4.1.6/openbb/package/regulators_sec.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.750396 openbb-4.1.6/openbb/py.typed
+-rw-r--r--   0        0        0     2862 2024-04-01 14:39:04.199116 openbb-4.1.6/pyproject.toml
+-rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 openbb-4.1.6/PKG-INFO
```

### Comparing `openbb-4.1.5/README.md` & `openbb-4.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/__init__.py` & `openbb-4.1.6/openbb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import List, Optional, Union
 
 from openbb_core.app.static.app_factory import (
     BaseApp as _BaseApp,
     create_app as _create_app,
 )
 from openbb_core.app.static.package_builder import PackageBuilder as _PackageBuilder
+from openbb_core.app.static.reference_loader import ReferenceLoader as _ReferenceLoader
 
 _this_dir = Path(__file__).parent.resolve()
 
 
 def build(
     modules: Optional[Union[str, List[str]]] = None,
     lint: bool = True,
@@ -32,14 +33,15 @@
     verbose : bool, optional
         Enable/disable verbose mode
     """
     _PackageBuilder(_this_dir, lint, verbose).build(modules)
 
 
 _PackageBuilder(_this_dir).auto_build()
+_ReferenceLoader(_this_dir)
 
 try:
     # pylint: disable=import-outside-toplevel
     from openbb.package.__extensions__ import Extensions as _Extensions
 
     obb: Union[_BaseApp, _Extensions] = _create_app(_Extensions)  # type: ignore
     sdk = obb
```

### Comparing `openbb-4.1.5/openbb/package/__extensions__.py` & `openbb-4.1.6/openbb/package/__extensions__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,37 +16,37 @@
     /etf
     /fixedincome
     /index
     /news
     /regulators
 
 Extensions:
-    - commodity@1.0.1
-    - crypto@1.1.3
-    - currency@1.1.3
-    - derivatives@1.1.3
-    - economy@1.1.3
-    - equity@1.1.3
-    - etf@1.1.3
-    - fixedincome@1.1.3
-    - index@1.1.3
-    - news@1.1.3
-    - regulators@1.1.3
+    - commodity@1.0.2
+    - crypto@1.1.4
+    - currency@1.1.4
+    - derivatives@1.1.4
+    - economy@1.1.4
+    - equity@1.1.4
+    - etf@1.1.4
+    - fixedincome@1.1.4
+    - index@1.1.4
+    - news@1.1.4
+    - regulators@1.1.4
 
-    - benzinga@1.1.3
-    - federal_reserve@1.1.3
-    - fmp@1.1.3
-    - fred@1.1.3
-    - intrinio@1.1.3
-    - oecd@1.1.3
-    - polygon@1.1.3
-    - sec@1.1.3
-    - tiingo@1.1.3
-    - tradingeconomics@1.1.3
-    - yfinance@1.1.3    """
+    - benzinga@1.1.4
+    - federal_reserve@1.1.4
+    - fmp@1.1.4
+    - fred@1.1.4
+    - intrinio@1.1.4
+    - oecd@1.1.4
+    - polygon@1.1.4
+    - sec@1.1.4
+    - tiingo@1.1.4
+    - tradingeconomics@1.1.4
+    - yfinance@1.1.4    """
     # fmt: on
 
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @property
     def crypto(self):
```

### Comparing `openbb-4.1.5/openbb/package/crypto.py` & `openbb-4.1.6/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/crypto_price.py` & `openbb-4.1.6/openbb/package/crypto_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple items allowed for provider(s): fmp, polygon, tiingo, yfinance."
+                description="Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
@@ -50,15 +50,15 @@
         **kwargs
     ) -> OBBject:
         """Get historical price data for cryptocurrency pair(s) within a provider.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple items allowed for provider(s): fmp, polygon, tiingo, yfinance.
+            Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         provider : Optional[Literal['fmp', 'polygon', 'tiingo', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
@@ -135,15 +135,15 @@
                 },
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": [
                             "fmp",
                             "polygon",
                             "tiingo",
                             "yfinance",
                         ]
```

### Comparing `openbb-4.1.5/openbb/package/currency.py` & `openbb-4.1.6/openbb/package/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,25 +150,25 @@
     @exception_handler
     @validate
     def snapshots(
         self,
         base: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="The base currency symbol. Multiple items allowed for provider(s): fmp."
+                description="The base currency symbol. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ] = "usd",
         quote_type: Annotated[
             Literal["direct", "indirect"],
             OpenBBCustomParameter(
                 description="Whether the quote is direct or indirect. Selecting 'direct' will return the exchange rate as the amount of domestic currency required to buy one unit of the foreign currency. Selecting 'indirect' (default) will return the exchange rate as the amount of foreign currency required to buy one unit of the domestic currency."
             ),
         ] = "indirect",
         counter_currencies: Annotated[
-            Union[str, List[str], None],
+            Union[List[str], str, None],
             OpenBBCustomParameter(
                 description="An optional list of counter currency symbols to filter for. None returns all."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
             OpenBBCustomParameter(
@@ -178,18 +178,18 @@
         **kwargs
     ) -> OBBject:
         """Snapshots of currency exchange rates from an indirect or direct perspective of a base currency.
 
         Parameters
         ----------
         base : Union[str, List[str]]
-            The base currency symbol. Multiple items allowed for provider(s): fmp.
+            The base currency symbol. Multiple comma separated items allowed for provider(s): fmp.
         quote_type : Literal['direct', 'indirect']
             Whether the quote is direct or indirect. Selecting 'direct' will return the exchange rate as the amount of domestic currency required to buy one unit of the foreign currency. Selecting 'indirect' (default) will return the exchange rate as the amount of foreign currency required to buy one unit of the domestic currency.
-        counter_currencies : Union[str, List[str], None]
+        counter_currencies : Union[List[str], str, None]
             An optional list of counter currency symbols to filter for. None returns all.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
@@ -261,10 +261,10 @@
                 },
                 standard_params={
                     "base": base,
                     "quote_type": quote_type,
                     "counter_currencies": counter_currencies,
                 },
                 extra_params=kwargs,
-                extra_info={"base": {"multiple_items_allowed": ["fmp"]}},
+                info={"base": {"multiple_items_allowed": ["fmp"]}},
             )
         )
```

### Comparing `openbb-4.1.5/openbb/package/currency_price.py` & `openbb-4.1.6/openbb/package/currency_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple items allowed for provider(s): fmp, polygon, tiingo, yfinance."
+                description="Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
@@ -57,15 +57,15 @@
         helping analysts, traders, and economists understand currency performance,
         evaluate economic health, and make predictions about future movements.
 
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple items allowed for provider(s): fmp, polygon, tiingo, yfinance.
+            Symbol to get data for. Can use CURR1-CURR2 or CURR1CURR2 format. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         provider : Optional[Literal['fmp', 'polygon', 'tiingo', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
@@ -138,15 +138,15 @@
                 },
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": [
                             "fmp",
                             "polygon",
                             "tiingo",
                             "yfinance",
                         ]
```

### Comparing `openbb-4.1.5/openbb/package/derivatives.py` & `openbb-4.1.6/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/derivatives_options.py` & `openbb-4.1.6/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/economy.py` & `openbb-4.1.6/openbb/package/economy.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         provider : Optional[Literal['fmp', 'tradingeconomics']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
         country : Optional[str]
-            Country of the event. Multiple items allowed. (provider: tradingeconomics)
+            Country of the event. Multiple comma separated items allowed. (provider: tradingeconomics)
         importance : Optional[Literal['Low', 'Medium', 'High']]
             Importance of the event. (provider: tradingeconomics)
         group : Optional[Literal['interest rate', 'inflation', 'bonds', 'consumer', 'gdp', 'government', 'housing', 'labour', 'markets', 'money', 'prices', 'trade', 'business']]
             Grouping of events (provider: tradingeconomics)
 
         Returns
         -------
@@ -148,14 +148,15 @@
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
+                info={"country": {"multiple_items_allowed": ["tradingeconomics"]}},
             )
         )
 
     @exception_handler
     @validate
     def composite_leading_indicator(
         self,
@@ -248,15 +249,15 @@
     @exception_handler
     @validate
     def cpi(
         self,
         country: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="The country to get data. Multiple items allowed for provider(s): fred."
+                description="The country to get data. Multiple comma separated items allowed for provider(s): fred."
             ),
             OpenBBCustomChoices(
                 choices=[
                     "australia",
                     "austria",
                     "belgium",
                     "brazil",
@@ -347,15 +348,15 @@
         **kwargs
     ) -> OBBject:
         """Consumer Price Index (CPI).  Returns either the rescaled index value, or a rate of change (inflation).
 
         Parameters
         ----------
         country : Union[str, List[str]]
-            The country to get data. Multiple items allowed for provider(s): fred.
+            The country to get data. Multiple comma separated items allowed for provider(s): fred.
         units : Literal['growth_previous', 'growth_same', 'index_2015']
             The unit of measurement for the data.
             Options:
             - `growth_previous`: Percent growth from the previous period.
               If monthly data, this is month-over-month, etc
             - `growth_same`: Percent growth from the same period in the previous year.
               If looking at monthly data, this would be year-over-year, etc.
@@ -416,27 +417,24 @@
                     "units": units,
                     "frequency": frequency,
                     "harmonized": harmonized,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
-                extra_info={"country": {"multiple_items_allowed": ["fred"]}},
+                info={"country": {"multiple_items_allowed": ["fred"]}},
             )
         )
 
     @exception_handler
     @validate
     def fred_regional(
         self,
         symbol: Annotated[
-            Union[str, List[str]],
-            OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fred."
-            ),
+            str, OpenBBCustomParameter(description="Symbol to get data for.")
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
         ] = None,
@@ -460,16 +458,16 @@
     ) -> OBBject:
         """Query the Geo Fred API for regional economic data by series group.
         The series group ID is found by using `fred_search` and the `series_id` parameter.
 
 
         Parameters
         ----------
-        symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fred.
+        symbol : str
+            Symbol to get data for.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         limit : Optional[int]
             The number of data entries to return.
         provider : Optional[Literal['fred']]
@@ -575,15 +573,14 @@
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["fred"]}},
             )
         )
 
     @exception_handler
     @validate
     def fred_search(
         self,
@@ -713,15 +710,15 @@
     @exception_handler
     @validate
     def fred_series(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fred."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fred."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
@@ -745,15 +742,15 @@
         **kwargs
     ) -> OBBject:
         """Get data by series ID from FRED.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fred.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fred.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         limit : Optional[int]
             The number of data entries to return.
         provider : Optional[Literal['fred', 'intrinio']]
@@ -849,15 +846,15 @@
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["fred"]}},
+                info={"symbol": {"multiple_items_allowed": ["fred"]}},
             )
         )
 
     @property
     def gdp(self):
         # pylint: disable=import-outside-toplevel
         from . import economy_gdp
```

### Comparing `openbb-4.1.5/openbb/package/economy_gdp.py` & `openbb-4.1.6/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/equity.py` & `openbb-4.1.6/openbb/package/equity.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,38 +73,40 @@
         )
 
     @exception_handler
     @validate
     def market_snapshots(
         self,
         provider: Annotated[
-            Optional[Literal["fmp", "polygon"]],
+            Optional[Literal["fmp", "intrinio", "polygon"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get an updated equity market snapshot. This includes price data for thousands of stocks.
 
         Parameters
         ----------
-        provider : Optional[Literal['fmp', 'polygon']]
+        provider : Optional[Literal['fmp', 'intrinio', 'polygon']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
         market : Literal['amex', 'ams', 'ase', 'asx', 'ath', 'bme', 'bru', 'bud', 'bue', 'cai', 'cnq', 'cph', 'dfm', 'doh', 'etf', 'euronext', 'hel', 'hkse', 'ice', 'iob', 'ist', 'jkt', 'jnb', 'jpx', 'kls', 'koe', 'ksc', 'kuw', 'lse', 'mex', 'mutual_fund', 'nasdaq', 'neo', 'nse', 'nyse', 'nze', 'osl', 'otc', 'pnk', 'pra', 'ris', 'sao', 'sau', 'set', 'sgo', 'shh', 'shz', 'six', 'sto', 'tai', 'tlv', 'tsx', 'two', 'vie', 'wse', 'xetra']
             The market to fetch data for. (provider: fmp)
+        date : Optional[Union[datetime.date, datetime.datetime, str]]
+            The date of the data. Can be a datetime or an ISO datetime string. Historical data appears to go back to mid-June 2022. Example: '2024-03-08T12:15:00+0400' (provider: intrinio)
 
         Returns
         -------
         OBBject
             results : List[MarketSnapshots]
                 Serializable results.
-            provider : Optional[Literal['fmp', 'polygon']]
+            provider : Optional[Literal['fmp', 'intrinio', 'polygon']]
                 Provider name.
             warnings : Optional[List[Warning_]]
                 List of warnings.
             chart : Optional[Chart]
                 Chart object.
             extra : Dict[str, Any]
                 Extra info.
@@ -126,15 +128,16 @@
         prev_close : Optional[float]
             The previous close price.
         change : Optional[float]
             The change in price from the previous close.
         change_percent : Optional[float]
             The change in price from the previous close, as a normalized percent.
         last_price : Optional[float]
-            The last price of the stock. (provider: fmp)
+            The last price of the stock. (provider: fmp);
+            The last trade price. (provider: intrinio)
         last_price_timestamp : Optional[Union[date, datetime]]
             The timestamp of the last price. (provider: fmp)
         ma50 : Optional[float]
             The 50-day moving average. (provider: fmp)
         ma200 : Optional[float]
             The 200-day moving average. (provider: fmp)
         year_high : Optional[float]
@@ -153,14 +156,35 @@
             Number of shares outstanding. (provider: fmp)
         name : Optional[str]
             The company name associated with the symbol. (provider: fmp)
         exchange : Optional[str]
             The exchange of the stock. (provider: fmp)
         earnings_date : Optional[Union[date, datetime]]
             The upcoming earnings announcement date. (provider: fmp)
+        last_size : Optional[int]
+            The last trade size. (provider: intrinio)
+        last_volume : Optional[int]
+            The last trade volume. (provider: intrinio)
+        last_trade_timestamp : Optional[datetime]
+            The timestamp of the last trade. (provider: intrinio);
+            The last trade timestamp. (provider: polygon)
+        bid_size : Optional[int]
+            The size of the last bid price. Bid price and size is not always available. (provider: intrinio);
+            The current bid size. (provider: polygon)
+        bid_price : Optional[float]
+            The last bid price. Bid price and size is not always available. (provider: intrinio)
+        ask_price : Optional[float]
+            The last ask price. Ask price and size is not always available. (provider: intrinio)
+        ask_size : Optional[int]
+            The size of the last ask price. Ask price and size is not always available. (provider: intrinio);
+            The current ask size. (provider: polygon)
+        last_bid_timestamp : Optional[datetime]
+            The timestamp of the last bid price. Bid price and size is not always available. (provider: intrinio)
+        last_ask_timestamp : Optional[datetime]
+            The timestamp of the last ask price. Ask price and size is not always available. (provider: intrinio)
         vwap : Optional[float]
             The volume weighted average price of the stock on the current trading day. (provider: polygon)
         prev_open : Optional[float]
             The previous trading session opening price. (provider: polygon)
         prev_high : Optional[float]
             The previous trading session high price. (provider: polygon)
         prev_low : Optional[float]
@@ -169,47 +193,41 @@
             The previous trading session volume. (provider: polygon)
         prev_vwap : Optional[float]
             The previous trading session VWAP. (provider: polygon)
         last_updated : Optional[datetime]
             The last time the data was updated. (provider: polygon)
         bid : Optional[float]
             The current bid price. (provider: polygon)
-        bid_size : Optional[int]
-            The current bid size. (provider: polygon)
-        ask_size : Optional[int]
-            The current ask size. (provider: polygon)
         ask : Optional[float]
             The current ask price. (provider: polygon)
         quote_timestamp : Optional[datetime]
             The timestamp of the last quote. (provider: polygon)
         last_trade_price : Optional[float]
             The last trade price. (provider: polygon)
         last_trade_size : Optional[int]
             The last trade size. (provider: polygon)
         last_trade_conditions : Optional[List[int]]
             The last trade condition codes. (provider: polygon)
         last_trade_exchange : Optional[int]
             The last trade exchange ID code. (provider: polygon)
-        last_trade_timestamp : Optional[datetime]
-            The last trade timestamp. (provider: polygon)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.market_snapshots(provider='fmp')
         """  # noqa: E501
 
         return self._run(
             "/equity/market_snapshots",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/market_snapshots",
-                        ("fmp", "polygon"),
+                        ("fmp", "intrinio", "polygon"),
                     )
                 },
                 standard_params={},
                 extra_params=kwargs,
             )
         )
 
@@ -232,15 +250,15 @@
     @exception_handler
     @validate
     def profile(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio, yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -248,15 +266,15 @@
         **kwargs
     ) -> OBBject:
         """Get general information about a company. This includes company name, industry, sector and price data.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio, yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance.
         provider : Optional[Literal['fmp', 'intrinio', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
         -------
@@ -412,15 +430,15 @@
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
                     }
                 },
             )
         )
```

### Comparing `openbb-4.1.5/openbb/package/equity_calendar.py` & `openbb-4.1.6/openbb/package/equity_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,87 +291,52 @@
         CalendarIpo
         -----------
         symbol : Optional[str]
             Symbol representing the entity requested in the data.
         ipo_date : Optional[date]
             The date of the IPO, when the stock first trades on a major exchange.
         status : Optional[Literal['upcoming', 'priced', 'withdrawn']]
-
-                    The status of the IPO. Upcoming IPOs have not taken place yet but are expected to.
-                    Priced IPOs have taken place.
-                    Withdrawn IPOs were expected to take place, but were subsequently withdrawn and did not take place
-                 (provider: intrinio)
+            The status of the IPO. Upcoming IPOs have not taken place yet but are expected to. Priced IPOs have taken place. Withdrawn IPOs were expected to take place, but were subsequently withdrawn. (provider: intrinio)
         exchange : Optional[str]
-
-                    The acronym of the stock exchange that the company is going to trade publicly on.
-                    Typically NYSE or NASDAQ.
-                 (provider: intrinio)
+            The acronym of the stock exchange that the company is going to trade publicly on. Typically NYSE or NASDAQ. (provider: intrinio)
         offer_amount : Optional[float]
             The total dollar amount of shares offered in the IPO. Typically this is share price * share count (provider: intrinio)
         share_price : Optional[float]
             The price per share at which the IPO was offered. (provider: intrinio)
         share_price_lowest : Optional[float]
-
-                    The expected lowest price per share at which the IPO will be offered.
-                    Before an IPO is priced, companies typically provide a range of prices per share at which
-                    they expect to offer the IPO (typically available for upcoming IPOs).
-                 (provider: intrinio)
+            The expected lowest price per share at which the IPO will be offered. Before an IPO is priced, companies typically provide a range of prices per share at which they expect to offer the IPO (typically available for upcoming IPOs). (provider: intrinio)
         share_price_highest : Optional[float]
-
-                    The expected highest price per share at which the IPO will be offered.
-                    Before an IPO is priced, companies typically provide a range of prices per share at which
-                    they expect to offer the IPO (typically available for upcoming IPOs).
-                 (provider: intrinio)
+            The expected highest price per share at which the IPO will be offered. Before an IPO is priced, companies typically provide a range of prices per share at which they expect to offer the IPO (typically available for upcoming IPOs). (provider: intrinio)
         share_count : Optional[int]
             The number of shares offered in the IPO. (provider: intrinio)
         share_count_lowest : Optional[int]
-
-                    The expected lowest number of shares that will be offered in the IPO. Before an IPO is priced,
-                    companies typically provide a range of shares that they expect to offer in the IPO
-                    (typically available for upcoming IPOs).
-                 (provider: intrinio)
+            The expected lowest number of shares that will be offered in the IPO. Before an IPO is priced, companies typically provide a range of shares that they expect to offer in the IPO (typically available for upcoming IPOs). (provider: intrinio)
         share_count_highest : Optional[int]
-
-                    The expected highest number of shares that will be offered in the IPO. Before an IPO is priced,
-                    companies typically provide a range of shares that they expect to offer in the IPO
-                    (typically available for upcoming IPOs).
-                 (provider: intrinio)
+            The expected highest number of shares that will be offered in the IPO. Before an IPO is priced, companies typically provide a range of shares that they expect to offer in the IPO (typically available for upcoming IPOs). (provider: intrinio)
         announcement_url : Optional[str]
             The URL to the company's announcement of the IPO (provider: intrinio)
         sec_report_url : Optional[str]
-
-                    The URL to the company's S-1, S-1/A, F-1, or F-1/A SEC filing,
-                    which is required to be filed before an IPO takes place.
-                 (provider: intrinio)
+            The URL to the company's S-1, S-1/A, F-1, or F-1/A SEC filing, which is required to be filed before an IPO takes place. (provider: intrinio)
         open_price : Optional[float]
             The opening price at the beginning of the first trading day (only available for priced IPOs). (provider: intrinio)
         close_price : Optional[float]
             The closing price at the end of the first trading day (only available for priced IPOs). (provider: intrinio)
         volume : Optional[int]
             The volume at the end of the first trading day (only available for priced IPOs). (provider: intrinio)
         day_change : Optional[float]
-
-                    The percentage change between the open price and the close price on the first trading day
-                    (only available for priced IPOs).
-                 (provider: intrinio)
+            The percentage change between the open price and the close price on the first trading day (only available for priced IPOs). (provider: intrinio)
         week_change : Optional[float]
-
-                    The percentage change between the open price on the first trading day and the close price approximately
-                    a week after the first trading day (only available for priced IPOs).
-                 (provider: intrinio)
+            The percentage change between the open price on the first trading day and the close price approximately a week after the first trading day (only available for priced IPOs). (provider: intrinio)
         month_change : Optional[float]
-
-                    The percentage change between the open price on the first trading day and the close price approximately
-                    a month after the first trading day (only available for priced IPOs).
-                 (provider: intrinio)
+            The percentage change between the open price on the first trading day and the close price approximately a month after the first trading day (only available for priced IPOs). (provider: intrinio)
         id : Optional[str]
             The Intrinio ID of the IPO. (provider: intrinio)
-        company : Optional[openbb_intrinio.utils.references.IntrinioCompany]
+        company : Optional[IntrinioCompany]
             The company that is going public via the IPO. (provider: intrinio)
-        security : Optional[openbb_intrinio.utils.references.IntrinioSecurity]
+        security : Optional[IntrinioSecurity]
             The primary Security for the Company that is going public via the IPO (provider: intrinio)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.calendar.ipo(provider='intrinio')
         >>> # Get all IPOs available.
```

### Comparing `openbb-4.1.5/openbb/package/equity_compare.py` & `openbb-4.1.6/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/equity_discovery.py` & `openbb-4.1.6/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/equity_estimates.py` & `openbb-4.1.6/openbb/package/equity_estimates.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,55 +22,55 @@
         return self.__doc__ or ""
 
     @exception_handler
     @validate
     def analyst_search(
         self,
         analyst_name: Annotated[
-            Optional[str],
+            Union[str, None, List[Optional[str]]],
             OpenBBCustomParameter(
-                description="A comma separated list of analyst names to bring back. Omitting will bring back all available analysts."
+                description="Analyst names to return. Omitting will return all available analysts. Multiple comma separated items allowed for provider(s): benzinga."
             ),
         ] = None,
         firm_name: Annotated[
-            Optional[str],
+            Union[str, None, List[Optional[str]]],
             OpenBBCustomParameter(
-                description="A comma separated list of firm names to bring back. Omitting will bring back all available firms."
+                description="Firm names to return. Omitting will return all available firms. Multiple comma separated items allowed for provider(s): benzinga."
             ),
         ] = None,
         provider: Annotated[
             Optional[Literal["benzinga"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'benzinga' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Search for specific analysts and get their forecast track record.
 
         Parameters
         ----------
-        analyst_name : Optional[str]
-            A comma separated list of analyst names to bring back. Omitting will bring back all available analysts.
-        firm_name : Optional[str]
-            A comma separated list of firm names to bring back. Omitting will bring back all available firms.
+        analyst_name : Union[str, None, List[Optional[str]]]
+            Analyst names to return. Omitting will return all available analysts. Multiple comma separated items allowed for provider(s): benzinga.
+        firm_name : Union[str, None, List[Optional[str]]]
+            Firm names to return. Omitting will return all available firms. Multiple comma separated items allowed for provider(s): benzinga.
         provider : Optional[Literal['benzinga']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'benzinga' if there is
             no default.
-        analyst_ids : Optional[Union[str, List[str]]]
-            A comma separated list of analyst IDs to bring back. (provider: benzinga)
-        firm_ids : Optional[Union[str, List[str]]]
-            A comma separated list of firm IDs to bring back. (provider: benzinga)
+        analyst_ids : Optional[str]
+            List of analyst IDs to return. Multiple comma separated items allowed. (provider: benzinga)
+        firm_ids : Optional[str]
+            Firm IDs to return. Multiple comma separated items allowed. (provider: benzinga)
         limit : Optional[int]
             Number of results returned. Limit 1000. (provider: benzinga)
         page : Optional[int]
             Page offset. For optimization, performance and technical reasons, page offsets are limited from 0 - 100000. Limit the query results by other parameters such as date. (provider: benzinga)
-        fields : Optional[Union[str, List[str]]]
-            Comma-separated list of fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields. (provider: benzinga)
+        fields : Optional[str]
+            Fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields. Multiple comma separated items allowed. (provider: benzinga)
 
         Returns
         -------
         OBBject
             results : List[AnalystSearch]
                 Serializable results.
             provider : Optional[Literal['benzinga']]
@@ -191,25 +191,32 @@
                     )
                 },
                 standard_params={
                     "analyst_name": analyst_name,
                     "firm_name": firm_name,
                 },
                 extra_params=kwargs,
+                info={
+                    "analyst_name": {"multiple_items_allowed": ["benzinga"]},
+                    "firm_name": {"multiple_items_allowed": ["benzinga"]},
+                    "analyst_ids": {"multiple_items_allowed": ["benzinga"]},
+                    "firm_ids": {"multiple_items_allowed": ["benzinga"]},
+                    "fields": {"multiple_items_allowed": ["benzinga"]},
+                },
             )
         )
 
     @exception_handler
     @validate
     def consensus(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "yfinance"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -217,24 +224,24 @@
         **kwargs
     ) -> OBBject:
         """Get consensus price target and recommendation.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, yfinance.
         provider : Optional[Literal['fmp', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
         -------
         OBBject
-            results : Union[List[PriceTargetConsensus], PriceTargetConsensus]
+            results : List[PriceTargetConsensus]
                 Serializable results.
             provider : Optional[Literal['fmp', 'yfinance']]
                 Provider name.
             warnings : Optional[List[Warning_]]
                 List of warnings.
             chart : Optional[Chart]
                 Chart object.
@@ -281,55 +288,50 @@
                         ("fmp", "yfinance"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["yfinance"]}},
+                info={"symbol": {"multiple_items_allowed": ["fmp", "yfinance"]}},
             )
         )
 
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
-            str, OpenBBCustomParameter(description="Symbol to get data for.")
+            Union[str, List[str]],
+            OpenBBCustomParameter(
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
+            ),
         ],
-        period: Annotated[
-            Literal["quarter", "annual"],
-            OpenBBCustomParameter(description="Time period of the data to return."),
-        ] = "annual",
-        limit: Annotated[
-            int,
-            OpenBBCustomParameter(description="The number of data entries to return."),
-        ] = 30,
         provider: Annotated[
             Optional[Literal["fmp"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get historical analyst estimates for earnings and revenue.
 
         Parameters
         ----------
-        symbol : str
-            Symbol to get data for.
-        period : Literal['quarter', 'annual']
-            Time period of the data to return.
-        limit : int
-            The number of data entries to return.
+        symbol : Union[str, List[str]]
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
+        period : Literal['quarter', 'annual']
+            Time period of the data to return. (provider: fmp)
+        limit : Optional[int]
+            The number of data entries to return. (provider: fmp)
 
         Returns
         -------
         OBBject
             results : List[AnalystEstimates]
                 Serializable results.
             provider : Optional[Literal['fmp']]
@@ -343,53 +345,53 @@
 
         AnalystEstimates
         ----------------
         symbol : str
             Symbol representing the entity requested in the data.
         date : date
             The date of the data.
-        estimated_revenue_low : int
+        estimated_revenue_low : Optional[int]
             Estimated revenue low.
-        estimated_revenue_high : int
+        estimated_revenue_high : Optional[int]
             Estimated revenue high.
-        estimated_revenue_avg : int
+        estimated_revenue_avg : Optional[int]
             Estimated revenue average.
-        estimated_ebitda_low : int
+        estimated_sga_expense_low : Optional[int]
+            Estimated SGA expense low.
+        estimated_sga_expense_high : Optional[int]
+            Estimated SGA expense high.
+        estimated_sga_expense_avg : Optional[int]
+            Estimated SGA expense average.
+        estimated_ebitda_low : Optional[int]
             Estimated EBITDA low.
-        estimated_ebitda_high : int
+        estimated_ebitda_high : Optional[int]
             Estimated EBITDA high.
-        estimated_ebitda_avg : int
+        estimated_ebitda_avg : Optional[int]
             Estimated EBITDA average.
-        estimated_ebit_low : int
+        estimated_ebit_low : Optional[int]
             Estimated EBIT low.
-        estimated_ebit_high : int
+        estimated_ebit_high : Optional[int]
             Estimated EBIT high.
-        estimated_ebit_avg : int
+        estimated_ebit_avg : Optional[int]
             Estimated EBIT average.
-        estimated_net_income_low : int
+        estimated_net_income_low : Optional[int]
             Estimated net income low.
-        estimated_net_income_high : int
+        estimated_net_income_high : Optional[int]
             Estimated net income high.
-        estimated_net_income_avg : int
+        estimated_net_income_avg : Optional[int]
             Estimated net income average.
-        estimated_sga_expense_low : int
-            Estimated SGA expense low.
-        estimated_sga_expense_high : int
-            Estimated SGA expense high.
-        estimated_sga_expense_avg : int
-            Estimated SGA expense average.
-        estimated_eps_avg : float
+        estimated_eps_avg : Optional[float]
             Estimated EPS average.
-        estimated_eps_high : float
+        estimated_eps_high : Optional[float]
             Estimated EPS high.
-        estimated_eps_low : float
+        estimated_eps_low : Optional[float]
             Estimated EPS low.
-        number_analyst_estimated_revenue : int
+        number_analyst_estimated_revenue : Optional[int]
             Number of analysts who estimated revenue.
-        number_analysts_estimated_eps : int
+        number_analysts_estimated_eps : Optional[int]
             Number of analysts who estimated EPS.
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.estimates.historical(symbol='AAPL', provider='fmp')
         """  # noqa: E501
@@ -402,29 +404,28 @@
                         provider,
                         "/equity/estimates/historical",
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
-                    "period": period,
-                    "limit": limit,
                 },
                 extra_params=kwargs,
+                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
             )
         )
 
     @exception_handler
     @validate
     def price_target(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): benzinga."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): benzinga, fmp."
             ),
         ] = None,
         limit: Annotated[
             int,
             OpenBBCustomParameter(description="The number of data entries to return."),
         ] = 200,
         provider: Annotated[
@@ -436,15 +437,15 @@
         **kwargs
     ) -> OBBject:
         """Get analyst price targets by company.
 
         Parameters
         ----------
         symbol : Union[str, None, List[Optional[str]]]
-            Symbol to get data for. Multiple items allowed for provider(s): benzinga.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): benzinga, fmp.
         limit : int
             The number of data entries to return.
         provider : Optional[Literal['benzinga', 'fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'benzinga' if there is
             no default.
         page : Optional[int]
@@ -457,19 +458,19 @@
             End date of the data, in YYYY-MM-DD format. (provider: benzinga)
         updated : Optional[Union[datetime.date, int]]
             Records last Updated Unix timestamp (UTC). This will force the sort order to be Greater Than or Equal to the timestamp indicated. The date can be a date string or a Unix timestamp. The date string must be in the format of YYYY-MM-DD. (provider: benzinga)
         importance : Optional[int]
             Importance level to filter by. Uses Greater Than or Equal To the importance indicated (provider: benzinga)
         action : Optional[Literal['downgrades', 'maintains', 'reinstates', 'reiterates', 'upgrades', 'assumes', 'initiates', 'terminates', 'removes', 'suspends', 'firm_dissolved']]
             Filter by a specific action_company. (provider: benzinga)
-        analyst_ids : Optional[Union[str, List[str]]]
+        analyst_ids : Optional[Union[List[str], str]]
             Comma-separated list of analyst (person) IDs. Omitting will bring back all available analysts. (provider: benzinga)
-        firm_ids : Optional[Union[str, List[str]]]
+        firm_ids : Optional[Union[List[str], str]]
             Comma-separated list of firm IDs. (provider: benzinga)
-        fields : Optional[Union[str, List[str]]]
+        fields : Optional[Union[List[str], str]]
             Comma-separated list of fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields. (provider: benzinga)
         with_grade : bool
             Include upgrades and downgrades in the response. (provider: fmp)
 
         Returns
         -------
         OBBject
@@ -562,10 +563,10 @@
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["benzinga"]}},
+                info={"symbol": {"multiple_items_allowed": ["benzinga", "fmp"]}},
             )
         )
```

### Comparing `openbb-4.1.5/openbb/package/equity_fundamental.py` & `openbb-4.1.6/openbb/package/equity_fundamental.py`

 * *Files 2% similar despite different names*

```diff
@@ -1321,21 +1321,21 @@
     @exception_handler
     @validate
     def historical_attributes(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): intrinio."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         tag: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Intrinio data tag ID or code. Multiple items allowed for provider(s): intrinio."
+                description="Intrinio data tag ID or code. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
@@ -1371,17 +1371,17 @@
         **kwargs
     ) -> OBBject:
         """Get the historical values of a data tag from Intrinio.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): intrinio.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio.
         tag : Union[str, List[str]]
-            Intrinio data tag ID or code. Multiple items allowed for provider(s): intrinio.
+            Intrinio data tag ID or code. Multiple comma separated items allowed for provider(s): intrinio.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         frequency : Optional[Literal['daily', 'weekly', 'monthly', 'quarterly', 'year...
             The frequency of the data.
         limit : Optional[int]
@@ -1443,15 +1443,15 @@
                     "end_date": end_date,
                     "frequency": frequency,
                     "limit": limit,
                     "tag_type": tag_type,
                     "sort": sort,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {"multiple_items_allowed": ["intrinio"]},
                     "tag": {"multiple_items_allowed": ["intrinio"]},
                 },
             )
         )
 
     @exception_handler
@@ -1582,20 +1582,20 @@
             extra : Dict[str, Any]
                 Extra info.
 
         HistoricalSplits
         ----------------
         date : date
             The date of the data.
-        label : str
-            Label of the historical stock splits.
-        numerator : float
-            Numerator of the historical stock splits.
-        denominator : float
-            Denominator of the historical stock splits.
+        numerator : Optional[float]
+            Numerator of the split.
+        denominator : Optional[float]
+            Denominator of the split.
+        split_ratio : Optional[str]
+            Split ratio.
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.fundamental.historical_splits(symbol='AAPL', provider='fmp')
         """  # noqa: E501
 
@@ -1988,15 +1988,15 @@
             str, OpenBBCustomParameter(description="Symbol to get data for.")
         ],
         limit: Annotated[
             int,
             OpenBBCustomParameter(description="The number of data entries to return."),
         ] = 10,
         period: Annotated[
-            Literal["quarter", "annual"],
+            Literal["annual", "quarter"],
             OpenBBCustomParameter(description="Time period of the data to return."),
         ] = "annual",
         provider: Annotated[
             Optional[Literal["fmp"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -2007,15 +2007,15 @@
 
         Parameters
         ----------
         symbol : str
             Symbol to get data for.
         limit : int
             The number of data entries to return.
-        period : Literal['quarter', 'annual']
+        period : Literal['annual', 'quarter']
             Time period of the data to return.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
@@ -2122,21 +2122,21 @@
     @exception_handler
     @validate
     def latest_attributes(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): intrinio."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         tag: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Intrinio data tag ID or code. Multiple items allowed for provider(s): intrinio."
+                description="Intrinio data tag ID or code. Multiple comma separated items allowed for provider(s): intrinio."
             ),
         ],
         provider: Annotated[
             Optional[Literal["intrinio"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'intrinio' if there is\n    no default."
             ),
@@ -2144,17 +2144,17 @@
         **kwargs
     ) -> OBBject:
         """Get the latest value of a data tag from Intrinio.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): intrinio.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): intrinio.
         tag : Union[str, List[str]]
-            Intrinio data tag ID or code. Multiple items allowed for provider(s): intrinio.
+            Intrinio data tag ID or code. Multiple comma separated items allowed for provider(s): intrinio.
         provider : Optional[Literal['intrinio']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'intrinio' if there is
             no default.
 
         Returns
         -------
@@ -2196,15 +2196,15 @@
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "tag": tag,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {"multiple_items_allowed": ["intrinio"]},
                     "tag": {"multiple_items_allowed": ["intrinio"]},
                 },
             )
         )
 
     @exception_handler
@@ -2294,51 +2294,37 @@
     @exception_handler
     @validate
     def management_compensation(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
-        start_date: Annotated[
-            Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="Start date of the data, in YYYY-MM-DD format."
-            ),
-        ] = None,
-        end_date: Annotated[
-            Union[datetime.date, None, str],
-            OpenBBCustomParameter(
-                description="End date of the data, in YYYY-MM-DD format."
-            ),
-        ] = None,
         provider: Annotated[
             Optional[Literal["fmp"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
         """Get executive management team compensation for a given company over time.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp.
-        start_date : Union[datetime.date, None, str]
-            Start date of the data, in YYYY-MM-DD format.
-        end_date : Union[datetime.date, None, str]
-            End date of the data, in YYYY-MM-DD format.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
+        year : Optional[int]
+            Year of the compensation. (provider: fmp)
 
         Returns
         -------
         OBBject
             results : List[ExecutiveCompensation]
                 Serializable results.
             provider : Optional[Literal['fmp']]
@@ -2352,36 +2338,40 @@
 
         ExecutiveCompensation
         ---------------------
         symbol : str
             Symbol representing the entity requested in the data.
         cik : Optional[str]
             Central Index Key (CIK) for the requested entity.
-        filing_date : date
-            Date of the filing.
-        accepted_date : datetime
-            Date the filing was accepted.
-        name_and_position : str
-            Name and position of the executive.
-        year : int
+        company_name : Optional[str]
+            The name of the company.
+        industry : Optional[str]
+            The industry of the company.
+        year : Optional[int]
             Year of the compensation.
-        salary : float
-            Salary of the executive.
-        bonus : float
-            Bonus of the executive.
-        stock_award : float
-            Stock award of the executive.
-        incentive_plan_compensation : float
-            Incentive plan compensation of the executive.
-        all_other_compensation : float
-            All other compensation of the executive.
-        total : float
-            Total compensation of the executive.
-        url : str
-            URL of the filing data.
+        name_and_position : Optional[str]
+            Name and position.
+        salary : Optional[Annotated[float, Ge(ge=0)]]
+            Salary.
+        bonus : Optional[Annotated[float, Ge(ge=0)]]
+            Bonus payments.
+        stock_award : Optional[Annotated[float, Ge(ge=0)]]
+            Stock awards.
+        incentive_plan_compensation : Optional[Annotated[float, Ge(ge=0)]]
+            Incentive plan compensation.
+        all_other_compensation : Optional[Annotated[float, Ge(ge=0)]]
+            All other compensation.
+        total : Optional[Annotated[float, Ge(ge=0)]]
+            Total compensation.
+        filing_date : Optional[date]
+            Date of the filing. (provider: fmp)
+        accepted_date : Optional[datetime]
+            Date the filing was accepted. (provider: fmp)
+        url : Optional[str]
+            URL to the filing data. (provider: fmp)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.fundamental.management_compensation(symbol='AAPL', provider='fmp')
         """  # noqa: E501
 
@@ -2393,30 +2383,28 @@
                         provider,
                         "/equity/fundamental/management_compensation",
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
-                    "start_date": start_date,
-                    "end_date": end_date,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
             )
         )
 
     @exception_handler
     @validate
     def metrics(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio, yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         period: Annotated[
             Optional[Literal["annual", "quarter"]],
             OpenBBCustomParameter(description="Time period of the data to return."),
         ] = "annual",
         limit: Annotated[
@@ -2432,15 +2420,15 @@
         **kwargs
     ) -> OBBject:
         """Get fundamental metrics for a given company.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio, yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance.
         period : Optional[Literal['annual', 'quarter']]
             Time period of the data to return.
         limit : Optional[int]
             The number of data entries to return.
         provider : Optional[Literal['fmp', 'intrinio', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
@@ -2714,30 +2702,30 @@
                 },
                 standard_params={
                     "symbol": symbol,
                     "period": period,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
     def multiples(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -2745,15 +2733,15 @@
         **kwargs
     ) -> OBBject:
         """Get equity valuation multiples for a given company.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
         -------
@@ -2910,15 +2898,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
             )
         )
 
     @exception_handler
     @validate
     @deprecated(
         "This endpoint is deprecated; use `/equity/profile` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.3.",
@@ -3375,15 +3363,15 @@
     @validate
     def revenue_per_geography(
         self,
         symbol: Annotated[
             str, OpenBBCustomParameter(description="Symbol to get data for.")
         ],
         period: Annotated[
-            Literal["quarter", "annual"],
+            Literal["annual", "quarter"],
             OpenBBCustomParameter(description="Time period of the data to return."),
         ] = "annual",
         structure: Annotated[
             Literal["hierarchical", "flat"],
             OpenBBCustomParameter(description="Structure of the returned data."),
         ] = "flat",
         provider: Annotated[
@@ -3396,15 +3384,15 @@
     ) -> OBBject:
         """Get the revenue geographic breakdown for a given company over time.
 
         Parameters
         ----------
         symbol : str
             Symbol to get data for.
-        period : Literal['quarter', 'annual']
+        period : Literal['annual', 'quarter']
             Time period of the data to return.
         structure : Literal['hierarchical', 'flat']
             Structure of the returned data.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
@@ -3466,15 +3454,15 @@
     @validate
     def revenue_per_segment(
         self,
         symbol: Annotated[
             str, OpenBBCustomParameter(description="Symbol to get data for.")
         ],
         period: Annotated[
-            Literal["quarter", "annual"],
+            Literal["annual", "quarter"],
             OpenBBCustomParameter(description="Time period of the data to return."),
         ] = "annual",
         structure: Annotated[
             Literal["hierarchical", "flat"],
             OpenBBCustomParameter(description="Structure of the returned data."),
         ] = "flat",
         provider: Annotated[
@@ -3487,15 +3475,15 @@
     ) -> OBBject:
         """Get the revenue breakdown by business segment for a given company over time.
 
         Parameters
         ----------
         symbol : str
             Symbol to get data for.
-        period : Literal['quarter', 'annual']
+        period : Literal['annual', 'quarter']
             Time period of the data to return.
         structure : Literal['hierarchical', 'flat']
             Structure of the returned data.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
```

### Comparing `openbb-4.1.5/openbb/package/equity_ownership.py` & `openbb-4.1.6/openbb/package/equity_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,15 +592,15 @@
     @exception_handler
     @validate
     def share_statistics(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -608,15 +608,15 @@
         **kwargs
     ) -> OBBject:
         """Get data about share float for a given company.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): yfinance.
         provider : Optional[Literal['fmp', 'intrinio', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
         -------
@@ -687,10 +687,10 @@
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["yfinance"]}},
+                info={"symbol": {"multiple_items_allowed": ["yfinance"]}},
             )
         )
```

### Comparing `openbb-4.1.5/openbb/package/equity_price.py` & `openbb-4.1.6/openbb/package/equity_price.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     @exception_handler
     @validate
     def historical(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp, polygon, tiingo, yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance."
             ),
         ],
         interval: Annotated[
             Optional[str],
             OpenBBCustomParameter(description="Time interval of the data to return."),
         ] = "1d",
         start_date: Annotated[
@@ -57,15 +57,15 @@
         **kwargs
     ) -> OBBject:
         """Get historical price data for a given stock. This includes open, high, low, close, and volume.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp, polygon, tiingo, yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, polygon, tiingo, yfinance.
         interval : Optional[str]
             Time interval of the data to return.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         provider : Optional[Literal['fmp', 'intrinio', 'polygon', 'tiingo', 'yfinanc...
@@ -184,23 +184,25 @@
                 standard_params={
                     "symbol": symbol,
                     "interval": interval,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": [
                             "fmp",
                             "polygon",
                             "tiingo",
                             "yfinance",
                         ]
-                    }
+                    },
+                    "adjusted": {"deprecated": True},
+                    "prepost": {"deprecated": True},
                 },
             )
         )
 
     @exception_handler
     @validate
     def nbbo(
@@ -227,35 +229,21 @@
             If None, the provider specified in defaults is selected or 'polygon' if there is
             no default.
         limit : int
             The number of data entries to return. Up to ten million records will be returned. Pagination occurs in groups of 50,000. Remaining limit values will always return 50,000 more records unless it is the last page. High volume tickers will require multiple max requests for a single day's NBBO records. Expect stocks, like SPY, to approach 1GB in size, per day, as a raw CSV. Splitting large requests into chunks is recommended for full-day requests of high-volume symbols. (provider: polygon)
         date : Optional[datetime.date]
             A specific date to get data for. Use bracketed the timestamp parameters to specify exact time ranges. (provider: polygon)
         timestamp_lt : Optional[Union[datetime.datetime, str]]
-
-                    Query by datetime, less than. Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-                    YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-                 (provider: polygon)
+            Query by datetime, less than. Either a date with the format 'YYYY-MM-DD' or a TZ-aware timestamp string, 'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the day and hour. (provider: polygon)
         timestamp_gt : Optional[Union[datetime.datetime, str]]
-
-                    Query by datetime, greater than. Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-                    YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-                 (provider: polygon)
+            Query by datetime, greater than. Either a date with the format 'YYYY-MM-DD' or a TZ-aware timestamp string, 'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the day and hour. (provider: polygon)
         timestamp_lte : Optional[Union[datetime.datetime, str]]
-
-                    Query by datetime, less than or equal to.
-                    Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-                    YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-                 (provider: polygon)
+            Query by datetime, less than or equal to. Either a date with the format 'YYYY-MM-DD' or a TZ-aware timestamp string, 'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the day and hour. (provider: polygon)
         timestamp_gte : Optional[Union[datetime.datetime, str]]
-
-                    Query by datetime, greater than or equal to.
-                    Either a date with the format YYYY-MM-DD or a TZ-aware timestamp string,
-                    YYYY-MM-DDTH:M:S.000000000-04:00". Include all nanoseconds and the 'T' between the day and hour.
-                 (provider: polygon)
+            Query by datetime, greater than or equal to. Either a date with the format 'YYYY-MM-DD' or a TZ-aware timestamp string, 'YYYY-MM-DDTH:M:S.000000000-04:00'. Include all nanoseconds and the 'T' between the day and hour. (provider: polygon)
 
         Returns
         -------
         OBBject
             results : List[EquityNBBO]
                 Serializable results.
             provider : Optional[Literal['polygon']]
@@ -288,34 +276,21 @@
         tape : Optional[str]
             The exchange tape. (provider: polygon)
         conditions : Optional[Union[str, List[int], List[str]]]
             A list of condition codes. (provider: polygon)
         indicators : Optional[List[int]]
             A list of indicator codes. (provider: polygon)
         sequence_num : Optional[int]
-
-                    The sequence number represents the sequence in which message events happened.
-                    These are increasing and unique per ticker symbol, but will not always be sequential
-                    (e.g., 1, 2, 6, 9, 10, 11)
-                 (provider: polygon)
+            The sequence number represents the sequence in which message events happened. These are increasing and unique per ticker symbol, but will not always be sequential (e.g., 1, 2, 6, 9, 10, 11) (provider: polygon)
         participant_timestamp : Optional[datetime]
-
-                    The nanosecond accuracy Participant/Exchange Unix Timestamp.
-                    This is the timestamp of when the quote was actually generated at the exchange.
-                 (provider: polygon)
+            The nanosecond accuracy Participant/Exchange Unix Timestamp. This is the timestamp of when the quote was actually generated at the exchange. (provider: polygon)
         sip_timestamp : Optional[datetime]
-
-                    The nanosecond accuracy SIP Unix Timestamp.
-                    This is the timestamp of when the SIP received this quote from the exchange which produced it.
-                 (provider: polygon)
+            The nanosecond accuracy SIP Unix Timestamp. This is the timestamp of when the SIP received this quote from the exchange which produced it. (provider: polygon)
         trf_timestamp : Optional[datetime]
-
-                    The nanosecond accuracy TRF (Trade Reporting Facility) Unix Timestamp.
-                    This is the timestamp of when the trade reporting facility received this quote.
-                 (provider: polygon)
+            The nanosecond accuracy TRF (Trade Reporting Facility) Unix Timestamp. This is the timestamp of when the trade reporting facility received this quote. (provider: polygon)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.price.nbbo(symbol='AAPL', provider='polygon')
         """  # noqa: E501
 
@@ -339,15 +314,15 @@
     @exception_handler
     @validate
     def performance(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -355,15 +330,15 @@
         **kwargs
     ) -> OBBject:
         """Get price performance data for a given stock. This includes price changes for different time periods.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp.
         provider : Optional[Literal['fmp']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
 
         Returns
         -------
@@ -377,14 +352,16 @@
             chart : Optional[Chart]
                 Chart object.
             extra : Dict[str, Any]
                 Extra info.
 
         PricePerformance
         ----------------
+        symbol : Optional[str]
+            Symbol representing the entity requested in the data.
         one_day : Optional[float]
             One-day return.
         wtd : Optional[float]
             Week to date return.
         one_week : Optional[float]
             One-week return.
         mtd : Optional[float]
@@ -397,24 +374,26 @@
             Three-month return.
         six_month : Optional[float]
             Six-month return.
         ytd : Optional[float]
             Year to date return.
         one_year : Optional[float]
             One-year return.
+        two_year : Optional[float]
+            Two-year return.
         three_year : Optional[float]
             Three-year return.
+        four_year : Optional[float]
+            Four-year
         five_year : Optional[float]
             Five-year return.
         ten_year : Optional[float]
             Ten-year return.
         max : Optional[float]
             Return from the beginning of the time series.
-        symbol : Optional[str]
-            The ticker symbol. (provider: fmp)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.price.performance(symbol='AAPL', provider='fmp')
         """  # noqa: E501
 
@@ -428,26 +407,26 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                extra_info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
             )
         )
 
     @exception_handler
     @validate
     def quote(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. This endpoint will accept multiple symbols separated by commas. Multiple items allowed for provider(s): fmp, intrinio, yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance."
             ),
         ],
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "yfinance"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
@@ -455,15 +434,15 @@
         **kwargs
     ) -> OBBject:
         """Get the latest quote for a given stock. Quote includes price, volume, and other data.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. This endpoint will accept multiple symbols separated by commas. Multiple items allowed for provider(s): fmp, intrinio, yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, yfinance.
         provider : Optional[Literal['fmp', 'intrinio', 'yfinance']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
         source : Literal['iex', 'bats', 'bats_delayed', 'utp_delayed', 'cta_a_delayed', 'cta_b_delayed', 'intrinio_mx', 'intrinio_mx_plus', 'delayed_sip']
             Source of the data. (provider: intrinio)
 
@@ -559,23 +538,23 @@
             Market cap of the company. (provider: fmp)
         shares_outstanding : Optional[int]
             Number of shares outstanding. (provider: fmp)
         eps : Optional[float]
             Earnings per share. (provider: fmp)
         pe : Optional[float]
             Price earnings ratio. (provider: fmp)
-        earnings_announcement : Optional[Union[datetime, str]]
+        earnings_announcement : Optional[datetime]
             Upcoming earnings announcement date. (provider: fmp)
         is_darkpool : Optional[bool]
             Whether or not the current trade is from a darkpool. (provider: intrinio)
         source : Optional[str]
             Source of the Intrinio data. (provider: intrinio)
         updated_on : Optional[datetime]
             Date and Time when the data was last updated. (provider: intrinio)
-        security : Optional[openbb_intrinio.utils.references.IntrinioSecurity]
+        security : Optional[IntrinioSecurity]
             Security details related to the quote. (provider: intrinio)
         ma_50d : Optional[float]
             50-day moving average price. (provider: yfinance)
         ma_200d : Optional[float]
             200-day moving average price. (provider: yfinance)
         volume_average : Optional[float]
             Average daily trading volume. (provider: yfinance)
@@ -600,14 +579,14 @@
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
                     }
                 },
             )
         )
```

### Comparing `openbb-4.1.5/openbb/package/equity_shorts.py` & `openbb-4.1.6/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/fixedincome.py` & `openbb-4.1.6/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/fixedincome_corporate.py` & `openbb-4.1.6/openbb/package/fixedincome_corporate.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,21 +444,21 @@
             OpenBBCustomParameter(
                 description="End date of the data, in YYYY-MM-DD format."
             ),
         ] = None,
         maturity: Annotated[
             Union[float, str, List[Union[float, str]]],
             OpenBBCustomParameter(
-                description="Maturities in years. Multiple items allowed for provider(s): fred."
+                description="Maturities in years. Multiple comma separated items allowed for provider(s): fred."
             ),
         ] = 10.0,
         category: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Rate category. Options: spot_rate, par_yield. Multiple items allowed for provider(s): fred."
+                description="Rate category. Options: spot_rate, par_yield. Multiple comma separated items allowed for provider(s): fred."
             ),
             OpenBBCustomChoices(choices=["par_yield", "spot_rate"]),
         ] = "spot_rate",
         provider: Annotated[
             Optional[Literal["fred"]],
             OpenBBCustomParameter(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
@@ -477,17 +477,17 @@
         Parameters
         ----------
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         maturity : Union[float, str, List[Union[float, str]]]
-            Maturities in years. Multiple items allowed for provider(s): fred.
+            Maturities in years. Multiple comma separated items allowed for provider(s): fred.
         category : Union[str, List[str]]
-            Rate category. Options: spot_rate, par_yield. Multiple items allowed for provider(s): fred.
+            Rate category. Options: spot_rate, par_yield. Multiple comma separated items allowed for provider(s): fred.
         provider : Optional[Literal['fred']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fred' if there is
             no default.
 
         Returns
         -------
@@ -530,13 +530,13 @@
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                     "category": category,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "maturity": {"multiple_items_allowed": ["fred"]},
                     "category": {"multiple_items_allowed": ["fred"]},
                 },
             )
         )
```

### Comparing `openbb-4.1.5/openbb/package/fixedincome_government.py` & `openbb-4.1.6/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/fixedincome_rate.py` & `openbb-4.1.6/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/fixedincome_spreads.py` & `openbb-4.1.6/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/openbb/package/index.py` & `openbb-4.1.6/openbb/package/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         category=OpenBBDeprecationWarning,
     )
     def market(
         self,
         symbol: Annotated[
             Union[str, List[str]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio, polygon, yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, polygon, yfinance."
             ),
         ],
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
@@ -217,15 +217,15 @@
         **kwargs
     ) -> OBBject:
         """Historical Market Indices.
 
         Parameters
         ----------
         symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio, polygon, yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio, polygon, yfinance.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         interval : Optional[str]
             Time interval of the data to return.
         provider : Optional[Literal['fmp', 'intrinio', 'polygon', 'yfinance']]
@@ -300,15 +300,15 @@
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "interval": interval,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": [
                             "fmp",
                             "intrinio",
                             "polygon",
                             "yfinance",
                         ]
```

### Comparing `openbb-4.1.5/openbb/package/news.py` & `openbb-4.1.6/openbb/package/news.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @exception_handler
     @validate
     def company(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
             OpenBBCustomParameter(
-                description="Symbol to get data for. This endpoint will accept multiple symbols separated by commas. Multiple items allowed for provider(s): benzinga, fmp, intrinio, polygon, tiingo, yfinance."
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): benzinga, fmp, intrinio, polygon, tiingo, yfinance."
             ),
         ] = None,
         start_date: Annotated[
             Union[datetime.date, None, str],
             OpenBBCustomParameter(
                 description="Start date of the data, in YYYY-MM-DD format."
             ),
@@ -58,15 +58,15 @@
         **kwargs
     ) -> OBBject:
         """Company News. Get news for one or more companies.
 
         Parameters
         ----------
         symbol : Union[str, None, List[Optional[str]]]
-            Symbol to get data for. This endpoint will accept multiple symbols separated by commas. Multiple items allowed for provider(s): benzinga, fmp, intrinio, polygon, tiingo, yfinance.
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): benzinga, fmp, intrinio, polygon, tiingo, yfinance.
         start_date : Union[datetime.date, None, str]
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         limit : Optional[Annotated[int, Ge(ge=0)]]
             The number of data entries to return.
         provider : Optional[Literal['benzinga', 'fmp', 'intrinio', 'polygon', 'tiing...
@@ -150,15 +150,15 @@
         source : Optional[str]
             Name of the news source. (provider: fmp);
             Source of the article. (provider: polygon);
             News source. (provider: tiingo);
             Source of the news article (provider: yfinance)
         amp_url : Optional[str]
             AMP URL. (provider: polygon)
-        publisher : Optional[openbb_polygon.models.company_news.PolygonPublisher]
+        publisher : Optional[PolygonPublisher]
             Publisher of the article. (provider: polygon)
         article_id : Optional[int]
             Unique ID of the news article. (provider: tiingo)
         crawl_date : Optional[datetime]
             Date the news article was crawled. (provider: tiingo)
 
         Examples
@@ -196,15 +196,15 @@
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                extra_info={
+                info={
                     "symbol": {
                         "multiple_items_allowed": [
                             "benzinga",
                             "fmp",
                             "intrinio",
                             "polygon",
                             "tiingo",
```

### Comparing `openbb-4.1.5/openbb/package/regulators_sec.py` & `openbb-4.1.6/openbb/package/regulators_sec.py`

 * *Files identical despite different names*

### Comparing `openbb-4.1.5/pyproject.toml` & `openbb-4.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 [tool.poetry]
 name = "openbb"
-version = "4.1.5"
+version = "4.1.6"
 description = "OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 readme = "README.md"
 packages = [{ include = "openbb" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.1.3"
+openbb-core = "^1.1.5"
 
-openbb-benzinga = "^1.1.3"
-openbb-federal-reserve = "^1.1.3"
-openbb-fmp = "^1.1.3"
-openbb-fred = "^1.1.3"
-openbb-intrinio = "^1.1.3"
-openbb-oecd = "^1.1.3"
-openbb-polygon = "^1.1.3"
-openbb-sec = "^1.1.3"
-openbb-tiingo = "^1.1.3"
-openbb-tradingeconomics = "^1.1.3"
-openbb-yfinance = "^1.1.3"
-
-openbb-commodity = "^1.0.1"
-openbb-crypto = "^1.1.3"
-openbb-currency = "^1.1.3"
-openbb-derivatives = "^1.1.3"
-openbb-economy = "^1.1.3"
-openbb-equity = "^1.1.3"
-openbb-etf = "^1.1.3"
-openbb-fixedincome = "^1.1.3"
-openbb-index = "^1.1.3"
-openbb-news = "^1.1.3"
-openbb-regulators = "^1.1.3"
+openbb-benzinga = "^1.1.4"
+openbb-federal-reserve = "^1.1.4"
+openbb-fmp = "^1.1.4"
+openbb-fred = "^1.1.4"
+openbb-intrinio = "^1.1.4"
+openbb-oecd = "^1.1.4"
+openbb-polygon = "^1.1.4"
+openbb-sec = "^1.1.4"
+openbb-tiingo = "^1.1.4"
+openbb-tradingeconomics = "^1.1.4"
+openbb-yfinance = "^1.1.4"
+
+openbb-commodity = "^1.0.2"
+openbb-crypto = "^1.1.4"
+openbb-currency = "^1.1.4"
+openbb-derivatives = "^1.1.4"
+openbb-economy = "^1.1.4"
+openbb-equity = "^1.1.4"
+openbb-etf = "^1.1.4"
+openbb-fixedincome = "^1.1.4"
+openbb-index = "^1.1.4"
+openbb-news = "^1.1.4"
+openbb-regulators = "^1.1.4"
 
 # Community dependencies
-openbb-alpha-vantage = { version = "^1.1.3", optional = true }
-openbb-biztoc = { version = "^1.1.3", optional = true }
-openbb-cboe = { version = "^1.1.3", optional = true }
-openbb-ecb = { version = "^1.1.3", optional = true }
-openbb-finra = { version = "^1.1.3", optional = true }
-openbb-finviz = { version = "^1.0.2", optional = true }
-openbb-government-us = { version = "^1.1.3", optional = true }
-openbb-nasdaq = { version = "^1.1.3", optional = true }
-openbb-seeking-alpha = { version = "^1.1.3", optional = true }
-openbb-stockgrid = { version = "^1.1.3", optional = true }
-openbb-tmx = { version = "^1.0.0", optional = true }
-openbb-tradier = { version = "^1.0.0", optional = true }
-openbb-wsj = { version = "^1.1.3", optional = true }
-
-openbb-charting = { version = "^2.0.1", optional = true }
-openbb-econometrics = { version = "^1.1.3", optional = true }
-openbb-quantitative = { version = "^1.1.3", optional = true }
-openbb-technical = { version = "^1.1.4", optional = true }
+openbb-alpha-vantage = { version = "^1.1.4", optional = true }
+openbb-biztoc = { version = "^1.1.4", optional = true }
+openbb-cboe = { version = "^1.1.4", optional = true }
+openbb-ecb = { version = "^1.1.4", optional = true }
+openbb-finra = { version = "^1.1.4", optional = true }
+openbb-finviz = { version = "^1.0.3", optional = true }
+openbb-government-us = { version = "^1.1.4", optional = true }
+openbb-nasdaq = { version = "^1.1.4", optional = true }
+openbb-seeking-alpha = { version = "^1.1.4", optional = true }
+openbb-stockgrid = { version = "^1.1.4", optional = true }
+openbb-tmx = { version = "^1.0.1", optional = true }
+openbb-tradier = { version = "^1.0.1", optional = true }
+openbb-wsj = { version = "^1.1.4", optional = true }
+
+openbb-charting = { version = "^2.0.2", optional = true }
+openbb-econometrics = { version = "^1.1.4", optional = true }
+openbb-quantitative = { version = "^1.1.4", optional = true }
+openbb-technical = { version = "^1.1.5", optional = true }
 
 [tool.poetry.extras]
 alpha_vantage = ["openbb-alpha-vantage"]
 biztoc = ["openbb-biztoc"]
 cboe = ["openbb-cboe"]
 charting = ["openbb-charting"]
 ecb = ["openbb-ecb"]
```

### Comparing `openbb-4.1.5/PKG-INFO` & `openbb-4.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb
-Version: 4.1.5
+Version: 4.1.6
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,54 +24,54 @@
 Provides-Extra: quantitative
 Provides-Extra: seeking-alpha
 Provides-Extra: stockgrid
 Provides-Extra: technical
 Provides-Extra: tmx
 Provides-Extra: tradier
 Provides-Extra: wsj
-Requires-Dist: openbb-alpha-vantage (>=1.1.3,<2.0.0) ; extra == "alpha-vantage" or extra == "all"
-Requires-Dist: openbb-benzinga (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-biztoc (>=1.1.3,<2.0.0) ; extra == "biztoc" or extra == "all"
-Requires-Dist: openbb-cboe (>=1.1.3,<2.0.0) ; extra == "cboe" or extra == "all"
-Requires-Dist: openbb-charting (>=2.0.1,<3.0.0) ; extra == "charting" or extra == "all"
-Requires-Dist: openbb-commodity (>=1.0.1,<2.0.0)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-crypto (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-currency (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-derivatives (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-ecb (>=1.1.3,<2.0.0) ; extra == "ecb" or extra == "all"
-Requires-Dist: openbb-econometrics (>=1.1.3,<2.0.0) ; extra == "econometrics" or extra == "all"
-Requires-Dist: openbb-economy (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-equity (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-etf (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-federal-reserve (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-finra (>=1.1.3,<2.0.0) ; extra == "finra" or extra == "all"
-Requires-Dist: openbb-finviz (>=1.0.2,<2.0.0) ; extra == "finviz" or extra == "all"
-Requires-Dist: openbb-fixedincome (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-fmp (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-fred (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-government-us (>=1.1.3,<2.0.0) ; extra == "government-us" or extra == "all"
-Requires-Dist: openbb-index (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-intrinio (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-nasdaq (>=1.1.3,<2.0.0) ; extra == "nasdaq" or extra == "all"
-Requires-Dist: openbb-news (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-oecd (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-polygon (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-quantitative (>=1.1.3,<2.0.0) ; extra == "quantitative" or extra == "all"
-Requires-Dist: openbb-regulators (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-sec (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-seeking-alpha (>=1.1.3,<2.0.0) ; extra == "seeking-alpha" or extra == "all"
-Requires-Dist: openbb-stockgrid (>=1.1.3,<2.0.0) ; extra == "stockgrid" or extra == "all"
-Requires-Dist: openbb-technical (>=1.1.4,<2.0.0) ; extra == "technical" or extra == "all"
-Requires-Dist: openbb-tiingo (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-tmx (>=1.0.0,<2.0.0) ; extra == "tmx" or extra == "all"
-Requires-Dist: openbb-tradier (>=1.0.0,<2.0.0) ; extra == "tradier" or extra == "all"
-Requires-Dist: openbb-tradingeconomics (>=1.1.3,<2.0.0)
-Requires-Dist: openbb-wsj (>=1.1.3,<2.0.0) ; extra == "wsj" or extra == "all"
-Requires-Dist: openbb-yfinance (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-alpha-vantage (>=1.1.4,<2.0.0) ; extra == "alpha-vantage" or extra == "all"
+Requires-Dist: openbb-benzinga (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-biztoc (>=1.1.4,<2.0.0) ; extra == "biztoc" or extra == "all"
+Requires-Dist: openbb-cboe (>=1.1.4,<2.0.0) ; extra == "cboe" or extra == "all"
+Requires-Dist: openbb-charting (>=2.0.2,<3.0.0) ; extra == "charting" or extra == "all"
+Requires-Dist: openbb-commodity (>=1.0.2,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-crypto (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-currency (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-derivatives (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-ecb (>=1.1.4,<2.0.0) ; extra == "ecb" or extra == "all"
+Requires-Dist: openbb-econometrics (>=1.1.4,<2.0.0) ; extra == "econometrics" or extra == "all"
+Requires-Dist: openbb-economy (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-equity (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-etf (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-federal-reserve (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-finra (>=1.1.4,<2.0.0) ; extra == "finra" or extra == "all"
+Requires-Dist: openbb-finviz (>=1.0.3,<2.0.0) ; extra == "finviz" or extra == "all"
+Requires-Dist: openbb-fixedincome (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-fmp (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-fred (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-government-us (>=1.1.4,<2.0.0) ; extra == "government-us" or extra == "all"
+Requires-Dist: openbb-index (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-intrinio (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-nasdaq (>=1.1.4,<2.0.0) ; extra == "nasdaq" or extra == "all"
+Requires-Dist: openbb-news (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-oecd (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-polygon (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-quantitative (>=1.1.4,<2.0.0) ; extra == "quantitative" or extra == "all"
+Requires-Dist: openbb-regulators (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-sec (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-seeking-alpha (>=1.1.4,<2.0.0) ; extra == "seeking-alpha" or extra == "all"
+Requires-Dist: openbb-stockgrid (>=1.1.4,<2.0.0) ; extra == "stockgrid" or extra == "all"
+Requires-Dist: openbb-technical (>=1.1.5,<2.0.0) ; extra == "technical" or extra == "all"
+Requires-Dist: openbb-tiingo (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-tmx (>=1.0.1,<2.0.0) ; extra == "tmx" or extra == "all"
+Requires-Dist: openbb-tradier (>=1.0.1,<2.0.0) ; extra == "tradier" or extra == "all"
+Requires-Dist: openbb-tradingeconomics (>=1.1.4,<2.0.0)
+Requires-Dist: openbb-wsj (>=1.1.4,<2.0.0) ; extra == "wsj" or extra == "all"
+Requires-Dist: openbb-yfinance (>=1.1.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Platform
 
 [![Downloads](https://static.pepy.tech/badge/openbb)](https://pepy.tech/project/openbb)
 [![LatestRelease](https://badge.fury.io/py/openbb.svg)](https://github.com/OpenBB-finance/OpenBBTerminal)
```

