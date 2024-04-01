# Comparing `tmp/talipp-2.1.1.tar.gz` & `tmp/talipp-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talipp-2.1.1.tar", last modified: Mon Mar 25 21:39:28 2024, max compression
+gzip compressed data, was "talipp-2.1.2.tar", last modified: Mon Apr  1 21:54:14 2024, max compression
```

## Comparing `talipp-2.1.1.tar` & `talipp-2.1.2.tar`

### file list

```diff
@@ -1,77 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:39:28.111924 talipp-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-25 21:39:18.000000 talipp-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-25 21:39:18.000000 talipp-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-03-25 21:39:28.111924 talipp-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-03-25 21:39:18.000000 talipp-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 21:39:18.000000 talipp-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 21:39:28.111924 talipp-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-25 21:39:18.000000 talipp-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:39:28.103924 talipp-2.1.1/talipp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicator_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:39:28.111924 talipp-2.1.1/talipp/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ADX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ALMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/AO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ATR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/AccuDist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/Aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/BB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/BOP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/CCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/CHOP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ChaikinOsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ChandeKrollStop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/CoppockCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/DEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/DPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/DonchianChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/EMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/EMV.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/FibRetracement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ForceIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/HMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/Ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/Indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/KAMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/KST.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/KVO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/KeltnerChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/MACD.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/MassIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/McGinleyDynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/MeanDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/OBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ParabolicSAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/PivotsHL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ROC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/RSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/SFX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/SMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/SMMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/SOBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/STC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/StdDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/Stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/StochRSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/SuperTrend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/T3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/TEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/TRIX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/TSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/TTM.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/UO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/VTX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/VWAP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/VWMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/WMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/ZLEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/indicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/ma.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-03-25 21:39:18.000000 talipp-2.1.1/talipp/ohlcv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:39:28.103924 talipp-2.1.1/talipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-03-25 21:39:27.000000 talipp-2.1.1/talipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-25 21:39:28.000000 talipp-2.1.1/talipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 21:39:27.000000 talipp-2.1.1/talipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 21:39:27.000000 talipp-2.1.1/talipp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:14.645612 talipp-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 21:54:05.000000 talipp-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 21:54:05.000000 talipp-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-04-01 21:54:14.645612 talipp-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-01 21:54:05.000000 talipp-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:05.000000 talipp-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:54:14.645612 talipp-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-01 21:54:05.000000 talipp-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:14.629612 talipp-2.1.2/talipp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicator_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:14.637612 talipp-2.1.2/talipp/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ADX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ALMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/AO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ATR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/AccuDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/Aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/BB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/BOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/CCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/CHOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ChaikinOsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ChandeKrollStop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/CoppockCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/DEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/DPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/DonchianChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/EMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/EMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/FibRetracement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ForceIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/HMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/Ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/Indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/KAMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/KST.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/KVO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/KeltnerChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/MACD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/MassIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/McGinleyDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/MeanDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/OBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ParabolicSAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/PivotsHL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ROC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/RSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/SFX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/SMMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/SOBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/STC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/StdDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/Stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/StochRSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/SuperTrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/T3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/TEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/TRIX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/TSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/TTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/UO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/VTX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/VWAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/VWMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/WMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/ZLEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/ma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-01 21:54:05.000000 talipp-2.1.2/talipp/ohlcv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:14.629612 talipp-2.1.2/talipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-04-01 21:54:14.000000 talipp-2.1.2/talipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-01 21:54:14.000000 talipp-2.1.2/talipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:54:14.000000 talipp-2.1.2/talipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:54:14.000000 talipp-2.1.2/talipp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:54:14.645612 talipp-2.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ADX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ALMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_AO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ATR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_AccuDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_Aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_BB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_BOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_CCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_CHOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ChaikinOsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ChandeKrollStop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_CoppockCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_DEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_DPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_DonchianChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_EMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_EMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ForceIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_HMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_KAMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_KST.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_KVO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_KeltnerChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_MACD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_MassIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_McGinleyDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_MeanDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_OBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_OHLCV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ParabolicSAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ROC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_RSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_SFX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_SMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_SMMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_SOBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_STC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_StdDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_Stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_StochRSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_SuperTrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_T3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_TEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_TRIX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_TSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_TTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_UO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_VTX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_VWAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_VWMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_WMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_ZLEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_indicator_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_indicator_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_indicator_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-01 21:54:05.000000 talipp-2.1.2/test/test_input.py
```

### Comparing `talipp-2.1.1/LICENSE` & `talipp-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talipp-2.1.1/PKG-INFO` & `talipp-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: talipp
-Version: 2.1.1
-Summary: TALi++ - Incremental Technical Analysis Library
+Version: 2.1.2
+Summary: talipp - Incremental Technical Analysis Library
 Home-page: https://github.com/nardew/talipp
 Author: nardew
 Author-email: talipp.pyth@gmail.com
 License: UNKNOWN
