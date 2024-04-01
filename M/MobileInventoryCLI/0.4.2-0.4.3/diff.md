# Comparing `tmp/MobileInventoryCLI-0.4.2.tar.gz` & `tmp/MobileInventoryCLI-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.2.tar", last modified: Mon Apr  1 18:30:26 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.3.tar", last modified: Mon Apr  1 19:03:51 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.2.tar` & `MobileInventoryCLI-0.4.3.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.847666 MobileInventoryCLI-0.4.2/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.827666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.830999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.834332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.834332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.834332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.837666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.837666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2346 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    97976 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.837666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.837666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.837666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     3921 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.837666 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15992 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    19634 2024-04-01 18:30:08.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.840999 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       17 2024-04-01 18:30:22.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-01 18:27:30.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:26.844332 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      690 2024-04-01 18:30:26.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4593 2024-04-01 18:30:26.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-01 18:30:26.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-01 18:30:26.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-01 18:30:26.000000 MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      690 2024-04-01 18:30:26.847666 MobileInventoryCLI-0.4.2/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-01 18:30:26.847666 MobileInventoryCLI-0.4.2/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      801 2024-04-01 18:30:26.000000 MobileInventoryCLI-0.4.2/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.864375 MobileInventoryCLI-0.4.3/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.844375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.847709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.851042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.851042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.851042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.851042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2346 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    99795 2024-04-01 18:56:25.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3921 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.854375 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1711 2024-04-01 19:02:09.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 19:00:25.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-01 19:01:10.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    19912 2024-04-01 19:03:23.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.857709 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       17 2024-04-01 19:03:46.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      191 2024-04-01 19:00:04.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.861042 MobileInventoryCLI-0.4.3/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-01 18:30:37.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 19:03:51.864375 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      690 2024-04-01 19:03:51.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-01 19:03:51.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-01 19:03:51.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-01 19:03:51.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-01 19:03:51.000000 MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      690 2024-04-01 19:03:51.864375 MobileInventoryCLI-0.4.3/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-01 19:03:51.864375 MobileInventoryCLI-0.4.3/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      801 2024-04-01 19:03:51.000000 MobileInventoryCLI-0.4.3/setup.py
```

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2279,8 +2279,65 @@
         self.Date=Date
         self.start=start
         self.end=end
         self.break_end=break_end
         self.break_start=break_start
         
 
-Shift.metadata.create_all(ENGINE)
+Shift.metadata.create_all(ENGINE)
+
+
+class Template:
+    def init(self,**kwargs):
+        __tablename__=self.__class__.__name__
+        fields=[i.name in self.__table__.columns]
+        for i in fields:
+            if i in list(kwargs.keys()):
+                setattr(self,i,kwargs.get(i))
+
+    def __str__(self,vc=Fore.light_yellow,fc=Fore.light_green,cc=Fore.light_magenta):
+        m=[]
+        m.append(f"{cc}{__class__.__name__}{Style.reset}(")
+        fields=[i.name in self.__table__.columns]
+        for i in fields:
+            m.append(f"{fc}{i}{Style.reset}={vc}{getattr(self,i)}{Style.reset}")
+
+class Billing(BASE,Template):
+    __tablename__="Billing"
+    sellerAddress=Column(String)
+    sellerName=Column(String)
+    purchaserName=Column(String)
+    purchaserAddress=Column(String)
+    BillingId=Column(Integer,primary_key=True)
+    Date=Column(Date)
+    RetailersPermitSerial=Column(String)
+    CertofReg=Column(String)
+    def __init__(self,**kwargs):
+        self.init(**kwargs)
+
+class RecieptEntry(BASE,Template):
+    __tablename__="RecieptEntry"
+    BillingId=Column(Integer,primary_key=True)
+    BillingDate=Column(Date)
+    EntryCode=Column(String)
+    EntryBarcode=Column(String)
+    EntryName=Column(String)
+    EntryId=Column(Integer)
+    EntryPrice=Column(Float)
+    QtySold=Column(Float)
+    def __init__(self,**kwargs):
+        self.init(**kwargs)
+
+class AdditionalExpenseOrFee(BASE,Template):
+    __tablename__="AdditionalExpenseOrFee"
+    AdditionalExpenseId=Column(Integer,primary_key=True)
+    Value=Column(Integer)
+    Name=Column(String)
+    Comment=Column(String)
+    DOE=Column(Date)#Date of Entry
+    DD=Column(Date)#Due Date
+    def __init__(self,**kwargs):
+        self.init(**kwargs)
+
+Billing.metadata.create_all(ENGINE)
+RecieptEntry.metadata.create_all(ENGINE)
+AdditionalExpenseOrFee.metadata.create_all(ENGINE)
```

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import csv
 from datetime import datetime
 from pathlib import Path
 from colored import Fore,Style,Back
 from barcode import Code39,UPCA,EAN8,EAN13
 import barcode,qrcode,os,sys,argparse
