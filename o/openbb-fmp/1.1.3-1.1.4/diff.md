# Comparing `tmp/openbb_fmp-1.1.3.tar.gz` & `tmp/openbb_fmp-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fmp-1.1.3.tar", max compression
+gzip compressed data, was "openbb_fmp-1.1.4.tar", max compression
```

## Comparing `openbb_fmp-1.1.3.tar` & `openbb_fmp-1.1.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      478 2024-01-17 14:26:16.735057 openbb_fmp-1.1.3/README.md
--rw-r--r--   0        0        0     8052 2024-03-11 10:41:33.400139 openbb_fmp-1.1.3/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-01-17 14:26:16.735305 openbb_fmp-1.1.3/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     1812 2024-01-26 17:52:27.964413 openbb_fmp-1.1.3/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-01-26 17:52:27.964536 openbb_fmp-1.1.3/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-02-06 11:54:53.227427 openbb_fmp-1.1.3/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-01-26 17:52:27.964755 openbb_fmp-1.1.3/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-02-06 11:54:53.227542 openbb_fmp-1.1.3/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-01-26 17:52:27.964845 openbb_fmp-1.1.3/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-01-17 14:26:16.735972 openbb_fmp-1.1.3/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-02-06 11:54:53.227667 openbb_fmp-1.1.3/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-01-26 17:52:27.965059 openbb_fmp-1.1.3/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     2365 2024-01-17 14:26:16.736191 openbb_fmp-1.1.3/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2971 2024-02-26 09:52:50.862019 openbb_fmp-1.1.3/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-01-17 14:26:16.736360 openbb_fmp-1.1.3/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5069 2024-03-11 10:41:33.400303 openbb_fmp-1.1.3/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-02-23 17:14:57.460235 openbb_fmp-1.1.3/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5064 2024-03-11 10:41:33.400421 openbb_fmp-1.1.3/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-01-26 17:52:27.965382 openbb_fmp-1.1.3/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6022 2024-03-11 10:41:33.400708 openbb_fmp-1.1.3/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-01-17 14:26:16.736707 openbb_fmp-1.1.3/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-01-26 17:52:27.965478 openbb_fmp-1.1.3/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-01-26 17:52:27.965578 openbb_fmp-1.1.3/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5078 2024-03-11 10:41:33.400898 openbb_fmp-1.1.3/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-01-17 14:26:16.736981 openbb_fmp-1.1.3/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-02-23 17:14:57.460712 openbb_fmp-1.1.3/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     5330 2024-02-23 17:14:57.460829 openbb_fmp-1.1.3/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     4587 2024-02-23 17:14:57.460975 openbb_fmp-1.1.3/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-01-17 14:26:16.737193 openbb_fmp-1.1.3/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6017 2024-02-23 17:14:57.461084 openbb_fmp-1.1.3/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     2893 2024-02-23 17:14:57.461200 openbb_fmp-1.1.3/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     2955 2024-02-23 17:14:57.461276 openbb_fmp-1.1.3/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6777 2024-02-23 17:14:57.461405 openbb_fmp-1.1.3/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-01-17 14:26:16.737503 openbb_fmp-1.1.3/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2774 2024-02-23 17:14:57.461509 openbb_fmp-1.1.3/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3621 2024-02-23 17:14:57.461609 openbb_fmp-1.1.3/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-03-11 10:41:33.401042 openbb_fmp-1.1.3/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-01-17 14:26:16.737773 openbb_fmp-1.1.3/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     3414 2024-02-23 17:14:57.461713 openbb_fmp-1.1.3/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0     9875 2024-02-06 11:54:53.228700 openbb_fmp-1.1.3/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     3771 2024-02-06 11:54:53.228809 openbb_fmp-1.1.3/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-01-17 14:26:16.738126 openbb_fmp-1.1.3/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-01-17 14:26:16.738200 openbb_fmp-1.1.3/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-01-17 14:26:16.738260 openbb_fmp-1.1.3/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-02-06 11:54:53.229116 openbb_fmp-1.1.3/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-01-17 14:26:16.738443 openbb_fmp-1.1.3/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-02-23 17:14:57.461832 openbb_fmp-1.1.3/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5116 2024-03-11 10:41:33.401163 openbb_fmp-1.1.3/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-01-17 14:26:16.738584 openbb_fmp-1.1.3/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-01-17 14:26:16.738782 openbb_fmp-1.1.3/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2064 2024-01-17 14:26:16.738886 openbb_fmp-1.1.3/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10111 2024-02-23 17:14:57.462052 openbb_fmp-1.1.3/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3903 2024-01-29 13:09:03.809492 openbb_fmp-1.1.3/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     5922 2024-03-11 10:41:33.401502 openbb_fmp-1.1.3/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     2782 2024-02-23 17:14:57.462155 openbb_fmp-1.1.3/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     3337 2024-02-23 17:14:57.462251 openbb_fmp-1.1.3/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     1824 2024-01-17 14:26:16.739587 openbb_fmp-1.1.3/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.739612 openbb_fmp-1.1.3/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-01-26 17:52:27.966210 openbb_fmp-1.1.3/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-01-26 17:52:27.966303 openbb_fmp-1.1.3/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-01-17 14:26:16.739811 openbb_fmp-1.1.3/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-01-17 14:26:16.739873 openbb_fmp-1.1.3/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-02-23 17:14:57.462345 openbb_fmp-1.1.3/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-02-23 17:14:57.462435 openbb_fmp-1.1.3/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.740037 openbb_fmp-1.1.3/openbb_fmp/py.typed
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.740106 openbb_fmp-1.1.3/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-03-11 10:41:33.401608 openbb_fmp-1.1.3/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     5246 2024-01-19 11:57:23.718194 openbb_fmp-1.1.3/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.740276 openbb_fmp-1.1.3/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0      433 2024-03-11 19:59:44.604031 openbb_fmp-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_fmp-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      478 2024-02-29 11:03:36.842618 openbb_fmp-1.1.4/README.md
+-rw-r--r--   0        0        0     8111 2024-03-21 17:38:35.639684 openbb_fmp-1.1.4/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-29 11:03:36.842842 openbb_fmp-1.1.4/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-03-22 12:40:11.813669 openbb_fmp-1.1.4/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-03-21 17:38:35.639999 openbb_fmp-1.1.4/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-03-21 17:38:35.640233 openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-03-21 17:38:35.640374 openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-03-21 17:38:35.640519 openbb_fmp-1.1.4/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-03-21 17:38:35.640658 openbb_fmp-1.1.4/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-03-21 17:38:35.640811 openbb_fmp-1.1.4/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-03-21 17:38:35.640987 openbb_fmp-1.1.4/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-03-21 17:38:35.641081 openbb_fmp-1.1.4/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-03-22 12:40:11.813778 openbb_fmp-1.1.4/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-03-22 23:30:27.583357 openbb_fmp-1.1.4/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-03-21 17:38:35.641324 openbb_fmp-1.1.4/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-03-21 17:38:35.641450 openbb_fmp-1.1.4/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-03-21 17:38:35.641570 openbb_fmp-1.1.4/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-03-21 17:38:35.641674 openbb_fmp-1.1.4/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-03-21 17:38:35.641803 openbb_fmp-1.1.4/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6022 2024-03-13 16:36:51.716717 openbb_fmp-1.1.4/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-03-13 16:36:51.716848 openbb_fmp-1.1.4/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-03-21 17:38:35.641919 openbb_fmp-1.1.4/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-03-13 16:36:51.717093 openbb_fmp-1.1.4/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-03-21 17:38:35.642025 openbb_fmp-1.1.4/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-03-21 17:38:35.642174 openbb_fmp-1.1.4/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-03-21 17:38:35.642277 openbb_fmp-1.1.4/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-03-22 12:40:11.813889 openbb_fmp-1.1.4/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5202 2024-03-22 12:40:11.813998 openbb_fmp-1.1.4/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-03-21 17:38:35.642537 openbb_fmp-1.1.4/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-03-22 12:40:11.814104 openbb_fmp-1.1.4/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-03-22 12:40:11.814211 openbb_fmp-1.1.4/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-03-22 12:40:11.814334 openbb_fmp-1.1.4/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6763 2024-03-22 12:40:11.814453 openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-03-21 17:38:35.643273 openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2774 2024-03-21 17:38:35.643512 openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-03-22 12:40:11.814603 openbb_fmp-1.1.4/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-03-21 17:38:35.643652 openbb_fmp-1.1.4/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-03-21 17:38:35.643772 openbb_fmp-1.1.4/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-03-22 12:40:11.814715 openbb_fmp-1.1.4/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-03-22 12:40:11.814800 openbb_fmp-1.1.4/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     3771 2024-03-21 17:38:35.644149 openbb_fmp-1.1.4/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-03-21 17:38:35.644284 openbb_fmp-1.1.4/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-03-21 17:38:35.644395 openbb_fmp-1.1.4/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-03-21 17:38:35.644504 openbb_fmp-1.1.4/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-03-21 17:38:35.644732 openbb_fmp-1.1.4/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-03-21 17:38:35.644866 openbb_fmp-1.1.4/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-03-21 17:38:35.644977 openbb_fmp-1.1.4/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-03-21 17:38:35.645125 openbb_fmp-1.1.4/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-03-21 17:38:35.645341 openbb_fmp-1.1.4/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-03-21 17:38:35.645507 openbb_fmp-1.1.4/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2064 2024-03-21 17:38:35.645627 openbb_fmp-1.1.4/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-03-22 12:40:11.814898 openbb_fmp-1.1.4/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3903 2024-03-21 17:38:35.645747 openbb_fmp-1.1.4/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     5922 2024-03-21 17:38:35.645934 openbb_fmp-1.1.4/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3131 2024-03-22 12:40:11.815005 openbb_fmp-1.1.4/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-03-22 12:40:11.815106 openbb_fmp-1.1.4/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     2900 2024-03-22 12:40:11.815214 openbb_fmp-1.1.4/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847376 openbb_fmp-1.1.4/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-03-21 17:38:35.646414 openbb_fmp-1.1.4/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-03-21 17:38:35.646526 openbb_fmp-1.1.4/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-03-21 17:38:35.646630 openbb_fmp-1.1.4/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-03-21 17:38:35.646749 openbb_fmp-1.1.4/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-03-13 16:36:51.721845 openbb_fmp-1.1.4/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-03-13 16:36:51.721964 openbb_fmp-1.1.4/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847941 openbb_fmp-1.1.4/openbb_fmp/py.typed
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847991 openbb_fmp-1.1.4/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-03-13 16:36:51.722083 openbb_fmp-1.1.4/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4243 2024-03-22 12:40:11.815337 openbb_fmp-1.1.4/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.848164 openbb_fmp-1.1.4/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0      433 2024-04-01 14:20:54.437530 openbb_fmp-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_fmp-1.1.4/PKG-INFO
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/__init__.py` & `openbb_fmp-1.1.4/openbb_fmp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         "EquityValuationMultiples": FMPEquityValuationMultiplesFetcher,
         "EtfCountries": FMPEtfCountriesFetcher,
         "EtfEquityExposure": FMPEtfEquityExposureFetcher,
         "EtfHoldings": FMPEtfHoldingsFetcher,
         "EtfHoldingsDate": FMPEtfHoldingsDateFetcher,
         "EtfHoldingsPerformance": FMPEtfHoldingsPerformanceFetcher,
         "EtfInfo": FMPEtfInfoFetcher,
