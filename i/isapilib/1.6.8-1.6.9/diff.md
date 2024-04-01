# Comparing `tmp/isapilib-1.6.8.tar.gz` & `tmp/isapilib-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isapilib-1.6.8.tar", last modified: Mon Mar 25 16:52:07 2024, max compression
+gzip compressed data, was "isapilib-1.6.9.tar", last modified: Mon Apr  1 16:21:37 2024, max compression
```

## Comparing `isapilib-1.6.8.tar` & `isapilib-1.6.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.757779 isapilib-1.6.8/
--rw-rw-rw-   0        0        0       67 2024-02-19 22:40:27.000000 isapilib-1.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0      209 2024-03-25 16:52:07.754420 isapilib-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-10-30 17:02:35.000000 isapilib-1.6.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.664800 isapilib-1.6.8/app/
--rw-rw-rw-   0        0        0        0 2024-01-19 19:11:10.000000 isapilib-1.6.8/app/__init__.py
--rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.6.8/app/asgi.py
--rw-rw-rw-   0        0        0     3416 2024-01-19 19:13:38.000000 isapilib-1.6.8/app/settings.py
--rw-rw-rw-   0        0        0      781 2024-02-19 17:24:37.000000 isapilib-1.6.8/app/urls.py
--rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.6.8/app/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.688661 isapilib-1.6.8/isapilib/
--rw-rw-rw-   0        0        0     3364 2024-02-20 15:50:12.000000 isapilib-1.6.8/isapilib/Connection.py
--rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.8/isapilib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.707939 isapilib-1.6.8/isapilib/api/
--rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.8/isapilib/api/__init__.py
--rw-rw-rw-   0        0        0    32245 2024-03-07 23:22:51.000000 isapilib-1.6.8/isapilib/api/models.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.715090 isapilib-1.6.8/isapilib/core/
--rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.8/isapilib/core/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-01-24 23:50:14.000000 isapilib-1.6.8/isapilib/core/models.py
--rw-rw-rw-   0        0        0     1404 2024-03-21 18:17:56.000000 isapilib-1.6.8/isapilib/decorators.py
--rw-rw-rw-   0        0        0      378 2024-03-12 17:04:53.000000 isapilib-1.6.8/isapilib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.718178 isapilib-1.6.8/isapilib/management/
--rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.8/isapilib/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.726948 isapilib-1.6.8/isapilib/management/commands/
--rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.8/isapilib/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1167 2024-03-07 23:41:08.000000 isapilib-1.6.8/isapilib/management/commands/check_branch.py
--rw-rw-rw-   0        0        0     1360 2024-03-07 23:25:53.000000 isapilib-1.6.8/isapilib/management/commands/external_migrate.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.734258 isapilib-1.6.8/isapilib/migrations/
--rw-rw-rw-   0        0        0    46380 2024-02-19 17:39:52.000000 isapilib-1.6.8/isapilib/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.8/isapilib/migrations/__init__.py
--rw-rw-rw-   0        0        0     8155 2024-02-20 18:28:12.000000 isapilib-1.6.8/isapilib/models.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.643454 isapilib-1.6.8/isapilib/static/
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.737521 isapilib-1.6.8/isapilib/static/css/
--rw-rw-rw-   0        0        0   232948 2024-02-19 22:23:07.000000 isapilib-1.6.8/isapilib/static/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.744175 isapilib-1.6.8/isapilib/static/img/
--rw-rw-rw-   0        0        0     1638 2024-02-19 17:54:17.000000 isapilib-1.6.8/isapilib/static/img/intelisis128.png
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.747180 isapilib-1.6.8/isapilib/templates/
--rw-rw-rw-   0        0        0     1836 2024-02-20 00:24:37.000000 isapilib-1.6.8/isapilib/templates/index.html
--rw-rw-rw-   0        0        0      124 2024-02-19 23:15:50.000000 isapilib-1.6.8/isapilib/urls.py
--rw-rw-rw-   0        0        0     3873 2024-03-21 18:17:56.000000 isapilib-1.6.8/isapilib/utilities.py
--rw-rw-rw-   0        0        0     1414 2024-03-25 16:51:47.000000 isapilib-1.6.8/isapilib/views.py
-drwxrwxrwx   0        0        0        0 2024-03-25 16:52:07.751353 isapilib-1.6.8/isapilib.egg-info/
--rw-rw-rw-   0        0        0      209 2024-03-25 16:52:07.000000 isapilib-1.6.8/isapilib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2024-03-25 16:52:07.000000 isapilib-1.6.8/isapilib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 16:52:07.000000 isapilib-1.6.8/isapilib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-03-25 16:52:07.000000 isapilib-1.6.8/isapilib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-25 16:52:07.000000 isapilib-1.6.8/isapilib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 16:52:07.757779 isapilib-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0      435 2024-03-25 16:52:05.000000 isapilib-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.840210 isapilib-1.6.9/
+-rw-rw-rw-   0        0        0       67 2024-02-19 22:40:27.000000 isapilib-1.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      209 2024-04-01 16:21:37.838146 isapilib-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-10-30 17:02:35.000000 isapilib-1.6.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.786300 isapilib-1.6.9/app/
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:11:10.000000 isapilib-1.6.9/app/__init__.py
+-rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.6.9/app/asgi.py
+-rw-rw-rw-   0        0        0     3416 2024-01-19 19:13:38.000000 isapilib-1.6.9/app/settings.py
+-rw-rw-rw-   0        0        0      781 2024-02-19 17:24:37.000000 isapilib-1.6.9/app/urls.py
+-rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.6.9/app/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.805418 isapilib-1.6.9/isapilib/
+-rw-rw-rw-   0        0        0     3364 2024-02-20 15:50:12.000000 isapilib-1.6.9/isapilib/Connection.py
+-rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.9/isapilib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.816019 isapilib-1.6.9/isapilib/api/
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.9/isapilib/api/__init__.py
+-rw-rw-rw-   0        0        0    32245 2024-03-27 20:02:07.000000 isapilib-1.6.9/isapilib/api/models.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.819674 isapilib-1.6.9/isapilib/core/
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.9/isapilib/core/__init__.py
+-rw-rw-rw-   0        0        0     2047 2024-04-01 14:35:05.000000 isapilib-1.6.9/isapilib/core/models.py
+-rw-rw-rw-   0        0        0     1404 2024-03-21 18:17:56.000000 isapilib-1.6.9/isapilib/decorators.py
+-rw-rw-rw-   0        0        0      378 2024-03-12 17:04:53.000000 isapilib-1.6.9/isapilib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.821189 isapilib-1.6.9/isapilib/management/
+-rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.9/isapilib/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.825924 isapilib-1.6.9/isapilib/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.9/isapilib/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1167 2024-03-07 23:41:08.000000 isapilib-1.6.9/isapilib/management/commands/check_branch.py
+-rw-rw-rw-   0        0        0     1360 2024-03-07 23:25:53.000000 isapilib-1.6.9/isapilib/management/commands/external_migrate.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.829935 isapilib-1.6.9/isapilib/migrations/
+-rw-rw-rw-   0        0        0    46380 2024-02-19 17:39:52.000000 isapilib-1.6.9/isapilib/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.9/isapilib/migrations/__init__.py
+-rw-rw-rw-   0        0        0     8155 2024-02-20 18:28:12.000000 isapilib-1.6.9/isapilib/models.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.774554 isapilib-1.6.9/isapilib/static/
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.831538 isapilib-1.6.9/isapilib/static/css/
+-rw-rw-rw-   0        0        0   232948 2024-02-19 22:23:07.000000 isapilib-1.6.9/isapilib/static/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.833460 isapilib-1.6.9/isapilib/static/img/
+-rw-rw-rw-   0        0        0     1638 2024-02-19 17:54:17.000000 isapilib-1.6.9/isapilib/static/img/intelisis128.png
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.834514 isapilib-1.6.9/isapilib/templates/
+-rw-rw-rw-   0        0        0     1836 2024-02-20 00:24:37.000000 isapilib-1.6.9/isapilib/templates/index.html
+-rw-rw-rw-   0        0        0      124 2024-02-19 23:15:50.000000 isapilib-1.6.9/isapilib/urls.py
+-rw-rw-rw-   0        0        0     3873 2024-03-21 18:17:56.000000 isapilib-1.6.9/isapilib/utilities.py
+-rw-rw-rw-   0        0        0     1414 2024-03-25 16:51:47.000000 isapilib-1.6.9/isapilib/views.py
+drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.837051 isapilib-1.6.9/isapilib.egg-info/
+-rw-rw-rw-   0        0        0      209 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 16:21:37.840210 isapilib-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      435 2024-04-01 16:21:36.000000 isapilib-1.6.9/setup.py
```

### Comparing `isapilib-1.6.8/app/settings.py` & `isapilib-1.6.9/app/settings.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/app/urls.py` & `isapilib-1.6.9/app/urls.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/Connection.py` & `isapilib-1.6.9/isapilib/Connection.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/api/models.py` & `isapilib-1.6.9/isapilib/api/models.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/core/models.py` & `isapilib-1.6.9/isapilib/core/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 from django.db import models
 
 from isapilib.utilities import execute_query
 
 
 class BaseModel(models.Model):
 
