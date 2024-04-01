# Comparing `tmp/MobileInventoryCLI-0.3.9.tar.gz` & `tmp/MobileInventoryCLI-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.3.9.tar", last modified: Tue Mar  5 21:45:38 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.0.tar", last modified: Mon Apr  1 18:22:11 2024, max compression
```

## Comparing `MobileInventoryCLI-0.3.9.tar` & `MobileInventoryCLI-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,100 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.661834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    16682 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.665167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    29201 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5141 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)     4357 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     2929 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     1300 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.668501 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     1556 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    12519 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    23609 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    35226 2024-03-05 21:45:18.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4281 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.671834 MobileInventoryCLI-0.3.9/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-03-05 21:44:01.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      666 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     3790 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      109 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-03-05 21:45:38.000000 MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      666 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-03-05 21:45:38.675167 MobileInventoryCLI-0.3.9/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      791 2024-03-05 21:45:36.000000 MobileInventoryCLI-0.3.9/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.777655 MobileInventoryCLI-0.4.0/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.760988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.764322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.764322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.767655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.767655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.767655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.767655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2346 2024-03-28 13:54:18.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    97965 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.767655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.767655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3921 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.770988 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15992 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    19350 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       17 2024-04-01 18:21:57.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.774322 MobileInventoryCLI-0.4.0/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.777655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.777655 MobileInventoryCLI-0.4.0/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-03-28 13:50:36.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-01 18:22:11.777655 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      690 2024-04-01 18:22:11.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4593 2024-04-01 18:22:11.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-01 18:22:11.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-01 18:22:11.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-01 18:22:11.000000 MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      690 2024-04-01 18:22:11.777655 MobileInventoryCLI-0.4.0/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-01 18:22:11.777655 MobileInventoryCLI-0.4.0/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      801 2024-04-01 18:22:08.000000 MobileInventoryCLI-0.4.0/setup.py
```

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,376 +1,346 @@
-#Collector2.py
-
+import pandas as pd
+import csv
+from datetime import datetime
+from pathlib import Path
+from colored import Fore,Style,Back
+from barcode import Code39,UPCA,EAN8,EAN13
+import barcode,qrcode,os,sys,argparse
+from datetime import datetime,timedelta
+import zipfile,tarfile
+import base64,json
+from ast import literal_eval
+import sqlalchemy
+from sqlalchemy import *
+from sqlalchemy.orm import *
+from sqlalchemy.ext.declarative import declarative_base as dbase
+from sqlalchemy.ext.automap import automap_base
+from pathlib import Path
+import upcean
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ExtractPkg.ExtractPkg2 import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Lookup.Lookup import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DayLog.DayLogger import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.db import *
-import MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Unified.Unified as unified
-
-
-class Collector2:
-    def __init__(self,engine,parent):
-        self.parent=parent
-        self.engine=engine
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ConvertCode.ConvertCode import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.setCode.setCode import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Locator.Locator import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ListMode2.ListMode2 import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.TasksMode.Tasks import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ExportList.ExportListCurrent import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
 
 
+import MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.possibleCode as pc
+
+class TouchStampC:
+    def search(self):
+        def mkT(text,self):
+            try:
+                if len(text.split(".")) == 2:
+                    prefix,code=text.split(".")
+                elif len(text.split(".")) == 1:
+                    code=text.split(".")[0]
+                    prefix=''
+                else:
+                    raise Exception("Correct # of args is 2 or 1 by split off of '.'")
+                return prefix,code
+            except Exception as e:
+                print(e)
+                return
 
-        self.cmds={
-        'quit':{
-            'cmds':['q','quit'],
-            'exec':lambda :exit("user quit"),
-            'desc':'quit program!'
-        },
-        'back':{
-            'cmds':['b','back'],
-            'exec':None,
-            'desc':'go back a menu if any'
-        },
-        'collect':{
-            'cmds':['collect','1'],
-            'exec':self.collect,
-            'desc':'collect code pairs',
-        },
-        'collect_barcode':{
-            'cmds':['collect_barcode','1b'],
-            'exec':self.collect_barcode,
-            'desc':'collect code pairs',
-        },
-        'collect_barcode_w_nu_code':{
-            'cmds':['collect_barcode_w_nu_code','1bnuc'],
-            'exec':self.collect_barcode_w_nu_code,
-            'desc':'collect code pairs with item code, but do not check item code uniqueness [all item code duplicates!]',
-        },
-        'export':{
-            'cmds':['export','2'],
-            'exec':self.export,
-            'desc':'export code pairs',
-        },
-        'edit':{
-            'cmds':['edit','3'],
-            'exec':self.edit,
-            'desc':'edit code pairs',
-        },
-        'list':{
-            'cmds':['list','4'],
-            'exec':self.list,
-            'desc':'list code pairs',
-        },
-        'save':{
-            'cmds':['save_cp','5'],
-            'exec':self.saveAll,
-            'desc':'save code pairs to img',
-        },
-        'clear':{
-            'cmds':['clear_all_cp','6'],
-            'exec':self.clearAll,
-            'desc':'clear all code pairs',
-        },
-        'remove':{
-            'cmds':['remove_pc','7'],
-            'exec':self.removePC,
-            'desc':'remove code pair',
-        },
-        '?PC?':{
-            'cmds':['help',],
-            'exec':self.helpSMG,
-            'desc':"show help!"
-        },
-        '?unified':{
-            'cmds':['?unified',],
-            'exec':self.helpSMG2,
-            'desc':"unified cmds!"
-        }
-        }
-        while True:
-            cmd=input("do what[help]? :")
-            for c in self.cmds:
-                if cmd.lower() in ['help','?']:
-                    self.helpSMG()
-                    break
-                if self.cmds[c]['exec']!=None and cmd.lower() in self.cmds[c]['cmds'] or cmd.split(",")[0].lower() in self.cmds[c]['cmds']:
-                    if cmd.split(',')[0].lower() in ['edit','3'] or cmd.lower() in ["edit",'3']:
-                        if len(cmd.split(",")) == 2:
-                            self.edit(cmd.split(",")[1])
-                        elif len(cmd.split(",")) == 3:
-                            self.edit(cmd.split(",")[1],cmd.split(",")[2])
-                        elif len(cmd.split(",")) == 4:
-                            self.edit(cmd.split(",")[1],cmd.split(",")[2],cmd.split(",")[3])
-                        else:
-                            print("""
-#edit,$PCId - prompt for value and entry
-#edit,$PCId,field - prompt for value
-#edit,$PCId,field,value - set field=$field,value=$value no prompt
-                        """)
-                    elif cmd.split(',')[0].lower() in ['list','4'] or cmd.lower() in ["list",'4']:
-                        if len(cmd.split(",")) == 2:
-                            self.list(cmd.split(",")[1])
-                        else:
-                            print("""
-#list,$PCId - print PC
-#list,all - list all PC
-                        """)
-
-                    elif cmd.split(',')[0].lower() in ['remove_pc','7'] or cmd.lower() == ["remove_pc",'7']:
-                        if len(cmd.split(",")) == 2:
-                            self.removePC(cmd.split(",")[1])
-                        elif len(cmd.split(",")) == 3:
-                            self.removePC(cmd.split(",")[1],onlyID=bool(cmd.split(",")[2]))
+        value=Prompt.__init2__(None,func=mkT,ptext="Code|Barcode: ",helpText=self.helpTxt,data=self)
+        if not value:
+            return
+        else:
+            prefix,code=value
+            with Session(self.engine) as session:
+                query=session.query(Entry)
+                if prefix.lower() == '':
+                    query=query.filter(or_(Entry.Barcode==code,Entry.Code==code,Entry.Barcode.icontains(code),Entry.Code.icontains(code)))
+                elif prefix.lower() == 'c':
+                    query=query.filter(or_(Entry.Code==code,Entry.Code.icontains(code)))
+                elif prefix.lower() == 'b':
+                    query=query.filter(or_(Entry.Barcode==code,Entry.Barcode.icontains(code)))
+                elif prefix.lower() == 'e':
+                    query=query.filter(Entry.EntryId==int(code))
+                results=query.all()
+                if len(results) < 1:
+                    query=session.query(TouchStamp).filter(TouchStamp.EntryId==code)
+                    results=query.all()
+                    ct=len(results)
+                    if len(results) > 0:
+                        for num,r in enumerate(results):
+                            print(f"{Fore.green}{num}{Style.reset}/{Fore.light_red}{ct-1}{Style.reset} -> {r}")
+                    else:
+                        print("No Results!")
+                else:
+                    ct=len(results)
+                    if len(results) > 0:
+                        msg=f"{Fore.light_green}Num{Style.reset}/{Fore.light_red}Total{Style.reset} -> {Fore.dark_goldenrod}Name - Barcode - Code - r.Size - Location - Price - r.EntryId{Style.reset}"
+                        print(msg)
+                        for num,r in enumerate(results):
+                            extra=f'{r.Name} - {r.Barcode} - {r.Code} - {r.Size} - {r.Location} - {r.Price} - {r.EntryId}'
+                            if num % 2 == 0:
+                                extra=f'{Fore.grey_70}{extra}{Style.reset}'
+                            
+                            print(f"{Fore.green}{num}{Style.reset}/{Fore.light_red}{ct-1}{Style.reset} -> {extra}")
+                        
+                        def mInt(text,self):
+                            if text != '':
+                                return int(text)
+                            return 0
+                        print(msg)
+                        whichResult=Prompt.__init2__(None,func=mInt,ptext=f"Which result to use(0-{len(results)-1})[0]?",helpText=self.helpTxt,data=self)
+                        print(whichResult)
+                        if isinstance(whichResult,int):
+                            e=results[whichResult]
+                            eid=e.EntryId
+
+                            rs=session.query(TouchStamp).filter(TouchStamp.EntryId==eid).all()
+                            rs_ct=len(rs)
+                            for num,r in enumerate(rs):
+                                print(f"{Fore.green}{num}{Style.reset}/{Fore.light_red}{rs_ct}{Style.reset} -> {r}")
+                            print(f"{Fore.light_yellow}There are {Style.reset}{Fore.red}{rs_ct}{Style.reset} TouchStamp Results!")
                         else:
-                            print("""
-#remove_pc,$PCId - remove codePair by ID
-#remove_pc,$PCId,onlyId - remove codepair by id only if True , if set to false will go by code|barcode|id and will delete all if all exist DANGEROUS!!!
-#remove_cp, - show this
-                        """)
+                            print("Please Enter a valid number!")
                     else:
-                        if self.cmds[c]['exec'] == None:
-                            return
-                        self.cmds[c]['exec']()
-                    break
-                elif self.cmds[c]['exec']==None and cmd.lower() in self.cmds[c]['cmds']:
-                    return
-                elif self.parent != None and self.parent.Unified(cmd):
-                    print("ran an external command!")
-                    break
+                        print("No Results!")
+            
+
 
-    def edit(self,ID,field=None,value=None):
+    def __init__(self,engine,parent):
         try:
-            if field and value:
-                with Session(self.engine) as session:
-                    result=session.query(PairCollection).filter(PairCollection.PairCollectionId==ID).first()
-                    if result:
-                        setattr(result,field,value)
-                        session.commit()
-                        session.flush()
-                        session.refresh(result)
-                        print(result)
+            self.engine=engine
+            self.parent=parent
+            #print("TouchStamp Locator for Fast Note Logging!")
+            self.helpTxt=f"""TouchStamp Locator for Fast Note Logging!
+{Fore.cyan}+ | +,Note,Barcode|Code {Style.reset}-{Fore.grey_70} create a new touchstamp entry, '+' on its own will{Style.reset}
+                        {Fore.cyan}{Style.reset} {Fore.grey_70} prompt for details; otherwise use details as describe{Style.reset}
+{Fore.cyan}s | s,Note,Barcode|Code {Style.reset}-{Fore.grey_70} synthesize barcode for a new touchstamp entry, 's' on its own will{Style.reset}
+                        {Fore.cyan}{Style.reset} {Fore.grey_70} prompt for details; otherwise use details as describe
+{Fore.cyan}e | e,Note,TouchStampId {Style.reset}-{Fore.grey_70} edit a touchstamp entry, 'e' on its own will{Style.reset}
+                        {Fore.cyan}{Style.reset} {Fore.grey_70} prompt for details; otherwise use details as describe
+{Fore.cyan}- | -,TouchStampId      {Style.reset}-{Fore.grey_70} remove an entry by prompt ('-' on its own), or by TouchStampId{Style.reset}
+{Fore.cyan}l                       {Style.reset}-{Fore.grey_70} list all{Style.reset}
+{Fore.cyan}l,$TouchStampId         {Style.reset}-{Fore.grey_70} list touch stamp id{Style.reset}
+{Fore.cyan}l,Note|TouchStampId,$searchable {Style.reset}-{Fore.grey_70} search for in fields{Style.reset}
+{Fore.cyan}q|quit {Style.reset}-{Fore.grey_70} quit program{Style.reset}
+{Fore.cyan}b|back {Style.reset}-{Fore.grey_70} go back a menu{Style.reset}
+{Fore.light_magenta}#code is:
+W/ PREFIX:
+    b.$code - #code is Entry.Barcode
+    c.$code - #code is Entry.Code
+    e.$code - #code is Entry.EntryId
+W/O PREFIX:
+    $code - #code is either Entry.Barcode or Entry.Code
+{Style.reset}
+{Fore.light_yellow}sc|search_code{Style.reset}-{Fore.grey_70}Search using #code{Style.reset}
+            """
+            while True:
+                def mkT(text,self):
+                    return text
+                cmd=Prompt.__init2__(None,func=mkT,ptext=f"Do What?",helpText=self.helpTxt,data=self)
+                if not cmd:
+                    return
+                if cmd.lower() in ['sc','search_code']:
+                    self.search()
+                elif cmd.split(",")[0].lower() in ['+','a']:
+                    cmdline=cmd.split(",")
+                    ct=len(cmdline)
+
+                    if ct > 1 and ct == 3:
+                        barcode=None
+                        with Session(self.engine) as session:
+                            bcd=session.query(Entry).filter(or_(Entry.Barcode==cmdline[2],Entry.Code==cmdline[2])).first()
+                            print(bcd)
+                            if bcd:
+                                ts=TouchStamp(Note=cmdline[1],EntryId=bcd.EntryId)
+                            else:
+                                ts=TouchStamp(Note=cmdline[1],EntryId=None)
+                            session.add(ts)
+                            session.commit()
+                            session.refresh(ts)
+                            print(ts)
                     else:
-                        print(f"{Fore.red}{Back.white}{'*'*20}{Style.reset}\n{Fore.dark_goldenrod}No Result!{Style.reset}\n{Fore.red}{Back.white}{'*'*20}{Style.reset}")
-            if field and not value:
-                with Session(self.engine) as session:
-                    result=session.query(PairCollection).filter(PairCollection.PairCollectionId==ID).first()
-                    if result:
-                        value=input(f"{Fore.red}{field}{Style.reset} : ")
-                        setattr(result,field,value)
-                        session.commit()
-                        session.flush()
-                        session.refresh(result)
-                        print(result)
+                        while True:
+                            try:
+                                def mkT(text,self):
+                                    return text
+                                
+                                code=Prompt.__init2__(self,func=mkT,ptext='Barcode|Code',helpText="Please enter the code you will be using!",data=self)
+                                print(code)
+                                if code in [None,]:
+                                    break
+
+                                note=Prompt.__init2__(self,func=mkT,ptext='Note',helpText="Please enter the note you will be writing!",data=self)
+
+                                if note in [None,]:
+                                    break
+                                
+                                with Session(self.engine) as session:
+                                    bcd=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code)).first()
+                                    print(bcd)
+
+                                    if bcd:
+                                        ts=TouchStamp(Note=note,EntryId=bcd.EntryId)
+                                    else:
+                                        ts=TouchStamp(Note=note,EntryId=None)
+                                    session.add(ts)
+                                    session.commit()
+                                    session.refresh(ts)
+                                    print(ts)
+                                    break
+                            except Exception as e:
+                                print(e)
+                elif cmd.split(",")[0].lower() in ['s']:
+                    cmdline=cmd.split(",")
+                    ct=len(cmdline)
+
+                    if ct > 1 and ct == 2:
+                        barcode=None
+                        with Session(self.engine) as session:
+                            ts=TouchStamp(Note=cmdline[1],EntryId=Entry.synthetic_field_str(None))
+                            session.add(ts)
+                            session.commit()
+                            session.refresh(ts)
+                            print(ts)
                     else:
-                        print(f"{Fore.red}{Back.white}{'*'*20}{Style.reset}\n{Fore.dark_goldenrod}No Result!{Style.reset}\n{Fore.red}{Back.white}{'*'*20}{Style.reset}")
-            if not field and not value:
-                with Session(self.engine) as session:
-                    result=session.query(PairCollection).filter(PairCollection.PairCollectionId==ID).first()
-                    if result:
-                        field=input(f"{','.join([i.name for i in PairCollection.__table__.columns])}\n{Fore.yellow}Field{Style.reset}: ")
-                        value=input(f"{Fore.red}{field}OLD:{Style.reset}({getattr(result,field)}) : ")
-                        setattr(result,field,value)
-                        session.commit()
-                        session.flush()
-                        session.refresh(result)
-                        print(result)
+                        while True:
+                            try:
+                                def mkT(text,self):
+                                    return text
+                                note=Prompt.__init2__(self,func=mkT,ptext="Note",helpText="The note you need to record!")
+                                if note in [None,]:
+                                    break
+                                with Session(self.engine) as session:
+                                    ts=TouchStamp(Note=note,EntryId=Entry.synthetic_field_str(None))
+                                    session.add(ts)
+                                    session.commit()
+                                    session.refresh(ts)
+                                    print(ts)
+                                break
+                            except Exception as e:
+                                print(e)
+                elif cmd.split(",")[0].lower() in ['-']:
+                    cmdline=cmd.split(",")
+                    ct=len(cmdline)
+
+                    if ct > 1 and ct == 2:
+                        barcode=None
+                        with Session(self.engine) as session:
+                            r=session.query(TouchStamp).filter(TouchStamp.TouchStampId==int(cmdline[1])).delete()
+                            session.commit()
+                            print(f"deleted {r}")
                     else:
-                        print(f"{Fore.red}{Back.white}{'*'*20}{Style.reset}\n{Fore.dark_goldenrod}No Result!{Style.reset}\n{Fore.red}{Back.white}{'*'*20}{Style.reset}")
-        except Exception as e:
-            print(e)
-
-    def saveAll(self):
-         with Session(self.engine) as session:
-                    result=session.query(PairCollection).all()
-                    try:
-                        for num, r in enumerate(result):
-                            print(f"""{Fore.red}{num}{Style.reset} -> {r}""")
-                            r.saveItemData(num=num)
-                    except Exception as e:
-                        print(f"""{Fore.red}0{Style.reset} -> {result}""")
-    def clearAll(self):
-         with Session(self.engine) as session:
-            result=session.query(PairCollection).delete()
-            session.commit()
-            session.flush()
-            print(result)
-
-
-    def list(self,ID=None):
-        try:
-            if ID == None:
-                ID=input("{Fore.green_yellow}ID{Style.reset}|{Fore.cyan}Code{Style.reset}|{Fore.rgb(254,20,36)}Barcode to remove:{Style.reset} ")
-            if ID.lower() not in ["all",'a','al','*']:
-                with Session(self.engine) as session:
-                    result=session.query(PairCollection).filter(or_(PairCollection.PairCollectionId==int(ID),PairCollection.Barcode==ID,PairCollection.Code==ID)).all()
-                    try:
-                        for num, r in result:
-                            print(f"""{Fore.red}{num}{Style.reset} -> {r}""")
-                    except Exception as e:
-                        print(f"""{Fore.red}0{Style.reset} -> {result}""")
-            else:
-                with Session(self.engine) as session:
-                    result=session.query(PairCollection).all()
-                    try:
-                        for num, r in enumerate(result):
-                            print(f"""{Fore.red}{num}{Style.reset} -> {r}""")
-                    except Exception as e:
-                        print(f"""{Fore.red}0{Style.reset} -> {result}""")
+                        while True:
+                            try:
+                                def mkT(text,self):
+                                    return text
+                                
+                                code=Prompt.__init2__(self,func=mkT,ptext='TouchStampId',helpText="Please enter the TouchStampId you wish to delete!",data=self)
+                                print(code)
+                                if code in [None,]:
+                                    break
+                                else:
+                                    with Session(self.engine) as session:
+                                        bcd=session.query(TouchStamp).filter(TouchStamp.TouchStampId==int(code)).delete()
+                                        session.commit()
+                                        print(bcd) 
+                                break
+                            except Exception as e:
+                                print(e)         
+                elif cmd.split(",")[0].lower() in ['e']:
+                    cmdline=cmd.split(",")
+                    ct=len(cmdline)
+
+                    if ct > 1 and ct == 3:
+                        with Session(self.engine) as session:
+                            tsid=int(cmdline[2])
+                            ts=session.query(TouchStamp).filter(TouchStamp.TouchStampId==tsid).first()
+                            if ts:
+                                note=input("Note: ")
+                                if note.startswith("+"):
+                                    ts.Note+=note
+                                elif note.endswith("+"):
+                                    ts.Note=note+ts.Note
+                                elif note.startswith("-"):
+                                    ts.Note.replace(note,' '*len(note))
+                                else:
+                                    ts.Note=note
+                                print(ts)
+                            else:
+                                print(f"No Such TouchStampId!")
+                            session.commit()
+                    else:
+                        while True:
+                            try:
+                                with Session(self.engine) as session:
+                                    def mkT(text,self):
+                                        try:
+                                            return int(text)
+                                        except Exception as e:
+                                            return None
+                                    tsid=Prompt.__init2__(None,func=mkT,ptext="TouchStampId",helpText="The TouchStampId for the Entry you wish to edit!",data=self)
+                                    if tsid in [None,]:
+                                        break
+                                    ts=session.query(TouchStamp).filter(TouchStamp.TouchStampId==tsid).first()
+                                    if ts:
+                                        note=input("Note: ")
+                                        if note.startswith("+"):
+                                            ts.Note+=note[1:]
+                                        elif note.endswith("+"):
+                                            ts.Note=note[:-1]+ts.Note
+                                        elif note.startswith("-"):
+                                            ts.Note=ts.Note.replace(note[1:],'')
+                                        else:
+                                            ts.Note=note
+                                        print(ts)
+                                    else:
+                                        print(f"No Such TouchStampId!")
+                                    session.commit()
+                                    break
+                            except Exception as e:
+                                print(e)
+                elif cmd.split(",")[0].lower() in ['l']:
+                    cmdline=cmd.split(",")
+                    ct=len(cmdline)
+                    if ct == 1:
+                        with Session(self.engine) as session:
+                            results=session.query(TouchStamp).all()
+                            ct=len(results)
+                            for num,i in enumerate(results):
+                                print(f"{num}/{ct} -> {i}")
+                    elif ct > 1 and ct == 2:
+                       with Session(self.engine) as session:
+                            results=session.query(TouchStamp).filter(TouchStamp.TouchStampId==int(cmdline[1])).all()
+                            ct=len(results)
+                            for num,i in enumerate(results):
+                                print(f"{num}/{ct} -> {i}")
+                    elif ct > 1 and ct == 3:
+                        field=cmdline[1]
+                        if field not in ['Timestamp',]:
+                            if field == 'Note':
+                                with Session(self.engine) as session:
+                                    results=session.query(TouchStamp).filter(TouchStamp.Note.icontains(cmdline[2].lower())).all()
+                                    ct=len(results)
+                                    for num,i in enumerate(results):
+                                        print(f"{num}/{ct} -> {i}")
+                                    print(f"Total Results {ct}")
+                            elif field == "TouchStampId":
+                                with Session(self.engine) as session:
+                                    results=session.query(TouchStamp).filter(TouchStamp.TouchStampId==int(cmdline[2])).all()
+                                    ct=len(results)
+                                    for num,i in enumerate(results):
+                                        print(f"{num}/{ct} -> {i}")
+                                    print(f"Total Results {ct}") 
+                            else:
+                                print("Unsupported Field to Search!")
+                        #list items by searching field
+                    else:
+                        print(self.helpTxt)
+                        #prompt for field to search
+                        #print relevant touchstamps
+                
         except Exception as e:
             print(e)
-
-    def removePC(self,ID=None,onlyID=True):
-        try:
-            if ID == None:
-                ID=input("{Fore.green_yellow}ID{Style.reset}|{Fore.cyan}Code{Style.reset}|{Fore.rgb(254,20,36)}Barcode to remove:{Style.reset} ")
-            if ID.lower() != "":
-                if not onlyID:
-                    with Session(self.engine) as session:
-                        result=session.query(PairCollection).filter(or_(PairCollection.PairCollectionId==int(ID),PairCollection.Barcode==ID,PairCollection.Code==ID)).delete()
-                        print(result)
-                        session.commit()
-                        session.flush()
-                else:
-                    with Session(self.engine) as session:
-                        result=session.query(PairCollection).filter(PairCollection.PairCollectionId==int(ID)).delete()
-                        print(result)
-                        session.commit()
-                        session.flush()
         except Exception as e:
             print(e)
-
-    def helpSMG2(self):
-        self.parent.Unified('?')
-
-    def helpSMG(self):
-        for num,k in enumerate(self.cmds):
-            if num%2==0:
-                color=Fore.green
-                color2=Fore.cyan
-            else:
-                color=Fore.dark_goldenrod
-                color2=Fore.red
-            print(f"{color}{self.cmds[k]['cmds']}{Style.reset} - {color2}{self.cmds[k]['desc']}{Style.reset}")
-
-    def export(self):
-        with Session(self.engine) as session:
-            result=session.query(PairCollection).all()
-            for num,i in enumerate(result):
-                i.saveItemData(num=num)
-                print(i)
-            if len(result) < 1:
-                print(f"{Fore.red}{Back.white}{'*'*20}{Style.reset}\n{Fore.dark_goldenrod}No Items in List!{Style.reset}\n{Fore.red}{Back.white}{'*'*20}{Style.reset}")
-            else:
-                print(f"{Fore.green}{Back.white}{'*'*20}{Style.reset}\n{Fore.dark_goldenrod}List Contains {len(result)} PairCollection()'s\n{Style.reset}{Fore.green}{Back.white}{'*'*20}{Style.reset}")
-
-
-    def collect(self):
-        while True:
-            try:
-                print(Style.reset)
-                barcode=input(f"{Style.reset}{Fore.cyan}{Style.bold}barcode: {Style.reset}{Fore.green}")
-                if barcode.lower() in ['q','quit']:
-                    print(Style.reset)
-                    exit("user quit")
-                elif barcode in ['b','back']:
-                    print(Style.reset)
-                    return
-                print(Style.reset)
-                code=input(f"{Style.reset}{Style.bold}{Fore.dark_goldenrod}code: {Style.reset}{Fore.grey_50}")
-                if code.lower() in ['q','quit']:
-                    print(Style.reset)
-                    exit('user quit!')
-                elif code.lower() in ['b','back']:
-                    print(Style.reset)
-                    return
-                
-                if barcode in ['','n/a'] and code not in ['','n/a']:
-                    barcode=code
-                elif barcode not in ['','n/a'] and code in ['','n/a']:
-                    pass
-                elif barcode not in ['','n/a'] and code not in ['','n/a']:
-                    pass
-                else:
-                    raise Exception(f"1 Not Enough Values!{barcode}|BCD CD|{code}")
-
-
-                if code in ['','n/a'] and barcode not in ['','n/a']:
-                    code=barcode
-                elif code not in ['','n/a'] and barcode not in ['','n/a']:
-                    pass
-                else:
-                    raise Exception(f"2 Not Enough Values! {barcode}|BCD CD|{code}")
-
-                print(Style.reset)
-                with Session(self.engine) as session:
-                    query=session.query(PairCollection).filter(or_(PairCollection.Barcode==barcode,PairCollection.Code==code))
-                    result=query.first()
-                    if not result:
-                        pcd=PairCollection(Barcode=barcode,Code=code)
-                        session.add(pcd)
-                        session.commit()
-                        session.flush()
-                        session.refresh(pcd)
-                        print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
-
-                    else:
-                        print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
-                print(Style.reset)
-            except Exception as e:
-                print(e)
-
-    def collect_barcode(self):
-        while True:
-            try:
-                print(Style.reset)
-                barcode=input(f"{Style.reset}{Fore.cyan}{Style.bold}barcode: {Style.reset}{Fore.green}")
-                if barcode.lower() in ['q','quit']:
-                    print(Style.reset)
-                    exit("user quit")
-                elif barcode in ['b','back']:
-                    print(Style.reset)
-                    return
-                print(Style.reset)
-                with Session(self.engine) as session:
-                    query=session.query(PairCollection).filter(PairCollection.Barcode==barcode)
-                    result=query.first()
-                    if not result:
-                        pcd=PairCollection(Barcode=barcode,Code='',Name=f"New Item Created From Scan @ {datetime.now().ctime()}")
-                        session.add(pcd)
-                        session.commit()
-                        session.flush()
-                        session.refresh(pcd)
-                        print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
-
-                    else:
-                        print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
-                print(Style.reset)
-            except Exception as e:
-                print(e)
-
-    def collect_barcode_w_nu_code(self):
-        while True:
-            try:
-                print(Style.reset)
-                barcode=input(f"{Style.reset}{Fore.cyan}{Style.bold}barcode: {Style.reset}{Fore.green}")
-                if barcode.lower() in ['q','quit']:
-                    print(Style.reset)
-                    exit("user quit")
-                elif barcode in ['b','back']:
-                    print(Style.reset)
-                    return
-                code=input(f"{Style.reset}{Style.bold}{Fore.dark_goldenrod}code: {Style.reset}{Fore.grey_50}")
-                if code.lower() in ['q','quit']:
-                    print(Style.reset)
-                    exit('user quit!')
-                elif code.lower() in ['b','back']:
-                    print(Style.reset)
-                    return
-                print(Style.reset)
-                with Session(self.engine) as session:
-                    query=session.query(PairCollection).filter(PairCollection.Barcode==barcode)
-                    result=query.first()
-                    if not result:
-                        pcd=PairCollection(Barcode=barcode,Code=code,Name=f"New Item Created From Scan @ {datetime.now().ctime()}")
-                        session.add(pcd)
-                        session.commit()
-                        session.flush()
-                        session.refresh(pcd)
-                        print(f"{Back.green}{'*'*10}{Style.reset}\n{pcd}\n{Back.green}{'*'*10}{Style.reset}")
-
-                    else:
-                        print(f"{Back.red}{'*'*10}{Style.reset}\n{result}\n{Back.red}{'*'*10}{Style.reset}")
-                print(Style.reset)
-            except Exception as e:
-                print(e)
```

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class renderImageFromText:
     def setWidthFromLongestLine(self,text):
         lines=text.split("\n")
         old=0
         for line in lines:
             if len(line) > old:
                 old=len(line)