+        "EtfPricePerformance": FMPPricePerformanceFetcher,
         "EtfSearch": FMPEtfSearchFetcher,
         "EtfSectors": FMPEtfSectorsFetcher,
         "ExecutiveCompensation": FMPExecutiveCompensationFetcher,
         "FinancialRatios": FMPFinancialRatiosFetcher,
         "HistoricalDividends": FMPHistoricalDividendsFetcher,
         "HistoricalEmployees": FMPHistoricalEmployeesFetcher,
         "HistoricalEps": FMPHistoricalEpsFetcher,
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/available_indices.py` & `openbb_fmp-1.1.4/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/balance_sheet.py` & `openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/balance_sheet_growth.py` & `openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/calendar_dividend.py` & `openbb_fmp-1.1.4/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/calendar_earnings.py` & `openbb_fmp-1.1.4/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/calendar_splits.py` & `openbb_fmp-1.1.4/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/cash_flow.py` & `openbb_fmp-1.1.4/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/cash_flow_growth.py` & `openbb_fmp-1.1.4/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/company_filings.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_date.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,70 @@
-"""FMP Company Filings Model."""
+"""FMP ETF Holdings Model."""
 
-import math
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.company_filings import (
-    CompanyFilingsData,
-    CompanyFilingsQueryParams,
+from openbb_core.provider.standard_models.etf_holdings_date import (
+    EtfHoldingsDateData,
+    EtfHoldingsDateQueryParams,
 )
-from openbb_core.provider.utils.helpers import amake_requests, get_querystring
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_fmp.utils.helpers import create_url, get_data_many
+from pydantic import Field
 
 
-class FMPCompanyFilingsQueryParams(CompanyFilingsQueryParams):
-    """FMP Copmany Filings Query.
+class FMPEtfHoldingsDateQueryParams(EtfHoldingsDateQueryParams):
+    """FMP ETF Holdings Query.
 
-    Source: https://site.financialmodelingprep.com/developer/docs/sec-filings-api/
+    Source: https://site.financialmodelingprep.com/developer/docs#Historical-ETF-Holdings
     """
 
-    __alias_dict__ = {"form_type": "type"}
+    cik: Optional[str] = Field(
+        description=QUERY_DESCRIPTIONS.get("cik", "")
+        + "The CIK of the filing entity. Overrides symbol.",
+        default=None,
+    )
 
 
-class FMPCompanyFilingsData(CompanyFilingsData):
-    """FMP Company Filings Data."""
+class FMPEtfHoldingsDateData(EtfHoldingsDateData):
+    """FMP ETF Holdings Data."""
 
-    __alias_dict__ = {
-        "filing_date": "fillingDate",
-        "accepted_date": "acceptedDate",
-        "report_type": "type",
-        "filing_url": "link",
-        "report_url": "finalLink",
-    }
 
-
-class FMPCompanyFilingsFetcher(
+class FMPEtfHoldingsDateFetcher(
     Fetcher[
-        FMPCompanyFilingsQueryParams,
-        List[FMPCompanyFilingsData],
+        FMPEtfHoldingsDateQueryParams,
+        List[FMPEtfHoldingsDateData],
     ]
 ):
     """Transform the query, extract and transform the data from the FMP endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> FMPCompanyFilingsQueryParams:
-        """Transform the query params."""
-        return FMPCompanyFilingsQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> FMPEtfHoldingsDateQueryParams:
+        """Transform the query."""
+        return FMPEtfHoldingsDateQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: FMPCompanyFilingsQueryParams,
+        query: FMPEtfHoldingsDateQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
-        base_url = "https://financialmodelingprep.com/api/v3/sec_filings"
-        query_str = get_querystring(query.model_dump(by_alias=True), ["symbol"])
-
-        # FMP only allows 1000 results per page
-        pages = math.ceil(query.limit / 1000)
-
-        urls = [
-            f"{base_url}/{query.symbol}?{query_str}&page={page}&apikey={api_key}"
-            for page in range(pages)
-        ]
+        url = create_url(
+            version=4,
+            endpoint="etf-holdings/portfolio-date",
+            api_key=api_key,
+            query=query,
+        )
 
-        data = await amake_requests(urls, **kwargs)
-
-        return data[: query.limit]
+        return await get_data_many(url, **kwargs)
 
     @staticmethod
     def transform_data(
-        query: FMPCompanyFilingsQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[FMPCompanyFilingsData]:
+        query: FMPEtfHoldingsDateQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
+    ) -> List[FMPEtfHoldingsDateData]:
         """Return the transformed data."""
-        return [FMPCompanyFilingsData.model_validate(d) for d in data]
+        return [FMPEtfHoldingsDateData.model_validate(d) for d in data]
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/company_news.py` & `openbb_fmp-1.1.4/openbb_fmp/models/company_news.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: FMPCompanyNewsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPCompanyNewsData]:
         """Return the transformed data."""
         modeled_data = [FMPCompanyNewsData.model_validate(d) for d in data]
