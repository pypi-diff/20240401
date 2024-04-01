# Comparing `tmp/py3gpp-0.4.0.tar.gz` & `tmp/py3gpp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3gpp-0.4.0.tar", last modified: Fri Mar 15 13:15:23 2024, max compression
+gzip compressed data, was "py3gpp-0.5.0.tar", last modified: Mon Apr  1 18:43:16 2024, max compression
```

## Comparing `py3gpp-0.4.0.tar` & `py3gpp-0.5.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:23.385707 py3gpp-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-15 13:15:10.000000 py3gpp-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-15 13:15:23.385707 py3gpp-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-15 13:15:10.000000 py3gpp-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:23.377707 py3gpp-0.4.0/py3gpp/
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:23.377707 py3gpp-0.4.0/py3gpp/codes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/codes/bg1.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/codes/bg2.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:23.381707 py3gpp-0.4.0/py3gpp/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/CommonConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/DMRSConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/PDSCHConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/PDSCHPTRSConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/nrCarrierConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/nrNumerologyConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/nrPDSCHConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/nrPDSCHDMRSConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/nrPDSCHPTRSConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/configs/nrPathLossConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrChannelEstimate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrCodeBlockDesegmentLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrCodeBlockSegmentLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrDLSCHInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrEqualizeMMSE.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrExtractResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrLDPCDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrLDPCEncode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrLayerMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrOFDMDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrOFDMInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrOFDMModulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPBCH.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPBCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPBCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPBCHIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPBCHPRBS.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCH.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCHIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCHPTRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPDSCHPTRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPRBS.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPSS.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPathLoss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPolarDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrPolarEncode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrRateMatchLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrRateMatchPolar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrRateRecoverLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrRateRecoverPolar.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrResourceGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrSSS.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrSSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrSetResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrSymbolDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrSymbolModulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrTBS.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-15 13:15:11.000000 py3gpp-0.4.0/py3gpp/nrTimingEstimate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:23.385707 py3gpp-0.4.0/py3gpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-15 13:15:23.000000 py3gpp-0.4.0/py3gpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-15 13:15:23.000000 py3gpp-0.4.0/py3gpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 13:15:23.000000 py3gpp-0.4.0/py3gpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 13:15:23.000000 py3gpp-0.4.0/py3gpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 13:15:23.000000 py3gpp-0.4.0/py3gpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-15 13:15:11.000000 py3gpp-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 13:15:23.385707 py3gpp-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-15 13:15:11.000000 py3gpp-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:15:23.385707 py3gpp-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrCodeBlockDesegmentLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrCodeBlockSegmentLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrDLSCHInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrLDPCEncode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrLayerMap.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPDSCH.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPDSCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPDSCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPDSCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPDSCHPTRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPDSCHPTRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPathLoss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPolarDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPolarEncode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrPolarEncode_nrPolarDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrRateMatchLDPC_nrRateRecoverLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrRateMatchPolar.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrRateRecoverLDPC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrRateRecoverPolar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_nrTBS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-15 13:15:11.000000 py3gpp-0.4.0/tests/test_phase_compensation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:16.657194 py3gpp-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-01 18:43:01.000000 py3gpp-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-01 18:43:16.657194 py3gpp-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-01 18:43:01.000000 py3gpp-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:16.653194 py3gpp-0.5.0/py3gpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:16.653194 py3gpp-0.5.0/py3gpp/codes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/codes/bg1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/codes/bg2.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:16.653194 py3gpp-0.5.0/py3gpp/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/CommonConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/DMRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/PDSCHConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/PDSCHPTRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/nrCarrierConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/nrNumerologyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/nrPDSCHConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/nrPDSCHDMRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/nrPDSCHPTRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/configs/nrPathLossConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrBCH.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrChannelEstimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrCodeBlockDesegmentLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrCodeBlockSegmentLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrDLSCHInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrEqualizeMMSE.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrExtractResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrLDPCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrLDPCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrLayerMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrOFDMDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrOFDMInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrOFDMModulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPBCH.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPBCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPBCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPBCHIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPBCHPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCH.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCHIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPSS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPathLoss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPolarDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrPolarEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrRateMatchLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrRateMatchPolar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrRateRecoverLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrRateRecoverPolar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrResourceGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrSSS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrSSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrSetResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrSymbolDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrSymbolModulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrTBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-01 18:43:01.000000 py3gpp-0.5.0/py3gpp/nrTimingEstimate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:16.657194 py3gpp-0.5.0/py3gpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-01 18:43:16.000000 py3gpp-0.5.0/py3gpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-01 18:43:16.000000 py3gpp-0.5.0/py3gpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:43:16.000000 py3gpp-0.5.0/py3gpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 18:43:16.000000 py3gpp-0.5.0/py3gpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 18:43:16.000000 py3gpp-0.5.0/py3gpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-01 18:43:01.000000 py3gpp-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:43:16.657194 py3gpp-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 18:43:01.000000 py3gpp-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:43:16.657194 py3gpp-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrBCH.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrCodeBlockDesegmentLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrCodeBlockSegmentLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrDLSCHInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrLDPCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrLayerMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPDSCH.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPDSCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPathLoss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPolarDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPolarEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrPolarEncode_nrPolarDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrRateMatchLDPC_nrRateRecoverLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrRateMatchPolar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrRateRecoverLDPC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrRateRecoverPolar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_nrTBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-01 18:43:01.000000 py3gpp-0.5.0/tests/test_phase_compensation.py
```

### Comparing `py3gpp-0.4.0/LICENSE` & `py3gpp-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/PKG-INFO` & `py3gpp-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.4.0
+Version: 0.5.0
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.4.0/README.md` & `py3gpp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/__init__.py` & `py3gpp-0.5.0/py3gpp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .nrRateRecoverPolar import nrRateRecoverPolar
 from .nrRateMatchPolar import nrRateMatchPolar
 from .nrPolarDecode import nrPolarDecode
 from .nrPolarEncode import nrPolarEncode
 from .nrCRCEncode import nrCRCEncode
 from .nrCRCDecode import nrCRCDecode
 from .nrBCHDecode import nrBCHDecode
