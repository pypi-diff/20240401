# Comparing `tmp/drf-spectacular-0.9.8.tar.gz` & `tmp/drf-spectacular-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-spectacular-0.9.8.tar", last modified: Sun Jun  7 21:35:10 2020, max compression
+gzip compressed data, was "dist/drf-spectacular-0.9.9.tar", last modified: Sat Jun 20 13:15:23 2020, max compression
```

## Comparing `drf-spectacular-0.9.8.tar` & `drf-spectacular-0.9.9.tar`

### file list

```diff
@@ -1,53 +1,110 @@
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/
--rw-rw-r--   0 ins       (1000) ins       (1000)    10617 2020-06-07 21:20:14.000000 drf-spectacular-0.9.8/CHANGELOG.rst
--rw-rw-r--   0 ins       (1000) ins       (1000)     1589 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/LICENSE
--rw-rw-r--   0 ins       (1000) ins       (1000)      213 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/MANIFEST.in
--rw-rw-r--   0 ins       (1000) ins       (1000)    10900 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/PKG-INFO
--rw-rw-r--   0 ins       (1000) ins       (1000)     8006 2020-06-05 18:08:54.000000 drf-spectacular-0.9.8/README.rst
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/
--rw-rw-r--   0 ins       (1000) ins       (1000)       22 2020-06-07 21:17:58.000000 drf-spectacular-0.9.8/drf_spectacular/__init__.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     1041 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/authentication.py
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/contrib/
--rw-rw-r--   0 ins       (1000) ins       (1000)      161 2020-06-05 18:26:17.000000 drf-spectacular-0.9.8/drf_spectacular/contrib/__init__.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     2234 2020-06-05 18:15:19.000000 drf-spectacular-0.9.8/drf_spectacular/contrib/django_oauth_toolkit.py
--rw-rw-r--   0 ins       (1000) ins       (1000)      691 2020-06-05 18:08:54.000000 drf-spectacular-0.9.8/drf_spectacular/contrib/djangorestframework_camel_case.py
--rw-rw-r--   0 ins       (1000) ins       (1000)      491 2020-06-05 18:15:35.000000 drf-spectacular-0.9.8/drf_spectacular/contrib/rest_framework_jwt.py
--rw-rw-r--   0 ins       (1000) ins       (1000)      790 2020-06-05 18:15:47.000000 drf-spectacular-0.9.8/drf_spectacular/contrib/rest_framework_simplejwt.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     1277 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/contrib/rest_polymorphic.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     1841 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/extensions.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     6691 2020-05-31 15:38:06.000000 drf-spectacular-0.9.8/drf_spectacular/generators.py
--rw-rw-r--   0 ins       (1000) ins       (1000)      922 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/helpers.py
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/management/
--rw-rw-r--   0 ins       (1000) ins       (1000)        0 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/management/__init__.py
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/management/commands/
--rw-rw-r--   0 ins       (1000) ins       (1000)        0 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/management/commands/__init__.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     2832 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/management/commands/spectacular.py
--rw-rw-r--   0 ins       (1000) ins       (1000)    40206 2020-06-07 15:55:44.000000 drf-spectacular-0.9.8/drf_spectacular/openapi.py
--rw-rw-r--   0 ins       (1000) ins       (1000)    23209 2020-06-06 16:50:24.000000 drf-spectacular-0.9.8/drf_spectacular/plumbing.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     1765 2020-06-06 19:39:57.000000 drf-spectacular-0.9.8/drf_spectacular/renderers.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     1760 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/serializers.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     2834 2020-05-31 15:38:09.000000 drf-spectacular-0.9.8/drf_spectacular/settings.py
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/templates/
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/templates/drf_spectacular/
--rw-rw-r--   0 ins       (1000) ins       (1000)      640 2020-05-31 16:45:29.000000 drf-spectacular-0.9.8/drf_spectacular/templates/drf_spectacular/redoc.html
--rw-rw-r--   0 ins       (1000) ins       (1000)      829 2020-05-31 16:45:23.000000 drf-spectacular-0.9.8/drf_spectacular/templates/drf_spectacular/swagger_ui.html
--rw-rw-r--   0 ins       (1000) ins       (1000)     2549 2020-05-26 08:07:10.000000 drf-spectacular-0.9.8/drf_spectacular/types.py
--rw-rw-r--   0 ins       (1000) ins       (1000)     8906 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/utils.py
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular/validation/
--rw-rw-r--   0 ins       (1000) ins       (1000)      869 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/validation/__init__.py
--rw-rw-r--   0 ins       (1000) ins       (1000)    35456 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/drf_spectacular/validation/openapi3_schema.json
--rw-rw-r--   0 ins       (1000) ins       (1000)     2955 2020-06-06 17:34:40.000000 drf-spectacular-0.9.8/drf_spectacular/views.py
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/drf_spectacular.egg-info/
--rw-rw-r--   0 ins       (1000) ins       (1000)    10900 2020-06-07 21:35:09.000000 drf-spectacular-0.9.8/drf_spectacular.egg-info/PKG-INFO
--rw-rw-r--   0 ins       (1000) ins       (1000)     1367 2020-06-07 21:35:09.000000 drf-spectacular-0.9.8/drf_spectacular.egg-info/SOURCES.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)        1 2020-06-07 21:35:09.000000 drf-spectacular-0.9.8/drf_spectacular.egg-info/dependency_links.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)      105 2020-06-07 21:35:09.000000 drf-spectacular-0.9.8/drf_spectacular.egg-info/requires.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)      130 2020-06-07 21:35:09.000000 drf-spectacular-0.9.8/drf_spectacular.egg-info/top_level.txt
-drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/requirements/
--rw-rw-r--   0 ins       (1000) ins       (1000)      104 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/requirements/base.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)       30 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/requirements/docs.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)      176 2020-06-07 16:03:12.000000 drf-spectacular-0.9.8/requirements/optionals.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)       27 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/requirements/packaging.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)      112 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/requirements/testing.txt
--rw-rw-r--   0 ins       (1000) ins       (1000)       67 2020-06-07 21:35:10.039870 drf-spectacular-0.9.8/setup.cfg
--rw-rw-r--   0 ins       (1000) ins       (1000)     3125 2020-05-21 19:05:10.000000 drf-spectacular-0.9.8/setup.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/
+-rw-rw-r--   0 ins       (1000) ins       (1000)    11535 2020-06-20 13:05:31.000000 drf-spectacular-0.9.9/CHANGELOG.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1589 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/LICENSE
+-rw-rw-r--   0 ins       (1000) ins       (1000)      313 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/MANIFEST.in
+-rw-rw-r--   0 ins       (1000) ins       (1000)    10913 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/PKG-INFO
+-rw-rw-r--   0 ins       (1000) ins       (1000)     8006 2020-06-05 18:08:54.000000 drf-spectacular-0.9.9/README.rst
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/docs/
+-rw-rw-r--   0 ins       (1000) ins       (1000)      634 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/docs/Makefile
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/docs/blueprints/
+-rw-rw-r--   0 ins       (1000) ins       (1000)      745 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/docs/blueprints/djstripe.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     3672 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/docs/blueprints/oscarapi.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1416 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/docs/blueprints.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)       29 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/docs/changelog.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1987 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/docs/conf.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     7623 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/docs/customization.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)      784 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/docs/drf_spectacular.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)      886 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/docs/drf_yasg.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)     5406 2020-06-05 18:08:54.000000 drf-spectacular-0.9.9/docs/faq.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1364 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/docs/index.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)       48 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/docs/license.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)      795 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/docs/make.bat
+-rw-rw-r--   0 ins       (1000) ins       (1000)       26 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/docs/readme.rst
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1135 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/docs/settings.rst
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular/
+-rw-rw-r--   0 ins       (1000) ins       (1000)       22 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/drf_spectacular/__init__.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1041 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/drf_spectacular/authentication.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular/contrib/
+-rw-rw-r--   0 ins       (1000) ins       (1000)      161 2020-06-05 18:26:17.000000 drf-spectacular-0.9.9/drf_spectacular/contrib/__init__.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2234 2020-06-05 18:15:19.000000 drf-spectacular-0.9.9/drf_spectacular/contrib/django_oauth_toolkit.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)      691 2020-06-05 18:08:54.000000 drf-spectacular-0.9.9/drf_spectacular/contrib/djangorestframework_camel_case.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)      491 2020-06-05 18:15:35.000000 drf-spectacular-0.9.9/drf_spectacular/contrib/rest_framework_jwt.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)      790 2020-06-05 18:15:47.000000 drf-spectacular-0.9.9/drf_spectacular/contrib/rest_framework_simplejwt.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1277 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/contrib/rest_polymorphic.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1841 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/extensions.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     6692 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/drf_spectacular/generators.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)      922 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/helpers.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular/management/
+-rw-rw-r--   0 ins       (1000) ins       (1000)        0 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/management/__init__.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular/management/commands/
+-rw-rw-r--   0 ins       (1000) ins       (1000)        0 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/management/commands/__init__.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2832 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/drf_spectacular/management/commands/spectacular.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)    40587 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/drf_spectacular/openapi.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)    24313 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/drf_spectacular/plumbing.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1765 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/drf_spectacular/renderers.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2515 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/drf_spectacular/serializers.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2834 2020-05-31 15:38:09.000000 drf-spectacular-0.9.9/drf_spectacular/settings.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular/templates/
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular/templates/drf_spectacular/
+-rw-rw-r--   0 ins       (1000) ins       (1000)      642 2020-06-20 12:18:27.000000 drf-spectacular-0.9.9/drf_spectacular/templates/drf_spectacular/redoc.html
+-rw-rw-r--   0 ins       (1000) ins       (1000)      831 2020-06-20 12:18:27.000000 drf-spectacular-0.9.9/drf_spectacular/templates/drf_spectacular/swagger_ui.html
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2549 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/drf_spectacular/types.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)    10358 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/drf_spectacular/utils.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/drf_spectacular/validation/
+-rw-rw-r--   0 ins       (1000) ins       (1000)      869 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/validation/__init__.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)    35456 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/drf_spectacular/validation/openapi3_schema.json
+-rw-rw-r--   0 ins       (1000) ins       (1000)     3010 2020-06-20 12:32:07.000000 drf-spectacular-0.9.9/drf_spectacular/views.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.530807 drf-spectacular-0.9.9/drf_spectacular.egg-info/
+-rw-rw-r--   0 ins       (1000) ins       (1000)    10913 2020-06-20 13:15:23.000000 drf-spectacular-0.9.9/drf_spectacular.egg-info/PKG-INFO
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2679 2020-06-20 13:15:23.000000 drf-spectacular-0.9.9/drf_spectacular.egg-info/SOURCES.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)        1 2020-06-20 13:15:23.000000 drf-spectacular-0.9.9/drf_spectacular.egg-info/dependency_links.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)      105 2020-06-20 13:15:23.000000 drf-spectacular-0.9.9/drf_spectacular.egg-info/requires.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)      130 2020-06-20 13:15:23.000000 drf-spectacular-0.9.9/drf_spectacular.egg-info/top_level.txt
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/requirements/
+-rw-rw-r--   0 ins       (1000) ins       (1000)      104 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/requirements/base.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)       30 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/requirements/docs.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)      174 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/requirements/optionals.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)       27 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/requirements/packaging.txt
+-rw-rw-r--   0 ins       (1000) ins       (1000)      125 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/requirements/testing.txt
+-rwxrwxr-x   0 ins       (1000) ins       (1000)     2869 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/runtests.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)       67 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/setup.cfg
+-rw-rw-r--   0 ins       (1000) ins       (1000)     3136 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/setup.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/tests/
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1797 2020-06-11 15:13:55.000000 drf-spectacular-0.9.9/tests/__init__.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     3935 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/conftest.py
+drwxrwxr-x   0 ins       (1000) ins       (1000)        0 2020-06-20 13:15:23.534807 drf-spectacular-0.9.9/tests/contrib/
+-rw-rw-r--   0 ins       (1000) ins       (1000)        0 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/contrib/__init__.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1090 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/contrib/test_djangorestframework_camel_case.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1167 2020-06-06 19:39:57.000000 drf-spectacular-0.9.9/tests/contrib/test_djangorestframework_camel_case.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1135 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/contrib/test_drf_jwt.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2091 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/tests/contrib/test_drf_jwt.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2882 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/contrib/test_oauth_toolkit.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1919 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/contrib/test_oauth_toolkit.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     3212 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/contrib/test_rest_polymorphic.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     6459 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/contrib/test_rest_polymorphic.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1245 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/contrib/test_simplejwt.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2678 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/contrib/test_simplejwt.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)       59 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/models.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2252 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/tests/test_basic.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     6223 2020-05-22 21:06:52.000000 drf-spectacular-0.9.9/tests/test_basic.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)      353 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/test_command.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     6508 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/test_extend_schema.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     8174 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/test_extend_schema.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2724 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/test_extensions.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     6844 2020-06-11 14:09:25.000000 drf-spectacular-0.9.9/tests/test_fields.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     7526 2020-06-06 16:38:57.000000 drf-spectacular-0.9.9/tests/test_fields.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2010 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/tests/test_meta.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)      962 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/tests/test_plumbing.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2391 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/test_polymorphic.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1947 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/test_polymorphic.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     2855 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/tests/test_postprocessing.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1355 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/test_postprocessing.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1530 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/tests/test_recursion.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1209 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/test_recursion.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)    24590 2020-06-20 11:33:26.000000 drf-spectacular-0.9.9/tests/test_regressions.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     5503 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/tests/test_versioning.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1274 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/tests/test_versioning_v1.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     1296 2020-05-26 08:07:10.000000 drf-spectacular-0.9.9/tests/test_versioning_v2.yml
+-rw-rw-r--   0 ins       (1000) ins       (1000)     3437 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/tests/test_view.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)     5050 2020-06-11 13:32:34.000000 drf-spectacular-0.9.9/tests/test_warnings.py
+-rw-rw-r--   0 ins       (1000) ins       (1000)       17 2020-05-21 19:05:10.000000 drf-spectacular-0.9.9/tests/urls.py
```

### Comparing `drf-spectacular-0.9.8/CHANGELOG.rst` & `drf-spectacular-0.9.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changelog
 =========
 