-        return filter_by_dates(modeled_data, query.start_date, query.end_date)  # type: ignore
+        return filter_by_dates(modeled_data, query.start_date, query.end_date)
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/company_overview.py` & `openbb_fmp-1.1.4/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/crypto_historical.py` & `openbb_fmp-1.1.4/openbb_fmp/models/crypto_historical.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """FMP Cryptos Historical Price Model."""
 
 # pylint: disable=unused-argument
 
-import warnings
+import asyncio
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
+from warnings import warn
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.crypto_historical import (
     CryptoHistoricalData,
     CryptoHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
-    ClientResponse,
-    amake_requests,
+    amake_request,
     get_querystring,
 )
 from openbb_fmp.utils.helpers import get_interval
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FMPCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """
     FMP Crypto Historical Price Query.
 
     Source:
     https://site.financialmodelingprep.com/developer/docs/cryptocurrency-historical-data-api/#Historical-Daily-Prices
@@ -100,48 +99,82 @@
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
                 url = f"{base_url}/historical-price-full/crypto/{url_params}"
             return url
 
-        # if there are more than 20 symbols, we need to increase the timeout
-        if len(query.symbol.split(",")) > 20:
-            kwargs.update({"preferences": {"request_timeout": 30}})
-
-        async def callback(response: ClientResponse, _: Any) -> List[Dict]:
-            data = await response.json()
-            symbol = response.url.parts[-1]
-            results = []
-            if not data:
-                _warn(f"No data found the the symbol: {symbol}")
-                return results
-
-            if isinstance(data, dict):
-                results = data.get("historical", [])
-
-            if "," in query.symbol:
-                for d in results:
-                    d["symbol"] = symbol
-            return results
+        symbols = query.symbol.split(",")
+
+        results = []
+        messages = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+
+            url = get_url_params(symbol)
+
+            data = []
+
+            response = await amake_request(url, **kwargs)
+
+            if isinstance(response, dict) and response.get("Error Message"):
+                message = f"Error fetching data for {symbol}: {response.get('Error Message', '')}"
+                warn(message)
+                messages.append(message)
 
-        urls = [get_url_params(symbol) for symbol in query.symbol.split(",")]
+            if not response:
+                message = f"No data found for {symbol}."
+                warn(message)
+                messages.append(message)
 
-        return await amake_requests(urls, callback, **kwargs)
+            if isinstance(response, list) and len(response) > 0:
+                data = response
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if isinstance(response, dict) and response.get("historical"):
+                data = response["historical"]
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if data:
+                results.extend(data)
+
+        tasks = [get_one(symbol) for symbol in symbols]
+
+        await asyncio.gather(*tasks)
+
+        if not results:
+            raise EmptyDataError(
+                f"{str(','.join(messages)).replace(',',' ') if messages else 'No data found'}"
+            )
+
+        return results
 
     @staticmethod
     def transform_data(
         query: FMPCryptoHistoricalQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPCryptoHistoricalData]:
         """Return the transformed data."""
 
         # Get rid of duplicate fields.
         to_pop = ["label", "changePercent", "unadjustedVolume"]
         results: List[FMPCryptoHistoricalData] = []
 
-        for d in sorted(data, key=lambda x: x["date"], reverse=False):
+        for d in sorted(
+            data,
+            key=lambda x: (
+                (x["date"], x["symbol"])
+                if len(query.symbol.split(",")) > 1
+                else x["date"]
+            ),
+            reverse=False,
+        ):
             _ = [d.pop(pop) for pop in to_pop if pop in d]
             if d.get("unadjusted_volume") == d.get("volume"):
                 _ = d.pop("unadjusted_volume")
             results.append(FMPCryptoHistoricalData.model_validate(d))
 
         return results
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/crypto_search.py` & `openbb_fmp-1.1.4/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/currency_historical.py` & `openbb_fmp-1.1.4/openbb_fmp/models/currency_historical.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """FMP Currency Historical Price Model."""
 
 # pylint: disable=unused-argument
 
-import warnings
+import asyncio
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
+from warnings import warn
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_historical import (
     CurrencyHistoricalData,
     CurrencyHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
-    ClientResponse,
-    amake_requests,
+    amake_request,
     get_querystring,
 )
 from openbb_fmp.utils.helpers import get_interval
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FMPCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """FMP Currency Historical Price Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Historical-Forex-Price
     """
 
@@ -98,48 +97,82 @@
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
                 url = f"{base_url}/historical-price-full/forex/{url_params}"
             return url
 
-        # if there are more than 20 symbols, we need to increase the timeout
-        if len(query.symbol.split(",")) > 20:
-            kwargs.update({"preferences": {"request_timeout": 30}})
-
-        async def callback(response: ClientResponse, _: Any) -> List[Dict]:
-            data = await response.json()
-            symbol = response.url.parts[-1]
-            results = []
-            if not data:
-                _warn(f"No data found the the symbol: {symbol}")
-                return results
-
-            if isinstance(data, dict):
-                results = data.get("historical", [])
-
-            if "," in query.symbol:
-                for d in results:
-                    d["symbol"] = symbol
-            return results
+        symbols = query.symbol.split(",")
+
+        results = []
+        messages = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+
+            url = get_url_params(symbol)
+
+            data = []
+
+            response = await amake_request(url, **kwargs)
+
+            if isinstance(response, dict) and response.get("Error Message"):
+                message = f"Error fetching data for {symbol}: {response.get('Error Message', '')}"
+                warn(message)
+                messages.append(message)
 
-        urls = [get_url_params(symbol) for symbol in query.symbol.split(",")]
+            if not response:
+                message = f"No data found for {symbol}."
+                warn(message)
+                messages.append(message)
 
-        return await amake_requests(urls, callback, **kwargs)
+            if isinstance(response, list) and len(response) > 0:
+                data = response
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if isinstance(response, dict) and response.get("historical"):
+                data = response["historical"]
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if data:
+                results.extend(data)
+
+        tasks = [get_one(symbol) for symbol in symbols]
+
+        await asyncio.gather(*tasks)
+
+        if not results:
+            raise EmptyDataError(
+                f"{str(','.join(messages)).replace(',',' ') if messages else 'No data found'}"
+            )
+
+        return results
 
     @staticmethod
     def transform_data(
         query: FMPCurrencyHistoricalQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPCurrencyHistoricalData]:
         """Return the transformed data."""
 
         # Get rid of duplicate fields.
         to_pop = ["label", "changePercent", "unadjustedVolume"]
         results: List[FMPCurrencyHistoricalData] = []
 
-        for d in sorted(data, key=lambda x: x["date"], reverse=False):
+        for d in sorted(
+            data,
+            key=lambda x: (
+                (x["date"], x["symbol"])
+                if len(query.symbol.split(",")) > 1
+                else x["date"]
+            ),
+            reverse=False,
+        ):
             _ = [d.pop(pop) for pop in to_pop if pop in d]
             if d.get("unadjusted_volume") == d.get("volume"):
                 _ = d.pop("unadjusted_volume")
             results.append(FMPCurrencyHistoricalData.model_validate(d))
 
         return results
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/currency_pairs.py` & `openbb_fmp-1.1.4/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/currency_snapshots.py` & `openbb_fmp-1.1.4/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/discovery_filings.py` & `openbb_fmp-1.1.4/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/earnings_call_transcript.py` & `openbb_fmp-1.1.4/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/economic_calendar.py` & `openbb_fmp-1.1.4/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_historical.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_historical.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """FMP Equity Historical Price Model."""
 
 # pylint: disable=unused-argument
 
-import warnings
+import asyncio
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
+from warnings import warn
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_historical import (
     EquityHistoricalData,
     EquityHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
-    ClientResponse,
-    amake_requests,
+    amake_request,
     get_querystring,
 )
 from openbb_fmp.utils.helpers import get_interval
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FMPEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """FMP Equity Historical Price Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Stock-Historical-Price
     """
 
@@ -101,48 +100,82 @@
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
                 url = f"{base_url}/historical-price-full/{url_params}"
             return url
 
-        # if there are more than 20 symbols, we need to increase the timeout
-        if len(query.symbol.split(",")) > 20:
-            kwargs.update({"preferences": {"request_timeout": 30}})
-
-        async def callback(response: ClientResponse, _: Any) -> List[Dict]:
-            data = await response.json()
-            symbol = response.url.parts[-1]
-            results = []
-            if not data:
-                _warn(f"No data found the the symbol: {symbol}")
-                return results
-
-            if isinstance(data, dict):
-                results = data.get("historical", [])
-
-            if "," in query.symbol:
-                for d in results:
-                    d["symbol"] = symbol
-            return results
+        symbols = query.symbol.split(",")
+
+        results = []
+        messages = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+
+            url = get_url_params(symbol)
+
+            data = []
+
+            response = await amake_request(url, **kwargs)
+
+            if isinstance(response, dict) and response.get("Error Message"):
+                message = f"Error fetching data for {symbol}: {response.get('Error Message', '')}"
+                warn(message)
+                messages.append(message)
 
-        urls = [get_url_params(symbol) for symbol in query.symbol.split(",")]
+            if not response:
+                message = f"No data found for {symbol}."
+                warn(message)
+                messages.append(message)
 
-        return await amake_requests(urls, callback, **kwargs)
+            if isinstance(response, list) and len(response) > 0:
+                data = response
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if isinstance(response, dict) and response.get("historical"):
+                data = response["historical"]
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if data:
+                results.extend(data)
+
+        tasks = [get_one(symbol) for symbol in symbols]
+
+        await asyncio.gather(*tasks)
+
+        if not results:
+            raise EmptyDataError(
+                f"{str(','.join(messages)).replace(',',' ') if messages else 'No data found'}"
+            )
+
+        return results
 
     @staticmethod
     def transform_data(
         query: FMPEquityHistoricalQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPEquityHistoricalData]:
         """Return the transformed data."""
 
         # Get rid of duplicate fields.
         to_pop = ["label", "changePercent"]
         results: List[FMPEquityHistoricalData] = []
 
-        for d in sorted(data, key=lambda x: x["date"], reverse=False):
+        for d in sorted(
+            data,
+            key=lambda x: (
+                (x["date"], x["symbol"])
+                if len(query.symbol.split(",")) > 1
+                else x["date"]
+            ),
+            reverse=False,
+        ):
             _ = [d.pop(pop) for pop in to_pop if pop in d]
             if d.get("unadjusted_volume") == d.get("volume"):
                 _ = d.pop("unadjusted_volume")
             results.append(FMPEquityHistoricalData.model_validate(d))
 
         return results
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_ownership.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_peers.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_profile.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """FMP Equity Profile Model."""
 
 # pylint: disable=unused-argument
 
+import asyncio
 from datetime import (
     date as dateType,
 )
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_info import (
     EquityInfoData,
     EquityInfoQueryParams,
 )
-from openbb_core.provider.utils.helpers import amake_requests
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import response_callback
 from pydantic import Field, field_validator, model_validator
 
 
 class FMPEquityProfileQueryParams(EquityInfoQueryParams):
     """FMP Equity Profile Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/companies-key-stats-free-api/
