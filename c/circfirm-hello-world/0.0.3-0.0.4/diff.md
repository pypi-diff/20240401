# Comparing `tmp/circfirm-hello-world-0.0.3.tar.gz` & `tmp/circfirm-hello-world-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circfirm-hello-world-0.0.3.tar", last modified: Wed Mar 27 21:00:49 2024, max compression
+gzip compressed data, was "circfirm-hello-world-0.0.4.tar", last modified: Mon Apr  1 20:18:18 2024, max compression
```

## Comparing `circfirm-hello-world-0.0.3.tar` & `circfirm-hello-world-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.747295 circfirm-hello-world-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.747295 circfirm-hello-world-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 21:00:46.000000 circfirm-hello-world-0.0.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/VERSION.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/circfirm_hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/circfirm_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-27 21:00:49.000000 circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-27 21:00:49.000000 circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 21:00:49.000000 circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 21:00:49.000000 circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 21:00:49.000000 circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/requirements-base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:00:49.751295 circfirm-hello-world-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-27 21:00:40.000000 circfirm-hello-world-0.0.3/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.736260 circfirm-hello-world-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 20:18:15.000000 circfirm-hello-world-0.0.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/VERSION.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/circfirm_hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/circfirm_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 20:18:18.000000 circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 20:18:18.000000 circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:18:18.000000 circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 20:18:18.000000 circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 20:18:18.000000 circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/requirements-base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:18:18.736260 circfirm-hello-world-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:18:18.732260 circfirm-hello-world-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-01 20:18:11.000000 circfirm-hello-world-0.0.4/tests/test_plugin.py
```

### Comparing `circfirm-hello-world-0.0.3/.github/workflows/publish.yml` & `circfirm-hello-world-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/.github/workflows/push.yml` & `circfirm-hello-world-0.0.4/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/.gitignore` & `circfirm-hello-world-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/.pre-commit-config.yaml` & `circfirm-hello-world-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/LICENSE` & `circfirm-hello-world-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/LICENSES/MIT.txt` & `circfirm-hello-world-0.0.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/PKG-INFO` & `circfirm-hello-world-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circfirm-hello-world
-Version: 0.0.3
+Version: 0.0.4
 Summary: An example Hello World plugin for circfirm
 Author-email: Alec Delaney <tekktrik@gmail.com>
 License: MIT
 Keywords: TODO: Add keywords here
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/PKG-INFO` & `circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circfirm-hello-world
-Version: 0.0.3
+Version: 0.0.4
 Summary: An example Hello World plugin for circfirm
 Author-email: Alec Delaney <tekktrik@gmail.com>
 License: MIT
 Keywords: TODO: Add keywords here
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `circfirm-hello-world-0.0.3/circfirm_hello_world.egg-info/SOURCES.txt` & `circfirm-hello-world-0.0.4/circfirm_hello_world.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circfirm-hello-world-0.0.3/pyproject.toml` & `circfirm-hello-world-0.0.4/pyproject.toml`

 * *Files identical despite different names*

