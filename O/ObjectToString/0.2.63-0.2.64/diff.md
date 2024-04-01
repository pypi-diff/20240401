# Comparing `tmp/ObjectToString-0.2.63.tar.gz` & `tmp/ObjectToString-0.2.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ObjectToString-0.2.63.tar", last modified: Sun Mar 31 15:31:05 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "ObjectToString-0.2.64.tar", last modified: Mon Apr  1 15:27:10 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `ObjectToString-0.2.63.tar` & `ObjectToString-0.2.64.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.63/
--rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.63/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.63/objecttostring/
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.63/ObjectToString.egg-info/
--rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.63/ObjectToString.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.63/ObjectToString.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.63/ObjectToString.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.63/ObjectToString.egg-info/top_level.txt
--rwxrwxrwx   0        0        0  3706368 2024-03-31 15:09:37.000000 ObjectToString-0.2.63/objecttostring/pdslib.cp312-win_amd64.pyd
--rwxrwxrwx   0        0        0  1966592 2024-03-31 14:51:53.000000 ObjectToString-0.2.63/objecttostring/python.exe
--rwxrwxrwx   0        0        0    56320 2024-03-31 14:51:11.000000 ObjectToString-0.2.63/objecttostring/python3.dll
--rwxrwxrwx   0        0        0 11250176 2024-03-31 14:51:42.000000 ObjectToString-0.2.63/objecttostring/python312.dll
--rwxrwxrwx   0        0        0     4368 2024-02-22 15:49:50.000000 ObjectToString-0.2.63/objecttostring/test1.py
--rwxrwxrwx   0        0        0      100 2024-03-31 15:30:28.000000 ObjectToString-0.2.63/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.63/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.63/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.64/
+-rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.64/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.64/objecttostring/
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.64/ObjectToString.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.64/ObjectToString.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.64/ObjectToString.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.64/ObjectToString.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.64/ObjectToString.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0  3702272 2024-04-01 15:13:54.000000 ObjectToString-0.2.64/objecttostring/pdslib.cp312-win_amd64.pyd
+-rwxrwxrwx   0        0        0     4368 2024-02-22 15:49:50.000000 ObjectToString-0.2.64/objecttostring/test1.py
+-rwxrwxrwx   0        0        0      100 2024-04-01 15:27:04.000000 ObjectToString-0.2.64/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.64/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.64/setup.py
```

### Comparing `ObjectToString-0.2.63/objecttostring/test1.py` & `ObjectToString-0.2.64/objecttostring/test1.py`

 * *Files identical despite different names*