-        return int(old*(self.fontsize*0.65))
+        return int(old*(self.fontsize*1.0))
 
     def setHeightFromLines(self,text):
         lines=text.split("\n")
         print(len(lines))
         f=(self.fontsize*1.333)
         ff=f*len(lines)
         return int(ff)
@@ -93,15 +93,24 @@
         self.padded=(20,20)
         
         self.text=text
         
 
         self.image=Image.new("RGB",self.size,self.white)
         self.draw=ImageDraw.Draw(self.image)
-        self.font=ImageFont.load_default()
+        try:
+            raise Exception("e")
+            self.font=ImageFont.load_default(size=16)
+            print()
+        except Exception as e:
+            try:
+                self.font=ImageFont.truetype("/system/fonts/DroidSansMono.ttf",16)
+            except Exception as e:
+                print(e)
+                self.font=ImageFont.load_default() 
         self.save()
 
     def save(self):
         try:
             self.draw.text(self.padded,self.text,self.black,font=self.font)
             if self.barcode_file not in [True,False,None]:
                 w=self.width-self.barcode_file.size[0]
```

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sqlalchemy.orm import *
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import *
 import zipfile
 from colored import Fore,Back,Style
 
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.db import *
-
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
 
 
 class ExtractPkg:
 	def __str__(self):
 		return "ExtractPkg and Update Config"
 
 	def __init__(self,tbl,error_log,engine):
@@ -70,15 +70,36 @@
 											results=ses.query(ltbl.Item).all()
 											print(dir(ltbl))
 											for num,item in enumerate(results):
 												n=str(item.ImagePath)
 												if n != 'None':
 													n=str(Path("Images")/Path(Path(n).name))
 
-												entry=Entry(Name=item.Name,Barcode=item.Barcode,Code=item.Code,Price=item.Price,Image=n)
+												fields=[i.name for i in Entry.__table__.columns]
+												cfresults=ses.query(ltbl.CustomField).all()
+												
+												dt={}
+												for cf in cfresults:
+													#print(cf.Name)
+													if cf.Name in fields:
+														#item_cf_ids.append(cf.CustomFieldId)
+														#print(item_cf_ids)
+														cfdata=ses.query(ltbl.ItemCustomField).filter(ltbl.ItemCustomField.ItemId==item.ItemId,ltbl.ItemCustomField.CustomFieldId==cf.CustomFieldId).first()
+														if cfdata != None:
+															dt[cf.Name]=cfdata.Value
+												dt["Name"]=item.Name
+												dt["Barcode"]=item.Barcode
+												dt["Code"]=item.Code
+												dt["Price"]=item.Price
+												dt["Image"]=n
+												dt["Note"]=json.dumps({'Note':item.Note,'MeasurementUnit':item.MeasurementUnit})
+												dt["Size"]=f"SIZE:{dt.get('Size')}|Unit:{dt.get('SizeUnit')}"
+												if item.Tags:
+													dt["Tags"]=json.dumps(item.Tags.split(","))
+												entry=Entry(**dt)
 												session.add(entry)
 												if num % 100 == 0:
 													session.commit()
 												print(f'{num+1}/{len(results)}')
 											session.commit()
 									print("done importing")
 								else:
```

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 {Fore.green}CMD{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan} ACTION {Style.reset}
 {Fore.GREY_50}|{Style.reset} -> {Fore.magenta} lines with this character means OR so 's'|'search' is means s and search are the same thing{Style.reset}
 {Fore.GREY_50},{Style.reset} -> {Fore.violet} this is the cmd-field separator, so 's,Name,C4' is search field $Name with value C4. In Other words consider the ',' to be a space to separate cmds from their values{Style.reset}
 {Fore.GREY_50}${Style.reset} -> {Fore.magenta}a variable value represented by the suffix-following, i.e. $field could be {Style.bold}Entry.Name{Style.reset}
 {Fore.yellow}---------------------------{Style.reset}
 {Fore.green}cl|clear_list|clrl{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}clear list{Style.reset}
 {Fore.green}search|s|sch,$fieldName,$value{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}search for item ; before results are displayed, you will be asked if you want to save your results to a user defined csv file.{Style.reset}
