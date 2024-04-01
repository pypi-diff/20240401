# Comparing `tmp/xia-module-pypi-0.0.2.tar.gz` & `tmp/xia-module-pypi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-pypi-0.0.2.tar", last modified: Sun Mar 31 07:28:13 2024, max compression
+gzip compressed data, was "xia-module-pypi-0.0.3.tar", last modified: Mon Apr  1 14:21:32 2024, max compression
```

## Comparing `xia-module-pypi-0.0.2.tar` & `xia-module-pypi-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 07:28:13.000000 xia-module-pypi-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 07:28:13.398490 xia-module-pypi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.390490 xia-module-pypi-0.0.2/xia_module_pypi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.390490 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/base/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.390490 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/cicd/github/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/cicd/github/deploy-gcp.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.390490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.390490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.390490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/template/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-31 07:28:04.000000 xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/template/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 07:28:13.394490 xia-module-pypi-0.0.2/xia_module_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-31 07:28:13.000000 xia-module-pypi-0.0.2/xia_module_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-31 07:28:13.000000 xia-module-pypi-0.0.2/xia_module_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 07:28:13.000000 xia-module-pypi-0.0.2/xia_module_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 07:28:13.000000 xia-module-pypi-0.0.2/xia_module_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 07:28:13.000000 xia-module-pypi-0.0.2/xia_module_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/template/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/top_level.txt
```

### Comparing `xia-module-pypi-0.0.2/LICENSE` & `xia-module-pypi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/setup.py` & `xia-module-pypi-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/pypi.py` & `xia-module-pypi-0.0.3/xia_module_pypi/pypi.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf` & `xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf` & `xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml` & `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/.gitignore` & `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/.gitignore`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/LICENSE` & `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi/templates/module-pypi/init/setup.py` & `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.2/xia_module_pypi.egg-info/SOURCES.txt` & `xia-module-pypi-0.0.3/xia_module_pypi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 xia_module_pypi.egg-info/dependency_links.txt
 xia_module_pypi.egg-info/requires.txt
 xia_module_pypi.egg-info/top_level.txt
 xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
 xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
 xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
 xia_module_pypi/templates/gcp-module-pypi/base/main.tf
-xia_module_pypi/templates/gcp-module-pypi/cicd/github/deploy-gcp.yml
+xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
+xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
 xia_module_pypi/templates/gcp-module-pypi/module/main.tf
 xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
 xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
 xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
 xia_module_pypi/templates/module-pypi/init/.gitignore
 xia_module_pypi/templates/module-pypi/init/LICENSE
 xia_module_pypi/templates/module-pypi/init/README.rst
```

