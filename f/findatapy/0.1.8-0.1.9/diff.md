# Comparing `tmp/findatapy-0.1.8.tar.gz` & `tmp/findatapy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\findatapy-0.1.8.tar", last modified: Sat Apr  4 17:58:49 2020, max compression
+gzip compressed data, was "dist\findatapy-0.1.9.tar", last modified: Sat Apr  4 18:48:28 2020, max compression
```

## Comparing `findatapy-0.1.8.tar` & `findatapy-0.1.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/doc/
--rw-rw-rw-   0        0        0        0 2017-01-18 12:14:54.000000 findatapy-0.1.8/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy/
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy/conf/
--rw-rw-rw-   0        0        0    73333 2015-08-18 08:45:58.000000 findatapy-0.1.8/findatapy/conf/all_econ_tickers.csv
--rw-rw-rw-   0        0        0     9173 2018-01-09 09:57:40.000000 findatapy-0.1.8/findatapy/conf/base_depos_tickers_list.csv
--rw-rw-rw-   0        0        0    75490 2018-09-25 10:34:58.000000 findatapy-0.1.8/findatapy/conf/configfindatapy.xlsm
--rw-rw-rw-   0        0        0     4069 2015-08-18 08:45:58.000000 findatapy-0.1.8/findatapy/conf/econ_country_codes.csv
--rw-rw-rw-   0        0        0    89331 2016-08-17 12:11:58.000000 findatapy-0.1.8/findatapy/conf/econ_tickers.xlsm
--rw-rw-rw-   0        0        0   159834 2016-09-27 17:05:46.000000 findatapy-0.1.8/findatapy/conf/fx_forwards_tickers.csv
--rw-rw-rw-   0        0        0      741 2018-01-09 09:57:36.000000 findatapy-0.1.8/findatapy/conf/fx_forwards_tickers_maker.csv
--rw-rw-rw-   0        0        0   746964 2016-08-15 10:15:36.000000 findatapy-0.1.8/findatapy/conf/fx_vol_tickers.csv
--rw-rw-rw-   0        0        0      634 2018-01-09 09:57:38.000000 findatapy-0.1.8/findatapy/conf/fx_vol_tickers_maker.csv
--rw-rw-rw-   0        0        0      728 2016-10-17 17:15:36.000000 findatapy-0.1.8/findatapy/conf/logging.conf
--rw-rw-rw-   0        0        0     2529 2019-08-14 10:22:48.000000 findatapy-0.1.8/findatapy/conf/time_series_categories_fields.csv
--rw-rw-rw-   0        0        0     2875 2018-09-25 10:35:40.000000 findatapy-0.1.8/findatapy/conf/time_series_fields_list.csv
--rw-rw-rw-   0        0        0    55194 2019-08-14 10:25:24.000000 findatapy-0.1.8/findatapy/conf/time_series_tickers_list.csv
--rw-rw-rw-   0        0        0       26 2015-01-26 13:09:36.000000 findatapy-0.1.8/findatapy/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy/market/
--rw-rw-rw-   0        0        0     1065 2017-02-21 16:52:26.000000 findatapy-0.1.8/findatapy/market/bbgloop_numba.py
--rw-rw-rw-   0        0        0     8636 2019-08-14 09:37:31.000000 findatapy-0.1.8/findatapy/market/datavendor.py
--rw-rw-rw-   0        0        0    43523 2019-08-14 10:19:09.000000 findatapy-0.1.8/findatapy/market/datavendorbbg.py
--rw-rw-rw-   0        0        0    99833 2020-04-04 17:29:29.000000 findatapy-0.1.8/findatapy/market/datavendorweb.py
--rw-rw-rw-   0        0        0     3026 2017-02-05 00:21:54.000000 findatapy-0.1.8/findatapy/market/fxclsvolume.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy/market/indices/
--rw-rw-rw-   0        0        0     4328 2017-11-15 10:44:02.000000 findatapy-0.1.8/findatapy/market/indices/indicesfx.py
--rw-rw-rw-   0        0        0       26 2017-11-15 10:44:02.000000 findatapy-0.1.8/findatapy/market/indices/indicestemplate.py
--rw-rw-rw-   0        0        0       26 2017-11-15 10:44:02.000000 findatapy-0.1.8/findatapy/market/indices/__init__.py
--rw-rw-rw-   0        0        0    33496 2020-02-20 10:55:10.000000 findatapy-0.1.8/findatapy/market/ioengine.py
--rw-rw-rw-   0        0        0    30542 2020-03-06 16:24:35.000000 findatapy-0.1.8/findatapy/market/market.py
--rw-rw-rw-   0        0        0    22833 2020-03-06 16:26:19.000000 findatapy-0.1.8/findatapy/market/marketdatagenerator.py
--rw-rw-rw-   0        0        0    19523 2019-11-02 16:16:43.000000 findatapy-0.1.8/findatapy/market/marketdatarequest.py
--rw-rw-rw-   0        0        0      358 2017-02-21 08:42:40.000000 findatapy-0.1.8/findatapy/market/setup.py
--rw-rw-rw-   0        0        0      491 2017-02-27 22:44:32.000000 findatapy-0.1.8/findatapy/market/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy/timeseries/
--rw-rw-rw-   0        0        0    51907 2019-08-12 17:27:28.000000 findatapy-0.1.8/findatapy/timeseries/calculations.py
--rw-rw-rw-   0        0        0     7025 2017-05-25 10:27:08.000000 findatapy-0.1.8/findatapy/timeseries/dataquality.py
--rw-rw-rw-   0        0        0    31301 2020-03-06 15:09:33.000000 findatapy-0.1.8/findatapy/timeseries/filter.py
--rw-rw-rw-   0        0        0     5826 2017-02-23 11:25:04.000000 findatapy-0.1.8/findatapy/timeseries/retstats.py
--rw-rw-rw-   0        0        0     5166 2017-01-11 10:39:46.000000 findatapy-0.1.8/findatapy/timeseries/timezone.py
--rw-rw-rw-   0        0        0      346 2017-02-12 14:49:20.000000 findatapy-0.1.8/findatapy/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy/util/
--rw-rw-rw-   0        0        0     1490 2016-08-12 15:58:54.000000 findatapy-0.1.8/findatapy/util/cachemanager.py
--rw-rw-rw-   0        0        0      941 2016-08-12 16:02:34.000000 findatapy-0.1.8/findatapy/util/commonman.py
--rw-rw-rw-   0        0        0    14210 2018-02-26 16:33:56.000000 findatapy-0.1.8/findatapy/util/configmanager.py
--rw-rw-rw-   0        0        0     6735 2020-04-04 17:53:09.000000 findatapy-0.1.8/findatapy/util/dataconstants.py
--rw-rw-rw-   0        0        0     3673 2018-10-11 14:32:10.000000 findatapy-0.1.8/findatapy/util/fxconv.py
--rw-rw-rw-   0        0        0     1821 2017-01-11 10:40:24.000000 findatapy-0.1.8/findatapy/util/loggermanager.py
--rw-rw-rw-   0        0        0      501 2019-11-03 14:23:00.000000 findatapy-0.1.8/findatapy/util/set_api_keys.py
--rw-rw-rw-   0        0        0      875 2016-08-17 10:51:42.000000 findatapy-0.1.8/findatapy/util/singleton.py
--rw-rw-rw-   0        0        0     3650 2018-04-23 09:38:14.000000 findatapy-0.1.8/findatapy/util/swimpool.py
--rw-rw-rw-   0        0        0     4331 2018-03-26 11:27:04.000000 findatapy-0.1.8/findatapy/util/tickerfactory.py
--rw-rw-rw-   0        0        0     1889 2017-01-11 10:40:36.000000 findatapy-0.1.8/findatapy/util/twitter.py
--rw-rw-rw-   0        0        0      532 2017-02-12 23:05:46.000000 findatapy-0.1.8/findatapy/util/__init__.py
--rw-rw-rw-   0        0        0       76 2017-02-08 00:00:54.000000 findatapy-0.1.8/findatapy/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy.egg-info/
--rw-rw-rw-   0        0        0        1 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-10-23 09:12:28.000000 findatapy-0.1.8/findatapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      660 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2598 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       39 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy_examples/
--rw-rw-rw-   0        0        0     4040 2017-03-13 17:15:22.000000 findatapy-0.1.8/findatapy_examples/alfred_example.py
--rw-rw-rw-   0        0        0     2076 2017-03-13 17:15:22.000000 findatapy-0.1.8/findatapy_examples/arctic_example.py
--rw-rw-rw-   0        0        0     2672 2018-04-21 16:06:46.000000 findatapy-0.1.8/findatapy_examples/cache_example.py
--rw-rw-rw-   0        0        0     1669 2018-01-09 12:38:52.000000 findatapy-0.1.8/findatapy_examples/cryptocurrencies_example.py
--rw-rw-rw-   0        0        0     5944 2019-08-14 10:33:25.000000 findatapy-0.1.8/findatapy_examples/cryptodata_example.py
--rw-rw-rw-   0        0        0     1913 2017-03-13 17:15:32.000000 findatapy-0.1.8/findatapy_examples/dataquality_example.py
--rw-rw-rw-   0        0        0     2815 2019-08-14 10:15:22.000000 findatapy-0.1.8/findatapy_examples/equitiesdata_example.py
--rw-rw-rw-   0        0        0     3477 2017-03-13 17:15:42.000000 findatapy-0.1.8/findatapy_examples/eventsdata_example.py
--rw-rw-rw-   0        0        0     2563 2018-04-21 14:10:18.000000 findatapy-0.1.8/findatapy_examples/flatfile_example.py
--rw-rw-rw-   0        0        0     1562 2017-03-13 17:15:42.000000 findatapy-0.1.8/findatapy_examples/freddata_example.py
--rw-rw-rw-   0        0        0     8638 2019-08-14 10:34:22.000000 findatapy-0.1.8/findatapy_examples/fxspotdata_example.py
--rw-rw-rw-   0        0        0     3444 2017-03-13 17:15:48.000000 findatapy-0.1.8/findatapy_examples/fxvoldata_example.py
--rw-rw-rw-   0        0        0    10195 2018-04-21 16:15:34.000000 findatapy-0.1.8/findatapy_examples/multiprocessing_example.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/findatapy_examples/notebooks/
--rw-rw-rw-   0        0        0        0 2016-08-17 10:49:54.000000 findatapy-0.1.8/findatapy_examples/notebooks/__init__.py
--rw-rw-rw-   0        0        0     2109 2019-11-02 18:48:23.000000 findatapy-0.1.8/findatapy_examples/test_fetchmd_crypto.py
--rw-rw-rw-   0        0        0        0 2016-08-11 14:20:52.000000 findatapy-0.1.8/findatapy_examples/__init__.py
--rw-rw-rw-   0        0        0      101 2019-11-02 12:43:16.000000 findatapy-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      660 2020-04-04 17:58:49.000000 findatapy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    12908 2020-04-04 17:51:29.000000 findatapy-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2020-04-04 17:58:49.000000 findatapy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1590 2020-04-04 17:51:33.000000 findatapy-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-04-04 17:58:49.000000 findatapy-0.1.8/tests/
--rw-rw-rw-   0        0        0     1092 2017-02-12 18:55:06.000000 findatapy-0.1.8/tests/generate_market_data_for_tests.py
--rw-rw-rw-   0        0        0      692 2019-11-02 16:19:38.000000 findatapy-0.1.8/tests/test_filtering.py
--rw-rw-rw-   0        0        0     1190 2020-02-20 09:53:40.000000 findatapy-0.1.8/tests/test_io.py
--rw-rw-rw-   0        0        0     1909 2019-11-03 14:26:35.000000 findatapy-0.1.8/tests/test_market_download.py
--rw-rw-rw-   0        0        0        0 2017-02-12 18:40:32.000000 findatapy-0.1.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/
+-rw-rw-rw-   0        0        0      101 2019-11-02 12:43:16.000000 findatapy-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      660 2020-04-04 18:48:28.000000 findatapy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12908 2020-04-04 17:51:29.000000 findatapy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/doc/
+-rw-rw-rw-   0        0        0        0 2017-01-18 12:14:54.000000 findatapy-0.1.9/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy/
+-rw-rw-rw-   0        0        0       76 2017-02-08 00:00:54.000000 findatapy-0.1.9/findatapy/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy/conf/
+-rw-rw-rw-   0        0        0       26 2015-01-26 13:09:36.000000 findatapy-0.1.9/findatapy/conf/__init__.py
+-rw-rw-rw-   0        0        0    73333 2015-08-18 08:45:58.000000 findatapy-0.1.9/findatapy/conf/all_econ_tickers.csv
+-rw-rw-rw-   0        0        0     9173 2018-01-09 09:57:40.000000 findatapy-0.1.9/findatapy/conf/base_depos_tickers_list.csv
+-rw-rw-rw-   0        0        0    75490 2018-09-25 10:34:58.000000 findatapy-0.1.9/findatapy/conf/configfindatapy.xlsm
+-rw-rw-rw-   0        0        0     4069 2015-08-18 08:45:58.000000 findatapy-0.1.9/findatapy/conf/econ_country_codes.csv
+-rw-rw-rw-   0        0        0    89331 2016-08-17 12:11:58.000000 findatapy-0.1.9/findatapy/conf/econ_tickers.xlsm
+-rw-rw-rw-   0        0        0   159834 2016-09-27 17:05:46.000000 findatapy-0.1.9/findatapy/conf/fx_forwards_tickers.csv
+-rw-rw-rw-   0        0        0      741 2018-01-09 09:57:36.000000 findatapy-0.1.9/findatapy/conf/fx_forwards_tickers_maker.csv
+-rw-rw-rw-   0        0        0   746964 2016-08-15 10:15:36.000000 findatapy-0.1.9/findatapy/conf/fx_vol_tickers.csv
+-rw-rw-rw-   0        0        0      634 2018-01-09 09:57:38.000000 findatapy-0.1.9/findatapy/conf/fx_vol_tickers_maker.csv
+-rw-rw-rw-   0        0        0      728 2016-10-17 17:15:36.000000 findatapy-0.1.9/findatapy/conf/logging.conf
+-rw-rw-rw-   0        0        0     2529 2019-08-14 10:22:48.000000 findatapy-0.1.9/findatapy/conf/time_series_categories_fields.csv
+-rw-rw-rw-   0        0        0     2875 2018-09-25 10:35:40.000000 findatapy-0.1.9/findatapy/conf/time_series_fields_list.csv
+-rw-rw-rw-   0        0        0    55194 2019-08-14 10:25:24.000000 findatapy-0.1.9/findatapy/conf/time_series_tickers_list.csv
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy/market/
+-rw-rw-rw-   0        0        0      491 2017-02-27 22:44:32.000000 findatapy-0.1.9/findatapy/market/__init__.py
+-rw-rw-rw-   0        0        0     1065 2017-02-21 16:52:26.000000 findatapy-0.1.9/findatapy/market/bbgloop_numba.py
+-rw-rw-rw-   0        0        0     8636 2019-08-14 09:37:31.000000 findatapy-0.1.9/findatapy/market/datavendor.py
+-rw-rw-rw-   0        0        0    43523 2019-08-14 10:19:09.000000 findatapy-0.1.9/findatapy/market/datavendorbbg.py
+-rw-rw-rw-   0        0        0   100003 2020-04-04 18:45:44.000000 findatapy-0.1.9/findatapy/market/datavendorweb.py
+-rw-rw-rw-   0        0        0     3026 2017-02-05 00:21:54.000000 findatapy-0.1.9/findatapy/market/fxclsvolume.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy/market/indices/
+-rw-rw-rw-   0        0        0       26 2017-11-15 10:44:02.000000 findatapy-0.1.9/findatapy/market/indices/__init__.py
+-rw-rw-rw-   0        0        0     4328 2017-11-15 10:44:02.000000 findatapy-0.1.9/findatapy/market/indices/indicesfx.py
+-rw-rw-rw-   0        0        0       26 2017-11-15 10:44:02.000000 findatapy-0.1.9/findatapy/market/indices/indicestemplate.py
+-rw-rw-rw-   0        0        0    33496 2020-02-20 10:55:10.000000 findatapy-0.1.9/findatapy/market/ioengine.py
+-rw-rw-rw-   0        0        0    30542 2020-03-06 16:24:35.000000 findatapy-0.1.9/findatapy/market/market.py
+-rw-rw-rw-   0        0        0    22833 2020-03-06 16:26:19.000000 findatapy-0.1.9/findatapy/market/marketdatagenerator.py
+-rw-rw-rw-   0        0        0    19523 2019-11-02 16:16:43.000000 findatapy-0.1.9/findatapy/market/marketdatarequest.py
+-rw-rw-rw-   0        0        0      358 2017-02-21 08:42:40.000000 findatapy-0.1.9/findatapy/market/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy/timeseries/
+-rw-rw-rw-   0        0        0      346 2017-02-12 14:49:20.000000 findatapy-0.1.9/findatapy/timeseries/__init__.py
+-rw-rw-rw-   0        0        0    51907 2019-08-12 17:27:28.000000 findatapy-0.1.9/findatapy/timeseries/calculations.py
+-rw-rw-rw-   0        0        0     7025 2017-05-25 10:27:08.000000 findatapy-0.1.9/findatapy/timeseries/dataquality.py
+-rw-rw-rw-   0        0        0    31301 2020-03-06 15:09:33.000000 findatapy-0.1.9/findatapy/timeseries/filter.py
+-rw-rw-rw-   0        0        0     5826 2017-02-23 11:25:04.000000 findatapy-0.1.9/findatapy/timeseries/retstats.py
+-rw-rw-rw-   0        0        0     5166 2017-01-11 10:39:46.000000 findatapy-0.1.9/findatapy/timeseries/timezone.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy/util/
+-rw-rw-rw-   0        0        0      532 2017-02-12 23:05:46.000000 findatapy-0.1.9/findatapy/util/__init__.py
+-rw-rw-rw-   0        0        0     1490 2016-08-12 15:58:54.000000 findatapy-0.1.9/findatapy/util/cachemanager.py
+-rw-rw-rw-   0        0        0      941 2016-08-12 16:02:34.000000 findatapy-0.1.9/findatapy/util/commonman.py
+-rw-rw-rw-   0        0        0    14210 2018-02-26 16:33:56.000000 findatapy-0.1.9/findatapy/util/configmanager.py
+-rw-rw-rw-   0        0        0     6735 2020-04-04 17:53:09.000000 findatapy-0.1.9/findatapy/util/dataconstants.py
+-rw-rw-rw-   0        0        0     3673 2018-10-11 14:32:10.000000 findatapy-0.1.9/findatapy/util/fxconv.py
+-rw-rw-rw-   0        0        0     1821 2017-01-11 10:40:24.000000 findatapy-0.1.9/findatapy/util/loggermanager.py
+-rw-rw-rw-   0        0        0      501 2019-11-03 14:23:00.000000 findatapy-0.1.9/findatapy/util/set_api_keys.py
+-rw-rw-rw-   0        0        0      875 2016-08-17 10:51:42.000000 findatapy-0.1.9/findatapy/util/singleton.py
+-rw-rw-rw-   0        0        0     3650 2018-04-23 09:38:14.000000 findatapy-0.1.9/findatapy/util/swimpool.py
+-rw-rw-rw-   0        0        0     4331 2018-03-26 11:27:04.000000 findatapy-0.1.9/findatapy/util/tickerfactory.py
+-rw-rw-rw-   0        0        0     1889 2017-01-11 10:40:36.000000 findatapy-0.1.9/findatapy/util/twitter.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy.egg-info/
+-rw-rw-rw-   0        0        0      660 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-10-23 09:12:28.000000 findatapy-0.1.9/findatapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      183 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy_examples/
+-rw-rw-rw-   0        0        0        0 2016-08-11 14:20:52.000000 findatapy-0.1.9/findatapy_examples/__init__.py
+-rw-rw-rw-   0        0        0     4040 2017-03-13 17:15:22.000000 findatapy-0.1.9/findatapy_examples/alfred_example.py
+-rw-rw-rw-   0        0        0     2076 2017-03-13 17:15:22.000000 findatapy-0.1.9/findatapy_examples/arctic_example.py
+-rw-rw-rw-   0        0        0     2672 2018-04-21 16:06:46.000000 findatapy-0.1.9/findatapy_examples/cache_example.py
+-rw-rw-rw-   0        0        0     1669 2018-01-09 12:38:52.000000 findatapy-0.1.9/findatapy_examples/cryptocurrencies_example.py
+-rw-rw-rw-   0        0        0     5944 2019-08-14 10:33:25.000000 findatapy-0.1.9/findatapy_examples/cryptodata_example.py
+-rw-rw-rw-   0        0        0     1913 2017-03-13 17:15:32.000000 findatapy-0.1.9/findatapy_examples/dataquality_example.py
+-rw-rw-rw-   0        0        0     2815 2019-08-14 10:15:22.000000 findatapy-0.1.9/findatapy_examples/equitiesdata_example.py
+-rw-rw-rw-   0        0        0     3477 2017-03-13 17:15:42.000000 findatapy-0.1.9/findatapy_examples/eventsdata_example.py
+-rw-rw-rw-   0        0        0     2563 2018-04-21 14:10:18.000000 findatapy-0.1.9/findatapy_examples/flatfile_example.py
+-rw-rw-rw-   0        0        0     1562 2017-03-13 17:15:42.000000 findatapy-0.1.9/findatapy_examples/freddata_example.py
+-rw-rw-rw-   0        0        0     8638 2019-08-14 10:34:22.000000 findatapy-0.1.9/findatapy_examples/fxspotdata_example.py
+-rw-rw-rw-   0        0        0     3444 2017-03-13 17:15:48.000000 findatapy-0.1.9/findatapy_examples/fxvoldata_example.py
+-rw-rw-rw-   0        0        0    10195 2018-04-21 16:15:34.000000 findatapy-0.1.9/findatapy_examples/multiprocessing_example.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/findatapy_examples/notebooks/
+-rw-rw-rw-   0        0        0        0 2016-08-17 10:49:54.000000 findatapy-0.1.9/findatapy_examples/notebooks/__init__.py
+-rw-rw-rw-   0        0        0     2109 2019-11-02 18:48:23.000000 findatapy-0.1.9/findatapy_examples/test_fetchmd_crypto.py
+-rw-rw-rw-   0        0        0       42 2020-04-04 18:48:28.000000 findatapy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2020-04-04 18:48:18.000000 findatapy-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-04 18:48:28.000000 findatapy-0.1.9/tests/
+-rw-rw-rw-   0        0        0        0 2017-02-12 18:40:32.000000 findatapy-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1092 2017-02-12 18:55:06.000000 findatapy-0.1.9/tests/generate_market_data_for_tests.py
+-rw-rw-rw-   0        0        0      692 2019-11-02 16:19:38.000000 findatapy-0.1.9/tests/test_filtering.py
+-rw-rw-rw-   0        0        0     1190 2020-02-20 09:53:40.000000 findatapy-0.1.9/tests/test_io.py
+-rw-rw-rw-   0        0        0     1909 2019-11-03 14:26:35.000000 findatapy-0.1.9/tests/test_market_download.py
```

### Comparing `findatapy-0.1.8/findatapy/conf/all_econ_tickers.csv` & `findatapy-0.1.9/findatapy/conf/all_econ_tickers.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/base_depos_tickers_list.csv` & `findatapy-0.1.9/findatapy/conf/base_depos_tickers_list.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/configfindatapy.xlsm` & `findatapy-0.1.9/findatapy/conf/configfindatapy.xlsm`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/econ_country_codes.csv` & `findatapy-0.1.9/findatapy/conf/econ_country_codes.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/econ_tickers.xlsm` & `findatapy-0.1.9/findatapy/conf/econ_tickers.xlsm`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/fx_forwards_tickers.csv` & `findatapy-0.1.9/findatapy/conf/fx_forwards_tickers.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/fx_forwards_tickers_maker.csv` & `findatapy-0.1.9/findatapy/conf/fx_forwards_tickers_maker.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/fx_vol_tickers.csv` & `findatapy-0.1.9/findatapy/conf/fx_vol_tickers.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/fx_vol_tickers_maker.csv` & `findatapy-0.1.9/findatapy/conf/fx_vol_tickers_maker.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/logging.conf` & `findatapy-0.1.9/findatapy/conf/logging.conf`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/time_series_categories_fields.csv` & `findatapy-0.1.9/findatapy/conf/time_series_categories_fields.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/time_series_fields_list.csv` & `findatapy-0.1.9/findatapy/conf/time_series_fields_list.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/conf/time_series_tickers_list.csv` & `findatapy-0.1.9/findatapy/conf/time_series_tickers_list.csv`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/bbgloop_numba.py` & `findatapy-0.1.9/findatapy/market/bbgloop_numba.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/datavendor.py` & `findatapy-0.1.9/findatapy/market/datavendor.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/datavendorbbg.py` & `findatapy-0.1.9/findatapy/market/datavendorbbg.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/datavendorweb.py` & `findatapy-0.1.9/findatapy/market/datavendorweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1339,27 +1339,31 @@
         multi_threaded = constants.dukascopy_multithreading # multithreading (can sometimes get errors but it's fine when retried, avoid using)
 
         if multi_threaded:
 
             completed = False
 
             for i in range(0, 5):