@@ -122,17 +126,38 @@
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         symbols = query.symbol.split(",")
         base_url = "https://financialmodelingprep.com/api/v3"
-        urls = [f"{base_url}/profile/{symbol}?apikey={api_key}" for symbol in symbols]
 
-        return await amake_requests(urls, **kwargs)
+        results = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+            url = f"{base_url}/profile/{symbol}?apikey={api_key}"
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+            if not result:
+                warn(f"Symbol Error: No data found for {symbol}")
+
+            if result:
+                results.append(result[0])
+
+        await asyncio.gather(*[get_one(symbol) for symbol in symbols])
+
+        if not results:
+            raise EmptyDataError("No data found for the given symbols.")
+
+        return sorted(
+            results,
+            key=(lambda item: (symbols.index(item.get("symbol", len(symbols))))),
+        )
 
     @staticmethod
     def transform_data(
         query: FMPEquityProfileQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FMPEquityProfileData]:
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_quote.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_quote.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """FMP Equity Quote Model."""
 
+import asyncio
 from datetime import datetime, timezone
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_quote import (
     EquityQuoteData,
     EquityQuoteQueryParams,
 )
-from openbb_core.provider.utils.helpers import amake_requests
-from openbb_fmp.utils.helpers import get_querystring
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import get_querystring, response_callback
 from pydantic import Field, field_validator
 
 
 class FMPEquityQuoteQueryParams(EquityQuoteQueryParams):
     """FMP Equity Quote Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Stock-Historical-Price
@@ -50,24 +53,26 @@
         default=None, description="Market cap of the company."
     )
     shares_outstanding: Optional[ForceInt] = Field(
         default=None, description="Number of shares outstanding."
     )
     eps: Optional[float] = Field(default=None, description="Earnings per share.")
     pe: Optional[float] = Field(default=None, description="Price earnings ratio.")
-    earnings_announcement: Optional[Union[datetime, str]] = Field(
+    earnings_announcement: Optional[datetime] = Field(
         default=None, description="Upcoming earnings announcement date."
     )
 
     @field_validator("last_timestamp", mode="before", check_fields=False)
     @classmethod
     def validate_last_timestamp(cls, v):  # pylint: disable=E0213
         """Return the date as a datetime object."""
-        v = int(v) if isinstance(v, str) else v
-        return datetime.utcfromtimestamp(int(v)).replace(tzinfo=timezone.utc)
+        if v:
+            v = int(v) if isinstance(v, str) else v
+            return datetime.fromtimestamp(int(v), tz=timezone.utc)
+        return None
 
     @field_validator("earnings_announcement", mode="before", check_fields=False)
     @classmethod
     def timestamp_validate(cls, v):  # pylint: disable=E0213
         """Return the datetime string as a datetime object."""
         if v:
             dt = datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.%f%z")
@@ -105,24 +110,37 @@
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         symbols = query.symbol.split(",")
-        symbols_split = [
-            ",".join(symbols[i : i + 10]) for i in range(0, len(symbols), 10)
-        ]
-
-        urls = [
-            f"{base_url}/quote/{symbol}?{query_str}&apikey={api_key}"
-            for symbol in symbols_split
-        ]
 
-        return await amake_requests(urls, **kwargs)
+        results = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+            url = f"{base_url}/quote/{symbol}?{query_str}&apikey={api_key}"
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+            if not result or len(result) == 0:
+                warn(f"Symbol Error: No data found for {symbol}")
+            if result and len(result) > 0:
+                results.extend(result)
+
+        await asyncio.gather(*[get_one(s) for s in symbols])
+
+        if not results:
+            raise EmptyDataError("No data found for the given symbols.")
+
+        return sorted(
+            results,
+            key=(lambda item: (symbols.index(item.get("symbol", len(symbols))))),
+        )
 
     @staticmethod
     def transform_data(
         query: FMPEquityQuoteQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPEquityQuoteData]:
         """Return the transformed data."""
         return [FMPEquityQuoteData.model_validate(d) for d in data]
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_screener.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_fmp-1.1.4/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """FMP Equity Valuation Multiples Model."""
 
+# pylint: disable=unused-argument
+
+import asyncio
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_valuation_multiples import (
     EquityValuationMultiplesData,
     EquityValuationMultiplesQueryParams,
 )
-from openbb_core.provider.utils.helpers import ClientResponse, amake_requests
-from openbb_fmp.utils.helpers import create_url
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import create_url, response_callback
 
 
 class FMPEquityValuationMultiplesQueryParams(EquityValuationMultiplesQueryParams):
     """FMP Equity Valuation Multiples Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Company-Key-Metrics
     """
@@ -107,28 +112,41 @@
     async def aextract_data(
         query: FMPEquityValuationMultiplesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
-        urls = [
-            create_url(
+
+        symbols = query.symbol.split(",")
+
+        results = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+            url = create_url(
                 3, f"key-metrics-ttm/{symbol}", api_key, query, exclude=["symbol"]
             )
-            for symbol in query.symbol.split(",")
-        ]
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+            if not result:
+                warn(f"Symbol Error: No data found for {symbol}.")
+            if result:
+                data = [{**d, "symbol": symbol} for d in result]
+                results.extend(data)
 
-        async def callback(response: ClientResponse, _: Any) -> List[Dict]:
-            data = await response.json()
-            symbol = response.url.parts[-1]
+        await asyncio.gather(*[get_one(symbol) for symbol in symbols])
 
-            return [{**d, "symbol": symbol} for d in data]
+        if not results:
+            raise EmptyDataError("No data found for given symbols.")
 
-        return await amake_requests(urls, callback, **kwargs)
+        return results
 
     @staticmethod
     def transform_data(
-        query: FMPEquityValuationMultiplesQueryParams, data: List[Dict], **kwargs: Any
+        query: FMPEquityValuationMultiplesQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
     ) -> List[FMPEquityValuationMultiplesData]:
         """Return the transformed data."""
         return [FMPEquityValuationMultiplesData.model_validate(d) for d in data]
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_countries.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_countries.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """FMP ETF Countries Model."""
 
+import asyncio
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
-import pandas as pd
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_countries import (
     EtfCountriesData,
     EtfCountriesQueryParams,
 )
-from openbb_fmp.utils.helpers import create_url, get_data_many
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import create_url, response_callback
+from pandas import DataFrame
 
 
 class FMPEtfCountriesQueryParams(EtfCountriesQueryParams):
     """FMP ETF Countries Query."""
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
@@ -38,47 +42,58 @@
     async def aextract_data(
         query: FMPEtfCountriesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
-        symbols = (
-            query.symbol.split(",") if "," in query.symbol else [query.symbol.upper()]
-        )
+        symbols = query.symbol.split(",")
         results = {}
 
-        for symbol in symbols:
+        async def get_one(symbol):
+            """Get data for one symbol."""
             data = {}
             url = create_url(
                 version=3,
                 endpoint=f"etf-country-weightings/{symbol}",
                 api_key=api_key,
             )
-            result = await get_data_many(url, **kwargs)
-            df = pd.DataFrame(result).set_index("country")
-            if len(df) > 0:
-                for i in df.index:
-                    data.update(
-                        {
-                            i: float(df.loc[i]["weightPercentage"].replace("%", ""))
-                            * 0.01
-                        }
-                    )
-                results.update({symbol: data})
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+
+            if not result:
+                warn(f"Symbol Error: No data found for {symbol}")
+
+            if result:
+                df = DataFrame(result).set_index("country")
+                if len(df) > 0:
+                    for i in df.index:
+                        data.update(
+                            {
+                                i: float(df.loc[i]["weightPercentage"].replace("%", ""))
+                                * 0.01
+                            }
+                        )
+                    results.update({symbol: data})
+
+        await asyncio.gather(*[get_one(symbol) for symbol in symbols])
+
+        if not results:
+            raise EmptyDataError("No data found for the given symbols.")
 
         output = (
-            pd.DataFrame(results)
+            DataFrame(results)
             .transpose()
             .reset_index()
             .fillna(value=0)
             .replace(0, None)
             .rename(columns={"index": "symbol"})
         ).transpose()
-        output.columns = output.loc["symbol"].to_list()
+        output.columns = output.loc["symbol"].to_list()  # type: ignore
         output = output.drop("symbol", axis=0).sort_values(
             by=output.columns[0], ascending=False
         )
 
         return (
             output.reset_index().rename(columns={"index": "country"}).to_dict("records")
         )
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_equity_exposure.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_equity_exposure.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """FMP ETF Equity Exposure Model."""
 
 # pylint: disable=unused-argument
 
 import asyncio
-import warnings
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_equity_exposure import (
     EtfEquityExposureData,
     EtfEquityExposureQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import response_callback
 from pydantic import field_validator
 
-_warn = warnings.warn
-
 
 class FMPEtfEquityExposureQueryParams(EtfEquityExposureQueryParams):
     """
     FMP ETF Equity Exposure Query Params.
 
     Source: https://site.financialmodelingprep.com/developer/docs/etf-stock-exposure-api/
     """
@@ -66,23 +65,26 @@
         api_key = credentials.get("fmp_api_key") if credentials else ""
         symbols = query.symbol.split(",")
         results = []
 
         async def get_one(symbol):
             """Get one symbol."""
             url = f"https://financialmodelingprep.com/api/v3/etf-stock-exposure/{symbol}?apikey={api_key}"
-            response = await amake_request(url)
+            response = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
             if not response:
-                _warn(f"No results found for {symbol}.")
-            results.extend(response)
+                warn(f"No results found for {symbol}.")
+            if response:
+                results.extend(response)
 
         await asyncio.gather(*[get_one(symbol) for symbol in symbols])
 
         if not results:
-            raise EmptyDataError()
+            raise EmptyDataError("No data was found for the given symbols.")
 
         return results
 
     @staticmethod
     def transform_data(
         query: FMPEtfEquityExposureQueryParams,
         data: List[Dict],
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_holdings.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """FMP ETF Holdings Model."""
 
 # pylint: disable=unused-argument
 
-import warnings
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import Any, Dict, List, Optional, Union
+from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_holdings import (
     EtfHoldingsData,
     EtfHoldingsQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
 from openbb_fmp.utils.helpers import create_url, get_data_many
 from pydantic import Field, field_validator
 
-_warn = warnings.warn
-
 
 class FMPEtfHoldingsQueryParams(EtfHoldingsQueryParams):
     """FMP ETF Holdings Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs#Historical-ETF-Holdings
     """
 
@@ -170,15 +168,15 @@
         if query.date is not None:
             url = create_url(
                 version=4, endpoint="etf-holdings", api_key=api_key, query=query
             )
             try:
                 data = await get_data_many(url, **kwargs)
             except Exception:
-                _warn(
+                warn(
                     "No data found for this symbol and date, attempting to retrieve the most recent data available."
                 )
 
         if query.date is None or not data:
             url = f"https://financialmodelingprep.com/api/v3/etf-holder/{query.symbol}?apikey={api_key}"
             data = await get_data_many(url, **kwargs)
         return data
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_holdings_performance.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_info.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """FMP ETF Info Model."""
 
 # pylint: disable=unused-argument
 
 import asyncio
-import warnings
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_info import (
     EtfInfoData,
     EtfInfoQueryParams,
 )
 from openbb_core.provider.utils.helpers import amake_request
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FMPEtfInfoQueryParams(EtfInfoQueryParams):
     """FMP ETF Info Query."""
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
 
@@ -81,15 +79,15 @@
         results = []
 
         async def get_one(symbol):
             """Get one symbol."""
             url = f"https://financialmodelingprep.com/api/v4/etf-info?symbol={symbol}&apikey={api_key}"
             response = await amake_request(url)
             if not response:
-                _warn(f"No results found for {symbol}.")
+                warn(f"No results found for {symbol}.")
             results.extend(response)
 
         await asyncio.gather(*[get_one(symbol) for symbol in symbols])
 
         return results
 
     @staticmethod
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_search.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/etf_sectors.py` & `openbb_fmp-1.1.4/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/executive_compensation.py` & `openbb_fmp-1.1.4/openbb_fmp/models/executive_compensation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,125 @@
 """FMP Executive Compensation Model."""
 
-from datetime import datetime, timedelta
+import asyncio
+from datetime import (
+    date as dateType,
+    datetime,
+)
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.executive_compensation import (
     ExecutiveCompensationData,
     ExecutiveCompensationQueryParams,
 )
-from openbb_core.provider.utils.helpers import amake_requests
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
 from openbb_fmp.utils.helpers import response_callback
-from pydantic import field_validator
+from pydantic import Field, field_validator
 
 
 class FMPExecutiveCompensationQueryParams(ExecutiveCompensationQueryParams):
     """FMP Executive Compensation Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/executive-compensation-api/
     """
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
+    year: Optional[int] = Field(default=None, description="Year of the compensation.")
+
 
 class FMPExecutiveCompensationData(ExecutiveCompensationData):
     """FMP Executive Compensation Data."""
 
+    __alias_dict__ = {
+        "company_name": "companyName",
+        "industry": "industryTitle",
+    }
+
+    filing_date: Optional[dateType] = Field(
+        default=None, description="Date of the filing."
+    )
+    accepted_date: Optional[datetime] = Field(
+        default=None, description="Date the filing was accepted."
+    )
+    url: Optional[str] = Field(default=None, description="URL to the filing data.")
+
     @field_validator("filingDate", mode="before", check_fields=False)
     @classmethod
     def filing_date_validate(cls, v):  # pylint: disable=E0213
         """Return the filing date as a datetime object."""
         return datetime.strptime(v, "%Y-%m-%d")
 
     @field_validator("acceptedDate", mode="before", check_fields=False)
     @classmethod
     def accepted_date_validate(cls, v):  # pylint: disable=E0213
         """Return the accepted date as a datetime object."""
         return datetime.strptime(v, "%Y-%m-%d %H:%M:%S")
 
 
 class FMPExecutiveCompensationFetcher(
-    Fetcher[  # type: ignore
+    Fetcher[
         FMPExecutiveCompensationQueryParams,
         List[FMPExecutiveCompensationData],
     ]
 ):
     """Transform the query, extract and transform the data from the FMP endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> FMPExecutiveCompensationQueryParams:
         """Transform the query params."""