+0.9.9 (2020-06-20)
+------------------
+
+- added explicit URL option to UI views. `#103 <https://github.com/tfranzel/drf-spectacular/issues/103>`_
+- improve auth extension doc `#99 <https://github.com/tfranzel/drf-spectacular/issues/99>`_
+- bugfix attr typo with Token auth extension `#99 <https://github.com/tfranzel/drf-spectacular/issues/99>`_
+- improve docstring extraction `#96 <https://github.com/tfranzel/drf-spectacular/issues/96>`_
+- Manual polymorphic [Jair Henrique]
+- Add summary field to extend_schema `#97 <https://github.com/tfranzel/drf-spectacular/issues/97>`_ [lilisha100]
+- reduce minimal package requirements
+- extend sdist with tests & doc
+- bugfix nested RO/WO serializer on COMPONENT_SPLIT_REQUEST
+- add pytest option --skip-missing-contrib `#87 <https://github.com/tfranzel/drf-spectacular/issues/87>`_
+- Save test files in temporary folder [Jair Henrique]
+- Setup isort library [Jair Henrique]
+
 0.9.8 (2020-06-07)
 ------------------
 
 - bugfix read-only many2many relation processing `#79 <https://github.com/tfranzel/drf-spectacular/issues/79>`_
 - Implement OrderedDict representer for yaml dumper [Jair Henrique]
 - bugfix UI permissions `#84 <https://github.com/tfranzel/drf-spectacular/issues/84>`_
 - fix abc import `#82 <https://github.com/tfranzel/drf-spectacular/issues/82>`_