-                # Use threading (not multiprocess interface, which has issues with dukascopy download)
-                pool = SwimPool().create_pool('thread', constants.market_thread_no['dukascopy'])
-                results = [pool.apply_async(self.fetch_file, args=(time, symbol, do_retrieve_df,)) for time in time_list]
 
-                logger.debug("Attempting Dukascopy download " + str(i) + "... ")
-                tick_list = [p.get(timeout=constants.timeout_downloader['dukascopy']) for p in results]
-
-                pool.close()
-                pool.join()
-
-                completed = True
-
-                break
+                try:
+                    # Use threading (not multiprocess interface, which has issues with dukascopy download)
+                    pool = SwimPool().create_pool('thread', constants.market_thread_no['dukascopy'])
+                    results = [pool.apply_async(self.fetch_file, args=(time, symbol, do_retrieve_df,)) for time in time_list]
+
+                    logger.debug("Attempting Dukascopy download " + str(i) + "... ")
+                    tick_list = [p.get(timeout=constants.timeout_downloader['dukascopy']) for p in results]
+
+                    pool.close()
+                    pool.join()
+
+                    completed = True
+
+                    break
+                except:
+                    logger.warning("Didn't download on " + str(i) + " attempt... ")
 
             if not(completed):
                 logger.warning("Failed to download from Dukascopy after several attempts")
 
         else:
             # fully single threaded
             tick_list = []