-        transformed_params = params
-        now = datetime.now().date()
-        if params.get("start_date") is None:
-            transformed_params["start_date"] = now - timedelta(days=10 * 365)
-
-        if params.get("end_date") is None:
-            transformed_params["end_date"] = now
-
-        return FMPExecutiveCompensationQueryParams(**transformed_params)
+        return FMPExecutiveCompensationQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: FMPExecutiveCompensationQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
+
         api_key = credentials.get("fmp_api_key") if credentials else ""
+
         base_url = "https://financialmodelingprep.com/api/v4/"
-        urls = [
-            f"{base_url}/governance/executive_compensation?symbol={s.strip()}&apikey={api_key}"
-            for s in query.symbol.split(",")
-        ]
-        return await amake_requests(urls, response_callback, **kwargs)
+
+        symbols = query.symbol.split(",")
+
+        results = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+
+            url = f"{base_url}/governance/executive_compensation?symbol={symbol}&apikey={api_key}"
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+            if not result:
+                warn(f"Symbol Error: No data found for {symbol}.")
+
+            if result:
+                results.extend(result)
+
+        await asyncio.gather(*[get_one(symbol) for symbol in symbols])
+
+        if not results:
+            raise EmptyDataError("No data found for given symbols.")
+
+        return sorted(results, key=lambda x: (x["year"]), reverse=True)
 
     @staticmethod
     def transform_data(
-        query: FMPExecutiveCompensationQueryParams, data: List[Dict], **kwargs: Any
+        query: FMPExecutiveCompensationQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
     ) -> List[FMPExecutiveCompensationData]:
         """Return the transformed data."""