```

### Comparing `drf-spectacular-0.9.8/LICENSE` & `drf-spectacular-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/PKG-INFO` & `drf-spectacular-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-spectacular
-Version: 0.9.8
+Version: 0.9.9
 Summary: Sane and flexible OpenAPI 3 schema generation for Django REST framework
 Home-page: https://github.com/tfranzel/drf-spectacular
 Author: T. Franzel
 Author-email: tfranzel@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/tfranzel/drf-spectacular
 Project-URL: Documentation, https://drf-spectacular.readthedocs.io
@@ -218,15 +218,15 @@
            :target: https://pypi.python.org/pypi/drf-spectacular
         .. |codecov| image:: https://codecov.io/gh/tfranzel/drf-spectacular/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/tfranzel/drf-spectacular
         .. |docs| image:: https://readthedocs.org/projects/drf-spectacular/badge/
            :target: https://drf-spectacular.readthedocs.io/
         
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `drf-spectacular-0.9.8/README.rst` & `drf-spectacular-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/authentication.py` & `drf-spectacular-0.9.9/drf_spectacular/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             'scheme': 'basic',
         }
 
 
 class TokenScheme(OpenApiAuthenticationExtension):
     target_class = 'rest_framework.authentication.TokenAuthentication'
     name = 'tokenAuth'
-    matches_subclass = True
+    match_subclasses = True
 
     def get_security_definition(self, auto_schema):
         return {
             'type': 'http',
             'scheme': 'bearer',
             'bearerFormat': self.target.keyword,
         }
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/contrib/django_oauth_toolkit.py` & `drf-spectacular-0.9.9/drf_spectacular/contrib/django_oauth_toolkit.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/contrib/djangorestframework_camel_case.py` & `drf-spectacular-0.9.9/drf_spectacular/contrib/djangorestframework_camel_case.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/contrib/rest_framework_simplejwt.py` & `drf-spectacular-0.9.9/drf_spectacular/contrib/rest_framework_simplejwt.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/contrib/rest_polymorphic.py` & `drf-spectacular-0.9.9/drf_spectacular/contrib/rest_polymorphic.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/extensions.py` & `drf-spectacular-0.9.9/drf_spectacular/extensions.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/generators.py` & `drf-spectacular-0.9.9/drf_spectacular/generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import inspect
 from urllib.parse import urljoin
 
-from django.urls import URLResolver, URLPattern
-from rest_framework import viewsets, views
+from django.urls import URLPattern, URLResolver
+from rest_framework import views, viewsets
 from rest_framework.schemas.generators import BaseSchemaGenerator  # type: ignore
 from rest_framework.schemas.generators import EndpointEnumerator as BaseEndpointEnumerator
 
 from drf_spectacular.extensions import OpenApiViewExtension
 from drf_spectacular.plumbing import (
-    ComponentRegistry, error, alpha_operation_sorter, reset_generator_stats, build_root_object,
-    modify_for_versioning, operation_matches_version, warn, is_versioning_supported
+    ComponentRegistry, alpha_operation_sorter, build_root_object, error, is_versioning_supported,
+    modify_for_versioning, operation_matches_version, reset_generator_stats, warn,
 )
 from drf_spectacular.settings import spectacular_settings
 
 
 class EndpointEnumerator(BaseEndpointEnumerator):
     def get_api_endpoints(self, patterns=None, prefix=''):
         """
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/helpers.py` & `drf-spectacular-0.9.9/drf_spectacular/helpers.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/management/commands/spectacular.py` & `drf-spectacular-0.9.9/drf_spectacular/management/commands/spectacular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from textwrap import dedent
 
 from django.core.management.base import BaseCommand
 from django.utils.module_loading import import_string
 
-from drf_spectacular.settings import spectacular_settings
 from drf_spectacular.plumbing import GENERATOR_STATS
-from drf_spectacular.renderers import OpenApiYamlRenderer, OpenApiJsonRenderer
+from drf_spectacular.renderers import OpenApiJsonRenderer, OpenApiYamlRenderer
+from drf_spectacular.settings import spectacular_settings
 from drf_spectacular.validation import validate_schema
 
 
 class Command(BaseCommand):
     help = dedent("""
         Generate a spectacular OpenAPI3-compliant schema for your API.
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/openapi.py` & `drf-spectacular-0.9.9/drf_spectacular/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-import inspect
 import re
 import typing
 from operator import attrgetter
 
 import uritemplate
-from django.core import validators, exceptions as django_exceptions
+from django.core import exceptions as django_exceptions
+from django.core import validators
 from django.db import models
 from rest_framework import permissions, renderers, serializers
 from rest_framework.fields import _UnvalidatedField, empty
 from rest_framework.generics import GenericAPIView
 from rest_framework.mixins import ListModelMixin
 from rest_framework.schemas.inspectors import ViewInspector
 from rest_framework.schemas.utils import get_pk_description  # type: ignore
 from rest_framework.settings import api_settings
 from rest_framework.utils.model_meta import get_field_info
 from rest_framework.views import APIView
 
-from drf_spectacular.extensions import (
-    OpenApiSerializerFieldExtension, OpenApiSerializerExtension
-)
-from drf_spectacular.settings import spectacular_settings
+from drf_spectacular.authentication import OpenApiAuthenticationExtension
 from drf_spectacular.contrib import *  # noqa: F403, F401
+from drf_spectacular.extensions import OpenApiSerializerExtension, OpenApiSerializerFieldExtension
 from drf_spectacular.plumbing import (
-    build_basic_type, warn, anyisinstance, force_instance, is_serializer,
-    follow_field_source, is_field, is_basic_type, build_array_type,
-    ComponentRegistry, ResolvedComponent, build_parameter_type, error,
-    resolve_regex_path_parameter, safe_ref, has_override, get_override,
-    append_meta, build_object_type, build_choice_field,
+    ComponentRegistry, ResolvedComponent, anyisinstance, append_meta, build_array_type,
+    build_basic_type, build_choice_field, build_object_type, build_parameter_type, error,
+    follow_field_source, force_instance, get_doc, get_override, has_override, is_basic_type,
+    is_field, is_serializer, resolve_regex_path_parameter, safe_ref, warn,
 )
+from drf_spectacular.settings import spectacular_settings
 from drf_spectacular.types import OpenApiTypes
 from drf_spectacular.utils import OpenApiParameter
-from drf_spectacular.authentication import OpenApiAuthenticationExtension
 
 
 class AutoSchema(ViewInspector):
     method_mapping = {
         'get': 'retrieve',
         'post': 'create',
         'put': 'update',
@@ -49,14 +46,18 @@
         self.method = method
 
         operation = {}
 
         operation['operationId'] = self.get_operation_id()
         operation['description'] = self.get_description()
 
+        summary = self.get_summary()
+        if summary:
+            operation['summary'] = summary
+
         parameters = self._get_parameters()
         if parameters:
             operation['parameters'] = parameters
 
         tags = self.get_tags()
         if tags:
             operation['tags'] = tags
@@ -165,18 +166,22 @@
         for key, parameter in override_parameters.items():
             parameters[key] = parameter
         return sorted(parameters.values(), key=lambda p: p['name'])
 
     def get_description(self):
         """ override this for custom behaviour """
         action_or_method = getattr(self.view, getattr(self.view, 'action', self.method.lower()), None)
-        view_doc = inspect.getdoc(self.view) or ''
-        action_doc = inspect.getdoc(action_or_method) or ''
+        view_doc = get_doc(self.view.__class__)
+        action_doc = get_doc(action_or_method)
         return action_doc or view_doc
 
+    def get_summary(self):
+        """ override this for custom behaviour """
+        return None
+
     def get_auth(self):
         """
         Obtains authentication classes and permissions from view. If authentication
         is known, resolve security requirement for endpoint and security definition for
         the component section.
         For custom authentication subclass ``OpenApiAuthenticationExtension``.
         """
@@ -380,21 +385,21 @@
         serializer_field_extension = OpenApiSerializerFieldExtension.get_match(field)
         if serializer_field_extension:
             schema = serializer_field_extension.map_serializer_field(self, direction)
             return append_meta(schema, meta)
 
         # nested serializer
         if isinstance(field, serializers.Serializer):
-            schema = self.resolve_serializer(field, direction).ref
-            return append_meta(schema, meta)
+            component = self.resolve_serializer(field, direction)
+            return append_meta(component.ref, meta) if component else None
 
         # nested serializer with many=True gets automatically replaced with ListSerializer
         if isinstance(field, serializers.ListSerializer):
-            schema = self.resolve_serializer(field.child, direction).ref
-            return append_meta(build_array_type(schema), meta)
+            component = self.resolve_serializer(field.child, direction)
+            return append_meta(build_array_type(component.ref), meta) if component else None
 
         # Related fields.
         if isinstance(field, serializers.ManyRelatedField):
             schema = self._map_serializer_field(field.child_relation, direction)
             # remove hand-over initkwargs applying only to outer scope
             schema.pop('description', None)
             schema.pop('readOnly', None)
@@ -617,14 +622,17 @@
         properties = {}
 
         for field in serializer.fields.values():
             if isinstance(field, serializers.HiddenField):
                 continue
 
             schema = self._map_serializer_field(field, direction)
+            # skip field if there is no schema for the direction
+            if not schema:
+                continue
 
             if field.required or schema.get('readOnly'):
                 required.add(field.field_name)
 
             self._map_field_validators(field, schema)
 
             properties[field.field_name] = safe_ref(schema)
@@ -632,15 +640,15 @@
         if spectacular_settings.COMPONENT_SPLIT_PATCH:
             if self.method == 'PATCH' and direction == 'request':
                 required = []
 
         return build_object_type(
             properties=properties,
             required=required,
-            description=inspect.getdoc(serializer),
+            description=get_doc(serializer.__class__),
         )
 
     def _map_field_validators(self, field, schema):
         for v in field.validators:
             # https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#data-types
             if isinstance(v, validators.EmailValidator):
                 schema['format'] = 'email'
@@ -752,15 +760,15 @@
         request_body_required = False
         if isinstance(serializer, serializers.ListSerializer):
             component = self.resolve_serializer(serializer.child, 'request')
             schema = build_array_type(component.ref)
             request_body_required = True
         elif is_serializer(serializer):
             component = self.resolve_serializer(serializer, 'request')
-            if not component:
+            if not component.schema:
                 # serializer is empty so skip content enumeration
                 return None
             schema = component.ref
             # request body is only required if any required property is not read-only
             readonly_props = [
                 p for p, s in component.schema.get('properties', {}).items() if s.get('readOnly')
             ]
@@ -818,15 +826,15 @@
 
         if not serializer:
             return {'description': 'No response body'}
         elif isinstance(serializer, serializers.ListSerializer):
             schema = self.resolve_serializer(serializer.child, 'response').ref
         elif is_serializer(serializer):
             component = self.resolve_serializer(serializer, 'response')
-            if not component:
+            if not component.schema:
                 return {'description': 'No response body'}
             schema = component.ref
         elif is_basic_type(serializer):
             schema = build_basic_type(serializer)
         elif isinstance(serializer, dict):
             # bypass processing and use given schema directly
             schema = serializer
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/plumbing.py` & `drf-spectacular-0.9.9/drf_spectacular/plumbing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import hashlib
 import inspect
 import json
 import sys
 from abc import ABCMeta
-from collections import defaultdict, OrderedDict
+from collections import OrderedDict, defaultdict
 from collections.abc import Hashable, Iterable
 from decimal import Decimal
 from enum import Enum
-from typing import List, Type, Optional, TypeVar, Union, Generic, DefaultDict
+from typing import DefaultDict, Generic, List, Optional, Type, TypeVar, Union
 
 import inflection
 import uritemplate
 from django import __version__ as DJANGO_VERSION
 from django.urls.resolvers import _PATH_PARAMETER_COMPONENT_RE, get_resolver  # type: ignore
 from django.utils.module_loading import import_string
-from rest_framework import fields, serializers, versioning, exceptions
+from rest_framework import (
+    exceptions, fields, generics, mixins, serializers, versioning, views, viewsets,
+)
 from uritemplate import URITemplate
 
 from drf_spectacular.settings import spectacular_settings
 from drf_spectacular.types import (
-    OPENAPI_TYPE_MAPPING, PYTHON_TYPE_MAPPING, DJANGO_PATH_CONVERTER_MAPPING, OpenApiTypes
+    DJANGO_PATH_CONVERTER_MAPPING, OPENAPI_TYPE_MAPPING, PYTHON_TYPE_MAPPING, OpenApiTypes,
 )
 from drf_spectacular.utils import OpenApiParameter
 
 try:
     from django.db.models.enums import Choices  # only available in Django>3
 except ImportError:
     class Choices:  # type: ignore
@@ -127,14 +129,48 @@
 
 def get_override(obj, prop):
     if not has_override(obj, prop):
         return None
     return obj._spectacular_annotation[prop]
 
 
+def get_doc(obj):
+    """ get doc string with fallback on obj's base classes (ignoring DRF documentation). """
+    if not inspect.isclass(obj):
+        return inspect.getdoc(obj) or ''
+
+    def safe_index(lst, item):
+        try:
+            return lst.index(item)
+        except ValueError:
+            return float("inf")
+
+    lib_doc_excludes = [
+        serializers.Serializer,
+        serializers.ModelSerializer,
+        serializers.HyperlinkedModelSerializer,
+        viewsets.ModelViewSet,
+        viewsets.GenericViewSet,
+        viewsets.ViewSet,
+        viewsets.ReadOnlyModelViewSet,
+        generics.GenericAPIView,
+        mixins.ListModelMixin,
+        mixins.CreateModelMixin,
+        mixins.RetrieveModelMixin,
+        mixins.UpdateModelMixin,
+        mixins.DestroyModelMixin,
+        views.APIView,
+    ]
+    lib_barrier = min(safe_index(obj.__mro__, c) for c in lib_doc_excludes)
+    for cls in obj.__mro__[:lib_barrier]:
+        if cls.__doc__:
+            return inspect.cleandoc(cls.__doc__)
+    return ''
+
+
 def build_basic_type(obj):
     """
     resolve either enum or actual type and yield schema template for modification
     """
     if obj in OPENAPI_TYPE_MAPPING:
         return dict(OPENAPI_TYPE_MAPPING[obj])
     elif obj in PYTHON_TYPE_MAPPING:
@@ -359,15 +395,15 @@
     def __init__(self, name, type, schema=None, object=None):
         self.name = name
         self.type = type
         self.schema = schema
         self.object = object
 
     def __bool__(self):
-        return bool(self.schema)
+        return bool(self.name and self.type and self.object)
 
     @property
     def key(self):
         return self.name, self.type
 
     @property
     def ref(self) -> dict:
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/renderers.py` & `drf-spectacular-0.9.9/drf_spectacular/renderers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import OrderedDict
 
 import yaml
 from rest_framework.exceptions import ErrorDetail
-from rest_framework.renderers import JSONRenderer, BaseRenderer
+from rest_framework.renderers import BaseRenderer, JSONRenderer
 
 
 class OpenApiYamlRenderer(BaseRenderer):
     media_type = 'application/vnd.oai.openapi'
     charset = None
     format = 'openapi'
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/settings.py` & `drf-spectacular-0.9.9/drf_spectacular/settings.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/templates/drf_spectacular/redoc.html` & `drf-spectacular-0.9.9/drf_spectacular/templates/drf_spectacular/redoc.html`

 * *Files 20% similar despite different names*