-{Fore.green}$field,$EntryId{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}Display Item $field using $EntryId{Style.reset}
-{Fore.green}$field,$EntryId,$Value{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}set Item $field to $Value using $EntryId then display it.{Style.reset}
+{Fore.green}img|im|Image,$EntryId{Style.reset}-{Fore.cyan}Display Image Path for EntryId{Style.reset}
+{Fore.green}img|im|Image,$EntryId,$value{Style.reset}-{Fore.cyan}set Image for $EntryId with $value{Style.reset}
+{Fore.green}rm_img|rm_im|del_img,$EntryId{Style.reset}-{Fore.cyan}remove Image from $EntryId{Style.reset}
 {Fore.green}show,$EntryId{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}Display By EntryId{Style.reset}
 {Fore.green}save|sv|save_csv{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}Save Entry Table to CSV file{Style.reset}
 {Fore.green}save_bar|sb|svbr{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}Save Entry Table barcodes{Style.reset}
 {Fore.green}save_bar_cd|savebrcd|sbc{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}Save Entry Table Barcode,Code{Style.reset}
 {Fore.green}factory_reset{Style.reset} {Style.bold}-{Style.reset} {Fore.red}reset everything!{Style.reset}
 {Fore.green}fields|f|flds{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}Display Entry fields{Style.reset}
 {Fore.green}slm{Style.reset} {Style.bold}-{Style.reset} {Fore.cyan}show list mode{Style.reset}