+from .nrBCH import nrBCH
 from .nrPRBS import nrPRBS
 from .nrSymbolModulate import nrSymbolModulate
 from .nrRateMatchLDPC import nrRateMatchLDPC
 from .nrRateRecoverLDPC import nrRateRecoverLDPC
 from .nrLDPCEncode import nrLDPCEncode
 from .nrLDPCDecode import nrLDPCDecode
 from .nrTBS import nrTBS
```

### Comparing `py3gpp-0.4.0/py3gpp/codes/bg1.csv` & `py3gpp-0.5.0/py3gpp/codes/bg1.csv`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/codes/bg2.csv` & `py3gpp-0.5.0/py3gpp/codes/bg2.csv`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/CommonConfig.py` & `py3gpp-0.5.0/py3gpp/configs/CommonConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/DMRSConfigBase.py` & `py3gpp-0.5.0/py3gpp/configs/DMRSConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/PDSCHConfigBase.py` & `py3gpp-0.5.0/py3gpp/configs/PDSCHConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/PDSCHPTRSConfigBase.py` & `py3gpp-0.5.0/py3gpp/configs/PDSCHPTRSConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/nrCarrierConfig.py` & `py3gpp-0.5.0/py3gpp/configs/nrCarrierConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/nrNumerologyConfig.py` & `py3gpp-0.5.0/py3gpp/configs/nrNumerologyConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/nrPDSCHConfig.py` & `py3gpp-0.5.0/py3gpp/configs/nrPDSCHConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/nrPDSCHDMRSConfig.py` & `py3gpp-0.5.0/py3gpp/configs/nrPDSCHDMRSConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/configs/nrPathLossConfig.py` & `py3gpp-0.5.0/py3gpp/configs/nrPathLossConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/helper.py` & `py3gpp-0.5.0/py3gpp/helper.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrBCHDecode.py` & `py3gpp-0.5.0/py3gpp/nrBCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrCRCEncode.py` & `py3gpp-0.5.0/py3gpp/nrCRCEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrChannelEstimate.py` & `py3gpp-0.5.0/py3gpp/nrChannelEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrCodeBlockDesegmentLDPC.py` & `py3gpp-0.5.0/py3gpp/nrCodeBlockDesegmentLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrCodeBlockSegmentLDPC.py` & `py3gpp-0.5.0/py3gpp/nrCodeBlockSegmentLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrDLSCHInfo.py` & `py3gpp-0.5.0/py3gpp/nrDLSCHInfo.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrLDPCDecode.py` & `py3gpp-0.5.0/py3gpp/nrLDPCDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrLDPCEncode.py` & `py3gpp-0.5.0/py3gpp/nrLDPCEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrLayerMap.py` & `py3gpp-0.5.0/py3gpp/nrLayerMap.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrOFDMDemodulate.py` & `py3gpp-0.5.0/py3gpp/nrOFDMDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrOFDMModulate.py` & `py3gpp-0.5.0/py3gpp/nrOFDMModulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPBCH.py` & `py3gpp-0.5.0/py3gpp/nrPBCH.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPBCHDMRSIndices.py` & `py3gpp-0.5.0/py3gpp/nrPBCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCH.py` & `py3gpp-0.5.0/py3gpp/nrPDSCH.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCHDMRS.py` & `py3gpp-0.5.0/py3gpp/nrPDSCHDMRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCHDMRSIndices.py` & `py3gpp-0.5.0/py3gpp/nrPDSCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCHDecode.py` & `py3gpp-0.5.0/py3gpp/nrPDSCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCHIndices.py` & `py3gpp-0.5.0/py3gpp/nrPDSCHIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCHPTRS.py` & `py3gpp-0.5.0/py3gpp/nrPDSCHPTRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPDSCHPTRSIndices.py` & `py3gpp-0.5.0/py3gpp/nrPDSCHPTRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPathLoss.py` & `py3gpp-0.5.0/py3gpp/nrPathLoss.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPolarDecode.py` & `py3gpp-0.5.0/py3gpp/nrPolarDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrPolarEncode.py` & `py3gpp-0.5.0/py3gpp/nrPolarEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrRateMatchLDPC.py` & `py3gpp-0.5.0/py3gpp/nrRateMatchLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrRateMatchPolar.py` & `py3gpp-0.5.0/py3gpp/nrRateMatchPolar.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrRateRecoverLDPC.py` & `py3gpp-0.5.0/py3gpp/nrRateRecoverLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrRateRecoverPolar.py` & `py3gpp-0.5.0/py3gpp/nrRateRecoverPolar.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrSSS.py` & `py3gpp-0.5.0/py3gpp/nrSSS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrSymbolDemodulate.py` & `py3gpp-0.5.0/py3gpp/nrSymbolDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrSymbolModulate.py` & `py3gpp-0.5.0/py3gpp/nrSymbolModulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrTBS.py` & `py3gpp-0.5.0/py3gpp/nrTBS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp/nrTimingEstimate.py` & `py3gpp-0.5.0/py3gpp/nrTimingEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/py3gpp.egg-info/PKG-INFO` & `py3gpp-0.5.0/py3gpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.4.0
+Version: 0.5.0
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.4.0/py3gpp.egg-info/SOURCES.txt` & `py3gpp-0.5.0/py3gpp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 py3gpp/__init__.py
 py3gpp/helper.py