```diff
@@ -14,11 +14,11 @@
       body {
         margin: 0;
         padding: 0;
       }
     </style>
   </head>
   <body>
-    <redoc spec-url="{{ url_name }}"></redoc>
+    <redoc spec-url="{{ schema_url }}"></redoc>
     <script src="https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js"> </script>
   </body>
 </html>
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/templates/drf_spectacular/swagger_ui.html` & `drf-spectacular-0.9.9/drf_spectacular/templates/drf_spectacular/swagger_ui.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" type="text/css" href="//unpkg.com/swagger-ui-dist@3/swagger-ui.css" />
   </head>
   <body>
     <div id="swagger-ui"></div>
     <script src="//unpkg.com/swagger-ui-dist@3/swagger-ui-bundle.js"></script>
     <script>
     const ui = SwaggerUIBundle({
-        url: "{{ url_name }}",
+        url: "{{ schema_url }}",
         dom_id: '#swagger-ui',
         presets: [
           SwaggerUIBundle.presets.apis,
           SwaggerUIBundle.SwaggerUIStandalonePreset
         ],
         layout: "BaseLayout",
         requestInterceptor: (request) => {
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/types.py` & `drf-spectacular-0.9.9/drf_spectacular/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import enum
-from datetime import datetime, date
+from datetime import date, datetime
 from decimal import Decimal
 from uuid import UUID
 
 
 class OpenApiTypes(enum.Enum):
     """
     Basic types known to the OpenApi specification or at least
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/utils.py` & `drf-spectacular-0.9.9/drf_spectacular/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,58 @@
 import inspect
+from typing import Dict, List, Type, Union
 
+from rest_framework.serializers import Serializer
 from rest_framework.settings import api_settings
 
+SerializerType = Union[Serializer, Type[Serializer]]
+
 
 class PolymorphicProxySerializer:
     """
     This class is to be used with :func:`@extend_schema <.extend_schema>` to
     signal a request/response might be polymorphic (accepts/returns data
-    possibly from different serializers)
+    possibly from different serializers). Usage usually looks like this:
+
+    .. code-block::
+
+        @extend_schema(
+            request=PolymorphicProxySerializer(
+                component_name='MetaPerson',
+                serializers=[
+                    LegalPersonSerializer, NaturalPersonSerializer,
+                ],
+                resource_type_field_name='person_type',
+            )
+        )
+        def create(self, request, *args, **kwargs):
+            return Response(...)
 
     Beware that this is not a real serializer and therefore is not derived from
     serializers.Serializer. It *cannot* be used in views as `serializer_class`
     or as field in a actual serializer. You likely want to handle this in the
     view method.
 
     Also make sure that each sub-serializer has a field named after the value of
-    `resource_type_field` (discriminator field) for the the mapping and parity
-    with with the generated schema.
-    """
+    ``resource_type_field_name`` (discriminator field). Generated clients will likely
+    depend on the existence of this field.
 
-    def __init__(self, component_name, serializers, resource_type_field_name):
+    For that reason, it is **strongly** recommended to pass the ``Serializers`` as **list**,
+    and by that let *drf-spectacular* retrieve the field and handle the mapping
+    automatically. In special circumstances, the field may not available when
+    drf-spectacular processes the serializer. In those cases you can explicitly state
+    the mapping with ``{'legal': LegalPersonSerializer, ...}``, but it is then your
+    responsibility to have a valid mapping.
+    """
+    def __init__(
+            self,
+            component_name: str,
+            serializers: Union[List[SerializerType], Dict[str, SerializerType]],
+            resource_type_field_name: str
+    ):
         self.component_name = component_name
         self.serializers = serializers
         self.resource_type_field_name = resource_type_field_name
 
 
 class OpenApiSchemaBase:
     pass
@@ -48,14 +77,15 @@
 def extend_schema(
         operation_id=None,
         parameters=None,
         request=None,
         responses=None,
         auth=None,
         description=None,
+        summary=None,
         deprecated=None,
         tags=None,
         exclude=False,
         operation=None,
         methods=None,
         versions=None,
 ):
@@ -75,14 +105,15 @@
         - ``dict`` with status codes as keys and `Serializers` as values.
         - :class:`.PolymorphicProxySerializer` for signaling that
           the operation may yield data from different serializers depending
           on the circumstances.
     :param request: replaces the discovered ``Serializer``.
     :param auth:
     :param description: replaces discovered doc strings
+    :param summary: an optional short summary of the description
     :param deprecated: mark operation as deprecated
     :param tags: override default list of tags
     :param exclude: set True to exclude operation from schema
     :param operation: manually override what auto-discovery would generate. you must
         provide a OpenAPI3-compliant dictionary that gets directly translated to YAML.
     :param methods: scope extend_schema to specific methods. matches all by default.
     :param versions: scope extend_schema to specific API version. matches all by default.
@@ -148,14 +179,19 @@
                 return super().get_response_serializers()
 
             def get_description(self):
                 if description and is_in_scope(self):
                     return description
                 return super().get_description()
 
+            def get_summary(self):
+                if summary and is_in_scope(self):
+                    return summary
+                return super().get_summary()
+
             def is_deprecated(self):
                 if deprecated and is_in_scope(self):
                     return deprecated
                 return super().is_deprecated()
 
             def get_tags(self):
                 if tags is not None and is_in_scope(self):
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular/validation/__init__.py` & `drf-spectacular-0.9.9/drf_spectacular/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/validation/openapi3_schema.json` & `drf-spectacular-0.9.9/drf_spectacular/validation/openapi3_schema.json`

 * *Files identical despite different names*

