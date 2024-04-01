# Comparing `tmp/creyPY-0.0.5.tar.gz` & `tmp/creyPY-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-0.0.5.tar", last modified: Mon Apr  1 15:56:14 2024, max compression
+gzip compressed data, was "creyPY-0.0.6.tar", last modified: Mon Apr  1 16:11:13 2024, max compression
```

## Comparing `creyPY-0.0.5.tar` & `creyPY-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:56:14.325080 creyPY-0.0.5/
--rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.5/LICENSE
--rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 15:56:14.324890 creyPY-0.0.5/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)       60 2024-04-01 15:11:19.000000 creyPY-0.0.5/README.md
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:56:14.323889 creyPY-0.0.5/creyPY/
--rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:43.000000 creyPY-0.0.5/creyPY/__init__.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:56:14.324564 creyPY-0.0.5/creyPY/const/
--rw-r--r--   0 conrad     (501) staff       (20)       58 2024-04-01 15:56:04.000000 creyPY-0.0.5/creyPY/const/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)     9324 2024-04-01 15:51:19.000000 creyPY-0.0.5/creyPY/const/i18n.py
--rw-r--r--   0 conrad     (501) staff       (20)     4373 2024-04-01 15:51:31.000000 creyPY-0.0.5/creyPY/const/stripe.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:56:14.324720 creyPY-0.0.5/creyPY.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 15:56:14.000000 creyPY-0.0.5/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      234 2024-04-01 15:56:14.000000 creyPY-0.0.5/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 15:56:14.000000 creyPY-0.0.5/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)        7 2024-04-01 15:56:14.000000 creyPY-0.0.5/creyPY.egg-info/top_level.txt
--rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 15:56:14.325114 creyPY-0.0.5/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)      352 2024-04-01 15:55:50.000000 creyPY-0.0.5/setup.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:11:13.657763 creyPY-0.0.6/
+-rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.6/LICENSE
+-rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:11:13.657489 creyPY-0.0.6/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      181 2024-04-01 16:11:11.000000 creyPY-0.0.6/README.md
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:11:13.655287 creyPY-0.0.6/creyPY/
+-rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:43.000000 creyPY-0.0.6/creyPY/__init__.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:11:13.656432 creyPY-0.0.6/creyPY/const/
+-rw-r--r--   0 conrad     (501) staff       (20)       58 2024-04-01 15:56:04.000000 creyPY-0.0.6/creyPY/const/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)      146 2024-04-01 16:01:50.000000 creyPY-0.0.6/creyPY/const/groups.py
+-rw-r--r--   0 conrad     (501) staff       (20)     9324 2024-04-01 15:51:19.000000 creyPY-0.0.6/creyPY/const/i18n.py
+-rw-r--r--   0 conrad     (501) staff       (20)     4373 2024-04-01 15:51:31.000000 creyPY-0.0.6/creyPY/const/stripe.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:11:13.656827 creyPY-0.0.6/creyPY/fastapi/
+-rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 16:05:47.000000 creyPY-0.0.6/creyPY/fastapi/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)     1886 2024-04-01 16:10:27.000000 creyPY-0.0.6/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 16:11:13.657229 creyPY-0.0.6/creyPY.egg-info/
+-rw-r--r--   0 conrad     (501) staff       (20)      266 2024-04-01 16:11:13.000000 creyPY-0.0.6/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      313 2024-04-01 16:11:13.000000 creyPY-0.0.6/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 16:11:13.000000 creyPY-0.0.6/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        7 2024-04-01 16:11:13.000000 creyPY-0.0.6/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 16:11:13.657803 creyPY-0.0.6/setup.cfg
+-rw-r--r--   0 conrad     (501) staff       (20)      352 2024-04-01 16:10:35.000000 creyPY-0.0.6/setup.py
```

### Comparing `creyPY-0.0.5/LICENSE` & `creyPY-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.5/creyPY/const/i18n.py` & `creyPY-0.0.6/creyPY/const/i18n.py`

 * *Files identical despite different names*

### Comparing `creyPY-0.0.5/creyPY/const/stripe.py` & `creyPY-0.0.6/creyPY/const/stripe.py`

 * *Files identical despite different names*

