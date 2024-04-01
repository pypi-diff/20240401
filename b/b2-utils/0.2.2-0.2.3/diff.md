# Comparing `tmp/b2-utils-0.2.2.tar.gz` & `tmp/b2-utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2-utils-0.2.2.tar", last modified: Thu Feb 22 13:30:38 2024, max compression
+gzip compressed data, was "b2-utils-0.2.3.tar", last modified: Mon Apr  1 13:02:28 2024, max compression
```

## Comparing `b2-utils-0.2.2.tar` & `b2-utils-0.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/
--rw-r--r--   0 felipesena  (1000) felipesena  (1000)     1281 2024-02-22 13:30:38.861849 b2-utils-0.2.2/PKG-INFO
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      520 2023-10-19 17:23:19.000000 b2-utils-0.2.2/README.md
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2543 2024-02-22 13:28:21.000000 b2-utils-0.2.2/pyproject.toml
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)       38 2024-02-22 13:30:38.861849 b2-utils-0.2.2/setup.cfg
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.857849 b2-utils-0.2.2/src/
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils/
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)        0 2023-10-19 17:23:19.000000 b2-utils-0.2.2/src/b2_utils/__init__.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2436 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/context.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     1537 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/decorators.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     8303 2024-02-22 12:44:06.000000 b2-utils-0.2.2/src/b2_utils/enums.py
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils/faker/
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      358 2024-02-20 18:12:57.000000 b2-utils-0.2.2/src/b2_utils/faker/__init__.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     8993 2024-02-20 18:12:57.000000 b2-utils-0.2.2/src/b2_utils/faker/providers.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2482 2024-02-20 18:12:57.000000 b2-utils-0.2.2/src/b2_utils/fields.py
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils/helpers/
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     5297 2024-02-20 18:12:57.000000 b2-utils-0.2.2/src/b2_utils/helpers/__init__.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     1042 2023-10-19 17:23:19.000000 b2-utils-0.2.2/src/b2_utils/helpers/auth.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     1990 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/helpers.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      386 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/mails.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     5402 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/mixins.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      424 2023-10-19 17:23:19.000000 b2-utils-0.2.2/src/b2_utils/pagination.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2302 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/permissions.py
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils/serializers/
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2537 2024-02-22 13:27:59.000000 b2-utils-0.2.2/src/b2_utils/serializers/__init__.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      480 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/serializers/mixins.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2574 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/serializers/relations.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2357 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/tasks.py
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils/templatetags/
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)        0 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/templatetags/__init__.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     1215 2024-02-20 18:12:57.000000 b2-utils-0.2.2/src/b2_utils/templatetags/b2_utils.py
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils/tests/
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      145 2023-10-19 17:23:19.000000 b2-utils-0.2.2/src/b2_utils/tests/__init__.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     1201 2024-02-22 12:30:11.000000 b2-utils-0.2.2/src/b2_utils/tests/helpers.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      118 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/typing.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     2440 2024-02-20 18:12:57.000000 b2-utils-0.2.2/src/b2_utils/validators.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)     1005 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/b2_utils/views.py
-drwxrwxr-x   0 felipesena  (1000) felipesena  (1000)        0 2024-02-22 13:30:38.861849 b2-utils-0.2.2/src/b2_utils.egg-info/
--rw-r--r--   0 felipesena  (1000) felipesena  (1000)     1281 2024-02-22 13:30:38.000000 b2-utils-0.2.2/src/b2_utils.egg-info/PKG-INFO
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      944 2024-02-22 13:30:38.000000 b2-utils-0.2.2/src/b2_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)        1 2024-02-22 13:30:38.000000 b2-utils-0.2.2/src/b2_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      153 2024-02-22 13:30:38.000000 b2-utils-0.2.2/src/b2_utils.egg-info/requires.txt
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)       32 2024-02-22 13:30:38.000000 b2-utils-0.2.2/src/b2_utils.egg-info/top_level.txt
--rwxrwxr-x   0 felipesena  (1000) felipesena  (1000)      655 2023-10-19 17:23:19.000000 b2-utils-0.2.2/src/manage.py
--rw-rw-r--   0 felipesena  (1000) felipesena  (1000)      144 2024-02-07 13:21:32.000000 b2-utils-0.2.2/src/settings.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.273141 b2-utils-0.2.3/
+-rw-r--r--   0 candidojr  (1000) candidojr  (1000)     1281 2024-04-01 13:02:28.273141 b2-utils-0.2.3/PKG-INFO
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      520 2024-04-01 12:20:01.000000 b2-utils-0.2.3/README.md
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2543 2024-04-01 12:45:53.000000 b2-utils-0.2.3/pyproject.toml
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)       38 2024-04-01 13:02:28.273141 b2-utils-0.2.3/setup.cfg
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.269141 b2-utils-0.2.3/src/
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.269141 b2-utils-0.2.3/src/b2_utils/
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/__init__.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2436 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/context.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     1537 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/decorators.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     8303 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/enums.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.269141 b2-utils-0.2.3/src/b2_utils/faker/
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      358 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/faker/__init__.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     8993 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/faker/providers.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2482 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/fields.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.269141 b2-utils-0.2.3/src/b2_utils/helpers/
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     5297 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/helpers/__init__.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     1042 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/helpers/auth.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     1990 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/helpers.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      386 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/mails.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     5402 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/mixins.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      424 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/pagination.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2302 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/permissions.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.269141 b2-utils-0.2.3/src/b2_utils/serializers/
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2537 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/serializers/__init__.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      480 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/serializers/mixins.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2596 2024-04-01 12:23:07.000000 b2-utils-0.2.3/src/b2_utils/serializers/relations.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2357 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/tasks.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.269141 b2-utils-0.2.3/src/b2_utils/templatetags/
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/templatetags/__init__.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     1215 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/templatetags/b2_utils.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.273141 b2-utils-0.2.3/src/b2_utils/tests/
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      145 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/tests/__init__.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     1201 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/tests/helpers.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      118 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/typing.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     2440 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/validators.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)     1005 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/b2_utils/views.py
+drwxrwxr-x   0 candidojr  (1000) candidojr  (1000)        0 2024-04-01 13:02:28.273141 b2-utils-0.2.3/src/b2_utils.egg-info/
+-rw-r--r--   0 candidojr  (1000) candidojr  (1000)     1281 2024-04-01 13:02:28.000000 b2-utils-0.2.3/src/b2_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      944 2024-04-01 13:02:28.000000 b2-utils-0.2.3/src/b2_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)        1 2024-04-01 13:02:28.000000 b2-utils-0.2.3/src/b2_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      153 2024-04-01 13:02:28.000000 b2-utils-0.2.3/src/b2_utils.egg-info/requires.txt
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)       32 2024-04-01 13:02:28.000000 b2-utils-0.2.3/src/b2_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 candidojr  (1000) candidojr  (1000)      655 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/manage.py
+-rw-rw-r--   0 candidojr  (1000) candidojr  (1000)      144 2024-04-01 12:20:01.000000 b2-utils-0.2.3/src/settings.py
```

### Comparing `b2-utils-0.2.2/PKG-INFO` & `b2-utils-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: A useful package provided by B2BIT
 Author-email: Felipe Sena 🏎️ <felipesena@b2bit.company>, Matheus Abdias 🐧 <matheusabdias.b2bit@gmail.com>
 Project-URL: Homepage, https://gitlab.com/b2bit.felipesena/b2-utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `b2-utils-0.2.2/README.md` & `b2-utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/pyproject.toml` & `b2-utils-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "b2-utils"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name = "Felipe Sena 🏎️", email = "felipesena@b2bit.company" },
     { name = "Matheus Abdias 🐧", email = "matheusabdias.b2bit@gmail.com" },
 ]
 description = "A useful package provided by B2BIT"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `b2-utils-0.2.2/src/b2_utils/context.py` & `b2-utils-0.2.3/src/b2_utils/context.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/decorators.py` & `b2-utils-0.2.3/src/b2_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/enums.py` & `b2-utils-0.2.3/src/b2_utils/enums.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/faker/providers.py` & `b2-utils-0.2.3/src/b2_utils/faker/providers.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/fields.py` & `b2-utils-0.2.3/src/b2_utils/fields.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/helpers/__init__.py` & `b2-utils-0.2.3/src/b2_utils/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/helpers/auth.py` & `b2-utils-0.2.3/src/b2_utils/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/helpers.py` & `b2-utils-0.2.3/src/b2_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/mixins.py` & `b2-utils-0.2.3/src/b2_utils/mixins.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/permissions.py` & `b2-utils-0.2.3/src/b2_utils/permissions.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/serializers/__init__.py` & `b2-utils-0.2.3/src/b2_utils/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/serializers/relations.py` & `b2-utils-0.2.3/src/b2_utils/serializers/relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             }
         else:
             kwargs["instance"] = self.queryset.get(pk=value.pk)
 
         if self.representation_fields:
             kwargs["fields"] = self.representation_fields
 
-        return self.representation_serializer(**kwargs).data
+        return self.representation_serializer(context=self.context, **kwargs).data
 
 
 class DynamicFieldsSerializer:
     def __init__(self, *args, **kwargs) -> None:
         fields = kwargs.pop("fields", None)
 
         super().__init__(*args, **kwargs)
```

### Comparing `b2-utils-0.2.2/src/b2_utils/tasks.py` & `b2-utils-0.2.3/src/b2_utils/tasks.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/templatetags/b2_utils.py` & `b2-utils-0.2.3/src/b2_utils/templatetags/b2_utils.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/tests/helpers.py` & `b2-utils-0.2.3/src/b2_utils/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/validators.py` & `b2-utils-0.2.3/src/b2_utils/validators.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils/views.py` & `b2-utils-0.2.3/src/b2_utils/views.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/b2_utils.egg-info/PKG-INFO` & `b2-utils-0.2.3/src/b2_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: A useful package provided by B2BIT
 Author-email: Felipe Sena 🏎️ <felipesena@b2bit.company>, Matheus Abdias 🐧 <matheusabdias.b2bit@gmail.com>
 Project-URL: Homepage, https://gitlab.com/b2bit.felipesena/b2-utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `b2-utils-0.2.2/src/b2_utils.egg-info/SOURCES.txt` & `b2-utils-0.2.3/src/b2_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b2-utils-0.2.2/src/manage.py` & `b2-utils-0.2.3/src/manage.py`

 * *Files identical despite different names*