### Comparing `drf-spectacular-0.9.8/drf_spectacular/views.py` & `drf-spectacular-0.9.9/drf_spectacular/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from collections import namedtuple
-from typing import Dict, Any
+from typing import Any, Dict
 
 from rest_framework.renderers import TemplateHTMLRenderer
 from rest_framework.response import Response
 from rest_framework.reverse import reverse
 from rest_framework.views import APIView
 
 from drf_spectacular.renderers import (
-    OpenApiJsonRenderer, OpenApiJsonRenderer2,
-    OpenApiYamlRenderer, OpenApiYamlRenderer2
+    OpenApiJsonRenderer, OpenApiJsonRenderer2, OpenApiYamlRenderer, OpenApiYamlRenderer2,
 )
 from drf_spectacular.settings import spectacular_settings
 from drf_spectacular.types import OpenApiTypes
 from drf_spectacular.utils import extend_schema
 
 if spectacular_settings.SERVE_INCLUDE_SCHEMA:
     SCHEMA_KWARGS: Dict[str, Any] = {'responses': {200: OpenApiTypes.OBJECT}}
@@ -56,29 +55,31 @@
     renderer_classes = [OpenApiJsonRenderer, OpenApiJsonRenderer2]
 
 
 class SpectacularSwaggerView(APIView):
     renderer_classes = [TemplateHTMLRenderer]
     permission_classes = spectacular_settings.SERVE_PERMISSIONS
     url_name = 'schema'
