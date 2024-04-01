# Comparing `tmp/godspeed_api-0.0.2.tar.gz` & `tmp/godspeed_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "godspeed_api-0.0.3.tar", last modified: Mon Apr  1 12:44:28 2024, max compression
```

## Comparing `godspeed_api-0.0.2.tar` & `godspeed_api-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/src/godspeed_api/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/src/godspeed_api/api.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/README.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/PKG-INFO
+drwxr-xr-x   0 almaz5200   (501) staff       (20)        0 2024-04-01 12:44:28.107118 godspeed_api-0.0.3/
+-rw-r--r--   0 almaz5200   (501) staff       (20)     1074 2024-04-01 12:29:18.000000 godspeed_api-0.0.3/LICENSE
+-rw-r--r--   0 almaz5200   (501) staff       (20)      493 2024-04-01 12:44:28.106965 godspeed_api-0.0.3/PKG-INFO
+-rw-r--r--   0 almaz5200   (501) staff       (20)       15 2024-04-01 12:24:25.000000 godspeed_api-0.0.3/README.md
+drwxr-xr-x   0 almaz5200   (501) staff       (20)        0 2024-04-01 12:44:28.106809 godspeed_api-0.0.3/godspeed_api.egg-info/
+-rw-r--r--   0 almaz5200   (501) staff       (20)      493 2024-04-01 12:44:28.000000 godspeed_api-0.0.3/godspeed_api.egg-info/PKG-INFO
+-rw-r--r--   0 almaz5200   (501) staff       (20)      170 2024-04-01 12:44:28.000000 godspeed_api-0.0.3/godspeed_api.egg-info/SOURCES.txt
+-rw-r--r--   0 almaz5200   (501) staff       (20)        1 2024-04-01 12:44:28.000000 godspeed_api-0.0.3/godspeed_api.egg-info/dependency_links.txt
+-rw-r--r--   0 almaz5200   (501) staff       (20)        1 2024-04-01 12:44:28.000000 godspeed_api-0.0.3/godspeed_api.egg-info/top_level.txt
+-rw-r--r--   0 almaz5200   (501) staff       (20)       38 2024-04-01 12:44:28.107302 godspeed_api-0.0.3/setup.cfg
+-rw-r--r--   0 almaz5200   (501) staff       (20)      667 2024-04-01 12:41:58.000000 godspeed_api-0.0.3/setup.py
```

### Comparing `godspeed_api-0.0.2/LICENSE` & `godspeed_api-0.0.3/LICENSE`

 * *Files identical despite different names*

