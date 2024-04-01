# Comparing `tmp/drapi-lemur-1.0.4.tar.gz` & `tmp/drapi-lemur-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drapi-lemur-1.0.4.tar", last modified: Mon Feb 12 02:04:54 2024, max compression
+gzip compressed data, was "drapi-lemur-1.0.5.tar", last modified: Mon Feb 12 02:49:40 2024, max compression
```

## Comparing `drapi-lemur-1.0.4.tar` & `drapi-lemur-1.0.5.tar`

### file list

```diff
@@ -1,217 +1,205 @@
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.241498 drapi-lemur-1.0.4/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       25 2024-01-15 01:07:06.000000 drapi-lemur-1.0.4/MANIFEST.in
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      657 2024-02-12 02:04:54.241293 drapi-lemur-1.0.4/PKG-INFO
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      425 2023-04-17 18:00:20.000000 drapi-lemur-1.0.4/README.md
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       79 2024-02-12 02:04:54.241932 drapi-lemur-1.0.4/setup.cfg
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1142 2024-02-12 02:04:06.000000 drapi-lemur-1.0.4/setup.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.199452 drapi-lemur-1.0.4/src/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6148 2024-02-09 21:56:20.000000 drapi-lemur-1.0.4/src/.DS_Store
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.200024 drapi-lemur-1.0.4/src/drapi/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     8196 2024-02-09 21:56:26.000000 drapi-lemur-1.0.4/src/drapi/.DS_Store
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/__init__.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.200526 drapi-lemur-1.0.4/src/drapi/__pycache__/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      151 2024-02-05 01:39:50.000000 drapi-lemur-1.0.4/src/drapi/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      155 2024-02-05 01:38:18.000000 drapi-lemur-1.0.4/src/drapi/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.201209 drapi-lemur-1.0.4/src/drapi/code/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6148 2024-02-09 21:56:31.000000 drapi-lemur-1.0.4/src/drapi/code/.DS_Store
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 22:32:57.000000 drapi-lemur-1.0.4/src/drapi/code/__init__.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.203937 drapi-lemur-1.0.4/src/drapi/code/drapi/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     8196 2024-01-15 01:12:11.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/.DS_Store
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/__init__.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.204768 drapi-lemur-1.0.4/src/drapi/code/drapi/c2s/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/c2s/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     4045 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/c2s/c2s.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1889 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/c2s/checkC2S.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6928 2024-02-12 01:01:54.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/compareGroups.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.205799 drapi-lemur-1.0.4/src/drapi/code/drapi/constants/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/constants/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6379 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/constants/constants.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     9415 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/constants/phiValues.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    18623 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/constants/phiVariables.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.209031 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/__init__.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     4520 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     4075 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     3955 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3504 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     6385 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     4373 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     1376 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     4594 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     2279 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     8834 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     2996 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     5686 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    26702 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/drapi.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      312 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/getPersonIDs.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.209943 drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6466 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/getEncountersMap.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3276 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/getPatientsMap.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1572 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/idealist.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.210402 drapi-lemur-1.0.4/src/drapi/code/drapi/images/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/images/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     2474 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/images/utilities.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      815 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/makeSymLinks.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.211348 drapi-lemur-1.0.4/src/drapi/code/drapi/notes/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/notes/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    29050 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/notes/freeText.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     5286 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/notes/pullNotes.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      823 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/notes/utils.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.212001 drapi-lemur-1.0.4/src/drapi/code/drapi/omop/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/omop/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     2969 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/omop/configProcessing.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     5545 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/omop/deidentify.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3215 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/oneFlorida.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     5590 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/prepTSVforSDOH.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/searchFolders.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1379 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/sql.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     2051 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/drapi/stats.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.212263 drapi-lemur-1.0.4/src/drapi/code/makeDirTemplate/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-11 01:04:41.000000 drapi-lemur-1.0.4/src/drapi/code/makeDirTemplate/__init__.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3549 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/code/tree.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.213902 drapi-lemur-1.0.4/src/drapi/sql/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1754 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/sql/9-Digit Zip Code.SQL
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      909 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/sql/Consent2Share.sql
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      701 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      994 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/sql/LADMF.sql
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     2341 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/sql/MRNfromPatientKey.sql
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      757 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/sql/MapOneFloridaIDs.SQL
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      896 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/sql/encounterNumber2patientKey.SQL
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.214136 drapi-lemur-1.0.4/src/drapi/templates/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6148 2024-02-09 21:56:20.000000 drapi-lemur-1.0.4/src/drapi/templates/.DS_Store
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.214643 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6148 2024-01-15 00:33:41.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/.DS_Store
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.189808 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.214897 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1184 2024-02-12 00:59:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.215389 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3093 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.216441 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       73 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.env
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3114 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     3987 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.222936 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     8606 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     9546 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     8799 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     7754 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6842 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/dataQualityTest.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)    14314 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    11047 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    14920 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     8148 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)    14716 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     8761 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/gatherFiles.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)    14776 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     9982 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     8329 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     7323 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6042 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     8919 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     4908 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)    16782 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     7192 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     9130 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makePersonIDMap.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      663 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.196350 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.224023 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       73 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.env
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3172 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      395 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.224602 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     8276 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/functions.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     5725 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.191873 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.224898 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:09:53.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/.deleteme
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.225160 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:09:56.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/.deleteme
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      663 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.226181 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       73 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.env
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3114 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      395 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.227003 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     4427 2024-02-12 00:59:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     6984 2024-02-12 01:01:54.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1931 2024-02-12 00:59:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.192930 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.227255 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:16.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/.deleteme
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.227513 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:16.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/.deleteme
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      663 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.228505 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       73 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.env
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     3114 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.229071 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    13016 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)    36696 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.193970 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.229371 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:38.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/.deleteme
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.229637 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:38.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/.deleteme
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      663 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.231921 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     3248 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      408 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_text.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     2604 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      179 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_text.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     2603 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      177 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_text.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)     2638 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql
--rwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)      202 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_text.sql
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.233466 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       73 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.env
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3114 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     7852 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.233983 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     5279 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadButton.png
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)   275966 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadDirectory.png
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     2008 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README-INSTALLATION.md
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     4198 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.235007 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    15760 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     5545 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     7797 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.195419 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.235292 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:46.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/.deleteme
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.235561 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:46.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/.deleteme
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      663 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.235832 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      168 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/grabPersonIDs.SQL
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.236136 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      756 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.236403 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      756 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.237442 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       73 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.env
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3114 2024-01-11 00:33:48.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      395 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/README.md
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.237716 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    24103 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.197234 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.237999 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:28.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.238248 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      110 2024-01-15 00:10:28.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      663 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      401 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/README.md
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)       98 2024-02-05 01:36:25.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/__init__.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.238784 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/__pycache__/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      296 2024-02-05 01:39:50.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      300 2024-02-05 01:38:18.000000 drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.239297 drapi-lemur-1.0.4/src/drapi/templates/scripts/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     3908 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/scripts/hippaDisclosure.py
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     1423 2024-01-08 00:02:10.000000 drapi-lemur-1.0.4/src/drapi/templates/scripts/sqlQuery.py
-drwxr-xr-x   0 herman   (222083068) UFAD\Domain Users (1166719947)        0 2024-02-12 02:04:54.240809 drapi-lemur-1.0.4/src/drapi_lemur.egg-info/
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)      657 2024-02-12 02:04:53.000000 drapi-lemur-1.0.4/src/drapi_lemur.egg-info/PKG-INFO
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)    12587 2024-02-12 02:04:54.000000 drapi-lemur-1.0.4/src/drapi_lemur.egg-info/SOURCES.txt
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        1 2024-02-12 02:04:53.000000 drapi-lemur-1.0.4/src/drapi_lemur.egg-info/dependency_links.txt
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)        6 2024-02-12 02:04:53.000000 drapi-lemur-1.0.4/src/drapi_lemur.egg-info/top_level.txt
--rw-r--r--   0 herman   (222083068) UFAD\Domain Users (1166719947)     4211 2024-02-05 02:16:38.000000 drapi-lemur-1.0.4/src/makeDirTemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/c2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/checkC2S.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/compareGroups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiValues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiVariables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4520 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6385 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4373 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1376 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4594 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8834 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2996 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5686 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25947 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/drapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/getPersonIDs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getEncountersMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getPatientsMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/idealist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/images/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/makeSymLinks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29050 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/freeText.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/pullNotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/configProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/deidentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/oneFlorida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/prepTSVforSDOH.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/searchFolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/code/makeDirTemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/makeDirTemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/9-Digit Zip Code.SQL
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/Consent2Share.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/LADMF.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/MRNfromPatientKey.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/MapOneFloridaIDs.SQL
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/encounterNumber2patientKey.SQL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3987 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9361 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8610 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7588 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/dataQualityTest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14059 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14603 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14419 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8538 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/gatherFiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14496 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9747 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16439 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7024 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8933 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makePersonIDMap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      395 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8100 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      395 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.env
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35999 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3248 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_text.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_text.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2603 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_text.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_text.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)   275966 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadDirectory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README-INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/grabPersonIDs.SQL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)    23578 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/scripts/hippaDisclosure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/scripts/sqlQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-12 02:49:39.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-02-12 02:49:40.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 02:49:39.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-12 02:49:39.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/makeDirTemplate.py
```

### Comparing `drapi-lemur-1.0.4/PKG-INFO` & `drapi-lemur-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drapi-lemur
-Version: 1.0.4
+Version: 1.0.5
 Summary: Data Request API for the Integrated Data Repository Research Services of University of Florida.
 Home-page: https://github.com/ChemGuy88/hermanCode/archive/refs/tags/v1.0.0.tar.gz
 Author: Herman Autore
 Author-email: hf.autore+drapi@gmail.com
 Keywords: CTSI,Clinical and Translational Science Institute,IDR,Integrated Data Repository,Integrated Data Repository Research Services,ODSRI,Office of Data Science and Research Implementation,Shands,Sloth 🦥,UF,UF Health,UFHealth,University of Florida
 
 Data Request API for the Integrated Data Repository Research Services of University of Florida.
```

### Comparing `drapi-lemur-1.0.4/setup.py` & `drapi-lemur-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_namespace_packages
 
 setup(name='drapi-lemur',
       package_dir={"": "src"},
       include_package_data=True,
       packages=find_namespace_packages(where="src"),
-      version='1.0.4',
+      version='1.0.5',
       description='Data Request API for the Integrated Data Repository Research Services of University of Florida.',
       long_description="Data Request API for the Integrated Data Repository Research Services of University of Florida.",
       author='Herman Autore',
       author_email='hf.autore+drapi@gmail.com',
       url='https://github.com/ChemGuy88/hermanCode/archive/refs/tags/v1.0.0.tar.gz',
       keywords=['CTSI',
                 'Clinical and Translational Science Institute',
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/c2s/c2s.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/c2s.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-"""
-Consent-to-Share helper functions. Consent-to-Share is also known as "C2S".
-"""
-
-import logging
-import os
-from pathlib import Path
-from typing import List
-from typing_extensions import Literal
-# Third-party libraries
-import pandas as pd
-# Local libraries
-from drapi.drapi import replace_sql_query
-from drapi.drapi import successiveParents
-
-# Arguments
-MODULE_ROOT_DIRECTORY_PATH = successiveParents(Path(__file__), 4)
-
-# Arguments: SQL connection settings
-SERVER = "EDW.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-
-def checkStatus(statusType=Literal["C2S", "death"],
-                location=Literal["gnv", "jax"],
-                listOfMRNs=List[str]) -> pd.DataFrame:
-    """
-    This functions performs the Consent-to-Share ("C2S") check before release, to ensure deceased or opted-out patients aren't contacted.
-    """
-
-    # Determine query type
-    if statusType == "C2S":
-        queryFilePath = MODULE_ROOT_DIRECTORY_PATH.joinpath("sql/Consent2Share.sql")
-    elif statusType == "death":
-        queryFilePath = MODULE_ROOT_DIRECTORY_PATH.joinpath("sql/LADMF.sql")
-
-    # Define values for query: LOCATION_NAME, LOCATION_TYPE
-    location_lower_case = location.lower()
-    if location_lower_case == "gnv":
-        locationNameForQuery = "UF"
-        locationValueForQuery = "101"
-    elif location_lower_case == "jax":
-        locationNameForQuery = "Jax"
-        locationValueForQuery = "110"
-
-    # Define value for query: LIST_OF_MRNS
-    MRNValuesForQuery = ",".join(f"'{MRNNumber}'" for MRNNumber in listOfMRNs)
-
-    # Load query template
-    with open(queryFilePath, "r") as file:
-        query0 = file.read()
-
-    # Prepare query
-    query = replace_sql_query(query=query0, old="{<PYTHON_PLACEHOLDER : LOCATION_NAME>}", new=locationNameForQuery)
-    query = replace_sql_query(query=query, old="{<PYTHON_PLACEHOLDER : LOCATION_TYPE>}", new=locationValueForQuery)
-    query = replace_sql_query(query=query, old="{<PYTHON_PLACEHOLDER : LIST_OF_MRNS>}", new=MRNValuesForQuery)
-
-    # Run query
-    logging.debug(query)
-    queryResult = pd.read_sql(sql=query, con=conStr)
-
-    return queryResult
-
-
-def doCheck(result, statusType):
-    """
-    Analyzes table values to deduce if the entire table passes the check. Any patients that fail the check are returned in a table.
-    """
-    result = pd.DataFrame(result)
-    if statusType == "C2S":
-        s1 = pd.Series(result["CONSENT_SHARE_IND"])
-        r1 = (s1 == "Y")
-        r1sum = r1.sum()
-        s2 = pd.Series(result["CONSENT_SHARE_DATE"])
-        r2 = s2.notna()
-        r2sum = r2.sum()
-        length = len(result)
-        if (r1sum == length) and (r2sum == length):
-            checkResultPass = True
-            failedRows = None
-        else:
-            checkResultPass = False
-            # Print failed rows
-            mask = ~r1 | ~r2
-            failedRows = result[mask]
-
-    elif statusType == "death":
-        s1 = pd.Series(result["PATNT_SSN_DTH_IND"])
-        r1 = (s1 == "N")
-        r1sum = r1.sum()
-        s2 = pd.Series(result["PATNT_SSN_DTH_DATE"])
-        r2 = s2.isna()
-        r2sum = r2.sum()
-        s3 = pd.Series(result["PATNT_DTH_IND"])
-        r3 = (s3 == "N")
-        r3sum = r3.sum()
-        s4 = pd.Series(result["PATNT_DTH_DATE"])
-        r4 = s4.isna()
-        r4sum = r4.sum()
-        length = len(result)
-        if (r1sum == length) and (r2sum == length) and (r3sum == length) and (r4sum == length):
-            checkResultPass = True
-            failedRows = None
-        else:
-            checkResultPass = False
-            # Print failed rows
-            mask = ~r1 | ~r2 | ~r3 | ~r4
-            failedRows = result[mask]
-
-    return checkResultPass, failedRows
+"""
+Consent-to-Share helper functions. Consent-to-Share is also known as "C2S".
+"""
+
+import logging
+import os
+from pathlib import Path
+from typing import List
+from typing_extensions import Literal
+# Third-party libraries
+import pandas as pd
+# Local libraries
+from drapi.drapi import replace_sql_query
+from drapi.drapi import successiveParents
+
+# Arguments
+MODULE_ROOT_DIRECTORY_PATH = successiveParents(Path(__file__), 4)
+
+# Arguments: SQL connection settings
+SERVER = "EDW.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+
+def checkStatus(statusType=Literal["C2S", "death"],
+                location=Literal["gnv", "jax"],
+                listOfMRNs=List[str]) -> pd.DataFrame:
+    """
+    This functions performs the Consent-to-Share ("C2S") check before release, to ensure deceased or opted-out patients aren't contacted.
+    """
+
+    # Determine query type
+    if statusType == "C2S":
+        queryFilePath = MODULE_ROOT_DIRECTORY_PATH.joinpath("sql/Consent2Share.sql")
+    elif statusType == "death":
+        queryFilePath = MODULE_ROOT_DIRECTORY_PATH.joinpath("sql/LADMF.sql")
+
+    # Define values for query: LOCATION_NAME, LOCATION_TYPE
+    location_lower_case = location.lower()
+    if location_lower_case == "gnv":
+        locationNameForQuery = "UF"
+        locationValueForQuery = "101"
+    elif location_lower_case == "jax":
+        locationNameForQuery = "Jax"
+        locationValueForQuery = "110"
+
+    # Define value for query: LIST_OF_MRNS
+    MRNValuesForQuery = ",".join(f"'{MRNNumber}'" for MRNNumber in listOfMRNs)
+
+    # Load query template
+    with open(queryFilePath, "r") as file:
+        query0 = file.read()
+
+    # Prepare query
+    query = replace_sql_query(query=query0, old="{<PYTHON_PLACEHOLDER : LOCATION_NAME>}", new=locationNameForQuery)
+    query = replace_sql_query(query=query, old="{<PYTHON_PLACEHOLDER : LOCATION_TYPE>}", new=locationValueForQuery)
+    query = replace_sql_query(query=query, old="{<PYTHON_PLACEHOLDER : LIST_OF_MRNS>}", new=MRNValuesForQuery)
+
+    # Run query
+    logging.debug(query)
+    queryResult = pd.read_sql(sql=query, con=conStr)
+
+    return queryResult
+
+
+def doCheck(result, statusType):
+    """
+    Analyzes table values to deduce if the entire table passes the check. Any patients that fail the check are returned in a table.
+    """
+    result = pd.DataFrame(result)
+    if statusType == "C2S":
+        s1 = pd.Series(result["CONSENT_SHARE_IND"])
+        r1 = (s1 == "Y")
+        r1sum = r1.sum()
+        s2 = pd.Series(result["CONSENT_SHARE_DATE"])
+        r2 = s2.notna()
+        r2sum = r2.sum()
+        length = len(result)
+        if (r1sum == length) and (r2sum == length):
+            checkResultPass = True
+            failedRows = None
+        else:
+            checkResultPass = False
+            # Print failed rows
+            mask = ~r1 | ~r2
+            failedRows = result[mask]
+
+    elif statusType == "death":
+        s1 = pd.Series(result["PATNT_SSN_DTH_IND"])
+        r1 = (s1 == "N")
+        r1sum = r1.sum()
+        s2 = pd.Series(result["PATNT_SSN_DTH_DATE"])
+        r2 = s2.isna()
+        r2sum = r2.sum()
+        s3 = pd.Series(result["PATNT_DTH_IND"])
+        r3 = (s3 == "N")
+        r3sum = r3.sum()
+        s4 = pd.Series(result["PATNT_DTH_DATE"])
+        r4 = s4.isna()
+        r4sum = r4.sum()
+        length = len(result)
+        if (r1sum == length) and (r2sum == length) and (r3sum == length) and (r4sum == length):
+            checkResultPass = True
+            failedRows = None
+        else:
+            checkResultPass = False
+            # Print failed rows
+            mask = ~r1 | ~r2 | ~r3 | ~r4
+            failedRows = result[mask]
+
+    return checkResultPass, failedRows
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/c2s/checkC2S.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/checkC2S.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/compareGroups.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/compareGroups.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-"""
-Compare two cohort (group) files.
-"""
-
-import logging
-from typing_extensions import (Literal,
-                               Union)
-# Third-party packages
-import pandas as pd
-
-
-def mappingAnalysis(x0: Union[pd.DataFrame, pd.Series], m0: pd.DataFrame, logger: logging.Logger, mappingMethod: Literal["inner", "outer"] = "inner") -> None:
-    """
-    # x0: The vector of input values
-    # m0: The matrix of mapping values, an n_m by 2 matrix
-    # x1: The vector of output values
-    """
-    assert len(x0.shape) == 1 or x0.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
-    assert len(m0.shape) == 2, "The mapping table should be of two dimensions."
-    assert m0.shape[1] == 2, "The mapping table should be of two columns."
-    if isinstance(x0, pd.DataFrame):
-        pass
-    elif isinstance(x0, pd.Series):
-        x0 = pd.DataFrame(x0)
-    else:
-        raise Exception(f"""`x0` is of an unexpected type: "{type(x0)}".""")
-    fromColumn = x0.columns.to_list()[0]
-    toColumn = m0.columns.to_list()[1]
-
-    mappingMethodsList = ["inner", "outer"]
-    x1 = {}
-    for mappingMethod in mappingMethodsList:
-        x1[mappingMethod] = x0.set_index(fromColumn).join(other=m0.set_index(fromColumn),
-                                                          how=mappingMethod,
-                                                          lsuffix="_L",
-                                                          rsuffix="_R")
-
-    lenx0 = len(x0)
-    lenx0unique = len(x0.drop_duplicates())
-    lenm0 = len(m0)
-    lenm0_1 = len(m0[fromColumn])
-    lenm0_2 = len(m0[toColumn])
-    lenm0_1unique = len(m0[fromColumn].drop_duplicates())
-    lenm0_2unique = len(m0[toColumn].drop_duplicates())
-    lenx1 = {}
-    lenx1unique = {}
-    for mappingMethod in mappingMethodsList:
-        lenx1[mappingMethod] = len(x1[mappingMethod])
-        lenx1unique[mappingMethod] = len(x1[mappingMethod].drop_duplicates())
-
-    logger.info(f"""The size of the input group is {lenx0:,}.""")
-    logger.info(f"""The size of the input group (unique values) is {lenx0unique:,}.""")
-    logger.info(f"""The size of the entire map is {lenm0:,}.""")
-    logger.info(f"""The size of the map's left side is {lenm0_1:,}.""")
-    logger.info(f"""The size of the map's right side is {lenm0_2:,}.""")
-    logger.info(f"""The size of the map's left side (unique values) is {lenm0_1unique:,}.""")
-    logger.info(f"""The size of the map's right side (unique values) is {lenm0_2unique:,}.""")
-    for mappingMethod in mappingMethodsList:
-        logger.info(f"""  Mapping values using method "{mappingMethod}".""")
-        logger.info(f"""    The size of the output group is {lenx1[mappingMethod]:,}.""")
-        logger.info(f"""    The size of the output group (unique values) is {lenx1unique[mappingMethod]:,}.""")
-
-
-def compareGroups(group1: Union[pd.DataFrame, pd.Series], group2: Union[pd.DataFrame, pd.Series], logger: logging.Logger) -> None:
-    """
-    """
-    assert len(group1.shape) == 1 or group1.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
-    assert len(group2.shape) == 1 or group2.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
-    if isinstance(group1, pd.DataFrame):
-        group1series = group1.iloc[:, 0]
-    else:
-        group1series = group1
-    if isinstance(group2, pd.DataFrame):
-        group2series = group2.iloc[:, 0]
-    else:
-        group2series = group2
-
-    c1l = len(group1series)
-    c2l = len(group2series)
-
-    c1inc2 = group1series.isin(group2series)
-    c2inc1 = group2series.isin(group1series)
-
-    c1inc2count = c1inc2.sum()
-    c2inc1count = c2inc1.sum()
-
-    c1inc2percent = c1inc2count / c1l
-    c2inc1percent = c2inc1count / c2l
-
-    intersection = set(group1series.to_list()).intersection(set(group2series.to_list()))
-    intersectionl = len(intersection)
-
-    logger.info("""The following results are of the set of groups 1 and 2. I.e., we are only counting the unique values.""")
-    logger.info(f"""Group 1 size: {c1l:,}.""")
-    logger.info(f"""Group 2 size: {c2l:,}.""")
-    logger.info(f"""Size of intersection of groups 1 and 2: {intersectionl:,}.""")
-    logger.info(f"""Percent of group 1 in group 2: {c1inc2percent:.2%}.""")
-    logger.info(f"""Percent of group 2 in group 1: {c2inc1percent:.2%}.""")
-
-
-def determineMapType(x0: Union[pd.DataFrame, pd.Series], x1: Union[pd.DataFrame, pd.Series]):
-    """
-    """
-    assert len(x0.shape) == 1 or x0.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
-    assert len(x1.shape) == 1 or x1.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
-
-    x0duplicated = x0.duplicated().sum() > 0
-    x1duplicated = x1.duplicated().sum() > 0
-
-    if x0duplicated and x1duplicated:
-        mapType = "m:m"
-    elif x0duplicated:
-        mapType = "m:1"
-    elif x1duplicated:
-        mapType = "1:m"
-    elif (not x0duplicated) & (not x1duplicated):
-        mapType = "1:1"
-    else:
-        raise Exception("Unexpected error.")
-
-    return mapType
-
-
-def _determineMapType_MapValues(x0: Union[pd.DataFrame, pd.Series],
-                                m0: pd.DataFrame) -> pd.DataFrame:
-    """
-    """
-    assert len(x0.shape) == 1 or x0.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
-    assert len(m0.shape) == 2, "The mapping table should be of two dimensions."
-    assert m0.shape[1] == 2, "The mapping table should be of two columns."
-    if isinstance(x0, pd.DataFrame):
-        pass
-    elif isinstance(x0, pd.Series):
-        x0 = pd.DataFrame(x0)
-    else:
-        raise Exception(f"""`x0` is of an unexpected type: "{type(x0)}".""")
-    fromColumn = x0.columns.to_list()[0]
-    toColumn = m0.columns.to_list()[1]
-    _ = toColumn
-
-    # Map values
-    x0 = pd.DataFrame(x0)  # To allow use of `set_index`
-    x1 = x0.set_index(fromColumn).join(other=m0.set_index(fromColumn),
-                                       how="inner",
-                                       lsuffix="_L",
-                                       rsuffix="_R")
-    return x1
-
-
-def determineMapTypeFromMap(x0: Union[pd.DataFrame, pd.Series],
-                            m0: pd.DataFrame,
-                            logger: Union[logging.Logger, None] = None,
-                            x1: Union[pd.DataFrame, pd.Series, None] = None) -> Literal["1:1", "m:1", "1:m"]:
-    """
-    """
-    if x1:
-        x1 = x1
-    elif isinstance(x1, type(None)):
-        x1 = _determineMapType_MapValues(x0=x0,
-                                         m0=m0)
-
-    # Count duplicates
-    mapType = determineMapType(x0=x0, x1=x1)
-
-    return mapType
+"""
+Compare two cohort (group) files.
+"""
+
+import logging
+from typing_extensions import (Literal,
+                               Union)
+# Third-party packages
+import pandas as pd
+
+
+def mappingAnalysis(x0: Union[pd.DataFrame, pd.Series], m0: pd.DataFrame, logger: logging.Logger, mappingMethod: Literal["inner", "outer"] = "inner") -> None:
+    """
+    # x0: The vector of input values
+    # m0: The matrix of mapping values, an n_m by 2 matrix
+    # x1: The vector of output values
+    """
+    assert len(x0.shape) == 1 or x0.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
+    assert len(m0.shape) == 2, "The mapping table should be of two dimensions."
+    assert m0.shape[1] == 2, "The mapping table should be of two columns."
+    if isinstance(x0, pd.DataFrame):
+        pass
+    elif isinstance(x0, pd.Series):
+        x0 = pd.DataFrame(x0)
+    else:
+        raise Exception(f"""`x0` is of an unexpected type: "{type(x0)}".""")
+    fromColumn = x0.columns.to_list()[0]
+    toColumn = m0.columns.to_list()[1]
+
+    mappingMethodsList = ["inner", "outer"]
+    x1 = {}
+    for mappingMethod in mappingMethodsList:
+        x1[mappingMethod] = x0.set_index(fromColumn).join(other=m0.set_index(fromColumn),
+                                                          how=mappingMethod,
+                                                          lsuffix="_L",
+                                                          rsuffix="_R")
+
+    lenx0 = len(x0)
+    lenx0unique = len(x0.drop_duplicates())
+    lenm0 = len(m0)
+    lenm0_1 = len(m0[fromColumn])
+    lenm0_2 = len(m0[toColumn])
+    lenm0_1unique = len(m0[fromColumn].drop_duplicates())
+    lenm0_2unique = len(m0[toColumn].drop_duplicates())
+    lenx1 = {}
+    lenx1unique = {}
+    for mappingMethod in mappingMethodsList:
+        lenx1[mappingMethod] = len(x1[mappingMethod])
+        lenx1unique[mappingMethod] = len(x1[mappingMethod].drop_duplicates())
+
+    logger.info(f"""The size of the input group is {lenx0:,}.""")
+    logger.info(f"""The size of the input group (unique values) is {lenx0unique:,}.""")
+    logger.info(f"""The size of the entire map is {lenm0:,}.""")
+    logger.info(f"""The size of the map's left side is {lenm0_1:,}.""")
+    logger.info(f"""The size of the map's right side is {lenm0_2:,}.""")
+    logger.info(f"""The size of the map's left side (unique values) is {lenm0_1unique:,}.""")
+    logger.info(f"""The size of the map's right side (unique values) is {lenm0_2unique:,}.""")
+    for mappingMethod in mappingMethodsList:
+        logger.info(f"""  Mapping values using method "{mappingMethod}".""")
+        logger.info(f"""    The size of the output group is {lenx1[mappingMethod]:,}.""")
+        logger.info(f"""    The size of the output group (unique values) is {lenx1unique[mappingMethod]:,}.""")
+
+
+def compareGroups(group1: Union[pd.DataFrame, pd.Series], group2: Union[pd.DataFrame, pd.Series], logger: logging.Logger) -> None:
+    """
+    """
+    assert len(group1.shape) == 1 or group1.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
+    assert len(group2.shape) == 1 or group2.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
+    if isinstance(group1, pd.DataFrame):
+        group1series = group1.iloc[:, 0]
+    else:
+        group1series = group1
+    if isinstance(group2, pd.DataFrame):
+        group2series = group2.iloc[:, 0]
+    else:
+        group2series = group2
+
+    c1l = len(group1series)
+    c2l = len(group2series)
+
+    c1inc2 = group1series.isin(group2series)
+    c2inc1 = group2series.isin(group1series)
+
+    c1inc2count = c1inc2.sum()
+    c2inc1count = c2inc1.sum()
+
+    c1inc2percent = c1inc2count / c1l
+    c2inc1percent = c2inc1count / c2l
+
+    intersection = set(group1series.to_list()).intersection(set(group2series.to_list()))
+    intersectionl = len(intersection)
+
+    logger.info("""The following results are of the set of groups 1 and 2. I.e., we are only counting the unique values.""")
+    logger.info(f"""Group 1 size: {c1l:,}.""")
+    logger.info(f"""Group 2 size: {c2l:,}.""")
+    logger.info(f"""Size of intersection of groups 1 and 2: {intersectionl:,}.""")
+    logger.info(f"""Percent of group 1 in group 2: {c1inc2percent:.2%}.""")
+    logger.info(f"""Percent of group 2 in group 1: {c2inc1percent:.2%}.""")
+
+
+def determineMapType(x0: Union[pd.DataFrame, pd.Series], x1: Union[pd.DataFrame, pd.Series]):
+    """
+    """
+    assert len(x0.shape) == 1 or x0.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
+    assert len(x1.shape) == 1 or x1.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
+
+    x0duplicated = x0.duplicated().sum() > 0
+    x1duplicated = x1.duplicated().sum() > 0
+
+    if x0duplicated and x1duplicated:
+        mapType = "m:m"
+    elif x0duplicated:
+        mapType = "m:1"
+    elif x1duplicated:
+        mapType = "1:m"
+    elif (not x0duplicated) & (not x1duplicated):
+        mapType = "1:1"
+    else:
+        raise Exception("Unexpected error.")
+
+    return mapType
+
+
+def _determineMapType_MapValues(x0: Union[pd.DataFrame, pd.Series],
+                                m0: pd.DataFrame) -> pd.DataFrame:
+    """
+    """
+    assert len(x0.shape) == 1 or x0.shape[1] == 1, "The input vector should be of one dimension or two dimensions with one column."
+    assert len(m0.shape) == 2, "The mapping table should be of two dimensions."
+    assert m0.shape[1] == 2, "The mapping table should be of two columns."
+    if isinstance(x0, pd.DataFrame):
+        pass
+    elif isinstance(x0, pd.Series):
+        x0 = pd.DataFrame(x0)
+    else:
+        raise Exception(f"""`x0` is of an unexpected type: "{type(x0)}".""")
+    fromColumn = x0.columns.to_list()[0]
+    toColumn = m0.columns.to_list()[1]
+    _ = toColumn
+
+    # Map values
+    x0 = pd.DataFrame(x0)  # To allow use of `set_index`
+    x1 = x0.set_index(fromColumn).join(other=m0.set_index(fromColumn),
+                                       how="inner",
+                                       lsuffix="_L",
+                                       rsuffix="_R")
+    return x1
+
+
+def determineMapTypeFromMap(x0: Union[pd.DataFrame, pd.Series],
+                            m0: pd.DataFrame,
+                            logger: Union[logging.Logger, None] = None,
+                            x1: Union[pd.DataFrame, pd.Series, None] = None) -> Literal["1:1", "m:1", "1:m"]:
+    """
+    """
+    if x1:
+        x1 = x1
+    elif isinstance(x1, type(None)):
+        x1 = _determineMapType_MapValues(x0=x0,
+                                         m0=m0)
+
+    # Count duplicates
+    mapType = determineMapType(x0=x0, x1=x1)
+
+    return mapType
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/constants/constants.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/constants/constants.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-"""
-Useful definitions used throughout IDR
-
-See the Notes portion for current IDR mapping standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Intermediate Results/Notes Portion/Data/Output/mapping
-See Noah's data request for my attempt at using these standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Concatenated Results/Code/makeMap.py
-"""
-from drapi.constants.phiVariables import LIST_OF_PHI_VARIABLES
-
-__all__ = ["DeIdIDName2DeIdIDSuffix",
-           "IDName2DeIdIDName",
-           "mapDtypes",
-           "DATA_TYPES_DICT"]
-
-IDName2DeIdIDNameRoot = {"ENCNTR_CSN_ID": "enc",
-                         "IDENT_ID_INT": "pat",
-                         "ORDR_PROC_ID": "order",
-                         "PATNT_KEY": "pat"}
-IDName2DeIdIDName = {IDName: f"deid_{DeIdIDNameRoot}_id" for IDName, DeIdIDNameRoot in IDName2DeIdIDNameRoot.items()}
-DeIdIDName2DeIdIDSuffix = {"pat": "PAT",
-                           "enc": "ENC",
-                           "note": "NOTE",
-                           "link_note": "LINK_NOTE",
-                           "order": "ORDER",
-                           "provider": "PROV"}
-mapDtypes = {0: int,
-             1: int,
-             2: str}
-
-# Define data types. NOTE that all the `String` variables contain numbers with leading zeros that get converted to integers in the current process. Either we convert these variables to `string` or we change the process.
-DATA_TYPES_BO = {"Acct Number - Enter DateTime Comb": "String",
-                 "Acct Number - Exit DateTime Comb": "String",
-                 "At Station": "String",
-                 "Authoring Provider Key": "Numeric",
-                 "Authorizing Provider Key": "Numeric",
-                 "Chemotherapy Rx Hosp Code Desc": "String",
-                 "Cosign Provider Key": "Numeric",
-                 "Diagnosis County": "String",
-                 "EPIC Patient ID": "String",
-                 "Encounter #": "Numeric",
-                 "Encounter # (CSN)": "Numeric",
-                 "Encounter # (Primary CSN)": "Numeric",
-                 "Encounter Key": "Numeric",
-                 "Encounter Key (Primary CSN)": "Numeric",
-                 "EncounterCSN": "Numeric",
-                 "Enterprise ID": "String",
-                 "From Station": "String",
-                 "F/u Physicians": "String",
-                 "Linkage Note ID": "Numeric",
-                 "Location of Svc": "String",
-                 "Location of Svc ID": "String",
-                 "Managing Physician": "String",
-                 "Medical Record Number": "Numeric",
-                 "MRN (Jax)": "Numeric",
-                 "MRN (UF)": "Numeric",
-                 "Note ID": "Numeric",
-                 "Note Key": "Numeric",
-                 "NRAS": "String",
-                 "Order ID": "Numeric",
-                 "Ordering Provider Key": "Numeric",
-                 "Order Key": "Numeric",
-                 "Provider Key": "Numeric",
-                 "Patient Encounter Key": "Numeric",
-                 "Patient Key": "Numeric",
-                 "PatientKey": "Numeric",
-                 "Patnt Key": "Numeric",
-                 "Prim  surgeon Code": "String",
-                 "Radiation Hosp Code Desc": "String",
-                 "Source Sys": "String",
-                 "Surgery Rx Hosp Code Desc": "String",
-                 "To Station": "String"}
-
-# Note that notes data are from the same source as BO data. These variable names are actually aliases and are here for convenience.
-DATA_TYPES_I2B2 = {"LOCATION_CD": "Numeric"}
-DATA_TYPES_NOTES = {"AuthoringProviderKey": "Numeric",
-                    "AuthorizingProviderKey": "Numeric",
-                    "ContactDate": "Datetime",
-                    "CosignProviderKey": "Numeric",
-                    "CreatedDatetime": "Datetime",
-                    "EncounterCSN": "Numeric",
-                    "EncounterDate": "Datetime",
-                    "EncounterKey": "Numeric",
-                    "LinkageNoteID": "Numeric",
-                    "MRN_GNV": "Numeric",
-                    "MRN_JAX": "Numeric",
-                    "NoteID": "Numeric",
-                    "NoteKey": "Numeric",
-                    "OrderID": "Numeric",
-                    "OrderKey": "Numeric",
-                    "OrderPlacedDatetime": "Datetime",
-                    "OrderResultDatetime": "Datetime",
-                    "OrderingProviderKey": "Numeric",
-                    "PatientKey": "Numeric",
-                    "ProviderKey": "Numeric",
-                    "ServiceDatetime": "Datetime"}
-
-DATA_TYPES_OMOP = {"care_site_id": "Numeric",
-                   "csn": "Numeric",
-                   "city": "String",
-                   "county": "String",
-                   "location_id": "Numeric",
-                   "observation_period_id": "Numeric",
-                   "patient_key": "Numeric",
-                   "person_id": "Numeric",
-                   "preceding_visit_occurrence_id": "Numeric",
-                   "provider_id": "Numeric",
-                   "visit_occurrence_id": "Numeric"}
-
-DATA_TYPES_DICT = DATA_TYPES_BO.copy()
-DATA_TYPES_DICT.update(DATA_TYPES_I2B2)
-DATA_TYPES_DICT.update(DATA_TYPES_NOTES)
-DATA_TYPES_DICT.update(DATA_TYPES_OMOP)
-
-DATA_TYPES_BY_PORTION = {"BO": DATA_TYPES_BO,
-                         "Notes": DATA_TYPES_NOTES,
-                         "OMOP": DATA_TYPES_OMOP}
-
-# Convert DRAPI data types to SQL data types
-DRAPI_TO_SQL_DATA_TYPES_MAP = {"Datetime": "TEXT",
-                               "Numeric": "INTEGER",
-                               "String": "TEXT"}
-DATA_TYPES_DICT_SQL = {name: DRAPI_TO_SQL_DATA_TYPES_MAP[drapiDataType] for name, drapiDataType in DATA_TYPES_DICT.items()}
-
-# QA: Make sure all PHI variables have their data type defined
-# assert all([varName in DATA_TYPES_DICT.keys() for varName in LIST_OF_PHI_VARIABLES])
-listOfMissingVariables = []
-for varName in LIST_OF_PHI_VARIABLES:
-    if varName not in DATA_TYPES_DICT.keys():
-        listOfMissingVariables.append(varName)
-if len(listOfMissingVariables) > 0:
-    text = "\n".join([f'"{varName}"' for varName in listOfMissingVariables])
-    raise Exception(f"Not all PHI variables have their data type defined: {text}")
+"""
+Useful definitions used throughout IDR
+
+See the Notes portion for current IDR mapping standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Intermediate Results/Notes Portion/Data/Output/mapping
+See Noah's data request for my attempt at using these standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Concatenated Results/Code/makeMap.py
+"""
+from drapi.constants.phiVariables import LIST_OF_PHI_VARIABLES
+
+__all__ = ["DeIdIDName2DeIdIDSuffix",
+           "IDName2DeIdIDName",
+           "mapDtypes",
+           "DATA_TYPES_DICT"]
+
+IDName2DeIdIDNameRoot = {"ENCNTR_CSN_ID": "enc",
+                         "IDENT_ID_INT": "pat",
+                         "ORDR_PROC_ID": "order",
+                         "PATNT_KEY": "pat"}
+IDName2DeIdIDName = {IDName: f"deid_{DeIdIDNameRoot}_id" for IDName, DeIdIDNameRoot in IDName2DeIdIDNameRoot.items()}
+DeIdIDName2DeIdIDSuffix = {"pat": "PAT",
+                           "enc": "ENC",
+                           "note": "NOTE",
+                           "link_note": "LINK_NOTE",
+                           "order": "ORDER",
+                           "provider": "PROV"}
+mapDtypes = {0: int,
+             1: int,
+             2: str}
+
+# Define data types. NOTE that all the `String` variables contain numbers with leading zeros that get converted to integers in the current process. Either we convert these variables to `string` or we change the process.
+DATA_TYPES_BO = {"Acct Number - Enter DateTime Comb": "String",
+                 "Acct Number - Exit DateTime Comb": "String",
+                 "At Station": "String",
+                 "Authoring Provider Key": "Numeric",
+                 "Authorizing Provider Key": "Numeric",
+                 "Chemotherapy Rx Hosp Code Desc": "String",
+                 "Cosign Provider Key": "Numeric",
+                 "Diagnosis County": "String",
+                 "EPIC Patient ID": "String",
+                 "Encounter #": "Numeric",
+                 "Encounter # (CSN)": "Numeric",
+                 "Encounter # (Primary CSN)": "Numeric",
+                 "Encounter Key": "Numeric",
+                 "Encounter Key (Primary CSN)": "Numeric",
+                 "EncounterCSN": "Numeric",
+                 "Enterprise ID": "String",
+                 "From Station": "String",
+                 "F/u Physicians": "String",
+                 "Linkage Note ID": "Numeric",
+                 "Location of Svc": "String",
+                 "Location of Svc ID": "String",
+                 "Managing Physician": "String",
+                 "Medical Record Number": "Numeric",
+                 "MRN (Jax)": "Numeric",
+                 "MRN (UF)": "Numeric",
+                 "Note ID": "Numeric",
+                 "Note Key": "Numeric",
+                 "NRAS": "String",
+                 "Order ID": "Numeric",
+                 "Ordering Provider Key": "Numeric",
+                 "Order Key": "Numeric",
+                 "Provider Key": "Numeric",
+                 "Patient Encounter Key": "Numeric",
+                 "Patient Key": "Numeric",
+                 "PatientKey": "Numeric",
+                 "Patnt Key": "Numeric",
+                 "Prim  surgeon Code": "String",
+                 "Radiation Hosp Code Desc": "String",
+                 "Source Sys": "String",
+                 "Surgery Rx Hosp Code Desc": "String",
+                 "To Station": "String"}
+
+# Note that notes data are from the same source as BO data. These variable names are actually aliases and are here for convenience.
+DATA_TYPES_I2B2 = {"LOCATION_CD": "Numeric"}
+DATA_TYPES_NOTES = {"AuthoringProviderKey": "Numeric",
+                    "AuthorizingProviderKey": "Numeric",
+                    "ContactDate": "Datetime",
+                    "CosignProviderKey": "Numeric",
+                    "CreatedDatetime": "Datetime",
+                    "EncounterCSN": "Numeric",
+                    "EncounterDate": "Datetime",
+                    "EncounterKey": "Numeric",
+                    "LinkageNoteID": "Numeric",
+                    "MRN_GNV": "Numeric",
+                    "MRN_JAX": "Numeric",
+                    "NoteID": "Numeric",
+                    "NoteKey": "Numeric",
+                    "OrderID": "Numeric",
+                    "OrderKey": "Numeric",
+                    "OrderPlacedDatetime": "Datetime",
+                    "OrderResultDatetime": "Datetime",
+                    "OrderingProviderKey": "Numeric",
+                    "PatientKey": "Numeric",
+                    "ProviderKey": "Numeric",
+                    "ServiceDatetime": "Datetime"}
+
+DATA_TYPES_OMOP = {"care_site_id": "Numeric",
+                   "csn": "Numeric",
+                   "city": "String",
+                   "county": "String",
+                   "location_id": "Numeric",
+                   "observation_period_id": "Numeric",
+                   "patient_key": "Numeric",
+                   "person_id": "Numeric",
+                   "preceding_visit_occurrence_id": "Numeric",
+                   "provider_id": "Numeric",
+                   "visit_occurrence_id": "Numeric"}
+
+DATA_TYPES_DICT = DATA_TYPES_BO.copy()
+DATA_TYPES_DICT.update(DATA_TYPES_I2B2)
+DATA_TYPES_DICT.update(DATA_TYPES_NOTES)
+DATA_TYPES_DICT.update(DATA_TYPES_OMOP)
+
+DATA_TYPES_BY_PORTION = {"BO": DATA_TYPES_BO,
+                         "Notes": DATA_TYPES_NOTES,
+                         "OMOP": DATA_TYPES_OMOP}
+
+# Convert DRAPI data types to SQL data types
+DRAPI_TO_SQL_DATA_TYPES_MAP = {"Datetime": "TEXT",
+                               "Numeric": "INTEGER",
+                               "String": "TEXT"}
+DATA_TYPES_DICT_SQL = {name: DRAPI_TO_SQL_DATA_TYPES_MAP[drapiDataType] for name, drapiDataType in DATA_TYPES_DICT.items()}
+
+# QA: Make sure all PHI variables have their data type defined
+# assert all([varName in DATA_TYPES_DICT.keys() for varName in LIST_OF_PHI_VARIABLES])
+listOfMissingVariables = []
+for varName in LIST_OF_PHI_VARIABLES:
+    if varName not in DATA_TYPES_DICT.keys():
+        listOfMissingVariables.append(varName)
+if len(listOfMissingVariables) > 0:
+    text = "\n".join([f'"{varName}"' for varName in listOfMissingVariables])
+    raise Exception(f"Not all PHI variables have their data type defined: {text}")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/constants/phiValues.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiValues.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/constants/phiVariables.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiVariables.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/drapi.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/drapi.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,755 +1,755 @@
-"""
-Utility functions commonly used in IDR data request projects.
-"""
-
-import datetime as dt
-import logging
-import os
-import re
-from array import array
-from collections.abc import Collection
-from datetime import datetime
-from datetime import date
-from datetime import time
-from dateutil.parser import parse
-from itertools import islice
-from logging import Logger
-from pathlib import Path
-from typing import Callable, List, Tuple, Union
-from typing_extensions import Literal
-import sys
-# Third-party packages
-import numpy as np
-import pandas as pd
-import sqlalchemy as sa
-import sqlite3
-from pandas.io.parsers.readers import TextFileReader
-# Local packages
-pass
-
-logger = logging.getLogger(__name__)
-
-# SQL Server settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = fr"{USERDOMAIN}\{USERNAME}"
-PWD = os.environ["HFA_UFADPWD"]
-
-# SQLAlchemy connections
-conStr = f"mssql+pymssql://{UID}:{PWD}@{SERVER}/{DATABASE}"  # Create connection string
-engine = sa.create_engine(conStr)  # Make connection/engine
-
-
-class StreamToLogger(object):
-    """
-    Fake file-like stream object that redirects writes to a logger instance.
-    h/t to https://stackoverflow.com/a/39215961/5478086
-    """
-
-    def __init__(self, logger, level):
-        self.logger = logger
-        self.level = level
-        self.linebuf = ''
-
-    def write(self, buf):
-        for line in buf.rstrip().splitlines():
-            self.logger.log(self.level, line.rstrip())
-
-    def flush(self):
-        pass
-
-
-class LoggerWriter:
-    """
-    h/t to https://stackoverflow.com/a/31688396/5478086
-    """
-
-    def __init__(self, level):
-        self.level = level
-
-    def write(self, message):
-        if message != '\n':
-            self.level(message)
-
-    def flush(self):
-        self.level(sys.stderr)
-
-
-def makeDirPath(directory_path: str) -> None:
-    """
-    Check if all directories exists in a path. If not, create them
-    """
-    path_obj = Path(directory_path)
-    paths = list(path_obj.parents)[::-1] + [path_obj]
-    for dir in paths:
-        if not os.path.exists(dir):
-            os.mkdir(dir)
-
-
-def getTimestamp():
-    return dt.datetime.now().strftime("%Y-%m-%d %H-%M-%S")
-
-
-def getPercentDifference(x, y):
-    """
-    Calculates a percentage if the denominator is not 0, else it returns `"N/A"`.
-    """
-    if y != 0:
-        return f"{x / y: 0.2%}"
-    else:
-        return "N/A"
-
-
-def flatExtend(iterable: Collection) -> list:
-    """
-    Creates a list from an iterable.
-    """
-    outputList = []
-    for el in iterable:
-        outputList.extend(el)
-    return outputList
-
-
-def readDataFile(fname: Path, *args, **kwargs) -> TextFileReader:
-    """
-    Opens a file based on the file extension of its file name `fname` using a Pandas built-in to return a DataFrame object. Below is the list of Pandas built-ins, whose odcumentation you can search to find out what keyword arguments (`kwargs`) to use.
-      - `pd.read_csv`
-      - `pd.read_json`
-      - `pd.read_xml`
-      - `pd.read_excel`
-      - `pd.read_hdf`
-      - `pd.read_sql`
-    """
-    suffix = fname.suffix.lower()
-    if suffix.endswith(('.csv',)):
-        TextFileReaderObject = pd.read_csv(fname, *args, **kwargs)
-    elif suffix.endswith(('.tsv',)):
-        kwargs["delimiter"] = "\t"
-        TextFileReaderObject = pd.read_csv(fname, *args, **kwargs)
-    elif suffix.endswith(('.json',)):
-        TextFileReaderObject = pd.read_json(fname, *args, **kwargs)
-    elif suffix.endswith(('.xml',)):
-        TextFileReaderObject = pd.read_xml(fname, *args, **kwargs)
-    elif suffix.endswith(('.xls', 'xlsx',)):
-        TextFileReaderObject = pd.read_excel(fname, *args, **kwargs)
-    elif suffix.endswith(('.hdf',)):
-        TextFileReaderObject = pd.read_hdf(fname, *args, **kwargs)
-    elif suffix.endswith(('.sql',)):
-        TextFileReaderObject = pd.read_sql(fname, *args, **kwargs)
-    else:
-        raise ValueError(f"""Unsupported filetype for file "{fname}".""")
-    return TextFileReaderObject
-
-
-def successiveParents(pathObj: Path, numLevels: int) -> Tuple[Path, int]:
-    """
-    Successively get the parents of the Path object submitted.
-    """
-    while numLevels > 0:
-        pathObj = pathObj.parent
-        numLevels -= 1
-    return pathObj, numLevels
-
-
-def fileContainsColumn(pathObj: Path, listOfColumns: list) -> bool:
-    """
-    Determines if the file defined by `pathObj` has any of the columns contained in `listOfColumns`.
-    """
-    condition = False
-    df = pd.read_csv(pathObj, nrows=10)
-    columns = df.columns
-    for columnName in listOfColumns:
-        if columnName in columns:
-            condition = True
-            break
-        else:
-            continue
-    return condition
-
-
-def getCommonDirectoryParent(primaryPath: Path, secondaryPath: Path) -> Path:
-    """
-    """
-    commonPrefix = os.path.commonprefix([primaryPath, secondaryPath])
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        if commonPrefix == "/":
-            pathResult = primaryPath
-        else:
-            pathResult = primaryPath.absolute().relative_to(secondaryPath)
-    elif operatingSystem == "win32":
-        if commonPrefix == "":
-            pathResult = primaryPath
-        else:
-            pathResult = primaryPath.absolute().relative_to(secondaryPath)
-    return pathResult
-
-
-def getFilesToRelease(filesToRelease: List[Path], fileCriteria: List[Callable]):
-    """
-    Applies the functions in the iterable `fileCriteria` to each Path object in `filesToRelease`.
-    """
-    filesToRelease = []
-    for file in filesToRelease:
-        criteria = []
-        for criteriaFunc in fileCriteria:
-            criteria.append(criteriaFunc(file))
-        criteriaMet = all(criteria)
-        if criteriaMet:
-            filesToRelease.append(file)
-        else:
-            pass
-
-
-def getLastIDNum(df, columnName="deid_num"):
-    """
-    Gets the last ID number in a de-identification map.
-    """
-    numbers = df[columnName].astype(int)
-    return max(numbers)
-
-
-def isNumber(string):
-    """
-    Checks if the string represents a number
-
-    For a discussion see https://stackoverflow.com/questions/354038/how-do-i-check-if-a-string-represents-a-number-float-or-int
-    """
-    try:
-        int(float(string))
-        return True
-    except ValueError as error:
-        msg = error.args[0]
-        if "invalid literal for int() with base 10:" in msg:  # This must be an old Python exception message
-            return False
-        elif "could not convert string to float:" in msg:  # I think this is the new exception message
-            return False
-        else:
-            raise Exception(error)
-
-
-def fileName2variableName(pathObj):
-    """
-    """
-    pattern = r"^(?P<variableName>.+) map"
-    string = pathObj.stem
-    obj = re.match(pattern, string)
-    if obj:
-        groupDict = obj.groupdict()
-        variableName = groupDict["variableName"]
-    else:
-        raise Exception("This file path objected was of an unexpected format.")
-    return variableName
-
-
-def mapGroupCriteria4unknownValue(value):
-    """
-    Checks if `value` is a number. If so, it checks if it's less than 0. If it's not a number, return `True`.
-
-    This is used in making de-identification maps, where negative ID values are usually used to represent unknown or null values.
-    """
-    if isNumber(value):
-        return float(value) < 0
-    else:
-        return False
-
-
-def makeMap(IDset: set,
-            IDName: str,
-            startFrom: Union[int, list],
-            irbNumber: str,
-            suffix: str,
-            columnSuffix: str,
-            logger: Logger,
-            groups: dict = {0: {"criteria": [mapGroupCriteria4unknownValue],
-                                "deidNum": 0}},
-            deIdentificationMapStyle: Literal["classic", "lemur"] = "lemur") -> pd.DataFrame:
-    """
-    Makes an IDR de-identification map.
-
-    INPUT
-        `IDset`, a set of IDs
-        `IDName`, the name of the ID
-        `startFrom`, the integer number to start from
-        `groups`, ID values to group or map in a many-to-one fashion. E.g., invalid IDs (negative numbers) are usually all mapped to the same de-identified number, like "0".
-        `deIdentificationMapStyle`, a string, one of {"classic, "lemur"}. The formats are as follow:
-            | Format Style  | de-Identififed ID Column Header   |
-            | ------------- | -------------------------------   |
-            | "clasic"      | `f"deid_{columnSuffix}_id"`       |
-            | "lemur"       | `f"de-Identified {IDName}"`       |
-
-    OUTPUT
-        `map_`, a Pandas DataFrame with the following format:
-        | `IDName` | deid_num   | de-Identififed ID Column Header |
-        | -------- | --------   | ------------------------ |
-        | IDset[0] | numbers[0] | ... |
-        | ...      | ...        | ... |
-    """
-    # QA: `irbNumber` must not be NoneType
-    if isinstance(irbNumber, type(None)):
-        raise Exception("""`irbNumber` cannot be of type "None".""")
-
-    # Assign header formats: de-Identififed ID Column Header
-    if deIdentificationMapStyle == "classic":
-        deIdentificationSerialNumberHeader = "deid_num"
-    elif deIdentificationMapStyle == "lemur":
-        deIdentificationSerialNumberHeader = "De-identification Serial Number"
-
-    # Assign header formats: de-Identififed ID Column Header
-    if deIdentificationMapStyle == "classic":
-        deIdentifiedIDColumnHeader = f"deid_{columnSuffix}_id"
-    elif deIdentificationMapStyle == "lemur":
-        deIdentifiedIDColumnHeader = f"De-identified {IDName}"
-
-    if len(IDset) == 0:
-        return pd.DataFrame(columns=[IDName,
-                                     deIdentificationSerialNumberHeader,
-                                     deIdentifiedIDColumnHeader])
-    else:
-        pass
-    if isinstance(startFrom, int):
-        startFrom = startFrom
-        numbers = list(range(startFrom, startFrom + len(IDset)))
-    elif isinstance(startFrom, list):
-        numbers = startFrom[:]
-        startFrom = numbers[0]
-    numbers.extend([None])
-    logger.info("    Sorting `IDset`.")
-    IDli = sortIntegersAndStrings(list(IDset))
-    logger.info("    Sorting `IDset` - done.")
-    logger.info("    Creating `mapDi`.")
-    mapDi = {IDNum: {} for IDNum in IDli}
-    logger.info("    Creating `mapDi` - done.")
-    lenIDli = len(IDli)
-    if lenIDli > 100000:
-        itChunk = 1000
-    else:
-        itChunk = max(round(lenIDli / 50), 1)
-    for it, IDNum in enumerate(IDli, start=1):
-        fromGroup = False
-        for group, groupAttributes in groups.items():
-            criteriaList = groupAttributes["criteria"]
-            criteria = [criterion(IDNum) for criterion in criteriaList]
-            if all(criteria):
-                deid_num = groupAttributes["deidNum"]
-                fromGroup = True
-                break
-        if fromGroup:
-            pass
-        else:
-            deid_num = numbers.pop(0)
-        deid_id = f"{irbNumber}_{suffix}_{deid_num}"
-        mapDi[IDNum] = {IDName: IDNum,
-                        deIdentificationSerialNumberHeader: deid_num,
-                        deIdentifiedIDColumnHeader: deid_id}
-        if it % itChunk == 0:
-            logger.info(f"  ..  Working on item {it:,} of {len(IDli):,} ({it/lenIDli:.2%} done).")
-    newMap = pd.DataFrame.from_dict(mapDi, orient="index")
-    newMap.index = range(1, len(newMap) + 1)
-    return newMap
-
-
-def makeSetComplement(set1, cardinalityOfNewSet):
-    """
-    Creates a complement to a set, based on the specified size of the complement. Elements of the first set are assumed to be integers from 1 and above, and cardinalities are non-zero positive integers.
-
-    TODO: Implement empty set handling
-    """
-    set1Min = 1
-    if len(set1) == 0:
-        raise ValueError("Set should not be empty.")
-    else:
-        set1Max = max(set1)
-    s1Contiguous = set(range(set1Min, set1Max + 1))
-    setDifference = s1Contiguous.difference(set1)
-    cardinalityOfSetDifference = len(setDifference)
-    cardinalityOfContiguousSubset = cardinalityOfNewSet - cardinalityOfSetDifference
-    if cardinalityOfContiguousSubset > 0:
-        setDifferenceSubset = setDifference
-        contiguousSubset = set(range(set1Max + 1, set1Max + cardinalityOfContiguousSubset + 1))
-    elif cardinalityOfContiguousSubset == 0:
-        setDifferenceSubset = setDifference
-        contiguousSubset = set()
-    elif cardinalityOfContiguousSubset < 0:
-        setDifferenceSubset = set(list(setDifference)[:cardinalityOfNewSet])
-        contiguousSubset = set()
-    newSet = setDifferenceSubset.union(contiguousSubset)
-    return newSet
-
-
-def loglevel2int(loglevel: Union[int, str]) -> int:
-    """
-    An agnostic converter that takes int or str and returns int. If input is int, output is the same as input"""
-    dummy = logging.getLogger("dummy")
-    dummy.setLevel(loglevel)
-    loglevel = dummy.level
-    return loglevel
-
-
-def replace_sql_query(query: str, old: str, new: str, loglevel: Union[int, str] = "INFO") -> str:
-    """
-    Replaces text in a SQL query only if it's not commented out. I.e., this function applies string.replace() only if the string doesn't begin with "--".
-    TODO Don't replace text after "--".
-    """
-    loglevel_asnumber = loglevel2int(loglevel)
-    logger.setLevel(loglevel_asnumber + 10)
-
-    pattern = r"^\w*--"
-    li = query.split("\n")
-    result = []
-    logger.debug("Starting")
-    for line in li:
-        logger.debug(f"""  Working on "{line}".""")
-        obj = re.search(pattern, line)
-        if obj:
-            logger.debug("    Passing")
-            nline = line
-        else:
-            nline = line.replace(old, new)
-            logger.debug(f"""    Replacing text in "{line}" --> "{nline}".""")
-        logger.debug("  Appending...")
-        result.append(nline)
-    logger.debug("Finished")
-    return "\n".join(result)
-
-
-def sqlite2df(tableContents: list, tableName: str, cursor: sqlite3.Cursor) -> pd.DataFrame:
-    """
-    `tableContents` must be a "*" query where all the columns are returned.
-    """
-    # Get metadata on table
-    query = f"PRAGMA table_info({tableName});"
-    cursor.execute(query)
-    query_results = cursor.fetchall()
-    column_header = [tu[1] for tu in query_results]
-
-    tableContents_asDict = {}
-    for it, table_info in enumerate(tableContents):
-        di = {}
-        for key, value in zip(column_header, table_info):
-            di[key] = value
-        tableContents_asDict[it] = di
-    df = pd.DataFrame.from_dict(tableContents_asDict, orient="index")
-    df.index = range(1, len(tableContents) + 1)
-    return df
-
-
-def patient_key_from_person_id(person_id: int, map_: dict = {}) -> Tuple[int, Literal[0, 1]]:
-    """
-    Assumes "map_" is a dictionary with person IDs as integers that map patient keys as integers.
-    """
-    if person_id in map_.keys():
-        patient_key = map_[person_id]
-        source = 0
-    else:
-        query = f"""use DWS_OMOP_PROD
-        SELECT
-            xref.PERSON_MAPPING.person_id as person_id,
-            xref.PERSON_MAPPING.patient_key as patient_key
-        FROM
-            xref.PERSON_MAPPING
-        WHERE
-            xref.PERSON_MAPPING.person_id IN ({person_id})"""
-        results = pd.read_sql(query, con=conStr)
-        person_id = results["person_id"][0]
-        patient_key = results["patient_key"][0]
-        source = 1
-    return patient_key, source
-
-
-def personIDs2patientKeys(personIDList: List[int]) -> pd.DataFrame:
-    """
-
-    """
-    list2str = ",".join([str(num) for num in personIDList])
-    query = f"""use DWS_OMOP_PROD
-    SELECT
-        xref.PERSON_MAPPING.person_id as person_id,
-        xref.PERSON_MAPPING.patient_key as patient_key
-    FROM
-        xref.PERSON_MAPPING
-    WHERE
-        xref.PERSON_MAPPING.person_id IN ({list2str})"""
-    results = pd.read_sql(query, con=conStr)
-    return results
-
-
-def epicID2patientKey(epicIDlist: List[str]) -> pd.DataFrame:
-    """
-    Executes a SQL query to map EPIC Patient IDs to Patient Keys.
-    """
-    IDsAsString = ",".join([f"'{el}'" for el in epicIDlist])
-    query = f"""USE DWS_PROD
-    SELECT
-        dbo.ALL_PATIENTS.PATNT_KEY AS 'Patient Key',
-        dbo.ALL_PATIENTS.PATNT_ID AS 'EPIC Patient ID'
-    FROM
-        dbo.ALL_PATIENTS
-    WHERE
-        (
-        dbo.ALL_PATIENTS.PATNT_ID  IN  ( {IDsAsString}  )
-        AND
-        ( dbo.ALL_PATIENTS.TEST_IND='N'  )
-        )"""
-    results = pd.read_sql(query, con=conStr)
-    return results
-
-
-def map2di(map_: pd.DataFrame, fromColumnIndex: int = 0, toColumnIndex: int = 2) -> dict:
-    """
-    `fromColumnIndex` is the variable to assign as the key to the dictionary.
-    `toColumnIndex` is the variable to assign as the value pair in the dictionary.
-    Assumes the following structure to "map_":
-    column 1      | column 2       | column 3      | ... | column k
-        x_(1,1)   |     x_(1,2)    |    x_(1,3)    | ... |   x_(1,k)
-        .         |     .          |     .         | ... |   .
-        .         |     .          |     .         | ... |   .
-        .         |     .          |     .         | ... |   .
-        x_(n,1)   |     x_(n,2)    |    x_(n,3)    | ... |   x_(n,k)
-    Where the columns are from 1, 2, 3, ..., i, ..., k-1, k, and the rows are from 1, 2, 3, ..., j, ..., n-1, n.
-    """
-    di = {}
-    errors = []
-    for _, row in map_.iterrows():
-        oldValue = row.values[fromColumnIndex]
-        newValue = row.values[toColumnIndex]
-        if oldValue in di.keys() and di[oldValue] != newValue:
-            errors.append({oldValue: newValue})
-        di[oldValue] = newValue
-    if len(errors) > 0:
-        raise Exception(f"This map is not one to one. At least one ID is duplicated with multiple de-identified IDs: {errors}")
-    else:
-        return di
-
-
-def float2str(value: float, navalue="") -> str:
-    """
-    Converts values to string-type. If a value is NaN it is replaced with a value that can be converted to a string, default empty string, "".
-    """
-    assert isinstance(navalue, str), """"navalue" is not a string type."""
-    if pd.isna(value):
-        newValue = str(navalue)
-    else:
-        newValue = str(int(value))
-    return newValue
-
-
-def numericOrString2integerOrString(value) -> Union[str, int]:
-    """
-    Determines if a value is numeric or string. If numeric, convert to an integer, else return as string.
-
-    Used by `makeMapsFromOthers.py`
-    """
-    if isNumber(value):
-        return int(float(value))
-    else:
-        return str(value)
-
-
-def sortIntegersAndStrings(li: list) -> list:
-    """
-    Sorts a list of integers and strings by sorted them separately and then concatenating the results.
-    """
-    series = pd.Series(li)
-    maskIntegers = series.apply(lambda el: isinstance(el, int))
-    maskStrings = series.apply(lambda el: isinstance(el, str))
-    li2 = sorted(series[maskIntegers].to_list()) + sorted(series[maskStrings].to_list())
-    return li2
-
-
-def str2int(value, navalue=-1):
-    """
-    Converts values to integer-type. If a value is NaN it is replaced with a value that can be converted to an integer, default is "-1".
-    """
-    assert isinstance(navalue, int), """"navalue" is not an integer type."""
-    if pd.isna(value):
-        newValue = int(navalue)
-    else:
-        newValue = int(float(value))
-    return newValue
-
-
-def str2intOr0(string):
-    """
-    Converts a string to its numeric value, or 0, if it has no numeric value.
-    """
-    if string.isnumeric():
-        return int(string)
-    else:
-        return 0
-
-
-def str2bool(value, navalue=""):
-    """
-    Converts values to boolean-type. If a value is missing it is replaced with an empty string.
-    """
-    if pd.isna(value):
-        newValue = int(navalue)
-    else:
-        newValue = bool(value)
-    return newValue
-
-
-def deconstructStudyID(string):
-    """
-    Deconstructs a de-identified study ID into its component parts, assuming the following format: STUDY-TYPESTUDY-NUMBER_SERIAL-NUMBER
-    Where "STUDY_TYPE" is the study type, e.g., "CED", "IRB", or "WIRB"
-          "STUDY-NUMBER" is the study serial number, usually a 9-digit number where the first four numbers is a four-digit year.
-          "SERIAL-NUMBER" is the de-identified study-specific serial number of a patient or other subject.
-    For example: "IRB202300123_222"
-    """
-    pattern = r"(?P<studyType>\w+)(?P<studyNumber>\d{9})_(?P<PHI_type>\w+)_(?P<deIdentificationNumber>\d+)"
-    regexObj = re.search(pattern, string)
-    if regexObj:
-        di = regexObj.groupdict()
-        return di
-    else:
-        raise Exception("String is of an unexpected format. See function docstring for expected format.")
-
-
-def studyID2tuple(string):
-    """
-    Extracts the numeric portion of a string.
-
-    Assumes the following format: STUDY-TYPESTUDY-NUMBER_SERIAL-NUMBER
-    Where "STUDY_TYPE" is the study type, e.g., "CED", "IRB", or "WIRB"
-          "STUDY-NUMBER" is the study serial number, usually a 9-digit number where the first four numbers is a four-digit year.
-          "SERIAL-NUMBER" is the de-identified study-specific serial number of a patient or other subject.
-    For example: "IRB202300123_222"
-
-    This is intended for use when sorting columns by the numeric value of the string, and not the text value.
-    """
-    di = deconstructStudyID(string)
-    studyType = di["studyType"]
-    studyNumber = int(di["studyNumber"])
-    PHI_type = di["PHI_type"]
-    deIdentificationNumber = int(di["deIdentificationNumber"])
-    tu = studyType, studyNumber, PHI_type, deIdentificationNumber
-    return tu
-
-
-def isValidPatientID(value):
-    """
-    Checks if the value is a valid UFHealth patient ID. Invalid patient IDs are defined as negative integers
-    """
-    isNumber_bool = isNumber(value)
-    if isNumber_bool:
-        number = int(value)
-        if number < 0:
-            result = False
-        elif number >= 0:  # Assumes `0` is a valid patient ID
-            result = True
-    elif not isNumber_bool:
-        result = True  # Assumes all non-numeric IDs are valid
-    return result
-
-
-def isDatetime(string):
-    """
-    Checks if a string contains a datetime format.
-    """
-    try:
-        _ = parse(string, fuzzy=False)
-        return True
-    except ValueError:
-        return False
-
-
-def ditchFloat(value):
-    """
-    Gets rid of float types if value is string, integer, float, or datetime
-    """
-    if isinstance(value, str):
-        value = str(value)
-        if value.isnumeric():
-            standardValue = int(value)
-        elif isNumber(value):
-            standardValue = int(float(value))
-        elif isDatetime(value):
-            standardValue = parse(value, fuzzy=False)
-        else:
-            raise ValueError(f"""Unexpected format in string value "{value}". We expected a string with a number, numeric, or datetime format.""")
-    elif isinstance(value, int) or isinstance(value, np.integer) or isinstance(value, float):
-        standardValue = int(value)
-    else:
-        raise ValueError(f"""Unexpected data type "{type(value)}" for value "{value}". Expect only string, float, or integers.""")
-    return standardValue
-
-
-def handleDatetimeForJson(obj):
-    """
-    JSON serializer for objects not serializable by default json code
-
-    h/t to https://stackoverflow.com/a/22238613/5478086
-    """
-    if isinstance(obj, (datetime, date, time)):
-        return obj.isoformat()
-    raise TypeError(f"Type {type(obj)} not serializable")
-
-
-def makeChunks(array_range: array, chunkSize: int) -> tuple:
-    """
-    Inspired by GeekForGeeks.com (https://www.geeksforgeeks.org/break-list-chunks-size-n-python/)
-
-    Only makes chunks of one dimensional arrays (e.g., lists, Pandas Series), but not dataframes.
-
-    Example:
-    array = range(30)
-    chunks = makeChunks(array, chunkSize)
-    """
-    array_range = iter(array_range)
-    return iter(lambda: tuple(islice(array_range, chunkSize)), ())
-
-
-# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
-# >>> tree function >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
-# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
-# h/t https://stackoverflow.com/a/59109706/5478086
-
-
-def tree(dir_path: Path, level: int = -1, limit_to_directories: bool = False,
-         length_limit: int = 1000):
-    """Given a directory Path object print a visual tree structure"""
-    # prefix components:
-    space = '    '
-    branch = '│   '
-    # pointers:
-    tee = '├── '
-    last = '└── '
-
-    dir_path = Path(dir_path)  # accept string coerceable to Path
-    files = 0
-    directories = 0
-
-    def inner(dir_path: Path, prefix: str = '', level=-1):
-        nonlocal files, directories
-        if not level:
-            return  # 0, stop iterating
-        if limit_to_directories:
-            contents = [d for d in dir_path.iterdir() if d.is_dir()]
-        else:
-            contents = list(dir_path.iterdir())
-        pointers = [tee] * (len(contents) - 1) + [last]
-        for pointer, path in zip(pointers, contents):
-            if path.is_dir():
-                yield prefix + pointer + path.name
-                directories += 1
-                extension = branch if pointer == tee else space
-                yield from inner(path, prefix=prefix + extension, level=level - 1)
-            elif not limit_to_directories:
-                yield prefix + pointer + path.name
-                files += 1
-    print(dir_path.name)
-    iterator = inner(dir_path, level=level)
-    for line in islice(iterator, length_limit):
-        print(line)
-    if next(iterator, None):
-        print(f'... length_limit, {length_limit}, reached, counted:')
-    print(f'\n{directories} directories' + (f', {files} files' if files else ''))
-
-
-# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
-# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
-# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+"""
+Utility functions commonly used in IDR data request projects.
+"""
+
+import datetime as dt
+import logging
+import os
+import re
+from array import array
+from collections.abc import Collection
+from datetime import datetime
+from datetime import date
+from datetime import time
+from dateutil.parser import parse
+from itertools import islice
+from logging import Logger
+from pathlib import Path
+from typing import Callable, List, Tuple, Union
+from typing_extensions import Literal
+import sys
+# Third-party packages
+import numpy as np
+import pandas as pd
+import sqlalchemy as sa
+import sqlite3
+from pandas.io.parsers.readers import TextFileReader
+# Local packages
+pass
+
+logger = logging.getLogger(__name__)
+
+# SQL Server settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = fr"{USERDOMAIN}\{USERNAME}"
+PWD = os.environ["HFA_UFADPWD"]
+
+# SQLAlchemy connections
+conStr = f"mssql+pymssql://{UID}:{PWD}@{SERVER}/{DATABASE}"  # Create connection string
+engine = sa.create_engine(conStr)  # Make connection/engine
+
+
+class StreamToLogger(object):
+    """
+    Fake file-like stream object that redirects writes to a logger instance.
+    h/t to https://stackoverflow.com/a/39215961/5478086
+    """
+
+    def __init__(self, logger, level):
+        self.logger = logger
+        self.level = level
+        self.linebuf = ''
+
+    def write(self, buf):
+        for line in buf.rstrip().splitlines():
+            self.logger.log(self.level, line.rstrip())
+
+    def flush(self):
+        pass
+
+
+class LoggerWriter:
+    """
+    h/t to https://stackoverflow.com/a/31688396/5478086
+    """
+
+    def __init__(self, level):
+        self.level = level
+
+    def write(self, message):
+        if message != '\n':
+            self.level(message)
+
+    def flush(self):
+        self.level(sys.stderr)
+
+
+def makeDirPath(directory_path: str) -> None:
+    """
+    Check if all directories exists in a path. If not, create them
+    """
+    path_obj = Path(directory_path)
+    paths = list(path_obj.parents)[::-1] + [path_obj]
+    for dir in paths:
+        if not os.path.exists(dir):
+            os.mkdir(dir)
+
+
+def getTimestamp():
+    return dt.datetime.now().strftime("%Y-%m-%d %H-%M-%S")
+
+
+def getPercentDifference(x, y):
+    """
+    Calculates a percentage if the denominator is not 0, else it returns `"N/A"`.
+    """
+    if y != 0:
+        return f"{x / y: 0.2%}"
+    else:
+        return "N/A"
+
+
+def flatExtend(iterable: Collection) -> list:
+    """
+    Creates a list from an iterable.
+    """
+    outputList = []
+    for el in iterable:
+        outputList.extend(el)
+    return outputList
+
+
+def readDataFile(fname: Path, *args, **kwargs) -> TextFileReader:
+    """
+    Opens a file based on the file extension of its file name `fname` using a Pandas built-in to return a DataFrame object. Below is the list of Pandas built-ins, whose odcumentation you can search to find out what keyword arguments (`kwargs`) to use.
+      - `pd.read_csv`
+      - `pd.read_json`
+      - `pd.read_xml`
+      - `pd.read_excel`
+      - `pd.read_hdf`
+      - `pd.read_sql`
+    """
+    suffix = fname.suffix.lower()
+    if suffix.endswith(('.csv',)):
+        TextFileReaderObject = pd.read_csv(fname, *args, **kwargs)
+    elif suffix.endswith(('.tsv',)):
+        kwargs["delimiter"] = "\t"
+        TextFileReaderObject = pd.read_csv(fname, *args, **kwargs)
+    elif suffix.endswith(('.json',)):
+        TextFileReaderObject = pd.read_json(fname, *args, **kwargs)
+    elif suffix.endswith(('.xml',)):
+        TextFileReaderObject = pd.read_xml(fname, *args, **kwargs)
+    elif suffix.endswith(('.xls', 'xlsx',)):
+        TextFileReaderObject = pd.read_excel(fname, *args, **kwargs)
+    elif suffix.endswith(('.hdf',)):
+        TextFileReaderObject = pd.read_hdf(fname, *args, **kwargs)
+    elif suffix.endswith(('.sql',)):
+        TextFileReaderObject = pd.read_sql(fname, *args, **kwargs)
+    else:
+        raise ValueError(f"""Unsupported filetype for file "{fname}".""")
+    return TextFileReaderObject
+
+
+def successiveParents(pathObj: Path, numLevels: int) -> Tuple[Path, int]:
+    """
+    Successively get the parents of the Path object submitted.
+    """
+    while numLevels > 0:
+        pathObj = pathObj.parent
+        numLevels -= 1
+    return pathObj, numLevels
+
+
+def fileContainsColumn(pathObj: Path, listOfColumns: list) -> bool:
+    """
+    Determines if the file defined by `pathObj` has any of the columns contained in `listOfColumns`.
+    """
+    condition = False
+    df = pd.read_csv(pathObj, nrows=10)
+    columns = df.columns
+    for columnName in listOfColumns:
+        if columnName in columns:
+            condition = True
+            break
+        else:
+            continue
+    return condition
+
+
+def getCommonDirectoryParent(primaryPath: Path, secondaryPath: Path) -> Path:
+    """
+    """
+    commonPrefix = os.path.commonprefix([primaryPath, secondaryPath])
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        if commonPrefix == "/":
+            pathResult = primaryPath
+        else:
+            pathResult = primaryPath.absolute().relative_to(secondaryPath)
+    elif operatingSystem == "win32":
+        if commonPrefix == "":
+            pathResult = primaryPath
+        else:
+            pathResult = primaryPath.absolute().relative_to(secondaryPath)
+    return pathResult
+
+
+def getFilesToRelease(filesToRelease: List[Path], fileCriteria: List[Callable]):
+    """
+    Applies the functions in the iterable `fileCriteria` to each Path object in `filesToRelease`.
+    """
+    filesToRelease = []
+    for file in filesToRelease:
+        criteria = []
+        for criteriaFunc in fileCriteria:
+            criteria.append(criteriaFunc(file))
+        criteriaMet = all(criteria)
+        if criteriaMet:
+            filesToRelease.append(file)
+        else:
+            pass
+
+
+def getLastIDNum(df, columnName="deid_num"):
+    """
+    Gets the last ID number in a de-identification map.
+    """
+    numbers = df[columnName].astype(int)
+    return max(numbers)
+
+
+def isNumber(string):
+    """
+    Checks if the string represents a number
+
+    For a discussion see https://stackoverflow.com/questions/354038/how-do-i-check-if-a-string-represents-a-number-float-or-int
+    """
+    try:
+        int(float(string))
+        return True
+    except ValueError as error:
+        msg = error.args[0]
+        if "invalid literal for int() with base 10:" in msg:  # This must be an old Python exception message
+            return False
+        elif "could not convert string to float:" in msg:  # I think this is the new exception message
+            return False
+        else:
+            raise Exception(error)
+
+
+def fileName2variableName(pathObj):
+    """
+    """
+    pattern = r"^(?P<variableName>.+) map"
+    string = pathObj.stem
+    obj = re.match(pattern, string)
+    if obj:
+        groupDict = obj.groupdict()
+        variableName = groupDict["variableName"]
+    else:
+        raise Exception("This file path objected was of an unexpected format.")
+    return variableName
+
+
+def mapGroupCriteria4unknownValue(value):
+    """
+    Checks if `value` is a number. If so, it checks if it's less than 0. If it's not a number, return `True`.
+
+    This is used in making de-identification maps, where negative ID values are usually used to represent unknown or null values.
+    """
+    if isNumber(value):
+        return float(value) < 0
+    else:
+        return False
+
+
+def makeMap(IDset: set,
+            IDName: str,
+            startFrom: Union[int, list],
+            irbNumber: str,
+            suffix: str,
+            columnSuffix: str,
+            logger: Logger,
+            groups: dict = {0: {"criteria": [mapGroupCriteria4unknownValue],
+                                "deidNum": 0}},
+            deIdentificationMapStyle: Literal["classic", "lemur"] = "lemur") -> pd.DataFrame:
+    """
+    Makes an IDR de-identification map.
+
+    INPUT
+        `IDset`, a set of IDs
+        `IDName`, the name of the ID
+        `startFrom`, the integer number to start from
+        `groups`, ID values to group or map in a many-to-one fashion. E.g., invalid IDs (negative numbers) are usually all mapped to the same de-identified number, like "0".
+        `deIdentificationMapStyle`, a string, one of {"classic, "lemur"}. The formats are as follow:
+            | Format Style  | de-Identififed ID Column Header   |
+            | ------------- | -------------------------------   |
+            | "clasic"      | `f"deid_{columnSuffix}_id"`       |
+            | "lemur"       | `f"de-Identified {IDName}"`       |
+
+    OUTPUT
+        `map_`, a Pandas DataFrame with the following format:
+        | `IDName` | deid_num   | de-Identififed ID Column Header |
+        | -------- | --------   | ------------------------ |
+        | IDset[0] | numbers[0] | ... |
+        | ...      | ...        | ... |
+    """
+    # QA: `irbNumber` must not be NoneType
+    if isinstance(irbNumber, type(None)):
+        raise Exception("""`irbNumber` cannot be of type "None".""")
+
+    # Assign header formats: de-Identififed ID Column Header
+    if deIdentificationMapStyle == "classic":
+        deIdentificationSerialNumberHeader = "deid_num"
+    elif deIdentificationMapStyle == "lemur":
+        deIdentificationSerialNumberHeader = "De-identification Serial Number"
+
+    # Assign header formats: de-Identififed ID Column Header
+    if deIdentificationMapStyle == "classic":
+        deIdentifiedIDColumnHeader = f"deid_{columnSuffix}_id"
+    elif deIdentificationMapStyle == "lemur":
+        deIdentifiedIDColumnHeader = f"De-identified {IDName}"
+
+    if len(IDset) == 0:
+        return pd.DataFrame(columns=[IDName,
+                                     deIdentificationSerialNumberHeader,
+                                     deIdentifiedIDColumnHeader])
+    else:
+        pass
+    if isinstance(startFrom, int):
+        startFrom = startFrom
+        numbers = list(range(startFrom, startFrom + len(IDset)))
+    elif isinstance(startFrom, list):
+        numbers = startFrom[:]
+        startFrom = numbers[0]
+    numbers.extend([None])
+    logger.info("    Sorting `IDset`.")
+    IDli = sortIntegersAndStrings(list(IDset))
+    logger.info("    Sorting `IDset` - done.")
+    logger.info("    Creating `mapDi`.")
+    mapDi = {IDNum: {} for IDNum in IDli}
+    logger.info("    Creating `mapDi` - done.")
+    lenIDli = len(IDli)
+    if lenIDli > 100000:
+        itChunk = 1000
+    else:
+        itChunk = max(round(lenIDli / 50), 1)
+    for it, IDNum in enumerate(IDli, start=1):
+        fromGroup = False
+        for group, groupAttributes in groups.items():
+            criteriaList = groupAttributes["criteria"]
+            criteria = [criterion(IDNum) for criterion in criteriaList]
+            if all(criteria):
+                deid_num = groupAttributes["deidNum"]
+                fromGroup = True
+                break
+        if fromGroup:
+            pass
+        else:
+            deid_num = numbers.pop(0)
+        deid_id = f"{irbNumber}_{suffix}_{deid_num}"
+        mapDi[IDNum] = {IDName: IDNum,
+                        deIdentificationSerialNumberHeader: deid_num,
+                        deIdentifiedIDColumnHeader: deid_id}
+        if it % itChunk == 0:
+            logger.info(f"  ..  Working on item {it:,} of {len(IDli):,} ({it/lenIDli:.2%} done).")
+    newMap = pd.DataFrame.from_dict(mapDi, orient="index")
+    newMap.index = range(1, len(newMap) + 1)
+    return newMap
+
+
+def makeSetComplement(set1, cardinalityOfNewSet):
+    """
+    Creates a complement to a set, based on the specified size of the complement. Elements of the first set are assumed to be integers from 1 and above, and cardinalities are non-zero positive integers.
+
+    TODO: Implement empty set handling
+    """
+    set1Min = 1
+    if len(set1) == 0:
+        raise ValueError("Set should not be empty.")
+    else:
+        set1Max = max(set1)
+    s1Contiguous = set(range(set1Min, set1Max + 1))
+    setDifference = s1Contiguous.difference(set1)
+    cardinalityOfSetDifference = len(setDifference)
+    cardinalityOfContiguousSubset = cardinalityOfNewSet - cardinalityOfSetDifference
+    if cardinalityOfContiguousSubset > 0:
+        setDifferenceSubset = setDifference
+        contiguousSubset = set(range(set1Max + 1, set1Max + cardinalityOfContiguousSubset + 1))
+    elif cardinalityOfContiguousSubset == 0:
+        setDifferenceSubset = setDifference
+        contiguousSubset = set()
+    elif cardinalityOfContiguousSubset < 0:
+        setDifferenceSubset = set(list(setDifference)[:cardinalityOfNewSet])
+        contiguousSubset = set()
+    newSet = setDifferenceSubset.union(contiguousSubset)
+    return newSet
+
+
+def loglevel2int(loglevel: Union[int, str]) -> int:
+    """
+    An agnostic converter that takes int or str and returns int. If input is int, output is the same as input"""
+    dummy = logging.getLogger("dummy")
+    dummy.setLevel(loglevel)
+    loglevel = dummy.level
+    return loglevel
+
+
+def replace_sql_query(query: str, old: str, new: str, loglevel: Union[int, str] = "INFO") -> str:
+    """
+    Replaces text in a SQL query only if it's not commented out. I.e., this function applies string.replace() only if the string doesn't begin with "--".
+    TODO Don't replace text after "--".
+    """
+    loglevel_asnumber = loglevel2int(loglevel)
+    logger.setLevel(loglevel_asnumber + 10)
+
+    pattern = r"^\w*--"
+    li = query.split("\n")
+    result = []
+    logger.debug("Starting")
+    for line in li:
+        logger.debug(f"""  Working on "{line}".""")
+        obj = re.search(pattern, line)
+        if obj:
+            logger.debug("    Passing")
+            nline = line
+        else:
+            nline = line.replace(old, new)
+            logger.debug(f"""    Replacing text in "{line}" --> "{nline}".""")
+        logger.debug("  Appending...")
+        result.append(nline)
+    logger.debug("Finished")
+    return "\n".join(result)
+
+
+def sqlite2df(tableContents: list, tableName: str, cursor: sqlite3.Cursor) -> pd.DataFrame:
+    """
+    `tableContents` must be a "*" query where all the columns are returned.
+    """
+    # Get metadata on table
+    query = f"PRAGMA table_info({tableName});"
+    cursor.execute(query)
+    query_results = cursor.fetchall()
+    column_header = [tu[1] for tu in query_results]
+
+    tableContents_asDict = {}
+    for it, table_info in enumerate(tableContents):
+        di = {}
+        for key, value in zip(column_header, table_info):
+            di[key] = value
+        tableContents_asDict[it] = di
+    df = pd.DataFrame.from_dict(tableContents_asDict, orient="index")
+    df.index = range(1, len(tableContents) + 1)
+    return df
+
+
+def patient_key_from_person_id(person_id: int, map_: dict = {}) -> Tuple[int, Literal[0, 1]]:
+    """
+    Assumes "map_" is a dictionary with person IDs as integers that map patient keys as integers.
+    """
+    if person_id in map_.keys():
+        patient_key = map_[person_id]
+        source = 0
+    else:
+        query = f"""use DWS_OMOP_PROD
+        SELECT
+            xref.PERSON_MAPPING.person_id as person_id,
+            xref.PERSON_MAPPING.patient_key as patient_key
+        FROM
+            xref.PERSON_MAPPING
+        WHERE
+            xref.PERSON_MAPPING.person_id IN ({person_id})"""
+        results = pd.read_sql(query, con=conStr)
+        person_id = results["person_id"][0]
+        patient_key = results["patient_key"][0]
+        source = 1
+    return patient_key, source
+
+
+def personIDs2patientKeys(personIDList: List[int]) -> pd.DataFrame:
+    """
+
+    """
+    list2str = ",".join([str(num) for num in personIDList])
+    query = f"""use DWS_OMOP_PROD
+    SELECT
+        xref.PERSON_MAPPING.person_id as person_id,
+        xref.PERSON_MAPPING.patient_key as patient_key
+    FROM
+        xref.PERSON_MAPPING
+    WHERE
+        xref.PERSON_MAPPING.person_id IN ({list2str})"""
+    results = pd.read_sql(query, con=conStr)
+    return results
+
+
+def epicID2patientKey(epicIDlist: List[str]) -> pd.DataFrame:
+    """
+    Executes a SQL query to map EPIC Patient IDs to Patient Keys.
+    """
+    IDsAsString = ",".join([f"'{el}'" for el in epicIDlist])
+    query = f"""USE DWS_PROD
+    SELECT
+        dbo.ALL_PATIENTS.PATNT_KEY AS 'Patient Key',
+        dbo.ALL_PATIENTS.PATNT_ID AS 'EPIC Patient ID'
+    FROM
+        dbo.ALL_PATIENTS
+    WHERE
+        (
+        dbo.ALL_PATIENTS.PATNT_ID  IN  ( {IDsAsString}  )
+        AND
+        ( dbo.ALL_PATIENTS.TEST_IND='N'  )
+        )"""
+    results = pd.read_sql(query, con=conStr)
+    return results
+
+
+def map2di(map_: pd.DataFrame, fromColumnIndex: int = 0, toColumnIndex: int = 2) -> dict:
+    """
+    `fromColumnIndex` is the variable to assign as the key to the dictionary.
+    `toColumnIndex` is the variable to assign as the value pair in the dictionary.
+    Assumes the following structure to "map_":
+    column 1      | column 2       | column 3      | ... | column k
+        x_(1,1)   |     x_(1,2)    |    x_(1,3)    | ... |   x_(1,k)
+        .         |     .          |     .         | ... |   .
+        .         |     .          |     .         | ... |   .
+        .         |     .          |     .         | ... |   .
+        x_(n,1)   |     x_(n,2)    |    x_(n,3)    | ... |   x_(n,k)
+    Where the columns are from 1, 2, 3, ..., i, ..., k-1, k, and the rows are from 1, 2, 3, ..., j, ..., n-1, n.
+    """
+    di = {}
+    errors = []
+    for _, row in map_.iterrows():
+        oldValue = row.values[fromColumnIndex]
+        newValue = row.values[toColumnIndex]
+        if oldValue in di.keys() and di[oldValue] != newValue:
+            errors.append({oldValue: newValue})
+        di[oldValue] = newValue
+    if len(errors) > 0:
+        raise Exception(f"This map is not one to one. At least one ID is duplicated with multiple de-identified IDs: {errors}")
+    else:
+        return di
+
+
+def float2str(value: float, navalue="") -> str:
+    """
+    Converts values to string-type. If a value is NaN it is replaced with a value that can be converted to a string, default empty string, "".
+    """
+    assert isinstance(navalue, str), """"navalue" is not a string type."""
+    if pd.isna(value):
+        newValue = str(navalue)
+    else:
+        newValue = str(int(value))
+    return newValue
+
+
+def numericOrString2integerOrString(value) -> Union[str, int]:
+    """
+    Determines if a value is numeric or string. If numeric, convert to an integer, else return as string.
+
+    Used by `makeMapsFromOthers.py`
+    """
+    if isNumber(value):
+        return int(float(value))
+    else:
+        return str(value)
+
+
+def sortIntegersAndStrings(li: list) -> list:
+    """
+    Sorts a list of integers and strings by sorted them separately and then concatenating the results.
+    """
+    series = pd.Series(li)
+    maskIntegers = series.apply(lambda el: isinstance(el, int))
+    maskStrings = series.apply(lambda el: isinstance(el, str))
+    li2 = sorted(series[maskIntegers].to_list()) + sorted(series[maskStrings].to_list())
+    return li2
+
+
+def str2int(value, navalue=-1):
+    """
+    Converts values to integer-type. If a value is NaN it is replaced with a value that can be converted to an integer, default is "-1".
+    """
+    assert isinstance(navalue, int), """"navalue" is not an integer type."""
+    if pd.isna(value):
+        newValue = int(navalue)
+    else:
+        newValue = int(float(value))
+    return newValue
+
+
+def str2intOr0(string):
+    """
+    Converts a string to its numeric value, or 0, if it has no numeric value.
+    """
+    if string.isnumeric():
+        return int(string)
+    else:
+        return 0
+
+
+def str2bool(value, navalue=""):
+    """
+    Converts values to boolean-type. If a value is missing it is replaced with an empty string.
+    """
+    if pd.isna(value):
+        newValue = int(navalue)
+    else:
+        newValue = bool(value)
+    return newValue
+
+
+def deconstructStudyID(string):
+    """
+    Deconstructs a de-identified study ID into its component parts, assuming the following format: STUDY-TYPESTUDY-NUMBER_SERIAL-NUMBER
+    Where "STUDY_TYPE" is the study type, e.g., "CED", "IRB", or "WIRB"
+          "STUDY-NUMBER" is the study serial number, usually a 9-digit number where the first four numbers is a four-digit year.
+          "SERIAL-NUMBER" is the de-identified study-specific serial number of a patient or other subject.
+    For example: "IRB202300123_222"
+    """
+    pattern = r"(?P<studyType>\w+)(?P<studyNumber>\d{9})_(?P<PHI_type>\w+)_(?P<deIdentificationNumber>\d+)"
+    regexObj = re.search(pattern, string)
+    if regexObj:
+        di = regexObj.groupdict()
+        return di
+    else:
+        raise Exception("String is of an unexpected format. See function docstring for expected format.")
+
+
+def studyID2tuple(string):
+    """
+    Extracts the numeric portion of a string.
+
+    Assumes the following format: STUDY-TYPESTUDY-NUMBER_SERIAL-NUMBER
+    Where "STUDY_TYPE" is the study type, e.g., "CED", "IRB", or "WIRB"
+          "STUDY-NUMBER" is the study serial number, usually a 9-digit number where the first four numbers is a four-digit year.
+          "SERIAL-NUMBER" is the de-identified study-specific serial number of a patient or other subject.
+    For example: "IRB202300123_222"
+
+    This is intended for use when sorting columns by the numeric value of the string, and not the text value.
+    """
+    di = deconstructStudyID(string)
+    studyType = di["studyType"]
+    studyNumber = int(di["studyNumber"])
+    PHI_type = di["PHI_type"]
+    deIdentificationNumber = int(di["deIdentificationNumber"])
+    tu = studyType, studyNumber, PHI_type, deIdentificationNumber
+    return tu
+
+
+def isValidPatientID(value):
+    """
+    Checks if the value is a valid UFHealth patient ID. Invalid patient IDs are defined as negative integers
+    """
+    isNumber_bool = isNumber(value)
+    if isNumber_bool:
+        number = int(value)
+        if number < 0:
+            result = False
+        elif number >= 0:  # Assumes `0` is a valid patient ID
+            result = True
+    elif not isNumber_bool:
+        result = True  # Assumes all non-numeric IDs are valid
+    return result
+
+
+def isDatetime(string):
+    """
+    Checks if a string contains a datetime format.
+    """
+    try:
+        _ = parse(string, fuzzy=False)
+        return True
+    except ValueError:
+        return False
+
+
+def ditchFloat(value):
+    """
+    Gets rid of float types if value is string, integer, float, or datetime
+    """
+    if isinstance(value, str):
+        value = str(value)
+        if value.isnumeric():
+            standardValue = int(value)
+        elif isNumber(value):
+            standardValue = int(float(value))
+        elif isDatetime(value):
+            standardValue = parse(value, fuzzy=False)
+        else:
+            raise ValueError(f"""Unexpected format in string value "{value}". We expected a string with a number, numeric, or datetime format.""")
+    elif isinstance(value, int) or isinstance(value, np.integer) or isinstance(value, float):
+        standardValue = int(value)
+    else:
+        raise ValueError(f"""Unexpected data type "{type(value)}" for value "{value}". Expect only string, float, or integers.""")
+    return standardValue
+
+
+def handleDatetimeForJson(obj):
+    """
+    JSON serializer for objects not serializable by default json code
+
+    h/t to https://stackoverflow.com/a/22238613/5478086
+    """
+    if isinstance(obj, (datetime, date, time)):
+        return obj.isoformat()
+    raise TypeError(f"Type {type(obj)} not serializable")
+
+
+def makeChunks(array_range: array, chunkSize: int) -> tuple:
+    """
+    Inspired by GeekForGeeks.com (https://www.geeksforgeeks.org/break-list-chunks-size-n-python/)
+
+    Only makes chunks of one dimensional arrays (e.g., lists, Pandas Series), but not dataframes.
+
+    Example:
+    array = range(30)
+    chunks = makeChunks(array, chunkSize)
+    """
+    array_range = iter(array_range)
+    return iter(lambda: tuple(islice(array_range, chunkSize)), ())
+
+
+# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+# >>> tree function >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+# >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
+# h/t https://stackoverflow.com/a/59109706/5478086
+
+
+def tree(dir_path: Path, level: int = -1, limit_to_directories: bool = False,
+         length_limit: int = 1000):
+    """Given a directory Path object print a visual tree structure"""
+    # prefix components:
+    space = '    '
+    branch = '│   '
+    # pointers:
+    tee = '├── '
+    last = '└── '
+
+    dir_path = Path(dir_path)  # accept string coerceable to Path
+    files = 0
+    directories = 0
+
+    def inner(dir_path: Path, prefix: str = '', level=-1):
+        nonlocal files, directories
+        if not level:
+            return  # 0, stop iterating
+        if limit_to_directories:
+            contents = [d for d in dir_path.iterdir() if d.is_dir()]
+        else:
+            contents = list(dir_path.iterdir())
+        pointers = [tee] * (len(contents) - 1) + [last]
+        for pointer, path in zip(pointers, contents):
+            if path.is_dir():
+                yield prefix + pointer + path.name
+                directories += 1
+                extension = branch if pointer == tee else space
+                yield from inner(path, prefix=prefix + extension, level=level - 1)
+            elif not limit_to_directories:
+                yield prefix + pointer + path.name
+                files += 1
+    print(dir_path.name)
+    iterator = inner(dir_path, level=level)
+    for line in islice(iterator, length_limit):
+        print(line)
+    if next(iterator, None):
+        print(f'... length_limit, {length_limit}, reached, counted:')
+    print(f'\n{directories} directories' + (f', {files} files' if files else ''))
+
+
+# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
+# <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/getEncountersMap.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getEncountersMap.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/getPatientsMap.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getPatientsMap.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/idealist/idealist.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/idealist.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/images/utilities.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/images/utilities.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/makeSymLinks.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/makeSymLinks.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/notes/freeText.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/notes/freeText.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/notes/pullNotes.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/notes/pullNotes.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/notes/utils.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/notes/utils.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/omop/configProcessing.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/omop/configProcessing.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""
-Utility functions for processing the OMOP Data Pull configuration file.
-"""
-
-import os
-import sys
-from pathlib import Path
-# Third-party packages
-import yaml
-# Custom packages
-from drapi.drapi import successiveParents
-
-
-def interpretPath(pathAsString: str) -> str:
-    """
-    Makes sure path separators are appropriate for the current operating system.
-    """
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        newPathAsString = pathAsString.replace("\\", "/")
-    elif operatingSystem == "win32":
-        newPathAsString = pathAsString.replace("/", "\\")
-    else:
-        raise Exception("Unsupported operating system")
-    return newPathAsString
-
-
-def editConfig(inputPath: Path, outputPath: Path, timestamp: str) -> None:
-    """
-    Edits a YAML config file so that the output paths have a timestamp according to the following formats:
-    Category 1 Directory: "parent1/parenti/parentn-1/parentn" --> "parent1/parenti/parentn-1/parentn/<timestamp>/"
-    Category 2 Directory: "parent1/parenti/parentn-1/parentn" --> "parent1/parenti/parentn-1/<timestamp>/parentn/"
-
-    Category 1 directories:
-      - mapping_location
-    Category 2 directories:
-      - deidentified_file_location
-      - identified_file_location
-    """
-    with open(inputPath) as file:
-        configFile = yaml.safe_load(file)
-
-    # Get paths as strings
-    identified_file_location_str = configFile["data_output"]["identified_file_location"]
-    deidentified_file_location_str = configFile["data_output"]["deidentified_file_location"]
-    mapping_location_str = configFile["data_output"]["mapping_location"]
-
-    # Make sure path separators are OS-appropriate
-    identified_file_location_str2 = interpretPath(identified_file_location_str)
-    deidentified_file_location_str2 = interpretPath(deidentified_file_location_str)
-    mapping_location_str2 = interpretPath(mapping_location_str)
-
-    # Add timestamp to path as subfolder
-    pathDict = {"identified_file_location": identified_file_location_str2,
-                "deidentified_file_location": deidentified_file_location_str2,
-                "mapping_location": mapping_location_str2}
-    CATEGORY_1 = ["mapping_location"]
-    CATEGORY_2 = ["identified_file_location", "deidentified_file_location"]
-    sep = os.sep
-    for pathName, pathStr in pathDict.items():
-        pathObj = Path(pathStr).absolute()
-        if pathName in CATEGORY_1:
-            newPath = pathObj.joinpath(timestamp)
-        elif pathName in CATEGORY_2:
-            pathDirName = pathObj.name
-            pathParent, _ = successiveParents(pathObj, 1)
-            newPath = pathParent.joinpath(timestamp).joinpath(pathDirName)
-        else:
-            raise Exception(f"""Unexpected value: "{pathName}".""")
-        configFile["data_output"][pathName] = str(newPath) + sep
-
-    with open(outputPath, "w") as file:
-        yaml.dump(configFile, file)
+"""
+Utility functions for processing the OMOP Data Pull configuration file.
+"""
+
+import os
+import sys
+from pathlib import Path
+# Third-party packages
+import yaml
+# Custom packages
+from drapi.drapi import successiveParents
+
+
+def interpretPath(pathAsString: str) -> str:
+    """
+    Makes sure path separators are appropriate for the current operating system.
+    """
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        newPathAsString = pathAsString.replace("\\", "/")
+    elif operatingSystem == "win32":
+        newPathAsString = pathAsString.replace("/", "\\")
+    else:
+        raise Exception("Unsupported operating system")
+    return newPathAsString
+
+
+def editConfig(inputPath: Path, outputPath: Path, timestamp: str) -> None:
+    """
+    Edits a YAML config file so that the output paths have a timestamp according to the following formats:
+    Category 1 Directory: "parent1/parenti/parentn-1/parentn" --> "parent1/parenti/parentn-1/parentn/<timestamp>/"
+    Category 2 Directory: "parent1/parenti/parentn-1/parentn" --> "parent1/parenti/parentn-1/<timestamp>/parentn/"
+
+    Category 1 directories:
+      - mapping_location
+    Category 2 directories:
+      - deidentified_file_location
+      - identified_file_location
+    """
+    with open(inputPath) as file:
+        configFile = yaml.safe_load(file)
+
+    # Get paths as strings
+    identified_file_location_str = configFile["data_output"]["identified_file_location"]
+    deidentified_file_location_str = configFile["data_output"]["deidentified_file_location"]
+    mapping_location_str = configFile["data_output"]["mapping_location"]
+
+    # Make sure path separators are OS-appropriate
+    identified_file_location_str2 = interpretPath(identified_file_location_str)
+    deidentified_file_location_str2 = interpretPath(deidentified_file_location_str)
+    mapping_location_str2 = interpretPath(mapping_location_str)
+
+    # Add timestamp to path as subfolder
+    pathDict = {"identified_file_location": identified_file_location_str2,
+                "deidentified_file_location": deidentified_file_location_str2,
+                "mapping_location": mapping_location_str2}
+    CATEGORY_1 = ["mapping_location"]
+    CATEGORY_2 = ["identified_file_location", "deidentified_file_location"]
+    sep = os.sep
+    for pathName, pathStr in pathDict.items():
+        pathObj = Path(pathStr).absolute()
+        if pathName in CATEGORY_1:
+            newPath = pathObj.joinpath(timestamp)
+        elif pathName in CATEGORY_2:
+            pathDirName = pathObj.name
+            pathParent, _ = successiveParents(pathObj, 1)
+            newPath = pathParent.joinpath(timestamp).joinpath(pathDirName)
+        else:
+            raise Exception(f"""Unexpected value: "{pathName}".""")
+        configFile["data_output"][pathName] = str(newPath) + sep
+
+    with open(outputPath, "w") as file:
+        yaml.dump(configFile, file)
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/omop/deidentify.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/omop/deidentify.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/oneFlorida.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/oneFlorida.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-Converts OneFlorida patient ID to UF medical record number (MRN).
-"""
-
-import os
-from pathlib import Path
-from typing_extensions import Literal
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import replace_sql_query, successiveParents
-
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-thisFilePath = Path(__file__)
-drapiRootDir, _ = successiveParents(thisFilePath, 3)
-sqlDir = drapiRootDir.joinpath("sql")
-
-# Variables: More
-sqlFilePath1 = sqlDir.joinpath("ConvertBetweenMrnAndOneFloridaPatID.SQL")
-sqlFilePath2 = sqlDir.joinpath("MapOneFloridaIDs.SQL")
-
-# Variables: SQL connection settings
-uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-
-def OFID2MRN(OFIDseries: pd.Series) -> pd.DataFrame:
-    """
-
-    """
-    listAsString = ",".join([str(el) for el in OFIDseries.values])
-
-    with open(sqlFilePath1, "r") as file:
-        query0 = file.read()
-
-    query = replace_sql_query(query=query0,
-                              old="{PYTHON_VARIABLE: ONE_FLORIDA_PATIENT_IDS}",
-                              new=listAsString)
-
-    MRNseries = pd.read_sql(query, con=conStr)
-
-    return MRNseries
-
-
-def mapOneFloridaIDs(IDTypeValues: pd.Series, IDType: Literal["PATID", "Patient Key", "MRN (UF)", "MRN (Jax)", "MRN (Pathology)"]) -> pd.Series:
-    """
-    Queries the ID map containing all of the following variables, any of which can be used as a query filter using the `IDType` parameter. The values to query by are used in the `IDTypeValues` parameter.
-        | Variable Definition           | Standard or Common Column Name    |
-        |-------------------------------|-----------------------------------|
-        | OneFlorida patient ID         | OneFlorida Patient ID             |
-        | IDR patient key               | Patient Key                       |
-        | UF Health Gainesvile MRN      | MRN (UF)                          |
-        | UF Health Jacksonville MRN    | MRN (Jax)                         |
-        | UF Health Pathology MRN       | MRN (Pathology)                   |
-    """
-
-    listAsString = ",".join([f"'{el}'" for el in IDTypeValues.iloc[:].sort_values()])
-
-    with open(sqlFilePath2, "r") as file:
-        query0 = file.read()
-
-    query = replace_sql_query(query=query0,
-                              old="{PYTHON_VARIABLE: IDTypeValues}",
-                              new=listAsString)
-    IDTypeInput = IDType.lower()
-    IDTypeDict = {"oneflorida patient id": "a.PATID",
-                  "patient key": "a.PATNT_KEY",
-                  "mrn (uf)": "b.IDENT_ID",
-                  "mrn (jax)": "c.IDENT_ID",
-                  "mrn (pathology)": "d.IDENT_ID"}
-    IDTypeSQL = IDTypeDict[IDTypeInput]
-    query = replace_sql_query(query=query,
-                              old="{PYTHON_VARIABLE: IDTypeSQL}",
-                              new=IDTypeSQL)
-
-    MRNseries = pd.read_sql(query, con=conStr)
-
-    return MRNseries
+"""
+Converts OneFlorida patient ID to UF medical record number (MRN).
+"""
+
+import os
+from pathlib import Path
+from typing_extensions import Literal
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import replace_sql_query, successiveParents
+
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+thisFilePath = Path(__file__)
+drapiRootDir, _ = successiveParents(thisFilePath, 3)
+sqlDir = drapiRootDir.joinpath("sql")
+
+# Variables: More
+sqlFilePath1 = sqlDir.joinpath("ConvertBetweenMrnAndOneFloridaPatID.SQL")
+sqlFilePath2 = sqlDir.joinpath("MapOneFloridaIDs.SQL")
+
+# Variables: SQL connection settings
+uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+
+def OFID2MRN(OFIDseries: pd.Series) -> pd.DataFrame:
+    """
+
+    """
+    listAsString = ",".join([str(el) for el in OFIDseries.values])
+
+    with open(sqlFilePath1, "r") as file:
+        query0 = file.read()
+
+    query = replace_sql_query(query=query0,
+                              old="{PYTHON_VARIABLE: ONE_FLORIDA_PATIENT_IDS}",
+                              new=listAsString)
+
+    MRNseries = pd.read_sql(query, con=conStr)
+
+    return MRNseries
+
+
+def mapOneFloridaIDs(IDTypeValues: pd.Series, IDType: Literal["PATID", "Patient Key", "MRN (UF)", "MRN (Jax)", "MRN (Pathology)"]) -> pd.Series:
+    """
+    Queries the ID map containing all of the following variables, any of which can be used as a query filter using the `IDType` parameter. The values to query by are used in the `IDTypeValues` parameter.
+        | Variable Definition           | Standard or Common Column Name    |
+        |-------------------------------|-----------------------------------|
+        | OneFlorida patient ID         | OneFlorida Patient ID             |
+        | IDR patient key               | Patient Key                       |
+        | UF Health Gainesvile MRN      | MRN (UF)                          |
+        | UF Health Jacksonville MRN    | MRN (Jax)                         |
+        | UF Health Pathology MRN       | MRN (Pathology)                   |
+    """
+
+    listAsString = ",".join([f"'{el}'" for el in IDTypeValues.iloc[:].sort_values()])
+
+    with open(sqlFilePath2, "r") as file:
+        query0 = file.read()
+
+    query = replace_sql_query(query=query0,
+                              old="{PYTHON_VARIABLE: IDTypeValues}",
+                              new=listAsString)
+    IDTypeInput = IDType.lower()
+    IDTypeDict = {"oneflorida patient id": "a.PATID",
+                  "patient key": "a.PATNT_KEY",
+                  "mrn (uf)": "b.IDENT_ID",
+                  "mrn (jax)": "c.IDENT_ID",
+                  "mrn (pathology)": "d.IDENT_ID"}
+    IDTypeSQL = IDTypeDict[IDTypeInput]
+    query = replace_sql_query(query=query,
+                              old="{PYTHON_VARIABLE: IDTypeSQL}",
+                              new=IDTypeSQL)
+
+    MRNseries = pd.read_sql(query, con=conStr)
+
+    return MRNseries
```

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/prepTSVforSDOH.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/prepTSVforSDOH.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/sql.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/sql.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/drapi/stats.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/stats.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/code/tree.py` & `drapi-lemur-1.0.5/src/drapi/code/tree.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/9-Digit Zip Code.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/9-Digit Zip Code.SQL`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/Consent2Share.sql` & `drapi-lemur-1.0.5/src/drapi/sql/Consent2Share.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/LADMF.sql` & `drapi-lemur-1.0.5/src/drapi/sql/LADMF.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/MRNfromPatientKey.sql` & `drapi-lemur-1.0.5/src/drapi/sql/MRNfromPatientKey.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/MapOneFloridaIDs.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/MapOneFloridaIDs.SQL`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-	SELECT 
-		a.PATID as "OneFlorida Patient ID",
-		a.PATNT_KEY as "Patient Key",
-		b.IDENT_ID as "MRN (UF)",
-		c.IDENT_ID as "MRN (Jax)",
-		d.IDENT_ID as "MRN (Pathology)"
-	FROM [DWS_PCORNET].[pcnv5].[PATIENT_MAPPING] a
-	left outer join [DWS_PROD].[dbo].[ALL_PATIENT_IDENTITIES] b on a.patnt_key = b.patnt_key and b.ident_id_type=101 and b.LOOKUP_IND = 'Y'
-	left outer join [DWS_PROD].[dbo].[ALL_PATIENT_IDENTITIES] c on a.patnt_key = c.patnt_key and c.ident_id_type=110 and c.LOOKUP_IND = 'Y'
-	left outer join [DWS_PROD].[dbo].[ALL_PATIENT_IDENTITIES] d on a.patnt_key = d.patnt_key and d.ident_id_type=99 and d.LOOKUP_IND = 'Y'
+	SELECT 
+		a.PATID as "OneFlorida Patient ID",
+		a.PATNT_KEY as "Patient Key",
+		b.IDENT_ID as "MRN (UF)",
+		c.IDENT_ID as "MRN (Jax)",
+		d.IDENT_ID as "MRN (Pathology)"
+	FROM [DWS_PCORNET].[pcnv5].[PATIENT_MAPPING] a
+	left outer join [DWS_PROD].[dbo].[ALL_PATIENT_IDENTITIES] b on a.patnt_key = b.patnt_key and b.ident_id_type=101 and b.LOOKUP_IND = 'Y'
+	left outer join [DWS_PROD].[dbo].[ALL_PATIENT_IDENTITIES] c on a.patnt_key = c.patnt_key and c.ident_id_type=110 and c.LOOKUP_IND = 'Y'
+	left outer join [DWS_PROD].[dbo].[ALL_PATIENT_IDENTITIES] d on a.patnt_key = d.patnt_key and d.ident_id_type=99 and d.LOOKUP_IND = 'Y'
 	where {PYTHON_VARIABLE: IDTypeSQL} in ( {PYTHON_VARIABLE: IDTypeValues}  )  -- Give the list of OneFlorida patient IDs
```

### Comparing `drapi-lemur-1.0.4/src/drapi/sql/encounterNumber2patientKey.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/encounterNumber2patientKey.SQL`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# README
-
-This is the folder structure for the Anaconda environment batch scripts. 
-```text
-    env-name
-    └── etc
-        └── conda
-            ├── activate.d
-            │   └── convenience.bat or convenience.sh
-            └── deactivate.d
-                └── convenience.bat or convenience.sh
-```
-Note `env-name` is the name of the anaconda environment, and `convenience` can be any name for your convenience batch script. A useful template is below. 
-
-```batch
-@REM Set environment variables (Remember to unset variables in the deactivation script)
-set "IPYTHONDIR=%CONDA_PREFIX%\etc\ipython"
-set "CONVENIENCE_PATH=%CONDA_PREFIX%\etc\conda\activate.d"
-set /p "HFA_UFADUID=" <%CONVENIENCE_PATH%\1.limerick
-set /p "HFA_UFADPWD=" <%CONVENIENCE_PATH%\2.limerick
-set "PYTHONPATH=%USERPROFILE%\Documents\GitHub\drapi-lemur\src"
-set "EMPTY_VAR="
-cls
-```
-
-For macOS, use shell scripts, with a different syntax.
-
-```shell
-# Set environment variables (Remember to unset variables in the deactivation script)
-export IPYTHONDIR="$CONDA_PREFIX/etc/ipython"
-export HFA_UFADUID="herman"
-export HFA_UFADPWD="mypassword"
+# README
+
+This is the folder structure for the Anaconda environment batch scripts. 
+```text
+    env-name
+    └── etc
+        └── conda
+            ├── activate.d
+            │   └── convenience.bat or convenience.sh
+            └── deactivate.d
+                └── convenience.bat or convenience.sh
+```
+Note `env-name` is the name of the anaconda environment, and `convenience` can be any name for your convenience batch script. A useful template is below. 
+
+```batch
+@REM Set environment variables (Remember to unset variables in the deactivation script)
+set "IPYTHONDIR=%CONDA_PREFIX%\etc\ipython"
+set "CONVENIENCE_PATH=%CONDA_PREFIX%\etc\conda\activate.d"
+set /p "HFA_UFADUID=" <%CONVENIENCE_PATH%\1.limerick
+set /p "HFA_UFADPWD=" <%CONVENIENCE_PATH%\2.limerick
+set "PYTHONPATH=%USERPROFILE%\Documents\GitHub\drapi-lemur\src"
+set "EMPTY_VAR="
+cls
+```
+
+For macOS, use shell scripts, with a different syntax.
+
+```shell
+# Set environment variables (Remember to unset variables in the deactivation script)
+export IPYTHONDIR="$CONDA_PREFIX/etc/ipython"
+export HFA_UFADUID="herman"
+export HFA_UFADPWD="mypassword"
 ```
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-"""
-Aliases variables that need to be de-identified.
-
-INPUT:
-Set Files
-
-PROCESS:
-Merge alias Set Files under the aliased (main) variable name
-
-OUTPUT:
-A new set file. This file would be the input to "makeMapsFromOthers.py"
-"""
-
-import csv
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from pandas.errors import EmptyDataError
-from sqlalchemy import create_engine
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-from drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT, FILE_NAME_TO_VARIABLE_NAME_DICT
-# Super-local
-from common import VARIABLE_ALIASES, DATA_TYPES_DICT
-
-# Arguments
-SET_FILES_DIR = Path(r"..\Concatenated Results\data\output\getIDValues\...\Set Files")
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                    # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                    #  "IRB_DIRECTORY",                 # noqa
-                                    #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                    #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-connection = create_engine(conStr).connect().execution_options(stream_results=True)
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `SET_FILES_DIR`: "{SET_FILES_DIR}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Script
-    for setFilePath in SET_FILES_DIR.iterdir():
-        logger.info(f"""  Working on set file : "{setFilePath.absolute().relative_to(rootDirectory)}".""")
-        try:
-            df = pd.read_table(setFilePath, header=None)
-        except EmptyDataError as err:
-            _ = err
-            df = pd.DataFrame(dtype=str)
-        variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[setFilePath.stem]
-        condition1 = variableName in VARIABLE_ALIASES.keys()
-        condition2 = variableName in VARIABLE_ALIASES.values()
-        dataType = DATA_TYPES_DICT[variableName]
-        if dataType == "Datetime":
-            quoting = csv.QUOTE_MINIMAL
-        elif dataType == "Numeric":
-            df = df.astype(float).astype("Int64")
-            quoting = csv.QUOTE_MINIMAL
-        elif dataType == "String":
-            quoting = csv.QUOTE_ALL
-        elif dataType == "Numeric_Or_String":
-            quoting = csv.QUOTE_ALL
-        else:
-            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
-        if condition1 or condition2:
-            if condition1:
-                aliasName = variableName
-                mainName = VARIABLE_ALIASES[aliasName]
-                logger.info(f"""    Variable is aliased to "{mainName}".""")
-            elif condition2:
-                mainName = variableName
-                logger.info("""    Variable is the main name of several aliases.""")
-            setFileName = f"{mainName}.txt"
-            newSetFilePath = runOutputDir.joinpath(setFileName)
-            if newSetFilePath.exists():
-                logger.info("""  ..  Variable set exists. Appending to file.""")
-                fileMode = "a"
-            else:
-                logger.info("""  ..  Variable set does not exists. Creating file.""")
-                fileMode = "w"
-            df.to_csv(newSetFilePath, quoting=quoting, mode=fileMode, index=False, header=False)
-        else:
-            logger.info("""    Variable set file is not aliased.""")
-            setFileName = f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]}.txt"
-            newSetFilePath = runOutputDir.joinpath(setFileName)
-            df.to_csv(newSetFilePath, quoting=quoting, index=False, header=False)
-
-    # Sort and remove duplicates from merged results.
-    logger.info("Sorting data and removing duplicates.")
-    listOfFiles = sorted(runOutputDir.iterdir())
-    for setFilePath in listOfFiles:
-        logger.info(f"""  Working on variable `setFilePath`: "{setFilePath.absolute().relative_to(rootDirectory)}".""")
-        try:
-            series = pd.read_table(setFilePath, header=None).iloc[:, 0]
-        except EmptyDataError as err:
-            _ = err
-            series = pd.Series(dtype=str)
-        logger.info(f"""    Starting size of variable set:               "{len(series):,}".""")
-        variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[setFilePath.stem]
-        dataType = DATA_TYPES_DICT[variableName]
-        if dataType == "Datetime":
-            quoting = csv.QUOTE_MINIMAL
-        elif dataType == "Numeric":
-            series = series.astype(float).astype("Int64")
-            quoting = csv.QUOTE_MINIMAL
-        elif dataType == "String":
-            quoting = csv.QUOTE_ALL
-        elif dataType == "Numeric_Or_String":
-            quoting = csv.QUOTE_ALL
-        else:
-            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
-        series = series.drop_duplicates().sort_values()
-        logger.info(f"""    Variable set size after removing duplicates: "{len(series):,}".""")
-        series.to_csv(setFilePath, quoting=quoting, index=False, header=False)
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Aliases variables that need to be de-identified.
+
+INPUT:
+Set Files
+
+PROCESS:
+Merge alias Set Files under the aliased (main) variable name
+
+OUTPUT:
+A new set file. This file would be the input to "makeMapsFromOthers.py"
+"""
+
+import csv
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from pandas.errors import EmptyDataError
+from sqlalchemy import create_engine
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+from drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT, FILE_NAME_TO_VARIABLE_NAME_DICT
+# Super-local
+from common import VARIABLE_ALIASES, DATA_TYPES_DICT
+
+# Arguments
+SET_FILES_DIR = Path(r"..\Concatenated Results\data\output\getIDValues\...\Set Files")
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                    # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                    #  "IRB_DIRECTORY",                 # noqa
+                                    #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                    #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+connection = create_engine(conStr).connect().execution_options(stream_results=True)
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `SET_FILES_DIR`: "{SET_FILES_DIR}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Script
+    for setFilePath in SET_FILES_DIR.iterdir():
+        logger.info(f"""  Working on set file : "{setFilePath.absolute().relative_to(rootDirectory)}".""")
+        try:
+            df = pd.read_table(setFilePath, header=None)
+        except EmptyDataError as err:
+            _ = err
+            df = pd.DataFrame(dtype=str)
+        variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[setFilePath.stem]
+        condition1 = variableName in VARIABLE_ALIASES.keys()
+        condition2 = variableName in VARIABLE_ALIASES.values()
+        dataType = DATA_TYPES_DICT[variableName]
+        if dataType == "Datetime":
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "Numeric":
+            df = df.astype(float).astype("Int64")
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "String":
+            quoting = csv.QUOTE_ALL
+        elif dataType == "Numeric_Or_String":
+            quoting = csv.QUOTE_ALL
+        else:
+            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
+        if condition1 or condition2:
+            if condition1:
+                aliasName = variableName
+                mainName = VARIABLE_ALIASES[aliasName]
+                logger.info(f"""    Variable is aliased to "{mainName}".""")
+            elif condition2:
+                mainName = variableName
+                logger.info("""    Variable is the main name of several aliases.""")
+            setFileName = f"{mainName}.txt"
+            newSetFilePath = runOutputDir.joinpath(setFileName)
+            if newSetFilePath.exists():
+                logger.info("""  ..  Variable set exists. Appending to file.""")
+                fileMode = "a"
+            else:
+                logger.info("""  ..  Variable set does not exists. Creating file.""")
+                fileMode = "w"
+            df.to_csv(newSetFilePath, quoting=quoting, mode=fileMode, index=False, header=False)
+        else:
+            logger.info("""    Variable set file is not aliased.""")
+            setFileName = f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]}.txt"
+            newSetFilePath = runOutputDir.joinpath(setFileName)
+            df.to_csv(newSetFilePath, quoting=quoting, index=False, header=False)
+
+    # Sort and remove duplicates from merged results.
+    logger.info("Sorting data and removing duplicates.")
+    listOfFiles = sorted(runOutputDir.iterdir())
+    for setFilePath in listOfFiles:
+        logger.info(f"""  Working on variable `setFilePath`: "{setFilePath.absolute().relative_to(rootDirectory)}".""")
+        try:
+            series = pd.read_table(setFilePath, header=None).iloc[:, 0]
+        except EmptyDataError as err:
+            _ = err
+            series = pd.Series(dtype=str)
+        logger.info(f"""    Starting size of variable set:               "{len(series):,}".""")
+        variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[setFilePath.stem]
+        dataType = DATA_TYPES_DICT[variableName]
+        if dataType == "Datetime":
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "Numeric":
+            series = series.astype(float).astype("Int64")
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "String":
+            quoting = csv.QUOTE_ALL
+        elif dataType == "Numeric_Or_String":
+            quoting = csv.QUOTE_ALL
+        else:
+            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
+        series = series.drop_duplicates().sort_values()
+        logger.info(f"""    Variable set size after removing duplicates: "{len(series):,}".""")
+        series.to_csv(setFilePath, quoting=quoting, index=False, header=False)
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-"""
-Variable constants common to this project
-"""
-
-__all__ = ["COLUMNS_TO_DE_IDENTIFY",
-           "BO_PORTION_DIR_MAC",
-           "BO_PORTION_DIR_WIN",
-           "MODIFIED_OMOP_PORTION_DIR_MAC",
-           "MODIFIED_OMOP_PORTION_DIR_WIN",
-           "MODIFIED_I2B2_PORTION_DIR_MAC",
-           "MODIFIED_I2B2_PORTION_DIR_WIN",
-           "NOTES_PORTION_DIR_MAC",
-           "NOTES_PORTION_DIR_WIN",
-           "OLD_MAPS_DIR_PATH",
-           "OMOP_PORTION_DIR_MAC",
-           "OMOP_PORTION_DIR_WIN",
-           "SDOH_PORTION_DIR_MAC",
-           "SDOH_PORTION_DIR_WIN"]
-
-from pathlib import Path
-# Local packages
-from drapi.constants.constants import DATA_TYPES_DICT
-from drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_BO,
-                                          LIST_OF_PHI_VARIABLES_I2B2,
-                                          LIST_OF_PHI_VARIABLES_NOTES,
-                                          LIST_OF_PHI_VARIABLES_OMOP,
-                                          VARIABLE_NAME_TO_FILE_NAME_DICT,
-                                          VARIABLE_SUFFIXES_BO,
-                                          VARIABLE_SUFFIXES_I2B2,
-                                          VARIABLE_SUFFIXES_NOTES,
-                                          VARIABLE_SUFFIXES_OMOP)
-from drapi.code.drapi.drapi import flatExtend
-
-# Project parameters: Meta-variables
-STUDY_TYPE = "Limited Data Set (LDS)"  # Pick from "Non-Human", "Limited Data Set (LDS)", "Identified"
-IRB_NUMBER = None  # TODO
-DATA_REQUEST_ROOT_DIRECTORY_DEPTH = 3  # TODO  # NOTE To prevent unexpected results, like moving, writing, or deleting the wrong files, set this to folder that is the immediate parent of concatenated result and the intermediate results folder.
-
-
-# Project parameters: Aliases: Definitions  # TODO
-# NOTE: Some variable names are not standardized. This section is used by the de-identification process when looking for the de-identification map. This way several variables can be de-identified with the same map. If you have variables with a custom, non-BO name, you should alias them, if necessary using the following format:
-# VAR_ALIASES_CUSTOM_VARS = {"Custom Variable 1": "BO Equivalent 1",
-#                            "Custom Variable 2": "BO Equivalent 2"}
-VAR_ALIASES_NOTES_ENCOUNTERS = {"EncounterCSN": "Encounter # (CSN)"}
-VAR_ALIASES_NOTES_PATIENTS = {"MRN_GNV": "MRN (UF)",
-                              "MRN_JAX": "MRN (Jax)",
-                              "PatientKey": "Patient Key"}
-VAR_ALIASES_NOTES_PROVIDERS = {"AuthoringProviderKey": "ProviderKey",
-                               "AuthorizingProviderKey": "ProviderKey",
-                               "CosignProviderKey": "ProviderKey",
-                               "OrderingProviderKey": "ProviderKey"}
-VAR_ALIASES_SDOH_ENCOUNTERS = {"NOTE_ENCNTR_KEY": "LinkageNoteID",
-                               "NOTE_KEY": "NoteKey"}
-LIST_OF_ALIAS_DICTS = [VAR_ALIASES_NOTES_ENCOUNTERS,
-                       VAR_ALIASES_NOTES_PATIENTS,
-                       VAR_ALIASES_NOTES_PROVIDERS,
-                       VAR_ALIASES_SDOH_ENCOUNTERS]
-VARIABLE_ALIASES = {}
-for di in LIST_OF_ALIAS_DICTS:
-    VARIABLE_ALIASES.update(di)
-
-# Project parameters: Aliases: Data types  # TODO
-# NOTE Add each variable in `VARIABLE_ALIASES` to `ALIAS_DATA_TYPES`.
-ALIAS_DATA_TYPES_MANUAL = {}  # TODO
-ALIAS_DATA_TYPES_AUTOMATIC = {}
-for alias, variableName in VARIABLE_ALIASES.items():
-    if alias not in DATA_TYPES_DICT.keys():
-        ALIAS_DATA_TYPES_AUTOMATIC[alias] = DATA_TYPES_DICT[variableName]
-    else:
-        pass
-ALIAS_DATA_TYPES = ALIAS_DATA_TYPES_MANUAL.copy()
-ALIAS_DATA_TYPES.update(ALIAS_DATA_TYPES_AUTOMATIC)
-DATA_TYPES_DICT.update(ALIAS_DATA_TYPES)
-
-# Project parameters: Aliases: Alias-to-File-name conversion  # TODO
-VARIABLES_TO_OVER_WRITE_MANUALLY = {}  # TODO
-VARIABLES_TO_ADD_FROM_ALIASES = {variableName: variableName for variableName in VARIABLE_ALIASES.keys()}
-VARIABLES_TO_OVER_WRITE_LIST = [VARIABLES_TO_ADD_FROM_ALIASES,
-                                VARIABLES_TO_OVER_WRITE_MANUALLY]  # NOTE The manual list must go last, to over-write the automatic additions.
-VARIABLES_TO_ADD_DICT = {}
-for di in VARIABLES_TO_OVER_WRITE_LIST:
-    VARIABLES_TO_ADD_DICT.update(di)
-VARIABLE_NAME_TO_FILE_NAME_DICT.update(VARIABLES_TO_ADD_DICT)
-FILE_NAME_TO_VARIABLE_NAME_DICT = {fileName: varName for varName, fileName in VARIABLE_NAME_TO_FILE_NAME_DICT.items()}
-
-# QA: Make sure all aliases have data types.
-li = []
-for alias in VARIABLE_ALIASES.keys():
-    if alias in DATA_TYPES_DICT.keys():
-        pass
-    else:
-        li.append(alias)
-if len(li) > 0:
-    string = "\n".join(sorted(li))
-    msg = f"""The following variable aliases have no data type assigned:\n{string}"""
-    raise Exception(msg)
-
-# Add aliases to list of variables to de-identify by adding the keys from `VARIABLE_ALIASES` and `ALIAS_DATA_TYPES` to `COLUMNS_TO_DE_IDENTIFY`.
-LIST_OF_PHI_VARIABLES_FROM_ALIASES = [variableName for variableName in VARIABLE_ALIASES.keys()] + [variableName for variableName in ALIAS_DATA_TYPES.keys()]
-LIST_OF_PHI_VARIABLES_FROM_ALIASES = list(set(LIST_OF_PHI_VARIABLES_FROM_ALIASES))
-
-# Project parameters: Columns to de-identify
-if STUDY_TYPE.lower() == "Non-Human":
-    LIST_OF_PHI_VARIABLES_TO_KEEP = []
-else:
-    LIST_OF_PHI_VARIABLES_TO_KEEP = []
-COLUMNS_TO_DE_IDENTIFY = flatExtend([LIST_OF_PHI_VARIABLES_BO,
-                                     LIST_OF_PHI_VARIABLES_I2B2,
-                                     LIST_OF_PHI_VARIABLES_NOTES,
-                                     LIST_OF_PHI_VARIABLES_OMOP,
-                                     LIST_OF_PHI_VARIABLES_FROM_ALIASES])
-COLUMNS_TO_DE_IDENTIFY = [variableName for variableName in COLUMNS_TO_DE_IDENTIFY if variableName not in LIST_OF_PHI_VARIABLES_TO_KEEP]
-
-# Project parameters: Variable suffixes
-VARIABLE_SUFFIXES_LIST = [VARIABLE_SUFFIXES_BO,
-                          VARIABLE_SUFFIXES_I2B2,
-                          VARIABLE_SUFFIXES_NOTES,
-                          VARIABLE_SUFFIXES_OMOP]
-VARIABLE_SUFFIXES = dict()
-for variableSuffixDict in VARIABLE_SUFFIXES_LIST:
-    VARIABLE_SUFFIXES.update(variableSuffixDict)
-
-# Project parameters: Portion directories
-BO_PORTION_DIR_MAC = Path(r"../Intermediate Results/BO Portion/data/output/getData/...")  # TODO
-BO_PORTION_DIR_WIN = Path(r"..\Intermediate Results\BO Portion\data\output\getData\...")  # TODO
-
-
-I2B2_PORTION_DIR_MAC = Path(r"../Concatenated Results/data/output/i2b2ConvertIDs/...")  # TODO
-I2B2_PORTION_DIR_WIN = Path(r"..\Concatenated Results\data\output\i2b2ConvertIDs\...")  # TODO
-
-MODIFIED_OMOP_PORTION_DIR_MAC = Path("data/output/convertColumns/...")  # TODO
-MODIFIED_OMOP_PORTION_DIR_WIN = Path(r"data\output\convertColumns\...")  # TODO
-
-MODIFIED_I2B2_PORTION_DIR_MAC = Path(r"../Concatenated Results/data/output/i2b2ConvertIDs/...")  # TODO
-MODIFIED_I2B2_PORTION_DIR_WIN = Path(r"..\Concatenated Results\data\output\i2b2ConvertIDs\...")  # TODO
-
-NOTES_ROOT_DIRECTORY = Path(r"..\Intermediate Results\Notes Data Portion\data\output\2023-11-20 16-37-27")  # TODO
-NOTES_PORTION_DIR_MAC = NOTES_ROOT_DIRECTORY.joinpath("free_text")
-NOTES_PORTION_DIR_WIN = NOTES_ROOT_DIRECTORY.joinpath("free_text")
-
-OMOP_PORTION_DIR_MAC = Path(r"Intermediate Results/OMOP Portion/data/output/...")  # TODO
-OMOP_PORTION_DIR_WIN = Path(r"Intermediate Results\OMOP Portion\data\output\...")  # TODO
-
-SDOH_PORTION_DIR_MAC = Path(r"..\Intermediate Results\SDoH Portion")  # TODO
-SDOH_PORTION_DIR_WIN = Path(r"..\Intermediate Results\SDoH Portion")  # TODO
-
-# Project parameters: File criteria
-BO_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
-I2B2_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
-NOTES_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
-OMOP_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
-SDOH_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".tsv"]
-
-
-# Project parameters: Maps
-OLD_MAPS_DIR_PATH = {"EncounterCSN": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_encounter.csv")],
-                     "LinkageNoteID": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_note_link.csv")],
-                     "NoteKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_note.csv")],
-                     "OrderKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_order.csv")],
-                     "PatientKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_patient.csv")],
-                     "ProviderKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_provider.csv")]}
-
-# Quality assurance
-if __name__ == "__main__":
-    ALL_VARS = [BO_PORTION_DIR_MAC,
-                BO_PORTION_DIR_WIN,
-                I2B2_PORTION_DIR_MAC,
-                I2B2_PORTION_DIR_WIN,
-                MODIFIED_OMOP_PORTION_DIR_MAC,
-                MODIFIED_OMOP_PORTION_DIR_WIN,
-                MODIFIED_I2B2_PORTION_DIR_MAC,
-                MODIFIED_I2B2_PORTION_DIR_WIN,
-                NOTES_ROOT_DIRECTORY,
-                NOTES_PORTION_DIR_MAC,
-                NOTES_PORTION_DIR_WIN,
-                OMOP_PORTION_DIR_MAC,
-                OMOP_PORTION_DIR_WIN,
-                SDOH_PORTION_DIR_MAC,
-                SDOH_PORTION_DIR_WIN]
-
-    for li in OLD_MAPS_DIR_PATH.values():
-        ALL_VARS.extend(li)
-
-    for path in ALL_VARS:
-        print(path.exists())
+"""
+Variable constants common to this project
+"""
+
+__all__ = ["COLUMNS_TO_DE_IDENTIFY",
+           "BO_PORTION_DIR_MAC",
+           "BO_PORTION_DIR_WIN",
+           "MODIFIED_OMOP_PORTION_DIR_MAC",
+           "MODIFIED_OMOP_PORTION_DIR_WIN",
+           "MODIFIED_I2B2_PORTION_DIR_MAC",
+           "MODIFIED_I2B2_PORTION_DIR_WIN",
+           "NOTES_PORTION_DIR_MAC",
+           "NOTES_PORTION_DIR_WIN",
+           "OLD_MAPS_DIR_PATH",
+           "OMOP_PORTION_DIR_MAC",
+           "OMOP_PORTION_DIR_WIN",
+           "SDOH_PORTION_DIR_MAC",
+           "SDOH_PORTION_DIR_WIN"]
+
+from pathlib import Path
+# Local packages
+from drapi.constants.constants import DATA_TYPES_DICT
+from drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_BO,
+                                          LIST_OF_PHI_VARIABLES_I2B2,
+                                          LIST_OF_PHI_VARIABLES_NOTES,
+                                          LIST_OF_PHI_VARIABLES_OMOP,
+                                          VARIABLE_NAME_TO_FILE_NAME_DICT,
+                                          VARIABLE_SUFFIXES_BO,
+                                          VARIABLE_SUFFIXES_I2B2,
+                                          VARIABLE_SUFFIXES_NOTES,
+                                          VARIABLE_SUFFIXES_OMOP)
+from drapi.code.drapi.drapi import flatExtend
+
+# Project parameters: Meta-variables
+STUDY_TYPE = "Limited Data Set (LDS)"  # Pick from "Non-Human", "Limited Data Set (LDS)", "Identified"
+IRB_NUMBER = None  # TODO
+DATA_REQUEST_ROOT_DIRECTORY_DEPTH = 3  # TODO  # NOTE To prevent unexpected results, like moving, writing, or deleting the wrong files, set this to folder that is the immediate parent of concatenated result and the intermediate results folder.
+
+
+# Project parameters: Aliases: Definitions  # TODO
+# NOTE: Some variable names are not standardized. This section is used by the de-identification process when looking for the de-identification map. This way several variables can be de-identified with the same map. If you have variables with a custom, non-BO name, you should alias them, if necessary using the following format:
+# VAR_ALIASES_CUSTOM_VARS = {"Custom Variable 1": "BO Equivalent 1",
+#                            "Custom Variable 2": "BO Equivalent 2"}
+VAR_ALIASES_NOTES_ENCOUNTERS = {"EncounterCSN": "Encounter # (CSN)"}
+VAR_ALIASES_NOTES_PATIENTS = {"MRN_GNV": "MRN (UF)",
+                              "MRN_JAX": "MRN (Jax)",
+                              "PatientKey": "Patient Key"}
+VAR_ALIASES_NOTES_PROVIDERS = {"AuthoringProviderKey": "ProviderKey",
+                               "AuthorizingProviderKey": "ProviderKey",
+                               "CosignProviderKey": "ProviderKey",
+                               "OrderingProviderKey": "ProviderKey"}
+VAR_ALIASES_SDOH_ENCOUNTERS = {"NOTE_ENCNTR_KEY": "LinkageNoteID",
+                               "NOTE_KEY": "NoteKey"}
+LIST_OF_ALIAS_DICTS = [VAR_ALIASES_NOTES_ENCOUNTERS,
+                       VAR_ALIASES_NOTES_PATIENTS,
+                       VAR_ALIASES_NOTES_PROVIDERS,
+                       VAR_ALIASES_SDOH_ENCOUNTERS]
+VARIABLE_ALIASES = {}
+for di in LIST_OF_ALIAS_DICTS:
+    VARIABLE_ALIASES.update(di)
+
+# Project parameters: Aliases: Data types  # TODO
+# NOTE Add each variable in `VARIABLE_ALIASES` to `ALIAS_DATA_TYPES`.
+ALIAS_DATA_TYPES_MANUAL = {}  # TODO
+ALIAS_DATA_TYPES_AUTOMATIC = {}
+for alias, variableName in VARIABLE_ALIASES.items():
+    if alias not in DATA_TYPES_DICT.keys():
+        ALIAS_DATA_TYPES_AUTOMATIC[alias] = DATA_TYPES_DICT[variableName]
+    else:
+        pass
+ALIAS_DATA_TYPES = ALIAS_DATA_TYPES_MANUAL.copy()
+ALIAS_DATA_TYPES.update(ALIAS_DATA_TYPES_AUTOMATIC)
+DATA_TYPES_DICT.update(ALIAS_DATA_TYPES)
+
+# Project parameters: Aliases: Alias-to-File-name conversion  # TODO
+VARIABLES_TO_OVER_WRITE_MANUALLY = {}  # TODO
+VARIABLES_TO_ADD_FROM_ALIASES = {variableName: variableName for variableName in VARIABLE_ALIASES.keys()}
+VARIABLES_TO_OVER_WRITE_LIST = [VARIABLES_TO_ADD_FROM_ALIASES,
+                                VARIABLES_TO_OVER_WRITE_MANUALLY]  # NOTE The manual list must go last, to over-write the automatic additions.
+VARIABLES_TO_ADD_DICT = {}
+for di in VARIABLES_TO_OVER_WRITE_LIST:
+    VARIABLES_TO_ADD_DICT.update(di)
+VARIABLE_NAME_TO_FILE_NAME_DICT.update(VARIABLES_TO_ADD_DICT)
+FILE_NAME_TO_VARIABLE_NAME_DICT = {fileName: varName for varName, fileName in VARIABLE_NAME_TO_FILE_NAME_DICT.items()}
+
+# QA: Make sure all aliases have data types.
+li = []
+for alias in VARIABLE_ALIASES.keys():
+    if alias in DATA_TYPES_DICT.keys():
+        pass
+    else:
+        li.append(alias)
+if len(li) > 0:
+    string = "\n".join(sorted(li))
+    msg = f"""The following variable aliases have no data type assigned:\n{string}"""
+    raise Exception(msg)
+
+# Add aliases to list of variables to de-identify by adding the keys from `VARIABLE_ALIASES` and `ALIAS_DATA_TYPES` to `COLUMNS_TO_DE_IDENTIFY`.
+LIST_OF_PHI_VARIABLES_FROM_ALIASES = [variableName for variableName in VARIABLE_ALIASES.keys()] + [variableName for variableName in ALIAS_DATA_TYPES.keys()]
+LIST_OF_PHI_VARIABLES_FROM_ALIASES = list(set(LIST_OF_PHI_VARIABLES_FROM_ALIASES))
+
+# Project parameters: Columns to de-identify
+if STUDY_TYPE.lower() == "Non-Human":
+    LIST_OF_PHI_VARIABLES_TO_KEEP = []
+else:
+    LIST_OF_PHI_VARIABLES_TO_KEEP = []
+COLUMNS_TO_DE_IDENTIFY = flatExtend([LIST_OF_PHI_VARIABLES_BO,
+                                     LIST_OF_PHI_VARIABLES_I2B2,
+                                     LIST_OF_PHI_VARIABLES_NOTES,
+                                     LIST_OF_PHI_VARIABLES_OMOP,
+                                     LIST_OF_PHI_VARIABLES_FROM_ALIASES])
+COLUMNS_TO_DE_IDENTIFY = [variableName for variableName in COLUMNS_TO_DE_IDENTIFY if variableName not in LIST_OF_PHI_VARIABLES_TO_KEEP]
+
+# Project parameters: Variable suffixes
+VARIABLE_SUFFIXES_LIST = [VARIABLE_SUFFIXES_BO,
+                          VARIABLE_SUFFIXES_I2B2,
+                          VARIABLE_SUFFIXES_NOTES,
+                          VARIABLE_SUFFIXES_OMOP]
+VARIABLE_SUFFIXES = dict()
+for variableSuffixDict in VARIABLE_SUFFIXES_LIST:
+    VARIABLE_SUFFIXES.update(variableSuffixDict)
+
+# Project parameters: Portion directories
+BO_PORTION_DIR_MAC = Path(r"../Intermediate Results/BO Portion/data/output/getData/...")  # TODO
+BO_PORTION_DIR_WIN = Path(r"..\Intermediate Results\BO Portion\data\output\getData\...")  # TODO
+
+
+I2B2_PORTION_DIR_MAC = Path(r"../Concatenated Results/data/output/i2b2ConvertIDs/...")  # TODO
+I2B2_PORTION_DIR_WIN = Path(r"..\Concatenated Results\data\output\i2b2ConvertIDs\...")  # TODO
+
+MODIFIED_OMOP_PORTION_DIR_MAC = Path("data/output/convertColumns/...")  # TODO
+MODIFIED_OMOP_PORTION_DIR_WIN = Path(r"data\output\convertColumns\...")  # TODO
+
+MODIFIED_I2B2_PORTION_DIR_MAC = Path(r"../Concatenated Results/data/output/i2b2ConvertIDs/...")  # TODO
+MODIFIED_I2B2_PORTION_DIR_WIN = Path(r"..\Concatenated Results\data\output\i2b2ConvertIDs\...")  # TODO
+
+NOTES_ROOT_DIRECTORY = Path(r"..\Intermediate Results\Notes Data Portion\data\output\2023-11-20 16-37-27")  # TODO
+NOTES_PORTION_DIR_MAC = NOTES_ROOT_DIRECTORY.joinpath("free_text")
+NOTES_PORTION_DIR_WIN = NOTES_ROOT_DIRECTORY.joinpath("free_text")
+
+OMOP_PORTION_DIR_MAC = Path(r"Intermediate Results/OMOP Portion/data/output/...")  # TODO
+OMOP_PORTION_DIR_WIN = Path(r"Intermediate Results\OMOP Portion\data\output\...")  # TODO
+
+SDOH_PORTION_DIR_MAC = Path(r"..\Intermediate Results\SDoH Portion")  # TODO
+SDOH_PORTION_DIR_WIN = Path(r"..\Intermediate Results\SDoH Portion")  # TODO
+
+# Project parameters: File criteria
+BO_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+I2B2_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+NOTES_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+OMOP_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+SDOH_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".tsv"]
+
+
+# Project parameters: Maps
+OLD_MAPS_DIR_PATH = {"EncounterCSN": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_encounter.csv")],
+                     "LinkageNoteID": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_note_link.csv")],
+                     "NoteKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_note.csv")],
+                     "OrderKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_order.csv")],
+                     "PatientKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_patient.csv")],
+                     "ProviderKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_provider.csv")]}
+
+# Quality assurance
+if __name__ == "__main__":
+    ALL_VARS = [BO_PORTION_DIR_MAC,
+                BO_PORTION_DIR_WIN,
+                I2B2_PORTION_DIR_MAC,
+                I2B2_PORTION_DIR_WIN,
+                MODIFIED_OMOP_PORTION_DIR_MAC,
+                MODIFIED_OMOP_PORTION_DIR_WIN,
+                MODIFIED_I2B2_PORTION_DIR_MAC,
+                MODIFIED_I2B2_PORTION_DIR_WIN,
+                NOTES_ROOT_DIRECTORY,
+                NOTES_PORTION_DIR_MAC,
+                NOTES_PORTION_DIR_WIN,
+                OMOP_PORTION_DIR_MAC,
+                OMOP_PORTION_DIR_WIN,
+                SDOH_PORTION_DIR_MAC,
+                SDOH_PORTION_DIR_WIN]
+
+    for li in OLD_MAPS_DIR_PATH.values():
+        ALL_VARS.extend(li)
+
+    for path in ALL_VARS:
+        print(path.exists())
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-"""
-Makes de-identification maps, building on existing maps.
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-"""
-
-import logging
-import re
-from collections import OrderedDict
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-import pprint
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    getPercentDifference,
-                                    successiveParents,
-                                    makeMap)
-from drapi.constants.phiVariables import (VARIABLE_NAME_TO_FILE_NAME_DICT,
-                                          FILE_NAME_TO_VARIABLE_NAME_DICT)
-# Project parameters: General
-from common import (IRB_NUMBER,
-                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    OLD_MAPS_DIR_PATH,
-                    VARIABLE_ALIASES,
-                    VARIABLE_SUFFIXES)
-
-# Arguments
-NEW_MAPS_DIR_PATH = Path(r"..\Concatenated Results\data\output\makeMapsFromOthers\...")  # TODO
-DE_IDENTIFICATION_MAP_STYLE = "lemur"
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Map new maps to variable names
-    logging.info("""Mapping new maps to variable names.""")
-    pattern = r"^([a-zA-Z_0-9\(\)# -]+) map"
-    newMapsFileDict = {}
-    for fpath in NEW_MAPS_DIR_PATH.iterdir():
-        fname = fpath.stem
-        obj = re.match(pattern, fname)
-        if obj:
-            extractedText = obj.groups()[0]
-            variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[extractedText]
-        else:
-            msg = "File name is of an unexpected format."
-            logging.info(msg)
-            raise Exception(msg)
-        newMapsFileDict[variableName] = [fpath]
-    logging.info("The list of variables extracted from the new maps:")
-    for el in sorted(newMapsFileDict.keys()):
-        logging.info(f"  {el}")
-
-    # Match old and new maps by variable name
-    logging.info("""Matching old and new maps by variable name.""")
-    matchedMaps0 = {}
-    MAPS_COLLECTION_DICT = {"Old Maps": OLD_MAPS_DIR_PATH,
-                            "New Maps": newMapsFileDict}
-    for mapCollectionName, mapCollection in MAPS_COLLECTION_DICT.items():
-        logging.info(f"""  Working on map collection "{mapCollectionName}".""")
-        for variableName, li in mapCollection.items():
-            if variableName in VARIABLE_ALIASES.keys():
-                variableLookUpName = VARIABLE_ALIASES[variableName]
-            else:
-                variableLookUpName = variableName
-            if variableLookUpName in matchedMaps0.keys():
-                matchedMaps0[variableLookUpName].extend(li)
-            else:
-                matchedMaps0[variableLookUpName] = li
-    matchedMaps = OrderedDict()
-    for key in sorted(matchedMaps0.keys()):
-        matchedMaps[key] = matchedMaps0[key]
-    text = pprint.pformat(matchedMaps, indent=4)
-    logging.info(f"""  The old and new maps have been matched to the variable names. Aliases have been used:\n{text}""")
-
-    # Load, concatenate, and save maps by variable names
-    logging.info("""Loading, concatenating, and saving maps by variable names.""")
-    concatenatedMapsDict = {}
-    for variableName, li in matchedMaps.items():
-        logging.info(f"""  Working on variable "{variableName}".""")
-        concatenatedMap = pd.DataFrame()
-        emptyMap = makeMap(IDset=set(),
-                           IDName=variableName,
-                           startFrom=1,
-                           irbNumber=IRB_NUMBER,
-                           suffix=VARIABLE_SUFFIXES[variableName]["deIdIDSuffix"],
-                           columnSuffix=variableName,
-                           deIdentificationMapStyle=DE_IDENTIFICATION_MAP_STYLE,
-                           logger=logging.getLogger())
-        newColumns = emptyMap.columns
-        for fpath in li:
-            fpath = Path(fpath)
-            logging.info(f"""    Working on map located at "{fpath.absolute().relative_to(rootDirectory)}".""")
-            df = pd.read_csv(fpath)
-            oldColumns = df.columns
-            logging.info(f"""  ..  Over-writing map header format to "{DE_IDENTIFICATION_MAP_STYLE}".""")
-            logging.info(f"""  ..  Old map columns: {oldColumns.to_list()}.""")
-            logging.info(f"""  ..  New map columns: {newColumns.to_list()}.""")
-            df.columns = newColumns
-            concatenatedMap = pd.concat([concatenatedMap, df])
-        concatenatedMapsDict[variableName] = concatenatedMap
-        fpath = runOutputDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]} map.csv")
-        concatenatedMap.to_csv(fpath, index=False)
-
-    # Quality control
-    results = {}
-    for variableName, df in concatenatedMapsDict.items():
-        uniqueIDs = len(df.iloc[:, 0].unique())
-        numIDs = len(df)
-        percentDifference = getPercentDifference(uniqueIDs, numIDs)
-        results[variableName] = {"Unique IDs": uniqueIDs,
-                                 "Total IDs": numIDs,
-                                 "Percent Similarity": percentDifference}
-    resultsdf = pd.DataFrame.from_dict(results, orient="index")
-    logging.info(f"Concatenation summary:\n{resultsdf.to_string()}")
-
-    # Clean up
-    # TODO If input directory is empty, delete
-    # TODO Delete intermediate run directory
-
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Makes de-identification maps, building on existing maps.
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+"""
+
+import logging
+import re
+from collections import OrderedDict
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+import pprint
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    getPercentDifference,
+                                    successiveParents,
+                                    makeMap)
+from drapi.constants.phiVariables import (VARIABLE_NAME_TO_FILE_NAME_DICT,
+                                          FILE_NAME_TO_VARIABLE_NAME_DICT)
+# Project parameters: General
+from common import (IRB_NUMBER,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
+                    OLD_MAPS_DIR_PATH,
+                    VARIABLE_ALIASES,
+                    VARIABLE_SUFFIXES)
+
+# Arguments
+NEW_MAPS_DIR_PATH = Path(r"..\Concatenated Results\data\output\makeMapsFromOthers\...")  # TODO
+DE_IDENTIFICATION_MAP_STYLE = "lemur"
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # Map new maps to variable names
+    logging.info("""Mapping new maps to variable names.""")
+    pattern = r"^([a-zA-Z_0-9\(\)# -]+) map"
+    newMapsFileDict = {}
+    for fpath in NEW_MAPS_DIR_PATH.iterdir():
+        fname = fpath.stem
+        obj = re.match(pattern, fname)
+        if obj:
+            extractedText = obj.groups()[0]
+            variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[extractedText]
+        else:
+            msg = "File name is of an unexpected format."
+            logging.info(msg)
+            raise Exception(msg)
+        newMapsFileDict[variableName] = [fpath]
+    logging.info("The list of variables extracted from the new maps:")
+    for el in sorted(newMapsFileDict.keys()):
+        logging.info(f"  {el}")
+
+    # Match old and new maps by variable name
+    logging.info("""Matching old and new maps by variable name.""")
+    matchedMaps0 = {}
+    MAPS_COLLECTION_DICT = {"Old Maps": OLD_MAPS_DIR_PATH,
+                            "New Maps": newMapsFileDict}
+    for mapCollectionName, mapCollection in MAPS_COLLECTION_DICT.items():
+        logging.info(f"""  Working on map collection "{mapCollectionName}".""")
+        for variableName, li in mapCollection.items():
+            if variableName in VARIABLE_ALIASES.keys():
+                variableLookUpName = VARIABLE_ALIASES[variableName]
+            else:
+                variableLookUpName = variableName
+            if variableLookUpName in matchedMaps0.keys():
+                matchedMaps0[variableLookUpName].extend(li)
+            else:
+                matchedMaps0[variableLookUpName] = li
+    matchedMaps = OrderedDict()
+    for key in sorted(matchedMaps0.keys()):
+        matchedMaps[key] = matchedMaps0[key]
+    text = pprint.pformat(matchedMaps, indent=4)
+    logging.info(f"""  The old and new maps have been matched to the variable names. Aliases have been used:\n{text}""")
+
+    # Load, concatenate, and save maps by variable names
+    logging.info("""Loading, concatenating, and saving maps by variable names.""")
+    concatenatedMapsDict = {}
+    for variableName, li in matchedMaps.items():
+        logging.info(f"""  Working on variable "{variableName}".""")
+        concatenatedMap = pd.DataFrame()
+        emptyMap = makeMap(IDset=set(),
+                           IDName=variableName,
+                           startFrom=1,
+                           irbNumber=IRB_NUMBER,
+                           suffix=VARIABLE_SUFFIXES[variableName]["deIdIDSuffix"],
+                           columnSuffix=variableName,
+                           deIdentificationMapStyle=DE_IDENTIFICATION_MAP_STYLE,
+                           logger=logging.getLogger())
+        newColumns = emptyMap.columns
+        for fpath in li:
+            fpath = Path(fpath)
+            logging.info(f"""    Working on map located at "{fpath.absolute().relative_to(rootDirectory)}".""")
+            df = pd.read_csv(fpath)
+            oldColumns = df.columns
+            logging.info(f"""  ..  Over-writing map header format to "{DE_IDENTIFICATION_MAP_STYLE}".""")
+            logging.info(f"""  ..  Old map columns: {oldColumns.to_list()}.""")
+            logging.info(f"""  ..  New map columns: {newColumns.to_list()}.""")
+            df.columns = newColumns
+            concatenatedMap = pd.concat([concatenatedMap, df])
+        concatenatedMapsDict[variableName] = concatenatedMap
+        fpath = runOutputDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]} map.csv")
+        concatenatedMap.to_csv(fpath, index=False)
+
+    # Quality control
+    results = {}
+    for variableName, df in concatenatedMapsDict.items():
+        uniqueIDs = len(df.iloc[:, 0].unique())
+        numIDs = len(df)
+        percentDifference = getPercentDifference(uniqueIDs, numIDs)
+        results[variableName] = {"Unique IDs": uniqueIDs,
+                                 "Total IDs": numIDs,
+                                 "Percent Similarity": percentDifference}
+    resultsdf = pd.DataFrame.from_dict(results, orient="index")
+    logging.info(f"Concatenation summary:\n{resultsdf.to_string()}")
+
+    # Clean up
+    # TODO If input directory is empty, delete
+    # TODO Delete intermediate run directory
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/gatherFiles.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,223 @@
-"""
-Convert person ID column to patient key
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-"""
-
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    readDataFile,
-                                    successiveParents)
-from drapi.idealist.idealist import idealistMap2dict
-# Local packages: Script parameters: General
-from common import DATA_REQUEST_ROOT_DIRECTORY_DEPTH
-# Local packages: Script parameters: Paths
-from common import OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN
-# Local packages: Script parameters: File criteria
-from common import OMOP_PORTION_FILE_CRITERIA
-
-# Arguments
-COLUMNS_TO_CONVERT_DI = {"person_id": "Patient Key"}
-
-MAC_PATHS = [OMOP_PORTION_DIR_MAC]
-WIN_PATHS = [OMOP_PORTION_DIR_WIN]
-
-LIST_OF_PORTION_CONDITIONS = [OMOP_PORTION_FILE_CRITERIA]
-
-PERSON_ID_MAP_PATH = Path(r"..\Intermediate Results\OMOP Portion\data\output\getPersonIDs\...\personIDsFound.csv")  # TODO
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Load person ID map
-    personIDMap = pd.read_csv(PERSON_ID_MAP_PATH)
-    personIDMapDi = idealistMap2dict(personIDMap, "person_id", "Patient Key")
-
-    # Convert columns
-    logging.info("""Getting the set of values for each variable to convert.""")
-    # Create file parameters dictionary
-
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logging.info(f"""Working on directory "{directory.relative_to(IRBDir)}".""")
-        for file in directory.iterdir():
-            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logging.info("""    File has met all conditions for processing.""")
-                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
-                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        logging.info(f"""  ..    Working on column "{columnName}".""")
-                        if columnName in COLUMNS_TO_CONVERT_DI.keys():
-                            logging.info("""  ..  ..  Column must be converted. Converting values.""")
-                            dfChunk[columnName] = dfChunk[columnName].apply(lambda IDNum: personIDMapDi[IDNum])
-                            dfChunk = dfChunk.rename(columns={columnName: COLUMNS_TO_CONVERT_DI[columnName]})
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logging.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logging.info("""    This file does not need to be processed.""")
-
-    # Clean up
-    # TODO If input directory is empty, delete
-    # TODO Delete intermediate run directory
-
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Copy files to a single destination directory. Optionally this directory can be added to a compressed archive.
+"""
+
+import logging
+import os
+import shutil
+import zipfile
+from pathlib import Path
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+LIST_OF_DIRECTORIES = []
+LIST_OF_FILES = []
+DESTINATION_FOLDER = fr"..\Concatenated Results\disclosure\{getTimestamp()}"
+
+OVERWRITE_IF_EXISTS_FOLDER = False
+OVERWRITE_IF_EXISTS_FILE = False
+
+CREATE_COMPRESSED_ARCHIVE = True
+DELETE_FOLDER_AFTER_ARCHIVING = True
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 1
+IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 4
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `LIST_OF_DIRECTORIES`: "{LIST_OF_DIRECTORIES}"
+    `LIST_OF_FILES`: "{LIST_OF_FILES}"
+    `DESTINATION_FOLDER`: "{DESTINATION_FOLDER}"
+    `OVERWRITE_IF_EXISTS_FOLDER`: "{OVERWRITE_IF_EXISTS_FOLDER}"
+    `OVERWRITE_IF_EXISTS_FILE`: "{OVERWRITE_IF_EXISTS_FILE}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Define the destination path
+    destinationFolder = Path(DESTINATION_FOLDER)
+
+    # Copy files and directories
+    if destinationFolder.exists():
+        logger.warning(f"""WARNING: The destination folder already exists: "{destinationFolder.absolute().relative_to(rootDirectory)}".""")
+        if OVERWRITE_IF_EXISTS_FOLDER:
+            logger.info("""  Removing folder contents to make room for new files.""")
+            for fpath in destinationFolder.iterdir():
+                logger.info(f"""    Removing "{fpath.absolute().relative_to(rootDirectory)}".""")
+                os.remove(fpath)
+                logger.info(f"""    Removing "{fpath.absolute().relative_to(rootDirectory)}" - done.""")
+        else:
+            msg = "  The destination folder exists and no option was passed to over-write it."
+            logger.fatal(msg)
+            raise Exception(msg)
+    else:
+        logger.info(f"""Making destination folder: "{destinationFolder.absolute().relative_to(rootDirectory)}".""")
+        makeDirPath(destinationFolder)
+
+    logger.info("""Working on list of files.""")
+    for fpathString in LIST_OF_FILES:
+        fpath = Path(fpathString)
+        logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+        dest = destinationFolder.joinpath(fpath.name)
+        logger.info(f"""    Saving to "{dest.absolute().relative_to(rootDirectory)}".""")
+        shutil.copyfile(fpath, dest)
+    logger.info("""Working on list of files - done.""")
+
+    logger.info("""Working on list of directories.""")
+    for directoryString in LIST_OF_DIRECTORIES:
+        directory = Path(directoryString)
+        for fpath in directory.iterdir():
+            logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+            dest = destinationFolder.joinpath(fpath.name)
+            logger.info(f"""    The destination path is "{dest.absolute().relative_to(rootDirectory)}".""")
+            if dest.exists():
+                msg = f"""    WARNING: This file already exists: "{dest}"."""
+                logger.warning(msg)
+                if OVERWRITE_IF_EXISTS_FILE:
+                    continueOperation = True
+                else:
+                    continueOperation = False
+            else:
+                continueOperation = True
+            if continueOperation:
+                logger.info("""    Saving to destination path.""")
+                shutil.copyfile(fpath, dest)
+            else:
+                logger.info("""    The file was not saved to the destination path. File over-write is set to `False`.""")
+    logger.info("""Working on list of directories - done.""")
+
+    # Create compressed archive
+    if CREATE_COMPRESSED_ARCHIVE:
+        archivePath = destinationFolder.with_suffix(".ZIP")
+        logger.info(f"""Creating compressed archive: "{archivePath.absolute().relative_to(rootDirectory)}"".""")
+        if archivePath.exists():
+            logger.info("""The archive folder already exists and will be removed before writing.""")
+            os.remove(archivePath)
+        else:
+            pass
+
+        with zipfile.ZipFile(file=archivePath,
+                             mode="a",
+                             compression=zipfile.ZIP_DEFLATED) as zipObj:
+            logger.info("Adding files to archive.")
+            for fpath in destinationFolder.iterdir():
+                logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+                newPath = fpath.name
+                zipObj.write(filename=fpath, arcname=newPath)
+        logger.info("Creating compressed archive - done.")
+
+        if DELETE_FOLDER_AFTER_ARCHIVING:
+            logger.info("""Removing intermediate folder.""")
+            shutil.rmtree(destinationFolder)
+            logger.info("""Removing intermediate folder - done.""")
+        else:
+            pass
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/dataQualityTest.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,166 @@
-"""
-Iterates over the files that would be processed in the pipeline and runs quality tests on them. Currently the quality tests are
-
-  1. Check for delimmeter issues. This is done by reading the whole file with `pd.read_csv`. Usually if there's an unexpected presence or absence of a delimmeter this will raise an error.
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-"""
-
-__all__ = ["runIntermediateDataDir"]
-
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-from pandas.errors import ParserError
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    readDataFile,
-                                    successiveParents)
-from common import (DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    BO_PORTION_DIR_MAC,
-                    BO_PORTION_DIR_WIN,
-                    BO_PORTION_FILE_CRITERIA)
-
-# Arguments
-CHUNK_SIZE = 50000
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Arguments: Portion Paths and conditions
-MAC_PATHS = [BO_PORTION_DIR_MAC]
-WIN_PATHS = [BO_PORTION_DIR_WIN]
-
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Data quality check
-    logging.info("""Getting the set of values for each variable to de-identify.""")
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Read file
-                logging.info("""    This file has met all conditions for testing.""")
-                # Test 1: Make sure all lines have the same number of delimiters
-                logging.info("""  ..  Test 1: Make sure all lines have the same number of delimiters.""")
-                try:
-                    numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
-                    logging.info("""  ..    There are no apparent problems reading this file.""")
-                except ParserError as err:
-                    args = err
-                    logging.info("""  ..    This file raised an error: "{err}".""")
-                # Test 2: ...
-                pass
-            else:
-                logging.info("""    This file does not need to be tested.""")
-
-    # Return path to sets fo ID values
-    # TODO If this is implemented as a function, instead of a stand-alone script, return `runOutputDir` to define `setsPathDir` in the "makeMap" scripts.
-    logging.info(f"""Finished collecting the set of ID values to de-identify. The set files are located in "{runOutputDir.relative_to(projectDir)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Convert person ID column to patient key
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+"""
+
+import logging
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    readDataFile,
+                                    successiveParents)
+from drapi.idealist.idealist import idealistMap2dict
+# Local packages: Script parameters: General
+from common import DATA_REQUEST_ROOT_DIRECTORY_DEPTH
+# Local packages: Script parameters: Paths
+from common import OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN
+# Local packages: Script parameters: File criteria
+from common import OMOP_PORTION_FILE_CRITERIA
+
+# Arguments
+COLUMNS_TO_CONVERT_DI = {"person_id": "Patient Key"}
+
+MAC_PATHS = [OMOP_PORTION_DIR_MAC]
+WIN_PATHS = [OMOP_PORTION_DIR_WIN]
+
+LIST_OF_PORTION_CONDITIONS = [OMOP_PORTION_FILE_CRITERIA]
+
+PERSON_ID_MAP_PATH = Path(r"..\Intermediate Results\OMOP Portion\data\output\getPersonIDs\...\personIDsFound.csv")  # TODO
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # Load person ID map
+    personIDMap = pd.read_csv(PERSON_ID_MAP_PATH)
+    personIDMapDi = idealistMap2dict(personIDMap, "person_id", "Patient Key")
+
+    # Convert columns
+    logging.info("""Getting the set of values for each variable to convert.""")
+    # Create file parameters dictionary
+
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logging.info(f"""Working on directory "{directory.relative_to(IRBDir)}".""")
+        for file in directory.iterdir():
+            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logging.info("""    File has met all conditions for processing.""")
+                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        logging.info(f"""  ..    Working on column "{columnName}".""")
+                        if columnName in COLUMNS_TO_CONVERT_DI.keys():
+                            logging.info("""  ..  ..  Column must be converted. Converting values.""")
+                            dfChunk[columnName] = dfChunk[columnName].apply(lambda IDNum: personIDMapDi[IDNum])
+                            dfChunk = dfChunk.rename(columns={columnName: COLUMNS_TO_CONVERT_DI[columnName]})
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logging.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logging.info("""    This file does not need to be processed.""")
+
+    # Clean up
+    # TODO If input directory is empty, delete
+    # TODO Delete intermediate run directory
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-"""
-De-identify files
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-# TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
-"""
-
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (fileName2variableName,
-                                    getTimestamp,
-                                    makeDirPath,
-                                    makeMap,
-                                    map2di,
-                                    numericOrString2integerOrString,
-                                    readDataFile,
-                                    successiveParents)
-from drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
-                                          VARIABLE_NAME_TO_FILE_NAME_DICT)
-# Local packages: Script parameters: General
-from common import (IRB_NUMBER,
-                    ALIAS_DATA_TYPES,
-                    COLUMNS_TO_DE_IDENTIFY,
-                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    DATA_TYPES_DICT,
-                    VARIABLE_ALIASES,
-                    VARIABLE_SUFFIXES)
-# Local packages: Script parameters: Paths
-from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
-                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
-                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
-                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
-                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
-# Local packages: Script parameters: File criteria
-from common import (BO_PORTION_FILE_CRITERIA,
-                    I2B2_PORTION_FILE_CRITERIA,
-                    NOTES_PORTION_FILE_CRITERIA,
-                    OMOP_PORTION_FILE_CRITERIA)
-
-# Arguments
-CONCATENATED_MAPS_DIR_PATH = Path(r"..\Concatenated Results\data\output\concatenateMaps\...")  # TODO
-
-MAPS_DIR_PATH = CONCATENATED_MAPS_DIR_PATH
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Arguments: Portion Paths and conditions
-if USE_MODIFIED_OMOP_DATA_SET:
-    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
-else:
-    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
-
-MAC_PATHS = [BO_PORTION_DIR_MAC,
-             I2B2_PORTION_DIR_MAC,
-             NOTES_PORTION_DIR_MAC,
-             OMOPPortionDirMac]
-WIN_PATHS = [BO_PORTION_DIR_WIN,
-             I2B2_PORTION_DIR_WIN,
-             NOTES_PORTION_DIR_WIN,
-             OMOPPortionDirWin]
-
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA,
-                              I2B2_PORTION_FILE_CRITERIA,
-                              NOTES_PORTION_FILE_CRITERIA,
-                              OMOP_PORTION_FILE_CRITERIA]
-
-# Arguments; General
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Assert all portions have file criteria accounted for
-    if len(listOfPortionDirs) == len(LIST_OF_PORTION_CONDITIONS):
-        pass
-    else:
-        raise Exception("The number of portions does not equal the number of portion conditions.")
-
-    # Load de-identification maps for each variable that needs to be de-identified
-    logging.info("""Loading de-identification maps for each variable that needs to be de-identified.""")
-    mapsDi = {}
-    mapsColumnNames = {}
-    variablesCollected = [FILE_NAME_TO_VARIABLE_NAME_DICT[fileName2variableName(fname)] for fname in MAPS_DIR_PATH.iterdir()]
-    for varName in variablesCollected:
-        logging.info(f"""  Loading map for "{varName}".""")
-        varPath = MAPS_DIR_PATH.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[varName]} map.csv")
-        map_ = pd.read_csv(varPath)
-        mapDi = map2di(map_)
-        mapsDi[varName] = mapDi
-        mapsColumnNames[varName] = map_.columns[-1]
-    # Add aliases to `mapsColumnNames`
-    for varName in VARIABLE_ALIASES.keys():
-        varAlias = VARIABLE_ALIASES[varName]
-        map_ = makeMap(IDset=set(),
-                       IDName=varName,
-                       startFrom=1,
-                       irbNumber=IRB_NUMBER,
-                       suffix=VARIABLE_SUFFIXES[varAlias]["deIdIDSuffix"],
-                       columnSuffix=varName,
-                       deIdentificationMapStyle="lemur",
-                       logger=logging.getLogger())
-        mapsColumnNames[varName] = map_.columns[-1]
-    # Add aliases to `DATA_TYPES_DICT`
-    DATA_TYPES_DICT.update(ALIAS_DATA_TYPES)
-
-    # De-identify columns
-    logging.info("""De-identifying files.""")
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logging.info("""    File has met all conditions for processing.""")
-                logging.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
-                logging.info(f"""  ..  This file has {numChunks} chunks.""")
-                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    # Work on chunk
-                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        logging.info(f"""  ..    Working on column "{columnName}".""")
-                        if columnName in COLUMNS_TO_DE_IDENTIFY:  # Keep this reference to `COLUMNS_TO_DE_IDENTIFY` as a way to make sure that all variables were collected during `getIDValues` and the `makeMap` scripts.
-                            variableDataType = DATA_TYPES_DICT[columnName]
-                            logging.info(f"""  ..  ..  Column must be de-identified. De-identifying values. Values are being treated as the following data type: "{variableDataType}".""")
-                            if columnName in VARIABLE_ALIASES.keys():
-                                mapsDiLookUpName = VARIABLE_ALIASES[columnName]
-                            else:
-                                mapsDiLookUpName = columnName
-                            # Look up values in de-identification maps according to data type. NOTE We are relying on pandas assigning the correct data type to the look-up values in the de-identification map.
-                            if variableDataType.lower() == "numeric":
-                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDNum: mapsDi[mapsDiLookUpName][IDNum] if not pd.isna(IDNum) else IDNum)
-                            elif columnName in ["NRAS"]:
-                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: f"{IRB_NUMBER}_DE-IDENTIFICATION FAILURE" if not pd.isna(IDvalue) else IDvalue)
-                                logging.info("""Using work-around for this variable. This variable is assigned the data type of "Numeric_Or_String", but its values were not reliably mapped to de-identified values.""")  # NOTE Hack. This is the same problem as the other variables below. Part of the problem is how pandas reads files.
-                            elif columnName in ["F/u Physicians", "Prim  surgeon Code"]:  # NOTE Hack. These variables are categorized as `numeric_or_string`, but they contain numbers with leading zeros that get converted to integers in the current process. Either we convert these variables to `string` or we change the process.
-                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: mapsDi[mapsDiLookUpName][str(IDvalue)] if not pd.isna(IDvalue) else IDvalue)
-                                logging.info("""Using work-around for this variable. This variable is assigned the data type of "Numeric_Or_String", but is being treated as a "String" variable. If continued use of the "String" data type is successful, then the current assignment of "Numeric_Or_String" should be deprecated.""")
-                            elif variableDataType.lower() == "string":
-                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: mapsDi[mapsDiLookUpName][str(IDvalue)] if not pd.isna(IDvalue) else IDvalue)
-                            elif variableDataType.lower() == "numeric_or_string":
-                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: mapsDi[mapsDiLookUpName][str(numericOrString2integerOrString(IDvalue))] if not pd.isna(IDvalue) else IDvalue)
-                            else:
-                                msg = "The table column is expected to have a data type associated with it."
-                                logging.error(msg)
-                                raise ValueError(msg)
-                            dfChunk = dfChunk.rename(columns={columnName: mapsColumnNames[columnName]})
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logging.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logging.info("""    This file does not need to be processed.""")
-
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+De-identify files
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+# TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
+"""
+
+import logging
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (fileName2variableName,
+                                    getTimestamp,
+                                    makeDirPath,
+                                    makeMap,
+                                    map2di,
+                                    numericOrString2integerOrString,
+                                    readDataFile,
+                                    successiveParents)
+from drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
+                                          VARIABLE_NAME_TO_FILE_NAME_DICT)
+# Local packages: Script parameters: General
+from common import (IRB_NUMBER,
+                    ALIAS_DATA_TYPES,
+                    COLUMNS_TO_DE_IDENTIFY,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
+                    DATA_TYPES_DICT,
+                    VARIABLE_ALIASES,
+                    VARIABLE_SUFFIXES)
+# Local packages: Script parameters: Paths
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
+                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+# Local packages: Script parameters: File criteria
+from common import (BO_PORTION_FILE_CRITERIA,
+                    I2B2_PORTION_FILE_CRITERIA,
+                    NOTES_PORTION_FILE_CRITERIA,
+                    OMOP_PORTION_FILE_CRITERIA)
+
+# Arguments
+CONCATENATED_MAPS_DIR_PATH = Path(r"..\Concatenated Results\data\output\concatenateMaps\...")  # TODO
+
+MAPS_DIR_PATH = CONCATENATED_MAPS_DIR_PATH
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: Portion Paths and conditions
+if USE_MODIFIED_OMOP_DATA_SET:
+    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
+else:
+    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
+
+MAC_PATHS = [BO_PORTION_DIR_MAC,
+             I2B2_PORTION_DIR_MAC,
+             NOTES_PORTION_DIR_MAC,
+             OMOPPortionDirMac]
+WIN_PATHS = [BO_PORTION_DIR_WIN,
+             I2B2_PORTION_DIR_WIN,
+             NOTES_PORTION_DIR_WIN,
+             OMOPPortionDirWin]
+
+LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA,
+                              I2B2_PORTION_FILE_CRITERIA,
+                              NOTES_PORTION_FILE_CRITERIA,
+                              OMOP_PORTION_FILE_CRITERIA]
+
+# Arguments; General
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # Assert all portions have file criteria accounted for
+    if len(listOfPortionDirs) == len(LIST_OF_PORTION_CONDITIONS):
+        pass
+    else:
+        raise Exception("The number of portions does not equal the number of portion conditions.")
+
+    # Load de-identification maps for each variable that needs to be de-identified
+    logging.info("""Loading de-identification maps for each variable that needs to be de-identified.""")
+    mapsDi = {}
+    mapsColumnNames = {}
+    variablesCollected = [FILE_NAME_TO_VARIABLE_NAME_DICT[fileName2variableName(fname)] for fname in MAPS_DIR_PATH.iterdir()]
+    for varName in variablesCollected:
+        logging.info(f"""  Loading map for "{varName}".""")
+        varPath = MAPS_DIR_PATH.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[varName]} map.csv")
+        map_ = pd.read_csv(varPath)
+        mapDi = map2di(map_)
+        mapsDi[varName] = mapDi
+        mapsColumnNames[varName] = map_.columns[-1]
+    # Add aliases to `mapsColumnNames`
+    for varName in VARIABLE_ALIASES.keys():
+        varAlias = VARIABLE_ALIASES[varName]
+        map_ = makeMap(IDset=set(),
+                       IDName=varName,
+                       startFrom=1,
+                       irbNumber=IRB_NUMBER,
+                       suffix=VARIABLE_SUFFIXES[varAlias]["deIdIDSuffix"],
+                       columnSuffix=varName,
+                       deIdentificationMapStyle="lemur",
+                       logger=logging.getLogger())
+        mapsColumnNames[varName] = map_.columns[-1]
+    # Add aliases to `DATA_TYPES_DICT`
+    DATA_TYPES_DICT.update(ALIAS_DATA_TYPES)
+
+    # De-identify columns
+    logging.info("""De-identifying files.""")
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+        for file in directory.iterdir():
+            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logging.info("""    File has met all conditions for processing.""")
+                logging.info("""  ..  Reading file to count the number of chunks.""")
+                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                logging.info(f"""  ..  This file has {numChunks} chunks.""")
+                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    # Work on chunk
+                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        # Work on column
+                        logging.info(f"""  ..    Working on column "{columnName}".""")
+                        if columnName in COLUMNS_TO_DE_IDENTIFY:  # Keep this reference to `COLUMNS_TO_DE_IDENTIFY` as a way to make sure that all variables were collected during `getIDValues` and the `makeMap` scripts.
+                            variableDataType = DATA_TYPES_DICT[columnName]
+                            logging.info(f"""  ..  ..  Column must be de-identified. De-identifying values. Values are being treated as the following data type: "{variableDataType}".""")
+                            if columnName in VARIABLE_ALIASES.keys():
+                                mapsDiLookUpName = VARIABLE_ALIASES[columnName]
+                            else:
+                                mapsDiLookUpName = columnName
+                            # Look up values in de-identification maps according to data type. NOTE We are relying on pandas assigning the correct data type to the look-up values in the de-identification map.
+                            if variableDataType.lower() == "numeric":
+                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDNum: mapsDi[mapsDiLookUpName][IDNum] if not pd.isna(IDNum) else IDNum)
+                            elif columnName in ["NRAS"]:
+                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: f"{IRB_NUMBER}_DE-IDENTIFICATION FAILURE" if not pd.isna(IDvalue) else IDvalue)
+                                logging.info("""Using work-around for this variable. This variable is assigned the data type of "Numeric_Or_String", but its values were not reliably mapped to de-identified values.""")  # NOTE Hack. This is the same problem as the other variables below. Part of the problem is how pandas reads files.
+                            elif columnName in ["F/u Physicians", "Prim  surgeon Code"]:  # NOTE Hack. These variables are categorized as `numeric_or_string`, but they contain numbers with leading zeros that get converted to integers in the current process. Either we convert these variables to `string` or we change the process.
+                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: mapsDi[mapsDiLookUpName][str(IDvalue)] if not pd.isna(IDvalue) else IDvalue)
+                                logging.info("""Using work-around for this variable. This variable is assigned the data type of "Numeric_Or_String", but is being treated as a "String" variable. If continued use of the "String" data type is successful, then the current assignment of "Numeric_Or_String" should be deprecated.""")
+                            elif variableDataType.lower() == "string":
+                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: mapsDi[mapsDiLookUpName][str(IDvalue)] if not pd.isna(IDvalue) else IDvalue)
+                            elif variableDataType.lower() == "numeric_or_string":
+                                dfChunk[columnName] = dfChunk[columnName].apply(lambda IDvalue: mapsDi[mapsDiLookUpName][str(numericOrString2integerOrString(IDvalue))] if not pd.isna(IDvalue) else IDvalue)
+                            else:
+                                msg = "The table column is expected to have a data type associated with it."
+                                logging.error(msg)
+                                raise ValueError(msg)
+                            dfChunk = dfChunk.rename(columns={columnName: mapsColumnNames[columnName]})
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logging.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logging.info("""    This file does not need to be processed.""")
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-"""
-De-identifies those above a certain age threshold by replacing the age with a label and setting the birthdate to "1/1/1800". The label is "> X", where "X" is the age threshold.
-"""
-
-import logging
-import os
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-# Local packages: Script parameters: General
-from drapi.constants.phiVariables import (DICT_OF_PHI_VARIABLES_AGE,
-                                          DICT_OF_PHI_VARIABLES_BIRTHDATES)
-# Local packages: Script parameters: Paths
-# Local packages: Script parameters: File criteria
-from common import BO_PORTION_FILE_CRITERIA
-
-# Arguments
-AGE_MAP = Path(r"..\Concatenated Results\data\output\makeAgeMap\2024-01-03 13-20-23\Age Map - De-identified Patient Key.CSV")
-USE_DE_IDENTIFIED_DATES = True
-
-DE_IDENTIFIED_AGE_VALUE = "> 90"
-DE_IDENTIFIED_BIRTHDATE_VALUE = "1/1/1800"
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Variables: Script parameters: Date variables
-# NOTE Set `USE_DE_IDENTIFIED_DATES` to `True` if the dates have been de-identified. If the IDs have been de-identified, it is not necessary to set this to `True`.
-if USE_DE_IDENTIFIED_DATES:
-    DE_IDENTIFICATION_PREFIX = "De-identified "
-    dictOfPHIVariablesBirthdates = {portion: [] for portion in DICT_OF_PHI_VARIABLES_BIRTHDATES.keys()}
-    for portion, li in DICT_OF_PHI_VARIABLES_BIRTHDATES.items():
-        for columnName in li:
-            dictOfPHIVariablesBirthdates[portion].append(f"{DE_IDENTIFICATION_PREFIX} {columnName}")
-else:
-    dictOfPHIVariablesBirthdates = DICT_OF_PHI_VARIABLES_BIRTHDATES
-
-# Variables: Script parameters: Age variables
-dictOfPHIVariablesAge = DICT_OF_PHI_VARIABLES_AGE
-
-# Arguments: Portion Paths and conditions
-MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\...")]  # TODO
-WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\...")]  # TODO
-
-listOfAgeColumns = [el for value in dictOfPHIVariablesAge.values() for el in value]
-listOfBirthdateColumns = [el for value in dictOfPHIVariablesBirthdates.values() for el in value]
-listOfColumnsToDeIdentify = listOfAgeColumns + listOfBirthdateColumns
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
-
-# Arguments; General
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `AGE_MAP`: "{AGE_MAP}"
-    `USE_MODIFIED_OMOP_DATA_SET`: "{USE_MODIFIED_OMOP_DATA_SET}"
-    `MAC_PATHS`: "{MAC_PATHS}"
-    `WIN_PATHS`: "{WIN_PATHS}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Load age de-identification map
-    logger.info("""Loading age de-identification map.""")
-    map_ = pd.read_csv(AGE_MAP, comment="#")
-    logger.info("""Loading age de-identification map - done.""")
-    PATIENT_LOOK_UP_ID_NAME = map_.columns[0]
-    mapMask = map_["Over Age Threshold"].apply(lambda integer: True if integer else (False if not integer else None))
-    patientsToDeIdentify = map_[PATIENT_LOOK_UP_ID_NAME][mapMask]
-
-    # De-identify by age
-    logger.info("""De-identifying files.""")
-    columnDeIdentificationRenamePrefix = f"{DE_IDENTIFICATION_PREFIX}"
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logger.info("""    File has met all conditions for processing.""")
-                logger.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE, dtype=str)])
-                logger.info(f"""  ..  This file has {numChunks} chunks.""")
-                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE, low_memory=False)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    # Work on chunk
-                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        logger.info(f"""  ..    Working on column "{columnName}".""")
-                        columnShouldBeProcessed = False
-                        if columnName in listOfColumnsToDeIdentify:
-                            columnShouldBeProcessed = True
-                        else:
-                            continue
-                        if columnShouldBeProcessed:
-                            logger.info("""  ..  ..  Column must be de-identified.""")
-                            mask = dfChunk[PATIENT_LOOK_UP_ID_NAME].isin(patientsToDeIdentify)
-                            if columnName in listOfAgeColumns:
-                                dfChunk.loc[mask, columnName] = DE_IDENTIFIED_AGE_VALUE
-                            elif columnName in listOfBirthdateColumns:
-                                dfChunk.loc[mask, columnName] = DE_IDENTIFIED_BIRTHDATE_VALUE
-                            if USE_DE_IDENTIFIED_DATES:
-                                if columnName in listOfAgeColumns:
-                                    columnRenamePrefix = columnDeIdentificationRenamePrefix
-                                else:
-                                    columnRenamePrefix = ""
-                            else:
-                                columnRenamePrefix = columnDeIdentificationRenamePrefix
-                            dfChunk = dfChunk.rename(columns={columnName: f"{columnRenamePrefix}{columnName}"})
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logger.info("""    This file does not need to be processed.""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+De-identifies those above a certain age threshold by replacing the age with a label and setting the birthdate to "1/1/1800". The label is "> X", where "X" is the age threshold.
+"""
+
+import logging
+import os
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+# Local packages: Script parameters: General
+from drapi.constants.phiVariables import (DICT_OF_PHI_VARIABLES_AGE,
+                                          DICT_OF_PHI_VARIABLES_BIRTHDATES)
+# Local packages: Script parameters: Paths
+# Local packages: Script parameters: File criteria
+from common import BO_PORTION_FILE_CRITERIA
+
+# Arguments
+AGE_MAP = Path(r"..\Concatenated Results\data\output\makeAgeMap\2024-01-03 13-20-23\Age Map - De-identified Patient Key.CSV")
+USE_DE_IDENTIFIED_DATES = True
+
+DE_IDENTIFIED_AGE_VALUE = "> 90"
+DE_IDENTIFIED_BIRTHDATE_VALUE = "1/1/1800"
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Variables: Script parameters: Date variables
+# NOTE Set `USE_DE_IDENTIFIED_DATES` to `True` if the dates have been de-identified. If the IDs have been de-identified, it is not necessary to set this to `True`.
+if USE_DE_IDENTIFIED_DATES:
+    DE_IDENTIFICATION_PREFIX = "De-identified "
+    dictOfPHIVariablesBirthdates = {portion: [] for portion in DICT_OF_PHI_VARIABLES_BIRTHDATES.keys()}
+    for portion, li in DICT_OF_PHI_VARIABLES_BIRTHDATES.items():
+        for columnName in li:
+            dictOfPHIVariablesBirthdates[portion].append(f"{DE_IDENTIFICATION_PREFIX} {columnName}")
+else:
+    dictOfPHIVariablesBirthdates = DICT_OF_PHI_VARIABLES_BIRTHDATES
+
+# Variables: Script parameters: Age variables
+dictOfPHIVariablesAge = DICT_OF_PHI_VARIABLES_AGE
+
+# Arguments: Portion Paths and conditions
+MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\...")]  # TODO
+WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\...")]  # TODO
+
+listOfAgeColumns = [el for value in dictOfPHIVariablesAge.values() for el in value]
+listOfBirthdateColumns = [el for value in dictOfPHIVariablesBirthdates.values() for el in value]
+listOfColumnsToDeIdentify = listOfAgeColumns + listOfBirthdateColumns
+LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
+
+# Arguments; General
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `AGE_MAP`: "{AGE_MAP}"
+    `USE_MODIFIED_OMOP_DATA_SET`: "{USE_MODIFIED_OMOP_DATA_SET}"
+    `MAC_PATHS`: "{MAC_PATHS}"
+    `WIN_PATHS`: "{WIN_PATHS}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Load age de-identification map
+    logger.info("""Loading age de-identification map.""")
+    map_ = pd.read_csv(AGE_MAP, comment="#")
+    logger.info("""Loading age de-identification map - done.""")
+    PATIENT_LOOK_UP_ID_NAME = map_.columns[0]
+    mapMask = map_["Over Age Threshold"].apply(lambda integer: True if integer else (False if not integer else None))
+    patientsToDeIdentify = map_[PATIENT_LOOK_UP_ID_NAME][mapMask]
+
+    # De-identify by age
+    logger.info("""De-identifying files.""")
+    columnDeIdentificationRenamePrefix = f"{DE_IDENTIFICATION_PREFIX}"
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+        for file in directory.iterdir():
+            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logger.info("""    File has met all conditions for processing.""")
+                logger.info("""  ..  Reading file to count the number of chunks.""")
+                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE, dtype=str)])
+                logger.info(f"""  ..  This file has {numChunks} chunks.""")
+                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE, low_memory=False)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    # Work on chunk
+                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        # Work on column
+                        logger.info(f"""  ..    Working on column "{columnName}".""")
+                        columnShouldBeProcessed = False
+                        if columnName in listOfColumnsToDeIdentify:
+                            columnShouldBeProcessed = True
+                        else:
+                            continue
+                        if columnShouldBeProcessed:
+                            logger.info("""  ..  ..  Column must be de-identified.""")
+                            mask = dfChunk[PATIENT_LOOK_UP_ID_NAME].isin(patientsToDeIdentify)
+                            if columnName in listOfAgeColumns:
+                                dfChunk.loc[mask, columnName] = DE_IDENTIFIED_AGE_VALUE
+                            elif columnName in listOfBirthdateColumns:
+                                dfChunk.loc[mask, columnName] = DE_IDENTIFIED_BIRTHDATE_VALUE
+                            if USE_DE_IDENTIFIED_DATES:
+                                if columnName in listOfAgeColumns:
+                                    columnRenamePrefix = columnDeIdentificationRenamePrefix
+                                else:
+                                    columnRenamePrefix = ""
+                            else:
+                                columnRenamePrefix = columnDeIdentificationRenamePrefix
+                            dfChunk = dfChunk.rename(columns={columnName: f"{columnRenamePrefix}{columnName}"})
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logger.info("""    This file does not need to be processed.""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,317 +1,317 @@
-"""
-Shifts the dates in a data set according to the date shift map for a patient.
-"""
-
-import logging
-import os
-import sys
-import datetime
-from pathlib import Path
-import re
-from typing import Union
-# Third-party packages
-import pandas as pd
-from pandas.errors import OutOfBoundsDatetime
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    makeMap,
-                                    map2di,
-                                    successiveParents)
-# Local packages: Script parameters: General
-from drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
-                                          LIST_OF_PHI_DATES_NOTES,
-                                          LIST_OF_PHI_DATES_OMOP)
-# Local packages: Script parameters: General
-from common import IRB_NUMBER
-# Local packages: Script parameters: Paths
-# Local packages: Script parameters: File criteria
-from common import BO_PORTION_FILE_CRITERIA
-
-# Arguments
-"""
-Argument descriptions
-`PATIENT_DATE_SHIFT_MAP`:                   A Path object. This is the file path of the date-shift map. It expects a four-columned CSV file.
-`LOOK_UP_NAME_MAP_INDEX`:                   An integer. Assuming a typical IDR de-identification map format, `0`` is for the identified, original ID name, and `2` is for the de-identified variable name.
-`LOOK_UP_NAME_DE_IDENTIFICATION_FORMAT`:    A string. This is required if `LOOK_UP_NAME_MAP_INDEX` is `2`. Options are "lemur" or "classic"
-`LIST_OF_PHI_DATES`:                        A list of strings. This list the column headers (i.e., variable names) that need to have their dates de-identified (i.e., date-shifted).
-
-`USE_MODIFIED_OMOP_DATA_SET`:               A boolean. This indicates which version of the OMOP data set to use, the original or the one that has had its columns converted. These versions are defined by their directory locations in `OMOP_PORTION_DIR_*` and `MODIFIED_OMOP_PORTION_DIR_*`, where `*` is `MAC` or `WIN`.
-`MAC_PATHS`:                                A list of Path objects. The Path objects point to the directories that should be processed.
-`WIN_PATHS`:                                A list of Path objects. The Path objects point to the directories that should be processed.
-`LIST_OF_PORTION_CONDITIONS`:               A list of functions. All these fucntions are evaluated on each of the files in each of the directories defined by `*_PATHS`.
-"""
-PATIENT_DATE_SHIFT_MAP = Path(r"..\Concatenated Results\data\output\makeDateShiftMap\...\Date Shift Map.CSV")
-LOOK_UP_NAME_MAP_INDEX = 2
-LOOK_UP_NAME_DE_IDENTIFICATION_FORMAT = "lemur"
-LIST_OF_PHI_DATES = LIST_OF_PHI_DATES_BO + LIST_OF_PHI_DATES_NOTES + LIST_OF_PHI_DATES_OMOP
-
-# Arguments: Portion Paths and conditions
-MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\2023-12-13 13-58-38")]
-WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\2023-12-13 13-58-38")]
-
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
-
-# Arguments; General
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `PATIENT_DATE_SHIFT_MAP`: "{PATIENT_DATE_SHIFT_MAP}"
-    `MAC_PATHS`: "{MAC_PATHS}"
-    `WIN_PATHS`: "{WIN_PATHS}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Load de-identification maps for dates, i.e., the date shift maps.
-    logger.info("""Loading de-identification maps for dates.""")
-    map_ = pd.read_csv(PATIENT_DATE_SHIFT_MAP)
-    dateShiftMapDi = map2di(map_, fromColumnIndex=LOOK_UP_NAME_MAP_INDEX, toColumnIndex=3)
-    lookUpNameOriginal = map_.columns[0]
-    lookUpNameSelected = map_.columns[LOOK_UP_NAME_MAP_INDEX]
-
-    # Create alias reverse look-up dictionary
-    from common import VARIABLE_ALIASES
-    reverseAliasLookup = {}
-    for alias, mainName in VARIABLE_ALIASES.items():
-        if mainName in reverseAliasLookup.keys():
-            reverseAliasLookup[mainName].append(alias)
-        else:
-            reverseAliasLookup[mainName] = [alias]
-
-    # Synthesize alias names. If we are looking for the original variable name, these are unchaged, but if we are looking for de-identified variable names, we must syntheisze the names.
-    if LOOK_UP_NAME_MAP_INDEX == 0:
-        pass
-    elif LOOK_UP_NAME_MAP_INDEX == 2:
-        listOfLookUpNameAliases = []
-        for alias in reverseAliasLookup[lookUpNameOriginal]:
-            df = makeMap(IDset={},
-                         IDName="PatientKey",
-                         startFrom=1,
-                         irbNumber=IRB_NUMBER,
-                         suffix="",
-                         columnSuffix="",
-                         logger=logger)
-            lookUpNameAlias = df.columns[-1]
-            listOfLookUpNameAliases.append(lookUpNameAlias)
-    else:
-        msg = """Invalid value for `LOOK_UP_NAME_MAP_INDEX`. See script arguments."""
-        logger.error(msg)
-        raise Exception(msg)
-
-    def string2datetime(string: str) -> Union[datetime.datetime, pd.Timestamp]:
-        """
-        Attempts to convert a string to a pandas datetime object. If it's out of range it converts it to a Python datetime object.
-
-        The Python datetime conversion works as follows:
-        Using regex it detects if the string is one of the following formats:
-            - Date and time with seconds-precision
-            - Date and time with minutes-precision
-            - Date
-        NOTE: Additional formats can be implemented by adding the corresponding regular expression and `strptime` call combination.
-        """
-        try:
-            newValue = pd.to_datetime(string)
-        except OutOfBoundsDatetime as err:
-            _ = err
-            pattern1 = r"(?P<newValue>\d+[\/-]\d+[\/-]\d+\W+\d+:\d+:\d+)"   # Second-precision
-            pattern2 = r"(?P<newValue>\d+[\/-]\d+[\/-]\d+\W+\d+:\d+)"  # Minutes-precision
-            pattern3 = r"(?P<newValue>\d+[\/-]\d+[\/-]\d)"  # Days-precision
-            reObj1 = re.match(pattern1, string)
-            reObj2 = re.match(pattern2, string)
-            reObj3 = re.match(pattern3, string)
-            if reObj1:
-                newValue = datetime.datetime.strptime(string, "%m/%d/%Y %H:%M:%S")
-            elif reObj2:
-                newValue = datetime.datetime.strptime(string, "%m/%d/%Y %H:%M")
-            elif reObj3:
-                newValue = datetime.datetime.strptime(string, "%m/%d/%Y")
-        return newValue
-
-    def datetimeOffset(timeObj: Union[datetime.datetime, pd.Timestamp], offset: int):
-        """
-        `offset`, an int, is the number of days.
-        """
-        if (pd.Timestamp.min < timeObj < pd.Timestamp.max):
-            newValue = timeObj + pd.DateOffset(offset)
-        else:
-            newValue = timeObj + datetime.timedelta(days=offset)
-        return newValue
-
-    logger.info("""De-identifying files.""")
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logger.info("""    File has met all conditions for processing.""")
-                logger.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE)])
-                logger.info(f"""  ..  This file has {numChunks} chunks.""")
-                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    # Work on chunk
-                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        logger.info(f"""  ..    Working on column "{columnName}".""")
-                        if columnName in LIST_OF_PHI_DATES:
-                            logger.info("""  ..  ..  Column must be de-identified. Date-shifting values.""")
-                            if lookUpNameSelected in dfChunk.columns:
-                                lookUpName = lookUpNameSelected
-                            elif any([alias in dfChunk.columns for alias in listOfLookUpNameAliases]):
-                                for alias in listOfLookUpNameAliases:
-                                    if alias in dfChunk.columns:
-                                        break
-                                lookUpName = alias
-                            else:
-                                msg = f"""The variable used to look up the date shift offset was not found. We searched for "{lookUpNameSelected}" and any of its aliases: {'", "'.join(listOfLookUpNameAliases)}"""
-                                logger.error(msg)
-                                raise Exception(msg)
-                            dateShiftValues = dfChunk[lookUpName].apply(lambda lookUpID: dateShiftMapDi[lookUpID])
-                            column = dfChunk[columnName].apply(string2datetime)
-                            df = pd.concat([column, dateShiftValues], axis=1)
-                            series = df.apply(lambda el: (el[columnName], el[lookUpName]), axis=1)
-                            dfChunk[columnName] = series.apply(lambda tu: datetimeOffset(timeObj=tu[0], offset=tu[1]))
-                            dfChunk = dfChunk.rename(columns={columnName: f"De-identified {columnName}"})
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logger.info("""    This file does not need to be processed.""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+Shifts the dates in a data set according to the date shift map for a patient.
+"""
+
+import logging
+import os
+import sys
+import datetime
+from pathlib import Path
+import re
+from typing import Union
+# Third-party packages
+import pandas as pd
+from pandas.errors import OutOfBoundsDatetime
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    makeMap,
+                                    map2di,
+                                    successiveParents)
+# Local packages: Script parameters: General
+from drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
+                                          LIST_OF_PHI_DATES_NOTES,
+                                          LIST_OF_PHI_DATES_OMOP)
+# Local packages: Script parameters: General
+from common import IRB_NUMBER
+# Local packages: Script parameters: Paths
+# Local packages: Script parameters: File criteria
+from common import BO_PORTION_FILE_CRITERIA
+
+# Arguments
+"""
+Argument descriptions
+`PATIENT_DATE_SHIFT_MAP`:                   A Path object. This is the file path of the date-shift map. It expects a four-columned CSV file.
+`LOOK_UP_NAME_MAP_INDEX`:                   An integer. Assuming a typical IDR de-identification map format, `0`` is for the identified, original ID name, and `2` is for the de-identified variable name.
+`LOOK_UP_NAME_DE_IDENTIFICATION_FORMAT`:    A string. This is required if `LOOK_UP_NAME_MAP_INDEX` is `2`. Options are "lemur" or "classic"
+`LIST_OF_PHI_DATES`:                        A list of strings. This list the column headers (i.e., variable names) that need to have their dates de-identified (i.e., date-shifted).
+
+`USE_MODIFIED_OMOP_DATA_SET`:               A boolean. This indicates which version of the OMOP data set to use, the original or the one that has had its columns converted. These versions are defined by their directory locations in `OMOP_PORTION_DIR_*` and `MODIFIED_OMOP_PORTION_DIR_*`, where `*` is `MAC` or `WIN`.
+`MAC_PATHS`:                                A list of Path objects. The Path objects point to the directories that should be processed.
+`WIN_PATHS`:                                A list of Path objects. The Path objects point to the directories that should be processed.
+`LIST_OF_PORTION_CONDITIONS`:               A list of functions. All these fucntions are evaluated on each of the files in each of the directories defined by `*_PATHS`.
+"""
+PATIENT_DATE_SHIFT_MAP = Path(r"..\Concatenated Results\data\output\makeDateShiftMap\...\Date Shift Map.CSV")
+LOOK_UP_NAME_MAP_INDEX = 2
+LOOK_UP_NAME_DE_IDENTIFICATION_FORMAT = "lemur"
+LIST_OF_PHI_DATES = LIST_OF_PHI_DATES_BO + LIST_OF_PHI_DATES_NOTES + LIST_OF_PHI_DATES_OMOP
+
+# Arguments: Portion Paths and conditions
+MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\2023-12-13 13-58-38")]
+WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentify\2023-12-13 13-58-38")]
+
+LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
+
+# Arguments; General
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `PATIENT_DATE_SHIFT_MAP`: "{PATIENT_DATE_SHIFT_MAP}"
+    `MAC_PATHS`: "{MAC_PATHS}"
+    `WIN_PATHS`: "{WIN_PATHS}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Load de-identification maps for dates, i.e., the date shift maps.
+    logger.info("""Loading de-identification maps for dates.""")
+    map_ = pd.read_csv(PATIENT_DATE_SHIFT_MAP)
+    dateShiftMapDi = map2di(map_, fromColumnIndex=LOOK_UP_NAME_MAP_INDEX, toColumnIndex=3)
+    lookUpNameOriginal = map_.columns[0]
+    lookUpNameSelected = map_.columns[LOOK_UP_NAME_MAP_INDEX]
+
+    # Create alias reverse look-up dictionary
+    from common import VARIABLE_ALIASES
+    reverseAliasLookup = {}
+    for alias, mainName in VARIABLE_ALIASES.items():
+        if mainName in reverseAliasLookup.keys():
+            reverseAliasLookup[mainName].append(alias)
+        else:
+            reverseAliasLookup[mainName] = [alias]
+
+    # Synthesize alias names. If we are looking for the original variable name, these are unchaged, but if we are looking for de-identified variable names, we must syntheisze the names.
+    if LOOK_UP_NAME_MAP_INDEX == 0:
+        pass
+    elif LOOK_UP_NAME_MAP_INDEX == 2:
+        listOfLookUpNameAliases = []
+        for alias in reverseAliasLookup[lookUpNameOriginal]:
+            df = makeMap(IDset={},
+                         IDName="PatientKey",
+                         startFrom=1,
+                         irbNumber=IRB_NUMBER,
+                         suffix="",
+                         columnSuffix="",
+                         logger=logger)
+            lookUpNameAlias = df.columns[-1]
+            listOfLookUpNameAliases.append(lookUpNameAlias)
+    else:
+        msg = """Invalid value for `LOOK_UP_NAME_MAP_INDEX`. See script arguments."""
+        logger.error(msg)
+        raise Exception(msg)
+
+    def string2datetime(string: str) -> Union[datetime.datetime, pd.Timestamp]:
+        """
+        Attempts to convert a string to a pandas datetime object. If it's out of range it converts it to a Python datetime object.
+
+        The Python datetime conversion works as follows:
+        Using regex it detects if the string is one of the following formats:
+            - Date and time with seconds-precision
+            - Date and time with minutes-precision
+            - Date
+        NOTE: Additional formats can be implemented by adding the corresponding regular expression and `strptime` call combination.
+        """
+        try:
+            newValue = pd.to_datetime(string)
+        except OutOfBoundsDatetime as err:
+            _ = err
+            pattern1 = r"(?P<newValue>\d+[\/-]\d+[\/-]\d+\W+\d+:\d+:\d+)"   # Second-precision
+            pattern2 = r"(?P<newValue>\d+[\/-]\d+[\/-]\d+\W+\d+:\d+)"  # Minutes-precision
+            pattern3 = r"(?P<newValue>\d+[\/-]\d+[\/-]\d)"  # Days-precision
+            reObj1 = re.match(pattern1, string)
+            reObj2 = re.match(pattern2, string)
+            reObj3 = re.match(pattern3, string)
+            if reObj1:
+                newValue = datetime.datetime.strptime(string, "%m/%d/%Y %H:%M:%S")
+            elif reObj2:
+                newValue = datetime.datetime.strptime(string, "%m/%d/%Y %H:%M")
+            elif reObj3:
+                newValue = datetime.datetime.strptime(string, "%m/%d/%Y")
+        return newValue
+
+    def datetimeOffset(timeObj: Union[datetime.datetime, pd.Timestamp], offset: int):
+        """
+        `offset`, an int, is the number of days.
+        """
+        if (pd.Timestamp.min < timeObj < pd.Timestamp.max):
+            newValue = timeObj + pd.DateOffset(offset)
+        else:
+            newValue = timeObj + datetime.timedelta(days=offset)
+        return newValue
+
+    logger.info("""De-identifying files.""")
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+        for file in directory.iterdir():
+            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logger.info("""    File has met all conditions for processing.""")
+                logger.info("""  ..  Reading file to count the number of chunks.""")
+                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE)])
+                logger.info(f"""  ..  This file has {numChunks} chunks.""")
+                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    # Work on chunk
+                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        # Work on column
+                        logger.info(f"""  ..    Working on column "{columnName}".""")
+                        if columnName in LIST_OF_PHI_DATES:
+                            logger.info("""  ..  ..  Column must be de-identified. Date-shifting values.""")
+                            if lookUpNameSelected in dfChunk.columns:
+                                lookUpName = lookUpNameSelected
+                            elif any([alias in dfChunk.columns for alias in listOfLookUpNameAliases]):
+                                for alias in listOfLookUpNameAliases:
+                                    if alias in dfChunk.columns:
+                                        break
+                                lookUpName = alias
+                            else:
+                                msg = f"""The variable used to look up the date shift offset was not found. We searched for "{lookUpNameSelected}" and any of its aliases: {'", "'.join(listOfLookUpNameAliases)}"""
+                                logger.error(msg)
+                                raise Exception(msg)
+                            dateShiftValues = dfChunk[lookUpName].apply(lambda lookUpID: dateShiftMapDi[lookUpID])
+                            column = dfChunk[columnName].apply(string2datetime)
+                            df = pd.concat([column, dateShiftValues], axis=1)
+                            series = df.apply(lambda el: (el[columnName], el[lookUpName]), axis=1)
+                            dfChunk[columnName] = series.apply(lambda tu: datetimeOffset(timeObj=tu[0], offset=tu[1]))
+                            dfChunk = dfChunk.rename(columns={columnName: f"De-identified {columnName}"})
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logger.info("""    This file does not need to be processed.""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-"""
-Deletes rows based on column values.
-"""
-
-import logging
-import os
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-# Local packages: Script parameters: General
-from drapi.constants.phiValues import PHI_VALUES_DICT_ALL
-# Local packages: Script parameters: General
-# Local packages: Script parameters: Paths
-# Local packages: Script parameters: File criteria
-from common import BO_PORTION_FILE_CRITERIA
-
-# Arguments
-COLUMN_VALUES_TO_DROP = PHI_VALUES_DICT_ALL
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Arguments: Portion Paths and conditions
-MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
-WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
-
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
-
-# Arguments; General
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `COLUMN_VALUES_TO_DROP`: "{COLUMN_VALUES_TO_DROP}"
-    `USE_MODIFIED_OMOP_DATA_SET`: "{USE_MODIFIED_OMOP_DATA_SET}"
-    `MAC_PATHS`: "{MAC_PATHS}"
-    `WIN_PATHS`: "{WIN_PATHS}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    logger.info("""De-identifying files.""")
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logger.info("""    File has met all conditions for processing.""")
-                logger.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE)])
-                logger.info(f"""  ..  This file has {numChunks} chunks.""")
-                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    # Work on chunk
-                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        logger.info(f"""  ..    Working on column "{columnName}".""")
-                        if columnName in COLUMN_VALUES_TO_DROP.keys():
-                            mask = ~dfChunk[columnName].isin(COLUMN_VALUES_TO_DROP[columnName])
-                            if mask.sum() > 0:
-                                logger.info("""  ..  ..  Column has values that need to be dropped. Dropping values.""")
-                            dfChunk = dfChunk[mask]
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logger.info("""    This file does not need to be processed.""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+Deletes rows based on column values.
+"""
+
+import logging
+import os
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+# Local packages: Script parameters: General
+from drapi.constants.phiValues import PHI_VALUES_DICT_ALL
+# Local packages: Script parameters: General
+# Local packages: Script parameters: Paths
+# Local packages: Script parameters: File criteria
+from common import BO_PORTION_FILE_CRITERIA
+
+# Arguments
+COLUMN_VALUES_TO_DROP = PHI_VALUES_DICT_ALL
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: Portion Paths and conditions
+MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
+WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
+
+LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
+
+# Arguments; General
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `COLUMN_VALUES_TO_DROP`: "{COLUMN_VALUES_TO_DROP}"
+    `USE_MODIFIED_OMOP_DATA_SET`: "{USE_MODIFIED_OMOP_DATA_SET}"
+    `MAC_PATHS`: "{MAC_PATHS}"
+    `WIN_PATHS`: "{WIN_PATHS}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    logger.info("""De-identifying files.""")
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+        for file in directory.iterdir():
+            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logger.info("""    File has met all conditions for processing.""")
+                logger.info("""  ..  Reading file to count the number of chunks.""")
+                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE)])
+                logger.info(f"""  ..  This file has {numChunks} chunks.""")
+                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    # Work on chunk
+                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        # Work on column
+                        logger.info(f"""  ..    Working on column "{columnName}".""")
+                        if columnName in COLUMN_VALUES_TO_DROP.keys():
+                            mask = ~dfChunk[columnName].isin(COLUMN_VALUES_TO_DROP[columnName])
+                            if mask.sum() > 0:
+                                logger.info("""  ..  ..  Column has values that need to be dropped. Dropping values.""")
+                            dfChunk = dfChunk[mask]
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logger.info("""    This file does not need to be processed.""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,297 +1,297 @@
-"""
-De-identify files
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-# TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
-# TODO Investigate if a symlink can be made for files that are copied without alteration, to save space and time on larger projects.
-"""
-
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (flatExtend,
-                                    getTimestamp,
-                                    makeDirPath,
-                                    readDataFile,
-                                    successiveParents)
-from drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE,
-                                          LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE_CONDITIONAL)
-# Project parameters: General
-from common import (STUDY_TYPE,
-                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-# Project parameters: Portion paths and criteria
-from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
-                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
-                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
-                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
-                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
-
-# Arguments: Use concatenated files
-USE_CONCATENATED_FILES = True  # TODO
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Arguments: File location definition: By concatenation
-CONCATENATED_PORTIONS_DIR_MAC = Path(r"..\Concatenated Results\data\output\deleteByColumnValues\...")  # TODO
-CONCATENATED_PORTIONS_DIR_WIN = Path(r"..\Concatenated Results\data\output\deleteByColumnValues\...")  # TODO
-
-# Arguments: Portion Paths and conditions
-if USE_MODIFIED_OMOP_DATA_SET:
-    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
-else:
-    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
-
-# Arguments: File location definition: OS-specific
-# There are two typical workflows. Deleting columns in the beginning of the workflow, or towards the end, after it's been de-identified (i.e., "concatenated")
-
-if USE_CONCATENATED_FILES:
-    MAC_PATHS = [CONCATENATED_PORTIONS_DIR_MAC]
-    WIN_PATHS = [CONCATENATED_PORTIONS_DIR_WIN]
-else:
-    MAC_PATHS = [BO_PORTION_DIR_MAC,
-                 I2B2_PORTION_DIR_MAC,
-                 NOTES_PORTION_DIR_MAC,
-                 OMOPPortionDirMac]
-    WIN_PATHS = [BO_PORTION_DIR_WIN,
-                 I2B2_PORTION_DIR_WIN,
-                 OMOPPortionDirWin,
-                 NOTES_PORTION_DIR_WIN]
-
-# Arguments: Definition of criteria for file release
-# NOTE (Developer's Note) The files to release and the file criteiria both act as criteria to release. The argument structure here is not very clear and it will take some time to create a generalizeable template. However, it seems that `LIST_OF_PORTION_CONDITIONS` is the only output of this arguments section, i.e., the only require input for the script. Also note that each portion has its own criteria, but they are not used in the template.
-BO_FILES_TO_RELEASE = []  # TODO
-
-NOTES_COHORT_NAME = ""  # TODO
-NOTES_METADATA_FILES_TO_RELEASE = ["provider_metadata.csv",
-                                   f"{NOTES_COHORT_NAME}_note_metadata.csv",
-                                   f"{NOTES_COHORT_NAME}_order_impression_metadata.csv",
-                                   f"{NOTES_COHORT_NAME}_order_metadata.csv",
-                                   f"{NOTES_COHORT_NAME}_order_narrative_metadata.csv",
-                                   f"{NOTES_COHORT_NAME}_order_result_comment_metadata.csv"]
-
-I2B2_COHORT_NAME = ""  # TODO
-I2B2_FILES_TO_RELEASE = [f"{I2B2_COHORT_NAME}_observation_fact_GNV.csv",
-                         f"{I2B2_COHORT_NAME}_observation_fact_JAX.csv",
-                         f"{I2B2_COHORT_NAME}_patient_dimension_GNV.csv",
-                         f"{I2B2_COHORT_NAME}_patient_dimension_JAX.csv",
-                         f"{I2B2_COHORT_NAME}_visit_dimension_GNV.csv",
-                         f"{I2B2_COHORT_NAME}_visit_dimension_JAX.csv"]
-
-OMOP_FILES_TO_RELEASE = ["condition_occurrence.csv",
-                         "death.csv",
-                         "device_exposure.csv",
-                         "drug_exposure.csv",
-                         "location.csv",
-                         "measurement_laboratories.csv",
-                         "measurement.csv",
-                         "observation_period.csv",
-                         "observation.csv",
-                         "person.csv",
-                         "procedure_occurrence.csv",
-                         "visit_occurrence.csv"]
-
-ZIP_CODE_FILES_TO_RELEASE = ["zipcodes.csv"]
-
-FILES_TO_RELEASE = flatExtend([BO_FILES_TO_RELEASE,
-                               NOTES_METADATA_FILES_TO_RELEASE,
-                               OMOP_FILES_TO_RELEASE])
-FILES_TO_RELEASE = [fname.lower() for fname in FILES_TO_RELEASE]
-
-
-CONCATENATED_PORTIONS_FILE_CRITERIA = [lambda pathObj: pathObj.name.lower() in FILES_TO_RELEASE,
-                                       lambda pathObj: pathObj.suffix.lower() == ".csv",
-                                       lambda pathObj: pathObj.is_file()]
-
-LIST_OF_PORTION_CONDITIONS = [CONCATENATED_PORTIONS_FILE_CRITERIA]
-
-# Arguments: Columns to delete: By portion
-# TODO Columns to delete. The list variable deletes column matches in any file. The dictionary variable delete the columns that are in the file named in the dictionary key.
-if STUDY_TYPE == "Non-Human":
-    COLUMNS_TO_DELETE_BO = ["HIV Status"]
-else:
-    COLUMNS_TO_DELETE_BO = []
-
-COLUMNS_TO_DELETE_I2B2 = ["LOCATION_CD"]
-
-COLUMNS_TO_DELETE_OMOP = ["person_source_value"] + LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE
-
-COLUMNS_TO_DELETE = flatExtend([COLUMNS_TO_DELETE_BO,
-                                COLUMNS_TO_DELETE_I2B2,
-                                COLUMNS_TO_DELETE_OMOP])
-
-# Arguments: Columns to delete: By file
-if STUDY_TYPE == "Non-Human":
-    COLUMNS_TO_DELETE_OMOP_TABLE_PERSON = LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE_CONDITIONAL
-else:
-    COLUMNS_TO_DELETE_OMOP_TABLE_PERSON = []
-if STUDY_TYPE == "Non-Human":
-    COLUMNS_TO_DELETE_OMOP_TABLE_LOCATION = ["address_1",
-                                             "address_2",
-                                             "city",
-                                             "county",
-                                             "latitude",
-                                             "longitude",
-                                             "zip"]
-elif STUDY_TYPE == "Limited Data Set (LDS)":
-    COLUMNS_TO_DELETE_OMOP_TABLE_LOCATION = ["address_1",
-                                             "address_2",
-                                             "latitude",
-                                             "longitude"]
-else:
-    raise Exception(f"""Unexpected value for `STUDY_TYPE`: "{STUDY_TYPE}".""")
-
-COLUMNS_TO_DELETE_DICT = {"condition_occurrence": [],
-                          "death": [],
-                          "device_exposure": [],
-                          "drug_exposure": ["sig"],
-                          "encounters": [],
-                          "location": COLUMNS_TO_DELETE_OMOP_TABLE_LOCATION,
-                          "measurement": [],
-                          "measurement_laboratories": [],
-                          "observation": [],
-                          "observation_period": [],
-                          "person": COLUMNS_TO_DELETE_OMOP_TABLE_PERSON,
-                          "procedure_occurrence": [],
-                          "visit_occurrence": []}
-
-# Arguments: General
-
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # De-identify columns
-    logging.info("""Deleting columns not authorized for release.""")
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            logging.info(f"""  Conditions: "{conditions}".""")
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logging.info("""    File has met all conditions for processing.""")
-                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
-                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    # Work on chunk
-                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        logging.info(f"""  ..    Working on column "{columnName}".""")
-                        if file.stem in COLUMNS_TO_DELETE_DICT.keys():
-                            listOfColumns = COLUMNS_TO_DELETE + COLUMNS_TO_DELETE_DICT[file.stem]
-                        else:
-                            listOfColumns = COLUMNS_TO_DELETE
-                        if columnName in listOfColumns:
-                            logging.info("""  ..  ..  Column must be deleted. Deleting column.""")
-                            dfChunk = dfChunk.drop(columns=columnName)
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logging.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logging.info("""    This file does not need to be processed.""")
-
-    # Clean up
-    # TODO If input directory is empty, delete
-    # TODO Delete intermediate run directory
-
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+De-identify files
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+# TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
+# TODO Investigate if a symlink can be made for files that are copied without alteration, to save space and time on larger projects.
+"""
+
+import logging
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (flatExtend,
+                                    getTimestamp,
+                                    makeDirPath,
+                                    readDataFile,
+                                    successiveParents)
+from drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE,
+                                          LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE_CONDITIONAL)
+# Project parameters: General
+from common import (STUDY_TYPE,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+# Project parameters: Portion paths and criteria
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
+                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+
+# Arguments: Use concatenated files
+USE_CONCATENATED_FILES = True  # TODO
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: File location definition: By concatenation
+CONCATENATED_PORTIONS_DIR_MAC = Path(r"..\Concatenated Results\data\output\deleteByColumnValues\...")  # TODO
+CONCATENATED_PORTIONS_DIR_WIN = Path(r"..\Concatenated Results\data\output\deleteByColumnValues\...")  # TODO
+
+# Arguments: Portion Paths and conditions
+if USE_MODIFIED_OMOP_DATA_SET:
+    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
+else:
+    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
+
+# Arguments: File location definition: OS-specific
+# There are two typical workflows. Deleting columns in the beginning of the workflow, or towards the end, after it's been de-identified (i.e., "concatenated")
+
+if USE_CONCATENATED_FILES:
+    MAC_PATHS = [CONCATENATED_PORTIONS_DIR_MAC]
+    WIN_PATHS = [CONCATENATED_PORTIONS_DIR_WIN]
+else:
+    MAC_PATHS = [BO_PORTION_DIR_MAC,
+                 I2B2_PORTION_DIR_MAC,
+                 NOTES_PORTION_DIR_MAC,
+                 OMOPPortionDirMac]
+    WIN_PATHS = [BO_PORTION_DIR_WIN,
+                 I2B2_PORTION_DIR_WIN,
+                 OMOPPortionDirWin,
+                 NOTES_PORTION_DIR_WIN]
+
+# Arguments: Definition of criteria for file release
+# NOTE (Developer's Note) The files to release and the file criteiria both act as criteria to release. The argument structure here is not very clear and it will take some time to create a generalizeable template. However, it seems that `LIST_OF_PORTION_CONDITIONS` is the only output of this arguments section, i.e., the only require input for the script. Also note that each portion has its own criteria, but they are not used in the template.
+BO_FILES_TO_RELEASE = []  # TODO
+
+NOTES_COHORT_NAME = ""  # TODO
+NOTES_METADATA_FILES_TO_RELEASE = ["provider_metadata.csv",
+                                   f"{NOTES_COHORT_NAME}_note_metadata.csv",
+                                   f"{NOTES_COHORT_NAME}_order_impression_metadata.csv",
+                                   f"{NOTES_COHORT_NAME}_order_metadata.csv",
+                                   f"{NOTES_COHORT_NAME}_order_narrative_metadata.csv",
+                                   f"{NOTES_COHORT_NAME}_order_result_comment_metadata.csv"]
+
+I2B2_COHORT_NAME = ""  # TODO
+I2B2_FILES_TO_RELEASE = [f"{I2B2_COHORT_NAME}_observation_fact_GNV.csv",
+                         f"{I2B2_COHORT_NAME}_observation_fact_JAX.csv",
+                         f"{I2B2_COHORT_NAME}_patient_dimension_GNV.csv",
+                         f"{I2B2_COHORT_NAME}_patient_dimension_JAX.csv",
+                         f"{I2B2_COHORT_NAME}_visit_dimension_GNV.csv",
+                         f"{I2B2_COHORT_NAME}_visit_dimension_JAX.csv"]
+
+OMOP_FILES_TO_RELEASE = ["condition_occurrence.csv",
+                         "death.csv",
+                         "device_exposure.csv",
+                         "drug_exposure.csv",
+                         "location.csv",
+                         "measurement_laboratories.csv",
+                         "measurement.csv",
+                         "observation_period.csv",
+                         "observation.csv",
+                         "person.csv",
+                         "procedure_occurrence.csv",
+                         "visit_occurrence.csv"]
+
+ZIP_CODE_FILES_TO_RELEASE = ["zipcodes.csv"]
+
+FILES_TO_RELEASE = flatExtend([BO_FILES_TO_RELEASE,
+                               NOTES_METADATA_FILES_TO_RELEASE,
+                               OMOP_FILES_TO_RELEASE])
+FILES_TO_RELEASE = [fname.lower() for fname in FILES_TO_RELEASE]
+
+
+CONCATENATED_PORTIONS_FILE_CRITERIA = [lambda pathObj: pathObj.name.lower() in FILES_TO_RELEASE,
+                                       lambda pathObj: pathObj.suffix.lower() == ".csv",
+                                       lambda pathObj: pathObj.is_file()]
+
+LIST_OF_PORTION_CONDITIONS = [CONCATENATED_PORTIONS_FILE_CRITERIA]
+
+# Arguments: Columns to delete: By portion
+# TODO Columns to delete. The list variable deletes column matches in any file. The dictionary variable delete the columns that are in the file named in the dictionary key.
+if STUDY_TYPE == "Non-Human":
+    COLUMNS_TO_DELETE_BO = ["HIV Status"]
+else:
+    COLUMNS_TO_DELETE_BO = []
+
+COLUMNS_TO_DELETE_I2B2 = ["LOCATION_CD"]
+
+COLUMNS_TO_DELETE_OMOP = ["person_source_value"] + LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE
+
+COLUMNS_TO_DELETE = flatExtend([COLUMNS_TO_DELETE_BO,
+                                COLUMNS_TO_DELETE_I2B2,
+                                COLUMNS_TO_DELETE_OMOP])
+
+# Arguments: Columns to delete: By file
+if STUDY_TYPE == "Non-Human":
+    COLUMNS_TO_DELETE_OMOP_TABLE_PERSON = LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE_CONDITIONAL
+else:
+    COLUMNS_TO_DELETE_OMOP_TABLE_PERSON = []
+if STUDY_TYPE == "Non-Human":
+    COLUMNS_TO_DELETE_OMOP_TABLE_LOCATION = ["address_1",
+                                             "address_2",
+                                             "city",
+                                             "county",
+                                             "latitude",
+                                             "longitude",
+                                             "zip"]
+elif STUDY_TYPE == "Limited Data Set (LDS)":
+    COLUMNS_TO_DELETE_OMOP_TABLE_LOCATION = ["address_1",
+                                             "address_2",
+                                             "latitude",
+                                             "longitude"]
+else:
+    raise Exception(f"""Unexpected value for `STUDY_TYPE`: "{STUDY_TYPE}".""")
+
+COLUMNS_TO_DELETE_DICT = {"condition_occurrence": [],
+                          "death": [],
+                          "device_exposure": [],
+                          "drug_exposure": ["sig"],
+                          "encounters": [],
+                          "location": COLUMNS_TO_DELETE_OMOP_TABLE_LOCATION,
+                          "measurement": [],
+                          "measurement_laboratories": [],
+                          "observation": [],
+                          "observation_period": [],
+                          "person": COLUMNS_TO_DELETE_OMOP_TABLE_PERSON,
+                          "procedure_occurrence": [],
+                          "visit_occurrence": []}
+
+# Arguments: General
+
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # De-identify columns
+    logging.info("""Deleting columns not authorized for release.""")
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+        for file in directory.iterdir():
+            logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            logging.info(f"""  Conditions: "{conditions}".""")
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logging.info("""    File has met all conditions for processing.""")
+                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    # Work on chunk
+                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        # Work on column
+                        logging.info(f"""  ..    Working on column "{columnName}".""")
+                        if file.stem in COLUMNS_TO_DELETE_DICT.keys():
+                            listOfColumns = COLUMNS_TO_DELETE + COLUMNS_TO_DELETE_DICT[file.stem]
+                        else:
+                            listOfColumns = COLUMNS_TO_DELETE
+                        if columnName in listOfColumns:
+                            logging.info("""  ..  ..  Column must be deleted. Deleting column.""")
+                            dfChunk = dfChunk.drop(columns=columnName)
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logging.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logging.info("""    This file does not need to be processed.""")
+
+    # Clean up
+    # TODO If input directory is empty, delete
+    # TODO Delete intermediate run directory
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-"""
-Get the set of ID values for all variables to de-identify.
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-"""
-
-__all__ = ["runIntermediateDataDir"]
-
-import csv
-import json
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from pandas.errors import EmptyDataError
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    readDataFile,
-                                    sortIntegersAndStrings,
-                                    successiveParents)
-from drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT
-# Project parameters: General
-from common import (COLUMNS_TO_DE_IDENTIFY,
-                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    DATA_TYPES_DICT)
-# Project parameters: Portion paths and criteria
-from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
-                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
-                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
-                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
-                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
-# Project parameters: Criteria
-from common import (BO_PORTION_FILE_CRITERIA,
-                    I2B2_PORTION_FILE_CRITERIA,
-                    NOTES_PORTION_FILE_CRITERIA,
-                    OMOP_PORTION_FILE_CRITERIA)
-
-
-# Arguments
-SETS_INTERMEDIATE_PATH = None
-
-CHUNK_SIZE = 50000
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Arguments: Portion Paths and conditions
-if USE_MODIFIED_OMOP_DATA_SET:
-    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
-else:
-    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
-
-PORTION_PATHS_MAC = {"BO": BO_PORTION_DIR_MAC,
-                     "i2b2": I2B2_PORTION_DIR_MAC,
-                     "Notes": NOTES_PORTION_DIR_MAC,
-                     "OMOP": OMOPPortionDirMac}
-PORTION_PATHS_WIN = {"BO": BO_PORTION_DIR_WIN,
-                     "i2b2": I2B2_PORTION_DIR_WIN,
-                     "Notes": NOTES_PORTION_DIR_WIN,
-                     "OMOP": OMOPPortionDirWin}
-
-DICT_OF_PORTION_CONDITIONS = {"BO": BO_PORTION_FILE_CRITERIA,
-                              "i2b2": I2B2_PORTION_FILE_CRITERIA,
-                              "Notes": NOTES_PORTION_FILE_CRITERIA,
-                              "OMOP": OMOP_PORTION_FILE_CRITERIA}
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in PORTION_PATHS_MAC.values()]) or all([path.exists() for path in PORTION_PATHS_WIN.values()])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        dictOfPortionPaths = PORTION_PATHS_MAC.copy()
-    elif operatingSystem == "win32":
-        dictOfPortionPaths = PORTION_PATHS_WIN.copy()
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Match portion paths and conditions
-    portionPathsAndConditions = {portionName: (dictOfPortionPaths[portionName], DICT_OF_PORTION_CONDITIONS[portionName]) for portionName in dictOfPortionPaths.keys()}
-    check1 = [pn1 in DICT_OF_PORTION_CONDITIONS.keys() for pn1 in dictOfPortionPaths.keys()]
-    check2 = [pn2 in dictOfPortionPaths.keys() for pn2 in DICT_OF_PORTION_CONDITIONS.keys()]
-    assert sum(check1) == len(check1), "Not all portion paths are associated with a portion condition"
-    assert sum(check2) == len(check2), "Not all portion conditions are associated with a portion path"
-
-    # Misc
-    columnSetsVarsDiFname = "Column Sets Dict.JSON"
-
-    # Get set of values
-    if SETS_INTERMEDIATE_PATH:
-        logging.info(f"""Using the set of values previously collected from "{SETS_INTERMEDIATE_PATH}".""")
-        with open(SETS_INTERMEDIATE_PATH.joinpath(columnSetsVarsDiFname)) as file:
-            columnSetsVarsDi = json.loads(file.read())
-    else:
-        logging.info("""Getting the set of values for each variable to de-identify.""")
-        columnSetsVarsDi = {columnName: {"fpath": runIntermediateDataDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[columnName]}.txt"),
-                                         "fileMode": "w",
-                                         "portionName": None,
-                                         "collected": False} for columnName in COLUMNS_TO_DE_IDENTIFY}
-        for portionName, (directory, fileConditions) in portionPathsAndConditions.items():
-            # Act on directory
-            logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-            for file in directory.iterdir():
-                logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-                conditions = [condition(file) for condition in fileConditions]
-                if all(conditions):
-                    # Read file
-                    logging.info("""    File has met all conditions for processing.""")
-                    numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
-                    dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
-                    for it, dfChunk in enumerate(dfChunks, start=1):
-                        dfChunk = pd.DataFrame(dfChunk)
-                        logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                        for columnName in dfChunk.columns:
-                            logging.info(f"""  ..    Working on column "{columnName}".""")
-                            if columnName in COLUMNS_TO_DE_IDENTIFY:
-                                logging.info("""  ..  ..  Column must be de-identified. Collecting values.""")
-                                dataType = DATA_TYPES_DICT[columnName]
-                                series = dfChunk[columnName]
-                                series = series.dropna()
-                                series = series.drop_duplicates()
-                                if dataType == "Datetime":
-                                    values = series.sort_values()
-                                    quoting = csv.QUOTE_NONE
-                                elif dataType == "Numeric":
-                                    series = series.astype(float).astype("Int64")
-                                    values = series.sort_values()
-                                    quoting = csv.QUOTE_NONE
-                                elif dataType == "String":
-                                    values = series.astype(str).sort_values()
-                                    quoting = csv.QUOTE_ALL
-                                elif dataType == "Numeric_Or_String":
-                                    mask = series.apply(lambda el: isinstance(el, float))
-                                    series.loc[mask[mask].index] = series[mask].astype(int)
-                                    values = sortIntegersAndStrings(series.to_list())
-                                    values = pd.Series(values)
-                                    quoting = csv.QUOTE_ALL
-                                else:
-                                    raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
-                                columnSetFpath = columnSetsVarsDi[columnName]["fpath"]
-                                columnSetFileMode = columnSetsVarsDi[columnName]["fileMode"]
-                                # logging.info(f"""  ..  ..  Values table preview:\n{values.head()}.""")
-                                values.to_csv(path_or_buf=columnSetFpath,
-                                              quoting=quoting,
-                                              index=False,
-                                              header=False,
-                                              mode=columnSetFileMode)
-                                # logging.info(f"""  ..  ..  Preview of table after saving:\n{pd.read_table(columnSetFpath)}.""")
-                                columnSetsVarsDi[columnName]["fileMode"] = "a"
-                                columnSetsVarsDi[columnName]["portionName"] = portionName
-                                columnSetsVarsDi[columnName]["collected"] = True
-                                logging.info(f"""  ..  ..  Values saved to "{columnSetFpath.absolute().relative_to(rootDirectory)}" in the project directory.""")
-                else:
-                    logging.info("""    This file does not need to be processed.""")
-
-        columnSetsVarsDiPath = runIntermediateDataDir.joinpath("Metadata", columnSetsVarsDiFname)
-        makeDirPath(columnSetsVarsDiPath.parent)
-        columnSetsVarsDiSerializable = columnSetsVarsDi.copy()
-        for columnName, di in columnSetsVarsDiSerializable.items():
-            columnSetsVarsDiSerializable[columnName]["fpath"] = str(di["fpath"])
-        with open(columnSetsVarsDiPath, "w") as file:
-            file.write(json.dumps(columnSetsVarsDi))
-
-    # Drop variables that weren't found
-    for columnName in COLUMNS_TO_DE_IDENTIFY:
-        if columnName in columnSetsVarsDi.keys():
-            if columnSetsVarsDi[columnName]["collected"] is False:
-                columnSetsVarsDi.pop(columnName)
-
-    # Remove duplicates from set files and save according to data type
-    logging.info("Removing duplicates from set files and saving according to data type.")
-    columnSetsVarsLi = sorted(list(columnSetsVarsDi.items()), key=lambda tu: tu[0].lower())
-    for columnName, fileDi in columnSetsVarsLi:
-        logging.info(f"""  Working on variable "{columnName}".""")
-        fpath = fileDi["fpath"]
-        try:
-            series = pd.read_table(fpath, header=None)[0]
-        except EmptyDataError as err:
-            _ = err
-            series = pd.Series(dtype=str)
-        # Save according to data type
-        portionName = fileDi["portionName"]
-        dataType = DATA_TYPES_DICT[columnName]
-        if dataType == "Datetime":
-            quoting = csv.QUOTE_MINIMAL
-        elif dataType == "Numeric":
-            series = series.astype(float).astype("Int64")
-            quoting = csv.QUOTE_MINIMAL
-        elif dataType == "String":
-            quoting = csv.QUOTE_ALL
-        elif dataType == "Numeric_Or_String":
-            quoting = csv.QUOTE_ALL
-        else:
-            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
-        series = series.drop_duplicates()
-        series = series.sort_values()
-        fpath2 = runOutputDir.joinpath("Set Files", f"{VARIABLE_NAME_TO_FILE_NAME_DICT[columnName]}.txt")
-        makeDirPath(fpath2.parent)
-        series.to_csv(fpath2, quoting=quoting, index=False, header=False)
-
-    # Return path to sets fo ID values
-    # TODO If this is implemented as a function, instead of a stand-alone script, return `runOutputDir` to define `setsPathDir` in the "makeMap" scripts.
-    logging.info(f"""Finished collecting the set of ID values to de-identify. The set files are located in "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Get the set of ID values for all variables to de-identify.
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+"""
+
+__all__ = ["runIntermediateDataDir"]
+
+import csv
+import json
+import logging
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from pandas.errors import EmptyDataError
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    readDataFile,
+                                    sortIntegersAndStrings,
+                                    successiveParents)
+from drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT
+# Project parameters: General
+from common import (COLUMNS_TO_DE_IDENTIFY,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
+                    DATA_TYPES_DICT)
+# Project parameters: Portion paths and criteria
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
+                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+# Project parameters: Criteria
+from common import (BO_PORTION_FILE_CRITERIA,
+                    I2B2_PORTION_FILE_CRITERIA,
+                    NOTES_PORTION_FILE_CRITERIA,
+                    OMOP_PORTION_FILE_CRITERIA)
+
+
+# Arguments
+SETS_INTERMEDIATE_PATH = None
+
+CHUNK_SIZE = 50000
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: Portion Paths and conditions
+if USE_MODIFIED_OMOP_DATA_SET:
+    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
+else:
+    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
+
+PORTION_PATHS_MAC = {"BO": BO_PORTION_DIR_MAC,
+                     "i2b2": I2B2_PORTION_DIR_MAC,
+                     "Notes": NOTES_PORTION_DIR_MAC,
+                     "OMOP": OMOPPortionDirMac}
+PORTION_PATHS_WIN = {"BO": BO_PORTION_DIR_WIN,
+                     "i2b2": I2B2_PORTION_DIR_WIN,
+                     "Notes": NOTES_PORTION_DIR_WIN,
+                     "OMOP": OMOPPortionDirWin}
+
+DICT_OF_PORTION_CONDITIONS = {"BO": BO_PORTION_FILE_CRITERIA,
+                              "i2b2": I2B2_PORTION_FILE_CRITERIA,
+                              "Notes": NOTES_PORTION_FILE_CRITERIA,
+                              "OMOP": OMOP_PORTION_FILE_CRITERIA}
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in PORTION_PATHS_MAC.values()]) or all([path.exists() for path in PORTION_PATHS_WIN.values()])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        dictOfPortionPaths = PORTION_PATHS_MAC.copy()
+    elif operatingSystem == "win32":
+        dictOfPortionPaths = PORTION_PATHS_WIN.copy()
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # Match portion paths and conditions
+    portionPathsAndConditions = {portionName: (dictOfPortionPaths[portionName], DICT_OF_PORTION_CONDITIONS[portionName]) for portionName in dictOfPortionPaths.keys()}
+    check1 = [pn1 in DICT_OF_PORTION_CONDITIONS.keys() for pn1 in dictOfPortionPaths.keys()]
+    check2 = [pn2 in dictOfPortionPaths.keys() for pn2 in DICT_OF_PORTION_CONDITIONS.keys()]
+    assert sum(check1) == len(check1), "Not all portion paths are associated with a portion condition"
+    assert sum(check2) == len(check2), "Not all portion conditions are associated with a portion path"
+
+    # Misc
+    columnSetsVarsDiFname = "Column Sets Dict.JSON"
+
+    # Get set of values
+    if SETS_INTERMEDIATE_PATH:
+        logging.info(f"""Using the set of values previously collected from "{SETS_INTERMEDIATE_PATH}".""")
+        with open(SETS_INTERMEDIATE_PATH.joinpath(columnSetsVarsDiFname)) as file:
+            columnSetsVarsDi = json.loads(file.read())
+    else:
+        logging.info("""Getting the set of values for each variable to de-identify.""")
+        columnSetsVarsDi = {columnName: {"fpath": runIntermediateDataDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[columnName]}.txt"),
+                                         "fileMode": "w",
+                                         "portionName": None,
+                                         "collected": False} for columnName in COLUMNS_TO_DE_IDENTIFY}
+        for portionName, (directory, fileConditions) in portionPathsAndConditions.items():
+            # Act on directory
+            logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+            for file in directory.iterdir():
+                logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+                conditions = [condition(file) for condition in fileConditions]
+                if all(conditions):
+                    # Read file
+                    logging.info("""    File has met all conditions for processing.""")
+                    numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                    dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                    for it, dfChunk in enumerate(dfChunks, start=1):
+                        dfChunk = pd.DataFrame(dfChunk)
+                        logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                        for columnName in dfChunk.columns:
+                            logging.info(f"""  ..    Working on column "{columnName}".""")
+                            if columnName in COLUMNS_TO_DE_IDENTIFY:
+                                logging.info("""  ..  ..  Column must be de-identified. Collecting values.""")
+                                dataType = DATA_TYPES_DICT[columnName]
+                                series = dfChunk[columnName]
+                                series = series.dropna()
+                                series = series.drop_duplicates()
+                                if dataType == "Datetime":
+                                    values = series.sort_values()
+                                    quoting = csv.QUOTE_NONE
+                                elif dataType == "Numeric":
+                                    series = series.astype(float).astype("Int64")
+                                    values = series.sort_values()
+                                    quoting = csv.QUOTE_NONE
+                                elif dataType == "String":
+                                    values = series.astype(str).sort_values()
+                                    quoting = csv.QUOTE_ALL
+                                elif dataType == "Numeric_Or_String":
+                                    mask = series.apply(lambda el: isinstance(el, float))
+                                    series.loc[mask[mask].index] = series[mask].astype(int)
+                                    values = sortIntegersAndStrings(series.to_list())
+                                    values = pd.Series(values)
+                                    quoting = csv.QUOTE_ALL
+                                else:
+                                    raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
+                                columnSetFpath = columnSetsVarsDi[columnName]["fpath"]
+                                columnSetFileMode = columnSetsVarsDi[columnName]["fileMode"]
+                                # logging.info(f"""  ..  ..  Values table preview:\n{values.head()}.""")
+                                values.to_csv(path_or_buf=columnSetFpath,
+                                              quoting=quoting,
+                                              index=False,
+                                              header=False,
+                                              mode=columnSetFileMode)
+                                # logging.info(f"""  ..  ..  Preview of table after saving:\n{pd.read_table(columnSetFpath)}.""")
+                                columnSetsVarsDi[columnName]["fileMode"] = "a"
+                                columnSetsVarsDi[columnName]["portionName"] = portionName
+                                columnSetsVarsDi[columnName]["collected"] = True
+                                logging.info(f"""  ..  ..  Values saved to "{columnSetFpath.absolute().relative_to(rootDirectory)}" in the project directory.""")
+                else:
+                    logging.info("""    This file does not need to be processed.""")
+
+        columnSetsVarsDiPath = runIntermediateDataDir.joinpath("Metadata", columnSetsVarsDiFname)
+        makeDirPath(columnSetsVarsDiPath.parent)
+        columnSetsVarsDiSerializable = columnSetsVarsDi.copy()
+        for columnName, di in columnSetsVarsDiSerializable.items():
+            columnSetsVarsDiSerializable[columnName]["fpath"] = str(di["fpath"])
+        with open(columnSetsVarsDiPath, "w") as file:
+            file.write(json.dumps(columnSetsVarsDi))
+
+    # Drop variables that weren't found
+    for columnName in COLUMNS_TO_DE_IDENTIFY:
+        if columnName in columnSetsVarsDi.keys():
+            if columnSetsVarsDi[columnName]["collected"] is False:
+                columnSetsVarsDi.pop(columnName)
+
+    # Remove duplicates from set files and save according to data type
+    logging.info("Removing duplicates from set files and saving according to data type.")
+    columnSetsVarsLi = sorted(list(columnSetsVarsDi.items()), key=lambda tu: tu[0].lower())
+    for columnName, fileDi in columnSetsVarsLi:
+        logging.info(f"""  Working on variable "{columnName}".""")
+        fpath = fileDi["fpath"]
+        try:
+            series = pd.read_table(fpath, header=None)[0]
+        except EmptyDataError as err:
+            _ = err
+            series = pd.Series(dtype=str)
+        # Save according to data type
+        portionName = fileDi["portionName"]
+        dataType = DATA_TYPES_DICT[columnName]
+        if dataType == "Datetime":
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "Numeric":
+            series = series.astype(float).astype("Int64")
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "String":
+            quoting = csv.QUOTE_ALL
+        elif dataType == "Numeric_Or_String":
+            quoting = csv.QUOTE_ALL
+        else:
+            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
+        series = series.drop_duplicates()
+        series = series.sort_values()
+        fpath2 = runOutputDir.joinpath("Set Files", f"{VARIABLE_NAME_TO_FILE_NAME_DICT[columnName]}.txt")
+        makeDirPath(fpath2.parent)
+        series.to_csv(fpath2, quoting=quoting, index=False, header=False)
+
+    # Return path to sets fo ID values
+    # TODO If this is implemented as a function, instead of a stand-alone script, return `runOutputDir` to define `setsPathDir` in the "makeMap" scripts.
+    logging.info(f"""Finished collecting the set of ID values to de-identify. The set files are located in "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-"""
-Get all variables/columns of tables/files in the project.
-"""
-
-import logging
-import os
-import sys
-from collections import OrderedDict
-from pathlib import Path
-# Third-party packages
-import numpy as np
-import pandas as pd
-from colorama import init as colorama_init
-from colorama import (Fore,
-                      Style)
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-# Project parameters:
-from common import DATA_REQUEST_ROOT_DIRECTORY_DEPTH
-# Project parameters: Portion paths and criteria
-from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
-                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
-                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
-                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
-                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
-# Project parameters: Criteria
-from common import (BO_PORTION_FILE_CRITERIA,
-                    I2B2_PORTION_FILE_CRITERIA,
-                    NOTES_PORTION_FILE_CRITERIA,
-                    OMOP_PORTION_FILE_CRITERIA)
-from drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
-                                          LIST_OF_PHI_DATES_NOTES,
-                                          LIST_OF_PHI_DATES_OMOP)
-
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
-
-# Arguments: Portion Paths and conditions
-if USE_MODIFIED_OMOP_DATA_SET:
-    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
-else:
-    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
-    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
-
-PORTIONS_OUTPUT_DIR_PATH_MAC = {"BO": BO_PORTION_DIR_MAC,  # TODO
-                                "i2b2": I2B2_PORTION_DIR_MAC,
-                                "Notes": NOTES_PORTION_DIR_MAC,
-                                "OMOP": OMOP_PORTION_DIR_MAC}
-PORTIONS_OUTPUT_DIR_PATH_WIN = {"BO": BO_PORTION_DIR_WIN,  # TODO
-                                "i2b2": I2B2_PORTION_DIR_WIN,
-                                "Notes": NOTES_PORTION_DIR_WIN,
-                                "OMOP": OMOP_PORTION_DIR_WIN}
-PORTION_FILE_CRITERIA_DICT = {"BO": BO_PORTION_FILE_CRITERIA,
-                              "i2b2": I2B2_PORTION_FILE_CRITERIA,
-                              "Notes": NOTES_PORTION_FILE_CRITERIA,
-                              "OMOP": OMOP_PORTION_FILE_CRITERIA}
-
-COMPARISON_SET = LIST_OF_PHI_DATES_BO + LIST_OF_PHI_DATES_NOTES + LIST_OF_PHI_DATES_OMOP
-
-# Arguments: Meta-variables
-LOG_LEVEL = "DEBUG"
-
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = np.all([path.exists() for path in PORTIONS_OUTPUT_DIR_PATH_MAC.values()]) or np.all([path.exists() for path in PORTIONS_OUTPUT_DIR_PATH_WIN.values()])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        portionsOutputDirPath = PORTIONS_OUTPUT_DIR_PATH_MAC
-    elif operatingSystem == "win32":
-        portionsOutputDirPath = PORTIONS_OUTPUT_DIR_PATH_WIN
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    ``: "{"..."}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-    """)
-    # Colorama initialization
-    colorama_init()
-
-    # Get columns
-    columns = {}
-    columnsByPortion = {portionName: {} for portionName in portionsOutputDirPath.keys()}
-    for portionName, portionPath in portionsOutputDirPath.items():
-        content_paths = [Path(dirObj) for dirObj in os.scandir(portionPath)]
-        content_names = "\n  ".join(sorted([path.name for path in content_paths]))
-        dirRelativePath = portionPath.absolute().relative_to(rootDirectory)
-        logger.info(f"""Reading files from the directory "{dirRelativePath}". Below are its contents:""")
-        for fpath in sorted(content_paths):
-            logger.info(f"""  {fpath.name}""")
-        for file in content_paths:
-            conditions = PORTION_FILE_CRITERIA_DICT[portionName]
-            conditionResults = [func(file) for func in conditions]
-            if all(conditionResults):
-                logger.debug(f"""  Reading "{file.absolute().relative_to(rootDirectory)}".""")
-                df = pd.read_csv(file, dtype=str, nrows=10)
-                columns[file.name] = df.columns
-                columnsByPortion[portionName][file.name] = df.columns
-
-    # Get all columns by file
-    logger.info("""Printing columns by file.""")
-    allColumns = set()
-    it = 0
-    columnsOrdered = OrderedDict(sorted(columns.items()))
-    for key, value1 in columnsOrdered.items():
-        if it > -1:
-            logger.info(key)
-            logger.info("")
-            for el in sorted(value1):
-                logger.info(f"  {el}")
-                allColumns.add(el)
-            logger.info("")
-        it += 1
-
-    # Get all columns by portion and file
-    logger.info("""Printing columns by portion and file.""")
-    allColumnsByPortion = OrderedDict({portionName: set() for portionName in sorted(columnsByPortion.keys())})
-    columnsByPortionOrdered = OrderedDict(sorted(columnsByPortion.items()))
-    for portionName, di in columnsByPortionOrdered.items():
-        logger.info(f"{portionName}")
-        for fileName, value2 in di.items():
-            logger.info(f"  {fileName}")
-            for el in sorted(value2):
-                logger.info(f"    {el}")
-                allColumnsByPortion[portionName].add(el)
-            logger.info("")
-
-    # Print the set of all columns
-    logger.info("""Printing the set of all columns.""")
-    for el in sorted(list(allColumns)):
-        logger.info(f"  {el}")
-    logger.info("")
-
-    # Print the set of all columns by portion
-    logger.info("""Print set of columns by portion.""")
-    for portionName, columnsSet in allColumnsByPortion.items():
-        logger.info(f"""{portionName}""")
-        for columnName in sorted(list(columnsSet)):
-            if columnName in COMPARISON_SET:
-                text = f"""{Fore.LIGHTCYAN_EX}{columnName}{Style.RESET_ALL}"""
-            else:
-                text = columnName
-            logger.info(f"  {text}")
-        logger.info("")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+Get all variables/columns of tables/files in the project.
+"""
+
+import logging
+import os
+import sys
+from collections import OrderedDict
+from pathlib import Path
+# Third-party packages
+import numpy as np
+import pandas as pd
+from colorama import init as colorama_init
+from colorama import (Fore,
+                      Style)
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+# Project parameters:
+from common import DATA_REQUEST_ROOT_DIRECTORY_DEPTH
+# Project parameters: Portion paths and criteria
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
+                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+# Project parameters: Criteria
+from common import (BO_PORTION_FILE_CRITERIA,
+                    I2B2_PORTION_FILE_CRITERIA,
+                    NOTES_PORTION_FILE_CRITERIA,
+                    OMOP_PORTION_FILE_CRITERIA)
+from drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
+                                          LIST_OF_PHI_DATES_NOTES,
+                                          LIST_OF_PHI_DATES_OMOP)
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: Portion Paths and conditions
+if USE_MODIFIED_OMOP_DATA_SET:
+    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
+else:
+    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
+
+PORTIONS_OUTPUT_DIR_PATH_MAC = {"BO": BO_PORTION_DIR_MAC,  # TODO
+                                "i2b2": I2B2_PORTION_DIR_MAC,
+                                "Notes": NOTES_PORTION_DIR_MAC,
+                                "OMOP": OMOP_PORTION_DIR_MAC}
+PORTIONS_OUTPUT_DIR_PATH_WIN = {"BO": BO_PORTION_DIR_WIN,  # TODO
+                                "i2b2": I2B2_PORTION_DIR_WIN,
+                                "Notes": NOTES_PORTION_DIR_WIN,
+                                "OMOP": OMOP_PORTION_DIR_WIN}
+PORTION_FILE_CRITERIA_DICT = {"BO": BO_PORTION_FILE_CRITERIA,
+                              "i2b2": I2B2_PORTION_FILE_CRITERIA,
+                              "Notes": NOTES_PORTION_FILE_CRITERIA,
+                              "OMOP": OMOP_PORTION_FILE_CRITERIA}
+
+COMPARISON_SET = LIST_OF_PHI_DATES_BO + LIST_OF_PHI_DATES_NOTES + LIST_OF_PHI_DATES_OMOP
+
+# Arguments: Meta-variables
+LOG_LEVEL = "DEBUG"
+
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = np.all([path.exists() for path in PORTIONS_OUTPUT_DIR_PATH_MAC.values()]) or np.all([path.exists() for path in PORTIONS_OUTPUT_DIR_PATH_WIN.values()])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        portionsOutputDirPath = PORTIONS_OUTPUT_DIR_PATH_MAC
+    elif operatingSystem == "win32":
+        portionsOutputDirPath = PORTIONS_OUTPUT_DIR_PATH_WIN
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    ``: "{"..."}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+    """)
+    # Colorama initialization
+    colorama_init()
+
+    # Get columns
+    columns = {}
+    columnsByPortion = {portionName: {} for portionName in portionsOutputDirPath.keys()}
+    for portionName, portionPath in portionsOutputDirPath.items():
+        content_paths = [Path(dirObj) for dirObj in os.scandir(portionPath)]
+        content_names = "\n  ".join(sorted([path.name for path in content_paths]))
+        dirRelativePath = portionPath.absolute().relative_to(rootDirectory)
+        logger.info(f"""Reading files from the directory "{dirRelativePath}". Below are its contents:""")
+        for fpath in sorted(content_paths):
+            logger.info(f"""  {fpath.name}""")
+        for file in content_paths:
+            conditions = PORTION_FILE_CRITERIA_DICT[portionName]
+            conditionResults = [func(file) for func in conditions]
+            if all(conditionResults):
+                logger.debug(f"""  Reading "{file.absolute().relative_to(rootDirectory)}".""")
+                df = pd.read_csv(file, dtype=str, nrows=10)
+                columns[file.name] = df.columns
+                columnsByPortion[portionName][file.name] = df.columns
+
+    # Get all columns by file
+    logger.info("""Printing columns by file.""")
+    allColumns = set()
+    it = 0
+    columnsOrdered = OrderedDict(sorted(columns.items()))
+    for key, value1 in columnsOrdered.items():
+        if it > -1:
+            logger.info(key)
+            logger.info("")
+            for el in sorted(value1):
+                logger.info(f"  {el}")
+                allColumns.add(el)
+            logger.info("")
+        it += 1
+
+    # Get all columns by portion and file
+    logger.info("""Printing columns by portion and file.""")
+    allColumnsByPortion = OrderedDict({portionName: set() for portionName in sorted(columnsByPortion.keys())})
+    columnsByPortionOrdered = OrderedDict(sorted(columnsByPortion.items()))
+    for portionName, di in columnsByPortionOrdered.items():
+        logger.info(f"{portionName}")
+        for fileName, value2 in di.items():
+            logger.info(f"  {fileName}")
+            for el in sorted(value2):
+                logger.info(f"    {el}")
+                allColumnsByPortion[portionName].add(el)
+            logger.info("")
+
+    # Print the set of all columns
+    logger.info("""Printing the set of all columns.""")
+    for el in sorted(list(allColumns)):
+        logger.info(f"  {el}")
+    logger.info("")
+
+    # Print the set of all columns by portion
+    logger.info("""Print set of columns by portion.""")
+    for portionName, columnsSet in allColumnsByPortion.items():
+        logger.info(f"""{portionName}""")
+        for columnName in sorted(list(columnsSet)):
+            if columnName in COMPARISON_SET:
+                text = f"""{Fore.LIGHTCYAN_EX}{columnName}{Style.RESET_ALL}"""
+            else:
+                text = columnName
+            logger.info(f"  {text}")
+        logger.info("")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-"""
-Converts i2b2 `PATIENT_NUM` and `ENCOUNTER_NUM` IDs to "Patient Key" and "Encounter # (CSN)", respectively.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from sqlalchemy import create_engine
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-I2B2_PORTION_OUTPUT_DIR_PATH = Path(r"..\Intermediate Results\i2b2 Portion\data\output\i2b2_dump\...\i2b2")
-I2B2_COHORT_IDS_FILE_PATH = Path(r"..\Intermediate Results\i2b2 Portion\data\Cohort IDs.CSV")
-ENCOUNTER_MAP_PATH = Path(r"..\Concatenated Results\data\output\i2b2MakeMap\...\i2b2 Encounter Map.CSV")
-PATIENT_MAP_PATH1 = Path(r"..\Concatenated Results\data\output\i2b2MakeMap\...\i2b2 Patient Map.CSV")  # i2b2 to EPIC Patient ID
-PATIENT_MAP_PATH2 = Path(r"..\Concatenated Results\data\output\i2b2MakeMap\...\i2b2 Patient Map.CSV")  # EPIC Patient ID to Patient Key
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-connection = create_engine(conStr).connect().execution_options(stream_results=True)
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `I2B2_PORTION_OUTPUT_DIR_PATH`: "{I2B2_PORTION_OUTPUT_DIR_PATH}"
-    `I2B2_COHORT_IDS_FILE_PATH`: "{I2B2_COHORT_IDS_FILE_PATH}"
-    `ENCOUNTER_MAP_PATH`: "{ENCOUNTER_MAP_PATH}"
-    `PATIENT_MAP_PATH1`: "{PATIENT_MAP_PATH1}"
-    `PATIENT_MAP_PATH2`: "{PATIENT_MAP_PATH2}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Load maps
-    logger.info("""Loading maps.""")
-    encounterMap = pd.read_csv(ENCOUNTER_MAP_PATH)
-
-    # Get un-linked patients and drop them.
-    cohortIDs = pd.read_csv(I2B2_COHORT_IDS_FILE_PATH)
-    unlinkedPatientsMask = cohortIDs["Patient Key"].isna()
-    unlinkedPatients = cohortIDs["I2B2_PATIENT_NUM"][unlinkedPatientsMask]
-
-    TARGET_ID_NAME = "Patient Key"
-
-    colnamedict = {"ENCOUNTER_NUM": encounterMap.columns[1],
-                   "PATIENT_NUM": TARGET_ID_NAME}
-
-    # Convert maps to dictionaries
-    logger.info("""Converting maps to dictionaries.""")
-    encounterDict = {k: v for k, v in zip(encounterMap.iloc[:, 0], encounterMap.iloc[:, 1])}
-    encounterDict[""] = ""
-    patientDict3 = {k: v for k, v in zip(cohortIDs["I2B2_PATIENT_NUM"], cohortIDs[TARGET_ID_NAME])}
-
-    # Convert i2b2 IDs
-    logger.info("""Converting i2b2 IDs.""")
-    MESSAGE_MODULO = 50
-    for fpath in I2B2_PORTION_OUTPUT_DIR_PATH.iterdir():
-        logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
-        if fpath.suffix.lower() == ".csv":
-            numChunks = 0
-            CHUNKSIZE = 10000
-            for _ in pd.read_csv(fpath, chunksize=CHUNKSIZE):
-                numChunks += 1
-            # Logger block
-            if numChunks < MESSAGE_MODULO:
-                numChunksTenth = numChunks
-            else:
-                numChunksTenth = round(numChunks / MESSAGE_MODULO)
-
-            # Iterate over file chunks
-            header = True
-            mode = "w"
-            savepath = runOutputDir.joinpath(fpath.name)
-            for it, chunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE), start=1):
-                if it % numChunksTenth == 0:
-                    logger.info(f"""    Working on chunk {it} of {numChunks}.""")
-                chunk = pd.DataFrame(chunk)
-                newChunk = chunk.copy()
-
-                # Drop un-linked patients
-                mdrop = newChunk["PATIENT_NUM"].isin(unlinkedPatients)
-                newChunk = newChunk[~mdrop]
-
-                # Convert patient IDs
-                if "PATIENT_NUM" in chunk.columns:
-                    newChunk["PATIENT_NUM"] = newChunk["PATIENT_NUM"].apply(lambda i2b2ID: patientDict3[i2b2ID])
-                    newChunk = newChunk.rename(columns={"PATIENT_NUM": colnamedict["PATIENT_NUM"]})
-
-                # Convert encounter IDs
-                if "ENCOUNTER_NUM" in chunk.columns:
-                    newChunk = newChunk.copy()
-                    mask = newChunk["ENCOUNTER_NUM"] < 0
-                    newChunk.loc[mask, "ENCOUNTER_NUM"] = ""
-                    newChunk["ENCOUNTER_NUM"] = newChunk["ENCOUNTER_NUM"].apply(lambda i2b2ID: encounterDict[i2b2ID])
-                    newChunk = newChunk.rename(columns={"ENCOUNTER_NUM": colnamedict["ENCOUNTER_NUM"]})
-
-                # Save converted chunk
-                newChunk.to_csv(savepath, header=header, mode=mode, index=False)
-                header = False
-                mode = "a"
-        else:
-            pass
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Converts i2b2 `PATIENT_NUM` and `ENCOUNTER_NUM` IDs to "Patient Key" and "Encounter # (CSN)", respectively.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from sqlalchemy import create_engine
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+I2B2_PORTION_OUTPUT_DIR_PATH = Path(r"..\Intermediate Results\i2b2 Portion\data\output\i2b2_dump\...\i2b2")
+I2B2_COHORT_IDS_FILE_PATH = Path(r"..\Intermediate Results\i2b2 Portion\data\Cohort IDs.CSV")
+ENCOUNTER_MAP_PATH = Path(r"..\Concatenated Results\data\output\i2b2MakeMap\...\i2b2 Encounter Map.CSV")
+PATIENT_MAP_PATH1 = Path(r"..\Concatenated Results\data\output\i2b2MakeMap\...\i2b2 Patient Map.CSV")  # i2b2 to EPIC Patient ID
+PATIENT_MAP_PATH2 = Path(r"..\Concatenated Results\data\output\i2b2MakeMap\...\i2b2 Patient Map.CSV")  # EPIC Patient ID to Patient Key
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+connection = create_engine(conStr).connect().execution_options(stream_results=True)
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `I2B2_PORTION_OUTPUT_DIR_PATH`: "{I2B2_PORTION_OUTPUT_DIR_PATH}"
+    `I2B2_COHORT_IDS_FILE_PATH`: "{I2B2_COHORT_IDS_FILE_PATH}"
+    `ENCOUNTER_MAP_PATH`: "{ENCOUNTER_MAP_PATH}"
+    `PATIENT_MAP_PATH1`: "{PATIENT_MAP_PATH1}"
+    `PATIENT_MAP_PATH2`: "{PATIENT_MAP_PATH2}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Load maps
+    logger.info("""Loading maps.""")
+    encounterMap = pd.read_csv(ENCOUNTER_MAP_PATH)
+
+    # Get un-linked patients and drop them.
+    cohortIDs = pd.read_csv(I2B2_COHORT_IDS_FILE_PATH)
+    unlinkedPatientsMask = cohortIDs["Patient Key"].isna()
+    unlinkedPatients = cohortIDs["I2B2_PATIENT_NUM"][unlinkedPatientsMask]
+
+    TARGET_ID_NAME = "Patient Key"
+
+    colnamedict = {"ENCOUNTER_NUM": encounterMap.columns[1],
+                   "PATIENT_NUM": TARGET_ID_NAME}
+
+    # Convert maps to dictionaries
+    logger.info("""Converting maps to dictionaries.""")
+    encounterDict = {k: v for k, v in zip(encounterMap.iloc[:, 0], encounterMap.iloc[:, 1])}
+    encounterDict[""] = ""
+    patientDict3 = {k: v for k, v in zip(cohortIDs["I2B2_PATIENT_NUM"], cohortIDs[TARGET_ID_NAME])}
+
+    # Convert i2b2 IDs
+    logger.info("""Converting i2b2 IDs.""")
+    MESSAGE_MODULO = 50
+    for fpath in I2B2_PORTION_OUTPUT_DIR_PATH.iterdir():
+        logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+        if fpath.suffix.lower() == ".csv":
+            numChunks = 0
+            CHUNKSIZE = 10000
+            for _ in pd.read_csv(fpath, chunksize=CHUNKSIZE):
+                numChunks += 1
+            # Logger block
+            if numChunks < MESSAGE_MODULO:
+                numChunksTenth = numChunks
+            else:
+                numChunksTenth = round(numChunks / MESSAGE_MODULO)
+
+            # Iterate over file chunks
+            header = True
+            mode = "w"
+            savepath = runOutputDir.joinpath(fpath.name)
+            for it, chunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE), start=1):
+                if it % numChunksTenth == 0:
+                    logger.info(f"""    Working on chunk {it} of {numChunks}.""")
+                chunk = pd.DataFrame(chunk)
+                newChunk = chunk.copy()
+
+                # Drop un-linked patients
+                mdrop = newChunk["PATIENT_NUM"].isin(unlinkedPatients)
+                newChunk = newChunk[~mdrop]
+
+                # Convert patient IDs
+                if "PATIENT_NUM" in chunk.columns:
+                    newChunk["PATIENT_NUM"] = newChunk["PATIENT_NUM"].apply(lambda i2b2ID: patientDict3[i2b2ID])
+                    newChunk = newChunk.rename(columns={"PATIENT_NUM": colnamedict["PATIENT_NUM"]})
+
+                # Convert encounter IDs
+                if "ENCOUNTER_NUM" in chunk.columns:
+                    newChunk = newChunk.copy()
+                    mask = newChunk["ENCOUNTER_NUM"] < 0
+                    newChunk.loc[mask, "ENCOUNTER_NUM"] = ""
+                    newChunk["ENCOUNTER_NUM"] = newChunk["ENCOUNTER_NUM"].apply(lambda i2b2ID: encounterDict[i2b2ID])
+                    newChunk = newChunk.rename(columns={"ENCOUNTER_NUM": colnamedict["ENCOUNTER_NUM"]})
+
+                # Save converted chunk
+                newChunk.to_csv(savepath, header=header, mode=mode, index=False)
+                header = False
+                mode = "a"
+        else:
+            pass
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-"""
-Collects i2b2 `PATIENT_NUM` and `ENCOUNTER_NUM` values.
-
-NOTE This is not needed if you use the output from i2b2_dump.get_IDs().
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from sqlalchemy import create_engine
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-I2B2_PORTION_OUTPUT_DIR_PATH = Path(r"..\Intermediate Results\i2b2 Portion\data\output\i2b2_dump\2023-11-20 20-35-58\i2b2")
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-connection = create_engine(conStr).connect().execution_options(stream_results=True)
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `I2B2_PORTION_OUTPUT_DIR_PATH`: "{I2B2_PORTION_OUTPUT_DIR_PATH}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Get set of all patient and encounter IDs
-    logger.info("Getting the set of all patient and encounter IDs.")
-    patientpath = runOutputDir.joinpath("Sets", "PATIENT_NUM.CSV")
-    encounterpath = runOutputDir.joinpath("Sets", "ENCOUNTER_NUM.CSV")
-    makeDirPath(patientpath.parent)
-    makeDirPath(encounterpath.parent)
-    patientmode = "w"
-    encountermode = "w"
-    patientheader = True
-    encounterheader = True
-    MESSAGE_MODULO = 50
-    for fpath in I2B2_PORTION_OUTPUT_DIR_PATH.iterdir():
-        logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
-        if fpath.suffix.lower() == ".csv":
-            numChunks = 0
-            CHUNKSIZE = 10000
-            for _ in pd.read_csv(fpath, chunksize=CHUNKSIZE):
-                numChunks += 1
-            if numChunks < MESSAGE_MODULO:
-                numChunksTenth = numChunks
-            else:
-                numChunksTenth = round(numChunks / MESSAGE_MODULO)
-            for it, chunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE), start=1):
-                if it % numChunksTenth == 0:
-                    logger.info(f"""    Working on chunk {it} of {numChunks}.""")
-                chunk = pd.DataFrame(chunk)
-                if "PATIENT_NUM" in chunk.columns:
-                    patientIDs = chunk["PATIENT_NUM"].drop_duplicates().sort_values()
-                    patientIDs.to_csv(patientpath, mode=patientmode, header=patientheader, index=False)
-                    patientmode = "a"
-                    patientheader = False
-                if "ENCOUNTER_NUM" in chunk.columns:
-                    encounterIDs = chunk["ENCOUNTER_NUM"].drop_duplicates().sort_values()
-                    encounterIDs.to_csv(encounterpath, mode=encountermode, header=encounterheader, index=False)
-                    encountermode = "a"
-                    encounterheader = False
-        else:
-            pass
-
-    # Save sorted, unique IDs, and drop negative encounter IDs
-    # Note that in i2b2, negative encounter IDs are actually negative patient IDs.
-    logger.info("Saving sorted, unique IDs - patients.")
-    patientset = pd.read_csv(patientpath)["PATIENT_NUM"].drop_duplicates().dropna().sort_values()
-    logger.info("Saving sorted, unique IDs - patients - done.")
-
-    logger.info("Saving sorted, unique IDs - encounters.")
-    encounterset = pd.read_csv(encounterpath)["ENCOUNTER_NUM"].drop_duplicates().dropna().sort_values()
-    logger.info("Saving sorted, unique IDs - encounters - done.")
-    mask = encounterset > 0
-    encounterset = encounterset[mask]
-
-    patientset.to_csv(patientpath, index=False)
-    encounterset.to_csv(encounterpath, index=False)
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Collects i2b2 `PATIENT_NUM` and `ENCOUNTER_NUM` values.
+
+NOTE This is not needed if you use the output from i2b2_dump.get_IDs().
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from sqlalchemy import create_engine
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+I2B2_PORTION_OUTPUT_DIR_PATH = Path(r"..\Intermediate Results\i2b2 Portion\data\output\i2b2_dump\2023-11-20 20-35-58\i2b2")
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+connection = create_engine(conStr).connect().execution_options(stream_results=True)
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `I2B2_PORTION_OUTPUT_DIR_PATH`: "{I2B2_PORTION_OUTPUT_DIR_PATH}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Get set of all patient and encounter IDs
+    logger.info("Getting the set of all patient and encounter IDs.")
+    patientpath = runOutputDir.joinpath("Sets", "PATIENT_NUM.CSV")
+    encounterpath = runOutputDir.joinpath("Sets", "ENCOUNTER_NUM.CSV")
+    makeDirPath(patientpath.parent)
+    makeDirPath(encounterpath.parent)
+    patientmode = "w"
+    encountermode = "w"
+    patientheader = True
+    encounterheader = True
+    MESSAGE_MODULO = 50
+    for fpath in I2B2_PORTION_OUTPUT_DIR_PATH.iterdir():
+        logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+        if fpath.suffix.lower() == ".csv":
+            numChunks = 0
+            CHUNKSIZE = 10000
+            for _ in pd.read_csv(fpath, chunksize=CHUNKSIZE):
+                numChunks += 1
+            if numChunks < MESSAGE_MODULO:
+                numChunksTenth = numChunks
+            else:
+                numChunksTenth = round(numChunks / MESSAGE_MODULO)
+            for it, chunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE), start=1):
+                if it % numChunksTenth == 0:
+                    logger.info(f"""    Working on chunk {it} of {numChunks}.""")
+                chunk = pd.DataFrame(chunk)
+                if "PATIENT_NUM" in chunk.columns:
+                    patientIDs = chunk["PATIENT_NUM"].drop_duplicates().sort_values()
+                    patientIDs.to_csv(patientpath, mode=patientmode, header=patientheader, index=False)
+                    patientmode = "a"
+                    patientheader = False
+                if "ENCOUNTER_NUM" in chunk.columns:
+                    encounterIDs = chunk["ENCOUNTER_NUM"].drop_duplicates().sort_values()
+                    encounterIDs.to_csv(encounterpath, mode=encountermode, header=encounterheader, index=False)
+                    encountermode = "a"
+                    encounterheader = False
+        else:
+            pass
+
+    # Save sorted, unique IDs, and drop negative encounter IDs
+    # Note that in i2b2, negative encounter IDs are actually negative patient IDs.
+    logger.info("Saving sorted, unique IDs - patients.")
+    patientset = pd.read_csv(patientpath)["PATIENT_NUM"].drop_duplicates().dropna().sort_values()
+    logger.info("Saving sorted, unique IDs - patients - done.")
+
+    logger.info("Saving sorted, unique IDs - encounters.")
+    encounterset = pd.read_csv(encounterpath)["ENCOUNTER_NUM"].drop_duplicates().dropna().sort_values()
+    logger.info("Saving sorted, unique IDs - encounters - done.")
+    mask = encounterset > 0
+    encounterset = encounterset[mask]
+
+    patientset.to_csv(patientpath, index=False)
+    encounterset.to_csv(encounterpath, index=False)
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-"""
-Concatenates files to create i2b2 `PATIENT_NUM` and `ENCOUNTER_NUM` maps.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from sqlalchemy import create_engine
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-ENCOUNTER_MAP_DIR_PATH = Path(r"..\Intermediate Results\BO Data Portion\data\output\getData\2023-11-27 16-30-11")
-PATIENT_MAP_DIR_PATH = Path(r"..\Intermediate Results\BO Data Portion\data\output\getData\2023-11-27 16-45-28")
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-connection = create_engine(conStr).connect().execution_options(stream_results=True)
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `ENCOUNTER_MAP_DIR_PATH`: "{ENCOUNTER_MAP_DIR_PATH}"
-    `PATIENT_MAP_DIR_PATH`: "{PATIENT_MAP_DIR_PATH}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Load encounter map
-    encounterMap = pd.DataFrame()
-    for fpath in ENCOUNTER_MAP_DIR_PATH.iterdir():
-        if fpath.suffix.lower() == ".csv":
-            df = pd.read_csv(fpath)
-            encounterMap = pd.concat([encounterMap, df])
-        else:
-            pass
-
-    # Load patient map
-    patientMap = pd.DataFrame()
-    for fpath in PATIENT_MAP_DIR_PATH.iterdir():
-        if fpath.suffix.lower() == ".csv":
-            df = pd.read_csv(fpath)
-            patientMap = pd.concat([patientMap, df])
-        else:
-            pass
-
-    # QA
-    n1 = len(encounterMap)
-    n2 = len(patientMap)
-    nu1 = len(encounterMap.iloc[:, 0].unique())
-    nu2 = len(encounterMap.iloc[:, 1].unique())
-    nu3 = len(patientMap.iloc[:, 0].unique())
-    nu4 = len(patientMap.iloc[:, 1].unique())
-
-    logger.info(f"""QA statistics:
-encounter map length:           {n1:,}
-num unique i2b2 encounter IDs:  {nu1:,}
-num unique other encounter IDs: {nu2:,}
-patient map length:             {n2:,}
-num unique i2b2 patient IDs:    {nu3:,}
-num unique other patient IDs:   {nu4:,}.""")
-
-    # Save maps
-    encounterpath = runOutputDir.joinpath("i2b2 Encounter Map.CSV")
-    patientpath = runOutputDir.joinpath("i2b2 Patient Map.CSV")
-
-    encounterMap.to_csv(encounterpath, index=False)
-    patientMap.to_csv(patientpath, index=False)
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Concatenates files to create i2b2 `PATIENT_NUM` and `ENCOUNTER_NUM` maps.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from sqlalchemy import create_engine
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+ENCOUNTER_MAP_DIR_PATH = Path(r"..\Intermediate Results\BO Data Portion\data\output\getData\2023-11-27 16-30-11")
+PATIENT_MAP_DIR_PATH = Path(r"..\Intermediate Results\BO Data Portion\data\output\getData\2023-11-27 16-45-28")
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+connection = create_engine(conStr).connect().execution_options(stream_results=True)
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `ENCOUNTER_MAP_DIR_PATH`: "{ENCOUNTER_MAP_DIR_PATH}"
+    `PATIENT_MAP_DIR_PATH`: "{PATIENT_MAP_DIR_PATH}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Load encounter map
+    encounterMap = pd.DataFrame()
+    for fpath in ENCOUNTER_MAP_DIR_PATH.iterdir():
+        if fpath.suffix.lower() == ".csv":
+            df = pd.read_csv(fpath)
+            encounterMap = pd.concat([encounterMap, df])
+        else:
+            pass
+
+    # Load patient map
+    patientMap = pd.DataFrame()
+    for fpath in PATIENT_MAP_DIR_PATH.iterdir():
+        if fpath.suffix.lower() == ".csv":
+            df = pd.read_csv(fpath)
+            patientMap = pd.concat([patientMap, df])
+        else:
+            pass
+
+    # QA
+    n1 = len(encounterMap)
+    n2 = len(patientMap)
+    nu1 = len(encounterMap.iloc[:, 0].unique())
+    nu2 = len(encounterMap.iloc[:, 1].unique())
+    nu3 = len(patientMap.iloc[:, 0].unique())
+    nu4 = len(patientMap.iloc[:, 1].unique())
+
+    logger.info(f"""QA statistics:
+encounter map length:           {n1:,}
+num unique i2b2 encounter IDs:  {nu1:,}
+num unique other encounter IDs: {nu2:,}
+patient map length:             {n2:,}
+num unique i2b2 patient IDs:    {nu3:,}
+num unique other patient IDs:   {nu4:,}.""")
+
+    # Save maps
+    encounterpath = runOutputDir.joinpath("i2b2 Encounter Map.CSV")
+    patientpath = runOutputDir.joinpath("i2b2 Patient Map.CSV")
+
+    encounterMap.to_csv(encounterpath, index=False)
+    patientMap.to_csv(patientpath, index=False)
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-"""
-Creates an age de-identification map. This is an object that identifies patients who are aged 90 or more at the time of processing (i.e., now, when the script is run).
-
-This is usually run before `deIdentifyByAge`.
-
-Optionally this also creates a second map using a second set of ID's, which is usually necessary if you are operating on a data set that has already had its IDs de-identified. This optional function uses the following parameters:
-
-    - `SECONDARY_MAP`
-    - `SECONDARY_MAP_COLUMN_NAME_FROM`
-    - `SECONDARY_MAP_COLUMN_NAME_TO`
-
-Note that there must be a variable (column) in common between the tables `SECONDARY_MAP` and `INPUT_FILE`, for the patients to be correctly mapped from one table to the other.
-"""
-
-import logging
-import os
-from datetime import datetime as dt
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-INPUT_FILE = Path(r"..\Concatenated Results\data\output\convertColumns\...\person.csv")
-PATIENT_ID_NAME = "Patient Key"
-DATE_OF_BIRTH_COLUMN = "birth_datetime"
-AGE_THRESHOLD = 90
-
-SECONDARY_MAP = Path(r"..\Concatenated Results\data\output\concatenateMaps\...\Patient Key map.csv")  # Path object or `None`
-SECONDARY_MAP_COLUMN_NAME_FROM = "Patient Key"
-SECONDARY_MAP_COLUMN_NAME_TO = "De-identified Patient Key"
-
-# Arguments; General
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 1
-IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `INPUT_FILE`: "{INPUT_FILE}"
-    `PATIENT_ID_NAME`: "{PATIENT_ID_NAME}"
-    `DATE_OF_BIRTH_COLUMN`: "{DATE_OF_BIRTH_COLUMN}"
-    `AGE_THRESHOLD`: "{AGE_THRESHOLD}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    logger.info(f"""Working on file "{INPUT_FILE.absolute().relative_to(rootDirectory)}".""")
-    # Set file options
-    exportPath = runIntermediateDataDir.joinpath(INPUT_FILE.name)
-    fileMode = "w"
-    fileHeaders = True
-    # Read file
-    logger.info("""    Reading file to count the number of chunks.""")
-    numChunks = sum([1 for _ in pd.read_csv(INPUT_FILE, chunksize=CHUNK_SIZE)])
-    logger.info(f"""    This file has {numChunks} chunks.""")
-    dfChunks = pd.read_csv(INPUT_FILE, chunksize=CHUNK_SIZE)
-    for it, dfChunk in enumerate(dfChunks, start=1):
-        dfChunk = pd.DataFrame(dfChunk)
-        # Work on chunk
-        logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-        dfChunk = dfChunk[[PATIENT_ID_NAME, DATE_OF_BIRTH_COLUMN]]
-        dfChunk = dfChunk.drop_duplicates()
-        dfChunk = dfChunk.set_index(PATIENT_ID_NAME)
-        series = dfChunk[DATE_OF_BIRTH_COLUMN]
-        series = pd.to_datetime(series)
-        currentAge = dt.today() - series
-        currentAge = currentAge.apply(lambda timeDelta: timeDelta.days / 365.25)
-        dfChunk["Over Age Threshold"] = currentAge >= AGE_THRESHOLD
-        dfChunk["Over Age Threshold"] = dfChunk["Over Age Threshold"].apply(lambda boolean: 1 if boolean else 0)
-
-        # Save chunk
-        dfChunk["Over Age Threshold"].to_csv(exportPath, mode=fileMode, header=fileHeaders, index=True)
-        fileMode = "a"
-        fileHeaders = False
-        logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-
-    # Sort and remove duplicates from map
-    logger.info("Sorting and removing duplicates from map.")
-    df1 = pd.read_csv(exportPath)
-    df1 = df1.drop_duplicates()
-    df1 = df1.sort_values(by=[PATIENT_ID_NAME, "Over Age Threshold"])
-    logger.info("Sorting and removing duplicates from map - done.")
-    savePath1 = runOutputDir.joinpath(f"Age Map - {PATIENT_ID_NAME}.CSV")
-    metadataText = f"""# Map generation parameters: `AGE_THRESHOLD`: "{AGE_THRESHOLD}".
-# Map generation parameters: `PATIENT_ID_NAME`: "{PATIENT_ID_NAME}".
-# Map generation parameters: `DATE_OF_BIRTH_COLUMN`: "{DATE_OF_BIRTH_COLUMN}".
-"""
-    with open(savePath1, "w") as file:
-        file.write(metadataText)
-    df1.to_csv(savePath1, index=False, mode="a")
-
-    # Create a map using a secondary map
-    if SECONDARY_MAP:
-        df1 = df1.set_index(PATIENT_ID_NAME)
-        df2 = pd.read_csv(SECONDARY_MAP)
-        df2 = df2.set_index(SECONDARY_MAP_COLUMN_NAME_FROM)
-        newMap = df1.join(other=df2[SECONDARY_MAP_COLUMN_NAME_TO],
-                          how="inner")
-        newMap = newMap[[SECONDARY_MAP_COLUMN_NAME_TO, "Over Age Threshold"]]
-        savePath2 = runOutputDir.joinpath(f"Age Map - {SECONDARY_MAP_COLUMN_NAME_TO}.CSV")
-        with open(savePath2, "w") as file:
-            file.write(metadataText)
-        newMap.to_csv(savePath2, index=False, mode="a")
-    else:
-        pass
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+Creates an age de-identification map. This is an object that identifies patients who are aged 90 or more at the time of processing (i.e., now, when the script is run).
+
+This is usually run before `deIdentifyByAge`.
+
+Optionally this also creates a second map using a second set of ID's, which is usually necessary if you are operating on a data set that has already had its IDs de-identified. This optional function uses the following parameters:
+
+    - `SECONDARY_MAP`
+    - `SECONDARY_MAP_COLUMN_NAME_FROM`
+    - `SECONDARY_MAP_COLUMN_NAME_TO`
+
+Note that there must be a variable (column) in common between the tables `SECONDARY_MAP` and `INPUT_FILE`, for the patients to be correctly mapped from one table to the other.
+"""
+
+import logging
+import os
+from datetime import datetime as dt
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+INPUT_FILE = Path(r"..\Concatenated Results\data\output\convertColumns\...\person.csv")
+PATIENT_ID_NAME = "Patient Key"
+DATE_OF_BIRTH_COLUMN = "birth_datetime"
+AGE_THRESHOLD = 90
+
+SECONDARY_MAP = Path(r"..\Concatenated Results\data\output\concatenateMaps\...\Patient Key map.csv")  # Path object or `None`
+SECONDARY_MAP_COLUMN_NAME_FROM = "Patient Key"
+SECONDARY_MAP_COLUMN_NAME_TO = "De-identified Patient Key"
+
+# Arguments; General
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 1
+IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `INPUT_FILE`: "{INPUT_FILE}"
+    `PATIENT_ID_NAME`: "{PATIENT_ID_NAME}"
+    `DATE_OF_BIRTH_COLUMN`: "{DATE_OF_BIRTH_COLUMN}"
+    `AGE_THRESHOLD`: "{AGE_THRESHOLD}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    logger.info(f"""Working on file "{INPUT_FILE.absolute().relative_to(rootDirectory)}".""")
+    # Set file options
+    exportPath = runIntermediateDataDir.joinpath(INPUT_FILE.name)
+    fileMode = "w"
+    fileHeaders = True
+    # Read file
+    logger.info("""    Reading file to count the number of chunks.""")
+    numChunks = sum([1 for _ in pd.read_csv(INPUT_FILE, chunksize=CHUNK_SIZE)])
+    logger.info(f"""    This file has {numChunks} chunks.""")
+    dfChunks = pd.read_csv(INPUT_FILE, chunksize=CHUNK_SIZE)
+    for it, dfChunk in enumerate(dfChunks, start=1):
+        dfChunk = pd.DataFrame(dfChunk)
+        # Work on chunk
+        logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+        dfChunk = dfChunk[[PATIENT_ID_NAME, DATE_OF_BIRTH_COLUMN]]
+        dfChunk = dfChunk.drop_duplicates()
+        dfChunk = dfChunk.set_index(PATIENT_ID_NAME)
+        series = dfChunk[DATE_OF_BIRTH_COLUMN]
+        series = pd.to_datetime(series)
+        currentAge = dt.today() - series
+        currentAge = currentAge.apply(lambda timeDelta: timeDelta.days / 365.25)
+        dfChunk["Over Age Threshold"] = currentAge >= AGE_THRESHOLD
+        dfChunk["Over Age Threshold"] = dfChunk["Over Age Threshold"].apply(lambda boolean: 1 if boolean else 0)
+
+        # Save chunk
+        dfChunk["Over Age Threshold"].to_csv(exportPath, mode=fileMode, header=fileHeaders, index=True)
+        fileMode = "a"
+        fileHeaders = False
+        logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
+
+    # Sort and remove duplicates from map
+    logger.info("Sorting and removing duplicates from map.")
+    df1 = pd.read_csv(exportPath)
+    df1 = df1.drop_duplicates()
+    df1 = df1.sort_values(by=[PATIENT_ID_NAME, "Over Age Threshold"])
+    logger.info("Sorting and removing duplicates from map - done.")
+    savePath1 = runOutputDir.joinpath(f"Age Map - {PATIENT_ID_NAME}.CSV")
+    metadataText = f"""# Map generation parameters: `AGE_THRESHOLD`: "{AGE_THRESHOLD}".
+# Map generation parameters: `PATIENT_ID_NAME`: "{PATIENT_ID_NAME}".
+# Map generation parameters: `DATE_OF_BIRTH_COLUMN`: "{DATE_OF_BIRTH_COLUMN}".
+"""
+    with open(savePath1, "w") as file:
+        file.write(metadataText)
+    df1.to_csv(savePath1, index=False, mode="a")
+
+    # Create a map using a secondary map
+    if SECONDARY_MAP:
+        df1 = df1.set_index(PATIENT_ID_NAME)
+        df2 = pd.read_csv(SECONDARY_MAP)
+        df2 = df2.set_index(SECONDARY_MAP_COLUMN_NAME_FROM)
+        newMap = df1.join(other=df2[SECONDARY_MAP_COLUMN_NAME_TO],
+                          how="inner")
+        newMap = newMap[[SECONDARY_MAP_COLUMN_NAME_TO, "Over Age Threshold"]]
+        savePath2 = runOutputDir.joinpath(f"Age Map - {SECONDARY_MAP_COLUMN_NAME_TO}.CSV")
+        with open(savePath2, "w") as file:
+            file.write(metadataText)
+        newMap.to_csv(savePath2, index=False, mode="a")
+    else:
+        pass
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,146 +1,138 @@
-"""
-Shifts the dates in a data set according to the date shift map for a patient.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import numpy as np
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-PATIENT_DE_IDENTIFICATION_MAP_PATH = Path(r"..\Concatenated Results\data\output\concatenateMaps\2023-12-13 11-59-04\Patient Key map.csv")
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    ``: "{"..."}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Load patient de-identification map
-    patientDeIdentificationMap = pd.read_csv(PATIENT_DE_IDENTIFICATION_MAP_PATH)
-
-    # Assign date shift values
-    array = np.random.randint(low=-30,
-                              high=30,
-                              size=len(patientDeIdentificationMap))
-    patientDeIdentificationMap["Date Shift"] = array
-
-    # Save results
-    savepath = runOutputDir.joinpath("Date Shift Map.CSV")
-    patientDeIdentificationMap.to_csv(savepath, index=False)
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+This is a template Python script.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+_ = None
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 3
+IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 1
+IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 4
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    ``: "{"..."}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Script
+    _ = pd
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-"""
-Makes de-identification maps, building on existing maps.
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-# NOTE Expects integer IDs, so no string IDs like Epic Patient IDs.
-"""
-
-import json
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from pandas.errors import EmptyDataError
-# Local packages
-from drapi.code.drapi.drapi import (ditchFloat,
-                                    getTimestamp,
-                                    handleDatetimeForJson,
-                                    makeDirPath,
-                                    makeMap,
-                                    makeSetComplement,
-                                    successiveParents)
-from drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
-                                          VARIABLE_NAME_TO_FILE_NAME_DICT)
-# Local packages: Script parameters: General
-from common import (IRB_NUMBER,
-                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    DATA_TYPES_DICT,
-                    OLD_MAPS_DIR_PATH,
-                    VARIABLE_ALIASES,
-                    VARIABLE_SUFFIXES)
-
-# Arguments
-SETS_PATH = Path(r"..\Concatenated Results\data\output\aliasVariables\...")
-
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in SETS_PATH.iterdir()])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        getIDValuesOutput = SETS_PATH
-    elif operatingSystem == "win32":
-        getIDValuesOutput = SETS_PATH
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Get set of values
-    # NOTE The code that used to be in this section was moved to "getIDValues.py"
-    logging.info(f"""Using the set of new values in the directory "{getIDValuesOutput.absolute().relative_to(rootDirectory)}".""")
-
-    # QA: Make sure all data variables are present in the script parameters.
-    collectedVariables = [FILE_NAME_TO_VARIABLE_NAME_DICT[fname.stem] for fname in getIDValuesOutput.iterdir()]
-    missingDataTypes = []
-    missingVariableSuffixes = []
-    for variableName in collectedVariables:
-        if variableName not in DATA_TYPES_DICT.keys():
-            missingDataTypes.append(variableName)
-        if variableName not in VARIABLE_SUFFIXES.keys():
-            missingVariableSuffixes.append(variableName)
-    if len(missingDataTypes) > 0:
-        text = "\n".join(missingDataTypes)
-        raise Exception(f"""Not all variables have a data type assigned to them:\n{text}""")
-    if len(missingVariableSuffixes) > 0:
-        text = "\n".join(missingVariableSuffixes)
-        raise Exception(f"Not all variables have a de-identification suffix assigned to them:\n{text}")
-
-    # Create reverse-look-up alias map
-    variableAliasesReverse = {}
-    for variableAlias, variableMainName in VARIABLE_ALIASES.items():
-        if variableMainName in variableAliasesReverse.keys():
-            variableAliasesReverse[variableMainName].append(variableAlias)
-        else:
-            variableAliasesReverse[variableMainName] = [variableAlias]
-
-    # Concatenate all old maps
-    oldMaps = {}
-    logging.info("""Concatenating all similar pre-existing maps.""")
-    for variableName in collectedVariables:
-        logging.info(f"""  Working on variable "{variableName}".""")
-        # Get maps explicitely or implicietly referring to this variable name.
-        condition1 = variableName in OLD_MAPS_DIR_PATH.keys()
-        if condition1:
-            variableLookupName = variableName
-            logging.info("""    Variable has pre-existing map(s).""")
-            listOfMapPaths = OLD_MAPS_DIR_PATH[variableLookupName]
-            dfConcat = pd.DataFrame()
-            for mapPath in listOfMapPaths:
-                logging.info(f"""  ..  Reading pre-existing map from "{mapPath.absolute().relative_to(rootDirectory)}".""")
-                df = pd.DataFrame(pd.read_csv(mapPath))
-                dfConcat = pd.concat([dfConcat, df])
-            oldMaps[variableName] = dfConcat
-        if variableName in variableAliasesReverse.keys():
-            for variableAlias in variableAliasesReverse[variableName]:
-                condition2 = variableAlias in OLD_MAPS_DIR_PATH.keys()
-                if condition2:
-                    variableLookupName = variableAlias
-                    logging.info("""    Variable has pre-existing aliased map(s).""")
-                    listOfMapPaths = OLD_MAPS_DIR_PATH[variableLookupName]
-                    dfConcat = pd.DataFrame()
-                    for mapPath in listOfMapPaths:
-                        logging.info(f"""  ..  Reading pre-existing map from "{mapPath}".""")
-                        df = pd.DataFrame(pd.read_csv(mapPath))
-                        dftemp = makeMap(IDset=set(), IDName=variableName, startFrom=0, irbNumber=IRB_NUMBER, suffix="", columnSuffix=variableName, deIdentificationMapStyle="lemur", logger=logging.getLogger())
-                        df.columns = dftemp.columns
-                        dfConcat = pd.concat([dfConcat, df])
-                    if condition1:
-                        df = oldMaps[variableName]
-                        dfConcat = pd.concat([dfConcat, df])
-                        oldMaps[variableName] = dfConcat
-                    else:
-                        oldMaps[variableName] = dfConcat
-        else:
-            condition2 = False
-        if not (condition1 or condition2):
-            logging.info("""    Variable has no pre-existing map.""")
-            oldMaps[variableName] = pd.DataFrame()
-
-    # Get the set difference between all old maps and the set of un-mapped values
-    valuesToMap = {}
-    setsToMapDataDir = runIntermediateDataDir.joinpath("valuesToMap")
-    makeDirPath(setsToMapDataDir)
-    logging.info("""Getting the set difference between all old maps and the set of un-mapped values.""")
-    for variableName in collectedVariables:
-        logging.info(f"""  Working on variable "{variableName}".""")
-        variableDataType = DATA_TYPES_DICT[variableName]
-
-        # Get old set of IDs
-        logging.info("""    Getting the old set of IDs.""")
-        oldMap = oldMaps[variableName]
-        oldMap = pd.DataFrame(oldMap)
-        if len(oldMap) > 0:
-            if variableDataType.lower() == "numeric":
-                oldIDSet = oldMap[variableName]
-                oldIDSet = pd.Series(oldIDSet)
-                oldIDSet = oldIDSet.unique()
-                oldIDSet = set([ditchFloat(el) for el in oldIDSet])  # NOTE: Hack. Convert values to type int or string
-            elif variableDataType.lower() == "string":
-                oldIDSet = oldMap[variableName]
-                oldIDSet = pd.Series(oldIDSet)
-                oldIDSet = oldIDSet.astype(str)
-                oldIDSet = oldIDSet.unique()
-            elif variableDataType.lower() == "numeric_or_string":
-                oldIDSet = oldMap[variableName]
-                oldIDSet = pd.Series(oldIDSet)
-                oldIDSet = oldIDSet.astype(str)
-                oldIDSet = oldIDSet.unique()
-            else:
-                msg = "The table column is expected to have a data type associated with it."
-                logging.error(msg)
-                raise Exception(msg)
-        elif len(oldMap) == 0:
-            oldIDSet = set()
-        logging.info(f"""    The size of this set is {len(oldIDSet):,}.""")
-
-        # Get new set of IDs
-        newSetPath = getIDValuesOutput.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]}.txt")
-        logging.info(f"""    Getting the new set of IDs from "{newSetPath.absolute().relative_to(rootDirectory)}".""")
-        try:
-            setSeries = pd.read_table(newSetPath, header=None)[0]
-            newIDSet = set(setSeries.to_list())
-        except EmptyDataError as err:
-            _ = err
-            newIDSet = set()
-        if variableDataType.lower() == "numeric":
-            newIDSet = set([ditchFloat(el) for el in newIDSet])  # NOTE: Hack. Convert values to type int or string
-        elif variableDataType.lower() == "string":
-            newIDSet = set([str(el) for el in newIDSet])
-        elif variableDataType.lower() == "numeric_or_string":
-            newIDSet = set([str(el) for el in newIDSet])
-        else:
-            msg = "The table column is expected to have a data type associated with it."
-            logging.error(msg)
-            raise Exception(msg)
-        logging.info(f"""    The size of this set is     {len(newIDSet):,}.""")
-
-        # Set difference
-        IDSetDiff = newIDSet.difference(oldIDSet)
-        logging.info(f"""    The set difference size is  {len(IDSetDiff):,}.""")
-        valuesToMap[variableName] = IDSetDiff
-
-        # Save new subset to `setsToMapDataDir`
-        fpath = setsToMapDataDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]}.JSON")
-        with open(fpath, "w") as file:
-            if variableDataType.lower() == "numeric":
-                li = [ditchFloat(IDNumber) for IDNumber in IDSetDiff]  # NOTE: Hack. Convert values to type int or string
-            elif variableDataType.lower() == "string":
-                li = list(IDSetDiff)
-            elif variableDataType.lower() == "numeric_or_string":
-                li = list(IDSetDiff)
-            else:
-                msg = "The table column is expected to have a data type associated with it."
-                logging.error(msg)
-                raise Exception(msg)
-            file.write(json.dumps(li, default=handleDatetimeForJson))
-        if len(IDSetDiff) == 0:
-            series = pd.Series(dtype=int)
-        else:
-            if variableDataType.lower() == "numeric":
-                series = pd.Series(sorted(list(IDSetDiff)))
-            elif variableDataType.lower() == "string":
-                series = pd.Series(sorted([str(el) for el in IDSetDiff]))
-            elif variableDataType.lower() == "numeric_or_string":
-                series = pd.Series(sorted([str(el) for el in IDSetDiff]))
-            else:
-                msg = "The table column is expected to have a data type associated with it."
-                logging.error(msg)
-                raise Exception(msg)
-
-    # Get numbers for new map
-    logging.info("""Getting numbers for new map.""")
-    newNumbersDict = {}
-    for variableName in collectedVariables:
-        oldMap = oldMaps[variableName]
-        if len(oldMap) > 0:
-            oldNumbersSet = set(oldMap.iloc[:, 1].values)
-        elif len(oldMap) == 0:
-            oldNumbersSet = set()
-        # Get quantity of numbers needed for map
-        quantityOfNumbersUnmapped = len(valuesToMap[variableName])
-        # Get new numbers
-        lenOlderNumbersSet = len(oldNumbersSet)
-        if lenOlderNumbersSet == 0:
-            newNumbers = list(range(1, quantityOfNumbersUnmapped + 1))
-        else:
-            newNumbersSet = makeSetComplement(oldNumbersSet, quantityOfNumbersUnmapped)
-            newNumbers = sorted(list(newNumbersSet))
-        newNumbersDict[variableName] = newNumbers
-
-    # Map un-mapped values
-    logging.info("""Mapping un-mapped values.""")
-    for file in setsToMapDataDir.iterdir():
-        variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[file.stem]
-        variableDataType = DATA_TYPES_DICT[variableName]
-        logging.info(f"""  Working on un-mapped values for variable "{variableName}" located at "{file.absolute().relative_to(rootDirectory)}".""")
-        # Map contents
-        values = valuesToMap[variableName]
-        if variableDataType.lower() == "numeric":
-            values = set(int(float(value)) for value in values)  # NOTE: Hack. Convert values to type int or string
-        elif variableDataType.lower() == "string":
-            pass
-        elif variableDataType.lower() == "numeric_or_string":
-            pass
-        else:
-            msg = "The table column is expected to have a data type associated with it."
-            logging.error(msg)
-            raise Exception(msg)
-        numbers = sorted(list(newNumbersDict[variableName]))
-        deIdIDSuffix = VARIABLE_SUFFIXES[variableName]["deIdIDSuffix"]
-        map_ = makeMap(IDset=values,
-                       IDName=variableName,
-                       startFrom=numbers,
-                       irbNumber=IRB_NUMBER,
-                       suffix=deIdIDSuffix,
-                       columnSuffix=variableName,
-                       deIdentificationMapStyle="lemur",
-                       logger=logging.getLogger())
-        # Save map
-        mapPath = runOutputDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]} map.csv")
-        map_.to_csv(mapPath, index=False)
-        logging.info(f"""    De-identification map saved to "{mapPath.absolute().relative_to(rootDirectory)}".""")
-
-    # Clean up
-    # TODO If input directory is empty, delete
-    # TODO Delete intermediate run directory
-
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Makes de-identification maps, building on existing maps.
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+# NOTE Expects integer IDs, so no string IDs like Epic Patient IDs.
+"""
+
+import json
+import logging
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from pandas.errors import EmptyDataError
+# Local packages
+from drapi.code.drapi.drapi import (ditchFloat,
+                                    getTimestamp,
+                                    handleDatetimeForJson,
+                                    makeDirPath,
+                                    makeMap,
+                                    makeSetComplement,
+                                    successiveParents)
+from drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
+                                          VARIABLE_NAME_TO_FILE_NAME_DICT)
+# Local packages: Script parameters: General
+from common import (IRB_NUMBER,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
+                    DATA_TYPES_DICT,
+                    OLD_MAPS_DIR_PATH,
+                    VARIABLE_ALIASES,
+                    VARIABLE_SUFFIXES)
+
+# Arguments
+SETS_PATH = Path(r"..\Concatenated Results\data\output\aliasVariables\...")
+
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in SETS_PATH.iterdir()])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        getIDValuesOutput = SETS_PATH
+    elif operatingSystem == "win32":
+        getIDValuesOutput = SETS_PATH
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # Get set of values
+    # NOTE The code that used to be in this section was moved to "getIDValues.py"
+    logging.info(f"""Using the set of new values in the directory "{getIDValuesOutput.absolute().relative_to(rootDirectory)}".""")
+
+    # QA: Make sure all data variables are present in the script parameters.
+    collectedVariables = [FILE_NAME_TO_VARIABLE_NAME_DICT[fname.stem] for fname in getIDValuesOutput.iterdir()]
+    missingDataTypes = []
+    missingVariableSuffixes = []
+    for variableName in collectedVariables:
+        if variableName not in DATA_TYPES_DICT.keys():
+            missingDataTypes.append(variableName)
+        if variableName not in VARIABLE_SUFFIXES.keys():
+            missingVariableSuffixes.append(variableName)
+    if len(missingDataTypes) > 0:
+        text = "\n".join(missingDataTypes)
+        raise Exception(f"""Not all variables have a data type assigned to them:\n{text}""")
+    if len(missingVariableSuffixes) > 0:
+        text = "\n".join(missingVariableSuffixes)
+        raise Exception(f"Not all variables have a de-identification suffix assigned to them:\n{text}")
+
+    # Create reverse-look-up alias map
+    variableAliasesReverse = {}
+    for variableAlias, variableMainName in VARIABLE_ALIASES.items():
+        if variableMainName in variableAliasesReverse.keys():
+            variableAliasesReverse[variableMainName].append(variableAlias)
+        else:
+            variableAliasesReverse[variableMainName] = [variableAlias]
+
+    # Concatenate all old maps
+    oldMaps = {}
+    logging.info("""Concatenating all similar pre-existing maps.""")
+    for variableName in collectedVariables:
+        logging.info(f"""  Working on variable "{variableName}".""")
+        # Get maps explicitely or implicietly referring to this variable name.
+        condition1 = variableName in OLD_MAPS_DIR_PATH.keys()
+        if condition1:
+            variableLookupName = variableName
+            logging.info("""    Variable has pre-existing map(s).""")
+            listOfMapPaths = OLD_MAPS_DIR_PATH[variableLookupName]
+            dfConcat = pd.DataFrame()
+            for mapPath in listOfMapPaths:
+                logging.info(f"""  ..  Reading pre-existing map from "{mapPath.absolute().relative_to(rootDirectory)}".""")
+                df = pd.DataFrame(pd.read_csv(mapPath))
+                dfConcat = pd.concat([dfConcat, df])
+            oldMaps[variableName] = dfConcat
+        if variableName in variableAliasesReverse.keys():
+            for variableAlias in variableAliasesReverse[variableName]:
+                condition2 = variableAlias in OLD_MAPS_DIR_PATH.keys()
+                if condition2:
+                    variableLookupName = variableAlias
+                    logging.info("""    Variable has pre-existing aliased map(s).""")
+                    listOfMapPaths = OLD_MAPS_DIR_PATH[variableLookupName]
+                    dfConcat = pd.DataFrame()
+                    for mapPath in listOfMapPaths:
+                        logging.info(f"""  ..  Reading pre-existing map from "{mapPath}".""")
+                        df = pd.DataFrame(pd.read_csv(mapPath))
+                        dftemp = makeMap(IDset=set(), IDName=variableName, startFrom=0, irbNumber=IRB_NUMBER, suffix="", columnSuffix=variableName, deIdentificationMapStyle="lemur", logger=logging.getLogger())
+                        df.columns = dftemp.columns
+                        dfConcat = pd.concat([dfConcat, df])
+                    if condition1:
+                        df = oldMaps[variableName]
+                        dfConcat = pd.concat([dfConcat, df])
+                        oldMaps[variableName] = dfConcat
+                    else:
+                        oldMaps[variableName] = dfConcat
+        else:
+            condition2 = False
+        if not (condition1 or condition2):
+            logging.info("""    Variable has no pre-existing map.""")
+            oldMaps[variableName] = pd.DataFrame()
+
+    # Get the set difference between all old maps and the set of un-mapped values
+    valuesToMap = {}
+    setsToMapDataDir = runIntermediateDataDir.joinpath("valuesToMap")
+    makeDirPath(setsToMapDataDir)
+    logging.info("""Getting the set difference between all old maps and the set of un-mapped values.""")
+    for variableName in collectedVariables:
+        logging.info(f"""  Working on variable "{variableName}".""")
+        variableDataType = DATA_TYPES_DICT[variableName]
+
+        # Get old set of IDs
+        logging.info("""    Getting the old set of IDs.""")
+        oldMap = oldMaps[variableName]
+        oldMap = pd.DataFrame(oldMap)
+        if len(oldMap) > 0:
+            if variableDataType.lower() == "numeric":
+                oldIDSet = oldMap[variableName]
+                oldIDSet = pd.Series(oldIDSet)
+                oldIDSet = oldIDSet.unique()
+                oldIDSet = set([ditchFloat(el) for el in oldIDSet])  # NOTE: Hack. Convert values to type int or string
+            elif variableDataType.lower() == "string":
+                oldIDSet = oldMap[variableName]
+                oldIDSet = pd.Series(oldIDSet)
+                oldIDSet = oldIDSet.astype(str)
+                oldIDSet = oldIDSet.unique()
+            elif variableDataType.lower() == "numeric_or_string":
+                oldIDSet = oldMap[variableName]
+                oldIDSet = pd.Series(oldIDSet)
+                oldIDSet = oldIDSet.astype(str)
+                oldIDSet = oldIDSet.unique()
+            else:
+                msg = "The table column is expected to have a data type associated with it."
+                logging.error(msg)
+                raise Exception(msg)
+        elif len(oldMap) == 0:
+            oldIDSet = set()
+        logging.info(f"""    The size of this set is {len(oldIDSet):,}.""")
+
+        # Get new set of IDs
+        newSetPath = getIDValuesOutput.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]}.txt")
+        logging.info(f"""    Getting the new set of IDs from "{newSetPath.absolute().relative_to(rootDirectory)}".""")
+        try:
+            setSeries = pd.read_table(newSetPath, header=None)[0]
+            newIDSet = set(setSeries.to_list())
+        except EmptyDataError as err:
+            _ = err
+            newIDSet = set()
+        if variableDataType.lower() == "numeric":
+            newIDSet = set([ditchFloat(el) for el in newIDSet])  # NOTE: Hack. Convert values to type int or string
+        elif variableDataType.lower() == "string":
+            newIDSet = set([str(el) for el in newIDSet])
+        elif variableDataType.lower() == "numeric_or_string":
+            newIDSet = set([str(el) for el in newIDSet])
+        else:
+            msg = "The table column is expected to have a data type associated with it."
+            logging.error(msg)
+            raise Exception(msg)
+        logging.info(f"""    The size of this set is     {len(newIDSet):,}.""")
+
+        # Set difference
+        IDSetDiff = newIDSet.difference(oldIDSet)
+        logging.info(f"""    The set difference size is  {len(IDSetDiff):,}.""")
+        valuesToMap[variableName] = IDSetDiff
+
+        # Save new subset to `setsToMapDataDir`
+        fpath = setsToMapDataDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]}.JSON")
+        with open(fpath, "w") as file:
+            if variableDataType.lower() == "numeric":
+                li = [ditchFloat(IDNumber) for IDNumber in IDSetDiff]  # NOTE: Hack. Convert values to type int or string
+            elif variableDataType.lower() == "string":
+                li = list(IDSetDiff)
+            elif variableDataType.lower() == "numeric_or_string":
+                li = list(IDSetDiff)
+            else:
+                msg = "The table column is expected to have a data type associated with it."
+                logging.error(msg)
+                raise Exception(msg)
+            file.write(json.dumps(li, default=handleDatetimeForJson))
+        if len(IDSetDiff) == 0:
+            series = pd.Series(dtype=int)
+        else:
+            if variableDataType.lower() == "numeric":
+                series = pd.Series(sorted(list(IDSetDiff)))
+            elif variableDataType.lower() == "string":
+                series = pd.Series(sorted([str(el) for el in IDSetDiff]))
+            elif variableDataType.lower() == "numeric_or_string":
+                series = pd.Series(sorted([str(el) for el in IDSetDiff]))
+            else:
+                msg = "The table column is expected to have a data type associated with it."
+                logging.error(msg)
+                raise Exception(msg)
+
+    # Get numbers for new map
+    logging.info("""Getting numbers for new map.""")
+    newNumbersDict = {}
+    for variableName in collectedVariables:
+        oldMap = oldMaps[variableName]
+        if len(oldMap) > 0:
+            oldNumbersSet = set(oldMap.iloc[:, 1].values)
+        elif len(oldMap) == 0:
+            oldNumbersSet = set()
+        # Get quantity of numbers needed for map
+        quantityOfNumbersUnmapped = len(valuesToMap[variableName])
+        # Get new numbers
+        lenOlderNumbersSet = len(oldNumbersSet)
+        if lenOlderNumbersSet == 0:
+            newNumbers = list(range(1, quantityOfNumbersUnmapped + 1))
+        else:
+            newNumbersSet = makeSetComplement(oldNumbersSet, quantityOfNumbersUnmapped)
+            newNumbers = sorted(list(newNumbersSet))
+        newNumbersDict[variableName] = newNumbers
+
+    # Map un-mapped values
+    logging.info("""Mapping un-mapped values.""")
+    for file in setsToMapDataDir.iterdir():
+        variableName = FILE_NAME_TO_VARIABLE_NAME_DICT[file.stem]
+        variableDataType = DATA_TYPES_DICT[variableName]
+        logging.info(f"""  Working on un-mapped values for variable "{variableName}" located at "{file.absolute().relative_to(rootDirectory)}".""")
+        # Map contents
+        values = valuesToMap[variableName]
+        if variableDataType.lower() == "numeric":
+            values = set(int(float(value)) for value in values)  # NOTE: Hack. Convert values to type int or string
+        elif variableDataType.lower() == "string":
+            pass
+        elif variableDataType.lower() == "numeric_or_string":
+            pass
+        else:
+            msg = "The table column is expected to have a data type associated with it."
+            logging.error(msg)
+            raise Exception(msg)
+        numbers = sorted(list(newNumbersDict[variableName]))
+        deIdIDSuffix = VARIABLE_SUFFIXES[variableName]["deIdIDSuffix"]
+        map_ = makeMap(IDset=values,
+                       IDName=variableName,
+                       startFrom=numbers,
+                       irbNumber=IRB_NUMBER,
+                       suffix=deIdIDSuffix,
+                       columnSuffix=variableName,
+                       deIdentificationMapStyle="lemur",
+                       logger=logging.getLogger())
+        # Save map
+        mapPath = runOutputDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[variableName]} map.csv")
+        map_.to_csv(mapPath, index=False)
+        logging.info(f"""    De-identification map saved to "{mapPath.absolute().relative_to(rootDirectory)}".""")
+
+    # Clean up
+    # TODO If input directory is empty, delete
+    # TODO Delete intermediate run directory
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-"""
-Makes de-identification maps from scratch.
-
-# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
-# TODO Needs to combine similar IDs, like different providers IDs.
-"""
-
-import logging
-import sys
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from pandas.errors import EmptyDataError
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    makeMap,
-                                    successiveParents)
-# Local packages: Script parameters: General
-from common import (IRB_NUMBER,
-                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    VARIABLE_SUFFIXES)
-# Project parameters: Portion paths
-from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
-                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
-                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
-                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
-# Project parameters: File criteria
-from common import (BO_PORTION_FILE_CRITERIA,
-                    I2B2_PORTION_FILE_CRITERIA,
-                    NOTES_PORTION_FILE_CRITERIA,
-                    OMOP_PORTION_FILE_CRITERIA)
-
-# Arguments
-LOG_LEVEL = "DEBUG"
-
-MAC_PATHS = [BO_PORTION_DIR_MAC,
-             I2B2_PORTION_DIR_MAC,
-             NOTES_PORTION_DIR_MAC,
-             OMOP_PORTION_DIR_MAC]
-WIN_PATHS = [BO_PORTION_DIR_WIN,
-             I2B2_PORTION_DIR_WIN,
-             NOTES_PORTION_DIR_WIN,
-             OMOP_PORTION_DIR_WIN]
-
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA,
-                              I2B2_PORTION_FILE_CRITERIA,
-                              NOTES_PORTION_FILE_CRITERIA,
-                              OMOP_PORTION_FILE_CRITERIA]
-
-SETS_PATH = Path(r"..\Concatenated Results\data\output\getIDValues\...\Set Files")
-
-CHUNK_SIZE = 50000
-
-# Arguments: Meta-variables
-CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
-PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
-IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-                                           #  "IRB_DIRECTORY",                   # noqa
-                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
-                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
-    outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-
-# Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
-if isAccessible:
-    # If you have access to either of the below directories, use this block.
-    operatingSystem = sys.platform
-    if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
-    else:
-        raise Exception("Unsupported operating system")
-else:
-    # If the above option doesn't work, manually copy the database to the `input` directory.
-    print("Not implemented. Check settings in your script.")
-    sys.exit()
-
-# Directory creation: General
-makeDirPath(runIntermediateDataDir)
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-if __name__ == "__main__":
-    # Logging block
-    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-    fileHandler = logging.FileHandler(logpath)
-    fileHandler.setLevel(LOG_LEVEL)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(LOG_LEVEL)
-
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler, streamHandler],
-                        level=LOG_LEVEL)
-
-    logging.info(f"""Begin running "{thisFilePath}".""")
-    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-
-    # Get set of values
-    # Imported from "getIDValues.py"
-
-    # Map values
-    for file in SETS_PATH.iterdir():
-        variableName = file.stem
-        logging.info(f"""  Working on variable "{variableName}" located at "{file.absolute().relative_to(rootDirectory)}".""")
-        # Read file
-        try:
-            df = pd.read_table(file, header=None)
-            series = df[0]
-        except EmptyDataError as err:
-            _ = err
-            series = pd.Series()
-        values = set(series.values)
-        # Map contents
-        deIdIDSuffix = VARIABLE_SUFFIXES[variableName]["deIdIDSuffix"]
-        map_ = makeMap(IDset=values, IDName=variableName, startFrom=1, irbNumber=IRB_NUMBER, suffix=deIdIDSuffix, columnSuffix=variableName, logger=logging.getLogger())
-        # Save map
-        mapPath = runOutputDir.joinpath(f"{variableName} map.csv")
-        map_.to_csv(mapPath, index=False)
-        logging.info(f"""    De-identification map saved to "{mapPath.absolute().relative_to(rootDirectory)}".""")
-
-    # Clean up
-    # TODO If input directory is empty, delete
-    # TODO Delete intermediate run directory
-
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Makes de-identification maps from scratch.
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
+# TODO Needs to combine similar IDs, like different providers IDs.
+"""
+
+import logging
+import sys
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from pandas.errors import EmptyDataError
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    makeMap,
+                                    successiveParents)
+# Local packages: Script parameters: General
+from common import (IRB_NUMBER,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
+                    VARIABLE_SUFFIXES)
+# Project parameters: Portion paths
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+# Project parameters: File criteria
+from common import (BO_PORTION_FILE_CRITERIA,
+                    I2B2_PORTION_FILE_CRITERIA,
+                    NOTES_PORTION_FILE_CRITERIA,
+                    OMOP_PORTION_FILE_CRITERIA)
+
+# Arguments
+LOG_LEVEL = "DEBUG"
+
+MAC_PATHS = [BO_PORTION_DIR_MAC,
+             I2B2_PORTION_DIR_MAC,
+             NOTES_PORTION_DIR_MAC,
+             OMOP_PORTION_DIR_MAC]
+WIN_PATHS = [BO_PORTION_DIR_WIN,
+             I2B2_PORTION_DIR_WIN,
+             NOTES_PORTION_DIR_WIN,
+             OMOP_PORTION_DIR_WIN]
+
+LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA,
+                              I2B2_PORTION_FILE_CRITERIA,
+                              NOTES_PORTION_FILE_CRITERIA,
+                              OMOP_PORTION_FILE_CRITERIA]
+
+SETS_PATH = Path(r"..\Concatenated Results\data\output\getIDValues\...\Set Files")
+
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
+    outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Directory creation: General
+makeDirPath(runIntermediateDataDir)
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+if __name__ == "__main__":
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+
+    # Get set of values
+    # Imported from "getIDValues.py"
+
+    # Map values
+    for file in SETS_PATH.iterdir():
+        variableName = file.stem
+        logging.info(f"""  Working on variable "{variableName}" located at "{file.absolute().relative_to(rootDirectory)}".""")
+        # Read file
+        try:
+            df = pd.read_table(file, header=None)
+            series = df[0]
+        except EmptyDataError as err:
+            _ = err
+            series = pd.Series()
+        values = set(series.values)
+        # Map contents
+        deIdIDSuffix = VARIABLE_SUFFIXES[variableName]["deIdIDSuffix"]
+        map_ = makeMap(IDset=values, IDName=variableName, startFrom=1, irbNumber=IRB_NUMBER, suffix=deIdIDSuffix, columnSuffix=variableName, logger=logging.getLogger())
+        # Save map
+        mapPath = runOutputDir.joinpath(f"{variableName} map.csv")
+        map_.to_csv(mapPath, index=False)
+        logging.info(f"""    De-identification map saved to "{mapPath.absolute().relative_to(rootDirectory)}".""")
+
+    # Clean up
+    # TODO If input directory is empty, delete
+    # TODO Delete intermediate run directory
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@REM REMEMBER: Change the following, if applicable:
-@REM 1. `condaEnvPrefix`
-set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
-@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
-@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
-Title My Anaconda IPython Starter
-color 08
-@REM The below command does the following:
-@REM - opens the anaconda environment located at `condaEnvPrefix`
-@REM - clears the screen
-@REM - starts ipython
-cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
+@REM REMEMBER: Change the following, if applicable:
+@REM 1. `condaEnvPrefix`
+set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
+@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
+@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
+Title My Anaconda IPython Starter
+color 08
+@REM The below command does the following:
+@REM - opens the anaconda environment located at `condaEnvPrefix`
+@REM - clears the screen
+@REM - starts ipython
+cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/functions.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/functions.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-"""
-"""
-
-import re
-from logging import Logger
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from sqlalchemy import create_engine
-# Local packages
-from drapi.code.drapi.drapi import (makeChunks,
-                                    replace_sql_query)
-
-
-def getData(queryName: str, querySubName: str, sqlFilePath: Path, cohortData: pd.DataFrame, conStr: str, runOutputDir, queryChunkSize: int, logger: Logger) -> pd.DataFrame:
-    """
-    """
-    connection1 = create_engine(conStr).connect().execution_options(stream_results=True)
-    connection2 = create_engine(conStr).connect().execution_options(stream_results=True)
-
-    # Read query file
-    with open(sqlFilePath, "r") as file:
-        query0 = file.read()
-
-    # Fill out query template
-    logger.info("""  Filling out query template.""")
-
-    query = query0[:]
-
-    # Save query to log
-    logger.log(9, query)
-
-    # Execute query
-    logger.info("""  ..  Executing query.""")
-
-    logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}".""")
-    queryGenerator0 = pd.read_sql(sql=query, con=connection1, chunksize=queryChunkSize)
-    chunks2 = [1 for _ in queryGenerator0]
-    numChunks2 = sum(chunks2)
-    logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}" - Done.""")
-
-    logger.info("""  ..  Creating query generator.""")
-    queryGenerator1 = pd.read_sql(sql=query, con=connection2, chunksize=queryChunkSize)
-    logger.info("""  ..  Creating query generator - Done.""")
-
-    padlen2 = len(str(numChunks2))
-    logger.info("""  ..  Iterating over query generator.""")
-    for it2, queryChunk in enumerate(queryGenerator1, start=1):
-        itstring2 = str(it2).zfill(padlen2)
-        logger.info(f"""  ..  ..  Executing query chunk {itstring2} of {numChunks2}.""")
-        result = queryChunk
-        logger.info("""  ..  ..  Finished query chunk.""")
-
-        logger.info("  ..  ..  Saving chunk.")
-        if len(querySubName) > 0:
-            querySubNamePart = f" - {querySubName}"
-        else:
-            querySubNamePart = querySubName
-        fpath = runOutputDir.joinpath(f"{queryName}{querySubNamePart} - {itstring2} of {numChunks2}.CSV")
-        result.to_csv(fpath, index=False)
-        logger.info("  ..  ..  Saving chunk - done.")
-
-    connection1.close()
-    connection2.close()
-
-
-def getData2(queryName: str, querySubName: str, sqlFilePath: Path, cohortData: pd.DataFrame, conStr: str, runOutputDir, queryChunkSize: int, logger: Logger) -> pd.DataFrame:
-    """
-    """
-    filterChunkSize = 20000
-    connection1 = create_engine(conStr).connect().execution_options(stream_results=True)
-    connection2 = create_engine(conStr).connect().execution_options(stream_results=True)
-
-    # Read query file
-    with open(sqlFilePath, "r") as file:
-        query0 = file.read()
-
-    # Fill out query template
-    logger.info("""  Filling out query template.""")
-
-    IDSeries1 = cohortData["Patient Key"]  # TODO
-    templatePlaceholder1 = "{PYTHON_VARIABLE: PATIENT_KEY}"  # TODO
-    variableDataType1 = "int"  # TODO
-    if variableDataType1 == "int":
-        IDValues1 = IDSeries1.drop_duplicates().dropna().astype("int64").sort_values().values
-    elif variableDataType1 == "varchar":
-        IDValues1 = IDSeries1.drop_duplicates().dropna().sort_values().values
-
-    IDsChunk0 = makeChunks(IDValues1, filterChunkSize)
-    IDsChunk1 = makeChunks(IDValues1, filterChunkSize)
-    numChunks1 = sum([1 for _ in IDsChunk0])
-    padlen1 = len(str(numChunks1))
-    for it1, IDsChunk in enumerate(IDsChunk1, start=1):
-        itstring1 = str(it1).zfill(padlen1)
-        logger.info(f"""    Working on filter chunk {itstring1} of {numChunks1} with `filterChunkSize` "{filterChunkSize:,}".""")
-
-        # Fill query template: lists to strings
-        if variableDataType1 == "int":
-            IDListAsString1 = ",".join([f"{el}" for el in IDsChunk])
-        elif variableDataType1 == "varchar":
-            IDListAsString1 = ",".join([f"'{el}'" for el in IDsChunk])
-
-        query = replace_sql_query(query=query0,
-                                  old="""(( ADMIT_EVENT_Derived.NUM_GRAM_WGHT )/1000)/((( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)*(( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)) as "Admit BMI",""",
-                                  new="""(( ADMIT_EVENT_Derived.NUM_GRAM_WGHT )/1000)/NULLIF(((( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)*(( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)), 0) as "Admit BMI",""")
-        query = replace_sql_query(query=query,
-                                  old=",(cast(wt.last_wt_oz as decimal(10,2))*0.0283495)/((cast(ht.last_ht_in as decimal(10,2))*0.0254)*(cast(ht.last_ht_in as decimal(10,2)))*0.0254) as bmi_manual_calc",
-                                  new=",(cast(wt.last_wt_oz as decimal(10,2))*0.0283495)/NULLIF(((cast(ht.last_ht_in as decimal(10,2))*0.0254)*(cast(ht.last_ht_in as decimal(10,2)))*0.0254), 0) as bmi_manual_calc")
-
-        query = replace_sql_query(query=query,
-                                  old=templatePlaceholder1,
-                                  new=IDListAsString1)
-
-        # Save query to log
-        logger.log(9, query)
-
-        # Execute query
-        logger.info("""  ..  Executing query.""")
-
-        logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}".""")
-        queryGenerator0 = pd.read_sql(sql=query, con=connection1, chunksize=queryChunkSize)
-        chunks2 = [1 for _ in queryGenerator0]
-        numChunks2 = sum(chunks2)
-        logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}" - Done.""")
-
-        logger.info("""  ..  Creating query generator.""")
-        queryGenerator1 = pd.read_sql(sql=query, con=connection2, chunksize=queryChunkSize)
-        logger.info("""  ..  Creating query generator - Done.""")
-
-        padlen2 = len(str(numChunks2))
-        logger.info("""  ..  Iterating over query generator.""")
-        for it2, queryChunk in enumerate(queryGenerator1, start=1):
-            itstring2 = str(it2).zfill(padlen2)
-            logger.info(f"""  ..  ..  Executing query chunk {itstring2} of {numChunks2}.""")
-            result = queryChunk
-            logger.info("""  ..  ..  Finished query chunk.""")
-
-            logger.info("  ..  ..  Saving chunk.")
-            if len(querySubName) > 0:
-                querySubNamePart = f" - {querySubName}"
-            else:
-                querySubNamePart = querySubName
-            fpath = runOutputDir.joinpath(f"{queryName}{querySubNamePart} - {itstring1} of {numChunks1} - {itstring2} of {numChunks2}.CSV")
-            result.to_csv(fpath, index=False)
-            logger.info("  ..  ..  Saving chunk - done.")
-
-    connection1.close()
-    connection2.close()
-
-
-def checkFileConditions(sqlFilePath: Path, cohortData: pd.DataFrame, stepNumberCondition: str, logger: Logger, conStr: str, runOutputDir: Path, getDataFunction: object, queryChunkSize: int):
-    """
-    """
-    logger.info(f"""  Working on file "{sqlFilePath}".""")
-    pattern = r"^(?P<universe>.+?) - (?P<queryName>[^-]+)( - )?(?P<querySubName>[^-]*).SQL$"
-    matchObj = re.match(pattern, sqlFilePath.name)
-    if matchObj:
-        groupdict = matchObj.groupdict()
-        queryName = groupdict["queryName"]
-        querySubName = groupdict["querySubName"]
-        condition1 = sqlFilePath.suffix.lower() == ".sql"
-    else:
-        condition1 = False
-
-    if condition1:
-        logger.info("  Processing file.")
-        getDataFunction(queryName=queryName,
-                        querySubName=querySubName,
-                        sqlFilePath=sqlFilePath,
-                        cohortData=cohortData,
-                        conStr=conStr,
-                        runOutputDir=runOutputDir,
-                        queryChunkSize=queryChunkSize,
-                        logger=logger)
-    else:
-        logger.info("  This file has not met the conditions for processing.")
+"""
+"""
+
+import re
+from logging import Logger
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from sqlalchemy import create_engine
+# Local packages
+from drapi.code.drapi.drapi import (makeChunks,
+                                    replace_sql_query)
+
+
+def getData(queryName: str, querySubName: str, sqlFilePath: Path, cohortData: pd.DataFrame, conStr: str, runOutputDir, queryChunkSize: int, logger: Logger) -> pd.DataFrame:
+    """
+    """
+    connection1 = create_engine(conStr).connect().execution_options(stream_results=True)
+    connection2 = create_engine(conStr).connect().execution_options(stream_results=True)
+
+    # Read query file
+    with open(sqlFilePath, "r") as file:
+        query0 = file.read()
+
+    # Fill out query template
+    logger.info("""  Filling out query template.""")
+
+    query = query0[:]
+
+    # Save query to log
+    logger.log(9, query)
+
+    # Execute query
+    logger.info("""  ..  Executing query.""")
+
+    logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}".""")
+    queryGenerator0 = pd.read_sql(sql=query, con=connection1, chunksize=queryChunkSize)
+    chunks2 = [1 for _ in queryGenerator0]
+    numChunks2 = sum(chunks2)
+    logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}" - Done.""")
+
+    logger.info("""  ..  Creating query generator.""")
+    queryGenerator1 = pd.read_sql(sql=query, con=connection2, chunksize=queryChunkSize)
+    logger.info("""  ..  Creating query generator - Done.""")
+
+    padlen2 = len(str(numChunks2))
+    logger.info("""  ..  Iterating over query generator.""")
+    for it2, queryChunk in enumerate(queryGenerator1, start=1):
+        itstring2 = str(it2).zfill(padlen2)
+        logger.info(f"""  ..  ..  Executing query chunk {itstring2} of {numChunks2}.""")
+        result = queryChunk
+        logger.info("""  ..  ..  Finished query chunk.""")
+
+        logger.info("  ..  ..  Saving chunk.")
+        if len(querySubName) > 0:
+            querySubNamePart = f" - {querySubName}"
+        else:
+            querySubNamePart = querySubName
+        fpath = runOutputDir.joinpath(f"{queryName}{querySubNamePart} - {itstring2} of {numChunks2}.CSV")
+        result.to_csv(fpath, index=False)
+        logger.info("  ..  ..  Saving chunk - done.")
+
+    connection1.close()
+    connection2.close()
+
+
+def getData2(queryName: str, querySubName: str, sqlFilePath: Path, cohortData: pd.DataFrame, conStr: str, runOutputDir, queryChunkSize: int, logger: Logger) -> pd.DataFrame:
+    """
+    """
+    filterChunkSize = 20000
+    connection1 = create_engine(conStr).connect().execution_options(stream_results=True)
+    connection2 = create_engine(conStr).connect().execution_options(stream_results=True)
+
+    # Read query file
+    with open(sqlFilePath, "r") as file:
+        query0 = file.read()
+
+    # Fill out query template
+    logger.info("""  Filling out query template.""")
+
+    IDSeries1 = cohortData["Patient Key"]  # TODO
+    templatePlaceholder1 = "{PYTHON_VARIABLE: PATIENT_KEY}"  # TODO
+    variableDataType1 = "int"  # TODO
+    if variableDataType1 == "int":
+        IDValues1 = IDSeries1.drop_duplicates().dropna().astype("int64").sort_values().values
+    elif variableDataType1 == "varchar":
+        IDValues1 = IDSeries1.drop_duplicates().dropna().sort_values().values
+
+    IDsChunk0 = makeChunks(IDValues1, filterChunkSize)
+    IDsChunk1 = makeChunks(IDValues1, filterChunkSize)
+    numChunks1 = sum([1 for _ in IDsChunk0])
+    padlen1 = len(str(numChunks1))
+    for it1, IDsChunk in enumerate(IDsChunk1, start=1):
+        itstring1 = str(it1).zfill(padlen1)
+        logger.info(f"""    Working on filter chunk {itstring1} of {numChunks1} with `filterChunkSize` "{filterChunkSize:,}".""")
+
+        # Fill query template: lists to strings
+        if variableDataType1 == "int":
+            IDListAsString1 = ",".join([f"{el}" for el in IDsChunk])
+        elif variableDataType1 == "varchar":
+            IDListAsString1 = ",".join([f"'{el}'" for el in IDsChunk])
+
+        query = replace_sql_query(query=query0,
+                                  old="""(( ADMIT_EVENT_Derived.NUM_GRAM_WGHT )/1000)/((( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)*(( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)) as "Admit BMI",""",
+                                  new="""(( ADMIT_EVENT_Derived.NUM_GRAM_WGHT )/1000)/NULLIF(((( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)*(( ADMIT_EVENT_Derived.NUM_CENTMTR_HGHT )/100)), 0) as "Admit BMI",""")
+        query = replace_sql_query(query=query,
+                                  old=",(cast(wt.last_wt_oz as decimal(10,2))*0.0283495)/((cast(ht.last_ht_in as decimal(10,2))*0.0254)*(cast(ht.last_ht_in as decimal(10,2)))*0.0254) as bmi_manual_calc",
+                                  new=",(cast(wt.last_wt_oz as decimal(10,2))*0.0283495)/NULLIF(((cast(ht.last_ht_in as decimal(10,2))*0.0254)*(cast(ht.last_ht_in as decimal(10,2)))*0.0254), 0) as bmi_manual_calc")
+
+        query = replace_sql_query(query=query,
+                                  old=templatePlaceholder1,
+                                  new=IDListAsString1)
+
+        # Save query to log
+        logger.log(9, query)
+
+        # Execute query
+        logger.info("""  ..  Executing query.""")
+
+        logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}".""")
+        queryGenerator0 = pd.read_sql(sql=query, con=connection1, chunksize=queryChunkSize)
+        chunks2 = [1 for _ in queryGenerator0]
+        numChunks2 = sum(chunks2)
+        logger.info(f"""  ..  Counting the number of query result chunks that are expected with `queryChunkSize` "{queryChunkSize:,}" - Done.""")
+
+        logger.info("""  ..  Creating query generator.""")
+        queryGenerator1 = pd.read_sql(sql=query, con=connection2, chunksize=queryChunkSize)
+        logger.info("""  ..  Creating query generator - Done.""")
+
+        padlen2 = len(str(numChunks2))
+        logger.info("""  ..  Iterating over query generator.""")
+        for it2, queryChunk in enumerate(queryGenerator1, start=1):
+            itstring2 = str(it2).zfill(padlen2)
+            logger.info(f"""  ..  ..  Executing query chunk {itstring2} of {numChunks2}.""")
+            result = queryChunk
+            logger.info("""  ..  ..  Finished query chunk.""")
+
+            logger.info("  ..  ..  Saving chunk.")
+            if len(querySubName) > 0:
+                querySubNamePart = f" - {querySubName}"
+            else:
+                querySubNamePart = querySubName
+            fpath = runOutputDir.joinpath(f"{queryName}{querySubNamePart} - {itstring1} of {numChunks1} - {itstring2} of {numChunks2}.CSV")
+            result.to_csv(fpath, index=False)
+            logger.info("  ..  ..  Saving chunk - done.")
+
+    connection1.close()
+    connection2.close()
+
+
+def checkFileConditions(sqlFilePath: Path, cohortData: pd.DataFrame, stepNumberCondition: str, logger: Logger, conStr: str, runOutputDir: Path, getDataFunction: object, queryChunkSize: int):
+    """
+    """
+    logger.info(f"""  Working on file "{sqlFilePath}".""")
+    pattern = r"^(?P<universe>.+?) - (?P<queryName>[^-]+)( - )?(?P<querySubName>[^-]*).SQL$"
+    matchObj = re.match(pattern, sqlFilePath.name)
+    if matchObj:
+        groupdict = matchObj.groupdict()
+        queryName = groupdict["queryName"]
+        querySubName = groupdict["querySubName"]
+        condition1 = sqlFilePath.suffix.lower() == ".sql"
+    else:
+        condition1 = False
+
+    if condition1:
+        logger.info("  Processing file.")
+        getDataFunction(queryName=queryName,
+                        querySubName=querySubName,
+                        sqlFilePath=sqlFilePath,
+                        cohortData=cohortData,
+                        conStr=conStr,
+                        runOutputDir=runOutputDir,
+                        queryChunkSize=queryChunkSize,
+                        logger=logger)
+    else:
+        logger.info("  This file has not met the conditions for processing.")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-"""
-Script template to pull BO data using a query filter.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-from sqlalchemy import create_engine
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-# Super-local imports
-from functions import checkFileConditions, getData, getData2
-
-# Arguments
-LIST_OF_SQL_FILES = []  # TODO
-COHORT_FILE_PATH = ""  # TODO
-USE_QUERY_FILTER = False  # TODO
-
-QUERY_CHUNK_SIZE = 10000
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-connection = create_engine(conStr).connect().execution_options(stream_results=True)
-
-# Variables: Other
-if not USE_QUERY_FILTER:
-    getDataFunction = getData
-else:
-    getDataFunction = getData2
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `LIST_OF_SQL_FILES`: "{LIST_OF_SQL_FILES}"
-    `USE_QUERY_FILTER`: "{USE_QUERY_FILTER}"
-    `COHORT_FILE_PATH`: "{COHORT_FILE_PATH}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Read cohort file
-    logger.info("""Reading cohort file.""")
-    cohortData = pd.read_csv(COHORT_FILE_PATH)
-    logger.info("""Reading cohort file - done.""")
-
-    # Iterate over SQL directory contents
-    logger.info("""Iterating over SQL directory contents.""")
-    sqlFiles = sorted(LIST_OF_SQL_FILES)
-    for sqlFilePath in sqlFiles:
-        checkFileConditions(sqlFilePath=sqlFilePath,
-                            cohortData=cohortData,
-                            stepNumberCondition="NA",
-                            logger=logger,
-                            conStr=conStr,
-                            runOutputDir=runOutputDir,
-                            getDataFunction=getDataFunction,
-                            queryChunkSize=QUERY_CHUNK_SIZE)
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Script template to pull BO data using a query filter.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+from sqlalchemy import create_engine
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+# Super-local imports
+from functions import checkFileConditions, getData, getData2
+
+# Arguments
+LIST_OF_SQL_FILES = []  # TODO
+COHORT_FILE_PATH = ""  # TODO
+USE_QUERY_FILTER = False  # TODO
+
+QUERY_CHUNK_SIZE = 10000
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+connection = create_engine(conStr).connect().execution_options(stream_results=True)
+
+# Variables: Other
+if not USE_QUERY_FILTER:
+    getDataFunction = getData
+else:
+    getDataFunction = getData2
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `LIST_OF_SQL_FILES`: "{LIST_OF_SQL_FILES}"
+    `USE_QUERY_FILTER`: "{USE_QUERY_FILTER}"
+    `COHORT_FILE_PATH`: "{COHORT_FILE_PATH}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Read cohort file
+    logger.info("""Reading cohort file.""")
+    cohortData = pd.read_csv(COHORT_FILE_PATH)
+    logger.info("""Reading cohort file - done.""")
+
+    # Iterate over SQL directory contents
+    logger.info("""Iterating over SQL directory contents.""")
+    sqlFiles = sorted(LIST_OF_SQL_FILES)
+    for sqlFilePath in sqlFiles:
+        checkFileConditions(sqlFilePath=sqlFilePath,
+                            cohortData=cohortData,
+                            stepNumberCondition="NA",
+                            logger=logger,
+                            conStr=conStr,
+                            runOutputDir=runOutputDir,
+                            getDataFunction=getDataFunction,
+                            queryChunkSize=QUERY_CHUNK_SIZE)
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@REM REMEMBER: Change the following, if applicable:
-@REM 1. `condaEnvPrefix`
-set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
-@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
-@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
-Title My Anaconda IPython Starter
-color 08
-@REM The below command does the following:
-@REM - opens the anaconda environment located at `condaEnvPrefix`
-@REM - clears the screen
-@REM - starts ipython
-cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
+@REM REMEMBER: Change the following, if applicable:
+@REM 1. `condaEnvPrefix`
+set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
+@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
+@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
+Title My Anaconda IPython Starter
+color 08
+@REM The below command does the following:
+@REM - opens the anaconda environment located at `condaEnvPrefix`
+@REM - clears the screen
+@REM - starts ipython
+cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,146 @@
-"""
-This is a template Python script.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-_ = None
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 3
-IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 1
-IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 4
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    ``: "{"..."}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Script
-    _ = pd
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Shifts the dates in a data set according to the date shift map for a patient.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import numpy as np
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+PATIENT_DE_IDENTIFICATION_MAP_PATH = Path(r"..\Concatenated Results\data\output\concatenateMaps\2023-12-13 11-59-04\Patient Key map.csv")
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    ``: "{"..."}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Load patient de-identification map
+    patientDeIdentificationMap = pd.read_csv(PATIENT_DE_IDENTIFICATION_MAP_PATH)
+
+    # Assign date shift values
+    array = np.random.randint(low=-30,
+                              high=30,
+                              size=len(patientDeIdentificationMap))
+    patientDeIdentificationMap["Date Shift"] = array
+
+    # Save results
+    savepath = runOutputDir.joinpath("Date Shift Map.CSV")
+    patientDeIdentificationMap.to_csv(savepath, index=False)
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-"""
-Compare two cohort (group) files.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-from drapi.code.drapi.compareGroups import (compareGroups,
-                                            determineMapType,
-                                            determineMapTypeFromMap,
-                                            mappingAnalysis)
-
-# Arguments
-COHORT_1_FILE_PATH = r""
-COHORT_2_FILE_PATH = r""
-PATIENT_MAP_FILE_PATH = r""
-FROM_COLUMN = ""
-TO_COLUMN = ""
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 3
-IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 3
-IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 6
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-# ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-#  "IRB_DIRECTORY",                 # noqa
-#  "DATA_REQUEST_DIRECTORY",        # noqa
-#  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `COHORT_1_FILE_PATH`: "{COHORT_1_FILE_PATH}"
-    `COHORT_2_FILE_PATH`: "{COHORT_2_FILE_PATH}"
-    `PATIENT_MAP_FILE_PATH`: "{PATIENT_MAP_FILE_PATH}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Load raw data
-    group1data0 = pd.read_csv(COHORT_1_FILE_PATH)
-    group2data = pd.read_csv(COHORT_2_FILE_PATH)
-
-    patientMap0 = pd.read_csv(PATIENT_MAP_FILE_PATH)
-
-    # Process data
-    patientMap = patientMap0[[FROM_COLUMN, TO_COLUMN]]
-
-    # Mapping analysis
-    mappingAnalysis(x0=group1data0,
-                    m0=patientMap,
-                    logger=logger)
-    group1data1_inner = group1data0.dropna().drop_duplicates().set_index(FROM_COLUMN).join(other=patientMap.set_index(FROM_COLUMN),
-                                                                                           how="inner",
-                                                                                           lsuffix="_L",
-                                                                                           rsuffix="_R").reset_index()
-    group1data1_outer = group1data0.dropna().drop_duplicates().set_index(FROM_COLUMN).join(other=patientMap.set_index(FROM_COLUMN),
-                                                                                           how="outer",
-                                                                                           lsuffix="_L",
-                                                                                           rsuffix="_R").reset_index()
-    group1series1 = group1data1_inner[TO_COLUMN].dropna().drop_duplicates()
-    group1series2 = group1data1_outer[TO_COLUMN].dropna().drop_duplicates()
-    group2series = group2data[TO_COLUMN].dropna().drop_duplicates()
-    compareGroups(group1=group1series1,
-                  group2=group2series,
-                  logger=logger)
-    compareGroups(group1=group1series2,
-                  group2=group2series,
-                  logger=logger)
-
-    mapType1 = determineMapType(x0=group1data0,
-                                x1=group1data1_inner[TO_COLUMN])
-    mapType2 = determineMapType(x0=group1data0,
-                                x1=group1data1_outer[TO_COLUMN])
-    mapType3 = determineMapTypeFromMap(x0=group1data0,
-                                       m0=patientMap,
-                                       logger=logger)
-    logger.info(f"""The mapping of group1 (inner-joined) is of type "{mapType1}".""")
-    logger.info(f"""The mapping of group1 (outer-joined) is of type "{mapType2}".""")
-    logger.info(f"""The mapping of group1 (from `determineMapTypeFromMap`) is of type "{mapType3}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+"""
+Compare two cohort (group) files.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+from drapi.code.drapi.compareGroups import (compareGroups,
+                                            determineMapType,
+                                            determineMapTypeFromMap,
+                                            mappingAnalysis)
+
+# Arguments
+COHORT_1_FILE_PATH = r""
+COHORT_2_FILE_PATH = r""
+PATIENT_MAP_FILE_PATH = r""
+FROM_COLUMN = ""
+TO_COLUMN = ""
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 3
+IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 3
+IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 6
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+# ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+#  "IRB_DIRECTORY",                 # noqa
+#  "DATA_REQUEST_DIRECTORY",        # noqa
+#  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `COHORT_1_FILE_PATH`: "{COHORT_1_FILE_PATH}"
+    `COHORT_2_FILE_PATH`: "{COHORT_2_FILE_PATH}"
+    `PATIENT_MAP_FILE_PATH`: "{PATIENT_MAP_FILE_PATH}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Load raw data
+    group1data0 = pd.read_csv(COHORT_1_FILE_PATH)
+    group2data = pd.read_csv(COHORT_2_FILE_PATH)
+
+    patientMap0 = pd.read_csv(PATIENT_MAP_FILE_PATH)
+
+    # Process data
+    patientMap = patientMap0[[FROM_COLUMN, TO_COLUMN]]
+
+    # Mapping analysis
+    mappingAnalysis(x0=group1data0,
+                    m0=patientMap,
+                    logger=logger)
+    group1data1_inner = group1data0.dropna().drop_duplicates().set_index(FROM_COLUMN).join(other=patientMap.set_index(FROM_COLUMN),
+                                                                                           how="inner",
+                                                                                           lsuffix="_L",
+                                                                                           rsuffix="_R").reset_index()
+    group1data1_outer = group1data0.dropna().drop_duplicates().set_index(FROM_COLUMN).join(other=patientMap.set_index(FROM_COLUMN),
+                                                                                           how="outer",
+                                                                                           lsuffix="_L",
+                                                                                           rsuffix="_R").reset_index()
+    group1series1 = group1data1_inner[TO_COLUMN].dropna().drop_duplicates()
+    group1series2 = group1data1_outer[TO_COLUMN].dropna().drop_duplicates()
+    group2series = group2data[TO_COLUMN].dropna().drop_duplicates()
+    compareGroups(group1=group1series1,
+                  group2=group2series,
+                  logger=logger)
+    compareGroups(group1=group1series2,
+                  group2=group2series,
+                  logger=logger)
+
+    mapType1 = determineMapType(x0=group1data0,
+                                x1=group1data1_inner[TO_COLUMN])
+    mapType2 = determineMapType(x0=group1data0,
+                                x1=group1data1_outer[TO_COLUMN])
+    mapType3 = determineMapTypeFromMap(x0=group1data0,
+                                       m0=patientMap,
+                                       logger=logger)
+    logger.info(f"""The mapping of group1 (inner-joined) is of type "{mapType1}".""")
+    logger.info(f"""The mapping of group1 (outer-joined) is of type "{mapType2}".""")
+    logger.info(f"""The mapping of group1 (from `determineMapTypeFromMap`) is of type "{mapType3}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import Collection
-
-MESSAGE_MODULO_CHUNKS = 100
-MIN_NUMBER_OF_MESSAGES = 100
-
-PLACEHOLDER1 = 1  # An integer
-PLACEHOLDER2 = []  # An iterable
-
-
-def func1(chunk1) -> Collection:
-    """
-    Dummy function that represents a process. `chunks` is a function of `chunk1`
-    """
-    result = []
-    return result
-
-
-def getNumChunks(result) -> int:
-    """
-    Dummy function that represents a counting process.
-    """
-    numChunks = 1
-    return numChunks
-
-
-def getChunks(result) -> Collection:
-    """
-    A dummy function that represents a chunking process.
-    """
-    chunks = []
-    return chunks
-
-
-numChunks1 = PLACEHOLDER1
-# >>> Calculate logging requency for loop layer 1
-if numChunks1 < MESSAGE_MODULO_CHUNKS:
-    moduloChunks1 = numChunks1
-else:
-    moduloChunks1 = round(numChunks1 / MESSAGE_MODULO_CHUNKS)
-if numChunks1 / moduloChunks1 < MIN_NUMBER_OF_MESSAGES:
-    moduloChunks1 = 1
-else:
-    pass
-# <<< <<< <<< <<<
-chunks = PLACEHOLDER2
-for it1, chunk1 in enumerate(chunks, start=1):
-    # >>> Set chunk verbosity for loop layer 1
-    if it1 % moduloChunks1 == 0:
-        allowLogging = True
-    else:
-        allowLogging = False
-    # <<< <<< <<< <<<
-    result1 = func1(chunk1)
-    numChunks2 = getNumChunks(result1)
-    chunks2 = getChunks(result1)
-    # >>> Calculate logging requency for loop layer 2
-    if numChunks2 < MESSAGE_MODULO_CHUNKS:
-        moduloChunks2 = numChunks2
-    else:
-        moduloChunks2 = round(numChunks2 / MESSAGE_MODULO_CHUNKS)
-    if numChunks2 / moduloChunks2 < MIN_NUMBER_OF_MESSAGES:
-        moduloChunks2 = 1
-    else:
-        pass
-    # <<< <<< <<< <<<
-    for it2, chunk2 in enumerate(chunks2, start=1):
-        # >>> Set chunk verbosity for loop layer 1
-        if it2 % moduloChunks2 == 0:
-            allowLogging = True
-        else:
-            allowLogging = False
-        # <<< <<< <<< <<<
+from typing import Collection
+
+MESSAGE_MODULO_CHUNKS = 100
+MIN_NUMBER_OF_MESSAGES = 100
+
+PLACEHOLDER1 = 1  # An integer
+PLACEHOLDER2 = []  # An iterable
+
+
+def func1(chunk1) -> Collection:
+    """
+    Dummy function that represents a process. `chunks` is a function of `chunk1`
+    """
+    result = []
+    return result
+
+
+def getNumChunks(result) -> int:
+    """
+    Dummy function that represents a counting process.
+    """
+    numChunks = 1
+    return numChunks
+
+
+def getChunks(result) -> Collection:
+    """
+    A dummy function that represents a chunking process.
+    """
+    chunks = []
+    return chunks
+
+
+numChunks1 = PLACEHOLDER1
+# >>> Calculate logging requency for loop layer 1
+if numChunks1 < MESSAGE_MODULO_CHUNKS:
+    moduloChunks1 = numChunks1
+else:
+    moduloChunks1 = round(numChunks1 / MESSAGE_MODULO_CHUNKS)
+if numChunks1 / moduloChunks1 < MIN_NUMBER_OF_MESSAGES:
+    moduloChunks1 = 1
+else:
+    pass
+# <<< <<< <<< <<<
+chunks = PLACEHOLDER2
+for it1, chunk1 in enumerate(chunks, start=1):
+    # >>> Set chunk verbosity for loop layer 1
+    if it1 % moduloChunks1 == 0:
+        allowLogging = True
+    else:
+        allowLogging = False
+    # <<< <<< <<< <<<
+    result1 = func1(chunk1)
+    numChunks2 = getNumChunks(result1)
+    chunks2 = getChunks(result1)
+    # >>> Calculate logging requency for loop layer 2
+    if numChunks2 < MESSAGE_MODULO_CHUNKS:
+        moduloChunks2 = numChunks2
+    else:
+        moduloChunks2 = round(numChunks2 / MESSAGE_MODULO_CHUNKS)
+    if numChunks2 / moduloChunks2 < MIN_NUMBER_OF_MESSAGES:
+        moduloChunks2 = 1
+    else:
+        pass
+    # <<< <<< <<< <<<
+    for it2, chunk2 in enumerate(chunks2, start=1):
+        # >>> Set chunk verbosity for loop layer 1
+        if it2 % moduloChunks2 == 0:
+            allowLogging = True
+        else:
+            allowLogging = False
+        # <<< <<< <<< <<<
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@REM REMEMBER: Change the following, if applicable:
-@REM 1. `condaEnvPrefix`
-set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
-@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
-@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
-Title My Anaconda IPython Starter
-color 08
-@REM The below command does the following:
-@REM - opens the anaconda environment located at `condaEnvPrefix`
-@REM - clears the screen
-@REM - starts ipython
-cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
+@REM REMEMBER: Change the following, if applicable:
+@REM 1. `condaEnvPrefix`
+set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
+@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
+@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
+Title My Anaconda IPython Starter
+color 08
+@REM The below command does the following:
+@REM - opens the anaconda environment located at `condaEnvPrefix`
+@REM - clears the screen
+@REM - starts ipython
+cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-"""
-Searches and selects notes by the list of note types contained in `NOTE_TYPES_TO_FILTER_BY` and outputs the corresponding metadata and notes text.
-
-Note we distinguish between the following three concepts
-    - Note Class (two values)
-    - Note Category (four values)
-    - Note Type (More than 100 values for each class.)
-See the NOTE comment tags in the code for details.
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-FREE_TEXT_DIR_PATH = Path(r"data\output\freeText\...\free_text")  # TODO
-COHORT_NAME = ""  # TODO
-NOTE_TYPES_TO_FILTER_BY = ["order_impression: IMAGING",
-                           "order_narative: IMAGING"]  # TODO
-DE_IDENTIFICATION_MAP_PATH_FOR_NOTES = r"data\output\freeText\...\mapping\map_note_link.csv"  # TODO
-DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS = r"data\output\freeText\...\mapping\map_order.csv"  # TODO
-USE_DE_IDENTIFIED_NOTE_VERSION = True  # TODO
-CHUNKSIZE = 10000
-
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-# ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-#  "IRB_DIRECTORY",                 # noqa
-#  "DATA_REQUEST_DIRECTORY",        # noqa
-#  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-noteDeIdentificationMaps = {"Notes": DE_IDENTIFICATION_MAP_PATH_FOR_NOTES,
-                            "Orders": DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS}
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `FREE_TEXT_DIR_PATH`: "{FREE_TEXT_DIR_PATH}"
-    `COHORT_NAME`: "{COHORT_NAME}"
-    `NOTE_TYPES_TO_FILTER_BY`: "{NOTE_TYPES_TO_FILTER_BY}"
-    `DE_IDENTIFICATION_MAP_PATH_FOR_NOTES`: "{DE_IDENTIFICATION_MAP_PATH_FOR_NOTES}"
-    `DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS`: "{DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS}"
-    `USE_DE_IDENTIFIED_NOTE_VERSION`: "{USE_DE_IDENTIFIED_NOTE_VERSION}"
-    `CHUNKSIZE`: "{CHUNKSIZE}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Search by note types
-    logger.info("Searching by note types.")
-    LIST_OF_NOTE_TARGET_FILES_AND_DIRS = ["_note"]
-    LIST_OF_ORDER_TARGET_FILES_AND_DIRS = ["_order_impression",
-                                           "_order",
-                                           "_order_narrative",
-                                           "_order_result_comment"]
-    LIST_OF_TARGET_FILES_AND_FOLDERS = LIST_OF_NOTE_TARGET_FILES_AND_DIRS + LIST_OF_ORDER_TARGET_FILES_AND_DIRS
-    resultsdi = {}
-    for fpath in FREE_TEXT_DIR_PATH.iterdir():
-        logger.info(f"""  Working on directory item "{fpath.absolute().relative_to(rootDirectory)}".""")
-        if fpath.suffix.lower() == ".csv" and any([fname in fpath.stem for fname in LIST_OF_TARGET_FILES_AND_FOLDERS]):
-            logger.info("""    This item has met the criteria for processing.""")
-            numChunks = 0
-            logger.info("""    Counting the number of chunks in the file.""")
-            for dfchunk in pd.read_csv(fpath, chunksize=CHUNKSIZE):
-                numChunks += 1
-            logger.info("""    Counting the number of chunks in the file - done.""")
-            fileResults = pd.DataFrame()
-            for it, dfchunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE), start=1):
-                logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                mask = dfchunk["NoteType"].isin(NOTE_TYPES_TO_FILTER_BY)
-                subset = dfchunk[mask]
-                fileResults = pd.concat([fileResults, subset])
-            resultsdi[fpath.stem] = fileResults.drop_duplicates()
-        else:
-            logger.info("""    This item has NOT met the criteria for processing.""")
-
-    # Save search results
-    logger.info("Saving search results to the drive.")
-    for noteCategory, df in resultsdi.items():
-        rsavepath = runOutputDir.joinpath("Selected Notes Metadata",
-                                          f"{noteCategory}.CSV")
-        makeDirPath(rsavepath.parent)
-        df.to_csv(rsavepath, index=False)
-    logger.info("Saving search results to the drive - done.")
-
-    # Concatenate results by note class
-    logger.info("Concatenating results by note class.")
-    results = {"Notes": None,
-               "Orders": None}
-    # NOTE: Here we introduce the "Note Category" concept, which is one of four values: "Note", "Order Impression", "Order Narrative" or "Order Result Comment".
-    for noteCategory, df in resultsdi.items():
-        if any([name in noteCategory for name in LIST_OF_NOTE_TARGET_FILES_AND_DIRS]):
-            results["Notes"] = pd.concat([results["Notes"], df["LinkageNoteID"]])
-        elif any([name in noteCategory for name in LIST_OF_ORDER_TARGET_FILES_AND_DIRS]):
-            results["Orders"] = pd.concat([results["Orders"], df["OrderKey"]])
-        else:
-            raise Exception("Something unexpected happened.")
-    # NOTE: Here we introduce the "Note Class" concept, which is one of two values: "Note" or "Order".
-    for noteClass, series in results.items():
-        series = pd.Series(series)
-        results[noteClass] = series.drop_duplicates().sort_values()
-    logger.info("Concatenating results by note class - done.")
-
-    # For each note class, filter by its corresponding note identifier, i.e., `LinkageNoteID` or `OrderKey`
-    for noteClass, noteIdentifierValues in results.items():
-        logger.info(f"""  Working on note class "{noteClass}".""")
-        # Get note class identifier map
-        if noteClass == "Notes":
-            NOTE_IDENTIFIER_TYPE = "LinkageNoteID"
-            NOTE_IDENTIFIER_TYPE_DE_IDENTIFIED = "deid_link_note_id"
-        elif noteClass == "Orders":
-            NOTE_IDENTIFIER_TYPE = "OrderKey"
-            NOTE_IDENTIFIER_TYPE_DE_IDENTIFIED = "deid_order_id"
-        noteIdentifierValues = pd.DataFrame(noteIdentifierValues)
-        noteIdentifierValues = noteIdentifierValues.set_index(NOTE_IDENTIFIER_TYPE).sort_index()
-        mapPath = noteDeIdentificationMaps[noteClass]
-        noteIdentifierMap = pd.read_csv(mapPath)
-        noteIdentifierMap = noteIdentifierMap.set_index(NOTE_IDENTIFIER_TYPE)
-        selectedNoteIdentiferMap = noteIdentifierValues.join(noteIdentifierMap, how="inner")
-        selectedNoteIdentiferMap = selectedNoteIdentiferMap.reset_index()
-        selectedNoteIdentiferMap = selectedNoteIdentiferMap.set_index(NOTE_IDENTIFIER_TYPE_DE_IDENTIFIED)
-
-        # Join map on note text files.
-        DICT_OF_TARGET_FILES_AND_FOLDERS = {"Notes": LIST_OF_NOTE_TARGET_FILES_AND_DIRS,
-                                            "Orders": LIST_OF_ORDER_TARGET_FILES_AND_DIRS}
-        if USE_DE_IDENTIFIED_NOTE_VERSION:
-            noteDeIdentificationPrefix = "deid"
-        else:
-            noteDeIdentificationPrefix = ""
-        for fpath in FREE_TEXT_DIR_PATH.glob("**/*"):
-            logger.info(f"""    Working on directory item "{fpath.absolute().relative_to(rootDirectory)}".""")
-            listOfClassTargetFilesAndFolders = DICT_OF_TARGET_FILES_AND_FOLDERS[noteClass]
-            if fpath.suffix.lower() == ".tsv" and any([fname in fpath.stem for fname in listOfClassTargetFilesAndFolders]) and "deid_" in fpath.stem:
-                logger.info("""  ..  This item has met the criteria for processing.""")
-                # Determine note identifier
-                if any([f"{noteDeIdentificationPrefix}{nameRoot}" in fpath.stem for nameRoot in LIST_OF_NOTE_TARGET_FILES_AND_DIRS]):
-                    noteIdentifierDeIdentifiedColumnName = "deid_link_note_id"
-                elif any([f"{noteDeIdentificationPrefix}{nameRoot}" in fpath.stem for nameRoot in LIST_OF_ORDER_TARGET_FILES_AND_DIRS]):
-                    noteIdentifierDeIdentifiedColumnName = "deid_order_id"
-                else:
-                    raise Exception("Something went wrong.")
-                # Count number of chunks
-                logger.info("""  ..  Counting the number of chunks in the file.""")
-                numChunks = 0
-                for dfchunk in pd.read_csv(fpath, chunksize=CHUNKSIZE, delimiter="\t"):
-                    numChunks += 1
-                # Iterate over chunks
-                logger.info("""  ..  Counting the number of chunks in the file - done.""")
-                header = True
-                mode = "w"
-                for it, dfchunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE, delimiter="\t"), start=1):
-                    logger.info(f"""  ..    Working on chunk {it} of {numChunks}.""")
-                    # Filter by selected note or order identifiers.
-                    dfchunk = dfchunk.set_index(noteIdentifierDeIdentifiedColumnName)
-                    selectedText = selectedNoteIdentiferMap.join(dfchunk, how="inner")
-                    selectedText = selectedText["note_text"]
-                    # Define `savepath` based on `fpath`
-                    savepath = runOutputDir.joinpath("Selected Notes",
-                                                     "{fpath.stem}.TSV")
-                    makeDirPath(savepath.parent)
-                    # Save to file
-                    selectedText = selectedText.reset_index()
-                    selectedText.to_csv(savepath, index=False, header=header, mode=mode, sep="\t")
-                    header = False
-                    mode = "a"
-                logger.info(f"""  ..  Chunks saved to "{savepath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logger.info("""  ..  This item has NOT met the criteria for processing.""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+Searches and selects notes by the list of note types contained in `NOTE_TYPES_TO_FILTER_BY` and outputs the corresponding metadata and notes text.
+
+Note we distinguish between the following three concepts
+    - Note Class (two values)
+    - Note Category (four values)
+    - Note Type (More than 100 values for each class.)
+See the NOTE comment tags in the code for details.
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+FREE_TEXT_DIR_PATH = Path(r"data\output\freeText\...\free_text")  # TODO
+COHORT_NAME = ""  # TODO
+NOTE_TYPES_TO_FILTER_BY = ["order_impression: IMAGING",
+                           "order_narative: IMAGING"]  # TODO
+DE_IDENTIFICATION_MAP_PATH_FOR_NOTES = r"data\output\freeText\...\mapping\map_note_link.csv"  # TODO
+DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS = r"data\output\freeText\...\mapping\map_order.csv"  # TODO
+USE_DE_IDENTIFIED_NOTE_VERSION = True  # TODO
+CHUNKSIZE = 10000
+
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+# ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+#  "IRB_DIRECTORY",                 # noqa
+#  "DATA_REQUEST_DIRECTORY",        # noqa
+#  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+pass
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+noteDeIdentificationMaps = {"Notes": DE_IDENTIFICATION_MAP_PATH_FOR_NOTES,
+                            "Orders": DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS}
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `FREE_TEXT_DIR_PATH`: "{FREE_TEXT_DIR_PATH}"
+    `COHORT_NAME`: "{COHORT_NAME}"
+    `NOTE_TYPES_TO_FILTER_BY`: "{NOTE_TYPES_TO_FILTER_BY}"
+    `DE_IDENTIFICATION_MAP_PATH_FOR_NOTES`: "{DE_IDENTIFICATION_MAP_PATH_FOR_NOTES}"
+    `DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS`: "{DE_IDENTIFICATION_MAP_PATH_FOR_ORDERS}"
+    `USE_DE_IDENTIFIED_NOTE_VERSION`: "{USE_DE_IDENTIFIED_NOTE_VERSION}"
+    `CHUNKSIZE`: "{CHUNKSIZE}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Search by note types
+    logger.info("Searching by note types.")
+    LIST_OF_NOTE_TARGET_FILES_AND_DIRS = ["_note"]
+    LIST_OF_ORDER_TARGET_FILES_AND_DIRS = ["_order_impression",
+                                           "_order",
+                                           "_order_narrative",
+                                           "_order_result_comment"]
+    LIST_OF_TARGET_FILES_AND_FOLDERS = LIST_OF_NOTE_TARGET_FILES_AND_DIRS + LIST_OF_ORDER_TARGET_FILES_AND_DIRS
+    resultsdi = {}
+    for fpath in FREE_TEXT_DIR_PATH.iterdir():
+        logger.info(f"""  Working on directory item "{fpath.absolute().relative_to(rootDirectory)}".""")
+        if fpath.suffix.lower() == ".csv" and any([fname in fpath.stem for fname in LIST_OF_TARGET_FILES_AND_FOLDERS]):
+            logger.info("""    This item has met the criteria for processing.""")
+            numChunks = 0
+            logger.info("""    Counting the number of chunks in the file.""")
+            for dfchunk in pd.read_csv(fpath, chunksize=CHUNKSIZE):
+                numChunks += 1
+            logger.info("""    Counting the number of chunks in the file - done.""")
+            fileResults = pd.DataFrame()
+            for it, dfchunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE), start=1):
+                logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                mask = dfchunk["NoteType"].isin(NOTE_TYPES_TO_FILTER_BY)
+                subset = dfchunk[mask]
+                fileResults = pd.concat([fileResults, subset])
+            resultsdi[fpath.stem] = fileResults.drop_duplicates()
+        else:
+            logger.info("""    This item has NOT met the criteria for processing.""")
+
+    # Save search results
+    logger.info("Saving search results to the drive.")
+    for noteCategory, df in resultsdi.items():
+        rsavepath = runOutputDir.joinpath("Selected Notes Metadata",
+                                          f"{noteCategory}.CSV")
+        makeDirPath(rsavepath.parent)
+        df.to_csv(rsavepath, index=False)
+    logger.info("Saving search results to the drive - done.")
+
+    # Concatenate results by note class
+    logger.info("Concatenating results by note class.")
+    results = {"Notes": None,
+               "Orders": None}
+    # NOTE: Here we introduce the "Note Category" concept, which is one of four values: "Note", "Order Impression", "Order Narrative" or "Order Result Comment".
+    for noteCategory, df in resultsdi.items():
+        if any([name in noteCategory for name in LIST_OF_NOTE_TARGET_FILES_AND_DIRS]):
+            results["Notes"] = pd.concat([results["Notes"], df["LinkageNoteID"]])
+        elif any([name in noteCategory for name in LIST_OF_ORDER_TARGET_FILES_AND_DIRS]):
+            results["Orders"] = pd.concat([results["Orders"], df["OrderKey"]])
+        else:
+            raise Exception("Something unexpected happened.")
+    # NOTE: Here we introduce the "Note Class" concept, which is one of two values: "Note" or "Order".
+    for noteClass, series in results.items():
+        series = pd.Series(series)
+        results[noteClass] = series.drop_duplicates().sort_values()
+    logger.info("Concatenating results by note class - done.")
+
+    # For each note class, filter by its corresponding note identifier, i.e., `LinkageNoteID` or `OrderKey`
+    for noteClass, noteIdentifierValues in results.items():
+        logger.info(f"""  Working on note class "{noteClass}".""")
+        # Get note class identifier map
+        if noteClass == "Notes":
+            NOTE_IDENTIFIER_TYPE = "LinkageNoteID"
+            NOTE_IDENTIFIER_TYPE_DE_IDENTIFIED = "deid_link_note_id"
+        elif noteClass == "Orders":
+            NOTE_IDENTIFIER_TYPE = "OrderKey"
+            NOTE_IDENTIFIER_TYPE_DE_IDENTIFIED = "deid_order_id"
+        noteIdentifierValues = pd.DataFrame(noteIdentifierValues)
+        noteIdentifierValues = noteIdentifierValues.set_index(NOTE_IDENTIFIER_TYPE).sort_index()
+        mapPath = noteDeIdentificationMaps[noteClass]
+        noteIdentifierMap = pd.read_csv(mapPath)
+        noteIdentifierMap = noteIdentifierMap.set_index(NOTE_IDENTIFIER_TYPE)
+        selectedNoteIdentiferMap = noteIdentifierValues.join(noteIdentifierMap, how="inner")
+        selectedNoteIdentiferMap = selectedNoteIdentiferMap.reset_index()
+        selectedNoteIdentiferMap = selectedNoteIdentiferMap.set_index(NOTE_IDENTIFIER_TYPE_DE_IDENTIFIED)
+
+        # Join map on note text files.
+        DICT_OF_TARGET_FILES_AND_FOLDERS = {"Notes": LIST_OF_NOTE_TARGET_FILES_AND_DIRS,
+                                            "Orders": LIST_OF_ORDER_TARGET_FILES_AND_DIRS}
+        if USE_DE_IDENTIFIED_NOTE_VERSION:
+            noteDeIdentificationPrefix = "deid"
+        else:
+            noteDeIdentificationPrefix = ""
+        for fpath in FREE_TEXT_DIR_PATH.glob("**/*"):
+            logger.info(f"""    Working on directory item "{fpath.absolute().relative_to(rootDirectory)}".""")
+            listOfClassTargetFilesAndFolders = DICT_OF_TARGET_FILES_AND_FOLDERS[noteClass]
+            if fpath.suffix.lower() == ".tsv" and any([fname in fpath.stem for fname in listOfClassTargetFilesAndFolders]) and "deid_" in fpath.stem:
+                logger.info("""  ..  This item has met the criteria for processing.""")
+                # Determine note identifier
+                if any([f"{noteDeIdentificationPrefix}{nameRoot}" in fpath.stem for nameRoot in LIST_OF_NOTE_TARGET_FILES_AND_DIRS]):
+                    noteIdentifierDeIdentifiedColumnName = "deid_link_note_id"
+                elif any([f"{noteDeIdentificationPrefix}{nameRoot}" in fpath.stem for nameRoot in LIST_OF_ORDER_TARGET_FILES_AND_DIRS]):
+                    noteIdentifierDeIdentifiedColumnName = "deid_order_id"
+                else:
+                    raise Exception("Something went wrong.")
+                # Count number of chunks
+                logger.info("""  ..  Counting the number of chunks in the file.""")
+                numChunks = 0
+                for dfchunk in pd.read_csv(fpath, chunksize=CHUNKSIZE, delimiter="\t"):
+                    numChunks += 1
+                # Iterate over chunks
+                logger.info("""  ..  Counting the number of chunks in the file - done.""")
+                header = True
+                mode = "w"
+                for it, dfchunk in enumerate(pd.read_csv(fpath, chunksize=CHUNKSIZE, delimiter="\t"), start=1):
+                    logger.info(f"""  ..    Working on chunk {it} of {numChunks}.""")
+                    # Filter by selected note or order identifiers.
+                    dfchunk = dfchunk.set_index(noteIdentifierDeIdentifiedColumnName)
+                    selectedText = selectedNoteIdentiferMap.join(dfchunk, how="inner")
+                    selectedText = selectedText["note_text"]
+                    # Define `savepath` based on `fpath`
+                    savepath = runOutputDir.joinpath("Selected Notes",
+                                                     "{fpath.stem}.TSV")
+                    makeDirPath(savepath.parent)
+                    # Save to file
+                    selectedText = selectedText.reset_index()
+                    selectedText.to_csv(savepath, index=False, header=header, mode=mode, sep="\t")
+                    header = False
+                    mode = "a"
+                logger.info(f"""  ..  Chunks saved to "{savepath.absolute().relative_to(rootDirectory)}".""")
+            else:
+                logger.info("""  ..  This item has NOT met the criteria for processing.""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,697 +1,697 @@
-from __future__ import annotations
-
-import concurrent.futures
-import logging
-import os
-import random
-import re
-import shutil
-from datetime import timedelta
-from logging import Logger
-from pathlib import Path
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from _typeshed.dbapi import DBAPIConnection
-# Third-party packages
-import pandas as pd
-import pymssql
-import sqlalchemy as sa
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    replace_sql_query,
-                                    successiveParents)
-
-# Arguments: Script settings
-COHORT_NAME = "SGMCPLGB"                                    # An arbitrary name used in file names
-COHORT_FILE = "cohort.csv"                                    # A file name that is located directory specified by the variable `data_dir`
-IRB_NUMBER = "IRB201902162"                                     # Used for creating the de-identification map IDs.
-ID_TYPE = "PatientKey"                                        # Pick from "EncounterCSN", "EncounterKey", or "PatientKey". Choose the ID type you used in `COHORT_FILE`
-NOTE_VERSION = "all"                                   # Pick from "all", or "last"
-DE_IDENTIFICATION_MODE = "phi"                         # Pick from "deid", "lds", or "phi"
-LOG_LEVEL = "DEBUG"                                      # See the "logging" module for valid values for the `loglevel` parameter.
-SQL_ENCOUNTER_EFFECTIVE_DATE_START = '2011-06-01'   # The beginning of date range of encounters to collect. Format: YYYY-MM-DD
-SQL_ENCOUNTER_EFFECTIVE_DATE_END = '2023-12-31'     # The end of date range of encounters to collect. Format: YYYY-MM-DD
-
-# Arguments: SQL connection settings
-USE_WINDOWS_AUTHENTICATION = True
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE_PROD = "DWS_PROD"
-DATABASE_NOTES = "DWS_NOTES"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "PROJECT_OR_PORTION_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path Construction: Project-specific
-notes_dir = runOutputDir.joinpath('free_text')  # all notes related files are saved in 'notes' subdirectory of 'data' directory
-map_dir = runOutputDir.joinpath('mapping')  # mappings are saved in 'mapping' subdirectory of 'data' folder.
-disclosure_dir = runOutputDir.joinpath('disclosure')
-
-# Variables: Map legacy variables to DRAPI-LEMUR standard variables: Script settings
-cohort = COHORT_NAME
-id_type = ID_TYPE
-note_version = NOTE_VERSION
-irb = IRB_NUMBER
-deid_mode = DE_IDENTIFICATION_MODE
-
-# Variables: Map legacy variables to DRAPI-LEMUR standard variables: Path construction
-base_dir = str(projectDir)
-data_dir = dataDir
-sql_dir = sqlDir
-
-# Variables: Map legacy variables to DRAPI-LEMUR standard variables: SQL Parameters
-host = SERVER
-database_prod = DATABASE_PROD
-database_notes = DATABASE_NOTES
-
-# Variables: SQL connection settings
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Directory creation: Project-specific
-for dir in [data_dir, sql_dir, notes_dir, disclosure_dir]:
-    makeDirPath(dir)
-if DE_IDENTIFICATION_MODE.lower() == "phi":
-    pass
-elif DE_IDENTIFICATION_MODE.lower() in ["deid", "lds"]:
-    makeDirPath(map_dir)
-else:
-    raise Exception(f"Unexpected value for `DE_IDENTIFICATION_MODE`: {DE_IDENTIFICATION_MODE}.")
-
-# Functions
-
-
-def connectToDatabase(host: str,
-                      database: str,
-                      useWindowsAuthentication=True) -> DBAPIConnection:
-    """
-    Connects to a SQL database given a `host` (server) and `database` value.
-    """
-    if useWindowsAuthentication:
-        connection = pymssql.connect(host=host,
-                                     database=database)
-    else:
-        conStr = f"mssql+pymssql://{uid}:{PWD}@{host}/{database}"
-        connection = sa.create_engine(conStr).connect()
-    return connection
-
-
-def executeQuery(query: str, host: str, database: str) -> pd.DataFrame:
-    """
-    Executes a SQL query.
-    INPUT:
-        `query`: a string
-        `host`: a string
-        `databse`: a string
-    OUTPUT:
-        A pandas dataframe object.
-    """
-    databaseConnection = connectToDatabase(host, database)
-    queryResult = pd.read_sql(query, databaseConnection)
-    databaseConnection.close()
-    return queryResult
-
-
-# notes methods
-
-
-def pull_metadata(note_version, id_type, note_type, sql_dir, cohort_dir, notes_dir, cohort, logger: Logger):
-    logger.info(f"""Function arguments:
-    `note_version`: {note_version}
-    `id_type`:      {id_type}
-    `note_type`:    {note_type}
-    `sql_dir`:      {sql_dir}
-    `cohort_dir`:   {cohort_dir}
-    `notes_dir`:    {notes_dir}
-    `cohort`:       {cohort}
-    `logger`:       {logger}""")
-    m = 'w'  # mode of the output file
-    h = True  # header of the output file
-    counter = 1  # used only for tracking/time estimation purposes
-    if (id_type == 'PatientKey'):
-        in_file = COHORT_FILE
-    elif (id_type == 'EncounterCSN' or id_type == 'EncounterKey'):
-        in_file = COHORT_FILE
-    for df in pd.read_csv(os.path.join(cohort_dir, in_file), chunksize=1000, engine='python'):
-        df = df[[id_type]]
-        id_str = df[id_type].unique().tolist()
-        logger.info(f"  This chunk of your input file containing patient or encounter ID's is of length {len(id_str):,}.")
-        id_str = "','".join(str(x) for x in id_str)
-        id_str = "'" + id_str + "'"
-        query_file = note_type + '_metadata.sql'
-        logger.info(f"Reading query file: {query_file}")
-        fpath = os.path.join(sql_dir, query_file)
-        with open(fpath, "r") as file:
-            query = file.read()
-        query = replace_sql_query(query, "XXXXX", id_str)
-        query = replace_sql_query(query, "{PYTHON_VARIABLE: SQL_ENCOUNTER_EFFECTIVE_DATE_START}", SQL_ENCOUNTER_EFFECTIVE_DATE_START)
-        query = replace_sql_query(query, "{PYTHON_VARIABLE: SQL_ENCOUNTER_EFFECTIVE_DATE_END}", SQL_ENCOUNTER_EFFECTIVE_DATE_END)
-
-        logger.log(9, f"Using the following query:\n>>> Begin query >>>\n{query}\n<<< End query <<<")
-        result = executeQuery(query=query,
-                              host=host,
-                              database=database_prod)
-
-        logger.info(f"The chunk query has {len(result):,} rows.")
-        result = result.drop_duplicates()
-
-        logger.info(f"After dropping duplicates, the chunk query has {len(result):,} rows.")
-        if (note_type == 'note' and note_version == 'last'):  # keep only the last version of the note
-            result = result.sort_values(by=['NoteKey', 'ContactNumber'], ascending=[True, False])
-            result = result.drop_duplicates(['NoteKey'])
-        result_file = cohort + '_' + note_type + '_metadata.csv'
-        result.to_csv(os.path.join(notes_dir, result_file), index=False, mode=m, header=h)
-        m = 'a'
-        h = False
-        logger.info(f'Completed chunk {counter}')
-        counter = counter + 1
-    return
-
-
-def split_metadata(note_type, notes_dir, cohort, logger: Logger):
-    in_file = cohort + '_' + note_type + '_metadata.csv'
-    file_count = 1
-    for df in pd.read_csv(os.path.join(notes_dir, in_file), chunksize=1000000):
-        out_file = cohort + '_' + note_type + '_metadata_' + str(file_count) + '.csv'
-
-        logger.info(f"Working on file {file_count}.")
-        # ensure that all ID columns are integers
-        columns = df.columns
-        for c in ['NoteKey', 'NoteID', 'LinkageNoteID', 'OrderKey', 'OrderID', 'PatientKey', 'EncounterKey', 'EncounterCSN', 'AuthoringProviderKey', 'CosignProviderKey', 'OrderingProviderKey', 'AuthorizingProviderKey']:
-            if (c in columns):
-                # fill missing values with 0 since 0 is never used for these IDs in reality
-                df[c] = df[c].fillna(0)
-                # use string instead of int type since some fields, such as EncounterCSN, are bigger than what python considers an integer
-                df[c] = df.apply(lambda row: str(row[c]).split('.0')[0], axis=1)
-        df.to_csv(os.path.join(notes_dir, out_file), index=False)
-        file_count = file_count + 1
-    return
-
-
-def pull_text(item, note_type, note_id, sql_dir, notes_dir, dir_final, logger: Logger):
-    logger.info(f"""Processing item "{item}".""")
-    # Pull text
-    header = True  # header of the output file
-    mode = 'w'  # mode of the output file
-    for notes in pd.read_csv(os.path.join(notes_dir, item), chunksize=10000, engine='python'):
-        note_list = notes[note_id].unique().tolist()
-        note_list = ",".join(str(int(x)) for x in note_list)
-        query_file = note_type + '_text.sql'
-        query_file = os.path.join(sql_dir, query_file)
-        fpath = os.path.join(sql_dir, query_file)
-        with open(fpath, "r") as file:
-            query = file.read()
-        query = replace_sql_query(query, "XXXXX", note_list)
-        result = executeQuery(query=query,
-                              host=host,
-                              database=database_notes)
-        # ensure that all ID columns are integers
-        columns = result.columns
-        for c in ['LinkageNoteID', 'OrderKey']:
-            if (c in columns):
-                # fill missing values with 0 since 0 is never used for these IDs in reality
-                result[c] = result[c].fillna(0)
-                # use string instead of int type since some fields, such as EncounterCSN, are bigger than what python considers an integer
-                result[c] = result.apply(lambda row: str(row[c]).split('.0')[0], axis=1)
-        file_count = item.split('.csv')[0].split('_')[-1]
-        file_out = note_type + '_' + str(file_count) + '.tsv'
-        result.to_csv(os.path.join(dir_final, file_out), header=header, mode=mode, sep='\t', encoding="UTF-8", index=False)
-        header = False
-        mode = 'a'
-    return
-
-
-def pull_text_in_parallel(note_type, sql_dir, notes_dir, cohort, logger: Logger):
-    # Prepare for text pull
-    if (note_type == 'note'):
-        dir_final = os.path.join(notes_dir, cohort + '_note')
-        if (not os.path.exists(dir_final)):
-            os.makedirs(dir_final)
-        note_id = 'LinkageNoteID'
-    elif (note_type == 'order_narrative'):
-        dir_final = os.path.join(notes_dir, cohort + '_order_narrative')
-        if (not os.path.exists(dir_final)):
-            os.makedirs(dir_final)
-        note_id = 'OrderKey'
-    elif (note_type == 'order_impression'):
-        dir_final = os.path.join(notes_dir, cohort + '_order_impression')
-        if (not os.path.exists(dir_final)):
-            os.makedirs(dir_final)
-        note_id = 'OrderKey'
-    elif (note_type == 'order_result_comment'):
-        dir_final = os.path.join(notes_dir, cohort + '_order_result_comment')
-        if (not os.path.exists(dir_final)):
-            os.makedirs(dir_final)
-        note_id = 'OrderKey'
-    # identify all metadata files for specific note type
-    pattern = cohort + '_' + note_type + '_metadata_.*.csv'  # hot fix 2022-05-10
-    items = [f for f in os.listdir(notes_dir) if re.match(pattern, f)]
-    logger.info(f"""This is the list of items that matched the criteria for processing: {items}.""")
-    # start pullng text. By default, number of parallel threads is set to 4.
-    with concurrent.futures.ThreadPoolExecutor(max_workers=4) as executor:
-        result_futures = {executor.submit(pull_text, item, note_type, note_id, sql_dir, notes_dir, dir_final, logger): item for item in items}
-        for future in concurrent.futures.as_completed(result_futures):
-            item = result_futures[future]
-            try:
-                _ = future.result()
-                logger.info(f"""Completed item "{item}".""")
-            except Exception as e:
-                logger.info(f"""An exception was generated by item "{item}": "{e}".""")
-    return
-
-
-def combine_order_metadata(notes_dir, cohort):
-    m = 'w'
-    h = True
-    for file1 in ['order_narrative', 'order_impression', 'order_result_comment']:
-        file = cohort + '_' + file1 + '_metadata.csv'
-        if os.path.exists(os.path.join(notes_dir, file)):
-            df = pd.read_csv(os.path.join(notes_dir, file))
-            if (file1 in ['order_narrative', 'order_impression']):
-                df['Line'] = ''
-            df = df[['OrderKey', 'Line', 'OrderID', 'OrderPlacedDatetime', 'OrderResultDatetime', 'PatientKey', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterKey', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
-            df.to_csv(os.path.join(notes_dir, '{}_order_metadata.csv'.format(cohort)), index=False, mode=m, header=h)
-            m = 'a'
-            h = False
-    return
-
-
-def create_encounters(notes_dir):
-    df = pd.DataFrame()
-    for file in ['{}_order_narrative_metadata.csv'.format(cohort), '{}_order_impression_metadata.csv'.format(cohort), '{}_order_result_comment_metadata.csv'.format(cohort), '{}_note_metadata.csv'.format(cohort)]:
-        for dfx in pd.read_csv(os.path.join(notes_dir, file), chunksize=100000):
-            df1 = dfx[['EncounterCSN']].drop_duplicates()
-            df = pd.concat([df, df1])
-            df.drop_duplicates(inplace=True)
-    df.to_csv(os.path.join(notes_dir, 'encounters.csv'), index=False)
-    return
-
-
-def create_provider_metadata(notes_dir, cohort):
-    m = 'w'
-    h = True
-    df = pd.DataFrame()
-    for file1 in ['order_narrative', 'order_impression', 'order_result_comment', 'note']:
-        # for file in ['note']:
-        file = cohort + '_' + file1 + '_metadata.csv'
-        if os.path.exists(os.path.join(notes_dir, file)):
-            for dfx in pd.read_csv(os.path.join(notes_dir, file), chunksize=100000):
-                if (file1 in ['order_narrative', 'order_impression', 'order_result_comment']):
-                    df1 = dfx[['OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty']]
-                    df1 = df1.rename(columns={"OrderingProviderKey": "ProviderKey", "OrderingProviderType": "ProviderType", "OrderingProviderSpecialty": "ProviderSpecialty"})
-                    df2 = dfx[['AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
-                    df2 = df2.rename(columns={"AuthorizingProviderKey": "ProviderKey", "AuthorizingProviderType": "ProviderType", "AuthorizingProviderSpecialty": "ProviderSpecialty"})
-                elif (file1 in ['note']):
-                    df1 = dfx[['AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty']]
-                    df1 = df1.rename(columns={"AuthoringProviderKey": "ProviderKey", "AuthoringProviderType": "ProviderType", "AuthoringProviderSpecialty": "ProviderSpecialty"})
-                    df2 = dfx[['CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']]
-                    df2 = df2.rename(columns={"CosignProviderKey": "ProviderKey", "CosignProviderType": "ProviderType", "CosignProviderSpecialty": "ProviderSpecialty"})
-                df1 = pd.concat([df1, df2])
-                df1.drop_duplicates(inplace=True)
-                df = pd.concat([df, df1])
-                df.drop_duplicates(inplace=True)
-            df.to_csv(os.path.join(notes_dir, 'provider_metadata.csv'), index=False, mode=m, header=h)
-            m = 'a'
-            h = False
-    return
-
-
-def generate_map(deid_mode, in_dir, map_dir, concept, cohort):
-    """
-    `concept` can be any of the following values:
-        - patient
-        - encounter
-        - note
-        - note_link
-        - order
-        - provider
-    """
-    # define variables
-    if (concept == 'patient'):
-        concept_cd = 'PAT'
-        concept_id = 'deid_pat_id'
-        file = os.path.join(in_dir, COHORT_FILE)  # NOTE
-        concept_column = 'PatientKey'
-    elif (concept == 'encounter'):
-        concept_cd = 'ENC'
-        concept_id = 'deid_enc_id'
-        create_encounters(in_dir)
-        file = os.path.join(in_dir, 'encounters.csv')
-        concept_column = 'EncounterCSN'
-    elif (concept == 'note'):
-        concept_cd = 'NOTE'
-        concept_id = 'deid_note_id'
-        file = os.path.join(in_dir, '{}_note_metadata.csv'.format(cohort))
-        concept_column = 'NoteKey'
-    elif (concept == 'note_link'):
-        concept_cd = 'LINK_NOTE'
-        concept_id = 'deid_link_note_id'
-        file = os.path.join(in_dir, '{}_note_metadata.csv'.format(cohort))
-        concept_column = 'LinkageNoteID'
-    elif (concept == 'order'):
-        concept_cd = 'ORDER'
-        concept_id = 'deid_order_id'
-        combine_order_metadata(in_dir, cohort)
-        file = os.path.join(in_dir, '{}_order_metadata.csv'.format(cohort))
-        concept_column = 'OrderKey'
-    elif (concept == 'provider'):
-        concept_cd = 'PROV'
-        concept_id = 'deid_provider_id'
-        create_provider_metadata(in_dir, cohort)
-        file = os.path.join(in_dir, 'provider_metadata.csv')
-        concept_column = 'ProviderKey'
-    else:
-        logging.error(f"""Nonexisting concept in `generate_map` method: "{concept}".""")
-
-    ids_final = pd.DataFrame()
-    for ids in pd.read_csv(file, chunksize=10000):
-        ids = ids[[concept_column]].drop_duplicates()
-        ids_final = pd.concat([ids_final, ids])
-        ids_final.drop_duplicates(inplace=True)
-    ids_map = ids_final.reset_index()
-    ids_map['deid_num'] = ids_map.index + 1
-    # assign deid value 0 for unknown input (e.g., provider key < 0)
-    ids_map[concept_id] = ids_map.apply(lambda row: (str(irb) + '_' + concept_cd + '_0') if (int(row[concept_column]) < 0) else (str(irb) + '_' + concept_cd + '_' + str(int(row['deid_num']))), axis=1)
-    if (deid_mode == 'deid' and concept == 'patient'):
-        ids_map['date_shift'] = ids_map.apply(lambda row: random.randint(-30, 30), axis=1)
-    out_file = 'map_{}.csv'.format(concept)
-    ids_map = ids_map.drop(['index'], axis=1)
-    ids_map.to_csv(os.path.join(map_dir, out_file), index=False)
-    return
-
-
-def deid_metadata(deid_mode, note_type, map_dir, notes_dir, disclosure_dir):
-    # define variables
-    text_file = '{}_{}_metadata.csv'.format(cohort, note_type)
-    if (note_type == 'note'):
-        if (deid_mode == 'deid'):
-            final_columns = ['deid_note_id', 'deid_link_note_id', 'ContactNumber', 'ContactDate_shifted', 'CreatedDatetime_shifted', 'ServiceDatetime_shifted', 'deid_pat_id', 'NoteType', 'InpatientNoteType', 'EncounterDate_shifted', 'deid_enc_id', 'deid_authoring_provider_id', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'deid_cosign_provider_id', 'CosignProviderType', 'CosignProviderSpecialty']
-        elif (deid_mode == 'lds'):
-            final_columns = ['deid_note_id', 'deid_link_note_id', 'ContactNumber', 'ContactDate', 'CreatedDatetime', 'ServiceDatetime', 'deid_pat_id', 'NoteType', 'InpatientNoteType', 'EncounterDate', 'deid_enc_id', 'deid_authoring_provider_id', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'deid_cosign_provider_id', 'CosignProviderType', 'CosignProviderSpecialty']
-        elif (deid_mode == 'phi'):
-            final_columns = ['NoteID', 'LinkageNoteID', 'ContactNumber', 'ContactDate', 'CreatedDatetime', 'ServiceDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'InpatientNoteType', 'EncounterDate', 'EncounterCSN', 'AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']
-    elif (note_type == 'order'):
-        if (deid_mode == 'deid'):
-            final_columns = ['deid_order_id', 'Line', 'OrderPlacedDatetime_shifted', 'OrderResultDatetime_shifted', 'deid_pat_id', 'NoteType', 'EncounterDate_shifted', 'deid_enc_id', 'deid_ordering_provider_id', 'OrderingProviderType', 'OrderingProviderSpecialty', 'deid_authorizing_provider_id', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
-        elif (deid_mode == 'lds'):
-            final_columns = ['deid_order_id', 'Line', 'OrderPlacedDatetime', 'OrderResultDatetime', 'deid_pat_id', 'NoteType', 'EncounterDate', 'deid_enc_id', 'deid_ordering_provider_id', 'OrderingProviderType', 'OrderingProviderSpecialty', 'deid_authorizing_provider_id', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
-        elif (deid_mode == 'phi'):
-            final_columns = ['OrderID', 'Line', 'OrderPlacedDatetime', 'OrderResultDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
-    # import mappings
-    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
-    if (deid_mode == 'deid'):
-        map_pat = map_pat[['PatientKey', 'deid_pat_id', 'date_shift']]
-    else:
-        map_pat = map_pat[['PatientKey', 'deid_pat_id']]
-    map_enc = pd.read_csv(os.path.join(map_dir, 'map_encounter.csv'))
-    map_enc = map_enc[['EncounterCSN', 'deid_enc_id']]
-    map_prov = pd.read_csv(os.path.join(map_dir, 'map_provider.csv'))
-    map_prov = map_prov[['ProviderKey', 'deid_provider_id']]
-    if (note_type == 'order'):
-        map_order = pd.read_csv(os.path.join(map_dir, 'map_order.csv'))
-        map_order = map_order[['OrderKey', 'deid_order_id']]
-    elif (note_type == 'note'):
-        map_note = pd.read_csv(os.path.join(map_dir, 'map_note.csv'))
-        map_note = map_note[['NoteKey', 'deid_note_id']]
-        map_linkage_note = pd.read_csv(os.path.join(map_dir, 'map_note_link.csv'))
-        map_linkage_note = map_linkage_note[['LinkageNoteID', 'deid_link_note_id']]
-
-    # merge file with mapping files
-    m = 'w'
-    h = True
-    for df in pd.read_csv(os.path.join(notes_dir, text_file), chunksize=100000):
-        df = pd.merge(df, map_pat, how='left', on='PatientKey')
-        df = df[df['PatientKey'] > 0]
-        df = pd.merge(df, map_enc, how='left', on='EncounterCSN')
-        df = df[df['EncounterKey'] > 0]
-        if (note_type == 'order'):
-            df = pd.merge(df, map_order, how='left', on='OrderKey')
-            df = pd.merge(df, map_prov, how='left', left_on='OrderingProviderKey', right_on='ProviderKey')
-            df = df.rename(columns={"deid_provider_id": "deid_ordering_provider_id"})
-            df = pd.merge(df, map_prov, how='left', left_on='AuthorizingProviderKey', right_on='ProviderKey')
-            df = df.rename(columns={"deid_provider_id": "deid_authorizing_provider_id"})
-        elif (note_type == 'note'):
-            df = pd.merge(df, map_note, how='left', on='NoteKey')
-            df = pd.merge(df, map_linkage_note, how='left', on='LinkageNoteID')
-            df = pd.merge(df, map_prov, how='left', left_on='AuthoringProviderKey', right_on='ProviderKey')
-            df = df.rename(columns={"deid_provider_id": "deid_authoring_provider_id"})
-            df = pd.merge(df, map_prov, how='left', left_on='CosignProviderKey', right_on='ProviderKey')
-            df = df.rename(columns={"deid_provider_id": "deid_cosign_provider_id"})
-        if (deid_mode == 'deid'):
-            if (note_type == 'note'):
-                df['ContactDate'] = pd.to_datetime(df['ContactDate'])
-                df['ContactDate'] = df['ContactDate'].fillna('0')
-                df['CreatedDatetime'] = pd.to_datetime(df['CreatedDatetime'])
-                df['CreatedDatetime'] = df['CreatedDatetime'].fillna('0')
-                df['ServiceDatetime'] = pd.to_datetime(df['ServiceDatetime'])
-                df['ServiceDatetime'] = df['ServiceDatetime'].fillna('0')
-                df['EncounterDate'] = pd.to_datetime(df['EncounterDate'])
-                df['EncounterDate'] = df['EncounterDate'].fillna('0')
-                df['ContactDate_shifted'] = df.apply(lambda row: row['ContactDate'] + timedelta(days=row['date_shift']) if row['ContactDate'] != '0' else '', axis=1)
-                df['CreatedDatetime_shifted'] = df.apply(lambda row: row['CreatedDatetime'] + timedelta(days=row['date_shift']) if row['CreatedDatetime'] != '0' else '', axis=1)
-                df['ServiceDatetime_shifted'] = df.apply(lambda row: row['ServiceDatetime'] + timedelta(days=row['date_shift']) if row['ServiceDatetime'] != '0' else '', axis=1)
-                df['EncounterDate_shifted'] = df.apply(lambda row: row['EncounterDate'] + timedelta(days=row['date_shift']) if row['EncounterDate'] != '0' else '', axis=1)
-            elif (note_type == 'order'):
-                df['OrderPlacedDatetime'] = pd.to_datetime(df['OrderPlacedDatetime'])
-                df['OrderPlacedDatetime'] = df['OrderPlacedDatetime'].fillna('0')
-                df['OrderResultDatetime'] = pd.to_datetime(df['OrderResultDatetime'])
-                df['OrderResultDatetime'] = df['OrderResultDatetime'].fillna('0')
-                df['EncounterDate'] = pd.to_datetime(df['EncounterDate'])
-                df['EncounterDate'] = df['EncounterDate'].fillna('0')
-                df['OrderPlacedDatetime_shifted'] = df.apply(lambda row: row['OrderPlacedDatetime'] + timedelta(days=row['date_shift']) if row['OrderPlacedDatetime'] != '0' else '', axis=1)
-                df['OrderResultDatetime_shifted'] = df.apply(lambda row: row['OrderResultDatetime'] + timedelta(days=row['date_shift']) if row['OrderResultDatetime'] != '0' else '', axis=1)
-                df['EncounterDate_shifted'] = df.apply(lambda row: row['EncounterDate'] + timedelta(days=row['date_shift']) if row['EncounterDate'] != '0' else '', axis=1)
-        df = df[final_columns]
-        df.to_csv(os.path.join(disclosure_dir, text_file), index=False, mode=m, header=h)
-        m = 'a'
-        h = False
-    return
-
-
-def deid_tsv_note(map_dir, notes_dir, logger: Logger):
-    map_note_link = pd.read_csv(os.path.join(map_dir, 'map_note_link.csv'))
-    for file_prefix in ['note']:
-        # find all files with specified prefix in the name
-        pattern = file_prefix + '_.*.tsv'
-        in_dir = os.path.join(notes_dir, '{}_{}'.format(cohort, file_prefix))
-        final_columns = ['deid_link_note_id', 'note_text']
-        items = [f for f in os.listdir(in_dir) if re.match(pattern, f)]
-        for file in items:
-            logger.info(f"""Processing `file` "{file}".""")
-            out_file = 'deid_{}'.format(file)
-            m = 'w'
-            h = True
-            for df in pd.read_csv(os.path.join(in_dir, file), chunksize=100000, sep='\t'):
-                df = pd.merge(df, map_note_link, how='left', on='LinkageNoteID')
-                df = df[final_columns]
-                df.to_csv(os.path.join(in_dir, out_file), index=False, sep='\t', mode=m, header=h)
-                m = 'a'
-                h = False
-    return
-
-
-def deid_tsv_order(map_dir, notes_dir, logger: Logger):
-    map_order = pd.read_csv(os.path.join(map_dir, 'map_order.csv'))
-    for file_prefix in ['order_narrative', 'order_impression', 'order_result_comment']:
-        # find all files with specified prefix in the name
-        pattern = file_prefix + '_.*.tsv'
-        in_dir = os.path.join(notes_dir, '{}_{}'.format(cohort, file_prefix))
-        if (file_prefix == 'order_result_comment'):
-            final_columns = ['deid_order_id', 'LINE', 'note_text']
-        else:
-            final_columns = ['deid_order_id', 'note_text']
-        items = [f for f in os.listdir(in_dir) if re.match(pattern, f)]
-        for file in items:
-            logger.info(f"""    Processing `file` "{file}".""")
-            out_file = 'deid_{}'.format(file)
-            m = 'w'
-            h = True
-            for df in pd.read_csv(os.path.join(in_dir, file), chunksize=100000, sep='\t'):
-                df = pd.merge(df, map_order, how='left', on='OrderKey')
-                df = df[final_columns]
-                df.to_csv(os.path.join(in_dir, out_file), index=False, sep='\t', mode=m, header=h)
-                m = 'a'
-                h = False
-    return
-
-
-def format_metadata_files(note_type, notes_dir, disclosure_dir):
-    # define variables
-    text_file = '{}_{}_metadata.csv'.format(cohort, note_type)
-    if (note_type == 'note'):
-        final_columns = ['NoteID', 'LinkageNoteID', 'ContactNumber', 'ContactDate', 'CreatedDatetime', 'ServiceDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'InpatientNoteType', 'EncounterDate', 'EncounterCSN', 'AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']
-    elif (note_type == 'order'):
-        final_columns = ['OrderID', 'Line', 'OrderPlacedDatetime', 'OrderResultDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
-    # read and format the file
-    m = 'w'
-    h = True
-    for df in pd.read_csv(os.path.join(notes_dir, text_file), chunksize=100000):
-        df = df[final_columns]
-        df.to_csv(os.path.join(disclosure_dir, text_file), index=False, mode=m, header=h)
-        m = 'a'
-        h = False
-    return
-
-
-def copy_tsv(cohort, notes_dir, disclosure_dir):
-    for item in ['note', 'order_narrative', 'order_impression', 'order_result_comment']:
-        dir = cohort + '_' + item
-        if (os.path.exists(os.path.join(notes_dir, dir))):
-            file_list = [f for f in os.listdir(os.path.join(notes_dir, dir))]
-            for f in file_list:
-                shutil.copy(os.path.join(os.path.join(notes_dir, dir, f)), os.path.join(os.path.join(disclosure_dir, f)))
-    return
-
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `COHORT_NAME`: "{COHORT_NAME}"
-    `COHORT_FILE`: "{COHORT_FILE}"
-    `IRB_NUMBER`: "{IRB_NUMBER}"
-    `ID_TYPE`: "{ID_TYPE}"
-    `NOTE_VERSION`: "{NOTE_VERSION}"
-    `DE_IDENTIFICATION_MODE`: "{DE_IDENTIFICATION_MODE}"
-    `SQL_ENCOUNTER_EFFECTIVE_DATE_START`: "{SQL_ENCOUNTER_EFFECTIVE_DATE_START}"
-    `SQL_ENCOUNTER_EFFECTIVE_DATE_END`: "{SQL_ENCOUNTER_EFFECTIVE_DATE_END}"
-
-    # Arguments: SQL connection settings
-    `USE_WINDOWS_AUTHENTICATION` : "{USE_WINDOWS_AUTHENTICATION}"
-    `SERVER`                     : "{SERVER}"
-    `DATABASE_PROD`              : "{DATABASE_PROD}"
-    `DATABASE_NOTES`             : "{DATABASE_NOTES}"
-    `USERDOMAIN`                 : "{USERDOMAIN}"
-    `USERNAME`                   : "{USERNAME}"
-    `UID`                        : "{UID}"
-    `PWD`                        : censored
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-    """)
-    logger.info(f"""`base_dir` set to "{base_dir}".""")
-
-    # pull metadata
-    pull_metadata(note_version, id_type, 'note', sql_dir, data_dir, notes_dir, cohort, logger)
-    pull_metadata(note_version, id_type, 'order_narrative', sql_dir, data_dir, notes_dir, cohort, logger)
-    pull_metadata(note_version, id_type, 'order_impression', sql_dir, data_dir, notes_dir, cohort, logger)
-    pull_metadata(note_version, id_type, 'order_result_comment', sql_dir, data_dir, notes_dir, cohort, logger)
-
-    # split metadata into chunks, so that we can process data in chunks
-    split_metadata('note', notes_dir, cohort, logger)
-    split_metadata('order_narrative', notes_dir, cohort, logger)
-    split_metadata('order_impression', notes_dir, cohort, logger)
-    split_metadata('order_result_comment', notes_dir, cohort, logger)
-
-    # pull text in parallel
-    pull_text_in_parallel('note', sql_dir, notes_dir, cohort, logger)
-    pull_text_in_parallel('order_narrative', sql_dir, notes_dir, cohort, logger)
-    pull_text_in_parallel('order_impression', sql_dir, notes_dir, cohort, logger)
-    pull_text_in_parallel('order_result_comment', sql_dir, notes_dir, cohort, logger)
-    if (deid_mode == 'phi'):
-
-        # copy note_metadata file to disclosure folder
-        format_metadata_files('note', notes_dir, disclosure_dir)
-
-        # combine all order metadata files and copy to discosure folder
-        combine_order_metadata(notes_dir, cohort)
-        format_metadata_files('order', notes_dir, disclosure_dir)
-
-        # copy .tsv files with free text
-        copy_tsv(cohort, notes_dir, disclosure_dir)
-    else:
-        # generate mappings
-        generate_map(deid_mode, data_dir, map_dir, 'patient', cohort)
-        generate_map(deid_mode, notes_dir, map_dir, 'encounter', cohort)
-        generate_map(deid_mode, notes_dir, map_dir, 'note', cohort)
-        generate_map(deid_mode, notes_dir, map_dir, 'note_link', cohort)
-        generate_map(deid_mode, notes_dir, map_dir, 'order', cohort)
-        generate_map(deid_mode, notes_dir, map_dir, 'provider', cohort)
-
-        # deidentify metadata. We can create deidentified dataset or limited dataset.
-        deid_metadata(deid_mode, 'note', map_dir, notes_dir, disclosure_dir)
-        deid_metadata(deid_mode, 'order', map_dir, notes_dir, disclosure_dir)
-
-        # prepare for text deidentification, i.e., deidentify ID in .tsv file(s)
-        deid_tsv_note(map_dir, notes_dir, logger)
-        deid_tsv_order(map_dir, notes_dir, logger)
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
+from __future__ import annotations
+
+import concurrent.futures
+import logging
+import os
+import random
+import re
+import shutil
+from datetime import timedelta
+from logging import Logger
+from pathlib import Path
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from _typeshed.dbapi import DBAPIConnection
+# Third-party packages
+import pandas as pd
+import pymssql
+import sqlalchemy as sa
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    replace_sql_query,
+                                    successiveParents)
+
+# Arguments: Script settings
+COHORT_NAME = "SGMCPLGB"                                    # An arbitrary name used in file names
+COHORT_FILE = "cohort.csv"                                    # A file name that is located directory specified by the variable `data_dir`
+IRB_NUMBER = "IRB201902162"                                     # Used for creating the de-identification map IDs.
+ID_TYPE = "PatientKey"                                        # Pick from "EncounterCSN", "EncounterKey", or "PatientKey". Choose the ID type you used in `COHORT_FILE`
+NOTE_VERSION = "all"                                   # Pick from "all", or "last"
+DE_IDENTIFICATION_MODE = "phi"                         # Pick from "deid", "lds", or "phi"
+LOG_LEVEL = "DEBUG"                                      # See the "logging" module for valid values for the `loglevel` parameter.
+SQL_ENCOUNTER_EFFECTIVE_DATE_START = '2011-06-01'   # The beginning of date range of encounters to collect. Format: YYYY-MM-DD
+SQL_ENCOUNTER_EFFECTIVE_DATE_END = '2023-12-31'     # The end of date range of encounters to collect. Format: YYYY-MM-DD
+
+# Arguments: SQL connection settings
+USE_WINDOWS_AUTHENTICATION = True
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE_PROD = "DWS_PROD"
+DATABASE_NOTES = "DWS_NOTES"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "PROJECT_OR_PORTION_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path Construction: Project-specific
+notes_dir = runOutputDir.joinpath('free_text')  # all notes related files are saved in 'notes' subdirectory of 'data' directory
+map_dir = runOutputDir.joinpath('mapping')  # mappings are saved in 'mapping' subdirectory of 'data' folder.
+disclosure_dir = runOutputDir.joinpath('disclosure')
+
+# Variables: Map legacy variables to DRAPI-LEMUR standard variables: Script settings
+cohort = COHORT_NAME
+id_type = ID_TYPE
+note_version = NOTE_VERSION
+irb = IRB_NUMBER
+deid_mode = DE_IDENTIFICATION_MODE
+
+# Variables: Map legacy variables to DRAPI-LEMUR standard variables: Path construction
+base_dir = str(projectDir)
+data_dir = dataDir
+sql_dir = sqlDir
+
+# Variables: Map legacy variables to DRAPI-LEMUR standard variables: SQL Parameters
+host = SERVER
+database_prod = DATABASE_PROD
+database_notes = DATABASE_NOTES
+
+# Variables: SQL connection settings
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Directory creation: Project-specific
+for dir in [data_dir, sql_dir, notes_dir, disclosure_dir]:
+    makeDirPath(dir)
+if DE_IDENTIFICATION_MODE.lower() == "phi":
+    pass
+elif DE_IDENTIFICATION_MODE.lower() in ["deid", "lds"]:
+    makeDirPath(map_dir)
+else:
+    raise Exception(f"Unexpected value for `DE_IDENTIFICATION_MODE`: {DE_IDENTIFICATION_MODE}.")
+
+# Functions
+
+
+def connectToDatabase(host: str,
+                      database: str,
+                      useWindowsAuthentication=True) -> DBAPIConnection:
+    """
+    Connects to a SQL database given a `host` (server) and `database` value.
+    """
+    if useWindowsAuthentication:
+        connection = pymssql.connect(host=host,
+                                     database=database)
+    else:
+        conStr = f"mssql+pymssql://{uid}:{PWD}@{host}/{database}"
+        connection = sa.create_engine(conStr).connect()
+    return connection
+
+
+def executeQuery(query: str, host: str, database: str) -> pd.DataFrame:
+    """
+    Executes a SQL query.
+    INPUT:
+        `query`: a string
+        `host`: a string
+        `databse`: a string
+    OUTPUT:
+        A pandas dataframe object.
+    """
+    databaseConnection = connectToDatabase(host, database)
+    queryResult = pd.read_sql(query, databaseConnection)
+    databaseConnection.close()
+    return queryResult
+
+
+# notes methods
+
+
+def pull_metadata(note_version, id_type, note_type, sql_dir, cohort_dir, notes_dir, cohort, logger: Logger):
+    logger.info(f"""Function arguments:
+    `note_version`: {note_version}
+    `id_type`:      {id_type}
+    `note_type`:    {note_type}
+    `sql_dir`:      {sql_dir}
+    `cohort_dir`:   {cohort_dir}
+    `notes_dir`:    {notes_dir}
+    `cohort`:       {cohort}
+    `logger`:       {logger}""")
+    m = 'w'  # mode of the output file
+    h = True  # header of the output file
+    counter = 1  # used only for tracking/time estimation purposes
+    if (id_type == 'PatientKey'):
+        in_file = COHORT_FILE
+    elif (id_type == 'EncounterCSN' or id_type == 'EncounterKey'):
+        in_file = COHORT_FILE
+    for df in pd.read_csv(os.path.join(cohort_dir, in_file), chunksize=1000, engine='python'):
+        df = df[[id_type]]
+        id_str = df[id_type].unique().tolist()
+        logger.info(f"  This chunk of your input file containing patient or encounter ID's is of length {len(id_str):,}.")
+        id_str = "','".join(str(x) for x in id_str)
+        id_str = "'" + id_str + "'"
+        query_file = note_type + '_metadata.sql'
+        logger.info(f"Reading query file: {query_file}")
+        fpath = os.path.join(sql_dir, query_file)
+        with open(fpath, "r") as file:
+            query = file.read()
+        query = replace_sql_query(query, "XXXXX", id_str)
+        query = replace_sql_query(query, "{PYTHON_VARIABLE: SQL_ENCOUNTER_EFFECTIVE_DATE_START}", SQL_ENCOUNTER_EFFECTIVE_DATE_START)
+        query = replace_sql_query(query, "{PYTHON_VARIABLE: SQL_ENCOUNTER_EFFECTIVE_DATE_END}", SQL_ENCOUNTER_EFFECTIVE_DATE_END)
+
+        logger.log(9, f"Using the following query:\n>>> Begin query >>>\n{query}\n<<< End query <<<")
+        result = executeQuery(query=query,
+                              host=host,
+                              database=database_prod)
+
+        logger.info(f"The chunk query has {len(result):,} rows.")
+        result = result.drop_duplicates()
+
+        logger.info(f"After dropping duplicates, the chunk query has {len(result):,} rows.")
+        if (note_type == 'note' and note_version == 'last'):  # keep only the last version of the note
+            result = result.sort_values(by=['NoteKey', 'ContactNumber'], ascending=[True, False])
+            result = result.drop_duplicates(['NoteKey'])
+        result_file = cohort + '_' + note_type + '_metadata.csv'
+        result.to_csv(os.path.join(notes_dir, result_file), index=False, mode=m, header=h)
+        m = 'a'
+        h = False
+        logger.info(f'Completed chunk {counter}')
+        counter = counter + 1
+    return
+
+
+def split_metadata(note_type, notes_dir, cohort, logger: Logger):
+    in_file = cohort + '_' + note_type + '_metadata.csv'
+    file_count = 1
+    for df in pd.read_csv(os.path.join(notes_dir, in_file), chunksize=1000000):
+        out_file = cohort + '_' + note_type + '_metadata_' + str(file_count) + '.csv'
+
+        logger.info(f"Working on file {file_count}.")
+        # ensure that all ID columns are integers
+        columns = df.columns
+        for c in ['NoteKey', 'NoteID', 'LinkageNoteID', 'OrderKey', 'OrderID', 'PatientKey', 'EncounterKey', 'EncounterCSN', 'AuthoringProviderKey', 'CosignProviderKey', 'OrderingProviderKey', 'AuthorizingProviderKey']:
+            if (c in columns):
+                # fill missing values with 0 since 0 is never used for these IDs in reality
+                df[c] = df[c].fillna(0)
+                # use string instead of int type since some fields, such as EncounterCSN, are bigger than what python considers an integer
+                df[c] = df.apply(lambda row: str(row[c]).split('.0')[0], axis=1)
+        df.to_csv(os.path.join(notes_dir, out_file), index=False)
+        file_count = file_count + 1
+    return
+
+
+def pull_text(item, note_type, note_id, sql_dir, notes_dir, dir_final, logger: Logger):
+    logger.info(f"""Processing item "{item}".""")
+    # Pull text
+    header = True  # header of the output file
+    mode = 'w'  # mode of the output file
+    for notes in pd.read_csv(os.path.join(notes_dir, item), chunksize=10000, engine='python'):
+        note_list = notes[note_id].unique().tolist()
+        note_list = ",".join(str(int(x)) for x in note_list)
+        query_file = note_type + '_text.sql'
+        query_file = os.path.join(sql_dir, query_file)
+        fpath = os.path.join(sql_dir, query_file)
+        with open(fpath, "r") as file:
+            query = file.read()
+        query = replace_sql_query(query, "XXXXX", note_list)
+        result = executeQuery(query=query,
+                              host=host,
+                              database=database_notes)
+        # ensure that all ID columns are integers
+        columns = result.columns
+        for c in ['LinkageNoteID', 'OrderKey']:
+            if (c in columns):
+                # fill missing values with 0 since 0 is never used for these IDs in reality
+                result[c] = result[c].fillna(0)
+                # use string instead of int type since some fields, such as EncounterCSN, are bigger than what python considers an integer
+                result[c] = result.apply(lambda row: str(row[c]).split('.0')[0], axis=1)
+        file_count = item.split('.csv')[0].split('_')[-1]
+        file_out = note_type + '_' + str(file_count) + '.tsv'
+        result.to_csv(os.path.join(dir_final, file_out), header=header, mode=mode, sep='\t', encoding="UTF-8", index=False)
+        header = False
+        mode = 'a'
+    return
+
+
+def pull_text_in_parallel(note_type, sql_dir, notes_dir, cohort, logger: Logger):
+    # Prepare for text pull
+    if (note_type == 'note'):
+        dir_final = os.path.join(notes_dir, cohort + '_note')
+        if (not os.path.exists(dir_final)):
+            os.makedirs(dir_final)
+        note_id = 'LinkageNoteID'
+    elif (note_type == 'order_narrative'):
+        dir_final = os.path.join(notes_dir, cohort + '_order_narrative')
+        if (not os.path.exists(dir_final)):
+            os.makedirs(dir_final)
+        note_id = 'OrderKey'
+    elif (note_type == 'order_impression'):
+        dir_final = os.path.join(notes_dir, cohort + '_order_impression')
+        if (not os.path.exists(dir_final)):
+            os.makedirs(dir_final)
+        note_id = 'OrderKey'
+    elif (note_type == 'order_result_comment'):
+        dir_final = os.path.join(notes_dir, cohort + '_order_result_comment')
+        if (not os.path.exists(dir_final)):
+            os.makedirs(dir_final)
+        note_id = 'OrderKey'
+    # identify all metadata files for specific note type
+    pattern = cohort + '_' + note_type + '_metadata_.*.csv'  # hot fix 2022-05-10
+    items = [f for f in os.listdir(notes_dir) if re.match(pattern, f)]
+    logger.info(f"""This is the list of items that matched the criteria for processing: {items}.""")
+    # start pullng text. By default, number of parallel threads is set to 4.
+    with concurrent.futures.ThreadPoolExecutor(max_workers=4) as executor:
+        result_futures = {executor.submit(pull_text, item, note_type, note_id, sql_dir, notes_dir, dir_final, logger): item for item in items}
+        for future in concurrent.futures.as_completed(result_futures):
+            item = result_futures[future]
+            try:
+                _ = future.result()
+                logger.info(f"""Completed item "{item}".""")
+            except Exception as e:
+                logger.info(f"""An exception was generated by item "{item}": "{e}".""")
+    return
+
+
+def combine_order_metadata(notes_dir, cohort):
+    m = 'w'
+    h = True
+    for file1 in ['order_narrative', 'order_impression', 'order_result_comment']:
+        file = cohort + '_' + file1 + '_metadata.csv'
+        if os.path.exists(os.path.join(notes_dir, file)):
+            df = pd.read_csv(os.path.join(notes_dir, file))
+            if (file1 in ['order_narrative', 'order_impression']):
+                df['Line'] = ''
+            df = df[['OrderKey', 'Line', 'OrderID', 'OrderPlacedDatetime', 'OrderResultDatetime', 'PatientKey', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterKey', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
+            df.to_csv(os.path.join(notes_dir, '{}_order_metadata.csv'.format(cohort)), index=False, mode=m, header=h)
+            m = 'a'
+            h = False
+    return
+
+
+def create_encounters(notes_dir):
+    df = pd.DataFrame()
+    for file in ['{}_order_narrative_metadata.csv'.format(cohort), '{}_order_impression_metadata.csv'.format(cohort), '{}_order_result_comment_metadata.csv'.format(cohort), '{}_note_metadata.csv'.format(cohort)]:
+        for dfx in pd.read_csv(os.path.join(notes_dir, file), chunksize=100000):
+            df1 = dfx[['EncounterCSN']].drop_duplicates()
+            df = pd.concat([df, df1])
+            df.drop_duplicates(inplace=True)
+    df.to_csv(os.path.join(notes_dir, 'encounters.csv'), index=False)
+    return
+
+
+def create_provider_metadata(notes_dir, cohort):
+    m = 'w'
+    h = True
+    df = pd.DataFrame()
+    for file1 in ['order_narrative', 'order_impression', 'order_result_comment', 'note']:
+        # for file in ['note']:
+        file = cohort + '_' + file1 + '_metadata.csv'
+        if os.path.exists(os.path.join(notes_dir, file)):
+            for dfx in pd.read_csv(os.path.join(notes_dir, file), chunksize=100000):
+                if (file1 in ['order_narrative', 'order_impression', 'order_result_comment']):
+                    df1 = dfx[['OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty']]
+                    df1 = df1.rename(columns={"OrderingProviderKey": "ProviderKey", "OrderingProviderType": "ProviderType", "OrderingProviderSpecialty": "ProviderSpecialty"})
+                    df2 = dfx[['AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
+                    df2 = df2.rename(columns={"AuthorizingProviderKey": "ProviderKey", "AuthorizingProviderType": "ProviderType", "AuthorizingProviderSpecialty": "ProviderSpecialty"})
+                elif (file1 in ['note']):
+                    df1 = dfx[['AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty']]
+                    df1 = df1.rename(columns={"AuthoringProviderKey": "ProviderKey", "AuthoringProviderType": "ProviderType", "AuthoringProviderSpecialty": "ProviderSpecialty"})
+                    df2 = dfx[['CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']]
+                    df2 = df2.rename(columns={"CosignProviderKey": "ProviderKey", "CosignProviderType": "ProviderType", "CosignProviderSpecialty": "ProviderSpecialty"})
+                df1 = pd.concat([df1, df2])
+                df1.drop_duplicates(inplace=True)
+                df = pd.concat([df, df1])
+                df.drop_duplicates(inplace=True)
+            df.to_csv(os.path.join(notes_dir, 'provider_metadata.csv'), index=False, mode=m, header=h)
+            m = 'a'
+            h = False
+    return
+
+
+def generate_map(deid_mode, in_dir, map_dir, concept, cohort):
+    """
+    `concept` can be any of the following values:
+        - patient
+        - encounter
+        - note
+        - note_link
+        - order
+        - provider
+    """
+    # define variables
+    if (concept == 'patient'):
+        concept_cd = 'PAT'
+        concept_id = 'deid_pat_id'
+        file = os.path.join(in_dir, COHORT_FILE)  # NOTE
+        concept_column = 'PatientKey'
+    elif (concept == 'encounter'):
+        concept_cd = 'ENC'
+        concept_id = 'deid_enc_id'
+        create_encounters(in_dir)
+        file = os.path.join(in_dir, 'encounters.csv')
+        concept_column = 'EncounterCSN'
+    elif (concept == 'note'):
+        concept_cd = 'NOTE'
+        concept_id = 'deid_note_id'
+        file = os.path.join(in_dir, '{}_note_metadata.csv'.format(cohort))
+        concept_column = 'NoteKey'
+    elif (concept == 'note_link'):
+        concept_cd = 'LINK_NOTE'
+        concept_id = 'deid_link_note_id'
+        file = os.path.join(in_dir, '{}_note_metadata.csv'.format(cohort))
+        concept_column = 'LinkageNoteID'
+    elif (concept == 'order'):
+        concept_cd = 'ORDER'
+        concept_id = 'deid_order_id'
+        combine_order_metadata(in_dir, cohort)
+        file = os.path.join(in_dir, '{}_order_metadata.csv'.format(cohort))
+        concept_column = 'OrderKey'
+    elif (concept == 'provider'):
+        concept_cd = 'PROV'
+        concept_id = 'deid_provider_id'
+        create_provider_metadata(in_dir, cohort)
+        file = os.path.join(in_dir, 'provider_metadata.csv')
+        concept_column = 'ProviderKey'
+    else:
+        logging.error(f"""Nonexisting concept in `generate_map` method: "{concept}".""")
+
+    ids_final = pd.DataFrame()
+    for ids in pd.read_csv(file, chunksize=10000):
+        ids = ids[[concept_column]].drop_duplicates()
+        ids_final = pd.concat([ids_final, ids])
+        ids_final.drop_duplicates(inplace=True)
+    ids_map = ids_final.reset_index()
+    ids_map['deid_num'] = ids_map.index + 1
+    # assign deid value 0 for unknown input (e.g., provider key < 0)
+    ids_map[concept_id] = ids_map.apply(lambda row: (str(irb) + '_' + concept_cd + '_0') if (int(row[concept_column]) < 0) else (str(irb) + '_' + concept_cd + '_' + str(int(row['deid_num']))), axis=1)
+    if (deid_mode == 'deid' and concept == 'patient'):
+        ids_map['date_shift'] = ids_map.apply(lambda row: random.randint(-30, 30), axis=1)
+    out_file = 'map_{}.csv'.format(concept)
+    ids_map = ids_map.drop(['index'], axis=1)
+    ids_map.to_csv(os.path.join(map_dir, out_file), index=False)
+    return
+
+
+def deid_metadata(deid_mode, note_type, map_dir, notes_dir, disclosure_dir):
+    # define variables
+    text_file = '{}_{}_metadata.csv'.format(cohort, note_type)
+    if (note_type == 'note'):
+        if (deid_mode == 'deid'):
+            final_columns = ['deid_note_id', 'deid_link_note_id', 'ContactNumber', 'ContactDate_shifted', 'CreatedDatetime_shifted', 'ServiceDatetime_shifted', 'deid_pat_id', 'NoteType', 'InpatientNoteType', 'EncounterDate_shifted', 'deid_enc_id', 'deid_authoring_provider_id', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'deid_cosign_provider_id', 'CosignProviderType', 'CosignProviderSpecialty']
+        elif (deid_mode == 'lds'):
+            final_columns = ['deid_note_id', 'deid_link_note_id', 'ContactNumber', 'ContactDate', 'CreatedDatetime', 'ServiceDatetime', 'deid_pat_id', 'NoteType', 'InpatientNoteType', 'EncounterDate', 'deid_enc_id', 'deid_authoring_provider_id', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'deid_cosign_provider_id', 'CosignProviderType', 'CosignProviderSpecialty']
+        elif (deid_mode == 'phi'):
+            final_columns = ['NoteID', 'LinkageNoteID', 'ContactNumber', 'ContactDate', 'CreatedDatetime', 'ServiceDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'InpatientNoteType', 'EncounterDate', 'EncounterCSN', 'AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']
+    elif (note_type == 'order'):
+        if (deid_mode == 'deid'):
+            final_columns = ['deid_order_id', 'Line', 'OrderPlacedDatetime_shifted', 'OrderResultDatetime_shifted', 'deid_pat_id', 'NoteType', 'EncounterDate_shifted', 'deid_enc_id', 'deid_ordering_provider_id', 'OrderingProviderType', 'OrderingProviderSpecialty', 'deid_authorizing_provider_id', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
+        elif (deid_mode == 'lds'):
+            final_columns = ['deid_order_id', 'Line', 'OrderPlacedDatetime', 'OrderResultDatetime', 'deid_pat_id', 'NoteType', 'EncounterDate', 'deid_enc_id', 'deid_ordering_provider_id', 'OrderingProviderType', 'OrderingProviderSpecialty', 'deid_authorizing_provider_id', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
+        elif (deid_mode == 'phi'):
+            final_columns = ['OrderID', 'Line', 'OrderPlacedDatetime', 'OrderResultDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
+    # import mappings
+    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
+    if (deid_mode == 'deid'):
+        map_pat = map_pat[['PatientKey', 'deid_pat_id', 'date_shift']]
+    else:
+        map_pat = map_pat[['PatientKey', 'deid_pat_id']]
+    map_enc = pd.read_csv(os.path.join(map_dir, 'map_encounter.csv'))
+    map_enc = map_enc[['EncounterCSN', 'deid_enc_id']]
+    map_prov = pd.read_csv(os.path.join(map_dir, 'map_provider.csv'))
+    map_prov = map_prov[['ProviderKey', 'deid_provider_id']]
+    if (note_type == 'order'):
+        map_order = pd.read_csv(os.path.join(map_dir, 'map_order.csv'))
+        map_order = map_order[['OrderKey', 'deid_order_id']]
+    elif (note_type == 'note'):
+        map_note = pd.read_csv(os.path.join(map_dir, 'map_note.csv'))
+        map_note = map_note[['NoteKey', 'deid_note_id']]
+        map_linkage_note = pd.read_csv(os.path.join(map_dir, 'map_note_link.csv'))
+        map_linkage_note = map_linkage_note[['LinkageNoteID', 'deid_link_note_id']]
+
+    # merge file with mapping files
+    m = 'w'
+    h = True
+    for df in pd.read_csv(os.path.join(notes_dir, text_file), chunksize=100000):
+        df = pd.merge(df, map_pat, how='left', on='PatientKey')
+        df = df[df['PatientKey'] > 0]
+        df = pd.merge(df, map_enc, how='left', on='EncounterCSN')
+        df = df[df['EncounterKey'] > 0]
+        if (note_type == 'order'):
+            df = pd.merge(df, map_order, how='left', on='OrderKey')
+            df = pd.merge(df, map_prov, how='left', left_on='OrderingProviderKey', right_on='ProviderKey')
+            df = df.rename(columns={"deid_provider_id": "deid_ordering_provider_id"})
+            df = pd.merge(df, map_prov, how='left', left_on='AuthorizingProviderKey', right_on='ProviderKey')
+            df = df.rename(columns={"deid_provider_id": "deid_authorizing_provider_id"})
+        elif (note_type == 'note'):
+            df = pd.merge(df, map_note, how='left', on='NoteKey')
+            df = pd.merge(df, map_linkage_note, how='left', on='LinkageNoteID')
+            df = pd.merge(df, map_prov, how='left', left_on='AuthoringProviderKey', right_on='ProviderKey')
+            df = df.rename(columns={"deid_provider_id": "deid_authoring_provider_id"})
+            df = pd.merge(df, map_prov, how='left', left_on='CosignProviderKey', right_on='ProviderKey')
+            df = df.rename(columns={"deid_provider_id": "deid_cosign_provider_id"})
+        if (deid_mode == 'deid'):
+            if (note_type == 'note'):
+                df['ContactDate'] = pd.to_datetime(df['ContactDate'])
+                df['ContactDate'] = df['ContactDate'].fillna('0')
+                df['CreatedDatetime'] = pd.to_datetime(df['CreatedDatetime'])
+                df['CreatedDatetime'] = df['CreatedDatetime'].fillna('0')
+                df['ServiceDatetime'] = pd.to_datetime(df['ServiceDatetime'])
+                df['ServiceDatetime'] = df['ServiceDatetime'].fillna('0')
+                df['EncounterDate'] = pd.to_datetime(df['EncounterDate'])
+                df['EncounterDate'] = df['EncounterDate'].fillna('0')
+                df['ContactDate_shifted'] = df.apply(lambda row: row['ContactDate'] + timedelta(days=row['date_shift']) if row['ContactDate'] != '0' else '', axis=1)
+                df['CreatedDatetime_shifted'] = df.apply(lambda row: row['CreatedDatetime'] + timedelta(days=row['date_shift']) if row['CreatedDatetime'] != '0' else '', axis=1)
+                df['ServiceDatetime_shifted'] = df.apply(lambda row: row['ServiceDatetime'] + timedelta(days=row['date_shift']) if row['ServiceDatetime'] != '0' else '', axis=1)
+                df['EncounterDate_shifted'] = df.apply(lambda row: row['EncounterDate'] + timedelta(days=row['date_shift']) if row['EncounterDate'] != '0' else '', axis=1)
+            elif (note_type == 'order'):
+                df['OrderPlacedDatetime'] = pd.to_datetime(df['OrderPlacedDatetime'])
+                df['OrderPlacedDatetime'] = df['OrderPlacedDatetime'].fillna('0')
+                df['OrderResultDatetime'] = pd.to_datetime(df['OrderResultDatetime'])
+                df['OrderResultDatetime'] = df['OrderResultDatetime'].fillna('0')
+                df['EncounterDate'] = pd.to_datetime(df['EncounterDate'])
+                df['EncounterDate'] = df['EncounterDate'].fillna('0')
+                df['OrderPlacedDatetime_shifted'] = df.apply(lambda row: row['OrderPlacedDatetime'] + timedelta(days=row['date_shift']) if row['OrderPlacedDatetime'] != '0' else '', axis=1)
+                df['OrderResultDatetime_shifted'] = df.apply(lambda row: row['OrderResultDatetime'] + timedelta(days=row['date_shift']) if row['OrderResultDatetime'] != '0' else '', axis=1)
+                df['EncounterDate_shifted'] = df.apply(lambda row: row['EncounterDate'] + timedelta(days=row['date_shift']) if row['EncounterDate'] != '0' else '', axis=1)
+        df = df[final_columns]
+        df.to_csv(os.path.join(disclosure_dir, text_file), index=False, mode=m, header=h)
+        m = 'a'
+        h = False
+    return
+
+
+def deid_tsv_note(map_dir, notes_dir, logger: Logger):
+    map_note_link = pd.read_csv(os.path.join(map_dir, 'map_note_link.csv'))
+    for file_prefix in ['note']:
+        # find all files with specified prefix in the name
+        pattern = file_prefix + '_.*.tsv'
+        in_dir = os.path.join(notes_dir, '{}_{}'.format(cohort, file_prefix))
+        final_columns = ['deid_link_note_id', 'note_text']
+        items = [f for f in os.listdir(in_dir) if re.match(pattern, f)]
+        for file in items:
+            logger.info(f"""Processing `file` "{file}".""")
+            out_file = 'deid_{}'.format(file)
+            m = 'w'
+            h = True
+            for df in pd.read_csv(os.path.join(in_dir, file), chunksize=100000, sep='\t'):
+                df = pd.merge(df, map_note_link, how='left', on='LinkageNoteID')
+                df = df[final_columns]
+                df.to_csv(os.path.join(in_dir, out_file), index=False, sep='\t', mode=m, header=h)
+                m = 'a'
+                h = False
+    return
+
+
+def deid_tsv_order(map_dir, notes_dir, logger: Logger):
+    map_order = pd.read_csv(os.path.join(map_dir, 'map_order.csv'))
+    for file_prefix in ['order_narrative', 'order_impression', 'order_result_comment']:
+        # find all files with specified prefix in the name
+        pattern = file_prefix + '_.*.tsv'
+        in_dir = os.path.join(notes_dir, '{}_{}'.format(cohort, file_prefix))
+        if (file_prefix == 'order_result_comment'):
+            final_columns = ['deid_order_id', 'LINE', 'note_text']
+        else:
+            final_columns = ['deid_order_id', 'note_text']
+        items = [f for f in os.listdir(in_dir) if re.match(pattern, f)]
+        for file in items:
+            logger.info(f"""    Processing `file` "{file}".""")
+            out_file = 'deid_{}'.format(file)
+            m = 'w'
+            h = True
+            for df in pd.read_csv(os.path.join(in_dir, file), chunksize=100000, sep='\t'):
+                df = pd.merge(df, map_order, how='left', on='OrderKey')
+                df = df[final_columns]
+                df.to_csv(os.path.join(in_dir, out_file), index=False, sep='\t', mode=m, header=h)
+                m = 'a'
+                h = False
+    return
+
+
+def format_metadata_files(note_type, notes_dir, disclosure_dir):
+    # define variables
+    text_file = '{}_{}_metadata.csv'.format(cohort, note_type)
+    if (note_type == 'note'):
+        final_columns = ['NoteID', 'LinkageNoteID', 'ContactNumber', 'ContactDate', 'CreatedDatetime', 'ServiceDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'InpatientNoteType', 'EncounterDate', 'EncounterCSN', 'AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty', 'CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']
+    elif (note_type == 'order'):
+        final_columns = ['OrderID', 'Line', 'OrderPlacedDatetime', 'OrderResultDatetime', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']
+    # read and format the file
+    m = 'w'
+    h = True
+    for df in pd.read_csv(os.path.join(notes_dir, text_file), chunksize=100000):
+        df = df[final_columns]
+        df.to_csv(os.path.join(disclosure_dir, text_file), index=False, mode=m, header=h)
+        m = 'a'
+        h = False
+    return
+
+
+def copy_tsv(cohort, notes_dir, disclosure_dir):
+    for item in ['note', 'order_narrative', 'order_impression', 'order_result_comment']:
+        dir = cohort + '_' + item
+        if (os.path.exists(os.path.join(notes_dir, dir))):
+            file_list = [f for f in os.listdir(os.path.join(notes_dir, dir))]
+            for f in file_list:
+                shutil.copy(os.path.join(os.path.join(notes_dir, dir, f)), os.path.join(os.path.join(disclosure_dir, f)))
+    return
+
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `COHORT_NAME`: "{COHORT_NAME}"
+    `COHORT_FILE`: "{COHORT_FILE}"
+    `IRB_NUMBER`: "{IRB_NUMBER}"
+    `ID_TYPE`: "{ID_TYPE}"
+    `NOTE_VERSION`: "{NOTE_VERSION}"
+    `DE_IDENTIFICATION_MODE`: "{DE_IDENTIFICATION_MODE}"
+    `SQL_ENCOUNTER_EFFECTIVE_DATE_START`: "{SQL_ENCOUNTER_EFFECTIVE_DATE_START}"
+    `SQL_ENCOUNTER_EFFECTIVE_DATE_END`: "{SQL_ENCOUNTER_EFFECTIVE_DATE_END}"
+
+    # Arguments: SQL connection settings
+    `USE_WINDOWS_AUTHENTICATION` : "{USE_WINDOWS_AUTHENTICATION}"
+    `SERVER`                     : "{SERVER}"
+    `DATABASE_PROD`              : "{DATABASE_PROD}"
+    `DATABASE_NOTES`             : "{DATABASE_NOTES}"
+    `USERDOMAIN`                 : "{USERDOMAIN}"
+    `USERNAME`                   : "{USERNAME}"
+    `UID`                        : "{UID}"
+    `PWD`                        : censored
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+    """)
+    logger.info(f"""`base_dir` set to "{base_dir}".""")
+
+    # pull metadata
+    pull_metadata(note_version, id_type, 'note', sql_dir, data_dir, notes_dir, cohort, logger)
+    pull_metadata(note_version, id_type, 'order_narrative', sql_dir, data_dir, notes_dir, cohort, logger)
+    pull_metadata(note_version, id_type, 'order_impression', sql_dir, data_dir, notes_dir, cohort, logger)
+    pull_metadata(note_version, id_type, 'order_result_comment', sql_dir, data_dir, notes_dir, cohort, logger)
+
+    # split metadata into chunks, so that we can process data in chunks
+    split_metadata('note', notes_dir, cohort, logger)
+    split_metadata('order_narrative', notes_dir, cohort, logger)
+    split_metadata('order_impression', notes_dir, cohort, logger)
+    split_metadata('order_result_comment', notes_dir, cohort, logger)
+
+    # pull text in parallel
+    pull_text_in_parallel('note', sql_dir, notes_dir, cohort, logger)
+    pull_text_in_parallel('order_narrative', sql_dir, notes_dir, cohort, logger)
+    pull_text_in_parallel('order_impression', sql_dir, notes_dir, cohort, logger)
+    pull_text_in_parallel('order_result_comment', sql_dir, notes_dir, cohort, logger)
+    if (deid_mode == 'phi'):
+
+        # copy note_metadata file to disclosure folder
+        format_metadata_files('note', notes_dir, disclosure_dir)
+
+        # combine all order metadata files and copy to discosure folder
+        combine_order_metadata(notes_dir, cohort)
+        format_metadata_files('order', notes_dir, disclosure_dir)
+
+        # copy .tsv files with free text
+        copy_tsv(cohort, notes_dir, disclosure_dir)
+    else:
+        # generate mappings
+        generate_map(deid_mode, data_dir, map_dir, 'patient', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'encounter', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'note', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'note_link', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'order', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'provider', cohort)
+
+        # deidentify metadata. We can create deidentified dataset or limited dataset.
+        deid_metadata(deid_mode, 'note', map_dir, notes_dir, disclosure_dir)
+        deid_metadata(deid_mode, 'order', map_dir, notes_dir, disclosure_dir)
+
+        # prepare for text deidentification, i.e., deidentify ID in .tsv file(s)
+        deid_tsv_note(map_dir, notes_dir, logger)
+        deid_tsv_order(map_dir, notes_dir, logger)
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@REM REMEMBER: Change the following, if applicable:
-@REM 1. `condaEnvPrefix`
-set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
-@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
-@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
-Title My Anaconda IPython Starter
-color 08
-@REM The below command does the following:
-@REM - opens the anaconda environment located at `condaEnvPrefix`
-@REM - clears the screen
-@REM - starts ipython
-cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
+@REM REMEMBER: Change the following, if applicable:
+@REM 1. `condaEnvPrefix`
+set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
+@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
+@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
+Title My Anaconda IPython Starter
+color 08
+@REM The below command does the following:
+@REM - opens the anaconda environment located at `condaEnvPrefix`
+@REM - clears the screen
+@REM - starts ipython
+cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadButton.png` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadButton.png`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadDirectory.png` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadDirectory.png`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README-INSTALLATION.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README-INSTALLATION.md`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,297 +1,297 @@
-"""
-OMOP Data Pull Script
-
-Please be sure to review the README for this script before running.
-"""
-
-__all__ = []
-
-import glob
-import logging
-import os
-import sys
-from pathlib import Path
-# Third-party libraries
-import pandas as pd
-import sqlalchemy as sa
-import yaml
-# Super-local libraries
-import drapi.code.drapi.omop.deidentify as deidentify
-from drapi.code.drapi.drapi import (makeDirPath,
-                                    getTimestamp)
-from drapi.code.drapi.omop.configProcessing import (editConfig,
-                                                    interpretPath)
-
-# Arguments
-LOG_LEVEL = "DEBUG"  # Lowest level available is "9"
-
-# Arguments: SQL server settings
-if False:
-    # TODO Not implemented. See `db_connect`
-    USERNAME_ENVIRONMENT_VARIABLE = "USER"
-    PASSWORD_ENVIRONMENT_VARIABLE = "HFA_UFADPWD"
-    SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
-    DATABASE = "DWS_OMOP_PROD"
-    USERDOMAIN = "UFAD"
-
-# Variables
-timestamp = getTimestamp()
-config_file0 = os.path.join("Config1.yml")
-config_file = os.path.join("Data", "Output", "Config2.yml")
-editConfig(config_file0, config_file, timestamp)
-base_dir = Path(__file__).parent.parent
-
-# Variables: SQL server settings
-if False:
-    # TODO Not implemented. See `db_connect`
-    username = os.environ[USERNAME_ENVIRONMENT_VARIABLE]
-    userid = fr"{USERDOMAIN}\{username}"
-    userpwd = os.environ[PASSWORD_ENVIRONMENT_VARIABLE]
-
-
-def db_connect(host, database):
-    # SQL Server settings
-    SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
-    DATABASE = "DWS_OMOP_PROD"
-    USERDOMAIN = "UFAD"
-    USERNAME = os.environ["USER"]
-    UID = fr"{USERDOMAIN}\{USERNAME}"
-    PWD = os.environ["HFA_UFADPWD"]
-    connstr = f"mssql+pymssql://{UID}:{PWD}@{SERVER}/{DATABASE}"
-    engine = sa.create_engine(connstr)
-    return engine
-
-
-def db_close(db_conn):
-    db_conn.dispose()
-
-
-def import_config():
-    try:
-        config_setting = yaml.safe_load(open(config_file))
-    except Exception as e:
-        logging.critical(e)
-        sys.exit(1)
-    return config_setting
-
-
-def db_query(query, db_connection):
-    dfs = pd.DataFrame()
-    for chunk in pd.read_sql(query, db_connection, chunksize=50000):
-        df = pd.DataFrame(chunk)
-        dfs = dfs.append(df, ignore_index=False)
-    return dfs
-
-
-def db_execute_read_query(host, database, query):
-    db_conn = db_connect(host, database)
-    data = db_query(query, db_conn)
-    db_close(db_conn)
-    return data
-
-
-def db_info(config):
-    host = config['db_connections']['data_pull']['server']
-    database = config['db_connections']['data_pull']['database']
-    schema = config['db_connections']['data_pull']['schema']
-    dict_of_dates = config['clinical_data_tables']
-    dict_of_search = config['data_selection']
-    person_id_file_path = interpretPath(search_config['person_id'])
-    start_date = str(search_config['date_range']['start_date'])
-    end_date = str(search_config['date_range']['end_date'])
-    start_date = "'" + start_date + "'"
-    end_date = "'" + end_date + "'"
-    try:
-        list_of_tables = list(dict_of_dates)
-    except TypeError as error:
-        message = error.args[0]
-        if "object is not iterable" in message:
-            list_of_tables = []
-        else:
-            raise
-    return host, database, schema, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, search_config, dict_of_search
-
-
-def person_info_query(search_config):
-    person_id_file_path = interpretPath(search_config['person_id'])
-    list_of_tables = search_config['person_information_tables']['person_and_death']
-    if (list_of_tables):
-        for i in range(len(list_of_tables)):
-            h = True
-            m = 'w'
-            current_table = list_of_tables[i]
-            columns = search_config.get(current_table)
-            columns_string = ', '.join(map(str, columns))
-            for person_id in pd.read_csv(person_id_file_path, chunksize=500):
-                person_id_list = person_id.iloc[:, 0]
-                person_id_list_string = ', '.join(map(str, person_id_list))
-                query_string = "SELECT " + columns_string + " FROM " + schema + "." + current_table + " WHERE person_id IN (" + person_id_list_string + ")"
-                data = db_execute_read_query(host, database, query_string)
-                if not data.empty:
-                    identified_file_location_AsString = interpretPath(search_config['data_output']['identified_file_location'])
-                    file_location = identified_file_location_AsString + current_table + '.csv'
-                    csv_output_file = (file_location)
-                    try:
-                        data.to_csv(csv_output_file, index=False, header=h, mode=m)
-                        h = False
-                        m = 'a'
-                    except Exception as err:
-                        errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
-                        message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
-                        logging.error(message)
-    list_of_tables = search_config['person_information_tables']['location_table']
-    if (list_of_tables and ('person' in search_config['person_information_tables']['person_and_death'])):
-        identified_file_location_AsString = interpretPath(search_config['data_output']['identified_file_location'])
-        person_file_path = identified_file_location_AsString + 'person.csv'
-        h = True
-        m = 'w'
-        for location_id in pd.read_csv(person_file_path, chunksize=500):
-            location_id_list = []
-            location_id_list = location_id['location_id']
-            location_id_list_string = ', '.join(map(str, location_id_list))
-            current_table = list_of_tables[0]
-            columns = search_config.get(current_table)
-            columns_string = ', '.join(map(str, columns))
-            query_string = "SELECT " + columns_string + " FROM " + current_table + " WHERE location_id IN (" + location_id_list_string + ")"
-            data = db_execute_read_query(host, database, query_string)
-            if not data.empty:
-                identified_file_location_AsString = interpretPath(search_config['data_output']['identified_file_location'])
-                file_location = identified_file_location_AsString + current_table + '.csv'
-                csv_output_file = (file_location)
-                try:
-                    data.to_csv(csv_output_file, index=False, header=h, mode=m)
-                    h = False
-                    m = 'a'
-                except Exception as err:
-                    errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
-                    message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
-                    logging.error(message)
-
-
-def query_attempt(search_config, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, dict_of_search):
-    numTables = len(list_of_tables)
-    for i in range(numTables):
-        h = True
-        m = 'w'
-        h1 = True
-        m1 = 'w'
-        current_table = list_of_tables[i]
-        message = f"""  Working on table "{current_table}", table {i+1} of {numTables}."""
-        logging.info(message)
-        columns = search_config.get(current_table)
-        columns_string = ', '.join(map(str, columns))
-        # Get number of chunks of table
-        numChunks = sum([1 for _ in pd.read_csv(person_id_file_path, chunksize=500)])
-        for it, person_id in enumerate(pd.read_csv(person_id_file_path, chunksize=500), start=1):
-            logging.debug(f"""    Working on table chunk {it} of {numChunks}""")
-            person_id_list = person_id.iloc[:, 0]
-            person_id_list_string = ', '.join(map(str, person_id_list))
-            date_sorted_by = dict_of_dates.get(current_table)
-            query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE person_id IN (" + person_id_list_string + ") AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
-            if ((dict_of_search.get(current_table) is not None)):
-                row_query_string = ''
-                rows = dict_of_search.get(current_table)
-                before, sep, after = current_table.partition('_')
-                current_key = before
-                if (current_table == 'condition_occurrence'):
-                    row_query_string = "("
-                    for i in range(len(rows)):
-                        row_string = rows[i]
-                        row_query_string += "(SELECT " + columns_string + " FROM " + current_table + " WHERE " + current_key + "_source_value LIKE '" + row_string + "%' AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
-                        if (i != len(rows) - 1):
-                            row_query_string += " UNION "
-                        else:
-                            row_query_string += ")"
-                elif (current_table == 'measurement'):
-                    rows_string = "', '".join(map(str, rows))
-                    row_query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE " + current_key + "_source_value IN ('" + rows_string + "') AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
-                    if (dict_of_search.get('measurement_laboratory_search') is not None):
-                        row_string = "', '".join(map(str, dict_of_search.get('measurement_laboratory_search')))
-                        search_query_string = "(SELECT " + columns_string + " FROM " + current_key + " WHERE " + current_key + "_source_value IN ('" + row_string + "') AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
-                    else:
-                        search_query_string = "(SELECT " + columns_string + " FROM " + current_key + " WHERE " + current_key + "_source_value LIKE '%[0-9]-[0-9]'  AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
-                    query = query_string + " INTERSECT " + search_query_string + " ORDER BY person_id, " + date_sorted_by
-                    logging.log(9, f"  ..  >>> This is the query >>>\n{query}\n<<< End of query <<<")
-                    data1 = db_execute_read_query(host, database, query)
-                    identified_file_location_asString = interpretPath(search_config['data_output']['identified_file_location'])
-                    file_location = identified_file_location_asString + 'measurement_laboratories.csv'
-                    if not data1.empty:
-                        csv_output_file = (file_location)
-                        try:
-                            logging.log(9, f"""  ..  Saving query chunk results to "{csv_output_file}".""")
-                            data1.to_csv(csv_output_file, index=False, header=h1, mode=m1)
-                            h1 = False
-                            m1 = 'a'
-                        except Exception as err:
-                            errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
-                            message = f" . . . . . . .An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
-                            logging.error(message)
-                else:
-                    rows_string = "', '".join(map(str, rows))
-                    row_query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE " + current_key + "_source_value IN ('" + rows_string + "') AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
-                query = query_string + " INTERSECT " + row_query_string
-                query_string = query
-            query_string += " ORDER BY person_id, " + date_sorted_by
-            logging.log(9, f"  ..  >>> This is the query >>>\n{query_string}\n<<< End of query <<<")
-            data = db_execute_read_query(host, database, query_string)
-            if not data.empty:
-                identified_file_location_asString = interpretPath(search_config['data_output']['identified_file_location'])
-                file_location = identified_file_location_asString + current_table + '.csv'
-                csv_output_file = (file_location)
-                try:
-                    logging.debug(f"""  ..  Saving query chunk results to "{csv_output_file}".""")
-                    data.to_csv(csv_output_file, index=False, header=h, mode=m)
-                    h = False
-                    m = 'a'
-                except Exception as err:
-                    errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
-                    message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
-                    logging.error(message)
-        logging.info(f"""  Done processing table "{current_table}".""")
-
-
-def deidentify_(mapping_file_location):
-    data_release = search_config.get('data_release')
-    if ('deidentified' in data_release or 'limited' in data_release):
-        path = interpretPath(search_config['data_output']['identified_file_location'])
-        map_path = interpretPath(search_config['data_output']['mapping_location'])
-        all_files = glob.glob(path + "/*.csv")
-        map_files = glob.glob(map_path + "/*.csv")
-        for file in all_files:
-            current_table = os.path.basename(file)
-            file_location = search_config['data_output']['deidentified_file_location'] + data_release[0] + "-" + current_table
-            deidentified_file = deidentify.shift_person_occurrence(file, map_files, data_release)
-            deidentified_file.to_csv(file_location, index=False)
-
-
-if __name__ == '__main__':
-    # Logging block
-    loglevel = "DEBUG"
-    this_file_path = Path(__file__)
-    logpath = os.path.join(base_dir, "logs", f"log {timestamp}.log")
-    makeDirPath(Path(logpath).parent)
-    fileHandler = logging.FileHandler(logpath)
-    streamHandler = logging.StreamHandler()
-    streamHandler.setLevel(loglevel)
-    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
-                        handlers=[fileHandler,
-                                  streamHandler],
-                        level=loglevel)
-
-    logging.info("Starting program.")
-    # import search configuration
-    search_config = import_config()
-    # import connection information for DB connection
-    host, database, schema, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, search_config, dict_of_search = db_info(search_config)
-
-    logging.debug(f"""Reading cohort from `person_id_file_path`: "{person_id_file_path}".""")
-
-    for dataType, path in search_config["data_output"].items():
-        path = Path(interpretPath(path))
-        makeDirPath(path)
-
-    if (list_of_tables):
-        query_attempt(search_config, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, dict_of_search)
-    person_info_query(search_config)
-    # deidentify_(mapping_file_location)
-    logging.info("Finished program.")
+"""
+OMOP Data Pull Script
+
+Please be sure to review the README for this script before running.
+"""
+
+__all__ = []
+
+import glob
+import logging
+import os
+import sys
+from pathlib import Path
+# Third-party libraries
+import pandas as pd
+import sqlalchemy as sa
+import yaml
+# Super-local libraries
+import drapi.code.drapi.omop.deidentify as deidentify
+from drapi.code.drapi.drapi import (makeDirPath,
+                                    getTimestamp)
+from drapi.code.drapi.omop.configProcessing import (editConfig,
+                                                    interpretPath)
+
+# Arguments
+LOG_LEVEL = "DEBUG"  # Lowest level available is "9"
+
+# Arguments: SQL server settings
+if False:
+    # TODO Not implemented. See `db_connect`
+    USERNAME_ENVIRONMENT_VARIABLE = "USER"
+    PASSWORD_ENVIRONMENT_VARIABLE = "HFA_UFADPWD"
+    SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
+    DATABASE = "DWS_OMOP_PROD"
+    USERDOMAIN = "UFAD"
+
+# Variables
+timestamp = getTimestamp()
+config_file0 = os.path.join("Config1.yml")
+config_file = os.path.join("Data", "Output", "Config2.yml")
+editConfig(config_file0, config_file, timestamp)
+base_dir = Path(__file__).parent.parent
+
+# Variables: SQL server settings
+if False:
+    # TODO Not implemented. See `db_connect`
+    username = os.environ[USERNAME_ENVIRONMENT_VARIABLE]
+    userid = fr"{USERDOMAIN}\{username}"
+    userpwd = os.environ[PASSWORD_ENVIRONMENT_VARIABLE]
+
+
+def db_connect(host, database):
+    # SQL Server settings
+    SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
+    DATABASE = "DWS_OMOP_PROD"
+    USERDOMAIN = "UFAD"
+    USERNAME = os.environ["USER"]
+    UID = fr"{USERDOMAIN}\{USERNAME}"
+    PWD = os.environ["HFA_UFADPWD"]
+    connstr = f"mssql+pymssql://{UID}:{PWD}@{SERVER}/{DATABASE}"
+    engine = sa.create_engine(connstr)
+    return engine
+
+
+def db_close(db_conn):
+    db_conn.dispose()
+
+
+def import_config():
+    try:
+        config_setting = yaml.safe_load(open(config_file))
+    except Exception as e:
+        logging.critical(e)
+        sys.exit(1)
+    return config_setting
+
+
+def db_query(query, db_connection):
+    dfs = pd.DataFrame()
+    for chunk in pd.read_sql(query, db_connection, chunksize=50000):
+        df = pd.DataFrame(chunk)
+        dfs = dfs.append(df, ignore_index=False)
+    return dfs
+
+
+def db_execute_read_query(host, database, query):
+    db_conn = db_connect(host, database)
+    data = db_query(query, db_conn)
+    db_close(db_conn)
+    return data
+
+
+def db_info(config):
+    host = config['db_connections']['data_pull']['server']
+    database = config['db_connections']['data_pull']['database']
+    schema = config['db_connections']['data_pull']['schema']
+    dict_of_dates = config['clinical_data_tables']
+    dict_of_search = config['data_selection']
+    person_id_file_path = interpretPath(search_config['person_id'])
+    start_date = str(search_config['date_range']['start_date'])
+    end_date = str(search_config['date_range']['end_date'])
+    start_date = "'" + start_date + "'"
+    end_date = "'" + end_date + "'"
+    try:
+        list_of_tables = list(dict_of_dates)
+    except TypeError as error:
+        message = error.args[0]
+        if "object is not iterable" in message:
+            list_of_tables = []
+        else:
+            raise
+    return host, database, schema, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, search_config, dict_of_search
+
+
+def person_info_query(search_config):
+    person_id_file_path = interpretPath(search_config['person_id'])
+    list_of_tables = search_config['person_information_tables']['person_and_death']
+    if (list_of_tables):
+        for i in range(len(list_of_tables)):
+            h = True
+            m = 'w'
+            current_table = list_of_tables[i]
+            columns = search_config.get(current_table)
+            columns_string = ', '.join(map(str, columns))
+            for person_id in pd.read_csv(person_id_file_path, chunksize=500):
+                person_id_list = person_id.iloc[:, 0]
+                person_id_list_string = ', '.join(map(str, person_id_list))
+                query_string = "SELECT " + columns_string + " FROM " + schema + "." + current_table + " WHERE person_id IN (" + person_id_list_string + ")"
+                data = db_execute_read_query(host, database, query_string)
+                if not data.empty:
+                    identified_file_location_AsString = interpretPath(search_config['data_output']['identified_file_location'])
+                    file_location = identified_file_location_AsString + current_table + '.csv'
+                    csv_output_file = (file_location)
+                    try:
+                        data.to_csv(csv_output_file, index=False, header=h, mode=m)
+                        h = False
+                        m = 'a'
+                    except Exception as err:
+                        errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
+                        message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
+                        logging.error(message)
+    list_of_tables = search_config['person_information_tables']['location_table']
+    if (list_of_tables and ('person' in search_config['person_information_tables']['person_and_death'])):
+        identified_file_location_AsString = interpretPath(search_config['data_output']['identified_file_location'])
+        person_file_path = identified_file_location_AsString + 'person.csv'
+        h = True
+        m = 'w'
+        for location_id in pd.read_csv(person_file_path, chunksize=500):
+            location_id_list = []
+            location_id_list = location_id['location_id']
+            location_id_list_string = ', '.join(map(str, location_id_list))
+            current_table = list_of_tables[0]
+            columns = search_config.get(current_table)
+            columns_string = ', '.join(map(str, columns))
+            query_string = "SELECT " + columns_string + " FROM " + current_table + " WHERE location_id IN (" + location_id_list_string + ")"
+            data = db_execute_read_query(host, database, query_string)
+            if not data.empty:
+                identified_file_location_AsString = interpretPath(search_config['data_output']['identified_file_location'])
+                file_location = identified_file_location_AsString + current_table + '.csv'
+                csv_output_file = (file_location)
+                try:
+                    data.to_csv(csv_output_file, index=False, header=h, mode=m)
+                    h = False
+                    m = 'a'
+                except Exception as err:
+                    errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
+                    message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
+                    logging.error(message)
+
+
+def query_attempt(search_config, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, dict_of_search):
+    numTables = len(list_of_tables)
+    for i in range(numTables):
+        h = True
+        m = 'w'
+        h1 = True
+        m1 = 'w'
+        current_table = list_of_tables[i]
+        message = f"""  Working on table "{current_table}", table {i+1} of {numTables}."""
+        logging.info(message)
+        columns = search_config.get(current_table)
+        columns_string = ', '.join(map(str, columns))
+        # Get number of chunks of table
+        numChunks = sum([1 for _ in pd.read_csv(person_id_file_path, chunksize=500)])
+        for it, person_id in enumerate(pd.read_csv(person_id_file_path, chunksize=500), start=1):
+            logging.debug(f"""    Working on table chunk {it} of {numChunks}""")
+            person_id_list = person_id.iloc[:, 0]
+            person_id_list_string = ', '.join(map(str, person_id_list))
+            date_sorted_by = dict_of_dates.get(current_table)
+            query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE person_id IN (" + person_id_list_string + ") AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
+            if ((dict_of_search.get(current_table) is not None)):
+                row_query_string = ''
+                rows = dict_of_search.get(current_table)
+                before, sep, after = current_table.partition('_')
+                current_key = before
+                if (current_table == 'condition_occurrence'):
+                    row_query_string = "("
+                    for i in range(len(rows)):
+                        row_string = rows[i]
+                        row_query_string += "(SELECT " + columns_string + " FROM " + current_table + " WHERE " + current_key + "_source_value LIKE '" + row_string + "%' AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
+                        if (i != len(rows) - 1):
+                            row_query_string += " UNION "
+                        else:
+                            row_query_string += ")"
+                elif (current_table == 'measurement'):
+                    rows_string = "', '".join(map(str, rows))
+                    row_query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE " + current_key + "_source_value IN ('" + rows_string + "') AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
+                    if (dict_of_search.get('measurement_laboratory_search') is not None):
+                        row_string = "', '".join(map(str, dict_of_search.get('measurement_laboratory_search')))
+                        search_query_string = "(SELECT " + columns_string + " FROM " + current_key + " WHERE " + current_key + "_source_value IN ('" + row_string + "') AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
+                    else:
+                        search_query_string = "(SELECT " + columns_string + " FROM " + current_key + " WHERE " + current_key + "_source_value LIKE '%[0-9]-[0-9]'  AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
+                    query = query_string + " INTERSECT " + search_query_string + " ORDER BY person_id, " + date_sorted_by
+                    logging.log(9, f"  ..  >>> This is the query >>>\n{query}\n<<< End of query <<<")
+                    data1 = db_execute_read_query(host, database, query)
+                    identified_file_location_asString = interpretPath(search_config['data_output']['identified_file_location'])
+                    file_location = identified_file_location_asString + 'measurement_laboratories.csv'
+                    if not data1.empty:
+                        csv_output_file = (file_location)
+                        try:
+                            logging.log(9, f"""  ..  Saving query chunk results to "{csv_output_file}".""")
+                            data1.to_csv(csv_output_file, index=False, header=h1, mode=m1)
+                            h1 = False
+                            m1 = 'a'
+                        except Exception as err:
+                            errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
+                            message = f" . . . . . . .An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
+                            logging.error(message)
+                else:
+                    rows_string = "', '".join(map(str, rows))
+                    row_query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE " + current_key + "_source_value IN ('" + rows_string + "') AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
+                query = query_string + " INTERSECT " + row_query_string
+                query_string = query
+            query_string += " ORDER BY person_id, " + date_sorted_by
+            logging.log(9, f"  ..  >>> This is the query >>>\n{query_string}\n<<< End of query <<<")
+            data = db_execute_read_query(host, database, query_string)
+            if not data.empty:
+                identified_file_location_asString = interpretPath(search_config['data_output']['identified_file_location'])
+                file_location = identified_file_location_asString + current_table + '.csv'
+                csv_output_file = (file_location)
+                try:
+                    logging.debug(f"""  ..  Saving query chunk results to "{csv_output_file}".""")
+                    data.to_csv(csv_output_file, index=False, header=h, mode=m)
+                    h = False
+                    m = 'a'
+                except Exception as err:
+                    errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
+                    message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
+                    logging.error(message)
+        logging.info(f"""  Done processing table "{current_table}".""")
+
+
+def deidentify_(mapping_file_location):
+    data_release = search_config.get('data_release')
+    if ('deidentified' in data_release or 'limited' in data_release):
+        path = interpretPath(search_config['data_output']['identified_file_location'])
+        map_path = interpretPath(search_config['data_output']['mapping_location'])
+        all_files = glob.glob(path + "/*.csv")
+        map_files = glob.glob(map_path + "/*.csv")
+        for file in all_files:
+            current_table = os.path.basename(file)
+            file_location = search_config['data_output']['deidentified_file_location'] + data_release[0] + "-" + current_table
+            deidentified_file = deidentify.shift_person_occurrence(file, map_files, data_release)
+            deidentified_file.to_csv(file_location, index=False)
+
+
+if __name__ == '__main__':
+    # Logging block
+    loglevel = "DEBUG"
+    this_file_path = Path(__file__)
+    logpath = os.path.join(base_dir, "logs", f"log {timestamp}.log")
+    makeDirPath(Path(logpath).parent)
+    fileHandler = logging.FileHandler(logpath)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(loglevel)
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler,
+                                  streamHandler],
+                        level=loglevel)
+
+    logging.info("Starting program.")
+    # import search configuration
+    search_config = import_config()
+    # import connection information for DB connection
+    host, database, schema, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, search_config, dict_of_search = db_info(search_config)
+
+    logging.debug(f"""Reading cohort from `person_id_file_path`: "{person_id_file_path}".""")
+
+    for dataType, path in search_config["data_output"].items():
+        path = Path(interpretPath(path))
+        makeDirPath(path)
+
+    if (list_of_tables):
+        query_attempt(search_config, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, dict_of_search)
+    person_info_query(search_config)
+    # deidentify_(mapping_file_location)
+    logging.info("Finished program.")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-"""
-Get "Person ID" from "Patient Key"
-"""
-
-import logging
-import os
-from pathlib import Path
-# Third-party packages
-import pandas as pd
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-PATIENT_KEYS_CSV_FILE_PATH = Path("data/input/Cohort - Patient Key.CSV")  # TODO
-PATIENT_KEYS_CSV_FILE_HEADER = "Patient Key"  # TODO
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_OMOP_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: Path construction: Project-specific
-personID_SQLQueryFilePath = sqlDir.joinpath("grabPersonIDs.SQL")
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Directory creation: Project-specific
-pass
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-    # Arguments
-    `PATIENT_KEYS_CSV_FILE_PATH`: "{PATIENT_KEYS_CSV_FILE_PATH}"
-    `PATIENT_KEYS_CSV_FILE_HEADER`: "{PATIENT_KEYS_CSV_FILE_HEADER}"
-
-    # Arguments: Meta-arguments
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    # Script
-    # Get patient keys
-    patientKeysInput = pd.read_csv(PATIENT_KEYS_CSV_FILE_PATH, dtype={0: int}).drop_duplicates()
-    listAsString = ",".join([str(x) for x in patientKeysInput.values.flatten()])
-
-    # Get input file header
-    assert patientKeysInput.shape[1] == 1, "Expected file input should be just one column containing patient keys."
-    if PATIENT_KEYS_CSV_FILE_HEADER:
-        inputFileHeader = PATIENT_KEYS_CSV_FILE_HEADER
-    else:
-        inputFileHeader = patientKeysInput.columns[0]
-
-    # Query person IDs
-    logger.info("""Querying database for person IDs.""")
-    with open(personID_SQLQueryFilePath, "r") as file:
-        text = file.read()
-    query = text.replace("XXXXX", listAsString)
-    queryResults = pd.read_sql(query, con=conStr)
-    logger.info("""Querying database for person IDs - done.""")
-
-    # Compare number of Person IDs returned with Patient Keys queried
-    patientKeysInput = patientKeysInput.rename(columns={inputFileHeader: "Patient Key"})
-    patientKeysInput["Patient Key"] = patientKeysInput["Patient Key"].astype(int)
-    queryResults["Patient Key"] = queryResults["Patient Key"].astype(int)
-    patientKeysInput["Found"] = patientKeysInput["Patient Key"].isin(queryResults["Patient Key"])
-    personIDsFound = patientKeysInput.set_index("Patient Key").join(queryResults.set_index("Patient Key"), "Patient Key", "left")
-    personIDsFound = personIDsFound.sort_values("person_id")
-
-    # Summary statistics
-    numFound = personIDsFound["Found"].sum()
-    numPatientKeys = len(patientKeysInput)
-    logger.info(f"""A total of {numFound:,} patient keys of {numPatientKeys:,} were mapped to OMOP person IDs.""")
-    logger.info("""If the number of person IDs is LESS THAN the number of patient keys, it's possible that some patients were merged BEFORE the OMOP database was updated.""")
-    logger.info("""If the number of person IDs is GREATER THAN the number of patient keys, it's possible that some patients were merged AFTER the OMOP database was updated.""")
-
-    # If any column contains NaNs, convert the column to the "Object" data type, to preserve data quality
-    personIDsFound2 = personIDsFound.copy()
-    for column in personIDsFound.columns:
-        if personIDsFound[column].isna().sum() > 0:
-            li = []
-            for value in personIDsFound[column].values:
-                if pd.isna(value):
-                    li.append("")
-                else:
-                    li.append(str(int(value)))
-            personIDsFound2[column] = li
-
-    # Save results: Person IDs found
-    personIDsFoundExportPath = runOutputDir.joinpath("personIDsFound.csv")
-    personIDsFound2.to_csv(personIDsFoundExportPath)
-    logger.info(f"""The map of patient keys to person IDs, and those missing or found, was saved to "{personIDsFoundExportPath}".""")
-
-    # Save results: person IDs
-    personIDs = personIDsFound["person_id"].drop_duplicates().dropna().sort_values().astype(int)
-    personIDsExportPath = runOutputDir.joinpath("personIDs.csv")
-    personIDs.to_csv(personIDsExportPath, index=False)
-    logger.info(f"""Person IDs were saved to "{personIDsExportPath.relative_to(projectDir)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+"""
+Get "Person ID" from "Patient Key"
+"""
+
+import logging
+import os
+from pathlib import Path
+# Third-party packages
+import pandas as pd
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+PATIENT_KEYS_CSV_FILE_PATH = Path("data/input/Cohort - Patient Key.CSV")  # TODO
+PATIENT_KEYS_CSV_FILE_HEADER = "Patient Key"  # TODO
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_OMOP_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: Project-specific
+personID_SQLQueryFilePath = sqlDir.joinpath("grabPersonIDs.SQL")
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Directory creation: Project-specific
+pass
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+    # Arguments
+    `PATIENT_KEYS_CSV_FILE_PATH`: "{PATIENT_KEYS_CSV_FILE_PATH}"
+    `PATIENT_KEYS_CSV_FILE_HEADER`: "{PATIENT_KEYS_CSV_FILE_HEADER}"
+
+    # Arguments: Meta-arguments
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    # Script
+    # Get patient keys
+    patientKeysInput = pd.read_csv(PATIENT_KEYS_CSV_FILE_PATH, dtype={0: int}).drop_duplicates()
+    listAsString = ",".join([str(x) for x in patientKeysInput.values.flatten()])
+
+    # Get input file header
+    assert patientKeysInput.shape[1] == 1, "Expected file input should be just one column containing patient keys."
+    if PATIENT_KEYS_CSV_FILE_HEADER:
+        inputFileHeader = PATIENT_KEYS_CSV_FILE_HEADER
+    else:
+        inputFileHeader = patientKeysInput.columns[0]
+
+    # Query person IDs
+    logger.info("""Querying database for person IDs.""")
+    with open(personID_SQLQueryFilePath, "r") as file:
+        text = file.read()
+    query = text.replace("XXXXX", listAsString)
+    queryResults = pd.read_sql(query, con=conStr)
+    logger.info("""Querying database for person IDs - done.""")
+
+    # Compare number of Person IDs returned with Patient Keys queried
+    patientKeysInput = patientKeysInput.rename(columns={inputFileHeader: "Patient Key"})
+    patientKeysInput["Patient Key"] = patientKeysInput["Patient Key"].astype(int)
+    queryResults["Patient Key"] = queryResults["Patient Key"].astype(int)
+    patientKeysInput["Found"] = patientKeysInput["Patient Key"].isin(queryResults["Patient Key"])
+    personIDsFound = patientKeysInput.set_index("Patient Key").join(queryResults.set_index("Patient Key"), "Patient Key", "left")
+    personIDsFound = personIDsFound.sort_values("person_id")
+
+    # Summary statistics
+    numFound = personIDsFound["Found"].sum()
+    numPatientKeys = len(patientKeysInput)
+    logger.info(f"""A total of {numFound:,} patient keys of {numPatientKeys:,} were mapped to OMOP person IDs.""")
+    logger.info("""If the number of person IDs is LESS THAN the number of patient keys, it's possible that some patients were merged BEFORE the OMOP database was updated.""")
+    logger.info("""If the number of person IDs is GREATER THAN the number of patient keys, it's possible that some patients were merged AFTER the OMOP database was updated.""")
+
+    # If any column contains NaNs, convert the column to the "Object" data type, to preserve data quality
+    personIDsFound2 = personIDsFound.copy()
+    for column in personIDsFound.columns:
+        if personIDsFound[column].isna().sum() > 0:
+            li = []
+            for value in personIDsFound[column].values:
+                if pd.isna(value):
+                    li.append("")
+                else:
+                    li.append(str(int(value)))
+            personIDsFound2[column] = li
+
+    # Save results: Person IDs found
+    personIDsFoundExportPath = runOutputDir.joinpath("personIDsFound.csv")
+    personIDsFound2.to_csv(personIDsFoundExportPath)
+    logger.info(f"""The map of patient keys to person IDs, and those missing or found, was saved to "{personIDsFoundExportPath}".""")
+
+    # Save results: person IDs
+    personIDs = personIDsFound["person_id"].drop_duplicates().dropna().sort_values().astype(int)
+    personIDsExportPath = runOutputDir.joinpath("personIDs.csv")
+    personIDs.to_csv(personIDsExportPath, index=False)
+    logger.info(f"""Person IDs were saved to "{personIDsExportPath.relative_to(projectDir)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@REM REMEMBER: Change the following, if applicable:
-@REM 1. `condaEnvPrefix`
-set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
-@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
-@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
-Title My Anaconda IPython Starter
-color 08
-@REM The below command does the following:
-@REM - opens the anaconda environment located at `condaEnvPrefix`
-@REM - clears the screen
-@REM - starts ipython
-cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
+@REM REMEMBER: Change the following, if applicable:
+@REM 1. `condaEnvPrefix`
+set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
+@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
+@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
+Title My Anaconda IPython Starter
+color 08
+@REM The below command does the following:
+@REM - opens the anaconda environment located at `condaEnvPrefix`
+@REM - clears the screen
+@REM - starts ipython
+cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/README.md`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/README.md`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,525 +1,525 @@
-"""
-Downloads i2b2 data. Optionally also de-identifies it into a limited data set.
-"""
-
-from __future__ import annotations
-
-import os
-import logging
-from logging import Logger
-from pathlib import Path
-from typing import TYPE_CHECKING, Union
-if TYPE_CHECKING:
-    from _typeshed.dbapi import DBAPIConnection
-from typing_extensions import Literal
-# Third-party packages
-import pandas as pd
-import pymssql
-import sqlalchemy as sa
-# Local packages
-from drapi.code.drapi.drapi import (getTimestamp,
-                                    makeDirPath,
-                                    successiveParents)
-
-# Arguments
-COHORT_IDS_FILE_PATH = Path(r"..\..\..\work_2023_02_21\data\intermediate\createCohortFile_requestedCohort\2023-03-02 10-15-50\i2b2Cohort_fromRequestedCohort.CSV")
-COHORT_ID_TYPE = "i2b2 Patient Number"  # A string. One of the `filderID` values of `getIDs`.
-COHORT_COLUMN_NAME = "I2B2_PATIENT_NUM"  # A string. The column name of `COHORT_IDS_FILE_PATH` that contains the IDs.
-COHORT_NAME = 'SGMCPLGB'  # A string. The name of cohort or study, e.g., "cancer_patients"
-IRB_NUMBER = 'IRB201902162'  # A string. The IRB protocol and its number. E.g., "IRB123456789", "CED123456789", or "NH12345678". This is used in creating the patient de-identified IDs.
-DE_IDENTIFY = None  # None-type or string "LDS", for "Limited data set".
-
-# Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
-IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
-
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
-
-LOG_LEVEL = "INFO"
-
-# Arguments: SQL connection settings
-USE_WINDOWS_AUTHENTICATION = True
-SERVER = "EDW.shands.ufl.edu"
-SERVER_I2B2 = "IDR01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-DATABASE_I2B2_GNV = "I2B2LTDDATA"
-DATABASE_I2B2_JAX = "I2B2LTDDATAJAX"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
-# Variables: Path construction: General
-runTimestamp = getTimestamp()
-thisFilePath = Path(__file__)
-thisFileStem = thisFilePath.stem
-projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
-IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
-dataDir = projectDir.joinpath("data")
-if dataDir:
-    inputDataDir = dataDir.joinpath("input")
-    outputDataDir = dataDir.joinpath("output")
-    if outputDataDir:
-        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
-logsDir = projectDir.joinpath("logs")
-if logsDir:
-    runLogsDir = logsDir.joinpath(thisFileStem)
-sqlDir = projectDir.joinpath("sql")
-
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
-    rootDirectory = projectDir
-elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
-    rootDirectory = dataRequestDir
-elif ROOT_DIRECTORY == "IRB_DIRECTORY":
-    rootDirectory = IRBDir
-elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
-    rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-
-# Variables: Map legacy variables to DRAPI-LEMUR standard variables
-cohort = COHORT_NAME
-irb = IRB_NUMBER
-
-base_dir = projectDir
-data_dir = dataDir
-i2b2_dir = runOutputDir.joinpath("i2b2")
-map_dir = runOutputDir.joinpath("mapping")
-disclosure_dir = runOutputDir.joinpath("disclosure")
-
-host = SERVER
-database_prod = DATABASE
-host_i2b2 = SERVER_I2B2
-database_i2b2_GNV = DATABASE_I2B2_GNV
-database_i2b2_JAX = DATABASE_I2B2_JAX
-
-# Directory creation: General
-makeDirPath(runOutputDir)
-makeDirPath(runLogsDir)
-
-# Directory creation: Project-specific
-makeDirPath(i2b2_dir)
-if DE_IDENTIFY.lower():
-    makeDirPath(map_dir)
-    makeDirPath(disclosure_dir)
-elif isinstance(DE_IDENTIFY, type(None)):
-    pass
-else:
-    raise Exception("Invalid option for `DE_IDENTIFY`.")
-
-# Functions: SQL
-
-
-def connectToDatabase(host: str,
-                      database: str,
-                      useWindowsAuthentication=True) -> DBAPIConnection:
-    """
-    Connects to a SQL database given a `host` (server) and `database` value.
-    """
-    if useWindowsAuthentication:
-        connection = pymssql.connect(host=host,
-                                     database=database)
-    else:
-        conStr = f"mssql+pymssql://{uid}:{PWD}@{host}/{database}"
-        connection = sa.create_engine(conStr).connect()
-    return connection
-
-
-def executeQuery(query: str, host: str, database: str) -> pd.DataFrame:
-    """
-    Executes a SQL query.
-    INPUT:
-        `query`: a string
-        `host`: a string
-        `databse`: a string
-    OUTPUT:
-        A pandas dataframe object.
-    """
-    databaseConnection = connectToDatabase(host, database)
-    queryResult = pd.read_sql(query, databaseConnection)
-    databaseConnection.close()
-    return queryResult
-
-
-# Functions: Script-specific
-def getIDs(cohortFilePath: Union[Path, str],
-           filterID: Literal["Patient Key", "EPIC Patient ID", "i2b2 Patient Number", "MRN (UF)", "MRN (Jax)"],
-           logger: Logger,
-           cohortColumnName: Union[None, str] = None) -> None:
-    """
-    Get i2b2 patient IDs from any of the following ID types:
-        - Patient Key
-        - EPIC Patient ID
-        - i2b2 Patient Number
-        - MRN (UF)
-        - MRN (Jax)
-    """
-
-    if filterID == "Patient Key":
-        filterStatement = "WHERE\n\tB.PATNT_KEY IN (XXXXX)"
-        filterIDColumnName = filterID
-    elif filterID == "EPIC Patient ID":
-        filterStatement = "WHERE\n\tA.PATIENT_IDE IN (XXXXX)"
-        filterIDColumnName = filterID
-    elif filterID == "i2b2 Patient Number":
-        filterStatement = "WHERE\n\tA.PATIENT_NUM IN (XXXXX)"
-        filterIDColumnName = filterID
-    elif filterID == "MRN (UF)":
-        filterStatement = "WHERE\n\tC.IDENT_ID IN (XXXXX)"  # NOTE: Not tested
-        filterIDColumnName = filterID
-    elif filterID == "MRN (Jax)":
-        filterStatement = "WHERE\n\tD.IDENT_ID IN (XXXXX)"  # NOTE: Not tested
-        filterIDColumnName = filterID
-    else:
-        raise Exception("No valid option for `filterID` was passed.")
-
-    if cohortColumnName:
-        lookupColumnName = cohortColumnName
-    else:
-        lookupColumnName = filterIDColumnName
-
-    query = f"""
-    SELECT DISTINCT
-        A.PATIENT_IDE AS 'EPIC Patient ID',
-        A.PATIENT_NUM AS 'I2B2_PATIENT_NUM',
-        B.PATNT_KEY AS 'Patient Key',
-        C.IDENT_ID AS 'MRN (UF)',
-        D.IDENT_ID AS 'MRN (Jax)'
-    FROM
-        [DWS_I2B2].[dbo].PATIENT_MAPPING A
-        LEFT OUTER JOIN [DWS_PROD].[dbo].ALL_PATIENT_IDENTITIES B ON A.PATIENT_IDE = B.PATNT_ID
-        LEFT OUTER JOIN [DWS_PROD].[dbo].ALL_PATIENT_IDENTITIES C ON A.PATIENT_IDE = C.PATNT_ID AND C.IDENT_ID_TYPE=101 AND C.LOOKUP_IND='Y'
-        LEFT OUTER JOIN [DWS_PROD].[dbo].ALL_PATIENT_IDENTITIES D ON A.PATIENT_IDE = D.PATNT_ID AND D.IDENT_ID_TYPE=110 AND D.LOOKUP_IND='Y'
-    {filterStatement}
-    """
-    m = 'w'
-    h = True
-    for chunk in pd.read_csv(COHORT_IDS_FILE_PATH, chunksize=3000):
-        chunk = chunk[[lookupColumnName]]
-        chunk = chunk.drop_duplicates()
-        id = chunk[lookupColumnName].tolist()
-        ids = "','".join(str(x) for x in id)
-        ids = "'" + ids + "'"
-        query1 = query.replace('XXXXX', ids)
-        result = executeQuery(query1, host, database_prod)
-        result = result.drop_duplicates()
-        result.to_csv(os.path.join(data_dir, 'Cohort IDs.CSV'), index=False, mode=m, header=h)
-        m = 'a'
-        h = False
-        logger.debug(query1)
-
-
-def i2b2_dump_main(source, table, cohort_dir, i2b2_dir, cohort, logger):
-    """
-    source: 'GNV' or 'JAX'. Indicates which i2b2 instance to use as the source of data.
-    table: 'patient_dimension', 'visit_dimension', or 'observation_fact'. Indicates which table to dump.
-    cohort_dir: Specifies directory where cohort file is saved.
-    i2b2_dir: directory where i2b2 data will be saved.
-    cohort: The name of the cohort. E.g., 'subjects'.
-    """
-    h = True
-    m = 'w'
-    # Cohort should be saved in "Cohort IDs.CSV" file. It should contain i2b2 patient IDs in 'I2B2_PATIENT_NUM' column.
-    for it, ids in enumerate(pd.read_csv(os.path.join(cohort_dir, 'Cohort IDs.CSV'), chunksize=100), start=1):
-        logger.info(f"""  Working on batch {it:,}.""")
-        ids = ids[['I2B2_PATIENT_NUM']].drop_duplicates().dropna()
-        ids = ids['I2B2_PATIENT_NUM'].unique().tolist()
-        ids = "','".join(str(x) for x in ids)
-        ids = "'" + ids + "'"
-
-        if (source == 'GNV'):
-            database = 'I2B2LTDDATA'
-        elif (source == 'JAX'):
-            database = 'I2B2LTDDATAJAX'
-
-        if (table == 'patient_dimension'):
-            query = """
-            select  PATIENT_NUM,VITAL_STATUS_CD,BIRTH_DATE,DEATH_DATE,SEX_CD,AGE_IN_YEARS_NUM,LANGUAGE_CD,RACE_CD,MARITAL_STATUS_CD,RELIGION_CD,ZIP_CD,STATECITYZIP_PATH,INCOME_CD,ETHNIC_CD,PAYER_CD,SMOKING_STATUS_CD,COUNTY_CD,SSN_VITAL_STATUS_CD,MYCHART_CD,CANCER_IND
-            from database.dbo.PATIENT_DIMENSION
-            where PATIENT_NUM in ( XXXXX )
-            """
-        elif (table == 'visit_dimension'):
-            query = """
-            select
-            PATIENT_NUM,ENCOUNTER_NUM,ACTIVE_STATUS_CD,START_DATE,END_DATE,INOUT_CD,LOCATION_CD,LOCATION_PATH,LENGTH_OF_STAY
-            from database.dbo.VISIT_DIMENSION
-            where PATIENT_NUM in ( XXXXX )
-            """
-        elif (table == 'observation_fact'):
-            query = """
-            select  PATIENT_NUM,ENCOUNTER_NUM,CONCEPT_CD,START_DATE,MODIFIER_CD,VALTYPE_CD,TVAL_CHAR,NVAL_NUM,VALUEFLAG_CD,QUANTITY_NUM,UNITS_CD,END_DATE,LOCATION_CD
-            from database.dbo.OBSERVATION_FACT
-            where PATIENT_NUM in ( XXXXX )
-            """
-        query = query.replace('XXXXX', ids)
-        query = query.replace('database', database)
-        if (source == 'GNV'):
-            result = executeQuery(query, host_i2b2, database_i2b2_GNV)
-        elif (source == 'JAX'):
-            result = executeQuery(query, host_i2b2, database_i2b2_JAX)
-        result = result.drop_duplicates()
-        file = cohort + '_' + table + '_' + source + '.csv'
-        result.to_csv(os.path.join(i2b2_dir, file), mode=m, header=h, index=False)
-        h = False
-        m = 'a'
-    logger.info(f"""Completed i2b2 dump for table "{table}" for location "{source}".""")
-
-
-def generate_patient_map(map_dir, cohort_dir):
-    pat = pd.read_csv(os.path.join(cohort_dir, 'Cohort IDs.CSV'))
-    pat_map = pat[['Patient Key']].drop_duplicates()
-    pat_map = pat_map.reset_index()
-    pat_map['deid_num'] = pat_map.index + 1
-    pat_map['deid_pat_ID'] = pat_map.apply(lambda row: str(irb) + '_PAT_' + str(int(row['deid_num'])), axis=1)
-    pat = pd.merge(pat, pat_map, how='left', on='Patient Key')
-    pat.to_csv(os.path.join(map_dir, 'map_patient.csv'), index=False)
-
-
-def generate_encounter_map_i2b2(map_dir, i2b2_dir):
-    # GNV
-    in_file = cohort + '_visit_dimension_GNV.csv'
-    df = pd.read_csv(os.path.join(i2b2_dir, in_file))
-    df = df[['ENCOUNTER_NUM']].drop_duplicates()
-    df1 = pd.DataFrame()
-    in_file = cohort + '_observation_fact_GNV.csv'
-    for chunk in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
-        chunk = chunk[['ENCOUNTER_NUM']].drop_duplicates()
-        df1 = pd.concat([df1, chunk])
-        df1 = df1.drop_duplicates()
-    df = pd.concat([df, df1])
-    df = df.drop_duplicates()
-    df = df.reset_index()
-    df['deid_num'] = df.index + 1
-    df['deid_enc_ID'] = df.apply(lambda row: str(irb) + '_ENC_' + str(int(row['deid_num'])), axis=1)
-    df['source'] = 'GNV'
-    size = df.shape[0]
-
-    # JAX
-    in_file = cohort + '_visit_dimension_JAX.csv'
-    df2 = pd.read_csv(os.path.join(i2b2_dir, in_file))
-    df2 = df2[['ENCOUNTER_NUM']].drop_duplicates()
-    df1 = pd.DataFrame()
-    in_file = cohort + '_observation_fact_JAX.csv'
-    for chunk in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
-        chunk = chunk[['ENCOUNTER_NUM']].drop_duplicates()
-        df1 = pd.concat([df1, chunk])
-        df1 = df1.drop_duplicates()
-    df2 = pd.concat([df2, df1])
-    df2 = df2.drop_duplicates()
-    df2 = df2.reset_index()
-    df2['deid_num'] = df2.index + 1 + size
-    df2['deid_enc_ID'] = df2.apply(lambda row: str(irb) + '_ENC_' + str(int(row['deid_num'])), axis=1)
-    df2['source'] = 'JAX'
-
-    # Concatenate GNV and JAX
-    df = pd.concat([df, df2])
-    df.to_csv(os.path.join(map_dir, 'map_encounter.csv'), index=False)
-
-
-def generate_mappings():
-    generate_patient_map(map_dir, data_dir)
-    generate_encounter_map_i2b2(map_dir, i2b2_dir)
-
-
-def lds_i2b2_patient_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
-    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
-    df = pd.DataFrame(columns=['deid_pat_ID', 'VITAL_STATUS_CD', 'BIRTH_DATE', 'DEATH_DATE', 'SEX_CD', 'AGE_IN_YEARS_NUM', 'LANGUAGE_CD', 'RACE_CD', 'MARITAL_STATUS_CD', 'RELIGION_CD', 'ZIP_CD', 'STATECITYZIP_PATH', 'INCOME_CD', 'ETHNIC_CD', 'PAYER_CD', 'SMOKING_STATUS_CD', 'COUNTY_CD', 'SSN_VITAL_STATUS_CD', 'MYCHART_CD', 'CANCER_IND'])
-    df.to_csv(os.path.join(disclosure_dir_i2b2, 'patient_dimension.csv'), index=False)
-
-    # GNV
-    in_file = cohort + '_patient_dimension_GNV.csv'
-    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
-        df = df.drop_duplicates()
-        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
-        df = df[['deid_pat_ID', 'VITAL_STATUS_CD', 'BIRTH_DATE', 'DEATH_DATE', 'SEX_CD', 'AGE_IN_YEARS_NUM', 'LANGUAGE_CD', 'RACE_CD', 'MARITAL_STATUS_CD', 'RELIGION_CD', 'ZIP_CD', 'STATECITYZIP_PATH', 'INCOME_CD', 'ETHNIC_CD', 'PAYER_CD', 'SMOKING_STATUS_CD', 'COUNTY_CD', 'SSN_VITAL_STATUS_CD', 'MYCHART_CD', 'CANCER_IND']]
-        df.to_csv(os.path.join(disclosure_dir_i2b2, 'patient_dimension.csv'), header=False, index=False, mode='a')
-    logger.info("De-identified GNV patient dimension.")
-
-    # JAX
-    in_file = cohort + '_patient_dimension_JAX.csv'
-    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
-        df = df.drop_duplicates()
-        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
-        df = df[['deid_pat_ID', 'VITAL_STATUS_CD', 'BIRTH_DATE', 'DEATH_DATE', 'SEX_CD', 'AGE_IN_YEARS_NUM', 'LANGUAGE_CD', 'RACE_CD', 'MARITAL_STATUS_CD', 'RELIGION_CD', 'ZIP_CD', 'STATECITYZIP_PATH', 'INCOME_CD', 'ETHNIC_CD', 'PAYER_CD', 'SMOKING_STATUS_CD', 'COUNTY_CD', 'SSN_VITAL_STATUS_CD', 'MYCHART_CD', 'CANCER_IND']]
-        df.to_csv(os.path.join(disclosure_dir_i2b2, 'patient_dimension.csv'), header=False, index=False, mode='a')
-    logger.info("De-identified JAX patient dimension.")
-
-
-def lds_i2b2_visit_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
-    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
-    map_enc = pd.read_csv(os.path.join(map_dir, 'map_encounter.csv'))
-    df = pd.DataFrame(columns=['deid_pat_ID', 'deid_enc_ID', 'ACTIVE_STATUS_CD', 'START_DATE', 'END_DATE', 'INOUT_CD', 'LOCATION_CD', 'LOCATION_PATH', 'LENGTH_OF_STAY'])
-    df.to_csv(os.path.join(disclosure_dir_i2b2, 'visit_dimension.csv'), index=False)
-
-    # GNV
-    in_file = cohort + '_visit_dimension_GNV.csv'
-    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
-        df = df.drop_duplicates()
-        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
-        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
-        df = df[['deid_pat_ID', 'deid_enc_ID', 'ACTIVE_STATUS_CD', 'START_DATE', 'END_DATE', 'INOUT_CD', 'LOCATION_CD', 'LOCATION_PATH', 'LENGTH_OF_STAY']]
-        df.to_csv(os.path.join(disclosure_dir_i2b2, 'visit_dimension.csv'), header=False, index=False, mode='a')
-    logger.info("De-identified GNV visit dimension.")
-
-    # JAX
-    in_file = cohort + '_visit_dimension_JAX.csv'
-    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
-        df = df.drop_duplicates()
-        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
-        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
-        df = df[['deid_pat_ID', 'deid_enc_ID', 'ACTIVE_STATUS_CD', 'START_DATE', 'END_DATE', 'INOUT_CD', 'LOCATION_CD', 'LOCATION_PATH', 'LENGTH_OF_STAY']]
-        df.to_csv(os.path.join(disclosure_dir_i2b2, 'visit_dimension.csv'), header=False, index=False, mode='a')
-    logger.info("De-identified JAX visit dimension.")
-
-
-def lds_i2b2_observation_fact(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
-    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
-    map_enc = pd.read_csv(os.path.join(map_dir, 'map_encounter.csv'))
-    df = pd.DataFrame(columns=['deid_pat_ID', 'deid_enc_ID', 'CONCEPT_CD', 'START_DATE', 'MODIFIER_CD', 'VALTYPE_CD', 'TVAL_CHAR', 'NVAL_NUM', 'VALUEFLAG_CD', 'QUANTITY_NUM', 'UNITS_CD', 'END_DATE', 'LOCATION_CD'])
-    df.to_csv(os.path.join(disclosure_dir_i2b2, 'observation_fact.csv'), index=False)
-
-    CHUNK_SIZE = 10000
-
-    # GNV
-    in_file = cohort + '_observation_fact_GNV.csv'
-    logger.info("""  ..  Reading file to count the number of chunks.""")
-    numChunks = sum([1 for _ in pd.read_csv(in_file, chunksize=CHUNK_SIZE, dtype=str)])
-    logger.info(f"""  ..  This file has {numChunks} chunks.""")
-    fpath = os.path.join(i2b2_dir, in_file)
-    dfChunks = pd.read_csv(fpath, chunksize=CHUNK_SIZE, low_memory=False)
-    for it, df in enumerate(dfChunks, start=1):
-        logger.info(f"""  Working on chunk {it:,} of {numChunks:,}.""")
-        df = df.drop_duplicates()
-        df = df[df['PATIENT_NUM'] != 'PATIENT_NUM']
-        df['PATIENT_NUM'] = df['PATIENT_NUM'].astype(int)
-        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
-        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
-        df = df[['deid_pat_ID', 'deid_enc_ID', 'CONCEPT_CD', 'START_DATE', 'MODIFIER_CD', 'VALTYPE_CD', 'TVAL_CHAR', 'NVAL_NUM', 'VALUEFLAG_CD', 'QUANTITY_NUM', 'UNITS_CD', 'END_DATE', 'LOCATION_CD']]
-        df.to_csv(os.path.join(disclosure_dir_i2b2, 'observation_fact.csv'), header=False, index=False, mode='a')
-    logger.info("De-identified GNV observation fact.")
-
-    # JAX
-    in_file = cohort + '_observation_fact_JAX.csv'
-    logger.info("""  ..  Reading file to count the number of chunks.""")
-    numChunks = sum([1 for _ in pd.read_csv(in_file, chunksize=CHUNK_SIZE, dtype=str)])
-    logger.info(f"""  ..  This file has {numChunks} chunks.""")
-    fpath = os.path.join(i2b2_dir, in_file)
-    dfChunks = pd.read_csv(fpath, chunksize=CHUNK_SIZE, low_memory=False)
-    for it, df in enumerate(dfChunks, start=1):
-        logger.info(f"""  Working on chunk {it:,} of {numChunks:,}.""")
-        df = df.drop_duplicates()
-        df = df[df['PATIENT_NUM'] != 'PATIENT_NUM']
-        df['PATIENT_NUM'] = df['PATIENT_NUM'].astype(int)
-        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
-        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
-        df = df[['deid_pat_ID', 'deid_enc_ID', 'CONCEPT_CD', 'START_DATE', 'MODIFIER_CD', 'VALTYPE_CD', 'TVAL_CHAR', 'NVAL_NUM', 'VALUEFLAG_CD', 'QUANTITY_NUM', 'UNITS_CD', 'END_DATE', 'LOCATION_CD']]
-        df.to_csv(os.path.join(disclosure_dir_i2b2, 'observation_fact.csv'), header=False, index=False, mode='a')
-    logger.info("De-identified JAX observation fact.")
-
-
-def lds_i2b2(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
-    lds_i2b2_patient_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger=logger)
-    lds_i2b2_visit_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger=logger)
-    lds_i2b2_observation_fact(map_dir, i2b2_dir, disclosure_dir_i2b2, logger=logger)
-
-
-def limited_data_set(logger):
-    lds_i2b2(map_dir, i2b2_dir, disclosure_dir, logger=logger)
-
-
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
-if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `COHORT_IDS_FILE_PATH`: "{COHORT_IDS_FILE_PATH}"
-    `COHORT_NAME`: "{COHORT_NAME}"
-    `IRB_NUMBER`: "{IRB_NUMBER}"
-
-    # Arguments: SQL connection settings
-    `USE_WINDOWS_AUTHENTICATION` : "{USE_WINDOWS_AUTHENTICATION}"
-    `SERVER`                     : "{SERVER}"
-    `SERVER_I2B2`                : "{SERVER_I2B2}"
-    `DATABASE`                   : "{DATABASE}"
-    `DATABASE_I2B2_GNV`          : "{DATABASE_I2B2_GNV}"
-    `DATABASE_I2B2_JAX`          : "{DATABASE_I2B2_JAX}"
-    `USERDOMAIN`                 : "{USERDOMAIN}"
-    `USERNAME`                   : "{USERNAME}"
-    `UID`                        : "{UID}"
-    `PWD`                        : censored
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    """)
-
-    # Generate i2b2 patient IDs
-    logger.info("Generating i2b2 patient IDs.")
-    getIDs(cohortFilePath=COHORT_IDS_FILE_PATH,
-           cohortColumnName=COHORT_COLUMN_NAME,
-           filterID=COHORT_ID_TYPE,
-           logger=logger)
-    logger.info("Generating i2b2 patient IDs - done.")
-
-    # Perform i2b2 dump
-    makeDirPath(i2b2_dir)
-    i2b2_dump_main('GNV', 'patient_dimension', data_dir, i2b2_dir, cohort, logger=logger)  # Pull data from patient_dimension in GNV i2b2 instance.
-    i2b2_dump_main('JAX', 'patient_dimension', data_dir, i2b2_dir, cohort, logger=logger)
-    i2b2_dump_main('GNV', 'visit_dimension', data_dir, i2b2_dir, cohort, logger=logger)
-    i2b2_dump_main('JAX', 'visit_dimension', data_dir, i2b2_dir, cohort, logger=logger)
-    i2b2_dump_main('GNV', 'observation_fact', data_dir, i2b2_dir, cohort, logger=logger)
-    i2b2_dump_main('JAX', 'observation_fact', data_dir, i2b2_dir, cohort, logger=logger)
-
-    # Prepare limited data set for disclosure
-    if DE_IDENTIFY.lower() == "lds":
-        generate_mappings()
-        limited_data_set(logger=logger)
-    elif isinstance(DE_IDENTIFY, type(None)):
-        pass
-    else:
-        raise Exception("Invalid option for `DE_IDENTIFY`.")
-
-    # Output location summary
-    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
-
-    # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(projectDir)}".""")
+"""
+Downloads i2b2 data. Optionally also de-identifies it into a limited data set.
+"""
+
+from __future__ import annotations
+
+import os
+import logging
+from logging import Logger
+from pathlib import Path
+from typing import TYPE_CHECKING, Union
+if TYPE_CHECKING:
+    from _typeshed.dbapi import DBAPIConnection
+from typing_extensions import Literal
+# Third-party packages
+import pandas as pd
+import pymssql
+import sqlalchemy as sa
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+
+# Arguments
+COHORT_IDS_FILE_PATH = Path(r"..\..\..\work_2023_02_21\data\intermediate\createCohortFile_requestedCohort\2023-03-02 10-15-50\i2b2Cohort_fromRequestedCohort.CSV")
+COHORT_ID_TYPE = "i2b2 Patient Number"  # A string. One of the `filderID` values of `getIDs`.
+COHORT_COLUMN_NAME = "I2B2_PATIENT_NUM"  # A string. The column name of `COHORT_IDS_FILE_PATH` that contains the IDs.
+COHORT_NAME = 'SGMCPLGB'  # A string. The name of cohort or study, e.g., "cancer_patients"
+IRB_NUMBER = 'IRB201902162'  # A string. The IRB protocol and its number. E.g., "IRB123456789", "CED123456789", or "NH12345678". This is used in creating the patient de-identified IDs.
+DE_IDENTIFY = None  # None-type or string "LDS", for "Limited data set".
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+USE_WINDOWS_AUTHENTICATION = True
+SERVER = "EDW.shands.ufl.edu"
+SERVER_I2B2 = "IDR01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+DATABASE_I2B2_GNV = "I2B2LTDDATA"
+DATABASE_I2B2_JAX = "I2B2LTDDATAJAX"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+
+# Variables: Map legacy variables to DRAPI-LEMUR standard variables
+cohort = COHORT_NAME
+irb = IRB_NUMBER
+
+base_dir = projectDir
+data_dir = dataDir
+i2b2_dir = runOutputDir.joinpath("i2b2")
+map_dir = runOutputDir.joinpath("mapping")
+disclosure_dir = runOutputDir.joinpath("disclosure")
+
+host = SERVER
+database_prod = DATABASE
+host_i2b2 = SERVER_I2B2
+database_i2b2_GNV = DATABASE_I2B2_GNV
+database_i2b2_JAX = DATABASE_I2B2_JAX
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Directory creation: Project-specific
+makeDirPath(i2b2_dir)
+if DE_IDENTIFY.lower():
+    makeDirPath(map_dir)
+    makeDirPath(disclosure_dir)
+elif isinstance(DE_IDENTIFY, type(None)):
+    pass
+else:
+    raise Exception("Invalid option for `DE_IDENTIFY`.")
+
+# Functions: SQL
+
+
+def connectToDatabase(host: str,
+                      database: str,
+                      useWindowsAuthentication=True) -> DBAPIConnection:
+    """
+    Connects to a SQL database given a `host` (server) and `database` value.
+    """
+    if useWindowsAuthentication:
+        connection = pymssql.connect(host=host,
+                                     database=database)
+    else:
+        conStr = f"mssql+pymssql://{uid}:{PWD}@{host}/{database}"
+        connection = sa.create_engine(conStr).connect()
+    return connection
+
+
+def executeQuery(query: str, host: str, database: str) -> pd.DataFrame:
+    """
+    Executes a SQL query.
+    INPUT:
+        `query`: a string
+        `host`: a string
+        `databse`: a string
+    OUTPUT:
+        A pandas dataframe object.
+    """
+    databaseConnection = connectToDatabase(host, database)
+    queryResult = pd.read_sql(query, databaseConnection)
+    databaseConnection.close()
+    return queryResult
+
+
+# Functions: Script-specific
+def getIDs(cohortFilePath: Union[Path, str],
+           filterID: Literal["Patient Key", "EPIC Patient ID", "i2b2 Patient Number", "MRN (UF)", "MRN (Jax)"],
+           logger: Logger,
+           cohortColumnName: Union[None, str] = None) -> None:
+    """
+    Get i2b2 patient IDs from any of the following ID types:
+        - Patient Key
+        - EPIC Patient ID
+        - i2b2 Patient Number
+        - MRN (UF)
+        - MRN (Jax)
+    """
+
+    if filterID == "Patient Key":
+        filterStatement = "WHERE\n\tB.PATNT_KEY IN (XXXXX)"
+        filterIDColumnName = filterID
+    elif filterID == "EPIC Patient ID":
+        filterStatement = "WHERE\n\tA.PATIENT_IDE IN (XXXXX)"
+        filterIDColumnName = filterID
+    elif filterID == "i2b2 Patient Number":
+        filterStatement = "WHERE\n\tA.PATIENT_NUM IN (XXXXX)"
+        filterIDColumnName = filterID
+    elif filterID == "MRN (UF)":
+        filterStatement = "WHERE\n\tC.IDENT_ID IN (XXXXX)"  # NOTE: Not tested
+        filterIDColumnName = filterID
+    elif filterID == "MRN (Jax)":
+        filterStatement = "WHERE\n\tD.IDENT_ID IN (XXXXX)"  # NOTE: Not tested
+        filterIDColumnName = filterID
+    else:
+        raise Exception("No valid option for `filterID` was passed.")
+
+    if cohortColumnName:
+        lookupColumnName = cohortColumnName
+    else:
+        lookupColumnName = filterIDColumnName
+
+    query = f"""
+    SELECT DISTINCT
+        A.PATIENT_IDE AS 'EPIC Patient ID',
+        A.PATIENT_NUM AS 'I2B2_PATIENT_NUM',
+        B.PATNT_KEY AS 'Patient Key',
+        C.IDENT_ID AS 'MRN (UF)',
+        D.IDENT_ID AS 'MRN (Jax)'
+    FROM
+        [DWS_I2B2].[dbo].PATIENT_MAPPING A
+        LEFT OUTER JOIN [DWS_PROD].[dbo].ALL_PATIENT_IDENTITIES B ON A.PATIENT_IDE = B.PATNT_ID
+        LEFT OUTER JOIN [DWS_PROD].[dbo].ALL_PATIENT_IDENTITIES C ON A.PATIENT_IDE = C.PATNT_ID AND C.IDENT_ID_TYPE=101 AND C.LOOKUP_IND='Y'
+        LEFT OUTER JOIN [DWS_PROD].[dbo].ALL_PATIENT_IDENTITIES D ON A.PATIENT_IDE = D.PATNT_ID AND D.IDENT_ID_TYPE=110 AND D.LOOKUP_IND='Y'
+    {filterStatement}
+    """
+    m = 'w'
+    h = True
+    for chunk in pd.read_csv(COHORT_IDS_FILE_PATH, chunksize=3000):
+        chunk = chunk[[lookupColumnName]]
+        chunk = chunk.drop_duplicates()
+        id = chunk[lookupColumnName].tolist()
+        ids = "','".join(str(x) for x in id)
+        ids = "'" + ids + "'"
+        query1 = query.replace('XXXXX', ids)
+        result = executeQuery(query1, host, database_prod)
+        result = result.drop_duplicates()
+        result.to_csv(os.path.join(data_dir, 'Cohort IDs.CSV'), index=False, mode=m, header=h)
+        m = 'a'
+        h = False
+        logger.debug(query1)
+
+
+def i2b2_dump_main(source, table, cohort_dir, i2b2_dir, cohort, logger):
+    """
+    source: 'GNV' or 'JAX'. Indicates which i2b2 instance to use as the source of data.
+    table: 'patient_dimension', 'visit_dimension', or 'observation_fact'. Indicates which table to dump.
+    cohort_dir: Specifies directory where cohort file is saved.
+    i2b2_dir: directory where i2b2 data will be saved.
+    cohort: The name of the cohort. E.g., 'subjects'.
+    """
+    h = True
+    m = 'w'
+    # Cohort should be saved in "Cohort IDs.CSV" file. It should contain i2b2 patient IDs in 'I2B2_PATIENT_NUM' column.
+    for it, ids in enumerate(pd.read_csv(os.path.join(cohort_dir, 'Cohort IDs.CSV'), chunksize=100), start=1):
+        logger.info(f"""  Working on batch {it:,}.""")
+        ids = ids[['I2B2_PATIENT_NUM']].drop_duplicates().dropna()
+        ids = ids['I2B2_PATIENT_NUM'].unique().tolist()
+        ids = "','".join(str(x) for x in ids)
+        ids = "'" + ids + "'"
+
+        if (source == 'GNV'):
+            database = 'I2B2LTDDATA'
+        elif (source == 'JAX'):
+            database = 'I2B2LTDDATAJAX'
+
+        if (table == 'patient_dimension'):
+            query = """
+            select  PATIENT_NUM,VITAL_STATUS_CD,BIRTH_DATE,DEATH_DATE,SEX_CD,AGE_IN_YEARS_NUM,LANGUAGE_CD,RACE_CD,MARITAL_STATUS_CD,RELIGION_CD,ZIP_CD,STATECITYZIP_PATH,INCOME_CD,ETHNIC_CD,PAYER_CD,SMOKING_STATUS_CD,COUNTY_CD,SSN_VITAL_STATUS_CD,MYCHART_CD,CANCER_IND
+            from database.dbo.PATIENT_DIMENSION
+            where PATIENT_NUM in ( XXXXX )
+            """
+        elif (table == 'visit_dimension'):
+            query = """
+            select
+            PATIENT_NUM,ENCOUNTER_NUM,ACTIVE_STATUS_CD,START_DATE,END_DATE,INOUT_CD,LOCATION_CD,LOCATION_PATH,LENGTH_OF_STAY
+            from database.dbo.VISIT_DIMENSION
+            where PATIENT_NUM in ( XXXXX )
+            """
+        elif (table == 'observation_fact'):
+            query = """
+            select  PATIENT_NUM,ENCOUNTER_NUM,CONCEPT_CD,START_DATE,MODIFIER_CD,VALTYPE_CD,TVAL_CHAR,NVAL_NUM,VALUEFLAG_CD,QUANTITY_NUM,UNITS_CD,END_DATE,LOCATION_CD
+            from database.dbo.OBSERVATION_FACT
+            where PATIENT_NUM in ( XXXXX )
+            """
+        query = query.replace('XXXXX', ids)
+        query = query.replace('database', database)
+        if (source == 'GNV'):
+            result = executeQuery(query, host_i2b2, database_i2b2_GNV)
+        elif (source == 'JAX'):
+            result = executeQuery(query, host_i2b2, database_i2b2_JAX)
+        result = result.drop_duplicates()
+        file = cohort + '_' + table + '_' + source + '.csv'
+        result.to_csv(os.path.join(i2b2_dir, file), mode=m, header=h, index=False)
+        h = False
+        m = 'a'
+    logger.info(f"""Completed i2b2 dump for table "{table}" for location "{source}".""")
+
+
+def generate_patient_map(map_dir, cohort_dir):
+    pat = pd.read_csv(os.path.join(cohort_dir, 'Cohort IDs.CSV'))
+    pat_map = pat[['Patient Key']].drop_duplicates()
+    pat_map = pat_map.reset_index()
+    pat_map['deid_num'] = pat_map.index + 1
+    pat_map['deid_pat_ID'] = pat_map.apply(lambda row: str(irb) + '_PAT_' + str(int(row['deid_num'])), axis=1)
+    pat = pd.merge(pat, pat_map, how='left', on='Patient Key')
+    pat.to_csv(os.path.join(map_dir, 'map_patient.csv'), index=False)
+
+
+def generate_encounter_map_i2b2(map_dir, i2b2_dir):
+    # GNV
+    in_file = cohort + '_visit_dimension_GNV.csv'
+    df = pd.read_csv(os.path.join(i2b2_dir, in_file))
+    df = df[['ENCOUNTER_NUM']].drop_duplicates()
+    df1 = pd.DataFrame()
+    in_file = cohort + '_observation_fact_GNV.csv'
+    for chunk in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
+        chunk = chunk[['ENCOUNTER_NUM']].drop_duplicates()
+        df1 = pd.concat([df1, chunk])
+        df1 = df1.drop_duplicates()
+    df = pd.concat([df, df1])
+    df = df.drop_duplicates()
+    df = df.reset_index()
+    df['deid_num'] = df.index + 1
+    df['deid_enc_ID'] = df.apply(lambda row: str(irb) + '_ENC_' + str(int(row['deid_num'])), axis=1)
+    df['source'] = 'GNV'
+    size = df.shape[0]
+
+    # JAX
+    in_file = cohort + '_visit_dimension_JAX.csv'
+    df2 = pd.read_csv(os.path.join(i2b2_dir, in_file))
+    df2 = df2[['ENCOUNTER_NUM']].drop_duplicates()
+    df1 = pd.DataFrame()
+    in_file = cohort + '_observation_fact_JAX.csv'
+    for chunk in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
+        chunk = chunk[['ENCOUNTER_NUM']].drop_duplicates()
+        df1 = pd.concat([df1, chunk])
+        df1 = df1.drop_duplicates()
+    df2 = pd.concat([df2, df1])
+    df2 = df2.drop_duplicates()
+    df2 = df2.reset_index()
+    df2['deid_num'] = df2.index + 1 + size
+    df2['deid_enc_ID'] = df2.apply(lambda row: str(irb) + '_ENC_' + str(int(row['deid_num'])), axis=1)
+    df2['source'] = 'JAX'
+
+    # Concatenate GNV and JAX
+    df = pd.concat([df, df2])
+    df.to_csv(os.path.join(map_dir, 'map_encounter.csv'), index=False)
+
+
+def generate_mappings():
+    generate_patient_map(map_dir, data_dir)
+    generate_encounter_map_i2b2(map_dir, i2b2_dir)
+
+
+def lds_i2b2_patient_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
+    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
+    df = pd.DataFrame(columns=['deid_pat_ID', 'VITAL_STATUS_CD', 'BIRTH_DATE', 'DEATH_DATE', 'SEX_CD', 'AGE_IN_YEARS_NUM', 'LANGUAGE_CD', 'RACE_CD', 'MARITAL_STATUS_CD', 'RELIGION_CD', 'ZIP_CD', 'STATECITYZIP_PATH', 'INCOME_CD', 'ETHNIC_CD', 'PAYER_CD', 'SMOKING_STATUS_CD', 'COUNTY_CD', 'SSN_VITAL_STATUS_CD', 'MYCHART_CD', 'CANCER_IND'])
+    df.to_csv(os.path.join(disclosure_dir_i2b2, 'patient_dimension.csv'), index=False)
+
+    # GNV
+    in_file = cohort + '_patient_dimension_GNV.csv'
+    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
+        df = df.drop_duplicates()
+        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
+        df = df[['deid_pat_ID', 'VITAL_STATUS_CD', 'BIRTH_DATE', 'DEATH_DATE', 'SEX_CD', 'AGE_IN_YEARS_NUM', 'LANGUAGE_CD', 'RACE_CD', 'MARITAL_STATUS_CD', 'RELIGION_CD', 'ZIP_CD', 'STATECITYZIP_PATH', 'INCOME_CD', 'ETHNIC_CD', 'PAYER_CD', 'SMOKING_STATUS_CD', 'COUNTY_CD', 'SSN_VITAL_STATUS_CD', 'MYCHART_CD', 'CANCER_IND']]
+        df.to_csv(os.path.join(disclosure_dir_i2b2, 'patient_dimension.csv'), header=False, index=False, mode='a')
+    logger.info("De-identified GNV patient dimension.")
+
+    # JAX
+    in_file = cohort + '_patient_dimension_JAX.csv'
+    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
+        df = df.drop_duplicates()
+        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
+        df = df[['deid_pat_ID', 'VITAL_STATUS_CD', 'BIRTH_DATE', 'DEATH_DATE', 'SEX_CD', 'AGE_IN_YEARS_NUM', 'LANGUAGE_CD', 'RACE_CD', 'MARITAL_STATUS_CD', 'RELIGION_CD', 'ZIP_CD', 'STATECITYZIP_PATH', 'INCOME_CD', 'ETHNIC_CD', 'PAYER_CD', 'SMOKING_STATUS_CD', 'COUNTY_CD', 'SSN_VITAL_STATUS_CD', 'MYCHART_CD', 'CANCER_IND']]
+        df.to_csv(os.path.join(disclosure_dir_i2b2, 'patient_dimension.csv'), header=False, index=False, mode='a')
+    logger.info("De-identified JAX patient dimension.")
+
+
+def lds_i2b2_visit_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
+    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
+    map_enc = pd.read_csv(os.path.join(map_dir, 'map_encounter.csv'))
+    df = pd.DataFrame(columns=['deid_pat_ID', 'deid_enc_ID', 'ACTIVE_STATUS_CD', 'START_DATE', 'END_DATE', 'INOUT_CD', 'LOCATION_CD', 'LOCATION_PATH', 'LENGTH_OF_STAY'])
+    df.to_csv(os.path.join(disclosure_dir_i2b2, 'visit_dimension.csv'), index=False)
+
+    # GNV
+    in_file = cohort + '_visit_dimension_GNV.csv'
+    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
+        df = df.drop_duplicates()
+        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
+        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
+        df = df[['deid_pat_ID', 'deid_enc_ID', 'ACTIVE_STATUS_CD', 'START_DATE', 'END_DATE', 'INOUT_CD', 'LOCATION_CD', 'LOCATION_PATH', 'LENGTH_OF_STAY']]
+        df.to_csv(os.path.join(disclosure_dir_i2b2, 'visit_dimension.csv'), header=False, index=False, mode='a')
+    logger.info("De-identified GNV visit dimension.")
+
+    # JAX
+    in_file = cohort + '_visit_dimension_JAX.csv'
+    for df in pd.read_csv(os.path.join(i2b2_dir, in_file), chunksize=10000):
+        df = df.drop_duplicates()
+        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
+        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
+        df = df[['deid_pat_ID', 'deid_enc_ID', 'ACTIVE_STATUS_CD', 'START_DATE', 'END_DATE', 'INOUT_CD', 'LOCATION_CD', 'LOCATION_PATH', 'LENGTH_OF_STAY']]
+        df.to_csv(os.path.join(disclosure_dir_i2b2, 'visit_dimension.csv'), header=False, index=False, mode='a')
+    logger.info("De-identified JAX visit dimension.")
+
+
+def lds_i2b2_observation_fact(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
+    map_pat = pd.read_csv(os.path.join(map_dir, 'map_patient.csv'))
+    map_enc = pd.read_csv(os.path.join(map_dir, 'map_encounter.csv'))
+    df = pd.DataFrame(columns=['deid_pat_ID', 'deid_enc_ID', 'CONCEPT_CD', 'START_DATE', 'MODIFIER_CD', 'VALTYPE_CD', 'TVAL_CHAR', 'NVAL_NUM', 'VALUEFLAG_CD', 'QUANTITY_NUM', 'UNITS_CD', 'END_DATE', 'LOCATION_CD'])
+    df.to_csv(os.path.join(disclosure_dir_i2b2, 'observation_fact.csv'), index=False)
+
+    CHUNK_SIZE = 10000
+
+    # GNV
+    in_file = cohort + '_observation_fact_GNV.csv'
+    logger.info("""  ..  Reading file to count the number of chunks.""")
+    numChunks = sum([1 for _ in pd.read_csv(in_file, chunksize=CHUNK_SIZE, dtype=str)])
+    logger.info(f"""  ..  This file has {numChunks} chunks.""")
+    fpath = os.path.join(i2b2_dir, in_file)
+    dfChunks = pd.read_csv(fpath, chunksize=CHUNK_SIZE, low_memory=False)
+    for it, df in enumerate(dfChunks, start=1):
+        logger.info(f"""  Working on chunk {it:,} of {numChunks:,}.""")
+        df = df.drop_duplicates()
+        df = df[df['PATIENT_NUM'] != 'PATIENT_NUM']
+        df['PATIENT_NUM'] = df['PATIENT_NUM'].astype(int)
+        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
+        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
+        df = df[['deid_pat_ID', 'deid_enc_ID', 'CONCEPT_CD', 'START_DATE', 'MODIFIER_CD', 'VALTYPE_CD', 'TVAL_CHAR', 'NVAL_NUM', 'VALUEFLAG_CD', 'QUANTITY_NUM', 'UNITS_CD', 'END_DATE', 'LOCATION_CD']]
+        df.to_csv(os.path.join(disclosure_dir_i2b2, 'observation_fact.csv'), header=False, index=False, mode='a')
+    logger.info("De-identified GNV observation fact.")
+
+    # JAX
+    in_file = cohort + '_observation_fact_JAX.csv'
+    logger.info("""  ..  Reading file to count the number of chunks.""")
+    numChunks = sum([1 for _ in pd.read_csv(in_file, chunksize=CHUNK_SIZE, dtype=str)])
+    logger.info(f"""  ..  This file has {numChunks} chunks.""")
+    fpath = os.path.join(i2b2_dir, in_file)
+    dfChunks = pd.read_csv(fpath, chunksize=CHUNK_SIZE, low_memory=False)
+    for it, df in enumerate(dfChunks, start=1):
+        logger.info(f"""  Working on chunk {it:,} of {numChunks:,}.""")
+        df = df.drop_duplicates()
+        df = df[df['PATIENT_NUM'] != 'PATIENT_NUM']
+        df['PATIENT_NUM'] = df['PATIENT_NUM'].astype(int)
+        df = pd.merge(df, map_pat, how='left', left_on='PATIENT_NUM', right_on='I2B2_PATIENT_NUM')
+        df = pd.merge(df, map_enc, how='left', on='ENCOUNTER_NUM')
+        df = df[['deid_pat_ID', 'deid_enc_ID', 'CONCEPT_CD', 'START_DATE', 'MODIFIER_CD', 'VALTYPE_CD', 'TVAL_CHAR', 'NVAL_NUM', 'VALUEFLAG_CD', 'QUANTITY_NUM', 'UNITS_CD', 'END_DATE', 'LOCATION_CD']]
+        df.to_csv(os.path.join(disclosure_dir_i2b2, 'observation_fact.csv'), header=False, index=False, mode='a')
+    logger.info("De-identified JAX observation fact.")
+
+
+def lds_i2b2(map_dir, i2b2_dir, disclosure_dir_i2b2, logger):
+    lds_i2b2_patient_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger=logger)
+    lds_i2b2_visit_dim(map_dir, i2b2_dir, disclosure_dir_i2b2, logger=logger)
+    lds_i2b2_observation_fact(map_dir, i2b2_dir, disclosure_dir_i2b2, logger=logger)
+
+
+def limited_data_set(logger):
+    lds_i2b2(map_dir, i2b2_dir, disclosure_dir, logger=logger)
+
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `COHORT_IDS_FILE_PATH`: "{COHORT_IDS_FILE_PATH}"
+    `COHORT_NAME`: "{COHORT_NAME}"
+    `IRB_NUMBER`: "{IRB_NUMBER}"
+
+    # Arguments: SQL connection settings
+    `USE_WINDOWS_AUTHENTICATION` : "{USE_WINDOWS_AUTHENTICATION}"
+    `SERVER`                     : "{SERVER}"
+    `SERVER_I2B2`                : "{SERVER_I2B2}"
+    `DATABASE`                   : "{DATABASE}"
+    `DATABASE_I2B2_GNV`          : "{DATABASE_I2B2_GNV}"
+    `DATABASE_I2B2_JAX`          : "{DATABASE_I2B2_JAX}"
+    `USERDOMAIN`                 : "{USERDOMAIN}"
+    `USERNAME`                   : "{USERNAME}"
+    `UID`                        : "{UID}"
+    `PWD`                        : censored
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    """)
+
+    # Generate i2b2 patient IDs
+    logger.info("Generating i2b2 patient IDs.")
+    getIDs(cohortFilePath=COHORT_IDS_FILE_PATH,
+           cohortColumnName=COHORT_COLUMN_NAME,
+           filterID=COHORT_ID_TYPE,
+           logger=logger)
+    logger.info("Generating i2b2 patient IDs - done.")
+
+    # Perform i2b2 dump
+    makeDirPath(i2b2_dir)
+    i2b2_dump_main('GNV', 'patient_dimension', data_dir, i2b2_dir, cohort, logger=logger)  # Pull data from patient_dimension in GNV i2b2 instance.
+    i2b2_dump_main('JAX', 'patient_dimension', data_dir, i2b2_dir, cohort, logger=logger)
+    i2b2_dump_main('GNV', 'visit_dimension', data_dir, i2b2_dir, cohort, logger=logger)
+    i2b2_dump_main('JAX', 'visit_dimension', data_dir, i2b2_dir, cohort, logger=logger)
+    i2b2_dump_main('GNV', 'observation_fact', data_dir, i2b2_dir, cohort, logger=logger)
+    i2b2_dump_main('JAX', 'observation_fact', data_dir, i2b2_dir, cohort, logger=logger)
+
+    # Prepare limited data set for disclosure
+    if DE_IDENTIFY.lower() == "lds":
+        generate_mappings()
+        limited_data_set(logger=logger)
+    elif isinstance(DE_IDENTIFY, type(None)):
+        pass
+    else:
+        raise Exception("Invalid option for `DE_IDENTIFY`.")
+
+    # Output location summary
+    logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(projectDir)}".""")
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@REM REMEMBER: Change the following, if applicable:
-@REM 1. `condaEnvPrefix`
-set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
-@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
-@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
-Title My Anaconda IPython Starter
-color 08
-@REM The below command does the following:
-@REM - opens the anaconda environment located at `condaEnvPrefix`
-@REM - clears the screen
-@REM - starts ipython
-cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
+@REM REMEMBER: Change the following, if applicable:
+@REM 1. `condaEnvPrefix`
+set condaEnvPrefix="C:\Users\herman\Anaconda3\envs\idr-bian2"
+@REM h/t to https://stackoverflow.com/questions/33024344/how-do-i-start-cmd-exe-k-with-multiple-commands
+@REM h/t to https://stackoverflow.com/questions/62992989/how-to-run-ipython-notebook-with-batch-file-on-windows-10
+Title My Anaconda IPython Starter
+color 08
+@REM The below command does the following:
+@REM - opens the anaconda environment located at `condaEnvPrefix`
+@REM - clears the screen
+@REM - starts ipython
+cmd.exe /k "C:\Users\herman\Anaconda3\Scripts\activate.bat %condaEnvPrefix% & cls & ipython"
```

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/scripts/hippaDisclosure.py` & `drapi-lemur-1.0.5/src/drapi/templates/scripts/hippaDisclosure.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi/templates/scripts/sqlQuery.py` & `drapi-lemur-1.0.5/src/drapi/templates/scripts/sqlQuery.py`

 * *Files identical despite different names*

### Comparing `drapi-lemur-1.0.4/src/drapi_lemur.egg-info/PKG-INFO` & `drapi-lemur-1.0.5/src/drapi_lemur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drapi-lemur
-Version: 1.0.4
+Version: 1.0.5
 Summary: Data Request API for the Integrated Data Repository Research Services of University of Florida.
 Home-page: https://github.com/ChemGuy88/hermanCode/archive/refs/tags/v1.0.0.tar.gz
 Author: Herman Autore
 Author-email: hf.autore+drapi@gmail.com
 Keywords: CTSI,Clinical and Translational Science Institute,IDR,Integrated Data Repository,Integrated Data Repository Research Services,ODSRI,Office of Data Science and Research Implementation,Shands,Sloth 🦥,UF,UF Health,UFHealth,University of Florida
 
 Data Request API for the Integrated Data Repository Research Services of University of Florida.
```

### Comparing `drapi-lemur-1.0.4/src/drapi_lemur.egg-info/SOURCES.txt` & `drapi-lemur-1.0.5/src/drapi_lemur.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-src/.DS_Store
 src/makeDirTemplate.py
-src/drapi/.DS_Store
 src/drapi/__init__.py
-src/drapi/__pycache__/__init__.cpython-37.pyc
-src/drapi/__pycache__/__init__.cpython-39.pyc
-src/drapi/code/.DS_Store
 src/drapi/code/__init__.py
 src/drapi/code/tree.py
-src/drapi/code/drapi/.DS_Store
 src/drapi/code/drapi/__init__.py
 src/drapi/code/drapi/compareGroups.py
 src/drapi/code/drapi/drapi.py
 src/drapi/code/drapi/getPersonIDs.py
 src/drapi/code/drapi/makeSymLinks.py
 src/drapi/code/drapi/oneFlorida.py
 src/drapi/code/drapi/prepTSVforSDOH.py
@@ -59,16 +53,14 @@
 src/drapi/sql/9-Digit Zip Code.SQL
 src/drapi/sql/Consent2Share.sql
 src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL
 src/drapi/sql/LADMF.sql
 src/drapi/sql/MRNfromPatientKey.sql
 src/drapi/sql/MapOneFloridaIDs.SQL
 src/drapi/sql/encounterNumber2patientKey.SQL
-src/drapi/templates/.DS_Store
-src/drapi/templates/makeDirTemplate/.DS_Store
 src/drapi/templates/makeDirTemplate/__init__.py
 src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md
 src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore
 src/drapi/templates/makeDirTemplate/MultiPortion Template/README.md
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.env
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md
@@ -146,15 +138,13 @@
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.env
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/README.md
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
 src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
-src/drapi/templates/makeDirTemplate/__pycache__/__init__.cpython-37.pyc
-src/drapi/templates/makeDirTemplate/__pycache__/__init__.cpython-39.pyc
 src/drapi/templates/scripts/hippaDisclosure.py
 src/drapi/templates/scripts/sqlQuery.py
 src/drapi_lemur.egg-info/PKG-INFO
 src/drapi_lemur.egg-info/SOURCES.txt
 src/drapi_lemur.egg-info/dependency_links.txt
 src/drapi_lemur.egg-info/top_level.txt
```

### Comparing `drapi-lemur-1.0.4/src/makeDirTemplate.py` & `drapi-lemur-1.0.5/src/makeDirTemplate.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-"""
-Create a working directory from a template. The general structure of the directory to be made is as follows:
-
-New Directory
-├── code
-├── data
-│   ├── input
-│   └── output
-├── logs
-├── sql
-├── .env
-├── .gitignore
-└── README.md
-
-where "New Directory" is the name of the directory to be created
-"""
-
-import argparse
-import json
-import os
-import sys
-import shutil
-from pathlib import Path
-# Local imports
-from drapi.templates.makeDirTemplate import PATH as makeDirTemplatePath
-
-
-def win2nixPath(string: str) -> str:
-    """
-    Converts a Windows-like path to a Linux-like path by changing the path separators.
-    """
-    platform = sys.platform
-    platformSeparator = os.sep
-    if platform == "darwin":
-        newString = platformSeparator.join(string.split("\\"))
-    elif platform == "win32":
-        newString = string
-    else:
-        raise Exception(f"""Unsupported operating system: "{platform}".""")
-    return newString
-
-
-ROOT_PATH = makeDirTemplatePath.__str__()
-# NOTE `optionsDict` expects `"path"` values to be in Windows format because it's later used by `win2nixPath`
-optionsDict = {"BO": {"number": 2,
-                      "path": r"\MultiPortion Template\Intermediate Results\BO Portion Template"},
-               "De-identification Suite": {"number": 1,
-                                           "path": r"\MultiPortion Template\Concatenated Results"},
-               "General Script": {"number": 3,
-                                  "path": r"\Intermediate Results\General Script Template"},
-               "i2b2": {"number": 4,
-                        "path": r"\MultiPortion Template\Intermediate Results\i2b2 Portion Template"},
-               "Multi-Portion Template": {"number": 0,
-                                          "path": r"\MultiPortion Template"},
-               "Notes": {"number": 5,
-                         "path": r"\MultiPortion Template\Intermediate Results\Notes Portion Template"},
-               "OMOP": {"number": 6,
-                        "path": r"\MultiPortion Template\Intermediate Results\OMOP Portion Template"}}
-
-optionsDict2 = {values["number"]: {"name": name,
-                                   "path": ROOT_PATH + win2nixPath(values["path"])} for name, values in optionsDict.items()}
-
-optionsNumbers = {name: value for name, values in optionsDict.items() for key, value in values.items() if key == "number"}
-
-
-def copyTemplateDirectory(templateChoice: int,
-                          destinationPath: str) -> None:
-    """
-    Given a template selection `templateChoice`, copies the corresponding template directory to the destination path, `destinationPath`.
-    """
-
-    templateDirPath = Path(optionsDict2[templateChoice]["path"])
-
-    shutil.copytree(src=templateDirPath,
-                    dst=destinationPath)
-
-    # Prepare template for use
-    for fpath in Path(destinationPath).glob("./**/*.*"):
-        # Remove placeholder files
-        if fpath.name.lower() == ".deleteme":
-            os.remove(fpath)
-        # Modify ".gitignore"
-        if fpath.name.lower() == ".gitignore":
-            print(fpath)
-            with open(fpath, "r") as file:
-                text = file.read()
-                text = text.replace("!**/launchIPython.bat\n", "")
-                text = text.replace("!.env", ".env")
-                text = text.replace("!data/input/\n", "")
-                text = text.replace("!data/output/\n", "")
-            with open(fpath, "w") as file:
-                file.write(text)
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-
-    parser.add_argument("templateChoice", help=f"""The template you wish to copy. Each template has a numerical option: {json.dumps(optionsNumbers)}""", choices=sorted(list(optionsDict2.keys())), type=int)
-
-    parser.add_argument("destinationPath", help="", type=str)
-
-    args = parser.parse_args()
-
-    templateChoice = args.templateChoice
-    destinationPath = args.destinationPath
-
-    copyTemplateDirectory(templateChoice=templateChoice,
-                          destinationPath=destinationPath)
+"""
+Create a working directory from a template. The general structure of the directory to be made is as follows:
+
+New Directory
+├── code
+├── data
+│   ├── input
+│   └── output
+├── logs
+├── sql
+├── .env
+├── .gitignore
+└── README.md
+
+where "New Directory" is the name of the directory to be created
+"""
+
+import argparse
+import json
+import os
+import sys
+import shutil
+from pathlib import Path
+# Local imports
+from drapi.templates.makeDirTemplate import PATH as makeDirTemplatePath
+
+
+def win2nixPath(string: str) -> str:
+    """
+    Converts a Windows-like path to a Linux-like path by changing the path separators.
+    """
+    platform = sys.platform
+    platformSeparator = os.sep
+    if platform == "darwin":
+        newString = platformSeparator.join(string.split("\\"))
+    elif platform == "win32":
+        newString = string
+    else:
+        raise Exception(f"""Unsupported operating system: "{platform}".""")
+    return newString
+
+
+ROOT_PATH = makeDirTemplatePath.__str__()
+# NOTE `optionsDict` expects `"path"` values to be in Windows format because it's later used by `win2nixPath`
+optionsDict = {"BO": {"number": 2,
+                      "path": r"\MultiPortion Template\Intermediate Results\BO Portion Template"},
+               "De-identification Suite": {"number": 1,
+                                           "path": r"\MultiPortion Template\Concatenated Results"},
+               "General Script": {"number": 3,
+                                  "path": r"\Intermediate Results\General Script Template"},
+               "i2b2": {"number": 4,
+                        "path": r"\MultiPortion Template\Intermediate Results\i2b2 Portion Template"},
+               "Multi-Portion Template": {"number": 0,
+                                          "path": r"\MultiPortion Template"},
+               "Notes": {"number": 5,
+                         "path": r"\MultiPortion Template\Intermediate Results\Notes Portion Template"},
+               "OMOP": {"number": 6,
+                        "path": r"\MultiPortion Template\Intermediate Results\OMOP Portion Template"}}
+
+optionsDict2 = {values["number"]: {"name": name,
+                                   "path": ROOT_PATH + win2nixPath(values["path"])} for name, values in optionsDict.items()}
+
+optionsNumbers = {name: value for name, values in optionsDict.items() for key, value in values.items() if key == "number"}
+
+
+def copyTemplateDirectory(templateChoice: int,
+                          destinationPath: str) -> None:
+    """
+    Given a template selection `templateChoice`, copies the corresponding template directory to the destination path, `destinationPath`.
+    """
+
+    templateDirPath = Path(optionsDict2[templateChoice]["path"])
+
+    shutil.copytree(src=templateDirPath,
+                    dst=destinationPath)
+
+    # Prepare template for use
+    for fpath in Path(destinationPath).glob("./**/*.*"):
+        # Remove placeholder files
+        if fpath.name.lower() == ".deleteme":
+            os.remove(fpath)
+        # Modify ".gitignore"
+        if fpath.name.lower() == ".gitignore":
+            print(fpath)
+            with open(fpath, "r") as file:
+                text = file.read()
+                text = text.replace("!**/launchIPython.bat\n", "")
+                text = text.replace("!.env", ".env")
+                text = text.replace("!data/input/\n", "")
+                text = text.replace("!data/output/\n", "")
+            with open(fpath, "w") as file:
+                file.write(text)
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument("templateChoice", help=f"""The template you wish to copy. Each template has a numerical option: {json.dumps(optionsNumbers)}""", choices=sorted(list(optionsDict2.keys())), type=int)
+
+    parser.add_argument("destinationPath", help="", type=str)
+
+    args = parser.parse_args()
+
+    templateChoice = args.templateChoice
+    destinationPath = args.destinationPath
+
+    copyTemplateDirectory(templateChoice=templateChoice,
+                          destinationPath=destinationPath)
```