-        result = []
+        results: List[FMPExecutiveCompensationData] = []
         for d in data:
-            if "year" in d:
-                if (
-                    d["year"] >= query.start_date.year
-                    and d["year"] <= query.end_date.year
-                ):
-                    result.append(FMPExecutiveCompensationData(**d))
+            if "year" in d and query.year is not None:
+                if d["year"] >= query.year and d["year"] <= query.year:
+                    results.append(FMPExecutiveCompensationData.model_validate(d))
             else:
-                result.append(FMPExecutiveCompensationData(**d))
-        return result
+                results.append(FMPExecutiveCompensationData.model_validate(d))
+        return results
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/financial_ratios.py` & `openbb_fmp-1.1.4/openbb_fmp/models/financial_ratios.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.financial_ratios import (
     FinancialRatiosData,
     FinancialRatiosQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
-    amake_requests,
+    amake_request,
     to_snake_case,
 )
+from openbb_fmp.utils.helpers import response_callback
 from pydantic import Field, model_validator
 
 
 class FMPFinancialRatiosQueryParams(FinancialRatiosQueryParams):
     """FMP Financial Ratios Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Company-Financial-Ratios
@@ -228,17 +230,22 @@
 
         url = (
             f"{base_url}/ratios/{query.symbol}?"
             f"period={query.period}&limit={query.limit}&apikey={api_key}"
             if query.period != "ttm"
             else ttm_url
         )
-        results = await amake_requests(url, **kwargs)
+        results = await amake_request(
+            url, response_callback=response_callback, **kwargs
+        )
+
+        if not results:
+            raise EmptyDataError(f"No data found for the symbol {query.symbol}.")
 
-        return results
+        return results  # type: ignore
 
     @staticmethod
     def transform_data(
         query: FMPFinancialRatiosQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPFinancialRatiosData]:
         """Return the transformed data."""
         results = [
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/historical_dividends.py` & `openbb_fmp-1.1.4/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/historical_employees.py` & `openbb_fmp-1.1.4/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/historical_eps.py` & `openbb_fmp-1.1.4/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/historical_splits.py` & `openbb_fmp-1.1.4/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/income_statement.py` & `openbb_fmp-1.1.4/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/income_statement_growth.py` & `openbb_fmp-1.1.4/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/index_constituents.py` & `openbb_fmp-1.1.4/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/index_historical.py` & `openbb_fmp-1.1.4/openbb_fmp/models/index_historical.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 """FMP Index Historical Model."""
 
 # pylint: disable=unused-argument
 
-import warnings
+import asyncio
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
+from warnings import warn
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.index_historical import (
     IndexHistoricalData,
     IndexHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
-    ClientResponse,
-    amake_requests,
+    amake_request,
     get_querystring,
 )
 from openbb_fmp.utils.helpers import get_interval
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FMPIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """FMP Index Historical Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/historical-index-price-api/
     """
 
@@ -99,38 +97,63 @@
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
                 url = f"{base_url}/historical-price-full/{url_params}"
             return url
 
-        # if there are more than 20 symbols, we need to increase the timeout
-        if len(query.symbol.split(",")) > 20:
-            kwargs.update({"preferences": {"request_timeout": 30}})
-
-        async def callback(response: ClientResponse, _: Any) -> List[Dict]:
-            data = await response.json()
-            symbol = response.url.parts[-1]
-            results = []
-            if not data:
-                _warn(f"No data found the the symbol: {symbol}")
-                return results
-
-            if isinstance(data, dict):
-                results = data.get("historical", [])
-            if isinstance(data, list):
-                results = data
-
-            if "," in query.symbol:
-                for d in results:
-                    d["symbol"] = symbol
-            return results
+        symbols = query.symbol.split(",")
+
+        results = []
+        messages = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+
+            url = get_url_params(symbol)
+
+            data = []
+
+            response = await amake_request(url, **kwargs)
+
+            if isinstance(response, dict) and response.get("Error Message"):
+                message = f"Error fetching data for {symbol}: {response.get('Error Message', '')}"
+                warn(message)
+                messages.append(message)
+
+            if not response:
+                message = f"No data found for {symbol}."
+                warn(message)
+                messages.append(message)
 
-        urls = [get_url_params(symbol) for symbol in query.symbol.split(",")]
-        return await amake_requests(urls, callback, **kwargs)
+            if isinstance(response, list) and len(response) > 0:
+                data = response
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if isinstance(response, dict) and response.get("historical"):
+                data = response["historical"]
+                if len(symbols) > 1:
+                    for d in data:
+                        d["symbol"] = symbol
+
+            if data:
+                results.extend(data)
+
+        tasks = [get_one(symbol) for symbol in symbols]
+
+        await asyncio.gather(*tasks)
+
+        if not results:
+            raise EmptyDataError(
+                f"{str(','.join(messages)).replace(',',' ') if messages else 'No data found'}"
+            )
+
+        return results
 
     @staticmethod
     def transform_data(
         query: FMPIndexHistoricalQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FMPIndexHistoricalData]:
@@ -138,14 +161,22 @@
         if not data:
             raise EmptyDataError()
 
         # Get rid of duplicate fields.
         to_pop = ["label", "changePercent", "unadjustedVolume", "adjClose"]
         results: List[FMPIndexHistoricalData] = []
 
-        for d in sorted(data, key=lambda x: x["date"], reverse=False):
+        for d in sorted(
+            data,
+            key=lambda x: (
+                (x["date"], x["symbol"])
+                if len(query.symbol.split(",")) > 1
+                else x["date"]
+            ),
+            reverse=False,
+        ):
             _ = [d.pop(pop) for pop in to_pop if pop in d]
             if d.get("volume") == 0:
                 _ = d.pop("volume")
             results.append(FMPIndexHistoricalData.model_validate(d))
 
         return results
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/insider_trading.py` & `openbb_fmp-1.1.4/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/institutional_ownership.py` & `openbb_fmp-1.1.4/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/key_executives.py` & `openbb_fmp-1.1.4/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/key_metrics.py` & `openbb_fmp-1.1.4/openbb_fmp/models/key_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """FMP Key Metrics Model."""
 
+import asyncio
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.key_metrics import (
     KeyMetricsData,
     KeyMetricsQueryParams,
 )
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
-from openbb_core.provider.utils.helpers import (
-    ClientResponse,
-    ClientSession,
-    amake_requests,
-)
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import response_callback
 from pydantic import Field
 
 
 class FMPKeyMetricsQueryParams(KeyMetricsQueryParams):
     """FMP Key Metrics Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/company-key-metrics-api/