@@ -26,9 +27,15 @@
 {Fore.green}export_list|el{Style.reset}-{Fore.cyan}export InList=True items to file prompted for{Style.reset}
 {Fore.green}clear|reset|screen_reset|#<>?{Style.reset}-{Fore.cyan}reset screen in case of screen corruption{Style.reset}
 {Fore.green}smle|smle,[Code|Barcode]{Style.reset}-{Fore.cyan}show list items if no argument, or show list items summary for item with Code or Barcode{Style.reset}
 {Fore.green}el|export_list{Style.reset}-{Fore.cyan}Export List to CSV file with delimiter ';', if you use 'q'|'quit' you will quit, 'b'|'back' you will return to previous menu, 'r'|'review_export'|'read' you will read the exported file provided by prompt or default at prompt!{Style.reset}
 {Fore.green}code_len{Style.reset}-{Fore.cyan}print len of scanned code{Style.reset}
 {Fore.green}location|geo|lctn|ln|l,$code{Style.reset}-{Fore.cyan}print location finding data for $code{Style.reset}
 {Fore.green}smle-e{Style.reset}-{Fore.cyan}save list items as png{Style.reset}
+{Fore.green}ni|new_item{Style.reset}-{Fore.cyan}create new Entry Item{Style.reset}
 {Fore.green}le-img{Style.reset}-{Fore.cyan}export list items as png{Style.reset}
 {Fore.green}smle,s|search|?{Style.reset} - {Fore.cyan}calls a prompt to search for InList==True with CODE|BARCODE instead of direct search waits for b for back, q for quit, for next CODE|BARCODE{Style.reset}
