# Comparing `tmp/MobileInventoryCLI-0.3.8.tar.gz` & `tmp/MobileInventoryCLI-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.3.8.tar", last modified: Tue Mar  5 21:43:51 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.3.9.tar", last modified: Tue Mar  5 21:45:38 2024, max compression
```

## Comparing `MobileInventoryCLI-0.3.8.tar` & `MobileInventoryCLI-0.3.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.768498 MobileInventoryCLI-0.3.8/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.755165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.758498 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.758498 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.758498 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    16682 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.758498 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    29201 2024-03-05 21:41:15.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5141 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)     4357 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     2929 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     1300 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.761831 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     1556 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    12519 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    23609 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    35216 2024-03-05 21:43:34.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4281 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.765165 MobileInventoryCLI-0.3.8/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.768498 MobileInventoryCLI-0.3.8/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.768498 MobileInventoryCLI-0.3.8/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-03-05 21:36:40.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:43:51.768498 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      666 2024-03-05 21:43:51.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     3790 2024-03-05 21:43:51.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-03-05 21:43:51.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      109 2024-03-05 21:43:51.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-03-05 21:43:51.000000 MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      666 2024-03-05 21:43:51.768498 MobileInventoryCLI-0.3.8/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-03-05 21:43:51.768498 MobileInventoryCLI-0.3.8/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      791 2024-03-05 21:43:49.000000 MobileInventoryCLI-0.3.8/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.661834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    16682 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    29201 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5141 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4357 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2929 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1300 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1556 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    12519 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    23609 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    35226 2024-03-05 21:45:18.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4281 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      666 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     3790 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      109 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      666 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      791 2024-03-05 21:45:36.000000 MobileInventoryCLI-0.3.9/setup.py
```

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 1% similar despite different names*

```diff
@@ -706,24 +706,24 @@
 						,'Display_1':0,
 						'Display_2':0,
 						'Display_3':0,
 						'Display_4':0,
 						'Display_5':0,
 						'Display_6':0,
 						'Stock_Total':0,
-				        'CaseID_BR':''
-				        'CaseID_LD':''
-				        'CaseID_6W':''
-				        'SBX_WTR_DSPLY':0
-				        'SBX_CHP_DSPLY':0
-				        'SBX_WTR_KLR':0
-				        'FLRL_CHP_DSPLY':0
-				        'FLRL_WTR_DSPL':0
-				        'WD_DSPLY':0
-				        'CHKSTND_SPLY':0
+				        'CaseID_BR':'',
+				        'CaseID_LD':'',
+				        'CaseID_6W':'',
+				        'SBX_WTR_DSPLY':0,
+				        'SBX_CHP_DSPLY':0,
+				        'SBX_WTR_KLR':0,
+				        'FLRL_CHP_DSPLY':0,
+				        'FLRL_WTR_DSPL':0,
+				        'WD_DSPLY':0,
+				        'CHKSTND_SPLY':0,
 						})
 					session.commit()
 					session.flush()
 					print(result)
 			print("-"*10)
 			return True
 		elif args[0].lower() in ["clear_all_img","cam","clrallimg"]:
```

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.3.8
+Version: 0.3.9
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.3.8/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.8/PKG-INFO` & `MobileInventoryCLI-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.3.8
+Version: 0.3.9
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.3.8/setup.py` & `MobileInventoryCLI-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.3.008'
+version='0.3.009'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