```

### Comparing `findatapy-0.1.8/findatapy/market/fxclsvolume.py` & `findatapy-0.1.9/findatapy/market/fxclsvolume.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/indices/indicesfx.py` & `findatapy-0.1.9/findatapy/market/indices/indicesfx.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/ioengine.py` & `findatapy-0.1.9/findatapy/market/ioengine.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/market.py` & `findatapy-0.1.9/findatapy/market/market.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/marketdatagenerator.py` & `findatapy-0.1.9/findatapy/market/marketdatagenerator.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/market/marketdatarequest.py` & `findatapy-0.1.9/findatapy/market/marketdatarequest.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/timeseries/calculations.py` & `findatapy-0.1.9/findatapy/timeseries/calculations.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/timeseries/dataquality.py` & `findatapy-0.1.9/findatapy/timeseries/dataquality.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/timeseries/filter.py` & `findatapy-0.1.9/findatapy/timeseries/filter.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/timeseries/retstats.py` & `findatapy-0.1.9/findatapy/timeseries/retstats.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/timeseries/timezone.py` & `findatapy-0.1.9/findatapy/timeseries/timezone.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/cachemanager.py` & `findatapy-0.1.9/findatapy/util/cachemanager.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/commonman.py` & `findatapy-0.1.9/findatapy/util/commonman.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/configmanager.py` & `findatapy-0.1.9/findatapy/util/configmanager.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/dataconstants.py` & `findatapy-0.1.9/findatapy/util/dataconstants.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/fxconv.py` & `findatapy-0.1.9/findatapy/util/fxconv.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/loggermanager.py` & `findatapy-0.1.9/findatapy/util/loggermanager.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/singleton.py` & `findatapy-0.1.9/findatapy/util/singleton.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/swimpool.py` & `findatapy-0.1.9/findatapy/util/swimpool.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/tickerfactory.py` & `findatapy-0.1.9/findatapy/util/tickerfactory.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/twitter.py` & `findatapy-0.1.9/findatapy/util/twitter.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy/util/__init__.py` & `findatapy-0.1.9/findatapy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy.egg-info/PKG-INFO` & `findatapy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: findatapy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Market data library
 Home-page: https://github.com/cuemacro/findatapy
 Author: Saeed Amen
 Author-email: saeed@cuemacro.com
 License: Apache 2.0
 Description: findatapy creates an easy to use Python API to download market data from many sources including 
         Quandl, Bloomberg, Yahoo, Google etc. using a unified high level interface. Users can also define their own custom
