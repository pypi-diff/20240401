# Comparing `tmp/xia-module-0.0.8.tar.gz` & `tmp/xia-module-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-0.0.8.tar", last modified: Sun Mar 31 05:40:34 2024, max compression
+gzip compressed data, was "xia-module-0.0.9.tar", last modified: Sun Mar 31 06:03:11 2024, max compression
```

## Comparing `xia-module-0.0.8.tar` & `xia-module-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 05:40:24.000000 xia-module-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-31 05:40:34.000000 xia-module-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-31 05:40:34.435383 xia-module-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 05:40:24.000000 xia-module-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 05:40:34.435383 xia-module-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 05:40:24.000000 xia-module-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/xia_module/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/xia_module/cicd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/cicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/cicd/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/xia_module/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/xia_module/templates/gcp-module/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/templates/gcp-module/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/xia_module/templates/module/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/templates/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-31 05:40:24.000000 xia-module-0.0.8/xia_module/templates/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:40:34.435383 xia-module-0.0.8/xia_module.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-31 05:40:34.000000 xia-module-0.0.8/xia_module.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-31 05:40:34.000000 xia-module-0.0.8/xia_module.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 05:40:34.000000 xia-module-0.0.8/xia_module.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-31 05:40:34.000000 xia-module-0.0.8/xia_module.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 05:40:34.000000 xia-module-0.0.8/xia_module.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.600995 xia-module-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 06:02:43.000000 xia-module-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-31 06:03:11.000000 xia-module-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-31 06:03:11.600995 xia-module-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 06:02:43.000000 xia-module-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 06:03:11.600995 xia-module-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 06:02:43.000000 xia-module-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.600995 xia-module-0.0.9/xia_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.600995 xia-module-0.0.9/xia_module/cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/cicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/cicd/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.596995 xia-module-0.0.9/xia_module/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.600995 xia-module-0.0.9/xia_module/templates/gcp-module/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/templates/gcp-module/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.600995 xia-module-0.0.9/xia_module/templates/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/templates/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-31 06:02:43.000000 xia-module-0.0.9/xia_module/templates/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:03:11.600995 xia-module-0.0.9/xia_module.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-31 06:03:11.000000 xia-module-0.0.9/xia_module.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-31 06:03:11.000000 xia-module-0.0.9/xia_module.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 06:03:11.000000 xia-module-0.0.9/xia_module.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-31 06:03:11.000000 xia-module-0.0.9/xia_module.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 06:03:11.000000 xia-module-0.0.9/xia_module.egg-info/top_level.txt
```

### Comparing `xia-module-0.0.8/LICENSE` & `xia-module-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-0.0.8/setup.py` & `xia-module-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-0.0.8/xia_module/cicd/github.py` & `xia-module-0.0.9/xia_module/cicd/github.py`

 * *Files identical despite different names*

### Comparing `xia-module-0.0.8/xia_module/module.py` & `xia-module-0.0.9/xia_module/module.py`

 * *Files identical despite different names*