+    url = None
     template_name = 'drf_spectacular/swagger_ui.html'
 
     @extend_schema(exclude=True)
     def get(self, request, *args, **kwargs):
         return Response(
-            {'url_name': reverse(self.url_name, request=request)},
+            {'schema_url': self.url or reverse(self.url_name, request=request)},
             template_name=self.template_name
         )
 
 
 class SpectacularRedocView(APIView):
     renderer_classes = [TemplateHTMLRenderer]
     permission_classes = spectacular_settings.SERVE_PERMISSIONS
     url_name = 'schema'
+    url = None
     template_name = 'drf_spectacular/redoc.html'
 
     @extend_schema(exclude=True)
     def get(self, request, *args, **kwargs):
         return Response(
-            {'url_name': reverse(self.url_name, request=request)},
+            {'schema_url': self.url or reverse(self.url_name, request=request)},
             template_name=self.template_name
         )
```

### Comparing `drf-spectacular-0.9.8/drf_spectacular.egg-info/PKG-INFO` & `drf-spectacular-0.9.9/drf_spectacular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-spectacular
-Version: 0.9.8
+Version: 0.9.9
 Summary: Sane and flexible OpenAPI 3 schema generation for Django REST framework
 Home-page: https://github.com/tfranzel/drf-spectacular
 Author: T. Franzel
 Author-email: tfranzel@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/tfranzel/drf-spectacular
 Project-URL: Documentation, https://drf-spectacular.readthedocs.io
