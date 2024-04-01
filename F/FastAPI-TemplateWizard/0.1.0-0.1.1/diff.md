# Comparing `tmp/FastAPI-TemplateWizard-0.1.0.tar.gz` & `tmp/FastAPI-TemplateWizard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastAPI-TemplateWizard-0.1.0.tar", last modified: Mon Apr  1 19:46:35 2024, max compression
+gzip compressed data, was "FastAPI-TemplateWizard-0.1.1.tar", last modified: Mon Apr  1 19:56:46 2024, max compression
```

## Comparing `FastAPI-TemplateWizard-0.1.0.tar` & `FastAPI-TemplateWizard-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 19:46:35.850749 FastAPI-TemplateWizard-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-01 19:46:35.848748 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/
--rw-rw-rw-   0        0        0      306 2024-04-01 19:46:35.000000 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-01 19:46:35.000000 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:46:35.000000 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-01 19:46:35.000000 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-01 19:46:35.000000 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:46:35.000000 FastAPI-TemplateWizard-0.1.0/FastAPI_TemplateWizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17098 2024-04-01 18:14:16.000000 FastAPI-TemplateWizard-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      306 2024-04-01 19:46:35.849748 FastAPI-TemplateWizard-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       74 2024-04-01 19:29:44.000000 FastAPI-TemplateWizard-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 19:46:35.850749 FastAPI-TemplateWizard-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-04-01 19:46:22.000000 FastAPI-TemplateWizard-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:56:46.662512 FastAPI-TemplateWizard-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-01 19:56:46.661511 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/
+-rw-rw-rw-   0        0        0      321 2024-04-01 19:56:46.000000 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-01 19:56:46.000000 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:56:46.000000 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-01 19:56:46.000000 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-01 19:56:46.000000 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:56:46.000000 FastAPI-TemplateWizard-0.1.1/FastAPI_TemplateWizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17098 2024-04-01 18:14:16.000000 FastAPI-TemplateWizard-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      321 2024-04-01 19:56:46.661511 FastAPI-TemplateWizard-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:56:46.662512 FastAPI-TemplateWizard-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2024-04-01 19:55:22.000000 FastAPI-TemplateWizard-0.1.1/setup.py
```

### Comparing `FastAPI-TemplateWizard-0.1.0/LICENSE` & `FastAPI-TemplateWizard-0.1.1/LICENSE`

 * *Files identical despite different names*

