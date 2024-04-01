# Comparing `tmp/creyPY-0.0.2.tar.gz` & `tmp/creyPY-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-0.0.2.tar", last modified: Mon Apr  1 15:41:51 2024, max compression
+gzip compressed data, was "creyPY-0.0.3.tar", last modified: Mon Apr  1 15:51:45 2024, max compression
```

## Comparing `creyPY-0.0.2.tar` & `creyPY-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:41:51.702375 creyPY-0.0.2/
--rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.2/LICENSE
--rw-r--r--   0 conrad     (501) staff       (20)      211 2024-04-01 15:41:51.702172 creyPY-0.0.2/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)       60 2024-04-01 15:11:19.000000 creyPY-0.0.2/README.md
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:41:51.701092 creyPY-0.0.2/const/
--rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:38:30.000000 creyPY-0.0.2/const/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)    13685 2024-04-01 15:18:05.000000 creyPY-0.0.2/const/all.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:41:51.701999 creyPY-0.0.2/creyPY.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)      211 2024-04-01 15:41:51.000000 creyPY-0.0.2/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      177 2024-04-01 15:41:51.000000 creyPY-0.0.2/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 15:41:51.000000 creyPY-0.0.2/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)        6 2024-04-01 15:41:51.000000 creyPY-0.0.2/creyPY.egg-info/top_level.txt
--rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 15:41:51.702421 creyPY-0.0.2/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)      291 2024-04-01 15:38:43.000000 creyPY-0.0.2/setup.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:51:45.093649 creyPY-0.0.3/
+-rw-r--r--   0 conrad     (501) staff       (20)     1063 2024-04-01 15:11:19.000000 creyPY-0.0.3/LICENSE
+-rw-r--r--   0 conrad     (501) staff       (20)      223 2024-04-01 15:51:45.093465 creyPY-0.0.3/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)       60 2024-04-01 15:11:19.000000 creyPY-0.0.3/README.md
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:51:45.092262 creyPY-0.0.3/creyPY/
+-rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:43.000000 creyPY-0.0.3/creyPY/__init__.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:51:45.093046 creyPY-0.0.3/creyPY/const/
+-rw-r--r--   0 conrad     (501) staff       (20)        0 2024-04-01 15:50:48.000000 creyPY-0.0.3/creyPY/const/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)     9324 2024-04-01 15:51:19.000000 creyPY-0.0.3/creyPY/const/i18n.py
+-rw-r--r--   0 conrad     (501) staff       (20)     4373 2024-04-01 15:51:31.000000 creyPY-0.0.3/creyPY/const/stripe.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2024-04-01 15:51:45.093307 creyPY-0.0.3/creyPY.egg-info/
+-rw-r--r--   0 conrad     (501) staff       (20)      223 2024-04-01 15:51:45.000000 creyPY-0.0.3/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      234 2024-04-01 15:51:45.000000 creyPY-0.0.3/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        1 2024-04-01 15:51:45.000000 creyPY-0.0.3/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        7 2024-04-01 15:51:45.000000 creyPY-0.0.3/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       38 2024-04-01 15:51:45.093690 creyPY-0.0.3/setup.cfg
+-rw-r--r--   0 conrad     (501) staff       (20)      358 2024-04-01 15:51:12.000000 creyPY-0.0.3/setup.py
```

### Comparing `creyPY-0.0.2/LICENSE` & `creyPY-0.0.3/LICENSE`

 * *Files identical despite different names*