-Description: # TALIpp - Incremental Technical Analysis Library
+Description: # talipp - Incremental Technical Analysis Library
         
         ![](https://img.shields.io/badge/python-3.8-blue.svg) 
         ![](https://img.shields.io/badge/python-3.9-blue.svg)
         ![](https://img.shields.io/badge/python-3.10-blue.svg)
         ![](https://img.shields.io/badge/python-3.11-blue.svg)
         ![PyPy](https://img.shields.io/badge/pypy-3-blue.svg)
         ![unit tests](https://github.com/nardew/talipp/workflows/unit%20tests/badge.svg)
         
         ---
         
-        ## New major release `talipp 2.0.0` available!
-        
-        - Scope: https://github.com/nardew/talipp/issues/111
-        - PR: https://github.com/nardew/talipp/pull/96
+        ## !!! [New documentation page available](https://nardew.github.io/talipp) !!!
         
         ---
         
         `talipp` (or `tali++`) is a Python library implementing financial indicators for technical analysis. The distinctive feature of the library is its incremental computation which fits extremely well real-time applications or applications with iterative input in general.  
         
         Unlike existing libraries for technical analysis which typically have to work on the whole input vector in order to calculate new values of indicators, `talipp` due to its incremental architecture calculates new indicators' values exclusively based on the delta input data. That implies, among others, it requires `O(1)` time to produce new values in comparison to `O(n)` required by other libraries.
```

### Comparing `talipp-2.1.1/README.md` & `talipp-2.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-# TALIpp - Incremental Technical Analysis Library
+# talipp - Incremental Technical Analysis Library
 
 ![](https://img.shields.io/badge/python-3.8-blue.svg) 
 ![](https://img.shields.io/badge/python-3.9-blue.svg)
 ![](https://img.shields.io/badge/python-3.10-blue.svg)
 ![](https://img.shields.io/badge/python-3.11-blue.svg)
 ![PyPy](https://img.shields.io/badge/pypy-3-blue.svg)
 ![unit tests](https://github.com/nardew/talipp/workflows/unit%20tests/badge.svg)
 
 ---
 
-## New major release `talipp 2.0.0` available!
-
-- Scope: https://github.com/nardew/talipp/issues/111
-- PR: https://github.com/nardew/talipp/pull/96
+## !!! [New documentation page available](https://nardew.github.io/talipp) !!!
 
 ---
 
 `talipp` (or `tali++`) is a Python library implementing financial indicators for technical analysis. The distinctive feature of the library is its incremental computation which fits extremely well real-time applications or applications with iterative input in general.  
 
 Unlike existing libraries for technical analysis which typically have to work on the whole input vector in order to calculate new values of indicators, `talipp` due to its incremental architecture calculates new indicators' values exclusively based on the delta input data. That implies, among others, it requires `O(1)` time to produce new values in comparison to `O(n)` required by other libraries.
```

### Comparing `talipp-2.1.1/setup.py` & `talipp-2.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.readlines()
 requirements = [line.strip() for line in requirements]
 
+with open("VERSION", "r") as fh:
+    version = fh.read()
+
 setuptools.setup(
     name="talipp",
-    version="2.1.1",
+    version=version,
     author="nardew",
     author_email="talipp.pyth@gmail.com",
-    description="TALi++ - Incremental Technical Analysis Library",
+    description="talipp - Incremental Technical Analysis Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nardew/talipp",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `talipp-2.1.1/talipp/indicators/ADX.py` & `talipp-2.1.2/talipp/indicators/ADX.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,41 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 @dataclass
 class ADXVal:
+    """`ADX` output type.
+
+    Args:
+        adx: ADX.
+        plus_di: Plus Directional Movement.
+        minus_di: Minus Directional Movement.
+    """
+
     adx: float = None
     plus_di: float = None
     minus_di: float = None
 
 
 class ADX(Indicator):
-    """
-    Average Directional Index
+    """Average Directional Index.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [ADXVal][talipp.indicators.ADX.ADXVal]
 
-    Output: a list of ADXVal
+    Args:
+        di_period: Directional Index period.
+        adx_period: Average Directional Index period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, di_period: int,
                  adx_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/ALMA.py` & `talipp-2.1.2/talipp/indicators/ALMA.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,28 @@
 from typing import List, Any
 
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class ALMA(Indicator):
-    """
-    Arnaud Legoux Moving Average
+    """Arnaud Legoux Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Moving average period.
+        offset: Weights offset.
+        sigma: Weights sigma factor.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  offset: float,
                  sigma: float,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/AO.py` & `talipp-2.1.2/talipp/indicators/AO.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV
 
 
 class AO(Indicator):
-    """
-    Awesome Oscillator
+    """Awesome Oscillator.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_period: Fast moving average period.
+        slow_period: Slow moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_period: int,
                  slow_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/ATR.py` & `talipp-2.1.2/talipp/indicators/ATR.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class ATR(Indicator):
-    """
-    Average True Range
+    """Average True Range
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
```

### Comparing `talipp-2.1.1/talipp/indicators/AccuDist.py` & `talipp-2.1.2/talipp/indicators/AccuDist.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,25 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class AccuDist(Indicator):
-    """
-    Accumulation and Distribution
+    """Accumulation and Distribution Line.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(
```

### Comparing `talipp-2.1.1/talipp/indicators/Aroon.py` & `talipp-2.1.2/talipp/indicators/Aroon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 from dataclasses import dataclass
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
+from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 @dataclass
 class AroonVal:
+    """`Aroon` output type.
+
+    Args:
+        up: Aroon up.
+        down: Aroon down.
+    """
+
     up: float = None
     down: float = None
 
 
 class Aroon(Indicator):
-    """
-    Aroon Up/Down
+    """Aroon Up/Down
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [AroonVal][talipp.indicators.Aroon.AroonVal]
 
-    Output: a list of AroonVal
+    Args:
+        period: Aroon period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
-                 input_modifier: InputModifierType = None):
+                 input_modifier: InputModifierType = None,
+                 input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          output_value_type=AroonVal,
-                         input_sampling=input_modifier)
+                         input_sampling=input_sampling)
 
         self.period = period
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
         if not has_valid_values(self.input_values, self.period+1):
```

### Comparing `talipp-2.1.1/talipp/indicators/BB.py` & `talipp-2.1.2/talipp/indicators/BB.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,41 @@
 from talipp.indicators.StdDev import StdDev
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 
 
 @dataclass
 class BBVal:
-    # lower band
-    lb: float = None
+    """`BB` output type.
 
-    # central band
-    cb: float = None
+    Args:
+        lb: Lower band.
+        cb: Central band.
+        ub: Upper band.
+    """
 
-    # upper band
+    lb: float = None
+    cb: float = None
     ub: float = None
 
 
 class BB(Indicator):
-    """
-    Bollinger Bands
+    """Bollinger Bands.
+
+    Input type: `float`
+
+    Output type: [BBVal][talipp.indicators.BB.BBVal]
 
-    Output: a list of BBVal
+    Args:
+        period: Period.
+        std_dev_mult: Standard deviation multiplier.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  std_dev_mult: float,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/BOP.py` & `talipp-2.1.2/talipp/indicators/BOP.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class BOP(Indicator):
-    """
-    Balance Of Power
+    """Balance Of Power.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
```

### Comparing `talipp-2.1.1/talipp/indicators/CCI.py` & `talipp-2.1.2/talipp/indicators/CCI.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,26 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.indicators.MeanDev import MeanDev
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class CCI(Indicator):
-    """
-    Commodity Channel Index
+    """Commodity Channel Index.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of OHLCV objects
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
@@ -32,9 +40,9 @@
         typical_price = (value.high + value.low + value.close) / 3.0
 
         self.mean_dev.add(typical_price)
 
         if not has_valid_values(self.mean_dev, 1):
             return None
 
-        # take SMA(typical_price) directly form MeanDev since it is already calculating it in the background
+        # take SMA(typical_price) directly from MeanDev since it is already calculating it in the background
         return (typical_price - self.mean_dev.ma[-1]) / (0.015 * self.mean_dev[-1])
```

### Comparing `talipp-2.1.1/talipp/indicators/CHOP.py` & `talipp-2.1.2/talipp/indicators/ForceIndex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-from math import log10
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
-from talipp.indicators.ATR import ATR
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
+from talipp.ma import MAFactory, MAType
 from talipp.ohlcv import OHLCV
 
 
-class CHOP(Indicator):
-    """
-    Choppiness Index
+class ForceIndex(Indicator):
+    """Force Index.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of OHLCV objects
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
+                 ma_type: MAType = MAType.EMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
-        self.period = period
-
-        self.atr = ATR(1)
-        self.add_sub_indicator(self.atr)
+        self.ma = MAFactory.get_ma(ma_type, period)
+        self.add_managed_sequence(self.ma)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.atr, self.period) or not has_valid_values(self.input_values, self.period):
+        if not has_valid_values(self.input_values, 2):
             return None
 
-        max_high = max(self.input_values[-self.period:], key = lambda x: x.high).high
-        min_low = min(self.input_values[-self.period:], key = lambda x: x.low).low
+        self.ma.add((self.input_values[-1].close - self.input_values[-2].close) * self.input_values[-1].volume)
 
-        if max_high != min_low:
-            return 100.0 * log10(sum(self.atr[-self.period:]) / (max_high - min_low) ) / log10(self.period)
-        else:
+        if not has_valid_values(self.ma, 1):
             return None
+
+        return self.ma[-1]
```

### Comparing `talipp-2.1.1/talipp/indicators/ChaikinOsc.py` & `talipp-2.1.2/talipp/indicators/ChaikinOsc.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,27 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV
 
 
 class ChaikinOsc(Indicator):
-    """
-    Chaikin Oscillator
+    """Chaikin Oscillator.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_period: Fast moving average period.
+        slow_period: Slow moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_period: int,
                  slow_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/ChandeKrollStop.py` & `talipp-2.1.2/talipp/indicators/ChandeKrollStop.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,39 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 @dataclass
 class ChandeKrollStopVal:
+    """`ChandeKrollStop` output type.
+
+        Args:
+            short_stop: Stop price for shorts.
+            long_stop: Stop price for longs.
+        """
+
     short_stop: float = None
     long_stop: float = None
 
 
 class ChandeKrollStop(Indicator):
-    """
-    Chande Kroll Stop
+    """Chande Kroll Stop.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [ChandeKrollStopVal][talipp.indicators.ChandeKrollStop.ChandeKrollStopVal]
 
-    Output: a list of ChandeKrollStopVal objects
+    Args:
+        atr_period: ATR period.
+        atr_mult: ATR multiplier.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, atr_period: int,
                  atr_mult: float,
                  period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/CoppockCurve.py` & `talipp-2.1.2/talipp/indicators/CoppockCurve.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.indicators.ROC import ROC
 from talipp.indicators.WMA import WMA
 from talipp.input import SamplingPeriodType
 
 
 class CoppockCurve(Indicator):
-    """
-    CoppockCurve
+    """CoppockCurve.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_roc_period: Fast [ROC][talipp.indicators.ROC] period.
+        slow_roc_period: Slow [ROC][talipp.indicators.ROC] period.
+        wma_period: [WMA][talipp.indicators.WMA] period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_roc_period: int,
                  slow_roc_period: int,
                  wma_period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/DEMA.py` & `talipp-2.1.2/talipp/indicators/DEMA.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.EMA import EMA
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class DEMA(Indicator):
-    """
-    Double Exponential Moving Average
+    """Double Exponential Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
```

### Comparing `talipp-2.1.1/talipp/indicators/DPO.py` & `talipp-2.1.2/talipp/indicators/HMA.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,54 @@
+from math import sqrt
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
+from talipp.indicators.WMA import WMA
 from talipp.input import SamplingPeriodType
-from talipp.ma import MAType, MAFactory
 
 
-class DPO(Indicator):
-    """
-    Detrended Price Oscillator
+class HMA(Indicator):
+    """Hull Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
-                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
         self.period = period
 
-        self.ma = MAFactory.get_ma(ma_type, period)
-        self.add_sub_indicator(self.ma)
+        self.wma = WMA(period)
+        self.wma2 = WMA(int(period / 2))
+        self.hma = WMA(int(sqrt(period)))
+
+        self.add_sub_indicator(self.wma)
+        self.add_sub_indicator(self.wma2)
+        self.add_managed_sequence(self.hma)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, int(self.period / 2) + 2) or not has_valid_values(self.ma, 1):
+        if not has_valid_values(self.wma, int(sqrt(self.period))):
+            return None
+
+        self.hma.add(2.0 * self.wma2[-1] - self.wma[-1])
+
+        if not has_valid_values(self.hma, 1):
             return None
 
-        return self.input_values[-(int(self.period / 2) + 1) - 1] - float(self.ma[-1])
+        return self.hma[-1]
```

### Comparing `talipp-2.1.1/talipp/indicators/DonchianChannels.py` & `talipp-2.1.2/talipp/indicators/DonchianChannels.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,40 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 @dataclass
 class DonchianChannelsVal:
-    # lower band
-    lb: float = None
+    """`DonchianChannels` output type.
 
-    # central band
-    cb: float = None
+    Args:
+        lb: Lower band.
+        cb: Central band.
+        ub: Upper band.
+    """
 
-    # upper band
+    lb: float = None
+    cb: float = None
     ub: float = None
 
 
 class DonchianChannels(Indicator):
-    """
-    Donchian Channels
+    """Donchian Channels.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [DonchianChannelsVal][talipp.indicators.DonchianChannels.DonchianChannelsVal]
 
-    Output: a list of DonnchianChannelsVal
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
     def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
```

### Comparing `talipp-2.1.1/talipp/indicators/EMA.py` & `talipp-2.1.2/talipp/indicators/EMA.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class EMA(Indicator):
-    """
-    Exponential Moving Average
+    """Exponential Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
```

### Comparing `talipp-2.1.1/talipp/indicators/EMV.py` & `talipp-2.1.2/talipp/indicators/VWMA.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
-from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV
 
 
-class EMV(Indicator):
-    """
-    Ease of Movement
+class VWMA(Indicator):
+    """Volume Weighted Moving Average.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
-                 volume_div: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
-                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
         self.period = period
-        self.volume_div = volume_div
-
-        self.emv_sma = MAFactory.get_ma(ma_type, period)
-        self.add_managed_sequence(self.emv_sma)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, 2):
+        if not has_valid_values(self.input_values, self.period):
             return None
-
-        value = self.input_values[-1]
-        value2 = self.input_values[-2]
-        if value.high != value.low:
-            distance = (value.high + value.low) / 2.0 - (value2.high + value2.low) / 2.0
-            box_ratio = (value.volume / float(self.volume_div)) / (value.high - value.low)
-            emv = distance / box_ratio
         else:
-            emv = 0.0
-
-        self.emv_sma.add(emv)
+            s = 0.0
+            v = 0.0
+            for value in self.input_values[-self.period:]:
+                s += value.close * value.volume
+                v += value.volume
 
-        if not has_valid_values(self.emv_sma, 1):
-            return None
-        else:
-            return self.emv_sma[-1]
+            return s / v
```

### Comparing `talipp-2.1.1/talipp/indicators/ForceIndex.py` & `talipp-2.1.2/talipp/indicators/ZLEMA.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
+from talipp.indicators.EMA import EMA
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
-from talipp.ma import MAFactory, MAType
-from talipp.ohlcv import OHLCV
 
 
-class ForceIndex(Indicator):
-    """
-    Force Index
+class ZLEMA(Indicator):
+    """Zero Lag Exponential Moving Average.
+
+    Input type: `float`
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
-                 input_values: List[OHLCV] = None,
+                 input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
-                 ma_type: MAType = MAType.EMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
-        self.ma = MAFactory.get_ma(ma_type, period)
-        self.add_managed_sequence(self.ma)
+        self.lag = round((period - 1) / 2.0)
+
+        self.ema = EMA(period)
+        self.add_managed_sequence(self.ema)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, 2):
+        if not has_valid_values(self.input_values, self.lag+1):
             return None
 
-        self.ma.add((self.input_values[-1].close - self.input_values[-2].close) * self.input_values[-1].volume)
+        self.ema.add(self.input_values[-1] + (self.input_values[-1] - self.input_values[-self.lag-1]))
 
-        if not has_valid_values(self.ma, 1):
+        if not has_valid_values(self.ema):
             return None
 
-        return self.ma[-1]
+        return self.ema[-1]
```

### Comparing `talipp-2.1.1/talipp/indicators/HMA.py` & `talipp-2.1.2/talipp/indicators/TRIX.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from math import sqrt
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
+from talipp.indicators.EMA import EMA
 from talipp.indicators.Indicator import Indicator, InputModifierType
-from talipp.indicators.WMA import WMA
 from talipp.input import SamplingPeriodType
 
 
-class HMA(Indicator):
-    """
-    Hull Moving Average
+class TRIX(Indicator):
+    """TRIX.
+
+    Input type: `float`
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
         self.period = period
 
-        self.wma = WMA(period)
-        self.wma2 = WMA(int(period / 2))
-        self.hma = WMA(int(sqrt(period)))
-
-        self.add_sub_indicator(self.wma)
-        self.add_sub_indicator(self.wma2)
-        self.add_managed_sequence(self.hma)
+        self.ema1 = EMA(period)
+        self.ema2 = EMA(period, input_indicator = self.ema1)
+        self.ema3 = EMA(period, input_indicator = self.ema2)
+
+        self.add_sub_indicator(self.ema1)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.wma, int(sqrt(self.period))):
-            return None
-
-        self.hma.add(2.0 * self.wma2[-1] - self.wma[-1])
-
-        if not has_valid_values(self.hma, 1):
+        if not has_valid_values(self.ema3, 2):
             return None
 
-        return self.hma[-1]
+        return 10000.0 * (self.ema3[-1] - self.ema3[-2]) / self.ema3[-2]
```

### Comparing `talipp-2.1.1/talipp/indicators/Ichimoku.py` & `talipp-2.1.2/talipp/indicators/Ichimoku.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,48 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 @dataclass
 class IchimokuVal:
-    base_line: float = None         # Kijun Sen
-    conversion_line: float = None   # Tenkan Sen
-    lagging_line: float = None      # Chikou Span
-    cloud_leading_fast_line: float = None   # Senkou Span
-    cloud_leading_slow_line: float = None   # Senkou Span
+    """`Ichimoku` output type.
+
+    Args:
+        base_line: Kijun Sen.
+        conversion_line: Tenkan Sen.
+        lagging_line: Chikou Span.
+        cloud_leading_fast_line: Senkou Span.
+        cloud_leading_slow_line: Senkou Span.
+    """
+
+    base_line: float = None
+    conversion_line: float = None
+    lagging_line: float = None
+    cloud_leading_fast_line: float = None
+    cloud_leading_slow_line: float = None
 
 
 class Ichimoku(Indicator):
-    """
-    Ichimoku Clouds
+    """Ichimoku Cloud.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [IchimokuVal][talipp.indicators.Ichimoku.IchimokuVal]
 
-    Output: a list of IchimokuVal
+    Args:
+        kijun_period: Kijun (base line) period.
+        tenkan_period: Tenkan (conversion line) period.
+        chikou_lag_period: Chikou (lagging line) period.
+        senkou_slow_period: Senkoun (leading) slow period.
+        senkou_lookup_period: Senkoun (leading) fast period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
     def __init__(self,
                  kijun_period: int,
                  tenkan_period: int,
                  chikou_lag_period: int,
                  senkou_slow_period: int,
                  senkou_lookup_period: int,
```

### Comparing `talipp-2.1.1/talipp/indicators/Indicator.py` & `talipp-2.1.2/talipp/indicators/Indicator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from abc import ABCMeta, abstractmethod
 from collections.abc import MutableSequence, Sequence
 from typing import List, Any, Callable, Union, Type
 from warnings import warn
 
+from talipp.exceptions import TalippException
 from talipp.indicator_util import has_valid_values
 from talipp.input import SamplingPeriodType, Sampler
 
 ListAny = List[Any]
 ManagedSequenceType = Union['Indicator', MutableSequence]
 InputModifierType = Callable[..., Any]
 
 
 class Indicator(Sequence):
+    """Base indicator class.
+
+    Args:
+        input_modifier: Input modifier.
+        output_value_type: Output value type.
+        input_sampling: Input sampling type.
+    """
+
     __metaclass__ = ABCMeta
 
     def __init__(self,
                  input_modifier: InputModifierType = None,
                  output_value_type: Type = float,
                  input_sampling: SamplingPeriodType = None):
         self.input_modifier = input_modifier
@@ -47,36 +56,50 @@
         self.sub_indicators.append(indicator)
 
     def add_managed_sequence(self, lst: ManagedSequenceType) -> None:
         self.managed_sequences.append(lst)
 
     def initialize(self, input_values: ListAny = None, input_indicator: 'Indicator' = None) -> None:
         if input_values is not None and input_indicator is not None:
-            raise Exception('Indicator cannot be initialized with both input_values and input_indicator!')
+            raise TalippException('Indicator cannot be initialized with both input_values and input_indicator!')
 
         self.remove_all()
 
         if input_values is not None:
             for value in input_values:
                 self.add(value)
 
         if input_indicator is not None:
             for value in input_indicator:
                 self.add(value)
 
             input_indicator.add_output_listener(self)
 
     def add_input_value(self, value: Any) -> None:
+        """**Deprecated.** Use [add][talipp.indicators.Indicator.Indicator.add] method instead.
+
+        Add a new input value.
+
+        Args:
+            value: Value to be added.
+        """
+
         warn('This method is deprecated and will be removed in the next major version. '
              'Please use add(...) method with the same signature instead.',
              DeprecationWarning,
              stacklevel=2)
         return self.add(value)
 
     def add(self, value: Any) -> None:
+        """Add a new input value.
+
+        Args:
+            value: Value to be added.
+        """
+
         if (self.input_sampler is not None
                 and has_valid_values(self.input_values)
                 and self.input_sampler.is_same_period(value, self.input_values[-1])):
             self.update(value)
         else:
             for sub_indicator in self.sub_indicators:
                 sub_indicator.add(value)
@@ -99,32 +122,53 @@
 
                 self._add_to_output_values(new_value)
 
                 for listener in self.output_listeners:
                     listener.add(new_value)
 
     def update_input_value(self, value: Any) -> None:
+        """**Deprecated.** Use [update][talipp.indicators.Indicator.Indicator.update] method instead.
+
+        Update the last input value.
+
+        Args:
+            value: Value to be used.
+        """
+
         warn('This method is deprecated and will be removed in the next major version. '
              'Please use update(...) method with the same signature instead.',
              DeprecationWarning,
              stacklevel=2)
         return self.update(value)
 
     def update(self, value: Any) -> None:
+        """Update the last input value.
+
+        Args:
+            value: Value to be used.
+        """
+
         self.remove()
         self.add(value)
 
     def remove_input_value(self) -> None:
+        """**Deprecated.** Use [remove][talipp.indicators.Indicator.Indicator.remove] method instead.
+
+        Remove the last input value.
+        """
+
         warn('This method is deprecated and will be removed in the next major version. '
              'Please use remove(...) method with the same signature instead.',
              DeprecationWarning,
              stacklevel=2)
         return self.remove()
 
     def remove(self) -> None:
+        """Remove the last input value."""
+
         for sub_indicator in self.sub_indicators:
             sub_indicator.remove()
 
         if len(self.input_values) > 0:
             self.input_values.pop(-1)
 
         self._remove_output_value()
@@ -148,14 +192,16 @@
         if len(self.output_values) > 0:
             self.output_values.pop(-1)
 
     def _remove_custom(self) -> None:
         pass
 
     def remove_all(self) -> None:
+        """Remove all input values."""
+
         for sub_indicator in self.sub_indicators:
             sub_indicator.remove_all()
 
         self.input_values = []
         self.output_values = []
 
         for lst in self.managed_sequences:
@@ -169,14 +215,20 @@
         for listener in self.output_listeners:
             listener.remove_all()
 
     def _remove_all_custom(self) -> None:
         pass
 
     def purge_oldest(self, size: int) -> None:
+        """Purge old input values.
+
+        Args:
+            size: number of oldest input values to be purged.
+        """
+
         for sub_indicator in self.sub_indicators:
             sub_indicator.purge_oldest(size)
 
         if len(self.input_values) > 0:
             self.input_values = self.input_values[size:]
 
         self._purge_oldest_output_value(size)
```

### Comparing `talipp-2.1.1/talipp/indicators/KAMA.py` & `talipp-2.1.2/talipp/indicators/KAMA.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,28 @@
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class KAMA(Indicator):
-    """
-    Kaufman's Adaptive Moving Average
+    """Kaufman's Adaptive Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Volatility period.
+        fast_ema_constant_period: Fast [EMA][talipp.indicators.EMA] smoothing factor.
+        slow_ema_constant_period: Slow [EMA][talipp.indicators.EMA] smoothing factor.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  fast_ema_constant_period: int,
                  slow_ema_constant_period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/KVO.py` & `talipp-2.1.2/talipp/indicators/KVO.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV
 
 
 class KVO(Indicator):
-    """
-    Klinger Volume Oscillator
+    """Klinger Volume Oscillator.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_period: Fast moving average period.
+        slow_period: Slow moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_period: int,
                  slow_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/KeltnerChannels.py` & `talipp-2.1.2/talipp/indicators/KeltnerChannels.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,29 +7,44 @@
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV, ValueExtractor
 
 
 @dataclass
 class KeltnerChannelsVal:
-    # lower band
-    lb: float = None
+    """`KeltnerChannels` output type.
 
-    # central band
-    cb: float = None
+    Args:
+        lb: Lower band.
+        cb: Central band.
+        ub: Upper band.
+    """
 
-    # upper band
+    lb: float = None
+    cb: float = None
     ub: float = None
 
 
 class KeltnerChannels(Indicator):
-    """
-    Keltner Channels
+    """Keltner Channels.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [KeltnerChannelsVal][talipp.indicators.KeltnerChannels.KeltnerChannelsVal]
 
-    Output: a list of KeltnerChannelsVal
+    Args:
+        ma_period: Moving average period.
+        atr_period: [ATR][talipp.indicators.ATR] period.
+        atr_mult_up: Upper band multiplier.
+        atr_mult_down: Lower band multiplier.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, ma_period: int,
                  atr_period: int,
                  atr_mult_up: float,
                  atr_mult_down: float,
                  input_values: List[OHLCV] = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/MACD.py` & `talipp-2.1.2/talipp/indicators/MACD.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,43 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 
 
 @dataclass
 class MACDVal:
+    """`MACD` output type.
+
+    Args:
+        macd: `MACD` value.
+        signal: Signal line.
+        histogram: Histogram.
+    """
+
     macd: float = None
     signal: float = None
     histogram: float = None
 
 
 class MACD(Indicator):
-    """
-    Moving Average Convergence Divergence
+    """Moving Average Convergence Divergence.
+
+    Input type: `float`
+
+    Output type: [MACDVal][talipp.indicators.MACD.MACDVal]
 
-    Output: a list of MACDVal
+    Args:
+        fast_period: Fast moving average period.
+        slow_period: Slow moving average period.
+        signal_period: Signal line moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_period: int,
                  slow_period: int,
                  signal_period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/MassIndex.py` & `talipp-2.1.2/talipp/indicators/MassIndex.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,35 +4,46 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV
 
 
 class MassIndex(Indicator):
-    """
-    Mass Index
+    """Mass Index.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        ma_period: Moving average period.
+        ma_ma_period: Moving average period of moving average.
+        ma_ratio_period: Moving averages ration period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
-    def __init__(self, ema_period: int,
-                 ema_ema_period: int,
-                 ema_ratio_period: int,
+    def __init__(self, ma_period: int,
+                 ma_ma_period: int,
+                 ma_ratio_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  ma_type: MAType = MAType.EMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
-        self.ema_ratio_period = ema_ratio_period
+        self.ma_ratio_period = ma_ratio_period
 
-        self.ma = MAFactory.get_ma(ma_type, ema_period)
-        self.ma_ma = MAFactory.get_ma(ma_type, ema_ema_period)
+        self.ma = MAFactory.get_ma(ma_type, ma_period)
+        self.ma_ma = MAFactory.get_ma(ma_type, ma_ma_period)
         self.ma_ratio = []
 
         self.add_managed_sequence(self.ma)
         self.add_managed_sequence(self.ma_ma)
         self.add_managed_sequence(self.ma_ratio)
 
         self.initialize(input_values, input_indicator)
@@ -47,11 +58,11 @@
         self.ma_ma.add(self.ma[-1])
 
         if not has_valid_values(self.ma_ma, 1):
             return None
 
         self.ma_ratio.append(self.ma[-1] / float(self.ma_ma[-1]))
 
-        if not has_valid_values(self.ma_ratio, self.ema_ratio_period):
+        if not has_valid_values(self.ma_ratio, self.ma_ratio_period):
             return None
 
-        return sum(self.ma_ratio[-self.ema_ratio_period:])
+        return sum(self.ma_ratio[-self.ma_ratio_period:])
```

### Comparing `talipp-2.1.1/talipp/indicators/McGinleyDynamic.py` & `talipp-2.1.2/talipp/indicators/ROC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
-class McGinleyDynamic(Indicator):
-    """
-    McGinley Dynamic
+class ROC(Indicator):
+    """Rate Of Change.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Look-back period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
@@ -21,13 +29,11 @@
                          input_sampling=input_sampling)
 
         self.period = period
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, self.period):
+        if not has_valid_values(self.input_values, self.period+1):
             return None
-        elif has_valid_values(self.input_values, self.period, exact=True):
-            return sum(self.input_values) / float(self.period)
         else:
-            return self.output_values[-1] + (self.input_values[-1] - self.output_values[-1]) / float(self.period * pow(self.input_values[-1] / float(self.output_values[-1]), 4))
+            return 100.0 * (self.input_values[-1] - self.input_values[-self.period - 1]) / self.input_values[-self.period - 1]
```

### Comparing `talipp-2.1.1/talipp/indicators/MeanDev.py` & `talipp-2.1.2/talipp/indicators/WMA.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
-from talipp.ma import MAType, MAFactory
 
 
-class MeanDev(Indicator):
-    """
-    Mean Deviation
+class WMA(Indicator):
+    """Weighted Moving Average.
+
+    Input type: `float`
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
-                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
         self.period = period
 
-        self.ma = MAFactory.get_ma(ma_type, period)
-        self.add_sub_indicator(self.ma)
+        self.denom_sum = period * (period + 1) / 2.0
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.ma, 1):
+        if not has_valid_values(self.input_values, self.period):
             return None
 
-        return sum(map(lambda x: abs(x - self.ma[-1]), self.input_values[-self.period:])) / float(self.period)
+        s = 0.0
+        for i in range(self.period, 0, -1):
+            index = len(self.input_values) - self.period + i - 1  # decreases from end of array with increasing i
+            s += self.input_values[index] * i
+
+        return s / self.denom_sum
```

### Comparing `talipp-2.1.1/talipp/indicators/OBV.py` & `talipp-2.1.2/talipp/indicators/McGinleyDynamic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
-from talipp.ohlcv import OHLCV
 
 
-class OBV(Indicator):
-    """
-    On Balance Volume
+class McGinleyDynamic(Indicator):
+    """McGinley Dynamic.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
-    def __init__(self, input_values: List[OHLCV] = None,
+    def __init__(self, period: int,
+                 input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
+        self.period = period
+
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, 1):
+        if not has_valid_values(self.input_values, self.period):
             return None
-        elif has_valid_values(self.input_values, 1, exact=True):
-            return self.input_values[0].volume
+        elif has_valid_values(self.input_values, self.period, exact=True):
+            return sum(self.input_values) / float(self.period)
         else:
-            value = self.input_values[-1]
-            prev_value = self.input_values[-2]
-
-            if value.close == prev_value.close:
-                return self.output_values[-1]
-            elif value.close > prev_value.close:
-                return self.output_values[-1] + value.volume
-            else:
-                return self.output_values[-1] - value.volume
+            return self.output_values[-1] + (self.input_values[-1] - self.output_values[-1]) / float(self.period * pow(self.input_values[-1] / float(self.output_values[-1]), 4))
```

### Comparing `talipp-2.1.1/talipp/indicators/ParabolicSAR.py` & `talipp-2.1.2/talipp/indicators/ParabolicSAR.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,31 +5,55 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class SARTrend(enum.Enum):
+    """`ParabolicSAR` trend."""
+
     UP = enum.auto()
+    """Up trend."""
+
     DOWN = enum.auto()
+    """Down trend."""
 
 
 @dataclass
 class ParabolicSARVal:
+    """`ParabolicSAR` output type.
+
+    Args:
+        value: `SAR` value.
+        trend: Actual trend.
+        ep: Extreme point.
+        accel_factor: Acceleration factor.
+    """
+
     value: float = None
     trend: SARTrend = None
     ep: float = None
     accel_factor: float = None
 
 
 class ParabolicSAR(Indicator):
-    """
-    Parabolic Stop And Reverse
+    """Parabolic Stop And Reverse.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [ParabolicSARVal][talipp.indicators.ParabolicSAR.ParabolicSARVal]
 
-    Output: a list of ParabolicSARVal
+    Args:
+        init_accel_factor: Initial acceleration factor.
+        accel_factor_inc: Acceleration factor increment.
+        max_accel_factor: Maximum acceleration factor.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     SAR_INIT_LEN = 5
 
     def __init__(self, init_accel_factor: float,
                  accel_factor_inc: float,
                  max_accel_factor: float,
```

### Comparing `talipp-2.1.1/talipp/indicators/ROC.py` & `talipp-2.1.2/talipp/indicators/StdDev.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,28 @@
+from math import sqrt
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
-class ROC(Indicator):
-    """
-    Rate Of Change
+class StdDev(Indicator):
+    """Standard Deviation.
+
+    Input type: `float`
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
@@ -21,11 +30,12 @@
                          input_sampling=input_sampling)
 
         self.period = period
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, self.period+1):
+        if not has_valid_values(self.input_values, self.period):
             return None
-        else:
-            return 100.0 * (self.input_values[-1] - self.input_values[-self.period - 1]) / self.input_values[-self.period - 1]
+
+        mean = sum(self.input_values[-self.period:]) / self.period
+        return sqrt(sum([(item - mean)**2 for item in self.input_values[-self.period:]]) / self.period)
```

### Comparing `talipp-2.1.1/talipp/indicators/RSI.py` & `talipp-2.1.2/talipp/indicators/RSI.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class RSI(Indicator):
-    """
-    Relative Strength Index
+    """Relative Strength Index.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
```

### Comparing `talipp-2.1.1/talipp/indicators/SFX.py` & `talipp-2.1.2/talipp/indicators/VTX.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,76 @@
 from dataclasses import dataclass
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.ATR import ATR
 from talipp.indicators.Indicator import Indicator, InputModifierType
-from talipp.indicators.StdDev import StdDev
 from talipp.input import SamplingPeriodType
-from talipp.ma import MAType, MAFactory
-from talipp.ohlcv import OHLCV, ValueExtractor
+from talipp.ohlcv import OHLCV
 
 
 @dataclass
-class SFXVal:
-    atr: float = None
-    std_dev: float = None
-    ma_std_dev: float = None
+class VTXVal:
+    """`VTX` output type.
 
-
-class SFX(Indicator):
+    Args:
+        plus_vtx: Positive movement.
+        minus_vtx: Negative movement.
     """
-    Output: A list of SFXVal
+
+    plus_vtx: float = None
+    minus_vtx: float = None
+
+
+class VTX(Indicator):
+    """Vortex Indicator.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [VTXVal][talipp.indicators.VTX.VTXVal]
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
-    def __init__(self, atr_period: int,
-                 std_dev_period: int,
-                 std_dev_smoothing_period: int,
+    def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
-                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
-                         output_value_type=SFXVal,
+                         output_value_type=VTXVal,
                          input_sampling=input_sampling)
 
-        self.atr = ATR(atr_period)
-        self.std_dev = StdDev(std_dev_period, input_modifier=ValueExtractor.extract_close)
-        self.ma_std_dev = MAFactory.get_ma(ma_type, std_dev_smoothing_period, input_indicator=self.std_dev)
+        self.period = period
+
+        self.plus_vm = []
+        self.add_managed_sequence(self.plus_vm)
+
+        self.minus_vm = []
+        self.add_managed_sequence(self.minus_vm)
 
+        self.atr = ATR(1)
         self.add_sub_indicator(self.atr)
-        self.add_sub_indicator(self.std_dev)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if has_valid_values(self.atr, 1):
-            atr = self.atr[-1]
-        else:
-            atr = None
-
-        if has_valid_values(self.std_dev, 1):
-            std_dev = self.std_dev[-1]
-        else:
-            std_dev = None
-
-        if has_valid_values(self.ma_std_dev, 1):
-            ma_std_dev = self.ma_std_dev[-1]
-        else:
-            ma_std_dev = None
+        if not has_valid_values(self.input_values, 2):
+            return None
+
+        value = self.input_values[-1]
+        value2 = self.input_values[-2]
+
+        self.plus_vm.append(abs(value.high - value2.low))
+        self.minus_vm.append(abs(value.low - value2.high))
+
+        if not has_valid_values(self.atr, self.period) or not has_valid_values(self.plus_vm, self.period) or \
+                not has_valid_values(self.minus_vm, self.period):
+            return None
 
-        return SFXVal(atr, std_dev, ma_std_dev)
+        atr_sum = float(sum(self.atr[-self.period:]))
+        return VTXVal(sum(self.plus_vm[-self.period:]) / atr_sum, sum(self.minus_vm[-self.period:]) / atr_sum)
```

### Comparing `talipp-2.1.1/talipp/indicators/SMA.py` & `talipp-2.1.2/talipp/indicators/SMA.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class SMA(Indicator):
-    """
-    Simple Moving Average
+    """Simple Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
```

### Comparing `talipp-2.1.1/talipp/indicators/SMMA.py` & `talipp-2.1.2/talipp/indicators/MeanDev.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
+from talipp.ma import MAType, MAFactory
 
 
-class SMMA(Indicator):
-    """
-    Smoothed Moving Average
+class MeanDev(Indicator):
+    """Mean Deviation.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
+
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
+                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
         self.period = period
 
+        self.ma = MAFactory.get_ma(ma_type, period)
+        self.add_sub_indicator(self.ma)
+
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, self.period):
+        if not has_valid_values(self.ma, 1):
             return None
-        elif has_valid_values(self.input_values, self.period, exact=True):
-            return float(sum(self.input_values)) / self.period
-        else:
-            return (self.output_values[-1] * (self.period - 1) + self.input_values[-1]) / self.period
+
+        return sum(map(lambda x: abs(x - self.ma[-1]), self.input_values[-self.period:])) / float(self.period)
```

### Comparing `talipp-2.1.1/talipp/indicators/SOBV.py` & `talipp-2.1.2/talipp/indicators/SOBV.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,26 @@
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.indicators.OBV import OBV
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class SOBV(Indicator):
-    """
-    Smoothed On Balance Volume
+    """Smoothed On Balance Volume.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
```

### Comparing `talipp-2.1.1/talipp/indicators/STC.py` & `talipp-2.1.2/talipp/indicators/STC.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,30 @@
 from talipp.indicators.Stoch import Stoch, StochVal
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType
 from talipp.ohlcv import OHLCV
 
 
 class STC(Indicator):
-    """
-    Schaff Trend Cycle
+    """Schaff Trend Cycle.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_macd_period: Fast [MACD][talipp.indicators.MACD] period.
+        slow_macd_period: Slow [MACD][talipp.indicators.MACD] period.
+        stoch_period: [Stoch][talipp.indicators.Stoch] period.
+        stoch_smoothing_period: [Stoch][talipp.indicators.Stoch] smooting period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        stoch_ma_type: [Stoch][talipp.indicators.Stoch] moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_macd_period: int,
                  slow_macd_period: int,
                  stoch_period: int,
                  stoch_smoothing_period:int,
                  input_values: List[float] = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/StdDev.py` & `talipp-2.1.2/talipp/indicators/SMMA.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-from math import sqrt
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
-class StdDev(Indicator):
-    """
-    Standard Deviation
+class SMMA(Indicator):
+    """Smoothed Moving Average
 
-    Output: a list of floats
-    """
+    Input type: `float`
+
+    Output type: `float`
 
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
+    """
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
@@ -24,10 +30,11 @@
         self.period = period
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
         if not has_valid_values(self.input_values, self.period):
             return None
-
-        mean = sum(self.input_values[-self.period:]) / self.period
-        return sqrt(sum([(item - mean)**2 for item in self.input_values[-self.period:]]) / self.period)
+        elif has_valid_values(self.input_values, self.period, exact=True):
+            return float(sum(self.input_values)) / self.period
+        else:
+            return (self.output_values[-1] * (self.period - 1) + self.input_values[-1]) / self.period
```

### Comparing `talipp-2.1.1/talipp/indicators/Stoch.py` & `talipp-2.1.2/talipp/indicators/Stoch.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,40 @@
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAFactory, MAType
 from talipp.ohlcv import OHLCV
 
 
 @dataclass
 class StochVal:
+    """`Stoch` output type.
+
+    Args:
+        k: `k` value.
+        d: `d` value.
+    """
+
     k: float = None
     d: float = None
 
 
 class Stoch(Indicator):
-    """
-    Stochastic
+    """Stochastic.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [StochVal][talipp.indicators.Stoch.StochVal]
 
-    Output: a list of StochVal
+    Args:
+        period: Period.
+        smoothing_period: Moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  smoothing_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/StochRSI.py` & `talipp-2.1.2/talipp/indicators/StochRSI.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,42 @@
 from talipp.indicators.RSI import RSI
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 
 
 @dataclass
 class StochRSIVal:
+    """`StochRSI` output type.
+
+    Args:
+        k: `k` value.
+        d: `d` value.
+    """
+
     k: float = None
     d: float = None
 
 
 class StochRSI(Indicator):
-    """
-    Stochastic RSI
+    """Stochastic RSI.
+
+    Input type: `float`
+
+    Output type: [StochRSIVal][talipp.indicators.StochRSI.StochRSIVal]
 
-    Output: a list of StochRSIVal
+    Args:
+        rsi_period: [RSI][talipp.indicators.RSI] period.
+        stoch_period: [Stoch][talipp.indicators.Stoch] period.
+        k_smoothing_period: Stoch's `k` moving average period.
+        d_smoothing_period: Stoch's `d` moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, rsi_period: int,
                  stoch_period: int,
                  k_smoothing_period: int,
                  d_smoothing_period: int,
                  input_values: List[float] = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/SuperTrend.py` & `talipp-2.1.2/talipp/indicators/SuperTrend.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,49 @@
 from talipp.indicators.ATR import ATR
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class Trend(enum.Enum):
+    """`SuperTrend` trend."""
+
     UP = enum.auto()
+    """Up trend."""
+
     DOWN = enum.auto()
+    """Down trend."""
 
 
 @dataclass
 class SuperTrendVal:
+    """`SuperTrend` output type.
+
+    Args:
+        value: `SuperTrend` value.
+        trend: `SuperTrend` trend.
+    """
     value: float = None
     trend: Trend = None
 
 
 class SuperTrend(Indicator):
-    """
-    Output: A list of SuperTrendVal
+    """SuperTrend.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [SuperTrendVal][talipp.indicators.SuperTrend.SuperTrendVal]
+
+    Args:
+        atr_period: [ATR][talipp.indicators.ATR] period.
+        mult: ATR multiplier.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, atr_period: int,
                  mult: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/T3.py` & `talipp-2.1.2/talipp/indicators/T3.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,27 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.EMA import EMA
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class T3(Indicator):
-    """
-    T3 Moving Average
+    """T3 Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        factor: Multiplicative factor.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  factor: float = 0.7,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/TEMA.py` & `talipp-2.1.2/talipp/indicators/TEMA.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.EMA import EMA
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 
 
 class TEMA(Indicator):
-    """
-    Triple Exponential Moving Average
+    """Triple Exponential Moving Average.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
```

### Comparing `talipp-2.1.1/talipp/indicators/TRIX.py` & `talipp-2.1.2/talipp/indicators/OBV.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
-from talipp.indicators.EMA import EMA
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
+from talipp.ohlcv import OHLCV
 
 
-class TRIX(Indicator):
-    """
-    TRIX
+class OBV(Indicator):
+    """On Balance Volume.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
-    def __init__(self, period: int,
-                 input_values: List[float] = None,
+    def __init__(self, input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
-        self.period = period
-
-        self.ema1 = EMA(period)
-        self.ema2 = EMA(period, input_indicator = self.ema1)
-        self.ema3 = EMA(period, input_indicator = self.ema2)
-
-        self.add_sub_indicator(self.ema1)
-
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.ema3, 2):
+        if not has_valid_values(self.input_values, 1):
             return None
-
-        return 10000.0 * (self.ema3[-1] - self.ema3[-2]) / self.ema3[-2]
+        elif has_valid_values(self.input_values, 1, exact=True):
+            return self.input_values[0].volume
+        else:
+            value = self.input_values[-1]
+            prev_value = self.input_values[-2]
+
+            if value.close == prev_value.close:
+                return self.output_values[-1]
+            elif value.close > prev_value.close:
+                return self.output_values[-1] + value.volume
+            else:
+                return self.output_values[-1] - value.volume
```

### Comparing `talipp-2.1.1/talipp/indicators/TSI.py` & `talipp-2.1.2/talipp/indicators/TSI.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,28 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 
 
 class TSI(Indicator):
-    """
-    True Strength Index
+    """True Strength Index.
+
+    Input type: `float`
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_period: Fast moving average period.
+        slow_period: Slow moving average period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_period: int,
                  slow_period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/TTM.py` & `talipp-2.1.2/talipp/indicators/TTM.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,41 @@
 from talipp.input import SamplingPeriodType
 from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV, ValueExtractor
 
 
 @dataclass
 class TTMVal:
-    # squeeze is on (=True) or off (=False+
-    squeeze: bool = None
+    """`TTM` output type.
+
+    Args:
+        squeeze: `True` if squeeze is on, otherwise `False`.
+        histogram: Histogram of the linear regression.
+    """
 
-    # histogram of the linear regression
+    squeeze: bool = None
     histogram: float = None
 
 
 class TTM(Indicator):
-    """
-    TTM Squeeze
+    """TTM Squeeze.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: [TTMVal][talipp.indicators.TTM.TTMVal]
 
-    Output: a list of TTMVal
+    Args:
+        period: Period.
+        bb_std_dev_mult: [BB][talipp.indicators.BB] standard deviation multiplier.
+        kc_atr_mult: [KeltnerChannels][talipp.indicators.KeltnerChannels] [ATR][talipp.indicators.ATR] multiplier.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  bb_std_dev_mult: float = 2,
                  kc_atr_mult: float = 1.5,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/UO.py` & `talipp-2.1.2/talipp/indicators/UO.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,28 @@
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class UO(Indicator):
-    """
-    Ultimate Oscillator
+    """Ultimate Oscillator.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        fast_period: Fast period.
+        mid_period: Mid period.
+        slow_period: Slow period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, fast_period: int,
                  mid_period: int,
                  slow_period: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
```

### Comparing `talipp-2.1.1/talipp/indicators/VTX.py` & `talipp-2.1.2/talipp/indicators/EMV.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-from dataclasses import dataclass
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
-from talipp.indicators.ATR import ATR
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
+from talipp.ma import MAType, MAFactory
 from talipp.ohlcv import OHLCV
 
 
-@dataclass
-class VTXVal:
-    plus_vtx: float = None
-    minus_vtx: float = None
+class EMV(Indicator):
+    """Ease of Movement.
 
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
 
-class VTX(Indicator):
-    """
-    Vortex Indicator
+    Output type: `float`
 
-    Output: a list of floats
+    Args:
+        period: Period.
+        volume_div: Volume divider.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
+                 volume_div: int,
                  input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
+                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
-                         output_value_type=VTXVal,
                          input_sampling=input_sampling)
 
         self.period = period
+        self.volume_div = volume_div
 
-        self.plus_vm = []
-        self.add_managed_sequence(self.plus_vm)
-
-        self.minus_vm = []
-        self.add_managed_sequence(self.minus_vm)
-
-        self.atr = ATR(1)
-        self.add_sub_indicator(self.atr)
+        self.emv_sma = MAFactory.get_ma(ma_type, period)
+        self.add_managed_sequence(self.emv_sma)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
         if not has_valid_values(self.input_values, 2):
             return None
 
         value = self.input_values[-1]
         value2 = self.input_values[-2]
+        if value.high != value.low:
+            distance = (value.high + value.low) / 2.0 - (value2.high + value2.low) / 2.0
+            box_ratio = (value.volume / float(self.volume_div)) / (value.high - value.low)
+            emv = distance / box_ratio
+        else:
+            emv = 0.0
 
-        self.plus_vm.append(abs(value.high - value2.low))
-        self.minus_vm.append(abs(value.low - value2.high))
+        self.emv_sma.add(emv)
 
-        if not has_valid_values(self.atr, self.period) or not has_valid_values(self.plus_vm, self.period) or \
-                not has_valid_values(self.minus_vm, self.period):
+        if not has_valid_values(self.emv_sma, 1):
             return None
-
-        atr_sum = float(sum(self.atr[-self.period:]))
-        return VTXVal(sum(self.plus_vm[-self.period:]) / atr_sum, sum(self.minus_vm[-self.period:]) / atr_sum)
+        else:
+            return self.emv_sma[-1]
```

### Comparing `talipp-2.1.1/talipp/indicators/VWAP.py` & `talipp-2.1.2/talipp/indicators/VWAP.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,25 @@
 
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class VWAP(Indicator):
-    """
-    Volume Weighted Average Price
-    Output: a list of floats
+    """Volume Weighted Average Price.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
+
+    Output type: `float`
+
+    Args:
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
```

### Comparing `talipp-2.1.1/talipp/indicators/WMA.py` & `talipp-2.1.2/talipp/indicators/DPO.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
+from talipp.ma import MAType, MAFactory
 
 
-class WMA(Indicator):
-    """
-    Weighted Moving Average
+class DPO(Indicator):
+    """Detrended Price Oscillator.
+
+    Input type: float
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        ma_type: Moving average type.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
                  input_values: List[float] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
+                 ma_type: MAType = MAType.SMA,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
         self.period = period
 
-        self.denom_sum = period * (period + 1) / 2.0
+        self.ma = MAFactory.get_ma(ma_type, period)
+        self.add_sub_indicator(self.ma)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, self.period):
+        if not has_valid_values(self.input_values, int(self.period / 2) + 2) or not has_valid_values(self.ma, 1):
             return None
 
-        s = 0.0
-        for i in range(self.period, 0, -1):
-            index = len(self.input_values) - self.period + i - 1  # decreases from end of array with increasing i
-            s += self.input_values[index] * i
-
-        return s / self.denom_sum
+        return self.input_values[-(int(self.period / 2) + 1) - 1] - float(self.ma[-1])
```

### Comparing `talipp-2.1.1/talipp/indicators/ZLEMA.py` & `talipp-2.1.2/talipp/indicators/CHOP.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,51 @@
+from math import log10
 from typing import List, Any
 
 from talipp.indicator_util import has_valid_values
-from talipp.indicators.EMA import EMA
+from talipp.indicators.ATR import ATR
 from talipp.indicators.Indicator import Indicator, InputModifierType
 from talipp.input import SamplingPeriodType
+from talipp.ohlcv import OHLCV
 
 
-class ZLEMA(Indicator):
-    """
-    Zero Lag Exponential Moving Average
+class CHOP(Indicator):
+    """Choppiness Index.
+
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
 
-    Output: a list of floats
+    Output type: `float`
+
+    Args:
+        period: Period.
+        input_values: List of input values.
+        input_indicator: Input indicator.
+        input_modifier: Input modifier.
+        input_sampling: Input sampling type.
     """
 
     def __init__(self, period: int,
-                 input_values: List[float] = None,
+                 input_values: List[OHLCV] = None,
                  input_indicator: Indicator = None,
                  input_modifier: InputModifierType = None,
                  input_sampling: SamplingPeriodType = None):
         super().__init__(input_modifier=input_modifier,
                          input_sampling=input_sampling)
 
-        self.lag = round((period - 1) / 2.0)
+        self.period = period
 
-        self.ema = EMA(period)
-        self.add_managed_sequence(self.ema)
+        self.atr = ATR(1)
+        self.add_sub_indicator(self.atr)
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
-        if not has_valid_values(self.input_values, self.lag+1):
+        if not has_valid_values(self.atr, self.period) or not has_valid_values(self.input_values, self.period):
             return None
 
-        self.ema.add(self.input_values[-1] + (self.input_values[-1] - self.input_values[-self.lag-1]))
+        max_high = max(self.input_values[-self.period:], key = lambda x: x.high).high
+        min_low = min(self.input_values[-self.period:], key = lambda x: x.low).low
 
-        if not has_valid_values(self.ema):
+        if max_high != min_low:
+            return 100.0 * log10(sum(self.atr[-self.period:]) / (max_high - min_low) ) / log10(self.period)
+        else:
             return None
-
-        return self.ema[-1]
```

### Comparing `talipp-2.1.1/talipp/indicators/__init__.py` & `talipp-2.1.2/talipp/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `talipp-2.1.1/talipp/ohlcv.py` & `talipp-2.1.2/talipp/ohlcv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,81 @@
+"""Collection of classes related to `OHLCV` input type."""
+
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import zip_longest
 from typing import List, Dict, Optional
 
 
 @dataclass
 class OHLCV:
+    """`OHLCV` input representation.
+
+    Attributes:
+        open: Open price.
+        high: High price.
+        low: Low price.
+        close: Close price.
+        volume: Volume.
+        time: Timestamp.
+    """
+
     open: Optional[float]
     high: Optional[float]
     low: Optional[float]
     close: Optional[float]
     volume: Optional[float] = None
     time: Optional[datetime] = None
 
 
 class OHLCVFactory:
+    """Static class serving to create `OHLCV` input objects from various representations."""
+
     @staticmethod
     def from_matrix(values: List[List[float]]) -> List[OHLCV]:
-        """
-        Converts lists representing OHLCV values into lists of OHLCV objects. Expected dimension of input OHLCV list
+        """Converts lists/tuples representing OHLCV values into a list of `OHLCV` objects.
+
+        Expected dimension of input OHLCV list
         is 4 (without volume and timestamp), 5 (with volume and without timestamp) or 6 (with volume and timestamp).
 
-        Unlike from_matrix2 in this method each input sublist represents an OHLCV tuple.
+        Examples:
+
+            [[1,2,3,4,5], [6,7,8,9,0]] -> [OHLCV(1,2,3,4,5), OHLCV(6,7,8,9,0)]
+            [[1,2,3,4], [6,7,8,9]] -> [OHLCV(1,2,3,4), OHLCV(6,7,8,9)]
+            [[1,2,3,4,5,6], [7,8,9,10,11,12]] -> [OHLCV(1,2,3,4,5,6), OHLCV(7,8,9,10,11,12)]
+
+        Args:
+            values: A list of values to be converted into `OHLCV` objects.
 
-        Example: [[1,2,3,4,5], [6,7,8,9,0]] -> [OHLCV(1,2,3,4,5), OHLCV(6,7,8,9,0)]
-        Example: [[1,2,3,4], [6,7,8,9]] -> [OHLCV(1,2,3,4), OHLCV(6,7,8,9)]
-        Example: [[1,2,3,4,5,6], [7,8,9,10,11,12]] -> [OHLCV(1,2,3,4,5,6), OHLCV(7,8,9,10,11,12)]
+        Returns:
+            A list of `OHLCV` objects.
         """
+
         return [OHLCV(x[0],
                       x[1],
                       x[2],
                       x[3],
                       x[4] if len(x) >= 5 else None,
                       x[5] if len(x) >= 6 else None) for x in values]
 
     @staticmethod
     def from_matrix2(values: List[List[float]]) -> List[OHLCV]:
-        """
-        Converts lists representing O, H, L, C, V and T(ime) values into lists of OHLCV objects.
+        """Converts lists representing O, H, L, C, V and T values into a list of `OHLCV` objects.
 
-        Unlike from_matrix in this method each input sublist represents all opens, highs, ...
+        Examples:
 
-        Example: [[1,2], [3,4], [5,6], [7,8]] -> [OHLCV(1,3,5,7), OHLCV(2,4,6,8)]
-        Example: [[1,2], [3,4], [5,6], [7,8], [9,0]] -> [OHLCV(1,3,5,7,9), OHLCV(2,4,6,8,0)]
-        Example: [[1,2], [3,4], [5,6], [7,8], [9,0], [11, 12]] -> [OHLCV(1,3,5,7,9,11), OHLCV(2,4,6,8,0,12)]
+            [[1,2], [3,4], [5,6], [7,8]] -> [OHLCV(1,3,5,7), OHLCV(2,4,6,8)]
+            [[1,2], [3,4], [5,6], [7,8], [9,0]] -> [OHLCV(1,3,5,7,9), OHLCV(2,4,6,8,0)]
+            [[1,2], [3,4], [5,6], [7,8], [9,0], [11, 12]] -> [OHLCV(1,3,5,7,9,11), OHLCV(2,4,6,8,0,12)]
+
+        Args:
+            values: A list of values to be converted into `OHLCV` objects.
+
+        Returns:
+            A list of `OHLCV` objects.
         """
 
         if len(values) == 4:
             return OHLCVFactory.from_matrix(list(map(list, zip_longest(values[0],
                                                                        values[1],
                                                                        values[2],
                                                                        values[3]))))
@@ -63,44 +91,104 @@
                                                                        values[2],
                                                                        values[3],
                                                                        values[4],
                                                                        values[5]))))
 
     @staticmethod
     def from_dict(values: Dict[str, List[float]]) -> List[OHLCV]:
-        """
-        Converts a dict with keys 'open', 'high', 'low', 'close', 'volume' and 'time' where each key
-        contains a list of simple values into a list of OHLCV objects. If some key is missing, corresponding values
-        in OHLCV will be None
+        """Converts a dict with OHLCV values into a list of `OHLCV` objects.
+
+        The dict consists of `open`, `high`, `low`, `close`, `volume` and `time` keys where each key
+        contains a list of simple values. If some key is missing, corresponding values
+        in OHLCV will be None.
+
+        Examples:
 
-        Example: {'open': [1,2], 'close': [3,4]} -> [OHLCV(1, None, None, 3, None, None), OHLCV(2, None, None, 4, None, None)]
+            {'open': [1,2], 'close': [3,4]} -> [OHLCV(1, None, None, 3, None, None), OHLCV(2, None, None, 4, None, None)]
+
+        Args:
+            values: A dict of values to be converted into `OHLCV` objects.
+
+        Returns:
+            A list of `OHLCV` objects.
         """
+
         return OHLCVFactory.from_matrix2([
             values['open'] if 'open' in values else [],
             values['high'] if 'high' in values else [],
             values['low'] if 'low' in values else [],
             values['close'] if 'close' in values else [],
             values['volume'] if 'volume' in values else [],
             values['time'] if 'time' in values else []
         ])
 
 
 class ValueExtractor:
+    """A set of static methods extracting attributes from `OHLCV` objects.
+
+    The methods primarily serve as input modifiers in indicators.
+    """
+
     @staticmethod
     def extract_open(value: OHLCV) -> float:
+        """Extract open price.
+
+        Args:
+            value: `OHLCV` value
+
+        Returns:
+            Open price.
+        """
+
         return value.open
 
     @staticmethod
     def extract_high(value: OHLCV) -> float:
+        """Extract high price.
+
+        Args:
+            value: `OHLCV` value
+
+        Returns:
+            High price.
+        """
+
         return value.high
 
     @staticmethod
     def extract_low(value: OHLCV) -> float:
+        """Extract low price.
+
+        Args:
+            value: `OHLCV` value
+
+        Returns:
+            Low price.
+        """
+
         return value.low
 
     @staticmethod
     def extract_close(value: OHLCV) -> float:
+        """Extract close price.
+
+        Args:
+            value: `OHLCV` value
+
+        Returns:
+            Close price.
+        """
+
         return value.close
 
     @staticmethod
     def extract_volume(value: OHLCV) -> float:
+        """Extract volume.
+
+        Args:
+            value: `OHLCV` value
+
+        Returns:
+            Volume.
+        """
+
         return value.volume
```

### Comparing `talipp-2.1.1/talipp.egg-info/PKG-INFO` & `talipp-2.1.2/talipp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: talipp
-Version: 2.1.1
-Summary: TALi++ - Incremental Technical Analysis Library
+Version: 2.1.2
+Summary: talipp - Incremental Technical Analysis Library
 Home-page: https://github.com/nardew/talipp
 Author: nardew
 Author-email: talipp.pyth@gmail.com
 License: UNKNOWN
-Description: # TALIpp - Incremental Technical Analysis Library
+Description: # talipp - Incremental Technical Analysis Library
         
         ![](https://img.shields.io/badge/python-3.8-blue.svg) 
         ![](https://img.shields.io/badge/python-3.9-blue.svg)
         ![](https://img.shields.io/badge/python-3.10-blue.svg)
         ![](https://img.shields.io/badge/python-3.11-blue.svg)
         ![PyPy](https://img.shields.io/badge/pypy-3-blue.svg)
         ![unit tests](https://github.com/nardew/talipp/workflows/unit%20tests/badge.svg)
         
         ---
         
-        ## New major release `talipp 2.0.0` available!
-        
-        - Scope: https://github.com/nardew/talipp/issues/111
-        - PR: https://github.com/nardew/talipp/pull/96
+        ## !!! [New documentation page available](https://nardew.github.io/talipp) !!!
         
         ---
         
         `talipp` (or `tali++`) is a Python library implementing financial indicators for technical analysis. The distinctive feature of the library is its incremental computation which fits extremely well real-time applications or applications with iterative input in general.  
         
         Unlike existing libraries for technical analysis which typically have to work on the whole input vector in order to calculate new values of indicators, `talipp` due to its incremental architecture calculates new indicators' values exclusively based on the delta input data. That implies, among others, it requires `O(1)` time to produce new values in comparison to `O(n)` required by other libraries.
```