-from datetime import datetime,timedelta
+from datetime import datetime,timedelta,date
 import zipfile,tarfile
 import base64,json
 from ast import literal_eval
 import sqlalchemy
 from sqlalchemy import *
 from sqlalchemy.orm import *
 from sqlalchemy.ext.declarative import declarative_base as dbase
```

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,36 @@
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Locator.Locator import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ListMode2.ListMode2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.TasksMode.Tasks import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Collector2.Collector2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.LocationSequencer.LocationSequencer import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.PunchCard.PunchCard import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Conversion.Conversion import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.POS.POS import *
 import MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.possibleCode as pc
 import MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Unified.Unified as unified
 #VERSION="0.3.0177"
+def readCL():
+	text=''
+	with open("changelog.txt","r") as log:
+		while True:
+			d=log.read(1024)
+			if not d:
+				break
+			text+=d
+		return text
+
 class Main:
 	def collector2(self):
 		self.Collector2=Collector2(engine=self.engine,parent=self)
 
 	ChangeLog='''
-	11:25 am 04-1-2024 -- found a bug in db.Entry for NoneType correction
-	11:26 am 04-1-2024 -- planning to add 3 new class
-
-
 	'''
 	def __init__(self,engine,tables,error_log):
+		self.ChangeLog=readCL()
 		self.ExtractPkg=ExtractPkg
 		self.DayLogger=DayLogger
 		self.Lookup=Lookup
 		self.engine=engine
 		self.tables=tables
 		self.error_log=error_log
 		self.unified=lambda line,self=self:unified.Unified.unified(self,line=line)
@@ -146,14 +154,19 @@
 			'exec':lambda self=self:Conversion(engine=self.engine,parent=self),
 			'desc':'Convert a value from one unit to another!'
 			},
 		'ChangeLog':{
 			'cmds':['cl','16','changelog'],
 			'exec':lambda self=self:print(self.ChangeLog),
 			'desc':'print dev messages'
+			},
+		'POS':{
+			'cmds':['pos','17','point_of_sale'],
+			'exec':lambda self=self:POS(engine=self.engine,parent=self),
+			'desc':'print dev messages'
 			},	
 		}
 		#
 		#self.modeString=''.join([f"{Fore.cyan}{self.modes[i]['cmds']} - {self.modes[i]['desc']}{Style.reset}\n" for i in self.modes])
 		def printHelp(self):
 			st=[]
 			for i in self.modes:
```

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.2
+Version: 0.4.3
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.2/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.3/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 MobileInventoryCLI.egg-info/dependency_links.txt
 MobileInventoryCLI.egg-info/requires.txt
 MobileInventoryCLI.egg-info/top_level.txt
 MobileInventoryCLI/CodeProcessing/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
@@ -40,14 +41,16 @@
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
```

### Comparing `MobileInventoryCLI-0.4.2/PKG-INFO` & `MobileInventoryCLI-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.2
+Version: 0.4.3
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.2/setup.py` & `MobileInventoryCLI-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.2'
+version='0.4.3'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

