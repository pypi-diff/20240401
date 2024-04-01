# Comparing `tmp/SQLAlchemy-serializer-1.4.5.tar.gz` & `tmp/SQLAlchemy-serializer-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemy-serializer-1.4.5.tar", last modified: Mon Apr  1 09:12:30 2024, max compression
+gzip compressed data, was "SQLAlchemy-serializer-1.4.6.tar", last modified: Mon Apr  1 10:35:21 2024, max compression
```

## Comparing `SQLAlchemy-serializer-1.4.5.tar` & `SQLAlchemy-serializer-1.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 09:12:30.656113 SQLAlchemy-serializer-1.4.5/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     1061 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.5/LICENSE
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 09:12:30.656200 SQLAlchemy-serializer-1.4.5/PKG-INFO
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12093 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.5/README.md
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 09:12:30.652231 SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 09:12:30.000000 SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/PKG-INFO
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      673 2024-04-01 09:12:30.000000 SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)        1 2024-04-01 09:12:30.000000 SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)       11 2024-04-01 09:12:30.000000 SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/requires.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)       22 2024-04-01 09:12:30.000000 SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/top_level.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)       79 2024-04-01 09:12:30.656592 SQLAlchemy-serializer-1.4.5/setup.cfg
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      788 2024-04-01 09:12:15.000000 SQLAlchemy-serializer-1.4.5/setup.py
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 09:12:30.652605 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      118 2024-04-01 08:57:32.000000 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/__init__.py
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 09:12:30.653463 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/lib/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)        0 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/lib/__init__.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     4674 2024-03-31 13:26:57.000000 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/lib/schema.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      279 2024-03-31 13:39:03.000000 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/lib/timezones.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      157 2024-03-31 09:48:02.000000 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/lib/utils.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     7974 2024-03-31 21:41:19.000000 SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/serializer.py
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 09:12:30.655893 SQLAlchemy-serializer-1.4.5/tests/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     1682 2024-04-01 08:10:33.000000 SQLAlchemy-serializer-1.4.5/tests/test_custom_serializer.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     9817 2024-04-01 08:14:28.000000 SQLAlchemy-serializer-1.4.5/tests/test_flat_model.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12890 2024-04-01 08:14:52.000000 SQLAlchemy-serializer-1.4.5/tests/test_nested_model.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     2598 2024-04-01 08:15:08.000000 SQLAlchemy-serializer-1.4.5/tests/test_recursive_model.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      491 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.5/tests/test_rules.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     7482 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.5/tests/test_schema.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     3314 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.5/tests/test_tree.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      775 2024-04-01 08:14:21.000000 SQLAlchemy-serializer-1.4.5/tests/test_tzinfo.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 10:35:21.240036 SQLAlchemy-serializer-1.4.6/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     1061 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.6/LICENSE
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 10:35:21.240141 SQLAlchemy-serializer-1.4.6/PKG-INFO
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12093 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.6/README.md
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 10:35:21.236129 SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 10:35:21.000000 SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      673 2024-04-01 10:35:21.000000 SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)        1 2024-04-01 10:35:21.000000 SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)       11 2024-04-01 10:35:21.000000 SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/requires.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)       22 2024-04-01 10:35:21.000000 SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/top_level.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)       79 2024-04-01 10:35:21.240551 SQLAlchemy-serializer-1.4.6/setup.cfg
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      788 2024-04-01 10:35:17.000000 SQLAlchemy-serializer-1.4.6/setup.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 10:35:21.236551 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      118 2024-04-01 08:57:32.000000 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/__init__.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 10:35:21.237486 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/lib/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)        0 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/lib/__init__.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     4674 2024-03-31 13:26:57.000000 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/lib/schema.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      279 2024-03-31 13:39:03.000000 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/lib/timezones.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      157 2024-03-31 09:48:02.000000 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/lib/utils.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     7974 2024-03-31 21:41:19.000000 SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/serializer.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 10:35:21.239788 SQLAlchemy-serializer-1.4.6/tests/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     1682 2024-04-01 08:10:33.000000 SQLAlchemy-serializer-1.4.6/tests/test_custom_serializer.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     9817 2024-04-01 08:14:28.000000 SQLAlchemy-serializer-1.4.6/tests/test_flat_model.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12890 2024-04-01 08:14:52.000000 SQLAlchemy-serializer-1.4.6/tests/test_nested_model.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     2598 2024-04-01 08:15:08.000000 SQLAlchemy-serializer-1.4.6/tests/test_recursive_model.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      491 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.6/tests/test_rules.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     7482 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.6/tests/test_schema.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     3314 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.6/tests/test_tree.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      775 2024-04-01 08:14:21.000000 SQLAlchemy-serializer-1.4.6/tests/test_tzinfo.py
```

### Comparing `SQLAlchemy-serializer-1.4.5/LICENSE` & `SQLAlchemy-serializer-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/PKG-INFO` & `SQLAlchemy-serializer-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemy-serializer
-Version: 1.4.5
+Version: 1.4.6
 Summary: Mixin for SQLAlchemy-models serialization without pain
 Home-page: https://github.com/n0nSmoker/SQLAlchemy-serializer
 Author: Y-Bro
 Keywords: sqlalchemy,serialize,to_dict,JSON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `SQLAlchemy-serializer-1.4.5/README.md` & `SQLAlchemy-serializer-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/PKG-INFO` & `SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemy-serializer
-Version: 1.4.5
+Version: 1.4.6
 Summary: Mixin for SQLAlchemy-models serialization without pain
 Home-page: https://github.com/n0nSmoker/SQLAlchemy-serializer
 Author: Y-Bro
 Keywords: sqlalchemy,serialize,to_dict,JSON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `SQLAlchemy-serializer-1.4.5/SQLAlchemy_serializer.egg-info/SOURCES.txt` & `SQLAlchemy-serializer-1.4.6/SQLAlchemy_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/setup.py` & `SQLAlchemy-serializer-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SQLAlchemy-serializer",
-    version="1.4.5",
+    version="1.4.6",
     description="Mixin for SQLAlchemy-models serialization without pain",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Y-Bro",
     url="https://github.com/n0nSmoker/SQLAlchemy-serializer",
     keywords=["sqlalchemy", "serialize", "to_dict", "JSON"],
     packages=["sqlalchemy_serializer", "sqlalchemy_serializer.lib"],
```

### Comparing `SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/lib/schema.py` & `SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/lib/schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/sqlalchemy_serializer/serializer.py` & `SQLAlchemy-serializer-1.4.6/sqlalchemy_serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_custom_serializer.py` & `SQLAlchemy-serializer-1.4.6/tests/test_custom_serializer.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_flat_model.py` & `SQLAlchemy-serializer-1.4.6/tests/test_flat_model.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_nested_model.py` & `SQLAlchemy-serializer-1.4.6/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_recursive_model.py` & `SQLAlchemy-serializer-1.4.6/tests/test_recursive_model.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_schema.py` & `SQLAlchemy-serializer-1.4.6/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_tree.py` & `SQLAlchemy-serializer-1.4.6/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.5/tests/test_tzinfo.py` & `SQLAlchemy-serializer-1.4.6/tests/test_tzinfo.py`

 * *Files identical despite different names*