@@ -223,43 +223,56 @@
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         base_url = "https://financialmodelingprep.com/api/v3"
 
-        async def response_callback(
-            response: ClientResponse, session: ClientSession
-        ) -> List[Dict]:
-            results = await response.json()
-            symbol = response.url.parts[-1]
-
-            # TTM data
-            ttm_url = f"{base_url}/key-metrics-ttm/{symbol}?&apikey={api_key}"
-            if query.with_ttm and (metrics_ttm := await session.get_one(ttm_url)):
-                results.insert(
-                    0,
-                    {
-                        "symbol": symbol,
-                        "period": "TTM",
-                        "date": datetime.now().strftime("%Y-%m-%d"),
-                        "calendar_year": datetime.now().year,
-                        **{k.replace("TTM", ""): v for k, v in metrics_ttm.items()},
-                    },
-                )
-
-            return results
-
-        urls = [
-            f"{base_url}/key-metrics/{symbol}?"
-            f"period={query.period}&limit={query.limit}&apikey={api_key}"
-            for symbol in query.symbol.split(",")
-        ]
+        symbols = query.symbol.split(",")
+
+        results = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+
+            url = f"{base_url}/key-metrics/{symbol}?period={query.period}&limit={query.limit}&apikey={api_key}"
+
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+
+            if not result:
+                warn(f"Symbol Error: No data found for {symbol}.")
+
+            if result:
+
+                ttm_url = f"{base_url}/key-metrics-ttm/{symbol}?&apikey={api_key}"
+                if query.with_ttm and (
+                    metrics_ttm := await amake_request(
+                        ttm_url, response_callback=response_callback, **kwargs
+                    )
+                ):
+                    result.insert(  # type: ignore
+                        0,
+                        {
+                            "symbol": symbol,
+                            "period": "TTM",
+                            "date": datetime.now().strftime("%Y-%m-%d"),
+                            "calendar_year": datetime.now().year,
+                            **{k.replace("TTM", ""): v for k, v in metrics_ttm.items()},  # type: ignore
+                        },
+                    )
+                results.extend(result)
+
+        await asyncio.gather(*[get_one(symbol) for symbol in symbols])
+
+        if not results:
+            raise EmptyDataError("No data found for given symbols.")
 
-        return await amake_requests(urls, response_callback=response_callback, **kwargs)
+        return results
 
     @staticmethod
     def transform_data(
         query: FMPKeyMetricsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPKeyMetricsData]:
         """Return the transformed data."""
         return [FMPKeyMetricsData.model_validate(d) for d in data]
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/market_indices.py` & `openbb_fmp-1.1.4/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/market_snapshots.py` & `openbb_fmp-1.1.4/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/price_performance.py` & `openbb_fmp-1.1.4/openbb_fmp/models/price_performance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """FMP Price Performance Model."""
 
 # pylint: disable=unused-argument
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.recent_performance import (
     RecentPerformanceData,
     RecentPerformanceQueryParams,
 )
 from openbb_fmp.utils.helpers import create_url, get_data_many
@@ -82,8 +83,17 @@
     @staticmethod
     def transform_data(
         query: FMPPricePerformanceQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FMPPricePerformanceData]:
         """Return the transformed data."""
+
+        symbols = query.symbol.split(",")
+        if len(data) != len(symbols):
+            data_symbols = [d["symbol"] for d in data]
+            missing_symbols = [
+                symbol for symbol in symbols if symbol not in data_symbols
+            ]
+            warn(f"Missing data for symbols: {missing_symbols}")
+
         return [FMPPricePerformanceData.model_validate(i) for i in data]
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/price_target.py` & `openbb_fmp-1.1.4/openbb_fmp/models/analyst_estimates.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,90 @@
-"""FMP Equity Ownership Model."""
+"""FMP Analyst Estimates Model."""
 
