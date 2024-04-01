# Comparing `tmp/crm1-0.0.2.tar.gz` & `tmp/crm1-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.2.tar", max compression
+gzip compressed data, was "crm1-0.0.3.tar", max compression
```

## Comparing `crm1-0.0.2.tar` & `crm1-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      169 2024-04-01 17:34:54.072808 crm1-0.0.2/crm1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.2/crm1/autorepotools.py
--rw-r--r--   0        0        0      116 2024-04-01 17:28:25.816110 crm1-0.0.2/crm1/data/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-01 17:35:12.466081 crm1-0.0.2/crm1/data/known_modext.py
--rw-r--r--   0        0        0      141 2024-04-01 17:35:24.455160 crm1-0.0.2/crm1/data/responses/__init__.py
--rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.2/crm1/data/responses/dependency.py
--rw-r--r--   0        0        0      938 2024-04-01 17:35:19.065640 crm1-0.0.2/crm1/data/responses/mod.py
--rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.2/crm1/data/responses/repository.py
--rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.2/crm1/types/__init__.py
--rw-r--r--   0        0        0     1103 2024-04-01 17:35:06.616656 crm1-0.0.2/crm1/types/dependency.py
--rw-r--r--   0        0        0     1268 2024-04-01 17:33:24.402313 crm1-0.0.2/crm1/types/mod.py
--rw-r--r--   0        0        0     1975 2024-04-01 18:12:09.042145 crm1-0.0.2/crm1/types/repository.py
--rw-r--r--   0        0        0     2736 2024-04-01 18:12:11.019815 crm1-0.0.2/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      598 2024-04-01 18:12:31.642977 crm1-0.0.2/crm1/utils.py
--rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.2/LICENSE
--rw-r--r--   0        0        0      418 2024-04-01 18:07:25.205241 crm1-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2636 2024-04-01 18:15:32.909827 crm1-0.0.2/README.md
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 crm1-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      169 2024-04-01 17:34:54.072808 crm1-0.0.3/crm1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.3/crm1/autorepotools.py
+-rw-r--r--   0        0        0      116 2024-04-01 17:28:25.816110 crm1-0.0.3/crm1/data/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-01 17:35:12.466081 crm1-0.0.3/crm1/data/known_modext.py
+-rw-r--r--   0        0        0      141 2024-04-01 17:35:24.455160 crm1-0.0.3/crm1/data/responses/__init__.py
+-rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.3/crm1/data/responses/dependency.py
+-rw-r--r--   0        0        0      938 2024-04-01 17:35:19.065640 crm1-0.0.3/crm1/data/responses/mod.py
+-rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.3/crm1/data/responses/repository.py
+-rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.3/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     5669 2024-04-01 19:21:07.202554 crm1-0.0.3/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.3/crm1/types/__init__.py
+-rw-r--r--   0        0        0     1103 2024-04-01 17:35:06.616656 crm1-0.0.3/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1268 2024-04-01 17:33:24.402313 crm1-0.0.3/crm1/types/mod.py
+-rw-r--r--   0        0        0     1975 2024-04-01 18:12:09.042145 crm1-0.0.3/crm1/types/repository.py
+-rw-r--r--   0        0        0     2736 2024-04-01 18:12:11.019815 crm1-0.0.3/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      598 2024-04-01 18:12:31.642977 crm1-0.0.3/crm1/utils.py
+-rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.3/LICENSE
+-rw-r--r--   0        0        0      397 2024-04-01 19:26:35.740855 crm1-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3869 2024-04-01 19:25:44.514186 crm1-0.0.3/README.md
+-rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 crm1-0.0.3/PKG-INFO
```

### Comparing `crm1-0.0.2/crm1/data/known_modext.py` & `crm1-0.0.3/crm1/data/known_modext.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/data/responses/mod.py` & `crm1-0.0.3/crm1/data/responses/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/data/responses/repository.py` & `crm1-0.0.3/crm1/data/responses/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/types/dependency.py` & `crm1-0.0.3/crm1/types/dependency.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/types/mod.py` & `crm1-0.0.3/crm1/types/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/types/repository.py` & `crm1-0.0.3/crm1/types/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/types/repository_pool.py` & `crm1-0.0.3/crm1/types/repository_pool.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/crm1/utils.py` & `crm1-0.0.3/crm1/utils.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.2/LICENSE` & `crm1-0.0.3/LICENSE`

 * *Files identical despite different names*