@@ -218,15 +218,15 @@
            :target: https://pypi.python.org/pypi/drf-spectacular
         .. |codecov| image:: https://codecov.io/gh/tfranzel/drf-spectacular/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/tfranzel/drf-spectacular
         .. |docs| image:: https://readthedocs.org/projects/drf-spectacular/badge/
            :target: https://drf-spectacular.readthedocs.io/
         
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `drf-spectacular-0.9.8/setup.py` & `drf-spectacular-0.9.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import re
 import os
+import re
 import shutil
 import sys
-from setuptools import setup
 
+from setuptools import setup
 
 name = 'drf-spectacular'
 package = 'drf_spectacular'
 description = 'Sane and flexible OpenAPI 3 schema generation for Django REST framework'
 url = 'https://github.com/tfranzel/drf-spectacular'
 author = 'T. Franzel'
 author_email = 'tfranzel@gmail.com'
@@ -31,17 +31,18 @@
                      init_py, re.MULTILINE).group(1)
 
 
 def get_packages(package):
     """
     Return root package and all sub-packages.
     """
-    return [dirpath
-            for dirpath, dirnames, filenames in os.walk(package)
-            if os.path.exists(os.path.join(dirpath, '__init__.py'))]
+    return [
+        dirpath for dirpath, dirnames, filenames in os.walk(package)
+        if os.path.exists(os.path.join(dirpath, '__init__.py'))
+    ]
 
 
 version = get_version(package)
 
 
 if sys.argv[-1] == 'publish':
     if os.system("pip freeze | grep twine"):
@@ -73,15 +74,15 @@
     author=author,
     author_email=author_email,
     packages=get_packages(package),
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=requirements,
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

