# Comparing `tmp/census_request_api-0.0.1.tar.gz` & `tmp/census_request_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "census_request_api-0.0.1.tar", last modified: Wed Mar 27 14:56:53 2024, max compression
+gzip compressed data, was "census_request_api-0.0.2.tar", last modified: Mon Apr  1 13:11:09 2024, max compression
```

## Comparing `census_request_api-0.0.1.tar` & `census_request_api-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lennon     (501) staff       (20)        0 2024-03-27 14:56:53.719916 census_request_api-0.0.1/
--rw-r--r--   0 lennon     (501) staff       (20)      164 2024-03-27 14:56:53.719019 census_request_api-0.0.1/PKG-INFO
--rw-r--r--   0 lennon     (501) staff       (20)        0 2024-03-27 14:52:50.000000 census_request_api-0.0.1/README.md
-drwxr-xr-x   0 lennon     (501) staff       (20)        0 2024-03-27 14:56:53.710091 census_request_api-0.0.1/census_request_api/
--rw-r--r--   0 lennon     (501) staff       (20)       26 2024-03-27 14:54:13.000000 census_request_api-0.0.1/census_request_api/__init__.py
--rw-r--r--   0 lennon     (501) staff       (20)     3024 2024-03-27 14:52:17.000000 census_request_api-0.0.1/census_request_api/main.py
-drwxr-xr-x   0 lennon     (501) staff       (20)        0 2024-03-27 14:56:53.716521 census_request_api-0.0.1/census_request_api.egg-info/
--rw-r--r--   0 lennon     (501) staff       (20)      164 2024-03-27 14:56:53.000000 census_request_api-0.0.1/census_request_api.egg-info/PKG-INFO
--rw-r--r--   0 lennon     (501) staff       (20)      285 2024-03-27 14:56:53.000000 census_request_api-0.0.1/census_request_api.egg-info/SOURCES.txt
--rw-r--r--   0 lennon     (501) staff       (20)        1 2024-03-27 14:56:53.000000 census_request_api-0.0.1/census_request_api.egg-info/dependency_links.txt
--rw-r--r--   0 lennon     (501) staff       (20)       16 2024-03-27 14:56:53.000000 census_request_api-0.0.1/census_request_api.egg-info/requires.txt
--rw-r--r--   0 lennon     (501) staff       (20)       19 2024-03-27 14:56:53.000000 census_request_api-0.0.1/census_request_api.egg-info/top_level.txt
--rw-r--r--   0 lennon     (501) staff       (20)       38 2024-03-27 14:56:53.720097 census_request_api-0.0.1/setup.cfg
--rw-r--r--   0 lennon     (501) staff       (20)      275 2024-03-27 14:56:46.000000 census_request_api-0.0.1/setup.py
+drwxr-xr-x   0 lennon     (501) staff       (20)        0 2024-04-01 13:11:09.912860 census_request_api-0.0.2/
+-rw-r--r--   0 lennon     (501) staff       (20)      164 2024-04-01 13:11:09.912284 census_request_api-0.0.2/PKG-INFO
+-rw-r--r--   0 lennon     (501) staff       (20)        0 2024-03-27 14:52:50.000000 census_request_api-0.0.2/README.md
+drwxr-xr-x   0 lennon     (501) staff       (20)        0 2024-04-01 13:11:09.908782 census_request_api-0.0.2/census_request_api/
+-rw-r--r--   0 lennon     (501) staff       (20)       26 2024-03-27 14:54:13.000000 census_request_api-0.0.2/census_request_api/__init__.py
+-rw-r--r--   0 lennon     (501) staff       (20)     3024 2024-03-27 14:52:17.000000 census_request_api-0.0.2/census_request_api/main.py
+drwxr-xr-x   0 lennon     (501) staff       (20)        0 2024-04-01 13:11:09.911512 census_request_api-0.0.2/census_request_api.egg-info/
+-rw-r--r--   0 lennon     (501) staff       (20)      164 2024-04-01 13:11:09.000000 census_request_api-0.0.2/census_request_api.egg-info/PKG-INFO
+-rw-r--r--   0 lennon     (501) staff       (20)      285 2024-04-01 13:11:09.000000 census_request_api-0.0.2/census_request_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lennon     (501) staff       (20)        1 2024-04-01 13:11:09.000000 census_request_api-0.0.2/census_request_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lennon     (501) staff       (20)       16 2024-04-01 13:11:09.000000 census_request_api-0.0.2/census_request_api.egg-info/requires.txt
+-rw-r--r--   0 lennon     (501) staff       (20)       19 2024-04-01 13:11:09.000000 census_request_api-0.0.2/census_request_api.egg-info/top_level.txt
+-rw-r--r--   0 lennon     (501) staff       (20)       38 2024-04-01 13:11:09.912998 census_request_api-0.0.2/setup.cfg
+-rw-r--r--   0 lennon     (501) staff       (20)      275 2024-04-01 13:08:00.000000 census_request_api-0.0.2/setup.py
```

### Comparing `census_request_api-0.0.1/census_request_api/main.py` & `census_request_api-0.0.2/census_request_api/main.py`

 * *Files identical despite different names*