+{Fore.green}sai0|set_all_inlist_0{Style.reset} - {Fore.cyan}set all Entry's to InList=False{Style.reset}
+{Fore.green}sai1|set_all_inlist_1{Style.reset} - {Fore.cyan}set all Entry's to InList=True{Style.reset}
+{Fore.green}import_csv{Style.reset} - {Fore.cyan}Import CSV data, must have Barcode,Code,Name headers and if other Entry Fields are specified, then those will be used too, icluding valid image paths.{Style.reset}
+{Fore.green}ie|item_editor|itm_edt{Style.reset}-{Fore.cyan}Use the Item Editor,auto-scaling for new fields when new fields are added!{Style.reset}
+{Fore.green}export_list_field|elf{Style.reset}-{Fore.cyan}Export specified field to QREncoded Img from Entry.InList==True{Style.reset}
```

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.3.9
+Version: 0.4.0
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -17,7 +17,8 @@
 Requires-Dist: pandas
 Requires-Dist: Pillow
 Requires-Dist: python-barcode
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: argparse
+Requires-Dist: geocoder
```

### Comparing `MobileInventoryCLI-0.3.9/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.0/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,45 +5,55 @@
 MobileInventoryCLI.egg-info/SOURCES.txt
 MobileInventoryCLI.egg-info/__init__.py
 MobileInventoryCLI.egg-info/dependency_links.txt
 MobileInventoryCLI.egg-info/requires.txt
 MobileInventoryCLI.egg-info/top_level.txt
 MobileInventoryCLI/CodeProcessing/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
```

### Comparing `MobileInventoryCLI-0.3.9/PKG-INFO` & `MobileInventoryCLI-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.3.9
+Version: 0.4.0
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -17,7 +17,8 @@
 Requires-Dist: pandas
 Requires-Dist: Pillow
 Requires-Dist: python-barcode
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: argparse
+Requires-Dist: geocoder
```

### Comparing `MobileInventoryCLI-0.3.9/setup.py` & `MobileInventoryCLI-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.3.009'
+version='0.4.0'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
 
           ],
       packages=find_packages(),
       python_requires='>=3.6',
-      install_requires=['pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse'],
+      install_requires=['pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder'],
       package_data={
         '':["*.config","*.txt","*.README"],
         }
       )
+
```

