# Comparing `tmp/SQLAlchemy-serializer-1.4.7.tar.gz` & `tmp/SQLAlchemy-serializer-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemy-serializer-1.4.7.tar", last modified: Mon Apr  1 12:59:50 2024, max compression
+gzip compressed data, was "SQLAlchemy-serializer-1.4.8.tar", last modified: Mon Apr  1 13:31:50 2024, max compression
```

## Comparing `SQLAlchemy-serializer-1.4.7.tar` & `SQLAlchemy-serializer-1.4.8.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 12:59:50.777151 SQLAlchemy-serializer-1.4.7/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     1061 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.7/LICENSE
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 12:59:50.777240 SQLAlchemy-serializer-1.4.7/PKG-INFO
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12093 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.7/README.md
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 12:59:50.772991 SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 12:59:50.000000 SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/PKG-INFO
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      673 2024-04-01 12:59:50.000000 SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)        1 2024-04-01 12:59:50.000000 SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)       11 2024-04-01 12:59:50.000000 SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/requires.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)       22 2024-04-01 12:59:50.000000 SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/top_level.txt
--rw-r--r--   0 iurii.boiko   (503) staff       (20)       79 2024-04-01 12:59:50.777606 SQLAlchemy-serializer-1.4.7/setup.cfg
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      788 2024-04-01 12:58:53.000000 SQLAlchemy-serializer-1.4.7/setup.py
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 12:59:50.773412 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      118 2024-04-01 08:57:32.000000 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/__init__.py
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 12:59:50.774450 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/lib/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)        0 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/lib/__init__.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     4674 2024-03-31 13:26:57.000000 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/lib/schema.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      279 2024-03-31 13:39:03.000000 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/lib/timezones.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      157 2024-03-31 09:48:02.000000 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/lib/utils.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     7911 2024-04-01 12:54:11.000000 SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/serializer.py
-drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 12:59:50.776913 SQLAlchemy-serializer-1.4.7/tests/
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     1682 2024-04-01 08:10:33.000000 SQLAlchemy-serializer-1.4.7/tests/test_custom_serializer.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     9817 2024-04-01 08:14:28.000000 SQLAlchemy-serializer-1.4.7/tests/test_flat_model.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)    12890 2024-04-01 08:14:52.000000 SQLAlchemy-serializer-1.4.7/tests/test_nested_model.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     2598 2024-04-01 08:15:08.000000 SQLAlchemy-serializer-1.4.7/tests/test_recursive_model.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      491 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.7/tests/test_rules.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     7482 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.7/tests/test_schema.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)     3314 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.7/tests/test_tree.py
--rw-r--r--   0 iurii.boiko   (503) staff       (20)      775 2024-04-01 08:14:21.000000 SQLAlchemy-serializer-1.4.7/tests/test_tzinfo.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 13:31:50.737500 SQLAlchemy-serializer-1.4.8/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     1061 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.8/LICENSE
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 13:31:50.737594 SQLAlchemy-serializer-1.4.8/PKG-INFO
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12093 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.8/README.md
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 13:31:50.733647 SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12563 2024-04-01 13:31:50.000000 SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      634 2024-04-01 13:31:50.000000 SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)        1 2024-04-01 13:31:50.000000 SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)       11 2024-04-01 13:31:50.000000 SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/requires.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)       22 2024-04-01 13:31:50.000000 SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/top_level.txt
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)       79 2024-04-01 13:31:50.738030 SQLAlchemy-serializer-1.4.8/setup.cfg
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      788 2024-04-01 13:31:45.000000 SQLAlchemy-serializer-1.4.8/setup.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 13:31:50.734063 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      118 2024-04-01 08:57:32.000000 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/__init__.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 13:31:50.734846 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/lib/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)        0 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/lib/__init__.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     4674 2024-03-31 13:26:57.000000 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/lib/schema.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      157 2024-03-31 09:48:02.000000 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/lib/utils.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     7911 2024-04-01 12:54:11.000000 SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/serializer.py
+drwxr-xr-x   0 iurii.boiko   (503) staff       (20)        0 2024-04-01 13:31:50.737270 SQLAlchemy-serializer-1.4.8/tests/
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     1682 2024-04-01 08:10:33.000000 SQLAlchemy-serializer-1.4.8/tests/test_custom_serializer.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     9817 2024-04-01 08:14:28.000000 SQLAlchemy-serializer-1.4.8/tests/test_flat_model.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)    12890 2024-04-01 08:14:52.000000 SQLAlchemy-serializer-1.4.8/tests/test_nested_model.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     2598 2024-04-01 08:15:08.000000 SQLAlchemy-serializer-1.4.8/tests/test_recursive_model.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      491 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.8/tests/test_rules.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     7482 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.8/tests/test_schema.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)     3314 2024-03-30 13:17:31.000000 SQLAlchemy-serializer-1.4.8/tests/test_tree.py
+-rw-r--r--   0 iurii.boiko   (503) staff       (20)      775 2024-04-01 08:14:21.000000 SQLAlchemy-serializer-1.4.8/tests/test_tzinfo.py
```

### Comparing `SQLAlchemy-serializer-1.4.7/LICENSE` & `SQLAlchemy-serializer-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/PKG-INFO` & `SQLAlchemy-serializer-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemy-serializer
-Version: 1.4.7
+Version: 1.4.8
 Summary: Mixin for SQLAlchemy-models serialization without pain
 Home-page: https://github.com/n0nSmoker/SQLAlchemy-serializer
 Author: Y-Bro
 Keywords: sqlalchemy,serialize,to_dict,JSON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `SQLAlchemy-serializer-1.4.7/README.md` & `SQLAlchemy-serializer-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/PKG-INFO` & `SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemy-serializer
-Version: 1.4.7
+Version: 1.4.8
 Summary: Mixin for SQLAlchemy-models serialization without pain
 Home-page: https://github.com/n0nSmoker/SQLAlchemy-serializer
 Author: Y-Bro
 Keywords: sqlalchemy,serialize,to_dict,JSON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `SQLAlchemy-serializer-1.4.7/SQLAlchemy_serializer.egg-info/SOURCES.txt` & `SQLAlchemy-serializer-1.4.8/SQLAlchemy_serializer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 SQLAlchemy_serializer.egg-info/dependency_links.txt
 SQLAlchemy_serializer.egg-info/requires.txt
 SQLAlchemy_serializer.egg-info/top_level.txt
 sqlalchemy_serializer/__init__.py
 sqlalchemy_serializer/serializer.py
 sqlalchemy_serializer/lib/__init__.py
 sqlalchemy_serializer/lib/schema.py
