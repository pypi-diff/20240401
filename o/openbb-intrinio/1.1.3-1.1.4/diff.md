# Comparing `tmp/openbb_intrinio-1.1.3.tar.gz` & `tmp/openbb_intrinio-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_intrinio-1.1.3.tar", max compression
+gzip compressed data, was "openbb_intrinio-1.1.4.tar", max compression
```

## Comparing `openbb_intrinio-1.1.3.tar` & `openbb_intrinio-1.1.4.tar`

### file list

```diff
@@ -1,37 +1,42 @@
--rw-r--r--   0        0        0      435 2024-01-17 14:26:16.765927 openbb_intrinio-1.1.3/README.md
--rw-r--r--   0        0        0     4213 2024-03-11 10:41:33.408194 openbb_intrinio-1.1.3/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-01-17 14:26:16.766160 openbb_intrinio-1.1.3/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-03-11 10:48:09.533354 openbb_intrinio-1.1.3/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7545 2024-01-17 14:26:16.766492 openbb_intrinio-1.1.3/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-03-11 10:41:33.408480 openbb_intrinio-1.1.3/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-01-17 14:26:16.766737 openbb_intrinio-1.1.3/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3208 2024-02-26 09:52:50.863582 openbb_intrinio-1.1.3/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-01-26 17:52:27.967597 openbb_intrinio-1.1.3/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-03-11 10:41:33.408600 openbb_intrinio-1.1.3/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2377 2024-02-23 17:14:57.465948 openbb_intrinio-1.1.3/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-02-23 17:14:57.466051 openbb_intrinio-1.1.3/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-01-17 14:26:16.767212 openbb_intrinio-1.1.3/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     2805 2024-01-17 14:26:16.767284 openbb_intrinio-1.1.3/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-01-17 14:26:16.767363 openbb_intrinio-1.1.3/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     3716 2024-01-17 14:26:16.767449 openbb_intrinio-1.1.3/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     4829 2024-02-23 17:14:57.467008 openbb_intrinio-1.1.3/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-02-06 11:54:53.231315 openbb_intrinio-1.1.3/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-03-11 10:41:33.408705 openbb_intrinio-1.1.3/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-03-11 10:41:33.408832 openbb_intrinio-1.1.3/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-02-06 11:54:53.231736 openbb_intrinio-1.1.3/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-01-17 14:26:16.767866 openbb_intrinio-1.1.3/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-03-11 19:09:39.079696 openbb_intrinio-1.1.3/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3328 2024-02-23 17:14:57.467275 openbb_intrinio-1.1.3/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-01-17 14:26:16.768261 openbb_intrinio-1.1.3/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     4745 2024-01-29 10:27:24.914018 openbb_intrinio-1.1.3/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-03-11 10:48:09.533946 openbb_intrinio-1.1.3/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     5359 2024-01-17 14:26:16.768736 openbb_intrinio-1.1.3/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-01-17 14:26:16.768800 openbb_intrinio-1.1.3/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-01-17 14:26:16.768865 openbb_intrinio-1.1.3/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2550 2024-02-23 17:14:57.467401 openbb_intrinio-1.1.3/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.768972 openbb_intrinio-1.1.3/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-01-17 14:26:16.769067 openbb_intrinio-1.1.3/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4002 2024-01-29 10:27:24.914152 openbb_intrinio-1.1.3/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     3280 2024-01-17 14:26:16.769203 openbb_intrinio-1.1.3/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0      489 2024-03-11 20:00:05.724692 openbb_intrinio-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 openbb_intrinio-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      435 2024-02-29 11:03:36.874696 openbb_intrinio-1.1.4/README.md
+-rw-r--r--   0        0        0     4877 2024-03-21 17:38:35.647407 openbb_intrinio-1.1.4/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-02-29 11:03:36.874926 openbb_intrinio-1.1.4/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22983 2024-03-21 17:38:35.647677 openbb_intrinio-1.1.4/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-03-21 17:38:35.647832 openbb_intrinio-1.1.4/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-03-21 17:38:35.648040 openbb_intrinio-1.1.4/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-03-21 17:38:35.648194 openbb_intrinio-1.1.4/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     3273 2024-03-22 23:30:27.583493 openbb_intrinio-1.1.4/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-03-21 17:38:35.648311 openbb_intrinio-1.1.4/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     8675 2024-03-13 16:36:51.743339 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2377 2024-03-21 17:38:35.648469 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-03-21 17:38:35.648601 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-03-21 17:38:35.648729 openbb_intrinio-1.1.4/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7025 2024-03-18 09:35:41.453005 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-03-14 20:24:16.781915 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-03-21 17:38:35.648867 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-03-21 17:38:35.648989 openbb_intrinio-1.1.4/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-03-21 17:38:35.649110 openbb_intrinio-1.1.4/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-03-21 17:38:35.649277 openbb_intrinio-1.1.4/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     3716 2024-03-13 16:36:51.743945 openbb_intrinio-1.1.4/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     4829 2024-03-13 16:36:51.744032 openbb_intrinio-1.1.4/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-03-21 17:38:35.649392 openbb_intrinio-1.1.4/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-03-21 17:38:35.649563 openbb_intrinio-1.1.4/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-03-13 16:36:51.744490 openbb_intrinio-1.1.4/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-03-21 17:38:35.649669 openbb_intrinio-1.1.4/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-03-21 17:38:35.649782 openbb_intrinio-1.1.4/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-03-13 16:36:51.745028 openbb_intrinio-1.1.4/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3328 2024-03-13 16:36:51.745129 openbb_intrinio-1.1.4/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-03-21 17:38:35.649897 openbb_intrinio-1.1.4/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8829 2024-03-19 14:52:38.490220 openbb_intrinio-1.1.4/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-03-21 17:38:35.650024 openbb_intrinio-1.1.4/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-03-13 16:36:51.745487 openbb_intrinio-1.1.4/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     5359 2024-03-21 17:38:35.650166 openbb_intrinio-1.1.4/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-03-21 17:38:35.650280 openbb_intrinio-1.1.4/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-03-13 16:36:51.745863 openbb_intrinio-1.1.4/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     2550 2024-03-21 17:38:35.650413 openbb_intrinio-1.1.4/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.876946 openbb_intrinio-1.1.4/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-02-29 11:03:36.877031 openbb_intrinio-1.1.4/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4002 2024-03-13 16:36:51.746151 openbb_intrinio-1.1.4/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-03-18 09:35:41.453455 openbb_intrinio-1.1.4/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0      489 2024-04-01 14:21:12.248104 openbb_intrinio-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 openbb_intrinio-1.1.4/PKG-INFO
```

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/__init__.py` & `openbb_intrinio-1.1.4/openbb_intrinio/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from openbb_intrinio.models.company_filings import IntrinioCompanyFilingsFetcher
 from openbb_intrinio.models.company_news import IntrinioCompanyNewsFetcher
 from openbb_intrinio.models.currency_pairs import IntrinioCurrencyPairsFetcher
 from openbb_intrinio.models.equity_historical import IntrinioEquityHistoricalFetcher
 from openbb_intrinio.models.equity_info import IntrinioEquityInfoFetcher
 from openbb_intrinio.models.equity_quote import IntrinioEquityQuoteFetcher
 from openbb_intrinio.models.equity_search import IntrinioEquitySearchFetcher
+from openbb_intrinio.models.etf_holdings import IntrinioEtfHoldingsFetcher
+from openbb_intrinio.models.etf_info import IntrinioEtfInfoFetcher
+from openbb_intrinio.models.etf_price_performance import (
+    IntrinioEtfPricePerformanceFetcher,
+)
+from openbb_intrinio.models.etf_search import IntrinioEtfSearchFetcher
 from openbb_intrinio.models.financial_ratios import IntrinioFinancialRatiosFetcher
 from openbb_intrinio.models.fred_series import IntrinioFredSeriesFetcher
 from openbb_intrinio.models.historical_attributes import (
     IntrinioHistoricalAttributesFetcher,
 )
 from openbb_intrinio.models.historical_dividends import (
     IntrinioHistoricalDividendsFetcher,
@@ -24,14 +30,15 @@
 from openbb_intrinio.models.insider_trading import IntrinioInsiderTradingFetcher
 
 # from openbb_intrinio.models.institutional_ownership import (
 #     IntrinioInstitutionalOwnershipFetcher,
 # )
 from openbb_intrinio.models.key_metrics import IntrinioKeyMetricsFetcher
 from openbb_intrinio.models.latest_attributes import IntrinioLatestAttributesFetcher
+from openbb_intrinio.models.market_snapshots import IntrinioMarketSnapshotsFetcher
 from openbb_intrinio.models.options_chains import IntrinioOptionsChainsFetcher
 from openbb_intrinio.models.options_unusual import IntrinioOptionsUnusualFetcher
 from openbb_intrinio.models.reported_financials import IntrinioReportedFinancialsFetcher
 from openbb_intrinio.models.search_attributes import (
     IntrinioSearchAttributesFetcher,
 )
 from openbb_intrinio.models.share_statistics import IntrinioShareStatisticsFetcher
@@ -51,25 +58,30 @@
         "CompanyNews": IntrinioCompanyNewsFetcher,
         "CurrencyPairs": IntrinioCurrencyPairsFetcher,
         "EquityHistorical": IntrinioEquityHistoricalFetcher,
         "EquityInfo": IntrinioEquityInfoFetcher,
         "EquityQuote": IntrinioEquityQuoteFetcher,
         "EquitySearch": IntrinioEquitySearchFetcher,
         "EtfHistorical": IntrinioEquityHistoricalFetcher,
+        "EtfHoldings": IntrinioEtfHoldingsFetcher,
+        "EtfInfo": IntrinioEtfInfoFetcher,
+        "EtfPricePerformance": IntrinioEtfPricePerformanceFetcher,
+        "EtfSearch": IntrinioEtfSearchFetcher,
         "FinancialRatios": IntrinioFinancialRatiosFetcher,
         "FredSeries": IntrinioFredSeriesFetcher,
         "HistoricalAttributes": IntrinioHistoricalAttributesFetcher,
         "HistoricalDividends": IntrinioHistoricalDividendsFetcher,
         "IncomeStatement": IntrinioIncomeStatementFetcher,
         "IndexHistorical": IntrinioIndexHistoricalFetcher,
         "InsiderTrading": IntrinioInsiderTradingFetcher,
         # "InstitutionalOwnership": IntrinioInstitutionalOwnershipFetcher, # Disabled due to unreliable Intrinio endpoint
         "KeyMetrics": IntrinioKeyMetricsFetcher,
         "LatestAttributes": IntrinioLatestAttributesFetcher,
         "MarketIndices": IntrinioIndexHistoricalFetcher,
+        "MarketSnapshots": IntrinioMarketSnapshotsFetcher,
         "OptionsChains": IntrinioOptionsChainsFetcher,
         "OptionsUnusual": IntrinioOptionsUnusualFetcher,
         "ReportedFinancials": IntrinioReportedFinancialsFetcher,
         "SearchAttributes": IntrinioSearchAttributesFetcher,
         "ShareStatistics": IntrinioShareStatisticsFetcher,
         "WorldNews": IntrinioWorldNewsFetcher,
     },
```

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/balance_sheet.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/calendar_ipo.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/calendar_ipo.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,78 +41,77 @@
 
 class IntrinioCalendarIpoData(CalendarIpoData):
     """Intrinio IPO Calendar Data."""
 
     __alias_dict__ = {"symbol": "ticker", "ipo_date": "date"}
 
     status: Optional[Literal["upcoming", "priced", "withdrawn"]] = Field(
-        description="""
-            The status of the IPO. Upcoming IPOs have not taken place yet but are expected to.
-            Priced IPOs have taken place.
-            Withdrawn IPOs were expected to take place, but were subsequently withdrawn and did not take place
-        """,
+        description=(
+            "The status of the IPO. Upcoming IPOs have not taken place yet but are expected to. "
+            "Priced IPOs have taken place. Withdrawn IPOs were expected to take place, but were subsequently withdrawn."
+        ),
         default=None,
     )
     exchange: Optional[str] = Field(
-        description="""
-            The acronym of the stock exchange that the company is going to trade publicly on.
-            Typically NYSE or NASDAQ.
-        """,
+        description=(
+            "The acronym of the stock exchange that the company is going to trade publicly on. "
+            "Typically NYSE or NASDAQ."
+        ),
         default=None,
     )
     offer_amount: Optional[float] = Field(
         description="The total dollar amount of shares offered in the IPO. Typically this is share price * share count",
         default=None,
     )
     share_price: Optional[float] = Field(
         description="The price per share at which the IPO was offered.", default=None
     )
     share_price_lowest: Optional[float] = Field(
-        description="""
-            The expected lowest price per share at which the IPO will be offered.
-            Before an IPO is priced, companies typically provide a range of prices per share at which
-            they expect to offer the IPO (typically available for upcoming IPOs).
-        """,
+        description=(
+            "The expected lowest price per share at which the IPO will be offered. "
+            "Before an IPO is priced, companies typically provide a range of prices per share at which "
+            "they expect to offer the IPO (typically available for upcoming IPOs)."
+        ),
         default=None,
     )
     share_price_highest: Optional[float] = Field(
-        description="""
-            The expected highest price per share at which the IPO will be offered.
-            Before an IPO is priced, companies typically provide a range of prices per share at which
-            they expect to offer the IPO (typically available for upcoming IPOs).
-        """,
+        description=(
+            "The expected highest price per share at which the IPO will be offered. "
+            "Before an IPO is priced, companies typically provide a range of prices per share at which "
+            "they expect to offer the IPO (typically available for upcoming IPOs)."
+        ),
         default=None,
     )
     share_count: Optional[int] = Field(
         description="The number of shares offered in the IPO.", default=None
     )
     share_count_lowest: Optional[int] = Field(
-        description="""
-            The expected lowest number of shares that will be offered in the IPO. Before an IPO is priced,
-            companies typically provide a range of shares that they expect to offer in the IPO
-            (typically available for upcoming IPOs).
-        """,
+        description=(
+            "The expected lowest number of shares that will be offered in the IPO. Before an IPO is priced, "
+            "companies typically provide a range of shares that they expect to offer in the IPO "
+            "(typically available for upcoming IPOs)."
+        ),
         default=None,
     )
     share_count_highest: Optional[int] = Field(
-        description="""
-            The expected highest number of shares that will be offered in the IPO. Before an IPO is priced,
-            companies typically provide a range of shares that they expect to offer in the IPO
-            (typically available for upcoming IPOs).
-        """,
+        description=(
+            "The expected highest number of shares that will be offered in the IPO. Before an IPO is priced, "
+            "companies typically provide a range of shares that they expect to offer in the IPO "
+            "(typically available for upcoming IPOs)."
+        ),
         default=None,
     )
     announcement_url: Optional[str] = Field(
         description="The URL to the company's announcement of the IPO", default=None
     )
     sec_report_url: Optional[str] = Field(
-        description="""
-            The URL to the company's S-1, S-1/A, F-1, or F-1/A SEC filing,
-            which is required to be filed before an IPO takes place.
-        """,
+        description=(
+            "The URL to the company's S-1, S-1/A, F-1, or F-1/A SEC filing, which is required to be filed "
+            "before an IPO takes place."
+        ),
         default=None,
     )
     open_price: Optional[float] = Field(
         description="The opening price at the beginning of the first trading day (only available for priced IPOs).",
         default=None,
     )
     close_price: Optional[float] = Field(
@@ -120,32 +119,32 @@
         default=None,
     )
     volume: Optional[int] = Field(
         description="The volume at the end of the first trading day (only available for priced IPOs).",
         default=None,
     )
     day_change: Optional[float] = Field(
-        description="""
-            The percentage change between the open price and the close price on the first trading day
-            (only available for priced IPOs).
-        """,
+        description=(
+            "The percentage change between the open price and the close price on the first trading day "
+            "(only available for priced IPOs)."
+        ),
         default=None,
     )
     week_change: Optional[float] = Field(
-        description="""
-            The percentage change between the open price on the first trading day and the close price approximately
-            a week after the first trading day (only available for priced IPOs).
-        """,
+        description=(
+            "The percentage change between the open price on the first trading day and the close price approximately "
+            "a week after the first trading day (only available for priced IPOs)."
+        ),
         default=None,
     )
     month_change: Optional[float] = Field(
-        description="""
-            The percentage change between the open price on the first trading day and the close price approximately
-            a month after the first trading day (only available for priced IPOs).
-        """,
+        description=(
+            "The percentage change between the open price on the first trading day and the close price approximately "
+            "a month after the first trading day (only available for priced IPOs)."
+        ),
         default=None,
     )
     id: Optional[str] = Field(description="The Intrinio ID of the IPO.", default=None)
     company: Optional[IntrinioCompany] = Field(
         description="The company that is going public via the IPO.", default=None
     )
     security: Optional[IntrinioSecurity] = Field(
```

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/cash_flow.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/company_filings.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/company_news.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/company_news.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,24 +75,26 @@
             """Return the response."""
             if response.status != 200:
                 return []
 
             symbol = response.url.parts[-2]
             data = await response.json()
 
-            return [{**d, "symbol": symbol} for d in data.get("news", [])]
+            if isinstance(data, dict):
+                return [{**d, "symbol": symbol} for d in data.get("news", [])]
+            return []
 
         urls = [
             f"{base_url}/{symbol}/news?{query_str}&api_key={api_key}"
-            for symbol in [s.strip() for s in query.symbol.split(",")]
+            for symbol in [s.strip() for s in getattr(query, "symbol", "").split(",")]
         ]
 
         return await amake_requests(urls, callback, **kwargs)
 
     # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: IntrinioCompanyNewsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[IntrinioCompanyNewsData]:
         """Return the transformed data."""
         modeled_data = [IntrinioCompanyNewsData.model_validate(d) for d in data]
-        return filter_by_dates(modeled_data, query.start_date, query.end_date)  # type: ignore
+        return filter_by_dates(modeled_data, query.start_date, query.end_date)
```

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/currency_pairs.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/equity_historical.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/equity_info.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/equity_quote.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/equity_search.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/financial_attributes.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/financial_ratios.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/fred_series.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/historical_attributes.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/historical_dividends.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/income_statement.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/index_historical.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/insider_trading.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/institutional_ownership.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/key_metrics.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/latest_attributes.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/market_indices.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/options_chains.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/options_unusual.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/reported_financials.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/search_attributes.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/share_statistics.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/models/world_news.py` & `openbb_intrinio-1.1.4/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/openbb_intrinio/utils/helpers.py` & `openbb_intrinio-1.1.4/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.3/PKG-INFO` & `openbb_intrinio-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-intrinio
-Version: 1.1.3
+Version: 1.1.4
 Summary: Intrinio extension for OpenBB
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
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Intrinio Provider
 
 This extension integrates the [Intrinio](https://intrinio.com/) data provider into the OpenBB Platform.
```

