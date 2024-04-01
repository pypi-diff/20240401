# Comparing `tmp/fast-templates-0.1.6.tar.gz` & `tmp/fast-templates-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-templates-0.1.6.tar", last modified: Mon Apr  1 20:46:29 2024, max compression
+gzip compressed data, was "fast-templates-0.1.7.tar", last modified: Mon Apr  1 21:10:05 2024, max compression
```

## Comparing `fast-templates-0.1.6.tar` & `fast-templates-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:46:29.594751 fast-templates-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-01 20:46:25.000000 fast-templates-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 20:46:29.594751 fast-templates-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 20:46:25.000000 fast-templates-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:46:29.594751 fast-templates-0.1.6/fast_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 20:46:29.000000 fast-templates-0.1.6/fast_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-01 20:46:29.000000 fast-templates-0.1.6/fast_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:46:29.000000 fast-templates-0.1.6/fast_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 20:46:29.000000 fast-templates-0.1.6/fast_templates.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 20:46:29.000000 fast-templates-0.1.6/fast_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 20:46:29.000000 fast-templates-0.1.6/fast_templates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:46:29.594751 fast-templates-0.1.6/fasttemplates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:46:25.000000 fast-templates-0.1.6/fasttemplates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-01 20:46:25.000000 fast-templates-0.1.6/fasttemplates/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-01 20:46:25.000000 fast-templates-0.1.6/fasttemplates/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 20:46:25.000000 fast-templates-0.1.6/fasttemplates/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:46:29.594751 fast-templates-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-01 20:46:25.000000 fast-templates-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.404669 fast-templates-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-01 21:10:01.000000 fast-templates-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 21:10:05.404669 fast-templates-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 21:10:01.000000 fast-templates-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.404669 fast-templates-0.1.7/fast_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 21:10:05.000000 fast-templates-0.1.7/fast_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 21:10:05.000000 fast-templates-0.1.7/fast_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:10:05.000000 fast-templates-0.1.7/fast_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 21:10:05.000000 fast-templates-0.1.7/fast_templates.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 21:10:05.000000 fast-templates-0.1.7/fast_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:10:05.000000 fast-templates-0.1.7/fast_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.396669 fast-templates-0.1.7/fasttemplates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/baselayout/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/db/mongo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/db/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/db/mongo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/routes/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/app/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/baselayout/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.396669 fast-templates-0.1.7/fasttemplates/templates/extras/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.396669 fast-templates-0.1.7/fasttemplates/templates/extras/cache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.396669 fast-templates-0.1.7/fasttemplates/templates/extras/cache/redis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.396669 fast-templates-0.1.7/fasttemplates/templates/extras/cache/redis/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/extras/cache/redis/app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/cache/redis/app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/cache/redis/app/utils/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/extras/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.400669 fast-templates-0.1.7/fasttemplates/templates/extras/db/mongo/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/db/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/db/mongo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:05.404669 fast-templates-0.1.7/fasttemplates/templates/extras/db/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/db/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/templates/extras/db/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 21:10:01.000000 fast-templates-0.1.7/fasttemplates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:10:05.404669 fast-templates-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-01 21:10:01.000000 fast-templates-0.1.7/setup.py
```

### Comparing `fast-templates-0.1.6/LICENSE` & `fast-templates-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.6/PKG-INFO` & `fast-templates-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-templates
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI to generate FastAPI templates
 Home-page: https://github.com/pybalt/FastAPI-TemplateWizard
 Author: pybalt
 Author-email: 96897286+pybalt@users.noreply.github.com
 License-File: LICENSE
 Requires-Dist: typer
 Requires-Dist: questionary
```

### Comparing `fast-templates-0.1.6/fast_templates.egg-info/PKG-INFO` & `fast-templates-0.1.7/fast_templates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-templates
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI to generate FastAPI templates
 Home-page: https://github.com/pybalt/FastAPI-TemplateWizard
 Author: pybalt
 Author-email: 96897286+pybalt@users.noreply.github.com
 License-File: LICENSE
 Requires-Dist: typer
 Requires-Dist: questionary
```

### Comparing `fast-templates-0.1.6/fasttemplates/constants.py` & `fast-templates-0.1.7/fasttemplates/constants.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.6/fasttemplates/main.py` & `fast-templates-0.1.7/fasttemplates/main.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.6/fasttemplates/utils.py` & `fast-templates-0.1.7/fasttemplates/utils.py`

 * *Files identical despite different names*

### Comparing `fast-templates-0.1.6/setup.py` & `fast-templates-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='fast-templates',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
+    package_data={'': ['**/*']},
     url='https://github.com/pybalt/FastAPI-TemplateWizard',
     author='pybalt',
     author_email='96897286+pybalt@users.noreply.github.com',
     description='A CLI to generate FastAPI templates',
     long_description=long_description,
     install_requires=[
         'typer',
```

