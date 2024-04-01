# Comparing `tmp/finazon_grpc_python-1.0.136.2.tar.gz` & `tmp/finazon_grpc_python-1.0.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finazon_grpc_python-1.0.136.2.tar", max compression
+gzip compressed data, was "finazon_grpc_python-1.0.141.tar", max compression
```

## Comparing `finazon_grpc_python-1.0.136.2.tar` & `finazon_grpc_python-1.0.141.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1064 2024-02-13 20:32:42.949886 finazon_grpc_python-1.0.136.2/LICENSE.txt
--rw-r--r--   0        0        0    10159 2024-03-04 14:48:33.533986 finazon_grpc_python-1.0.136.2/README.md
--rw-r--r--   0        0        0        0 2024-02-28 07:42:52.990282 finazon_grpc_python-1.0.136.2/finazon_grpc_python/__init__.py
--rw-r--r--   0        0        0     1997 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_pb2.py
--rw-r--r--   0        0        0     2977 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_pb2.pyi
--rw-r--r--   0        0        0     2715 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_pb2_grpc.py
--rw-r--r--   0        0        0      504 2024-03-04 14:48:56.423445 finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_service.py
--rw-r--r--   0        0        0     9699 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_pb2.py
--rw-r--r--   0        0        0    27137 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_pb2.pyi
--rw-r--r--   0        0        0     7871 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_pb2_grpc.py
--rw-r--r--   0        0        0     1175 2024-03-04 14:48:56.107425 finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_service.py
--rw-r--r--   0        0        0     2456 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_pb2.py
--rw-r--r--   0        0        0     4188 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_pb2.pyi
--rw-r--r--   0        0        0     2769 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_pb2_grpc.py
--rw-r--r--   0        0        0      537 2024-03-04 14:48:56.379442 finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_service.py
--rw-r--r--   0        0        0        0 2024-02-27 14:37:50.723171 finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/__init__.py
--rw-r--r--   0        0        0     1786 2024-02-28 12:02:26.373203 finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/client.py
--rw-r--r--   0        0        0      496 2024-02-28 12:00:04.869646 finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/errors.py
--rw-r--r--   0        0        0      177 2024-03-04 14:48:42.762573 finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/settings.py
--rw-r--r--   0        0        0     1966 2024-03-04 14:05:10.294573 finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/utils.py
--rw-r--r--   0        0        0     2225 2024-03-04 14:48:56.963479 finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_pb2.py
--rw-r--r--   0        0        0     3411 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_pb2.pyi
--rw-r--r--   0        0        0     2737 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_pb2_grpc.py
--rw-r--r--   0        0        0      528 2024-03-04 14:48:56.411444 finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_service.py
--rw-r--r--   0        0        0     1787 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_pb2.py
--rw-r--r--   0        0        0     2208 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_pb2.pyi
--rw-r--r--   0        0        0     2718 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-03-04 14:48:56.435445 finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_service.py
--rw-r--r--   0        0        0        0 2024-02-13 20:32:42.949886 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/__init__.py
--rw-r--r--   0        0        0      627 2024-03-04 14:34:47.300646 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/indicator_atr.py
--rw-r--r--   0        0        0      598 2024-03-04 14:22:48.014704 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/indicator_ma.py
--rw-r--r--   0        0        0      689 2024-03-04 14:25:40.473576 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/indicator_ma_pandas.py
--rw-r--r--   0        0        0      489 2024-02-28 13:49:10.731115 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/tickers.py
--rw-r--r--   0        0        0      635 2024-03-04 14:29:59.652016 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/time_series.py
--rw-r--r--   0        0        0      619 2024-03-04 14:14:13.758535 finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/time_series_pandas.py
--rw-r--r--   0        0        0     2790 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_pb2.py
--rw-r--r--   0        0        0     4502 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_pb2.pyi
--rw-r--r--   0        0        0     4553 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_pb2_grpc.py
--rw-r--r--   0        0        0      771 2024-03-04 14:48:56.195430 finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_service.py
--rw-r--r--   0        0        0     2181 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_pb2.py
--rw-r--r--   0        0        0     3276 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_pb2.pyi
--rw-r--r--   0        0        0     2713 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_pb2_grpc.py
--rw-r--r--   0        0        0      519 2024-03-04 14:48:56.063422 finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_service.py
--rw-r--r--   0        0        0     1805 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_pb2.py
--rw-r--r--   0        0        0     2230 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_pb2.pyi
--rw-r--r--   0        0        0     2778 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_pb2_grpc.py
--rw-r--r--   0        0        0      520 2024-03-04 14:48:56.451447 finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_service.py
--rw-r--r--   0        0        0     2634 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_pb2.py
--rw-r--r--   0        0        0     5228 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_pb2.pyi
--rw-r--r--   0        0        0     2711 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_pb2_grpc.py
--rw-r--r--   0        0        0      486 2024-03-04 14:48:56.395443 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_service.py
--rw-r--r--   0        0        0     3172 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_pb2.py
--rw-r--r--   0        0        0     6003 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_pb2.pyi
--rw-r--r--   0        0        0     4372 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_pb2_grpc.py
--rw-r--r--   0        0        0      716 2024-03-04 14:48:56.127426 finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_service.py
--rw-r--r--   0        0        0     3586 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_pb2.py
--rw-r--r--   0        0        0     7684 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_pb2.pyi
--rw-r--r--   0        0        0     2822 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-03-04 14:48:56.363441 finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_service.py
--rw-r--r--   0        0        0     5378 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_pb2.py
--rw-r--r--   0        0        0    11827 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_pb2.pyi
--rw-r--r--   0        0        0     8214 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_pb2_grpc.py
--rw-r--r--   0        0        0     1223 2024-03-04 14:48:56.171429 finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_service.py
--rw-r--r--   0        0        0    11776 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_pb2.py
--rw-r--r--   0        0        0    28018 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_pb2.pyi
--rw-r--r--   0        0        0    19109 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_pb2_grpc.py
--rw-r--r--   0        0        0     2765 2024-03-04 14:48:56.347440 finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_service.py
--rw-r--r--   0        0        0     2339 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_pb2.py
--rw-r--r--   0        0        0     4170 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_pb2.pyi
--rw-r--r--   0        0        0     2630 2024-03-04 14:48:56.967480 finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_pb2_grpc.py
--rw-r--r--   0        0        0      474 2024-03-04 14:48:56.211431 finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_service.py
--rw-r--r--   0        0        0      815 2024-03-04 14:48:42.758573 finazon_grpc_python-1.0.136.2/pyproject.toml
--rw-r--r--   0        0        0      443 2024-03-04 13:57:04.928973 finazon_grpc_python-1.0.136.2/requirements.txt
--rw-r--r--   0        0        0    11041 1970-01-01 00:00:00.000000 finazon_grpc_python-1.0.136.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-02-13 20:32:42.949886 finazon_grpc_python-1.0.141/LICENSE.txt
+-rw-r--r--   0        0        0    10159 2024-03-04 14:48:33.533986 finazon_grpc_python-1.0.141/README.md
+-rw-r--r--   0        0        0        0 2024-02-28 07:42:52.990282 finazon_grpc_python-1.0.141/finazon_grpc_python/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.py
+-rw-r--r--   0        0        0     2977 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.pyi
+-rw-r--r--   0        0        0     2715 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2_grpc.py
+-rw-r--r--   0        0        0      504 2024-04-01 10:30:58.049306 finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_service.py
+-rw-r--r--   0        0        0     9699 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.py
+-rw-r--r--   0        0        0    27137 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.pyi
+-rw-r--r--   0        0        0     7871 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2_grpc.py
+-rw-r--r--   0        0        0     1175 2024-04-01 10:30:57.909306 finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_service.py
+-rw-r--r--   0        0        0     2456 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.py
+-rw-r--r--   0        0        0     4188 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.pyi
+-rw-r--r--   0        0        0     2769 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2_grpc.py
+-rw-r--r--   0        0        0      537 2024-04-01 10:30:58.029306 finazon_grpc_python-1.0.141/finazon_grpc_python/binance_service.py
+-rw-r--r--   0        0        0        0 2024-02-27 14:37:50.723171 finazon_grpc_python-1.0.141/finazon_grpc_python/common/__init__.py
+-rw-r--r--   0        0        0     1786 2024-02-28 12:02:26.373203 finazon_grpc_python-1.0.141/finazon_grpc_python/common/client.py
+-rw-r--r--   0        0        0      496 2024-02-28 12:00:04.869646 finazon_grpc_python-1.0.141/finazon_grpc_python/common/errors.py
+-rw-r--r--   0        0        0      177 2024-04-01 10:30:50.613342 finazon_grpc_python-1.0.141/finazon_grpc_python/common/settings.py
+-rw-r--r--   0        0        0     1966 2024-03-04 14:05:10.294573 finazon_grpc_python-1.0.141/finazon_grpc_python/common/utils.py
+-rw-r--r--   0        0        0     2225 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.py
+-rw-r--r--   0        0        0     3411 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.pyi
+-rw-r--r--   0        0        0     2737 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2024-04-01 10:30:58.041306 finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_service.py
+-rw-r--r--   0        0        0     1787 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.py
+-rw-r--r--   0        0        0     2208 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.pyi
+-rw-r--r--   0        0        0     2718 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-04-01 10:30:58.053305 finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_service.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:32:42.949886 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/__init__.py
+-rw-r--r--   0        0        0      627 2024-03-04 14:34:47.300646 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_atr.py
+-rw-r--r--   0        0        0      598 2024-03-04 14:22:48.014704 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma.py
+-rw-r--r--   0        0        0      689 2024-03-04 14:25:40.473576 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma_pandas.py
+-rw-r--r--   0        0        0      489 2024-02-28 13:49:10.731115 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/tickers.py
+-rw-r--r--   0        0        0      635 2024-03-04 14:29:59.652016 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series.py
+-rw-r--r--   0        0        0      619 2024-03-04 14:14:13.758535 finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series_pandas.py
+-rw-r--r--   0        0        0     2790 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.py
+-rw-r--r--   0        0        0     4502 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.pyi
+-rw-r--r--   0        0        0     4553 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2_grpc.py
+-rw-r--r--   0        0        0      771 2024-04-01 10:30:57.949306 finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_service.py
+-rw-r--r--   0        0        0     2181 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.py
+-rw-r--r--   0        0        0     3276 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.pyi
+-rw-r--r--   0        0        0     2713 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2_grpc.py
+-rw-r--r--   0        0        0      519 2024-04-01 10:30:57.893306 finazon_grpc_python-1.0.141/finazon_grpc_python/forex_service.py
+-rw-r--r--   0        0        0     1805 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.py
+-rw-r--r--   0        0        0     2230 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.pyi
+-rw-r--r--   0        0        0     2778 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2_grpc.py
+-rw-r--r--   0        0        0      520 2024-04-01 10:30:58.061306 finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_service.py
+-rw-r--r--   0        0        0     2634 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.py
+-rw-r--r--   0        0        0     5228 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.pyi
+-rw-r--r--   0        0        0     2711 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2_grpc.py
+-rw-r--r--   0        0        0      486 2024-04-01 10:30:58.037306 finazon_grpc_python-1.0.141/finazon_grpc_python/sec_service.py
+-rw-r--r--   0        0        0     3172 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.py
+-rw-r--r--   0        0        0     6003 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.pyi
+-rw-r--r--   0        0        0     4372 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2_grpc.py
+-rw-r--r--   0        0        0      716 2024-04-01 10:30:57.921306 finazon_grpc_python-1.0.141/finazon_grpc_python/sip_service.py
+-rw-r--r--   0        0        0     3629 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.py
+-rw-r--r--   0        0        0     7809 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.pyi
+-rw-r--r--   0        0        0     2822 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-04-01 10:30:58.025306 finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_service.py
+-rw-r--r--   0        0        0     5421 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.py
+-rw-r--r--   0        0        0    11952 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.pyi
+-rw-r--r--   0        0        0     8214 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2_grpc.py
+-rw-r--r--   0        0        0     1223 2024-04-01 10:30:57.937306 finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_service.py
+-rw-r--r--   0        0        0    11776 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.py
+-rw-r--r--   0        0        0    28018 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.pyi
+-rw-r--r--   0        0        0    19109 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2_grpc.py
+-rw-r--r--   0        0        0     2765 2024-04-01 10:30:58.017306 finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_service.py
+-rw-r--r--   0        0        0     2382 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.py
+-rw-r--r--   0        0        0     4295 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.pyi
+-rw-r--r--   0        0        0     2630 2024-04-01 10:30:58.197305 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2_grpc.py
+-rw-r--r--   0        0        0      474 2024-04-01 10:30:57.953306 finazon_grpc_python-1.0.141/finazon_grpc_python/trade_service.py
+-rw-r--r--   0        0        0      813 2024-04-01 10:30:50.609342 finazon_grpc_python-1.0.141/pyproject.toml
+-rw-r--r--   0        0        0      443 2024-03-04 13:57:04.928973 finazon_grpc_python-1.0.141/requirements.txt
+-rw-r--r--   0        0        0    11039 1970-01-01 00:00:00.000000 finazon_grpc_python-1.0.141/PKG-INFO
```

### Comparing `finazon_grpc_python-1.0.136.2/LICENSE.txt` & `finazon_grpc_python-1.0.141/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/README.md` & `finazon_grpc_python-1.0.141/README.md`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/api_usage_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/api_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/benzinga_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/benzinga_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/binance_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/binance_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/client.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/common/client.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/common/utils.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/common/utils.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/crypto_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/crypto_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/datasets_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/datasets_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/indicator_atr.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_atr.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/indicator_ma.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/indicator_ma_pandas.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/indicator_ma_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/time_series.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/examples/time_series_pandas.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/examples/time_series_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/exchange_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/exchange_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/forex_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/forex_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/publishers_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/publishers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sec_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/sip_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/sip_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"finazon_grpc_python/snapshot.proto\x12\x07\x66inazon\"\xd5\x01\n\x12GetSnapshotRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0e\n\x06market\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x0b\n\x03\x63qs\x18\x06 \x01(\t\x12\x0b\n\x03\x63ik\x18\x07 \x01(\t\x12\r\n\x05\x63usip\x18\x08 \x01(\t\x12\x0c\n\x04isin\x18\t \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\n \x01(\t\x12\x12\n\nshare_figi\x18\x0b \x01(\t\x12\x0b\n\x03lei\x18\x0c \x01(\t\"W\n\rSnapshotOhlcv\x12\x0c\n\x04open\x18\x01 \x01(\x01\x12\x0c\n\x04high\x18\x02 \x01(\x01\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\r\n\x05\x63lose\x18\x04 \x01(\x01\x12\x0e\n\x06volume\x18\x05 \x01(\x01\"D\n\x11SnapshotLastTrade\x12\x10\n\x08\x65vent_at\x18\x01 \x01(\x03\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x0e\n\x06shares\x18\x03 \x01(\x03\"\x96\x01\n\x18SnapshotLastFiftyTwoWeek\x12\x0c\n\x04high\x18\x01 \x01(\x01\x12\x0f\n\x07high_at\x18\x02 \x01(\x03\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0e\n\x06low_at\x18\x04 \x01(\x03\x12\x0e\n\x06\x63hange\x18\x05 \x01(\x01\x12\x16\n\x0e\x63hange_percent\x18\x06 \x01(\x01\x12\x16\n\x0e\x61verage_volume\x18\x07 \x01(\x03\"g\n\x0eSnapshotChange\x12\x1a\n\x12\x64\x61y_change_percent\x18\x01 \x01(\x01\x12\x1b\n\x13week_change_percent\x18\x02 \x01(\x01\x12\x1c\n\x14month_change_percent\x18\x03 \x01(\x01\"\xb2\x02\n\x13GetSnapshotResponse\x12(\n\x08last_day\x18\x01 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12*\n\nlast_month\x18\x02 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12.\n\nlast_trade\x18\x03 \x01(\x0b\x32\x1a.finazon.SnapshotLastTrade\x12,\n\x0cprevious_day\x18\x04 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12>\n\x13last_fifty_two_week\x18\x05 \x01(\x0b\x32!.finazon.SnapshotLastFiftyTwoWeek\x12\'\n\x06\x63hange\x18\x06 \x01(\x0b\x32\x17.finazon.SnapshotChange2]\n\x0fSnapshotService\x12J\n\x0bGetSnapshot\x12\x1b.finazon.GetSnapshotRequest\x1a\x1c.finazon.GetSnapshotResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"finazon_grpc_python/snapshot.proto\x12\x07\x66inazon\"\xe6\x01\n\x12GetSnapshotRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0e\n\x06market\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x0b\n\x03\x63qs\x18\x06 \x01(\t\x12\x0b\n\x03\x63ik\x18\x07 \x01(\t\x12\r\n\x05\x63usip\x18\x08 \x01(\t\x12\x0c\n\x04isin\x18\t \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\n \x01(\t\x12\x12\n\nshare_figi\x18\x0b \x01(\t\x12\x0b\n\x03lei\x18\x0c \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\r \x01(\t\"W\n\rSnapshotOhlcv\x12\x0c\n\x04open\x18\x01 \x01(\x01\x12\x0c\n\x04high\x18\x02 \x01(\x01\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\r\n\x05\x63lose\x18\x04 \x01(\x01\x12\x0e\n\x06volume\x18\x05 \x01(\x01\"D\n\x11SnapshotLastTrade\x12\x10\n\x08\x65vent_at\x18\x01 \x01(\x03\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x0e\n\x06shares\x18\x03 \x01(\x03\"\x96\x01\n\x18SnapshotLastFiftyTwoWeek\x12\x0c\n\x04high\x18\x01 \x01(\x01\x12\x0f\n\x07high_at\x18\x02 \x01(\x03\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0e\n\x06low_at\x18\x04 \x01(\x03\x12\x0e\n\x06\x63hange\x18\x05 \x01(\x01\x12\x16\n\x0e\x63hange_percent\x18\x06 \x01(\x01\x12\x16\n\x0e\x61verage_volume\x18\x07 \x01(\x03\"g\n\x0eSnapshotChange\x12\x1a\n\x12\x64\x61y_change_percent\x18\x01 \x01(\x01\x12\x1b\n\x13week_change_percent\x18\x02 \x01(\x01\x12\x1c\n\x14month_change_percent\x18\x03 \x01(\x01\"\xb2\x02\n\x13GetSnapshotResponse\x12(\n\x08last_day\x18\x01 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12*\n\nlast_month\x18\x02 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12.\n\nlast_trade\x18\x03 \x01(\x0b\x32\x1a.finazon.SnapshotLastTrade\x12,\n\x0cprevious_day\x18\x04 \x01(\x0b\x32\x16.finazon.SnapshotOhlcv\x12>\n\x13last_fifty_two_week\x18\x05 \x01(\x0b\x32!.finazon.SnapshotLastFiftyTwoWeek\x12\'\n\x06\x63hange\x18\x06 \x01(\x0b\x32\x17.finazon.SnapshotChange2]\n\x0fSnapshotService\x12J\n\x0bGetSnapshot\x12\x1b.finazon.GetSnapshotRequest\x1a\x1c.finazon.GetSnapshotResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.snapshot_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _globals['_GETSNAPSHOTREQUEST']._serialized_start=48
-  _globals['_GETSNAPSHOTREQUEST']._serialized_end=261
-  _globals['_SNAPSHOTOHLCV']._serialized_start=263
-  _globals['_SNAPSHOTOHLCV']._serialized_end=350
-  _globals['_SNAPSHOTLASTTRADE']._serialized_start=352
-  _globals['_SNAPSHOTLASTTRADE']._serialized_end=420
-  _globals['_SNAPSHOTLASTFIFTYTWOWEEK']._serialized_start=423
-  _globals['_SNAPSHOTLASTFIFTYTWOWEEK']._serialized_end=573
-  _globals['_SNAPSHOTCHANGE']._serialized_start=575
-  _globals['_SNAPSHOTCHANGE']._serialized_end=678
-  _globals['_GETSNAPSHOTRESPONSE']._serialized_start=681
-  _globals['_GETSNAPSHOTRESPONSE']._serialized_end=987
-  _globals['_SNAPSHOTSERVICE']._serialized_start=989
-  _globals['_SNAPSHOTSERVICE']._serialized_end=1082
+  _globals['_GETSNAPSHOTREQUEST']._serialized_end=278
+  _globals['_SNAPSHOTOHLCV']._serialized_start=280
+  _globals['_SNAPSHOTOHLCV']._serialized_end=367
+  _globals['_SNAPSHOTLASTTRADE']._serialized_start=369
+  _globals['_SNAPSHOTLASTTRADE']._serialized_end=437
+  _globals['_SNAPSHOTLASTFIFTYTWOWEEK']._serialized_start=440
+  _globals['_SNAPSHOTLASTFIFTYTWOWEEK']._serialized_end=590
+  _globals['_SNAPSHOTCHANGE']._serialized_start=592
+  _globals['_SNAPSHOTCHANGE']._serialized_end=695
+  _globals['_GETSNAPSHOTRESPONSE']._serialized_start=698
+  _globals['_GETSNAPSHOTRESPONSE']._serialized_end=1004
+  _globals['_SNAPSHOTSERVICE']._serialized_start=1006
+  _globals['_SNAPSHOTSERVICE']._serialized_end=1099
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,28 @@
     CQS_FIELD_NUMBER: builtins.int
     CIK_FIELD_NUMBER: builtins.int
     CUSIP_FIELD_NUMBER: builtins.int
     ISIN_FIELD_NUMBER: builtins.int
     COMPOSITE_FIGI_FIELD_NUMBER: builtins.int
     SHARE_FIGI_FIELD_NUMBER: builtins.int
     LEI_FIELD_NUMBER: builtins.int
+    DATASET_FIELD_NUMBER: builtins.int
     publisher: builtins.str
     ticker: builtins.str
     market: builtins.str
     mic: builtins.str
     country: builtins.str
     cqs: builtins.str
     cik: builtins.str
     cusip: builtins.str
     isin: builtins.str
     composite_figi: builtins.str
     share_figi: builtins.str
     lei: builtins.str
+    dataset: builtins.str
     def __init__(
         self,
         *,
         publisher: builtins.str = ...,
         ticker: builtins.str = ...,
         market: builtins.str = ...,
         mic: builtins.str = ...,
@@ -53,16 +55,17 @@
         cqs: builtins.str = ...,
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
+        dataset: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___GetSnapshotRequest = GetSnapshotRequest
 
 @typing_extensions.final
 class SnapshotOhlcv(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/snapshot_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/snapshot_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!finazon_grpc_python/tickers.proto\x12\x07\x66inazon\"p\n\x10TickerStocksInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x10\n\x08\x63urrency\x18\x03 \x01(\t\x12\x11\n\tpublisher\x18\x04 \x01(\t\x12\x16\n\x0epublisher_name\x18\x05 \x01(\t\"\xec\x01\n\x18\x46indTickersStocksRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\x0b\n\x03\x63qs\x18\x0b \x01(\t\x12\x0b\n\x03\x63ik\x18\x0c \x01(\t\x12\r\n\x05\x63usip\x18\r \x01(\t\x12\x0c\n\x04isin\x18\x0e \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0f \x01(\t\x12\x12\n\nshare_figi\x18\x10 \x01(\t\x12\x0b\n\x03lei\x18\x11 \x01(\t\"E\n\x18\x46indTickerStocksResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.TickerStocksInfo\"M\n\x10TickerCryptoInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x16\n\x0epublisher_name\x18\x03 \x01(\t\"n\n\x18\x46indTickersCryptoRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0e\n\x06market\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\x05\x12\x11\n\tpage_size\x18\x05 \x01(\x05\"E\n\x18\x46indTickerCryptoResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.TickerCryptoInfo\"!\n\x0fTickerForexInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\"J\n\x17\x46indTickersForexRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\"C\n\x17\x46indTickerForexResponse\x12(\n\x06result\x18\x01 \x03(\x0b\x32\x18.finazon.TickerForexInfo\"\xa9\x01\n\x0cTickerUSInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08\x63urrency\x18\x02 \x01(\t\x12\x10\n\x08security\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x12\n\nasset_type\x18\x05 \x01(\t\x12\x0b\n\x03\x63ik\x18\x07 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\n \x01(\t\x12\x12\n\nshare_figi\x18\x0b \x01(\t\x12\x0b\n\x03lei\x18\x0c \x01(\t\"\xc3\x01\n\x13\x46indTickerUSRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0b\n\x03mic\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\x05\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x0b\n\x03\x63qs\x18\x05 \x01(\t\x12\x0b\n\x03\x63ik\x18\x06 \x01(\t\x12\r\n\x05\x63usip\x18\x07 \x01(\t\x12\x0c\n\x04isin\x18\x08 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\t \x01(\t\x12\x12\n\nshare_figi\x18\n \x01(\t\x12\x0b\n\x03lei\x18\x0b \x01(\t\"=\n\x14\x46indTickerUSResponse\x12%\n\x06result\x18\x01 \x03(\x0b\x32\x15.finazon.TickerUSInfo2\xf3\x02\n\x0eTickersService\x12[\n\x11\x46indTickersStocks\x12!.finazon.FindTickersStocksRequest\x1a!.finazon.FindTickerStocksResponse\"\x00\x12[\n\x11\x46indTickersCrypto\x12!.finazon.FindTickersCryptoRequest\x1a!.finazon.FindTickerCryptoResponse\"\x00\x12X\n\x10\x46indTickersForex\x12 .finazon.FindTickersForexRequest\x1a .finazon.FindTickerForexResponse\"\x00\x12M\n\x0c\x46indTickerUS\x12\x1c.finazon.FindTickerUSRequest\x1a\x1d.finazon.FindTickerUSResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!finazon_grpc_python/tickers.proto\x12\x07\x66inazon\"p\n\x10TickerStocksInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x02 \x01(\t\x12\x10\n\x08\x63urrency\x18\x03 \x01(\t\x12\x11\n\tpublisher\x18\x04 \x01(\t\x12\x16\n\x0epublisher_name\x18\x05 \x01(\t\"\xfd\x01\n\x18\x46indTickersStocksRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\x05\x12\x11\n\tpage_size\x18\x06 \x01(\x05\x12\x0b\n\x03\x63qs\x18\x0b \x01(\t\x12\x0b\n\x03\x63ik\x18\x0c \x01(\t\x12\r\n\x05\x63usip\x18\r \x01(\t\x12\x0c\n\x04isin\x18\x0e \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x0f \x01(\t\x12\x12\n\nshare_figi\x18\x10 \x01(\t\x12\x0b\n\x03lei\x18\x11 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x12 \x01(\t\"E\n\x18\x46indTickerStocksResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.TickerStocksInfo\"M\n\x10TickerCryptoInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x16\n\x0epublisher_name\x18\x03 \x01(\t\"n\n\x18\x46indTickersCryptoRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0e\n\x06market\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\x05\x12\x11\n\tpage_size\x18\x05 \x01(\x05\"E\n\x18\x46indTickerCryptoResponse\x12)\n\x06result\x18\x01 \x03(\x0b\x32\x19.finazon.TickerCryptoInfo\"!\n\x0fTickerForexInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\"J\n\x17\x46indTickersForexRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\"C\n\x17\x46indTickerForexResponse\x12(\n\x06result\x18\x01 \x03(\x0b\x32\x18.finazon.TickerForexInfo\"\xa9\x01\n\x0cTickerUSInfo\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x10\n\x08\x63urrency\x18\x02 \x01(\t\x12\x10\n\x08security\x18\x03 \x01(\t\x12\x0b\n\x03mic\x18\x04 \x01(\t\x12\x12\n\nasset_type\x18\x05 \x01(\t\x12\x0b\n\x03\x63ik\x18\x07 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\n \x01(\t\x12\x12\n\nshare_figi\x18\x0b \x01(\t\x12\x0b\n\x03lei\x18\x0c \x01(\t\"\xc3\x01\n\x13\x46indTickerUSRequest\x12\x0e\n\x06ticker\x18\x01 \x01(\t\x12\x0b\n\x03mic\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\x05\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x0b\n\x03\x63qs\x18\x05 \x01(\t\x12\x0b\n\x03\x63ik\x18\x06 \x01(\t\x12\r\n\x05\x63usip\x18\x07 \x01(\t\x12\x0c\n\x04isin\x18\x08 \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\t \x01(\t\x12\x12\n\nshare_figi\x18\n \x01(\t\x12\x0b\n\x03lei\x18\x0b \x01(\t\"=\n\x14\x46indTickerUSResponse\x12%\n\x06result\x18\x01 \x03(\x0b\x32\x15.finazon.TickerUSInfo2\xf3\x02\n\x0eTickersService\x12[\n\x11\x46indTickersStocks\x12!.finazon.FindTickersStocksRequest\x1a!.finazon.FindTickerStocksResponse\"\x00\x12[\n\x11\x46indTickersCrypto\x12!.finazon.FindTickersCryptoRequest\x1a!.finazon.FindTickerCryptoResponse\"\x00\x12X\n\x10\x46indTickersForex\x12 .finazon.FindTickersForexRequest\x1a .finazon.FindTickerForexResponse\"\x00\x12M\n\x0c\x46indTickerUS\x12\x1c.finazon.FindTickerUSRequest\x1a\x1d.finazon.FindTickerUSResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.tickers_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _globals['_TICKERSTOCKSINFO']._serialized_start=46
   _globals['_TICKERSTOCKSINFO']._serialized_end=158
   _globals['_FINDTICKERSSTOCKSREQUEST']._serialized_start=161
-  _globals['_FINDTICKERSSTOCKSREQUEST']._serialized_end=397
-  _globals['_FINDTICKERSTOCKSRESPONSE']._serialized_start=399
-  _globals['_FINDTICKERSTOCKSRESPONSE']._serialized_end=468
-  _globals['_TICKERCRYPTOINFO']._serialized_start=470
-  _globals['_TICKERCRYPTOINFO']._serialized_end=547
-  _globals['_FINDTICKERSCRYPTOREQUEST']._serialized_start=549
-  _globals['_FINDTICKERSCRYPTOREQUEST']._serialized_end=659
-  _globals['_FINDTICKERCRYPTORESPONSE']._serialized_start=661
-  _globals['_FINDTICKERCRYPTORESPONSE']._serialized_end=730
-  _globals['_TICKERFOREXINFO']._serialized_start=732
-  _globals['_TICKERFOREXINFO']._serialized_end=765
-  _globals['_FINDTICKERSFOREXREQUEST']._serialized_start=767
-  _globals['_FINDTICKERSFOREXREQUEST']._serialized_end=841
-  _globals['_FINDTICKERFOREXRESPONSE']._serialized_start=843
-  _globals['_FINDTICKERFOREXRESPONSE']._serialized_end=910
-  _globals['_TICKERUSINFO']._serialized_start=913
-  _globals['_TICKERUSINFO']._serialized_end=1082
-  _globals['_FINDTICKERUSREQUEST']._serialized_start=1085
-  _globals['_FINDTICKERUSREQUEST']._serialized_end=1280
-  _globals['_FINDTICKERUSRESPONSE']._serialized_start=1282
-  _globals['_FINDTICKERUSRESPONSE']._serialized_end=1343
-  _globals['_TICKERSSERVICE']._serialized_start=1346
-  _globals['_TICKERSSERVICE']._serialized_end=1717
+  _globals['_FINDTICKERSSTOCKSREQUEST']._serialized_end=414
+  _globals['_FINDTICKERSTOCKSRESPONSE']._serialized_start=416
+  _globals['_FINDTICKERSTOCKSRESPONSE']._serialized_end=485
+  _globals['_TICKERCRYPTOINFO']._serialized_start=487
+  _globals['_TICKERCRYPTOINFO']._serialized_end=564
+  _globals['_FINDTICKERSCRYPTOREQUEST']._serialized_start=566
+  _globals['_FINDTICKERSCRYPTOREQUEST']._serialized_end=676
+  _globals['_FINDTICKERCRYPTORESPONSE']._serialized_start=678
+  _globals['_FINDTICKERCRYPTORESPONSE']._serialized_end=747
+  _globals['_TICKERFOREXINFO']._serialized_start=749
+  _globals['_TICKERFOREXINFO']._serialized_end=782
+  _globals['_FINDTICKERSFOREXREQUEST']._serialized_start=784
+  _globals['_FINDTICKERSFOREXREQUEST']._serialized_end=858
+  _globals['_FINDTICKERFOREXRESPONSE']._serialized_start=860
+  _globals['_FINDTICKERFOREXRESPONSE']._serialized_end=927
+  _globals['_TICKERUSINFO']._serialized_start=930
+  _globals['_TICKERUSINFO']._serialized_end=1099
+  _globals['_FINDTICKERUSREQUEST']._serialized_start=1102
+  _globals['_FINDTICKERUSREQUEST']._serialized_end=1297
+  _globals['_FINDTICKERUSRESPONSE']._serialized_start=1299
+  _globals['_FINDTICKERUSRESPONSE']._serialized_end=1360
+  _globals['_TICKERSSERVICE']._serialized_start=1363
+  _globals['_TICKERSSERVICE']._serialized_end=1734
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -59,27 +59,29 @@
     CQS_FIELD_NUMBER: builtins.int
     CIK_FIELD_NUMBER: builtins.int
     CUSIP_FIELD_NUMBER: builtins.int
     ISIN_FIELD_NUMBER: builtins.int
     COMPOSITE_FIGI_FIELD_NUMBER: builtins.int
     SHARE_FIGI_FIELD_NUMBER: builtins.int
     LEI_FIELD_NUMBER: builtins.int
+    DATASET_FIELD_NUMBER: builtins.int
     ticker: builtins.str
     publisher: builtins.str
     country: builtins.str
     mic: builtins.str
     page: builtins.int
     page_size: builtins.int
     cqs: builtins.str
     cik: builtins.str
     cusip: builtins.str
     isin: builtins.str
     composite_figi: builtins.str
     share_figi: builtins.str
     lei: builtins.str
+    dataset: builtins.str
     def __init__(
         self,
         *,
         ticker: builtins.str = ...,
         publisher: builtins.str = ...,
         country: builtins.str = ...,
         mic: builtins.str = ...,
@@ -88,16 +90,17 @@
         cqs: builtins.str = ...,
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
+        dataset: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "isin", b"isin", "lei", b"lei", "mic", b"mic", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "isin", b"isin", "lei", b"lei", "mic", b"mic", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "ticker", b"ticker"]) -> None: ...
 
 global___FindTickersStocksRequest = FindTickersStocksRequest
 
 @typing_extensions.final
 class FindTickerStocksResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/tickers_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/tickers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/time_series_service.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/time_series_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_pb2.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66inazon_grpc_python/trade.proto\x12\x07\x66inazon\"A\n\nTradesItem\x12\x12\n\ntrade_date\x18\x01 \x01(\x03\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x10\n\x08quantity\x18\x03 \x01(\x03\"\xb3\x02\n\x10GetTradesRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0b\n\x03mic\x18\x03 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x0e\n\x06market\x18\x05 \x01(\t\x12\x10\n\x08start_at\x18\x06 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x07 \x01(\x03\x12\x0c\n\x04tape\x18\x08 \x01(\t\x12\x0c\n\x04page\x18\t \x01(\x05\x12\x11\n\tpage_size\x18\n \x01(\x05\x12\r\n\x05order\x18\x0b \x01(\t\x12\x0b\n\x03\x63qs\x18\x0c \x01(\t\x12\x0b\n\x03\x63ik\x18\r \x01(\t\x12\r\n\x05\x63usip\x18\x0e \x01(\t\x12\x0c\n\x04isin\x18\x0f \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x10 \x01(\t\x12\x12\n\nshare_figi\x18\x11 \x01(\t\x12\x0b\n\x03lei\x18\x12 \x01(\t\"8\n\x11GetTradesResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.finazon.TradesItem2T\n\x0cTradeService\x12\x44\n\tGetTrades\x12\x19.finazon.GetTradesRequest\x1a\x1a.finazon.GetTradesResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66inazon_grpc_python/trade.proto\x12\x07\x66inazon\"A\n\nTradesItem\x12\x12\n\ntrade_date\x18\x01 \x01(\x03\x12\r\n\x05price\x18\x02 \x01(\x01\x12\x10\n\x08quantity\x18\x03 \x01(\x03\"\xc4\x02\n\x10GetTradesRequest\x12\x11\n\tpublisher\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0b\n\x03mic\x18\x03 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x0e\n\x06market\x18\x05 \x01(\t\x12\x10\n\x08start_at\x18\x06 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x07 \x01(\x03\x12\x0c\n\x04tape\x18\x08 \x01(\t\x12\x0c\n\x04page\x18\t \x01(\x05\x12\x11\n\tpage_size\x18\n \x01(\x05\x12\r\n\x05order\x18\x0b \x01(\t\x12\x0b\n\x03\x63qs\x18\x0c \x01(\t\x12\x0b\n\x03\x63ik\x18\r \x01(\t\x12\r\n\x05\x63usip\x18\x0e \x01(\t\x12\x0c\n\x04isin\x18\x0f \x01(\t\x12\x16\n\x0e\x63omposite_figi\x18\x10 \x01(\t\x12\x12\n\nshare_figi\x18\x11 \x01(\t\x12\x0b\n\x03lei\x18\x12 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x13 \x01(\t\"8\n\x11GetTradesResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.finazon.TradesItem2T\n\x0cTradeService\x12\x44\n\tGetTrades\x12\x19.finazon.GetTradesRequest\x1a\x1a.finazon.GetTradesResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'finazon_grpc_python.trade_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _globals['_TRADESITEM']._serialized_start=44
   _globals['_TRADESITEM']._serialized_end=109
   _globals['_GETTRADESREQUEST']._serialized_start=112
-  _globals['_GETTRADESREQUEST']._serialized_end=419
-  _globals['_GETTRADESRESPONSE']._serialized_start=421
-  _globals['_GETTRADESRESPONSE']._serialized_end=477
-  _globals['_TRADESERVICE']._serialized_start=479
-  _globals['_TRADESERVICE']._serialized_end=563
+  _globals['_GETTRADESREQUEST']._serialized_end=436
+  _globals['_GETTRADESRESPONSE']._serialized_start=438
+  _globals['_GETTRADESRESPONSE']._serialized_end=494
+  _globals['_TRADESERVICE']._serialized_start=496
+  _globals['_TRADESERVICE']._serialized_end=580
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_pb2.pyi` & `finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     CQS_FIELD_NUMBER: builtins.int
     CIK_FIELD_NUMBER: builtins.int
     CUSIP_FIELD_NUMBER: builtins.int
     ISIN_FIELD_NUMBER: builtins.int
     COMPOSITE_FIGI_FIELD_NUMBER: builtins.int
     SHARE_FIGI_FIELD_NUMBER: builtins.int
     LEI_FIELD_NUMBER: builtins.int
+    DATASET_FIELD_NUMBER: builtins.int
     publisher: builtins.str
     ticker: builtins.str
     mic: builtins.str
     country: builtins.str
     market: builtins.str
     start_at: builtins.int
     end_at: builtins.int
@@ -73,14 +74,15 @@
     cqs: builtins.str
     cik: builtins.str
     cusip: builtins.str
     isin: builtins.str
     composite_figi: builtins.str
     share_figi: builtins.str
     lei: builtins.str
+    dataset: builtins.str
     def __init__(
         self,
         *,
         publisher: builtins.str = ...,
         ticker: builtins.str = ...,
         mic: builtins.str = ...,
         country: builtins.str = ...,
@@ -94,16 +96,17 @@
         cqs: builtins.str = ...,
         cik: builtins.str = ...,
         cusip: builtins.str = ...,
         isin: builtins.str = ...,
         composite_figi: builtins.str = ...,
         share_figi: builtins.str = ...,
         lei: builtins.str = ...,
+        dataset: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "start_at", b"start_at", "tape", b"tape", "ticker", b"ticker"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cik", b"cik", "composite_figi", b"composite_figi", "country", b"country", "cqs", b"cqs", "cusip", b"cusip", "dataset", b"dataset", "end_at", b"end_at", "isin", b"isin", "lei", b"lei", "market", b"market", "mic", b"mic", "order", b"order", "page", b"page", "page_size", b"page_size", "publisher", b"publisher", "share_figi", b"share_figi", "start_at", b"start_at", "tape", b"tape", "ticker", b"ticker"]) -> None: ...
 
 global___GetTradesRequest = GetTradesRequest
 
 @typing_extensions.final
 class GetTradesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `finazon_grpc_python-1.0.136.2/finazon_grpc_python/trade_pb2_grpc.py` & `finazon_grpc_python-1.0.141/finazon_grpc_python/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.136.2/pyproject.toml` & `finazon_grpc_python-1.0.141/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "finazon-grpc-python"
 packages = [{include = "finazon_grpc_python"}]
 include = ["requirements.txt", "finazon_grpc_python/*.p*"]
-version = "1.0.136.2"
+version = "1.0.141"
 description = "Finazon gRPC client library for Python"
 authors = ["Finazon <team@finazon.io>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/finazon-io/finazon-grpc-python"
 repository = "https://github.com/finazon-io/finazon-grpc-python"
```

### Comparing `finazon_grpc_python-1.0.136.2/PKG-INFO` & `finazon_grpc_python-1.0.141/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finazon-grpc-python
-Version: 1.0.136.2
+Version: 1.0.141
 Summary: Finazon gRPC client library for Python
 Home-page: https://github.com/finazon-io/finazon-grpc-python
 License: MIT
 Author: Finazon
 Author-email: team@finazon.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