-sqlalchemy_serializer/lib/timezones.py
 sqlalchemy_serializer/lib/utils.py
 tests/test_custom_serializer.py
 tests/test_flat_model.py
 tests/test_nested_model.py
 tests/test_recursive_model.py
 tests/test_rules.py
 tests/test_schema.py
```

### Comparing `SQLAlchemy-serializer-1.4.7/setup.py` & `SQLAlchemy-serializer-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SQLAlchemy-serializer",
-    version="1.4.7",
+    version="1.4.8",
     description="Mixin for SQLAlchemy-models serialization without pain",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Y-Bro",
     url="https://github.com/n0nSmoker/SQLAlchemy-serializer",
     keywords=["sqlalchemy", "serialize", "to_dict", "JSON"],
     packages=["sqlalchemy_serializer", "sqlalchemy_serializer.lib"],
```

### Comparing `SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/lib/schema.py` & `SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/lib/schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/sqlalchemy_serializer/serializer.py` & `SQLAlchemy-serializer-1.4.8/sqlalchemy_serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_custom_serializer.py` & `SQLAlchemy-serializer-1.4.8/tests/test_custom_serializer.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_flat_model.py` & `SQLAlchemy-serializer-1.4.8/tests/test_flat_model.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_nested_model.py` & `SQLAlchemy-serializer-1.4.8/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_recursive_model.py` & `SQLAlchemy-serializer-1.4.8/tests/test_recursive_model.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_schema.py` & `SQLAlchemy-serializer-1.4.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_tree.py` & `SQLAlchemy-serializer-1.4.8/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-serializer-1.4.7/tests/test_tzinfo.py` & `SQLAlchemy-serializer-1.4.8/tests/test_tzinfo.py`

 * *Files identical despite different names*