+py3gpp/nrBCH.py
 py3gpp/nrBCHDecode.py
 py3gpp/nrCRCDecode.py
 py3gpp/nrCRCEncode.py
 py3gpp/nrChannelEstimate.py
 py3gpp/nrCodeBlockDesegmentLDPC.py
 py3gpp/nrCodeBlockSegmentLDPC.py
 py3gpp/nrDLSCHInfo.py
@@ -64,14 +65,15 @@
 py3gpp/configs/__init__.py
 py3gpp/configs/nrCarrierConfig.py
 py3gpp/configs/nrNumerologyConfig.py
 py3gpp/configs/nrPDSCHConfig.py
 py3gpp/configs/nrPDSCHDMRSConfig.py
 py3gpp/configs/nrPDSCHPTRSConfig.py
 py3gpp/configs/nrPathLossConfig.py
+tests/test_nrBCH.py
 tests/test_nrBCHDecode.py
 tests/test_nrCRCDecode.py
 tests/test_nrCRCEncode.py
 tests/test_nrCodeBlockDesegmentLDPC.py
 tests/test_nrCodeBlockSegmentLDPC.py
 tests/test_nrDLSCHInfo.py
 tests/test_nrLDPCEncode.py
```

### Comparing `py3gpp-0.4.0/pyproject.toml` & `py3gpp-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 py3gpp = ["codes/*.csv"]
 
 [project]