-# pylint: disable=unused-argument
-
-from datetime import datetime
-from typing import Any, Dict, List, Optional
+import asyncio
+from typing import Any, Dict, List, Literal, Optional
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.price_target import (
-    PriceTargetData,
-    PriceTargetQueryParams,
+from openbb_core.provider.standard_models.analyst_estimates import (
+    AnalystEstimatesData,
+    AnalystEstimatesQueryParams,
 )
-from openbb_fmp.utils.helpers import create_url, get_data_urls
-from pydantic import Field, field_validator
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_fmp.utils.helpers import create_url, response_callback
+from pydantic import Field
 
 
-class FMPPriceTargetQueryParams(PriceTargetQueryParams):
-    """FMP Price Target Query.
+class FMPAnalystEstimatesQueryParams(AnalystEstimatesQueryParams):
+    """FMP Analyst Estimates Query.
 
-    Source: https://site.financialmodelingprep.com/developer/docs/#Price-Target
+    Source: https://site.financialmodelingprep.com/developer/docs/analyst-estimates-api/
     """
 
-    with_grade: bool = Field(
-        False,
-        description="Include upgrades and downgrades in the response.",
-    )
-
+    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
-class FMPPriceTargetData(PriceTargetData):
-    """FMP Price Target Data."""
-
-    __alias_dict__ = {
-        "analyst_firm": "gradingCompany",
-        "rating_current": "newGrade",
-        "rating_previous": "previousGrade",
-        "news_title": "newsTitle",
-        "url_news": "newsURL",
-        "url_base": "newsBaseURL",
-    }
-
-    news_url: Optional[str] = Field(
-        default=None, description="News URL of the price target."
-    )
-    news_title: Optional[str] = Field(
-        default=None, description="News title of the price target."
+    period: Literal["quarter", "annual"] = Field(
+        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
     )
-    news_publisher: Optional[str] = Field(
-        default=None, description="News publisher of the price target."
-    )
-    news_base_url: Optional[str] = Field(
-        default=None, description="News base URL of the price target."
+    limit: Optional[int] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
 
-    @field_validator("published_date", mode="before", check_fields=False)
-    def validate_date(cls, v: str):  # pylint: disable=E0213
-        """Validate the published date."""
-        v = v.replace("\n", "")
-        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.%fZ")  # type: ignore
+
+class FMPAnalystEstimatesData(AnalystEstimatesData):
+    """FMP Analyst Estimates Data."""
 
 
-class FMPPriceTargetFetcher(
+class FMPAnalystEstimatesFetcher(
     Fetcher[
-        FMPPriceTargetQueryParams,
-        List[FMPPriceTargetData],
+        FMPAnalystEstimatesQueryParams,
+        List[FMPAnalystEstimatesData],
     ]
 ):
     """Transform the query, extract and transform the data from the FMP endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> FMPPriceTargetQueryParams:
+    def transform_query(params: Dict[str, Any]) -> FMPAnalystEstimatesQueryParams:
         """Transform the query params."""
-        return FMPPriceTargetQueryParams(**params)
+        return FMPAnalystEstimatesQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: FMPPriceTargetQueryParams,
+        query: FMPAnalystEstimatesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
-        endpoint = "upgrades-downgrades" if query.with_grade else "price-target"
 
-        urls = []
-        for symbol in query.symbol.split(","):
-            query.symbol = symbol
-            urls.append(create_url(4, endpoint, api_key, query, exclude=["limit"]))
+        symbols = query.symbol.split(",")  # type: ignore
+
+        results = []
+
+        async def get_one(symbol):
+            """Get data for one symbol."""
+            url = create_url(
+                3, f"analyst-estimates/{symbol}", api_key, query, ["symbol"]
+            )
+            result = await amake_request(
+                url, response_callback=response_callback, **kwargs
+            )
+            if not result or len(result) == 0:
+                warn(f"Symbol Error: No data found for {symbol}")
+            if result:
+                results.extend(result)
+
+        await asyncio.gather(*[get_one(symbol) for symbol in symbols])
+
+        if not results:
+            raise EmptyDataError("No data returned for the given symbols.")
 
-        return await get_data_urls(urls)
+        return sorted(results, key=lambda x: (x["date"], x["symbol"]), reverse=False)
 
     @staticmethod
     def transform_data(
-        query: FMPPriceTargetQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[FMPPriceTargetData]:
+        query: FMPAnalystEstimatesQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[FMPAnalystEstimatesData]:
         """Return the transformed data."""
-        results: List[FMPPriceTargetData] = []
-        for item in data:
-            new_item = {
-                k if k != "analystCompany" else "analyst_firm": v
-                for k, v in item.items()
-            }
-            results.append(FMPPriceTargetData.model_validate(new_item))
-        return results
+        return [FMPAnalystEstimatesData.model_validate(d) for d in data]
```

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/revenue_business_line.py` & `openbb_fmp-1.1.4/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/revenue_geographic.py` & `openbb_fmp-1.1.4/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/risk_premium.py` & `openbb_fmp-1.1.4/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/share_statistics.py` & `openbb_fmp-1.1.4/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/treasury_rates.py` & `openbb_fmp-1.1.4/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/models/world_news.py` & `openbb_fmp-1.1.4/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/utils/definitions.py` & `openbb_fmp-1.1.4/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.3/openbb_fmp/utils/helpers.py` & `openbb_fmp-1.1.4/openbb_fmp/utils/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,36 @@
 """FMP Helpers Module."""
 
-import json
 from datetime import date as dateType
-from io import StringIO
-from typing import Any, Dict, List, Optional, TypeVar, Union
+from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.utils.client import ClientSession
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     amake_request,
     amake_requests,
     get_querystring,
 )
 from pydantic import BaseModel
 
-T = TypeVar("T", bound=BaseModel)
-
-
-class BasicResponse:
-    """Basic Response class."""
-
-    def __init__(self, response: StringIO):
-        """Initialize the BasicResponse class."""
-        # Find a way to get the status code
-        self.status_code = 200
-        response.seek(0)
-        self.text = response.read()
-
-    def json(self) -> dict:
-        """Return the response as a dictionary."""
-        return json.loads(self.text)
-
-
-def request(url: str) -> BasicResponse:
-    """Request function for PyScript.
-
-    Pass in Method and make sure to await!
-
-    Parameters
-    ----------
-    url: str
-        URL to make request to
-
-    Return
-    ------
-    response: BasicRequest
-        BasicRequest object with status_code and text attributes
-    """
-    # pylint: disable=import-outside-toplevel
-    from pyodide.http import open_url  # type: ignore
-
-    response = open_url(url)
-    return BasicResponse(response)
-
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
-) -> Union[dict, List[dict]]:
+) -> Union[Dict, List[Dict]]:
     """Callback for make_request."""
 
     data = await response.json()
-    if response.status != 200:
-        message = data.get("message", None) or data.get("error", "unknown error")
-        raise RuntimeError(f"Error in FMP request -> {message}")
-
-    if "Error Message" in data:
+    if isinstance(data, dict) and "Error Message" in data:
         raise RuntimeError(f"FMP Error Message -> {data['Error Message']}")
 
-    if len(data) == 0:
-        raise EmptyDataError()
+    if isinstance(data, dict) and "error" in data:
+        raise RuntimeError(
+            f"FMP Error Message -> {data['error']}. Status code: {response.status}"
+        )
 
     return data
 
 
 async def get_data(url: str, **kwargs: Any) -> Union[list, dict]:
     """Get data from FMP endpoint."""
     return await amake_request(url, response_callback=response_callback, **kwargs)
```

### Comparing `openbb_fmp-1.1.3/PKG-INFO` & `openbb_fmp-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-fmp
-Version: 1.1.3
+Version: 1.1.4
 Summary: FMP extension for OpenBB
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
 
 # OpenBB Financial Modeling Prep Provider
 
 This extension integrates the [Financial Modeling Prep](https://site.financialmodelingprep.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

