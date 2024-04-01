# Comparing `tmp/django-field-logger-0.0.8.tar.gz` & `tmp/django-field-logger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-field-logger-0.0.8.tar", last modified: Wed Jan 17 04:07:22 2024, max compression
+gzip compressed data, was "django-field-logger-0.0.9.tar", last modified: Wed Jan 17 04:32:51 2024, max compression
```

## Comparing `django-field-logger-0.0.8.tar` & `django-field-logger-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-01-17 04:07:22.839006 django-field-logger-0.0.8/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.8/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.8/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      449 2024-01-17 04:07:22.839006 django-field-logger-0.0.8/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     6474 2024-01-17 03:51:30.000000 django-field-logger-0.0.8/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-01-17 04:07:22.839006 django-field-logger-0.0.8/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      449 2024-01-17 04:07:22.000000 django-field-logger-0.0.8/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      411 2024-01-17 04:07:22.000000 django-field-logger-0.0.8/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-01-17 04:07:22.000000 django-field-logger-0.0.8/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2024-01-17 04:07:22.000000 django-field-logger-0.0.8/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-01-17 04:07:22.000000 django-field-logger-0.0.8/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-01-17 04:07:22.839006 django-field-logger-0.0.8/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.8/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.8/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2712 2024-01-16 23:45:31.000000 django-field-logger-0.0.8/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      990 2024-01-17 02:20:44.000000 django-field-logger-0.0.8/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2083 2024-01-17 01:19:22.000000 django-field-logger-0.0.8/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      882 2024-01-16 20:10:17.000000 django-field-logger-0.0.8/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      306 2024-01-17 02:28:29.000000 django-field-logger-0.0.8/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2024-01-17 04:07:22.839006 django-field-logger-0.0.8/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      736 2024-01-17 04:05:49.000000 django-field-logger-0.0.8/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-01-17 04:32:51.518648 django-field-logger-0.0.9/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.9/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.9/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      449 2024-01-17 04:32:51.518648 django-field-logger-0.0.9/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     6732 2024-01-17 04:32:03.000000 django-field-logger-0.0.9/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-01-17 04:32:51.518648 django-field-logger-0.0.9/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      449 2024-01-17 04:32:51.000000 django-field-logger-0.0.9/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      433 2024-01-17 04:32:51.000000 django-field-logger-0.0.9/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-01-17 04:32:51.000000 django-field-logger-0.0.9/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2024-01-17 04:32:51.000000 django-field-logger-0.0.9/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-01-17 04:32:51.000000 django-field-logger-0.0.9/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-01-17 04:32:51.518648 django-field-logger-0.0.9/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.9/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.9/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2712 2024-01-16 23:45:31.000000 django-field-logger-0.0.9/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      990 2024-01-17 02:20:44.000000 django-field-logger-0.0.9/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      345 2024-01-17 04:30:09.000000 django-field-logger-0.0.9/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2083 2024-01-17 01:19:22.000000 django-field-logger-0.0.9/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      882 2024-01-16 20:10:17.000000 django-field-logger-0.0.9/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      306 2024-01-17 02:28:29.000000 django-field-logger-0.0.9/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2024-01-17 04:32:51.518648 django-field-logger-0.0.9/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      736 2024-01-17 04:19:53.000000 django-field-logger-0.0.9/setup.py
```

### Comparing `django-field-logger-0.0.8/LICENSE` & `django-field-logger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.8/README.md` & `django-field-logger-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -169,7 +169,15 @@
 
 Additionally, ```FieldLog``` model provides the following properties:
 
 - ```model_class```: returns the model class of the instance that is being logged.
 - ```instance```: returns the instance that is being logged.
 - ```previous_log```: returns the previous log of the instance that is being logged.
 - ```created```: returns True if the log is the first one for that field in that instance, False otherwise.
+
+
+### The FieldLoggerMixin
+
+This package provides you a mixin class which is called ```FieldLoggerMixin```.
+This mixin class provides you the following property:
+
+- ```fieldlog_set``` returns the ```FieldLog``` queryset of the instance that is being logged.
```

### Comparing `django-field-logger-0.0.8/fieldlogger/config.py` & `django-field-logger-0.0.9/fieldlogger/config.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.8/fieldlogger/fieldlogger.py` & `django-field-logger-0.0.9/fieldlogger/fieldlogger.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.8/fieldlogger/models.py` & `django-field-logger-0.0.9/fieldlogger/models.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.8/fieldlogger/signals.py` & `django-field-logger-0.0.9/fieldlogger/signals.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.8/setup.py` & `django-field-logger-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="django-field-logger",
-    version="0.0.8",
+    version="0.0.9",
     author="Sergio Rodríguez",
     author_email="srodriguez3441@gmail.com",
     description="""A python package which logs each change made to a Django model instance.""",
     url="https://github.com/nibblex/django-field-logger",
     packages=setuptools.find_packages(),
     license="MIT",
     classifiers=[
```