-version = "0.4.0"
+version = "0.5.0"
 authors = [
     {name = "Benjamin Menküc", email = "benjamin@menkuec.de"},
 ]
 description = "Functions for 5G NR signal processing"
 name = "py3gpp"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `py3gpp-0.4.0/tests/test_nrBCHDecode.py` & `py3gpp-0.5.0/tests/test_nrBCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrCRCDecode.py` & `py3gpp-0.5.0/tests/test_nrCRCDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrCodeBlockDesegmentLDPC.py` & `py3gpp-0.5.0/tests/test_nrCodeBlockDesegmentLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrCodeBlockSegmentLDPC.py` & `py3gpp-0.5.0/tests/test_nrCodeBlockSegmentLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrLDPCEncode.py` & `py3gpp-0.5.0/tests/test_nrLDPCEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrLayerMap.py` & `py3gpp-0.5.0/tests/test_nrLayerMap.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPDSCH.py` & `py3gpp-0.5.0/tests/test_nrPDSCH.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPDSCHDMRS.py` & `py3gpp-0.5.0/tests/test_nrPDSCHDMRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPDSCHDMRSIndices.py` & `py3gpp-0.5.0/tests/test_nrPDSCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPDSCHDecode.py` & `py3gpp-0.5.0/tests/test_nrPDSCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPDSCHPTRS.py` & `py3gpp-0.5.0/tests/test_nrPDSCHPTRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPDSCHPTRSIndices.py` & `py3gpp-0.5.0/tests/test_nrPDSCHPTRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPathLoss.py` & `py3gpp-0.5.0/tests/test_nrPathLoss.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPolarDecode.py` & `py3gpp-0.5.0/tests/test_nrPolarDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPolarEncode.py` & `py3gpp-0.5.0/tests/test_nrPolarEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrPolarEncode_nrPolarDecode.py` & `py3gpp-0.5.0/tests/test_nrPolarEncode_nrPolarDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrRateMatchLDPC_nrRateRecoverLDPC.py` & `py3gpp-0.5.0/tests/test_nrRateMatchLDPC_nrRateRecoverLDPC.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrRateMatchPolar.py` & `py3gpp-0.5.0/tests/test_nrRateMatchPolar.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrRateRecoverPolar.py` & `py3gpp-0.5.0/tests/test_nrRateRecoverPolar.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_nrTBS.py` & `py3gpp-0.5.0/tests/test_nrTBS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.4.0/tests/test_phase_compensation.py` & `py3gpp-0.5.0/tests/test_phase_compensation.py`

 * *Files identical despite different names*