+    def _add_field(self, name):
+        new_field = models.TextField(db_column=name)
+        new_field.contribute_to_class(self, name)
+
+    def get(self, name):
+        if name not in [field.attname for field in self._meta.get_fields()]:
+            self._add_field(name)
+
+        return getattr(self, name)
+
+    def set(self, name, value):
+        if name not in [field.attname for field in self._meta.get_fields()]:
+            self._add_field(name)
+
+        setattr(self, name, value)
+
     def get_triggers(self, disabled=0, using='default'):
         tb_name = self._meta.db_table
         return execute_query('SELECT name FROM sys.triggers WHERE parent_id = OBJECT_ID(%s) AND is_disabled = %s',
                              [tb_name, disabled], using=using)
 
     def enable_trigger(self, name, using='default'):
         try:
```

### Comparing `isapilib-1.6.8/isapilib/decorators.py` & `isapilib-1.6.9/isapilib/decorators.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/management/commands/check_branch.py` & `isapilib-1.6.9/isapilib/management/commands/check_branch.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/management/commands/external_migrate.py` & `isapilib-1.6.9/isapilib/management/commands/external_migrate.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/migrations/0001_initial.py` & `isapilib-1.6.9/isapilib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/models.py` & `isapilib-1.6.9/isapilib/models.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/static/css/bootstrap.min.css` & `isapilib-1.6.9/isapilib/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/static/img/intelisis128.png` & `isapilib-1.6.9/isapilib/static/img/intelisis128.png`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/templates/index.html` & `isapilib-1.6.9/isapilib/templates/index.html`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/utilities.py` & `isapilib-1.6.9/isapilib/utilities.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib/views.py` & `isapilib-1.6.9/isapilib/views.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.8/isapilib.egg-info/SOURCES.txt` & `isapilib-1.6.9/isapilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