```

### Comparing `findatapy-0.1.8/findatapy.egg-info/SOURCES.txt` & `findatapy-0.1.9/findatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/alfred_example.py` & `findatapy-0.1.9/findatapy_examples/alfred_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/arctic_example.py` & `findatapy-0.1.9/findatapy_examples/arctic_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/cache_example.py` & `findatapy-0.1.9/findatapy_examples/cache_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/cryptocurrencies_example.py` & `findatapy-0.1.9/findatapy_examples/cryptocurrencies_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/cryptodata_example.py` & `findatapy-0.1.9/findatapy_examples/cryptodata_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/dataquality_example.py` & `findatapy-0.1.9/findatapy_examples/dataquality_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/equitiesdata_example.py` & `findatapy-0.1.9/findatapy_examples/equitiesdata_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/eventsdata_example.py` & `findatapy-0.1.9/findatapy_examples/eventsdata_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/flatfile_example.py` & `findatapy-0.1.9/findatapy_examples/flatfile_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/freddata_example.py` & `findatapy-0.1.9/findatapy_examples/freddata_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/fxspotdata_example.py` & `findatapy-0.1.9/findatapy_examples/fxspotdata_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/fxvoldata_example.py` & `findatapy-0.1.9/findatapy_examples/fxvoldata_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/multiprocessing_example.py` & `findatapy-0.1.9/findatapy_examples/multiprocessing_example.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/findatapy_examples/test_fetchmd_crypto.py` & `findatapy-0.1.9/findatapy_examples/test_fetchmd_crypto.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/PKG-INFO` & `findatapy-0.1.9/findatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: findatapy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Market data library
 Home-page: https://github.com/cuemacro/findatapy
 Author: Saeed Amen
 Author-email: saeed@cuemacro.com
 License: Apache 2.0
 Description: findatapy creates an easy to use Python API to download market data from many sources including 
         Quandl, Bloomberg, Yahoo, Google etc. using a unified high level interface. Users can also define their own custom
```

### Comparing `findatapy-0.1.8/README.md` & `findatapy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/setup.py` & `findatapy-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 long_description = """findatapy creates an easy to use Python API to download market data from many sources including 
 Quandl, Bloomberg, Yahoo, Google etc. using a unified high level interface. Users can also define their own custom 
 tickers, using configuration files. There is also functionality which is particularly useful for those downloading FX market data."""
 
 setup(name='findatapy',
-      version='0.1.8',
+      version='0.1.9',
       description='Market data library',
       author='Saeed Amen',
       author_email='saeed@cuemacro.com',
       license='Apache 2.0',
       long_description=long_description,
       keywords=['pandas', 'data', 'Bloomberg', 'tick', 'stocks', 'equities'],
       url='https://github.com/cuemacro/findatapy',
```

### Comparing `findatapy-0.1.8/tests/generate_market_data_for_tests.py` & `findatapy-0.1.9/tests/generate_market_data_for_tests.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/tests/test_filtering.py` & `findatapy-0.1.9/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/tests/test_io.py` & `findatapy-0.1.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `findatapy-0.1.8/tests/test_market_download.py` & `findatapy-0.1.9/tests/test_market_download.py`

 * *Files identical despite different names*

